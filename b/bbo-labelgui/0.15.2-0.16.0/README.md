# Comparing `tmp/bbo-labelgui-0.15.2.tar.gz` & `tmp/bbo-labelgui-0.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbo-labelgui-0.15.2.tar", last modified: Fri Apr 26 05:44:34 2024, max compression
+gzip compressed data, was "bbo-labelgui-0.16.0.tar", last modified: Fri May 31 10:22:31 2024, max compression
```

## Comparing `bbo-labelgui-0.15.2.tar` & `bbo-labelgui-0.16.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-04-26 05:44:34.437568 bbo-labelgui-0.15.2/
--rw-rw-r--   0 voit     (86501) voit     (86501)    25313 2023-11-13 15:37:28.000000 bbo-labelgui-0.15.2/LICENSE
--rw-rw-r--   0 voit     (86501) voit     (86501)     3569 2024-04-26 05:44:34.437568 bbo-labelgui-0.15.2/PKG-INFO
--rw-rw-r--   0 voit     (86501) voit     (86501)     2982 2023-11-13 15:37:28.000000 bbo-labelgui-0.15.2/README.md
-drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-04-26 05:44:34.433568 bbo-labelgui-0.15.2/bbo_labelgui.egg-info/
--rw-rw-r--   0 voit     (86501) voit     (86501)     3569 2024-04-26 05:44:34.000000 bbo-labelgui-0.15.2/bbo_labelgui.egg-info/PKG-INFO
--rw-rw-r--   0 voit     (86501) voit     (86501)      410 2024-04-26 05:44:34.000000 bbo-labelgui-0.15.2/bbo_labelgui.egg-info/SOURCES.txt
--rw-rw-r--   0 voit     (86501) voit     (86501)        1 2024-04-26 05:44:34.000000 bbo-labelgui-0.15.2/bbo_labelgui.egg-info/dependency_links.txt
--rw-rw-r--   0 voit     (86501) voit     (86501)       73 2024-04-26 05:44:34.000000 bbo-labelgui-0.15.2/bbo_labelgui.egg-info/requires.txt
--rw-rw-r--   0 voit     (86501) voit     (86501)        9 2024-04-26 05:44:34.000000 bbo-labelgui-0.15.2/bbo_labelgui.egg-info/top_level.txt
-drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-04-26 05:44:34.437568 bbo-labelgui-0.15.2/labelgui/
--rw-rw-r--   0 voit     (86501) voit     (86501)        0 2023-11-13 15:37:28.000000 bbo-labelgui-0.15.2/labelgui/__init__.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     3135 2023-11-23 08:02:58.000000 bbo-labelgui-0.15.2/labelgui/__main__.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     2036 2023-11-13 15:37:28.000000 bbo-labelgui-0.15.2/labelgui/check.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     1100 2023-11-13 15:37:28.000000 bbo-labelgui-0.15.2/labelgui/config.py
--rw-rw-r--   0 voit     (86501) voit     (86501)      652 2023-11-13 15:37:28.000000 bbo-labelgui-0.15.2/labelgui/helper_gui.py
--rw-rw-r--   0 voit     (86501) voit     (86501)      622 2023-11-13 15:37:28.000000 bbo-labelgui-0.15.2/labelgui/helper_video.py
--rwxrwxr-x   0 voit     (86501) voit     (86501)    67604 2024-04-26 05:44:22.000000 bbo-labelgui-0.15.2/labelgui/labeling_gui.py
--rwxrwxr-x   0 voit     (86501) voit     (86501)     2147 2023-11-13 15:37:28.000000 bbo-labelgui-0.15.2/labelgui/labeling_gui_cfg.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     4527 2023-11-23 11:12:37.000000 bbo-labelgui-0.15.2/labelgui/select_user.py
--rw-rw-r--   0 voit     (86501) voit     (86501)       38 2024-04-26 05:44:34.437568 bbo-labelgui-0.15.2/setup.cfg
--rw-rw-r--   0 voit     (86501) voit     (86501)     1073 2024-04-26 05:44:31.000000 bbo-labelgui-0.15.2/setup.py
+drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-05-31 10:22:31.535535 bbo-labelgui-0.16.0/
+-rw-rw-r--   0 voit     (86501) voit     (86501)    25313 2023-11-13 15:37:28.000000 bbo-labelgui-0.16.0/LICENSE
+-rw-rw-r--   0 voit     (86501) voit     (86501)     3569 2024-05-31 10:22:31.535535 bbo-labelgui-0.16.0/PKG-INFO
+-rw-rw-r--   0 voit     (86501) voit     (86501)     2982 2023-11-13 15:37:28.000000 bbo-labelgui-0.16.0/README.md
+drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-05-31 10:22:31.524534 bbo-labelgui-0.16.0/bbo_labelgui.egg-info/
+-rw-rw-r--   0 voit     (86501) voit     (86501)     3569 2024-05-31 10:22:31.000000 bbo-labelgui-0.16.0/bbo_labelgui.egg-info/PKG-INFO
+-rw-rw-r--   0 voit     (86501) voit     (86501)      410 2024-05-31 10:22:31.000000 bbo-labelgui-0.16.0/bbo_labelgui.egg-info/SOURCES.txt
+-rw-rw-r--   0 voit     (86501) voit     (86501)        1 2024-05-31 10:22:31.000000 bbo-labelgui-0.16.0/bbo_labelgui.egg-info/dependency_links.txt
+-rw-rw-r--   0 voit     (86501) voit     (86501)       73 2024-05-31 10:22:31.000000 bbo-labelgui-0.16.0/bbo_labelgui.egg-info/requires.txt
+-rw-rw-r--   0 voit     (86501) voit     (86501)        9 2024-05-31 10:22:31.000000 bbo-labelgui-0.16.0/bbo_labelgui.egg-info/top_level.txt
+drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2024-05-31 10:22:31.535535 bbo-labelgui-0.16.0/labelgui/
+-rw-rw-r--   0 voit     (86501) voit     (86501)        0 2023-11-13 15:37:28.000000 bbo-labelgui-0.16.0/labelgui/__init__.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     3135 2023-11-23 08:02:58.000000 bbo-labelgui-0.16.0/labelgui/__main__.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     2036 2023-11-13 15:37:28.000000 bbo-labelgui-0.16.0/labelgui/check.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     1100 2023-11-13 15:37:28.000000 bbo-labelgui-0.16.0/labelgui/config.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)      652 2023-11-13 15:37:28.000000 bbo-labelgui-0.16.0/labelgui/helper_gui.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)      622 2023-11-13 15:37:28.000000 bbo-labelgui-0.16.0/labelgui/helper_video.py
+-rwxrwxr-x   0 voit     (86501) voit     (86501)    67646 2024-05-31 08:58:34.000000 bbo-labelgui-0.16.0/labelgui/labeling_gui.py
+-rwxrwxr-x   0 voit     (86501) voit     (86501)     2147 2023-11-13 15:37:28.000000 bbo-labelgui-0.16.0/labelgui/labeling_gui_cfg.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     4527 2023-11-23 11:12:37.000000 bbo-labelgui-0.16.0/labelgui/select_user.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)       38 2024-05-31 10:22:31.535535 bbo-labelgui-0.16.0/setup.cfg
+-rw-rw-r--   0 voit     (86501) voit     (86501)     1073 2024-05-31 10:21:43.000000 bbo-labelgui-0.16.0/setup.py
```

### Comparing `bbo-labelgui-0.15.2/LICENSE` & `bbo-labelgui-0.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bbo-labelgui-0.15.2/PKG-INFO` & `bbo-labelgui-0.16.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbo-labelgui
-Version: 0.15.2
+Version: 0.16.0
 Summary: GUI for guided data labeling
 Home-page: https://github.com/bbo-lab/acm-traingui
 Author: BBO-lab @ caesar
 Author-email: kay-michael.voit@caesar.de
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bbo-labelgui-0.15.2/README.md` & `bbo-labelgui-0.16.0/README.md`

 * *Files identical despite different names*

### Comparing `bbo-labelgui-0.15.2/bbo_labelgui.egg-info/PKG-INFO` & `bbo-labelgui-0.16.0/bbo_labelgui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbo-labelgui
-Version: 0.15.2
+Version: 0.16.0
 Summary: GUI for guided data labeling
 Home-page: https://github.com/bbo-lab/acm-traingui
 Author: BBO-lab @ caesar
 Author-email: kay-michael.voit@caesar.de
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bbo-labelgui-0.15.2/labelgui/__main__.py` & `bbo-labelgui-0.16.0/labelgui/__main__.py`

 * *Files identical despite different names*

### Comparing `bbo-labelgui-0.15.2/labelgui/check.py` & `bbo-labelgui-0.16.0/labelgui/check.py`

 * *Files identical despite different names*

### Comparing `bbo-labelgui-0.15.2/labelgui/config.py` & `bbo-labelgui-0.16.0/labelgui/config.py`

 * *Files identical despite different names*

### Comparing `bbo-labelgui-0.15.2/labelgui/helper_gui.py` & `bbo-labelgui-0.16.0/labelgui/helper_gui.py`

 * *Files identical despite different names*

### Comparing `bbo-labelgui-0.15.2/labelgui/helper_video.py` & `bbo-labelgui-0.16.0/labelgui/helper_video.py`

 * *Files identical despite different names*

### Comparing `bbo-labelgui-0.15.2/labelgui/labeling_gui.py` & `bbo-labelgui-0.16.0/labelgui/labeling_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,14 +122,17 @@
         self.dy = int(128)
         self.vmin = int(0)
         self.vmax = int(127)
         self.dFrame = self.cfg['dFrame']
 
         self.minPose = int(self.cfg['minPose'])
         self.maxPose = int(self.cfg['maxPose'])
