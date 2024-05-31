# Comparing `tmp/iitmbsvideosdownloader-1.4.5.tar.gz` & `tmp/iitmbsvideosdownloader-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iitmbsvideosdownloader-1.4.5.tar", last modified: Sat Jul 29 06:22:31 2023, max compression
+gzip compressed data, was "iitmbsvideosdownloader-2.1.4.tar", last modified: Sat Sep 23 23:27:17 2023, max compression
```

## Comparing `iitmbsvideosdownloader-1.4.5.tar` & `iitmbsvideosdownloader-2.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 savi      (1000) savi      (1000)        0 2023-07-29 06:22:31.234295 iitmbsvideosdownloader-1.4.5/
--rwxrwxrwx   0 savi      (1000) savi      (1000)     1081 2023-02-09 17:48:29.000000 iitmbsvideosdownloader-1.4.5/LICENSE.txt
--rwxrwxrwx   0 savi      (1000) savi      (1000)      228 2023-07-29 06:22:31.234295 iitmbsvideosdownloader-1.4.5/PKG-INFO
--rwxrwxrwx   0 savi      (1000) savi      (1000)     2315 2023-02-11 12:05:04.000000 iitmbsvideosdownloader-1.4.5/README.md
-drwxrwxrwx   0 savi      (1000) savi      (1000)        0 2023-07-29 06:22:30.531175 iitmbsvideosdownloader-1.4.5/iitmbsvideosdownloader/
--rwxrwxrwx   0 savi      (1000) savi      (1000)      318 2023-02-14 19:22:42.000000 iitmbsvideosdownloader-1.4.5/iitmbsvideosdownloader/SITES.py
--rwxrwxrwx   0 savi      (1000) savi      (1000)     3814 2023-02-11 11:11:49.000000 iitmbsvideosdownloader-1.4.5/iitmbsvideosdownloader/SUBJECTS.py
--rwxrwxrwx   0 savi      (1000) savi      (1000)        0 2023-02-08 09:47:19.000000 iitmbsvideosdownloader-1.4.5/iitmbsvideosdownloader/__init__.py
--rwxrwxrwx   0 savi      (1000) savi      (1000)     8373 2023-07-29 05:11:21.000000 iitmbsvideosdownloader-1.4.5/iitmbsvideosdownloader/_downloader.py
--rwxrwxrwx   0 savi      (1000) savi      (1000)     7356 2023-07-29 05:09:28.000000 iitmbsvideosdownloader-1.4.5/iitmbsvideosdownloader/_functions.py
--rwxrwxrwx   0 savi      (1000) savi      (1000)     6109 2023-07-29 04:36:21.000000 iitmbsvideosdownloader-1.4.5/iitmbsvideosdownloader/_iitm.py
--rwxrwxrwx   0 savi      (1000) savi      (1000)     4949 2023-07-29 06:18:24.000000 iitmbsvideosdownloader-1.4.5/iitmbsvideosdownloader/iitmbsvideosdownloader.py
-drwxrwxrwx   0 savi      (1000) savi      (1000)        0 2023-07-29 06:22:31.109297 iitmbsvideosdownloader-1.4.5/iitmbsvideosdownloader.egg-info/
--rwxrwxrwx   0 savi      (1000) savi      (1000)      228 2023-07-29 06:22:23.000000 iitmbsvideosdownloader-1.4.5/iitmbsvideosdownloader.egg-info/PKG-INFO
--rwxrwxrwx   0 savi      (1000) savi      (1000)      527 2023-07-29 06:22:24.000000 iitmbsvideosdownloader-1.4.5/iitmbsvideosdownloader.egg-info/SOURCES.txt
--rwxrwxrwx   0 savi      (1000) savi      (1000)        1 2023-07-29 06:22:23.000000 iitmbsvideosdownloader-1.4.5/iitmbsvideosdownloader.egg-info/dependency_links.txt
--rwxrwxrwx   0 savi      (1000) savi      (1000)       17 2023-07-29 06:22:23.000000 iitmbsvideosdownloader-1.4.5/iitmbsvideosdownloader.egg-info/requires.txt
--rwxrwxrwx   0 savi      (1000) savi      (1000)       23 2023-07-29 06:22:23.000000 iitmbsvideosdownloader-1.4.5/iitmbsvideosdownloader.egg-info/top_level.txt
--rwxrwxrwx   0 savi      (1000) savi      (1000)      107 2023-07-29 06:22:31.265512 iitmbsvideosdownloader-1.4.5/setup.cfg
--rwxrwxrwx   0 savi      (1000) savi      (1000)      439 2023-07-29 06:21:59.000000 iitmbsvideosdownloader-1.4.5/setup.py
+drwxrwxrwx   0 savi      (1000) savi      (1000)        0 2023-09-23 23:27:17.854971 iitmbsvideosdownloader-2.1.4/
+-rwxrwxrwx   0 savi      (1000) savi      (1000)     1081 2023-02-09 17:48:29.000000 iitmbsvideosdownloader-2.1.4/LICENSE.txt
+-rwxrwxrwx   0 savi      (1000) savi      (1000)      228 2023-09-23 23:27:17.854971 iitmbsvideosdownloader-2.1.4/PKG-INFO
+-rwxrwxrwx   0 savi      (1000) savi      (1000)     2315 2023-02-11 12:05:04.000000 iitmbsvideosdownloader-2.1.4/README.md
+drwxrwxrwx   0 savi      (1000) savi      (1000)        0 2023-09-23 23:27:17.119352 iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader/
+-rwxrwxrwx   0 savi      (1000) savi      (1000)      348 2023-09-23 21:43:15.000000 iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader/SITES.py
+-rwxrwxrwx   0 savi      (1000) savi      (1000)     3814 2023-02-11 11:11:49.000000 iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader/SUBJECTS.py
+-rwxrwxrwx   0 savi      (1000) savi      (1000)        0 2023-02-08 09:47:19.000000 iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader/__init__.py
+-rwxrwxrwx   0 savi      (1000) savi      (1000)     8370 2023-09-23 23:18:02.000000 iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader/_downloader.py
+-rwxrwxrwx   0 savi      (1000) savi      (1000)     7356 2023-07-29 05:09:28.000000 iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader/_functions.py
+-rwxrwxrwx   0 savi      (1000) savi      (1000)     6109 2023-07-29 04:36:21.000000 iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader/_iitm.py
+-rwxrwxrwx   0 savi      (1000) savi      (1000)     7281 2023-09-23 23:12:29.000000 iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader/iitmbsvideosdownloader.py
+drwxrwxrwx   0 savi      (1000) savi      (1000)        0 2023-09-23 23:27:17.713925 iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader.egg-info/
+-rwxrwxrwx   0 savi      (1000) savi      (1000)      228 2023-09-23 23:27:10.000000 iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader.egg-info/PKG-INFO
+-rwxrwxrwx   0 savi      (1000) savi      (1000)      527 2023-09-23 23:27:11.000000 iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader.egg-info/SOURCES.txt
+-rwxrwxrwx   0 savi      (1000) savi      (1000)        1 2023-09-23 23:27:10.000000 iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader.egg-info/dependency_links.txt
+-rwxrwxrwx   0 savi      (1000) savi      (1000)       72 2023-09-23 23:27:10.000000 iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader.egg-info/requires.txt
+-rwxrwxrwx   0 savi      (1000) savi      (1000)       23 2023-09-23 23:27:10.000000 iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader.egg-info/top_level.txt
+-rwxrwxrwx   0 savi      (1000) savi      (1000)      107 2023-09-23 23:27:17.886215 iitmbsvideosdownloader-2.1.4/setup.cfg
+-rwxrwxrwx   0 savi      (1000) savi      (1000)      500 2023-09-23 23:20:59.000000 iitmbsvideosdownloader-2.1.4/setup.py
```

### Comparing `iitmbsvideosdownloader-1.4.5/LICENSE.txt` & `iitmbsvideosdownloader-2.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iitmbsvideosdownloader-1.4.5/README.md` & `iitmbsvideosdownloader-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `iitmbsvideosdownloader-1.4.5/iitmbsvideosdownloader/SUBJECTS.py` & `iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader/SUBJECTS.py`

 * *Files identical despite different names*

