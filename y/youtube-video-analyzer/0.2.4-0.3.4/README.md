# Comparing `tmp/youtube_video_analyzer-0.2.4.tar.gz` & `tmp/youtube_video_analyzer-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtube_video_analyzer-0.2.4.tar", last modified: Sat May 18 12:52:36 2024, max compression
+gzip compressed data, was "youtube_video_analyzer-0.3.4.tar", last modified: Fri May 31 10:11:22 2024, max compression
```

## Comparing `youtube_video_analyzer-0.2.4.tar` & `youtube_video_analyzer-0.3.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-05-18 12:52:36.967248 youtube_video_analyzer-0.2.4/
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     2652 2024-05-18 12:52:36.966899 youtube_video_analyzer-0.2.4/PKG-INFO
--rw-r--r--   0 corneliusvincent   (501) staff       (20)       38 2024-05-18 12:52:36.967338 youtube_video_analyzer-0.2.4/setup.cfg
--rw-r--r--   0 corneliusvincent   (501) staff       (20)      959 2024-05-18 12:52:20.000000 youtube_video_analyzer-0.2.4/setup.py
-drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-05-18 12:52:36.965785 youtube_video_analyzer-0.2.4/youtube_video_analyzer/
--rw-r--r--   0 corneliusvincent   (501) staff       (20)      181 2024-05-18 07:54:47.000000 youtube_video_analyzer-0.2.4/youtube_video_analyzer/__init__.py
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     2286 2024-05-18 08:03:45.000000 youtube_video_analyzer-0.2.4/youtube_video_analyzer/frame_extract.py
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     1288 2024-05-18 08:02:32.000000 youtube_video_analyzer-0.2.4/youtube_video_analyzer/sound_extract.py
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     3605 2024-05-18 12:52:05.000000 youtube_video_analyzer-0.2.4/youtube_video_analyzer/sound_intervals.py
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     2125 2024-05-18 08:01:36.000000 youtube_video_analyzer-0.2.4/youtube_video_analyzer/video_downloader.py
-drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-05-18 12:52:36.966656 youtube_video_analyzer-0.2.4/youtube_video_analyzer.egg-info/
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     2652 2024-05-18 12:52:36.000000 youtube_video_analyzer-0.2.4/youtube_video_analyzer.egg-info/PKG-INFO
--rw-r--r--   0 corneliusvincent   (501) staff       (20)      437 2024-05-18 12:52:36.000000 youtube_video_analyzer-0.2.4/youtube_video_analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 corneliusvincent   (501) staff       (20)        1 2024-05-18 12:52:36.000000 youtube_video_analyzer-0.2.4/youtube_video_analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 corneliusvincent   (501) staff       (20)       37 2024-05-18 12:52:36.000000 youtube_video_analyzer-0.2.4/youtube_video_analyzer.egg-info/requires.txt
--rw-r--r--   0 corneliusvincent   (501) staff       (20)       23 2024-05-18 12:52:36.000000 youtube_video_analyzer-0.2.4/youtube_video_analyzer.egg-info/top_level.txt
+drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-05-31 10:11:22.393777 youtube_video_analyzer-0.3.4/
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     4288 2024-05-31 10:11:22.393540 youtube_video_analyzer-0.3.4/PKG-INFO
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)       38 2024-05-31 10:11:22.393832 youtube_video_analyzer-0.3.4/setup.cfg
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)      984 2024-05-31 10:07:58.000000 youtube_video_analyzer-0.3.4/setup.py
+drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-05-31 10:11:22.392260 youtube_video_analyzer-0.3.4/youtube_video_analyzer/
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)      223 2024-05-31 09:08:57.000000 youtube_video_analyzer-0.3.4/youtube_video_analyzer/__init__.py
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     1538 2024-05-31 10:07:17.000000 youtube_video_analyzer-0.3.4/youtube_video_analyzer/face_detection.py
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     2286 2024-05-18 08:03:45.000000 youtube_video_analyzer-0.3.4/youtube_video_analyzer/frame_extract.py
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     1288 2024-05-18 08:02:32.000000 youtube_video_analyzer-0.3.4/youtube_video_analyzer/sound_extract.py
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     3605 2024-05-18 12:52:05.000000 youtube_video_analyzer-0.3.4/youtube_video_analyzer/sound_intervals.py
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     2125 2024-05-18 08:01:36.000000 youtube_video_analyzer-0.3.4/youtube_video_analyzer/video_downloader.py
+drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-05-31 10:11:22.393238 youtube_video_analyzer-0.3.4/youtube_video_analyzer.egg-info/
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     4288 2024-05-31 10:11:22.000000 youtube_video_analyzer-0.3.4/youtube_video_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)      478 2024-05-31 10:11:22.000000 youtube_video_analyzer-0.3.4/youtube_video_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)        1 2024-05-31 10:11:22.000000 youtube_video_analyzer-0.3.4/youtube_video_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)       51 2024-05-31 10:11:22.000000 youtube_video_analyzer-0.3.4/youtube_video_analyzer.egg-info/requires.txt
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)       23 2024-05-31 10:11:22.000000 youtube_video_analyzer-0.3.4/youtube_video_analyzer.egg-info/top_level.txt
```

### Comparing `youtube_video_analyzer-0.2.4/setup.py` & `youtube_video_analyzer-0.3.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="youtube_video_analyzer",
-    version="0.2.4",
+    version="0.3.4",
     author="Cornelius Vincent",
     author_email="pro.cornelius@gmail.com",
     description="A package for downloading YouTube videos, extracting audio and frames, and analyzing sound intervals",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Cornelius-BobCat/package-video-downloader",
     packages=setuptools.find_packages(),
@@ -21,12 +21,13 @@
     python_requires=">=3.6",
     install_requires=[
         "pytube",
         "moviepy",
         "librosa",
         "imageio",
         "numpy",
+        "opencv-python",
     ],
 )
 
 # python setup.py sdist bdist_wheel
 # twine upload dist/*
```

### Comparing `youtube_video_analyzer-0.2.4/youtube_video_analyzer/frame_extract.py` & `youtube_video_analyzer-0.3.4/youtube_video_analyzer/frame_extract.py`

 * *Files identical despite different names*

### Comparing `youtube_video_analyzer-0.2.4/youtube_video_analyzer/sound_extract.py` & `youtube_video_analyzer-0.3.4/youtube_video_analyzer/sound_extract.py`

 * *Files identical despite different names*

### Comparing `youtube_video_analyzer-0.2.4/youtube_video_analyzer/sound_intervals.py` & `youtube_video_analyzer-0.3.4/youtube_video_analyzer/sound_intervals.py`

 * *Files identical despite different names*

### Comparing `youtube_video_analyzer-0.2.4/youtube_video_analyzer/video_downloader.py` & `youtube_video_analyzer-0.3.4/youtube_video_analyzer/video_downloader.py`

 * *Files identical despite different names*

