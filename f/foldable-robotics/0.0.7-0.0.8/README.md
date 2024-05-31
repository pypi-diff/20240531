# Comparing `tmp/foldable_robotics-0.0.7-py2.py3-none-any.whl.zip` & `tmp/foldable_robotics-0.0.8-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 10707 bytes, number of entries: 14
+Zip file size: 11057 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat      581 b- defN 16-Sep-22 21:31 foldable_robotics/class_algebra.py
 -rw-rw-rw-  2.0 fat     1383 b- defN 17-May-30 15:07 foldable_robotics/dynamics_info.py
 -rw-rw-rw-  2.0 fat      937 b- defN 17-May-25 19:55 foldable_robotics/geometry.py
 -rw-rw-rw-  2.0 fat      844 b- defN 17-May-25 19:55 foldable_robotics/iterable.py
--rw-rw-rw-  2.0 fat     5315 b- defN 17-May-30 15:07 foldable_robotics/laminate.py
--rw-rw-rw-  2.0 fat     9311 b- defN 17-May-25 19:55 foldable_robotics/layer.py
+-rw-rw-rw-  2.0 fat     5453 b- defN 17-May-31 18:33 foldable_robotics/laminate.py
+-rw-rw-rw-  2.0 fat    10700 b- defN 17-May-31 18:33 foldable_robotics/layer.py
 -rw-rw-rw-  2.0 fat     7015 b- defN 17-May-30 15:07 foldable_robotics/manufacturing.py
 -rw-rw-rw-  2.0 fat        0 b- defN 17-Mar-21 16:00 foldable_robotics/__init__.py
--rw-rw-rw-  2.0 fat       10 b- defN 17-May-31 16:58 foldable_robotics-0.0.7.dist-info/DESCRIPTION.rst
--rw-rw-rw-  2.0 fat      578 b- defN 17-May-31 16:58 foldable_robotics-0.0.7.dist-info/metadata.json
--rw-rw-rw-  2.0 fat       18 b- defN 17-May-31 16:58 foldable_robotics-0.0.7.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat      116 b- defN 17-May-31 16:58 foldable_robotics-0.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      403 b- defN 17-May-31 16:58 foldable_robotics-0.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat     1253 b- defN 17-May-31 16:58 foldable_robotics-0.0.7.dist-info/RECORD
-14 files, 27764 bytes uncompressed, 8605 bytes compressed:  69.0%
+-rw-rw-rw-  2.0 fat       10 b- defN 17-May-31 18:34 foldable_robotics-0.0.8.dist-info/DESCRIPTION.rst
+-rw-rw-rw-  2.0 fat      578 b- defN 17-May-31 18:34 foldable_robotics-0.0.8.dist-info/metadata.json
+-rw-rw-rw-  2.0 fat       18 b- defN 17-May-31 18:34 foldable_robotics-0.0.8.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat      116 b- defN 17-May-31 18:34 foldable_robotics-0.0.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      403 b- defN 17-May-31 18:34 foldable_robotics-0.0.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat     1254 b- defN 17-May-31 18:34 foldable_robotics-0.0.8.dist-info/RECORD
+14 files, 29292 bytes uncompressed, 8955 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: foldable_robotics/manufacturing.py
 Comment: 
 
 Filename: foldable_robotics/__init__.py
 Comment: 
 
-Filename: foldable_robotics-0.0.7.dist-info/DESCRIPTION.rst
+Filename: foldable_robotics-0.0.8.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: foldable_robotics-0.0.7.dist-info/metadata.json
+Filename: foldable_robotics-0.0.8.dist-info/metadata.json
 Comment: 
 
-Filename: foldable_robotics-0.0.7.dist-info/top_level.txt
+Filename: foldable_robotics-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: foldable_robotics-0.0.7.dist-info/WHEEL
+Filename: foldable_robotics-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: foldable_robotics-0.0.7.dist-info/METADATA
+Filename: foldable_robotics-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: foldable_robotics-0.0.7.dist-info/RECORD
+Filename: foldable_robotics-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## foldable_robotics/laminate.py