### Comparing `iitmbsvideosdownloader-1.4.5/iitmbsvideosdownloader/_downloader.py` & `iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader/_downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from iitmbsvideosdownloader import SITES
 
 
 class Downloader:
     # downloads all files from y2mate
     def download_files(self, driver, video_links, yt_video_titles):
 
-        print(f"download_site is {self.DOWNLOAD_SITE.name}")
+        #print(f"download_site is {self.DOWNLOAD_SITE.name}")
 
         titles = list(video_links.keys())
         time.sleep(self.SLEEP_TIME)
         i = 0
         for video_id in video_links.values():
             self.download_file(driver, i, video_id, titles, yt_video_titles)
             time.sleep(self.SLEEP_TIME)
@@ -98,17 +98,16 @@
 
         downloadButton = driver.find_element(By.CLASS_NAME, "btn-file")
 
         time.sleep(self.SLEEP_TIME)
         downloadButton.click()
         self.log("Download Button from Popup Clicked, Downloading...", 3)
 
-        self.download_wait(self.DOWNLOAD_DIRECTORY)
-
         self.log("Download Assumed", 2)
+        self.download_wait(self.DOWNLOAD_DIRECTORY)
 
         if self.newest(self.DOWNLOAD_DIRECTORY) is None:
             self.log("Download failed, Retrying...", 2)
             self.download_file(driver, i, video_id, titles, yt_video_titles)
             return
 
         newest_file, extension = self.newest(self.DOWNLOAD_DIRECTORY)
@@ -183,17 +182,16 @@
 
         downloadButton = driver.find_element(By.CLASS_NAME, "btn-download-link")
 
         time.sleep(self.SLEEP_TIME)
         downloadButton.click()
         self.log("Download Button from Popup Clicked, Downloading...", 3)
 
-        self.download_wait(self.DOWNLOAD_DIRECTORY)
-
         self.log("Download Assumed", 2)
+        self.download_wait(self.DOWNLOAD_DIRECTORY)
 
         if self.newest(self.DOWNLOAD_DIRECTORY) is None:
             self.log("Download failed, Retrying...", 2)
             self.download_file(driver, i, video_id, titles, yt_video_titles)
             return
 
         newest_file, extension = self.newest(self.DOWNLOAD_DIRECTORY)
```

### Comparing `iitmbsvideosdownloader-1.4.5/iitmbsvideosdownloader/_functions.py` & `iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader/_functions.py`

 * *Files identical despite different names*

### Comparing `iitmbsvideosdownloader-1.4.5/iitmbsvideosdownloader/_iitm.py` & `iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader/_iitm.py`

 * *Files identical despite different names*

### Comparing `iitmbsvideosdownloader-1.4.5/iitmbsvideosdownloader.egg-info/SOURCES.txt` & `iitmbsvideosdownloader-2.1.4/iitmbsvideosdownloader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

