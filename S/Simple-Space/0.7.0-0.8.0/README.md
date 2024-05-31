# Comparing `tmp/simple_space-0.7.0.tar.gz` & `tmp/simple_space-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_space-0.7.0.tar", last modified: Thu May 30 22:02:32 2024, max compression
+gzip compressed data, was "simple_space-0.8.0.tar", last modified: Fri May 31 18:23:24 2024, max compression
```

## Comparing `simple_space-0.7.0.tar` & `simple_space-0.8.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 22:02:32.285267 simple_space-0.7.0/
--rw-rw-r--   0 user      (1000) user      (1000)     1062 2024-05-30 00:58:34.000000 simple_space-0.7.0/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)    11079 2024-05-30 22:02:32.285267 simple_space-0.7.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    10006 2024-05-30 19:17:31.000000 simple_space-0.7.0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 22:02:32.281267 simple_space-0.7.0/SimpleS/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 22:02:32.281267 simple_space-0.7.0/SimpleS/ImageRelated/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 07:48:36.000000 simple_space-0.7.0/SimpleS/ImageRelated/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     9526 2024-05-30 15:59:18.000000 simple_space-0.7.0/SimpleS/ImageRelated/basics.py
--rw-r--r--   0 user      (1000) user      (1000)     4603 2024-05-30 18:12:49.000000 simple_space-0.7.0/SimpleS/ImageRelated/enhancements.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 22:02:32.281267 simple_space-0.7.0/SimpleS/Points/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 07:48:29.000000 simple_space-0.7.0/SimpleS/Points/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     4748 2024-05-30 21:22:31.000000 simple_space-0.7.0/SimpleS/Points/dim2.py
--rw-rw-r--   0 user      (1000) user      (1000)     8666 2024-05-30 21:27:05.000000 simple_space-0.7.0/SimpleS/Points/dim3.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 22:02:16.000000 simple_space-0.7.0/SimpleS/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1394 2024-05-30 22:02:09.000000 simple_space-0.7.0/SimpleS/utils.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-30 22:02:32.285267 simple_space-0.7.0/Simple_Space.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)    11079 2024-05-30 22:02:32.000000 simple_space-0.7.0/Simple_Space.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      422 2024-05-30 22:02:32.000000 simple_space-0.7.0/Simple_Space.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-30 22:02:32.000000 simple_space-0.7.0/Simple_Space.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       57 2024-05-30 22:02:32.000000 simple_space-0.7.0/Simple_Space.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        8 2024-05-30 22:02:32.000000 simple_space-0.7.0/Simple_Space.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)     1082 2024-05-30 22:02:23.000000 simple_space-0.7.0/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-30 22:02:32.285267 simple_space-0.7.0/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-31 18:23:24.248083 simple_space-0.8.0/
+-rw-rw-r--   0 user      (1000) user      (1000)     1062 2024-05-30 00:58:34.000000 simple_space-0.8.0/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)    11079 2024-05-31 18:23:24.248083 simple_space-0.8.0/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    10006 2024-05-30 19:17:31.000000 simple_space-0.8.0/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-31 18:23:24.248083 simple_space-0.8.0/SimpleS/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-31 18:23:24.248083 simple_space-0.8.0/SimpleS/ImageRelated/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 07:48:36.000000 simple_space-0.8.0/SimpleS/ImageRelated/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9535 2024-05-31 18:18:31.000000 simple_space-0.8.0/SimpleS/ImageRelated/basics.py
+-rw-r--r--   0 user      (1000) user      (1000)     4794 2024-05-31 18:16:52.000000 simple_space-0.8.0/SimpleS/ImageRelated/enhancements.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-31 18:23:24.248083 simple_space-0.8.0/SimpleS/Points/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 07:48:29.000000 simple_space-0.8.0/SimpleS/Points/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4751 2024-05-31 18:21:41.000000 simple_space-0.8.0/SimpleS/Points/dim2.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8703 2024-05-31 18:21:04.000000 simple_space-0.8.0/SimpleS/Points/dim3.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 22:02:16.000000 simple_space-0.8.0/SimpleS/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1476 2024-05-31 18:22:46.000000 simple_space-0.8.0/SimpleS/utils.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-31 18:23:24.248083 simple_space-0.8.0/Simple_Space.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)    11079 2024-05-31 18:23:24.000000 simple_space-0.8.0/Simple_Space.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      422 2024-05-31 18:23:24.000000 simple_space-0.8.0/Simple_Space.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-31 18:23:24.000000 simple_space-0.8.0/Simple_Space.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       57 2024-05-31 18:23:24.000000 simple_space-0.8.0/Simple_Space.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        8 2024-05-31 18:23:24.000000 simple_space-0.8.0/Simple_Space.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     1082 2024-05-31 18:23:11.000000 simple_space-0.8.0/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-31 18:23:24.248083 simple_space-0.8.0/setup.cfg
```

### Comparing `simple_space-0.7.0/LICENSE` & `simple_space-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_space-0.7.0/PKG-INFO` & `simple_space-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simple-Space
-Version: 0.7.0
+Version: 0.8.0
 Summary: A Try at Better Understanding Space.
 Author-email: Hamed Hajipour <cloner174.org@gmail.com>
 Project-URL: Homepage, https://github.com/cloner174/Simple-Space
 Project-URL: Documentation, https://github.com/cloner174/Simple-Space#readme
 Project-URL: Repository, https://github.com/cloner174/Simple-Space.git
 Project-URL: Issues, https://github.com/cloner174/Simple-Space/issues
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `simple_space-0.7.0/README.md` & `simple_space-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `simple_space-0.7.0/SimpleS/ImageRelated/basics.py` & `simple_space-0.8.0/SimpleS/ImageRelated/basics.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,30 +67,30 @@
         path_to_save = save_path_generator(file_name,save_path,flag=None )
         plt.imsave(path_to_save, image, cmap=c_map)
     plt.imshow(image, cmap=c_map, interpolation=interpolation)
     
     plt.show()
 
 