```diff
@@ -6,14 +6,15 @@
 """
 
 from .class_algebra import ClassAlgebra
 from . import geometry
 import matplotlib.pyplot as plt
 from .iterable import Iterable
 from .layer import Layer
+import numpy
 
 class WrongNumLayers(Exception):
     pass
 
 class Laminate(Iterable,ClassAlgebra):
     def __init__(self, *layers):
         self.layers = list(layers)
@@ -112,57 +113,59 @@
         import foldable_robotics.manufacturing
         return foldable_robotics.manufacturing.map_line_stretch(self,*args,**kwargs)
         
     def export_dxf(self,name):
         for ii,layer in enumerate(self.layers):
             layername = name+str(ii)
             layer.export_dxf(layername)
-    def mesh_items(self,thickness):
+    def mesh_items(self,material_properties):
         import matplotlib.cm as cm
         mi = []
 #        lines = []
         z = 0
-        for ii,(layer,t) in enumerate(zip(self,thickness)):
-            color1 = list(cm.plasma(ii/(len(self))))
-            mi.extend(layer.mesh_items(z,color1))
+        for ii,(layer,mp) in enumerate(zip(self,material_properties)):
+#            color1 = list(cm.plasma(ii/(len(self))))
+            mi.extend(layer.mesh_items(z,mp.color))
         #    color1[3] = .1
-            z+=t
+            z+=mp.thickness
         return mi
 
     def mass_properties(laminate,material_properties):
         volume = 0
         mass = 0
         z=0
         centroid_x=0
         centroid_y=0
         centroid_z=0
         for ii,layer in enumerate(laminate):
             bottom = z
-            top = z+material_properties.thickness[ii]
+            top = z+material_properties[ii].thickness
             area=0
     
-            mass_i=0
-            volume_i=0
-    
-            for geom in layer.geoms:
-                area+=geom.area
-                volume_ii = geom.area*material_properties.thickness[ii]
-                mass_ii  = volume_ii*material_properties.density[ii]
-    
-                volume_i+=volume_ii
-                mass_i+=mass_ii
-                centroid = list(geom.centroid.coords)[0]
-                centroid_x += centroid[0]*mass_ii
-                centroid_y += centroid[1]*mass_ii
-                centroid_z += (bottom+top)/2*mass_ii
-                
+            area_i,volume_i,mass_i,centroid_i = layer.mass_props(material_properties[ii],bottom,top)
+
+            centroid_x_i,centroid_y_i,centroid_z_i = centroid_i
+            area+=area_i
             volume+=volume_i
             mass+=mass_i
-    
+
+            centroid_x += centroid_x_i*mass_i
+            centroid_y += centroid_y_i*mass_i
+            centroid_z += centroid_z_i*mass_i
+
             z=top
         
         centroid_x /= mass
         centroid_y /= mass
         centroid_z /= mass
-        return mass,volume,(centroid_x,centroid_y,centroid_z)
+        centroid = (centroid_x,centroid_y,centroid_z)
+        
+        I=numpy.zeros((3,3))
+        bottom = 0
+        for ii,layer in enumerate(laminate):
+            cn = numpy.array(centroid)                
+            I+=layer.inertia(cn,bottom,material_properties[ii])
+            bottom += material_properties[ii].thickness
+            
+        return mass,volume,centroid,I
```

## foldable_robotics/layer.py