+
+        self.allowed_poses = np.arange(self.minPose, self.maxPose, self.dFrame, dtype=int)
+
         if 'allowed_cams' in self.cfg:
             self.allowed_cams = [int(i) for i in self.cfg['allowed_cams']]
         else:
             self.allowed_cams = list(range(len(self.cfg['standardRecordingFileNames'])))
         self.allowed_cams = sorted(self.allowed_cams)
 
         self.pose_idx = self.minPose
@@ -356,18 +359,17 @@
             self.colors = self.colors + sorted_names[i::24]
 
     def get_pose_idx(self):
         return self.pose_idx
 
     def set_pose_idx(self, pose_idx):
         pose_idx = int(pose_idx)
-        if pose_idx < self.minPose:
-            pose_idx = self.minPose
-        elif self.pose_idx > self.maxPose:
-            pose_idx = self.maxPose
+
+        pose_idx = self.allowed_poses[np.argmin(np.abs(self.allowed_poses - pose_idx))]
+        
         self.pose_idx = pose_idx
         self.plot2d_change_frame()
         if 'next' in self.controls['buttons']:
             self.controls['buttons']['next'].clearFocus()
 
     def combo_lists_cams_change(self, new_index):
         print(new_index, type(new_index))
@@ -482,15 +484,15 @@
         img = reader.get_data(self.pose_idx)
         if self.controls['plots']['image2d'] is None:
             self.controls['plots']['image2d'] = ax.imshow(img,
                                                           aspect=1,
                                                           cmap='gray',
                                                           vmin=self.vmin,
                                                           vmax=self.vmax)