-def fill_shape(image, points, color = (255, 0, 0)):
+def fill_shape_in_image(image, points, color = (255, 0, 0)):
     """
     Fill an area of a shape in an image based on the points defining the edges of the shape.
     Parameters:
     image (numpy.ndarray): The image where the shape is to be filled.
     points (list of tuples): A list of (x, y) tuples defining the vertices of the shape.
     color (tuple): A tuple defining the color to fill the shape. For grayscale, use one value; for color, use (B, G, R).
     Returns:
     numpy.ndarray: The modified image with the filled shape.
     """
     points_array = np.array(points, dtype=np.int32).reshape((-1, 1, 2))
     cv2.fillPoly(image, [points_array], color)
     return image
 
 
-def force_image_to_GRAYSCALE(image):
+def force_image_to_grayscale(image):
     holder = 0.2989
     keeper = 0.5870
     informer = 0.1140
     gray_image = holder * image[:, :, 0] + keeper * image[:, :, 1] + informer * image[:, :, 2]
     return gray_image
```

### Comparing `simple_space-0.7.0/SimpleS/ImageRelated/enhancements.py` & `simple_space-0.8.0/SimpleS/ImageRelated/enhancements.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,16 @@
         if isinstance(image, str):
             self.image_path = image
             self.src = None
         else:
             self.src = image
         self.dilatation_result = None
         self.erosion_result = None
+        self.path_to_erosion_result = None
+        self.path_to_dilatation_result = None
     
     def erosion(self):
         erosion_shape = self.erosion_shape
         erosion_size = self.erosion_size
         element = cv.getStructuringElement(self.morph_shape(erosion_shape), (2 * erosion_size + 1, 2 * erosion_size + 1),(erosion_size, erosion_size))
         erosion_dst = cv.erode(self.src, element)
         return erosion_dst
@@ -48,23 +50,26 @@
         plt.show()
     
     def save_result(self) :
         
         now = datetime.datetime.now()
         now = now.strftime('%Y%m%d-%H%M%S')
         if self.file_name is not None:
