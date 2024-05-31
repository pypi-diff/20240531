# Comparing `tmp/pywaybackup-1.0.1.tar.gz` & `tmp/pywaybackup-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywaybackup-1.0.1.tar", last modified: Mon Apr 22 07:11:05 2024, max compression
+gzip compressed data, was "pywaybackup-1.0.2.tar", last modified: Fri May 31 07:32:31 2024, max compression
```

## Comparing `pywaybackup-1.0.1.tar` & `pywaybackup-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 manjaro   (1000) manjaro   (1001)        0 2024-04-22 07:11:05.163612 pywaybackup-1.0.1/
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)     1065 2024-02-25 19:19:33.000000 pywaybackup-1.0.1/LICENSE
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)     5403 2024-04-22 07:11:05.163612 pywaybackup-1.0.1/PKG-INFO
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)     5050 2024-04-22 06:58:25.000000 pywaybackup-1.0.1/README.md
-drwxr-xr-x   0 manjaro   (1000) manjaro   (1001)        0 2024-04-22 07:11:05.160279 pywaybackup-1.0.1/pywaybackup/
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)     4606 2024-04-12 12:30:05.000000 pywaybackup-1.0.1/pywaybackup/SnapshotCollection.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)     1644 2024-04-12 12:30:31.000000 pywaybackup-1.0.1/pywaybackup/Verbosity.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)        0 2024-02-25 19:19:33.000000 pywaybackup-1.0.1/pywaybackup/__init__.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)       21 2024-04-22 07:09:48.000000 pywaybackup-1.0.1/pywaybackup/__version__.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)    12030 2024-04-22 06:58:25.000000 pywaybackup-1.0.1/pywaybackup/archive.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)     2473 2024-04-22 07:09:20.000000 pywaybackup-1.0.1/pywaybackup/arguments.py
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)      879 2024-04-22 07:09:12.000000 pywaybackup-1.0.1/pywaybackup/main.py
-drwxr-xr-x   0 manjaro   (1000) manjaro   (1001)        0 2024-04-22 07:11:05.163612 pywaybackup-1.0.1/pywaybackup.egg-info/
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)     5403 2024-04-22 07:11:05.000000 pywaybackup-1.0.1/pywaybackup.egg-info/PKG-INFO
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)      416 2024-04-22 07:11:05.000000 pywaybackup-1.0.1/pywaybackup.egg-info/SOURCES.txt
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)        1 2024-04-22 07:11:05.000000 pywaybackup-1.0.1/pywaybackup.egg-info/dependency_links.txt
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)       52 2024-04-22 07:11:05.000000 pywaybackup-1.0.1/pywaybackup.egg-info/entry_points.txt
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)       30 2024-04-22 07:11:05.000000 pywaybackup-1.0.1/pywaybackup.egg-info/requires.txt
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)       12 2024-04-22 07:11:05.000000 pywaybackup-1.0.1/pywaybackup.egg-info/top_level.txt
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)       38 2024-04-22 07:11:05.163612 pywaybackup-1.0.1/setup.cfg
--rw-r--r--   0 manjaro   (1000) manjaro   (1001)     1091 2024-02-26 09:18:12.000000 pywaybackup-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 07:32:31.507852 pywaybackup-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-02-25 19:19:33.000000 pywaybackup-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7564 2024-05-31 07:32:31.507852 pywaybackup-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7151 2024-05-31 07:30:41.000000 pywaybackup-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 07:32:31.507852 pywaybackup-1.0.2/pywaybackup/
+-rw-r--r--   0 root         (0) root         (0)     4890 2024-05-31 07:26:13.000000 pywaybackup-1.0.2/pywaybackup/SnapshotCollection.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2024-04-12 12:30:31.000000 pywaybackup-1.0.2/pywaybackup/Verbosity.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-25 19:19:33.000000 pywaybackup-1.0.2/pywaybackup/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-31 07:28:21.000000 pywaybackup-1.0.2/pywaybackup/__version__.py
+-rw-r--r--   0 root         (0) root         (0)    12576 2024-05-31 07:26:13.000000 pywaybackup-1.0.2/pywaybackup/archive.py
+-rw-r--r--   0 root         (0) root         (0)     2473 2024-04-22 07:09:20.000000 pywaybackup-1.0.2/pywaybackup/arguments.py
+-rw-r--r--   0 root         (0) root         (0)      879 2024-05-31 07:19:19.000000 pywaybackup-1.0.2/pywaybackup/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 07:32:31.507852 pywaybackup-1.0.2/pywaybackup.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7564 2024-05-31 07:32:31.000000 pywaybackup-1.0.2/pywaybackup.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      416 2024-05-31 07:32:31.000000 pywaybackup-1.0.2/pywaybackup.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 07:32:31.000000 pywaybackup-1.0.2/pywaybackup.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-31 07:32:31.000000 pywaybackup-1.0.2/pywaybackup.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-05-31 07:32:31.000000 pywaybackup-1.0.2/pywaybackup.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-31 07:32:31.000000 pywaybackup-1.0.2/pywaybackup.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 07:32:31.507852 pywaybackup-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1091 2024-02-26 09:18:12.000000 pywaybackup-1.0.2/setup.py
```

### Comparing `pywaybackup-1.0.1/LICENSE` & `pywaybackup-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pywaybackup-1.0.1/pywaybackup/SnapshotCollection.py` & `pywaybackup-1.0.2/pywaybackup/SnapshotCollection.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,19 +32,19 @@
     @classmethod
     def count_list(cls):
         return len(cls.SNAPSHOT_COLLECTION)
 
     @classmethod
     def create_collection(cls):
         new_collection = []
