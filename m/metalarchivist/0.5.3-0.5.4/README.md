# Comparing `tmp/metalarchivist-0.5.3.tar.gz` & `tmp/metalarchivist-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalarchivist-0.5.3.tar", last modified: Fri May 31 12:30:31 2024, max compression
+gzip compressed data, was "metalarchivist-0.5.4.tar", last modified: Fri May 31 12:46:14 2024, max compression
```

## Comparing `metalarchivist-0.5.3.tar` & `metalarchivist-0.5.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:30:31.536565 metalarchivist-0.5.3/
--rwxrwxrwx   0 root         (0) root         (0)      693 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      702 2024-05-31 12:30:31.536565 metalarchivist-0.5.3/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      113 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/README.md
--rwxrwxrwx   0 root         (0) root         (0)      677 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 12:30:31.536565 metalarchivist-0.5.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:30:31.528565 metalarchivist-0.5.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:30:31.529565 metalarchivist-0.5.3/src/metalarchivist/
--rwxrwxrwx   0 root         (0) root         (0)     3601 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:30:31.532565 metalarchivist-0.5.3/src/metalarchivist/export/
--rwxrwxrwx   0 root         (0) root         (0)      257 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/export/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3585 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/export/album.py
--rwxrwxrwx   0 root         (0) root         (0)     3679 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/export/band.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:30:31.532565 metalarchivist-0.5.3/src/metalarchivist/export/data/
--rw-rw-rw-   0 root         (0) root         (0)     1754 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/export/data/user-agents.json
--rw-rw-rw-   0 root         (0) root         (0)     2685 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/export/genre.py
--rw-rw-rw-   0 root         (0) root         (0)    10565 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/export/label.py
--rwxrwxrwx   0 root         (0) root         (0)     7272 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/export/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:30:31.534565 metalarchivist-0.5.3/src/metalarchivist/interface/
--rwxrwxrwx   0 root         (0) root         (0)     1437 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/interface/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     9508 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/interface/album.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:30:31.534565 metalarchivist-0.5.3/src/metalarchivist/interface/api/
--rw-rw-rw-   0 root         (0) root         (0)     3514 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/interface/api/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4929 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/interface/api/page.py
--rwxrwxrwx   0 root         (0) root         (0)     8477 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/interface/band.py
--rw-rw-rw-   0 root         (0) root         (0)     7975 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/interface/genre.py
--rw-rw-rw-   0 root         (0) root         (0)     8163 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/interface/label.py
--rwxrwxrwx   0 root         (0) root         (0)      380 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/interface/search.py
--rw-rw-rw-   0 root         (0) root         (0)     7235 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/interface/theme.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:30:31.536565 metalarchivist-0.5.3/src/metalarchivist.egg-info/
--rw-r--r--   0 root         (0) root         (0)      702 2024-05-31 12:30:31.000000 metalarchivist-0.5.3/src/metalarchivist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1001 2024-05-31 12:30:31.000000 metalarchivist-0.5.3/src/metalarchivist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 12:30:31.000000 metalarchivist-0.5.3/src/metalarchivist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-05-31 12:30:31.000000 metalarchivist-0.5.3/src/metalarchivist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-31 12:30:31.000000 metalarchivist-0.5.3/src/metalarchivist.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:30:31.535565 metalarchivist-0.5.3/src/test/
--rwxrwxrwx   0 root         (0) root         (0)    10359 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/test/test_albums.py
--rwxrwxrwx   0 root         (0) root         (0)     4073 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/test/test_bands.py
--rwxrwxrwx   0 root         (0) root         (0)     8506 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/test/test_genres.py
--rw-rw-rw-   0 root         (0) root         (0)     6166 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/test/test_labels.py
--rw-rw-rw-   0 root         (0) root         (0)     4108 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/test/test_themes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:46:14.707263 metalarchivist-0.5.4/
+-rwxrwxrwx   0 root         (0) root         (0)      693 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      702 2024-05-31 12:46:14.707263 metalarchivist-0.5.4/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      113 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      677 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 12:46:14.707263 metalarchivist-0.5.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:46:14.700263 metalarchivist-0.5.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:46:14.701263 metalarchivist-0.5.4/src/metalarchivist/
+-rwxrwxrwx   0 root         (0) root         (0)     3601 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:46:14.703263 metalarchivist-0.5.4/src/metalarchivist/export/
+-rwxrwxrwx   0 root         (0) root         (0)      257 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/export/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3585 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/export/album.py
+-rwxrwxrwx   0 root         (0) root         (0)     3679 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/export/band.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:46:14.703263 metalarchivist-0.5.4/src/metalarchivist/export/data/
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/export/data/user-agents.json
+-rw-rw-rw-   0 root         (0) root         (0)     2685 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/export/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)    10565 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/export/label.py
+-rwxrwxrwx   0 root         (0) root         (0)     7272 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/export/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:46:14.705263 metalarchivist-0.5.4/src/metalarchivist/interface/
+-rwxrwxrwx   0 root         (0) root         (0)     1437 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/interface/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9478 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/interface/album.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:46:14.705263 metalarchivist-0.5.4/src/metalarchivist/interface/api/
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/interface/api/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4929 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/interface/api/page.py
+-rwxrwxrwx   0 root         (0) root         (0)     8477 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/interface/band.py
+-rw-rw-rw-   0 root         (0) root         (0)     7975 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/interface/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)     8163 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/interface/label.py
+-rwxrwxrwx   0 root         (0) root         (0)      380 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/interface/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     7235 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/metalarchivist/interface/theme.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:46:14.707263 metalarchivist-0.5.4/src/metalarchivist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      702 2024-05-31 12:46:14.000000 metalarchivist-0.5.4/src/metalarchivist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1001 2024-05-31 12:46:14.000000 metalarchivist-0.5.4/src/metalarchivist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 12:46:14.000000 metalarchivist-0.5.4/src/metalarchivist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-31 12:46:14.000000 metalarchivist-0.5.4/src/metalarchivist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-31 12:46:14.000000 metalarchivist-0.5.4/src/metalarchivist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:46:14.706263 metalarchivist-0.5.4/src/test/
+-rwxrwxrwx   0 root         (0) root         (0)    10359 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/test/test_albums.py
+-rwxrwxrwx   0 root         (0) root         (0)     4073 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/test/test_bands.py
+-rwxrwxrwx   0 root         (0) root         (0)     8506 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/test/test_genres.py
+-rw-rw-rw-   0 root         (0) root         (0)     6166 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/test/test_labels.py
+-rw-rw-rw-   0 root         (0) root         (0)     4108 2024-05-31 12:46:00.000000 metalarchivist-0.5.4/src/test/test_themes.py
```

### Comparing `metalarchivist-0.5.3/LICENSE` & `metalarchivist-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.3/PKG-INFO` & `metalarchivist-0.5.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.5.3
+Version: 0.5.4
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `metalarchivist-0.5.3/pyproject.toml` & `metalarchivist-0.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "metalarchivist"
-version = "0.5.3"
+version = "0.5.4"
 authors = [ { name = "z3c0", email = "z3c0@21337.tech" } ]
 description = "A package for extracting data from metal-archives.com"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [ "rich", "lxml", "urllib3", "pycryptodome" ]
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `metalarchivist-0.5.3/src/metalarchivist/__init__.py` & `metalarchivist-0.5.4/src/metalarchivist/__init__.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.3/src/metalarchivist/export/album.py` & `metalarchivist-0.5.4/src/metalarchivist/export/album.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.3/src/metalarchivist/export/band.py` & `metalarchivist-0.5.4/src/metalarchivist/export/band.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.3/src/metalarchivist/export/data/user-agents.json` & `metalarchivist-0.5.4/src/metalarchivist/export/data/user-agents.json`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.3/src/metalarchivist/export/genre.py` & `metalarchivist-0.5.4/src/metalarchivist/export/genre.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.3/src/metalarchivist/export/label.py` & `metalarchivist-0.5.4/src/metalarchivist/export/label.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.3/src/metalarchivist/export/util.py` & `metalarchivist-0.5.4/src/metalarchivist/export/util.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.3/src/metalarchivist/interface/__init__.py` & `metalarchivist-0.5.4/src/metalarchivist/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.3/src/metalarchivist/interface/album.py` & `metalarchivist-0.5.4/src/metalarchivist/interface/album.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,24 +130,23 @@
     metallum_id: str = field(init=False)
     number: str = field(init=False)
     title: str = field(init=False)
     length: AlbumTrackLength | None = field(init=False)
     track_key: str = field(init=False)
 
     def __post_init__(self, tablerow: lxml.etree.ElementBase):
-        number, title, length, lyrics = tablerow.xpath('./td')
+        number, title, length, *_ = tablerow.xpath('./td')
 
         self.metallum_id = metallum_id = number.xpath('./a').pop().attrib['name']
-        self.title = title = title.text
+        self.title = title = title.text.strip()
 
         self.track_key = create_key(metallum_id, title)
 
         self.number = re.sub(r'\.$', '', number.xpath('./text()').pop())
         self.length = AlbumTrackLength(length.text) if length.text else None
-        self.lyrics = lyrics.text
 
 
 @dataclass
 class AlbumTrackLyrics:
     metallum_id: str
     html: InitVar[bytes]
```

