# Comparing `tmp/loopstructuralvisualisation-0.1.2.tar.gz` & `tmp/loopstructuralvisualisation-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loopstructuralvisualisation-0.1.2.tar", last modified: Tue May 28 23:47:00 2024, max compression
+gzip compressed data, was "loopstructuralvisualisation-0.1.3.tar", last modified: Fri May 31 00:38:56 2024, max compression
```

## Comparing `loopstructuralvisualisation-0.1.2.tar` & `loopstructuralvisualisation-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:47:00.276342 loopstructuralvisualisation-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-28 23:46:54.000000 loopstructuralvisualisation-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-28 23:47:00.276342 loopstructuralvisualisation-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-28 23:46:54.000000 loopstructuralvisualisation-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:47:00.272342 loopstructuralvisualisation-0.1.2/loopstructuralvisualisation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:46:54.000000 loopstructuralvisualisation-0.1.2/loopstructuralvisualisation/_2d_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7714 2024-05-28 23:46:54.000000 loopstructuralvisualisation-0.1.2/loopstructuralvisualisation/_3d_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-28 23:46:54.000000 loopstructuralvisualisation-0.1.2/loopstructuralvisualisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-28 23:46:54.000000 loopstructuralvisualisation-0.1.2/loopstructuralvisualisation/api.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 23:46:54.000000 loopstructuralvisualisation-0.1.2/loopstructuralvisualisation/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:47:00.272342 loopstructuralvisualisation-0.1.2/loopstructuralvisualisation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-28 23:47:00.000000 loopstructuralvisualisation-0.1.2/loopstructuralvisualisation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-28 23:47:00.000000 loopstructuralvisualisation-0.1.2/loopstructuralvisualisation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 23:47:00.000000 loopstructuralvisualisation-0.1.2/loopstructuralvisualisation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 23:47:00.000000 loopstructuralvisualisation-0.1.2/loopstructuralvisualisation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-28 23:47:00.000000 loopstructuralvisualisation-0.1.2/loopstructuralvisualisation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-28 23:46:54.000000 loopstructuralvisualisation-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 23:47:00.276342 loopstructuralvisualisation-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-28 23:46:54.000000 loopstructuralvisualisation-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:38:56.905890 loopstructuralvisualisation-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-31 00:38:50.000000 loopstructuralvisualisation-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-31 00:38:56.905890 loopstructuralvisualisation-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-31 00:38:50.000000 loopstructuralvisualisation-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:38:56.901890 loopstructuralvisualisation-0.1.3/loopstructuralvisualisation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 00:38:50.000000 loopstructuralvisualisation-0.1.3/loopstructuralvisualisation/_2d_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-05-31 00:38:50.000000 loopstructuralvisualisation-0.1.3/loopstructuralvisualisation/_3d_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-31 00:38:50.000000 loopstructuralvisualisation-0.1.3/loopstructuralvisualisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-31 00:38:50.000000 loopstructuralvisualisation-0.1.3/loopstructuralvisualisation/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 00:38:50.000000 loopstructuralvisualisation-0.1.3/loopstructuralvisualisation/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:38:56.905890 loopstructuralvisualisation-0.1.3/loopstructuralvisualisation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-31 00:38:56.000000 loopstructuralvisualisation-0.1.3/loopstructuralvisualisation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-31 00:38:56.000000 loopstructuralvisualisation-0.1.3/loopstructuralvisualisation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 00:38:56.000000 loopstructuralvisualisation-0.1.3/loopstructuralvisualisation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-31 00:38:56.000000 loopstructuralvisualisation-0.1.3/loopstructuralvisualisation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-31 00:38:56.000000 loopstructuralvisualisation-0.1.3/loopstructuralvisualisation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-05-31 00:38:50.000000 loopstructuralvisualisation-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 00:38:56.905890 loopstructuralvisualisation-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-31 00:38:50.000000 loopstructuralvisualisation-0.1.3/setup.py
```

### Comparing `loopstructuralvisualisation-0.1.2/LICENSE` & `loopstructuralvisualisation-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `loopstructuralvisualisation-0.1.2/PKG-INFO` & `loopstructuralvisualisation-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loopstructuralvisualisation
-Version: 0.1.2
+Version: 0.1.3
 Summary: 3D geological modelling
 Author-email: Lachlan Grose <lachlan.grose@monash.edu>
 License: MIT
 Project-URL: Documentation, https://Loop3d.org/LoopStructural/
 Project-URL: Bug Tracker, https://github.com/loop3d/loopstructural-visualisation/issues
 Project-URL: Source Code, https://github.com/loop3d/loopstructural-visualisation
 Keywords: earth sciences,geology,3-D modelling,structural geology,uncertainty
@@ -20,16 +20,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.18
-Requires-Dist: pyvista
+Requires-Dist: pyvista>=0.42
+Requires-Dist: LoopStructural
 Provides-Extra: jupyter
 Requires-Dist: pyvista[jupyter]; extra == "jupyter"
+Provides-Extra: all
+Requires-Dist: pyvista[all]; extra == "all"
 
 # loopstructural-visualisation
 
 A LoopStructural interface for pyvista's Plotter class. 
 
 
+To install `pip install loopstructuralvisualisation` or for a jupyter notebook environment (including the pyvista[jupyuter] dependencies) `pip install loopstructuralvisualisation[jupyter]`
+
```