```diff
@@ -10,14 +10,15 @@
 import shapely.geometry
 import shapely.geometry as sg
 import shapely.affinity as sa
 from .class_algebra import ClassAlgebra
 import shapely.ops as so
 import shapely.wkt as sw
 import matplotlib.pyplot as plt
+import numpy
 
 def is_collection(item):
     collections = [
         shapely.geometry.MultiPolygon,
         shapely.geometry.GeometryCollection,
         shapely.geometry.MultiLineString,
         shapely.geometry.MultiPoint]
@@ -93,17 +94,20 @@
         interior2 = [pypoly2tri.shapes.Point(*item) for item in interior]
         cdt.AddHole(interior2)
     cdt.Triangulate()
     tris =cdt.GetTriangles()
     points = cdt.GetPoints()
     points2 = numpy.array([item.toTuple() for item in points])
     tris2 = numpy.array([[points.index(point) for point in tri.points_] for tri in tris],dtype = int)
-    z = points2[:,0:1]*0+z_offset
-    points3 = numpy.c_[points2,z]
-    return points3,tris2
+    return points2,tris2
+
+def points_2d_to_3d(points_2d,z_val):
+    z = points_2d[:,0:1]*0+z_val
+    points3 = numpy.c_[points_2d,z]
+    return points3
 
 def inertia_tensor(about_point,density,z_lower,z_upper,tris):
     import numpy
     z_lower = z_lower
     z_upper = z_upper
     from idealab_tools.geometry.triangle import Triangle
     tris3 = [Triangle(*tri) for tri in tris]
@@ -235,15 +239,16 @@
         import pyqtgraph.opengl as gl
 
         mi = []        
         
         for geom in self.geoms:
             if isinstance(geom,sg.Polygon):
                 
-                points3,tris2 = triangulate_geom(geom,z_offset)
+                points2,tris2 = triangulate_geom(geom,z_offset)
+                points3 = points_2d_to_3d(points2,z_offset)
                 verts =points3[tris2]
     #            verts2 =points3[tris2[:,::-1]]
                 
     #            vc =numpy.array([[1,0,0,1]]*len(points3))
     #            fc = [[1,0,0,1]]*len(tris2)
                 
                 verts_colors = [[color]*3]*len(tris2)
@@ -254,8 +259,47 @@
     #            for loop in [exterior]+interiors:
     #                loop = loop+loop[0:1]
     #                loop = numpy.array(loop)
     #                loop = numpy.c_[loop,loop[:,0]*0+ii]
     #                color = [1,1,1,1]
     #                pi =gl.GLLinePlotItem(pos = loop,color =color, width=10)
     #                lines.append(pi)        
-        return mi
+        return mi
+    def mass_props(self,material_property,bottom,top):
+        area_i = 0
+        mass_i=0
+        volume_i=0
+        
+        centroid_x_i=0
+        centroid_y_i=0
+        centroid_z_i=0
+
+        for geom in self.geoms:
+            area_i = geom.area
+            volume_ii = geom.area*material_property.thickness
+            mass_ii  = volume_ii*material_property.density
+
+            volume_i+=volume_ii
+            mass_i+=mass_ii
+            centroid = list(geom.centroid.coords)[0]
+            centroid_x_i += centroid[0]*mass_ii
+            centroid_y_i += centroid[1]*mass_ii
+            centroid_z_i += (bottom+top)/2*mass_ii
+
+        centroid_i = centroid_x_i/mass_ii,centroid_y_i/mass_ii,centroid_z_i/mass_ii
+        
+        return area_i,volume_i,mass_i,centroid_i 
+    
+    def inertia(self,about_point,z_lower,material_property):
+        I=numpy.zeros((3,3))
+        z_upper = z_lower+material_property.thickness
+
+        for geom in self.geoms:
+            points,tris = triangulate_geom(geom,z_lower)
+            tris = points[tris]
+            I+=inertia_tensor(about_point,material_property.density,z_lower,z_upper,tris)
+            
+        return I
+            
+            
+        
+
```

## Comparing `foldable_robotics-0.0.7.dist-info/metadata.json` & `foldable_robotics-0.0.8.dist-info/metadata.json`

 * *Files 19% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'version'": "'0.0.8'"}*

```diff
@@ -21,9 +21,9 @@
         }
     },
     "generator": "bdist_wheel (0.29.0)",
     "license": "MIT",
     "metadata_version": "2.0",
     "name": "foldable-robotics",
     "summary": "Foldable robotics is a package for designing and analyzing foldable laminate robots",
-    "version": "0.0.7"
+    "version": "0.0.8"
 }
```