### Comparing `metalarchivist-0.5.3/src/metalarchivist/interface/api/base.py` & `metalarchivist-0.5.4/src/metalarchivist/interface/api/base.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.3/src/metalarchivist/interface/api/page.py` & `metalarchivist-0.5.4/src/metalarchivist/interface/api/page.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.3/src/metalarchivist/interface/band.py` & `metalarchivist-0.5.4/src/metalarchivist/interface/band.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.3/src/metalarchivist/interface/genre.py` & `metalarchivist-0.5.4/src/metalarchivist/interface/genre.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.3/src/metalarchivist/interface/label.py` & `metalarchivist-0.5.4/src/metalarchivist/interface/label.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.3/src/metalarchivist/interface/theme.py` & `metalarchivist-0.5.4/src/metalarchivist/interface/theme.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.3/src/metalarchivist.egg-info/PKG-INFO` & `metalarchivist-0.5.4/src/metalarchivist.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.5.3
+Version: 0.5.4
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `metalarchivist-0.5.3/src/metalarchivist.egg-info/SOURCES.txt` & `metalarchivist-0.5.4/src/metalarchivist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.3/src/test/test_albums.py` & `metalarchivist-0.5.4/src/test/test_albums.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.3/src/test/test_bands.py` & `metalarchivist-0.5.4/src/test/test_bands.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.3/src/test/test_genres.py` & `metalarchivist-0.5.4/src/test/test_genres.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.3/src/test/test_labels.py` & `metalarchivist-0.5.4/src/test/test_labels.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.3/src/test/test_themes.py` & `metalarchivist-0.5.4/src/test/test_themes.py`

 * *Files identical despite different names*