### Comparing `loopstructuralvisualisation-0.1.2/loopstructuralvisualisation/_3d_viewer.py` & `loopstructuralvisualisation-0.1.3/loopstructuralvisualisation/_3d_viewer.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,14 +39,16 @@
         paint_with: Optional[BaseFeature] = None,
         colour: Optional[str] = "red",
         cmap: Optional[str] = None,
         opacity: Optional[float] = None,
         vmin: Optional[float] = None,
         vmax: Optional[float] = None,
         pyvista_kwargs: dict = {},
+        scalar_bar: bool = False,
+        slicer: bool = False,
     ):
         """Add an isosurface of a geological feature to the model
 
         Parameters
         ----------
         geological_feature : BaseFeature
             The geological feature to plot
@@ -65,89 +67,137 @@
         vmax : Optional[float], optional
             maximum value of the colourmap, by default None
         pyvista_kwargs : dict, optional
             other parameters passed to Plotter.add_mesh, by default {}
         """
 
         surfaces = geological_feature.surfaces(value)
-
+        meshes = []
         for surface in surfaces:
             s = surface.vtk
             if paint_with is not None:
                 clim = [paint_with.min(), paint_with.max()]
                 if vmin is not None:
                     clim[0] = vmin
                 if vmax is not None:
                     clim[1] = vmax
                 pyvista_kwargs["clim"] = clim
-                scalars = paint_with(surface.vertices)
+                pts = np.copy(surface.vertices)
+                if self.model is not None:
+                    pts = self.model.scale(pts)
+                scalars = paint_with(pts)
                 s["values"] = scalars
                 s.set_active_scalars("values")
                 colour = None
-            self.add_mesh(s, color=colour, cmap=cmap, opacity=opacity, **pyvista_kwargs)
+            meshes.append(s)
+        if slicer:
+            self.add_mesh_clip_plane(
+                pv.MultiBlock(meshes).combine(),
+                color=colour,
+                cmap=cmap,
+                opacity=opacity,
+                **pyvista_kwargs,
+            )
+        else:
+            self.add_mesh(
+                pv.MultiBlock(meshes).combine(),
+                color=colour,
+                cmap=cmap,
+                opacity=opacity,
+                **pyvista_kwargs,
+            )
+        if paint_with is not None and not scalar_bar:
+            self.remove_scalar_bar('values')
 
     def plot_scalar_field(
         self,
         geological_feature,
         cmap="viridis",
         vmin=None,
         vmax=None,
         opacity=None,
         pyvista_kwargs={},
+        scalar_bar: bool = False,
+        slicer=False,
     ):
         volume = geological_feature.scalar_field()
         if vmin is not None:
             pyvista_kwargs["clim"][0] = vmin
         if vmax is not None:
             pyvista_kwargs["clim"][1] = vmax
-        self.add_mesh(volume, cmap=cmap, opacity=opacity, **pyvista_kwargs)
+        if slicer:
+            self.add_mesh_clip_plane(volume, cmap=cmap, opacity=opacity, **pyvista_kwargs)
+        else:
+            self.add_mesh(volume, cmap=cmap, opacity=opacity, **pyvista_kwargs)
+        if not scalar_bar:
+            self.remove_scalar_bar(geological_feature.name)
 
-    def plot_block_model(self, cmap=None, model=None, pyvista_kwargs={}):
+    def plot_block_model(
+        self,
+        cmap=None,
+        model=None,
+        pyvista_kwargs={},
+        scalar_bar: bool = False,
+        slicer: bool = False,
+    ):
         model = self._check_model(model)
 
         block, codes = model.get_block_model()