-            erofile_path = f"{self.save_path}/{self.file_name}_Erosion_{now}WITHsize{self.erosion_size}WITHshape{self.erosion_shape}.png"
-            dilafile_path = f"{self.save_path}/{self.file_name}_Dilatation{now}WITHsize{self.dilatation_size}WITHshape{self.dilation_shape}.png"
+            if
+            erofile_path = f"{self.save_path}/{self.file_name}_Erosion_{now}_SIZE{self.erosion_size}SHAPE{self.erosion_shape}.png"
+            dilafile_path = f"{self.save_path}/{self.file_name}_Dilatation{now}_SIZE{self.dilatation_size}SHAPE{self.dilation_shape}.png"
         else:
-            erofile_path = f"{self.save_path}/Erosion_{now}WITHsize{self.erosion_size}WITHshape{self.erosion_shape}.png"
-            dilafile_path = f"{self.save_path}/Dilatation_{now}WITHsize{self.dilatation_size}WITHshape{self.dilation_shape}.png"
+            erofile_path = f"{self.save_path}/Erosion_{now}_SIZE{self.erosion_size}SHAPE{self.erosion_shape}.png"
+            dilafile_path = f"{self.save_path}/Dilatation_{now}_SIZE{self.dilatation_size}SHAPE{self.dilation_shape}.png"
         if self.erosion_result is not None:
             plt.imsave(erofile_path, self.erosion_result)
+            self.path_to_erosion_result = erofile_path
         if self.dilatation_result is not None:
             plt.imsave(dilafile_path, self.dilatation_result)