-        for cdx_entry in cls.SNAPSHOT_COLLECTION:
+        for idx, cdx_entry in enumerate(cls.SNAPSHOT_COLLECTION):
             timestamp, url = cdx_entry["timestamp"], cdx_entry["url"]
             url_archive = f"http://web.archive.org/web/{timestamp}{cls._url_get_filetype(url)}/{url}"
             collection_entry = {
-                "id": cls.SNAPSHOT_COLLECTION.index(cdx_entry),
+                "id": idx,
                 "timestamp": timestamp,
                 "url_archive": url_archive,
                 "url_origin": url,
                 "redirect_url": False,
                 "redirect_timestamp": False,
                 "response": False,
                 "file": False
@@ -61,15 +61,15 @@
         - collection_entry: A single snapshot entry of the collection (dict).
         - output: The output directory (str).
 
         Output:
         - download_file: The output path for the snapshot entry (str) with filename.
         """
         timestamp, url = collection_entry["timestamp"], collection_entry["url_origin"]
-        domain, subdir, filename = cls._url_split(url)
+        domain, subdir, filename = cls.url_split(url, index=True)
         if cls.MODE_CURRENT:
             download_dir = os.path.join(output, domain, subdir)
         else:
             download_dir = os.path.join(output, domain, timestamp, subdir)
         download_file = os.path.abspath(os.path.join(download_dir, filename))
         return download_file
 
@@ -105,16 +105,21 @@
             "css": "cs_"
             #"js": "js_"
         }
         urltype = urltype_mapping.get(file_extension, "id_")
         return urltype
 
     @classmethod
-    def _url_split(cls, url):
+    def url_split(cls, url, index=False):
         """
         Split a URL into domain, subdir and filename.
         """
+        if not urlparse(url).scheme:
+            url = "http://" + url
         parsed_url = urlparse(url)
-        domain = parsed_url.netloc
-        subdir = parsed_url.path.strip("/").rsplit("/", 1)[0]
-        filename = parsed_url.path.split("/")[-1] or "index.html"
+        domain = parsed_url.netloc.split("@")[-1].split(":")[0] # split mailto: and port
+        filename = parsed_url.path.split("/")[-1]
+        if index is True and filename == "":
+            filename = "index.html"
+        subdir = parsed_url.path.strip("/").replace(filename, "").strip("/")
+        filename = filename.replace("%20", " ") # replace url encoded spaces
         return domain, subdir, filename
```

### Comparing `pywaybackup-1.0.1/pywaybackup/Verbosity.py` & `pywaybackup-1.0.2/pywaybackup/Verbosity.py`

 * *Files identical despite different names*

### Comparing `pywaybackup-1.0.1/pywaybackup/archive.py` & `pywaybackup-1.0.2/pywaybackup/archive.py`

 * *Files 16% similar despite different names*

```diff
@@ -85,20 +85,33 @@
 
 # create filelist
 # timestamp format yyyyMMddhhmmss
 def query_list(url: str, range: int, start: int, end: int, explicit: bool, mode: str):
     try:
         v.write("\nQuerying snapshots...")
         query_range = ""
+        
         if not range:
             if start: query_range = query_range + f"&from={start}"
             if end: query_range = query_range + f"&to={end}"
         else: 
             query_range = "&from=" + str(datetime.now().year - range)
-        cdx_url = f"*.{url}/*" if not explicit else f"{url}"
+
+        # parse user input url and create according cdx url
+        domain, subdir, filename = sc.url_split(url)
+        if domain and not subdir and not filename:
+            cdx_url = f"*.{domain}/*" if not explicit else f"{domain}"
+        if domain and subdir and not filename:
+            cdx_url = f"{domain}/{subdir}/*"
+        if domain and subdir and filename:
+            cdx_url = f"{domain}/{subdir}/{filename}/*"
+        if domain and not subdir and filename:
+            cdx_url = f"{domain}/{filename}/*"
+
+        print(f"---> {cdx_url}")
         cdxQuery = f"https://web.archive.org/cdx/search/xd?output=json&url={cdx_url}{query_range}&fl=timestamp,digest,mimetype,statuscode,original&filter!=statuscode:200"
         cdxResult = requests.get(cdxQuery)
         sc.create_list(cdxResult, mode)
         v.write(f"\n-----> {sc.count_list()} snapshots found")
     except requests.exceptions.ConnectionError as e:
         v.write(f"\n-----> ERROR: could not query snapshots:\n{e}"); exit()
 
@@ -117,14 +130,15 @@
     v.write("\nDownloading snapshots...", progress=0)
     if workers > 1:
         v.write(f"\n-----> Simultaneous downloads: {workers}")
         batch_size = sc.count_list() // workers + 1
     else:
         batch_size = sc.count_list()
     sc.create_collection()
+    v.write("\n-----> Snapshots prepared")
     batch_list = [sc.SNAPSHOT_COLLECTION[i:i + batch_size] for i in range(0, len(sc.SNAPSHOT_COLLECTION), batch_size)]    
     threads = []
     worker = 0
     for batch in batch_list:
         worker += 1
         thread = threading.Thread(target=download_loop, args=(batch, output, workers, retry, no_redirect))
         threads.append(thread)
```

### Comparing `pywaybackup-1.0.1/pywaybackup/arguments.py` & `pywaybackup-1.0.2/pywaybackup/arguments.py`

 * *Files identical despite different names*

### Comparing `pywaybackup-1.0.1/pywaybackup/main.py` & `pywaybackup-1.0.2/pywaybackup/main.py`

 * *Files identical despite different names*

### Comparing `pywaybackup-1.0.1/setup.py` & `pywaybackup-1.0.2/setup.py`

 * *Files identical despite different names*