-        self.add_mesh(block, cmap=cmap, **pyvista_kwargs)
+        if slicer:
+            self.add_mesh_clip_plane(block, cmap=cmap, **pyvista_kwargs)
+        else:
+            self.add_mesh(block, cmap=cmap, **pyvista_kwargs)
+        if not scalar_bar:
+            self.remove_scalar_bar('statigraphy')
 
     def plot_fault_displacements(
         self,
         fault_list=None,
         bounding_box=None,
         model=None,
         cmap="rainbow",
         pyvista_kwargs={},
+        scalar_bar: bool = False,
     ):
         if fault_list is None:
             model = self._check_model(model)
             fault_list = model.faults
         if bounding_box is None:
             model = self._check_model(model)
             bounding_box = model.bounding_box
         pts = bounding_box.regular_grid()
         displacement_value = np.zeros(pts.shape[0])
         for f in fault_list:
             disp = f.displacementfeature.evaluate_value(bounding_box.vtk.points)
             displacement_value[~np.isnan(disp)] += disp[~np.isnan(disp)]
-        self.add_mesh(bounding_box.vtk, scalars=displacement_value, cmap=cmap, **pyvista_kwargs)
+        volume = bounding_box.vtk
+        volume['displacement'] = displacement_value
+        self.add_mesh(volume, cmap=cmap, **pyvista_kwargs)
+        if not scalar_bar:
+            self.remove_scalar_bar('displacement')
 
     def plot_model_surfaces(
         self,
         strati=True,
         faults=True,
         cmap=None,
         model=None,
         fault_colour="black",
         paint_with=None,
         displacement_cmap=None,
         pyvista_kwargs={},
+        scalar_bar: bool = False,
     ):
         model = self._check_model(model)
         if strati:
             surfaces = model.get_stratigraphic_surfaces()
             for s in surfaces:
                 self.add_mesh(s.vtk, cmap=cmap, **pyvista_kwargs)
+                if not scalar_bar:
+                    self.remove_scalar_bar()
         if faults:
             faults = model.get_fault_surfaces()
             for f in faults:
                 self.add_mesh(f.vtk, colour=fault_colour, **pyvista_kwargs)
 
     def plot_vector_field(self, geological_feature, scale=1.0, pyvista_kwargs={}):
         vectorfield = geological_feature.vector_field()
```

### Comparing `loopstructuralvisualisation-0.1.2/loopstructuralvisualisation/api.py` & `loopstructuralvisualisation-0.1.3/loopstructuralvisualisation/api.py`

 * *Files identical despite different names*

### Comparing `loopstructuralvisualisation-0.1.2/loopstructuralvisualisation.egg-info/PKG-INFO` & `loopstructuralvisualisation-0.1.3/loopstructuralvisualisation.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loopstructuralvisualisation
-Version: 0.1.2
+Version: 0.1.3
 Summary: 3D geological modelling
 Author-email: Lachlan Grose <lachlan.grose@monash.edu>
 License: MIT
 Project-URL: Documentation, https://Loop3d.org/LoopStructural/
 Project-URL: Bug Tracker, https://github.com/loop3d/loopstructural-visualisation/issues
 Project-URL: Source Code, https://github.com/loop3d/loopstructural-visualisation
 Keywords: earth sciences,geology,3-D modelling,structural geology,uncertainty
@@ -20,16 +20,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.18
-Requires-Dist: pyvista
+Requires-Dist: pyvista>=0.42
+Requires-Dist: LoopStructural
 Provides-Extra: jupyter
 Requires-Dist: pyvista[jupyter]; extra == "jupyter"
+Provides-Extra: all
+Requires-Dist: pyvista[all]; extra == "all"
 
 # loopstructural-visualisation
 
 A LoopStructural interface for pyvista's Plotter class. 
 
 
+To install `pip install loopstructuralvisualisation` or for a jupyter notebook environment (including the pyvista[jupyuter] dependencies) `pip install loopstructuralvisualisation[jupyter]`
+
```

### Comparing `loopstructuralvisualisation-0.1.2/pyproject.toml` & `loopstructuralvisualisation-0.1.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -29,21 +29,22 @@
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3.12',
 ]
 dependencies = [
     "numpy>=1.18",
-    "pyvista",
+    "pyvista>=0.42",
+    "LoopStructural",
 ]
 dynamic = ['version']
 
 [project.optional-dependencies]
-jupyter = ['pyvista[jupyter]']
-
+jupyter = ['pyvista[jupyter]',]
+all = ['pyvista[all]']
 [project.urls]
 Documentation = 'https://Loop3d.org/LoopStructural/'
 "Bug Tracker" = 'https://github.com/loop3d/loopstructural-visualisation/issues'
 "Source Code" = 'https://github.com/loop3d/loopstructural-visualisation'
 
 [tool.setuptools.dynamic]
 version = { attr = 'loopstructuralvisualisation.version.__version__' }
```