+            self.path_to_dilatation_result = dilafile_path
 
         return
     
     def main(self,
                 eros = True, erosion_size=1, erosion_shape=0,#erosion_shape -> can be 0 or 1 or 2
                 dilate = True, dilatation_size=1, dilation_shape=0,#erosion_shape -> can be 0 or 1 or 2
                 show = True,
@@ -117,8 +122,8 @@
         if val == 0:
             return cv.MORPH_RECT
         elif val == 1:
             return cv.MORPH_CROSS
         elif val == 2:
             return cv.MORPH_ELLIPSE
     
-#end#
+#end#
```

### Comparing `simple_space-0.7.0/SimpleS/Points/dim2.py` & `simple_space-0.8.0/SimpleS/Points/dim2.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import scipy.ndimage as ndi
 from skimage import img_as_ubyte
 from skimage.morphology import skeletonize
 
 
 
 
-def rotate_points(points, theta=0, axis=None):
+def rotate_2d_points(points, theta=0, axis=None):
     """Rotate or reflect 2D points by theta degrees around the origin or inverting the specified axis."""
     points = np.asarray(points)
     if points.shape[1] != 2:
         raise ValueError("Points should be in shape (n, 2)")
     if axis == 'x':
         # invert the y-coordinates.
         rot_matrix = np.array([
```

### Comparing `simple_space-0.7.0/SimpleS/Points/dim3.py` & `simple_space-0.8.0/SimpleS/Points/dim3.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
                 faces = np.asarray(faces)
                 print("Secssesful . Faces")
         
         return vertices, faces
     
     
 
-def rotate_points(points, theta, axis='z'):
+def rotate_3d_points(points, theta, axis='z'):
         """Rotate 3D points around the specified axis by theta degrees."""
         theta = np.radians(theta)
         if axis == 'x':
                 rot_matrix = np.array([
                         [1, 0, 0],
                         [0, np.cos(theta), -np.sin(theta)],
                         [0, np.sin(theta), np.cos(theta)]
@@ -45,15 +45,15 @@
                         [0, 0, 1]
                 ])
         
         return np.dot(points, rot_matrix.T)
     
     
 
-def plot_points(v, f=None, axis = 'on', title = '3D Data Visualization', faces_colors = 'blue', alpha=0.75, linewidths=1, edgecolors='r', point_color='blue',show =True, save=False, save_path = None, file_name = None ):
+def plot_3d_points_using_vertices(v, f=None, axis = 'on', title = '3D Data Visualization', faces_colors = 'blue', alpha=0.75, linewidths=1, edgecolors='r', point_color='blue',show =True, save=False, save_path = None, file_name = None ):
         """
         Plot 3D points or a mesh from vertices and optionally faces.
         
         Parameters:
         - v: List of vertices where each vertex is a list or tuple [x, y, z].
         - f: Optional. List of faces, where each face is a list of indices of vertices forming that face.
         - axis: if 'on' shows the title for each axis -> 'X-axis' and 'Y-axis' and 'Z-axis'.
@@ -103,15 +103,15 @@
         else:
                 plt.clf()
                 plt.close()
                 return
     
     
 
-def create_bool_image_from_points(points, image_size=(500, 500),save = False, save_path = None, file_name = None):
+def create_bool_image_from_3d_points(points, image_size=(500, 500),save = False, save_path = None, file_name = None):
         """
         Create a grayscale image from 3D points by projecting them onto a 2D plane using the z-coordinate
         as intensity.
         Args:
         points (numpy.ndarray): An array of points with shape (N, 3), where each row represents a 3D point (x, y, z).
         image_size (tuple): The dimensions of the output image (width, height).
         
@@ -138,15 +138,15 @@
         if save:
                 path_to_save = save_path_generator(file_name,save_path, flag=None)
                 plt.imsave(path_to_save, image )
         return image
     
     
 
-def fill_points(image, iterations=5, structure=None, structure_like = (3,3) , save = False, save_path = None, file_name = None):
+def fill_inside_3d_points(image, iterations=5, structure=None, structure_like = (3,3) , save = False, save_path = None, file_name = None):
         """Fill in the gaps in a binary image using morphological dilation."""
         if structure is None:
                 structure = np.ones(structure_like)
         try:
                 filled_image = binary_dilation(image, structure=structure, iterations=iterations)
         except Exception as e:
                 try:
@@ -155,15 +155,15 @@
                         raise ValueError(f"{e}")
         if save:
                 save_path_generator(file_name, save_path, flag=None)
         return filled_image
     
     
 
-def plot_points(points, title = '3D Points Plot', labels = 'on', elev=None, azim=None,save = False,save_path=None, file_name = None):
+def plot_3d_points(points, title = '3D Points Plot', labels = 'on', elev=None, azim=None,save = False,save_path=None, file_name = None):
         """
         Plot and optionally save a 3D plot of points with specified view angles.
         Args:
         - points (array-like): A list or array of points where each point is a list or tuple of three floats (x, y, z).
         - save_path (str, optional): Path to save the plot image. If None, the plot will not be saved.
         - elev (float, optional): Elevation angle in the z plane for viewing. If None, the angle is not adjusted.
         - azim (float, optional): Azimuth angle in the x,y plane for viewing. If None, the angle is not adjusted.
```

### Comparing `simple_space-0.7.0/SimpleS/utils.py` & `simple_space-0.8.0/SimpleS/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,14 +11,16 @@
                                 path = 'results'
                 else:
                         path = 'results'
                 os.makedirs(path,exist_ok=True)
                 if filename is not None:
                         if not filename.endswith('.png') or not filename.endswith('.jpg'):
                                 filename = filename + '.png'
+                        else:
+                                filename = filename
                 else:
                         now = datetime.datetime.now()
                         now = now.strftime('%Y%m%d-%H%M%S')
                         filename = f'Fig{now}.png'
                 if flag is not None:
                         filename = str(flag) + filename
                 savepath = os.path.join(path,filename)
```

### Comparing `simple_space-0.7.0/Simple_Space.egg-info/PKG-INFO` & `simple_space-0.8.0/Simple_Space.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simple-Space
-Version: 0.7.0
+Version: 0.8.0
 Summary: A Try at Better Understanding Space.
 Author-email: Hamed Hajipour <cloner174.org@gmail.com>
 Project-URL: Homepage, https://github.com/cloner174/Simple-Space
 Project-URL: Documentation, https://github.com/cloner174/Simple-Space#readme
 Project-URL: Repository, https://github.com/cloner174/Simple-Space.git
 Project-URL: Issues, https://github.com/cloner174/Simple-Space/issues
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `simple_space-0.7.0/pyproject.toml` & `simple_space-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Simple-Space"
-version = "0.7.0"
+version = "0.8.0"
 description = "A Try at Better Understanding Space."
 readme = "README.md"
 requires-python = ">=3.6"
 authors = [
     { name = "Hamed Hajipour", email = "cloner174.org@gmail.com" },
 ]
 classifiers = [
```