-            print(f"img {self.pose_idx}: {hashlib.md5(img).hexdigest()}")
+#            print(f"img {self.pose_idx}: {hashlib.md5(img).hexdigest()}")
             ax.legend('',
                       facecolor=self.colors[i_cam % np.size(self.colors)],
                       loc='upper left',
                       bbox_to_anchor=(0, 1))
             ax.axis('off')
         else:
             self.controls['plots']['image2d'].set_array(img)
@@ -1590,8 +1592,8 @@
 
 
 if __name__ == '__main__':
     main(Path('o:/analysis/'))
 
 
 class UnsupportedFormatException(Exception):
-    pass
+    pass
```

### Comparing `bbo-labelgui-0.15.2/labelgui/labeling_gui_cfg.py` & `bbo-labelgui-0.16.0/labelgui/labeling_gui_cfg.py`

 * *Files identical despite different names*

### Comparing `bbo-labelgui-0.15.2/labelgui/select_user.py` & `bbo-labelgui-0.16.0/labelgui/select_user.py`

 * *Files identical despite different names*

### Comparing `bbo-labelgui-0.15.2/setup.py` & `bbo-labelgui-0.16.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="bbo-labelgui",
-    version="0.15.2",
+    version="0.16.0",
     description="GUI for guided data labeling",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/bbo-lab/acm-traingui",
     author="BBO-lab @ caesar",
     author_email="kay-michael.voit@caesar.de",
     license="BSD",
```

