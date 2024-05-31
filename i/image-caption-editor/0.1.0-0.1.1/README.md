# Comparing `tmp/image_caption_editor-0.1.0.tar.gz` & `tmp/image_caption_editor-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_caption_editor-0.1.0.tar", last modified: Tue May 21 21:25:18 2024, max compression
+gzip compressed data, was "image_caption_editor-0.1.1.tar", last modified: Fri May 31 19:23:02 2024, max compression
```

## Comparing `image_caption_editor-0.1.0.tar` & `image_caption_editor-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 21:25:18.279318 image_caption_editor-0.1.0/
--rw-rw-rw-   0        0        0        0 2024-05-21 11:55:01.000000 image_caption_editor-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      368 2024-05-21 21:25:18.278308 image_caption_editor-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-21 11:54:51.000000 image_caption_editor-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 21:25:18.276317 image_caption_editor-0.1.0/image_caption_editor.egg-info/
--rw-rw-rw-   0        0        0      368 2024-05-21 21:25:18.000000 image_caption_editor-0.1.0/image_caption_editor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-05-21 21:25:18.000000 image_caption_editor-0.1.0/image_caption_editor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 21:25:18.000000 image_caption_editor-0.1.0/image_caption_editor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-05-21 21:25:18.000000 image_caption_editor-0.1.0/image_caption_editor.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-05-21 21:25:18.000000 image_caption_editor-0.1.0/image_caption_editor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 21:25:18.000000 image_caption_editor-0.1.0/image_caption_editor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 21:25:18.279318 image_caption_editor-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      731 2024-05-21 12:28:19.000000 image_caption_editor-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 19:23:02.533373 image_caption_editor-0.1.1/
+-rw-rw-rw-   0        0        0     1033 2024-05-31 19:14:06.000000 image_caption_editor-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2197 2024-05-31 19:23:02.533373 image_caption_editor-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1827 2024-05-31 19:14:06.000000 image_caption_editor-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 19:23:02.513731 image_caption_editor-0.1.1/image_caption_editor/
+-rw-rw-rw-   0        0        0        0 2024-05-31 19:15:28.000000 image_caption_editor-0.1.1/image_caption_editor/__init__.py
+-rw-rw-rw-   0        0        0     2896 2024-05-31 19:14:06.000000 image_caption_editor-0.1.1/image_caption_editor/app.py
+-rw-rw-rw-   0        0        0      159 2024-05-31 19:14:06.000000 image_caption_editor-0.1.1/image_caption_editor/run.py
+drwxrwxrwx   0        0        0        0 2024-05-31 19:23:02.533373 image_caption_editor-0.1.1/image_caption_editor.egg-info/
+-rw-rw-rw-   0        0        0     2197 2024-05-31 19:23:02.000000 image_caption_editor-0.1.1/image_caption_editor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2024-05-31 19:23:02.000000 image_caption_editor-0.1.1/image_caption_editor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 19:23:02.000000 image_caption_editor-0.1.1/image_caption_editor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-05-31 19:23:02.000000 image_caption_editor-0.1.1/image_caption_editor.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-05-31 19:23:02.000000 image_caption_editor-0.1.1/image_caption_editor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-31 19:23:02.000000 image_caption_editor-0.1.1/image_caption_editor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 19:23:02.533373 image_caption_editor-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      695 2024-05-31 19:22:49.000000 image_caption_editor-0.1.1/setup.py
```

### Comparing `image_caption_editor-0.1.0/setup.py` & `image_caption_editor-0.1.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='image-caption-editor',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'streamlit',
         'pillow'
     ],
     entry_points={
@@ -15,9 +15,9 @@
         ],
     },
     author='Casa AI',
     author_email='siju@delvelabs.ai',
     description='An interactive tool for editing image captions using Streamlit.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    url='https://github.com/Capybara-AI/Image-Caption-Editor',  # Link to your project's GitHub repo
-)
+    url='https://github.com/Capybara-AI/Image-Caption-Editor',
+)
```

