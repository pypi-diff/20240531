# Comparing `tmp/metalarchivist-0.5.2.tar.gz` & `tmp/metalarchivist-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalarchivist-0.5.2.tar", last modified: Fri May 31 11:49:06 2024, max compression
+gzip compressed data, was "metalarchivist-0.5.3.tar", last modified: Fri May 31 12:30:31 2024, max compression
```

## Comparing `metalarchivist-0.5.2.tar` & `metalarchivist-0.5.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 11:49:06.453067 metalarchivist-0.5.2/
--rwxrwxrwx   0 root         (0) root         (0)      693 2024-05-31 11:48:53.000000 metalarchivist-0.5.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      702 2024-05-31 11:49:06.453067 metalarchivist-0.5.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      113 2024-05-31 11:48:53.000000 metalarchivist-0.5.2/README.md
--rwxrwxrwx   0 root         (0) root         (0)      677 2024-05-31 11:48:53.000000 metalarchivist-0.5.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 11:49:06.453067 metalarchivist-0.5.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 11:49:06.446067 metalarchivist-0.5.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 11:49:06.447067 metalarchivist-0.5.2/src/metalarchivist/
--rwxrwxrwx   0 root         (0) root         (0)     3601 2024-05-31 11:48:53.000000 metalarchivist-0.5.2/src/metalarchivist/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 11:49:06.449066 metalarchivist-0.5.2/src/metalarchivist/export/
--rwxrwxrwx   0 root         (0) root         (0)      257 2024-05-31 11:48:53.000000 metalarchivist-0.5.2/src/metalarchivist/export/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4225 2024-05-31 11:48:53.000000 metalarchivist-0.5.2/src/metalarchivist/export/album.py
--rwxrwxrwx   0 root         (0) root         (0)     3679 2024-05-31 11:48:53.000000 metalarchivist-0.5.2/src/metalarchivist/export/band.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 11:49:06.449066 metalarchivist-0.5.2/src/metalarchivist/export/data/
--rw-rw-rw-   0 root         (0) root         (0)     1754 2024-05-31 11:48:53.000000 metalarchivist-0.5.2/src/metalarchivist/export/data/user-agents.json
--rw-rw-rw-   0 root         (0) root         (0)     2685 2024-05-31 11:48:53.000000 metalarchivist-0.5.2/src/metalarchivist/export/genre.py
--rw-rw-rw-   0 root         (0) root         (0)    10565 2024-05-31 11:48:53.000000 metalarchivist-0.5.2/src/metalarchivist/export/label.py
--rwxrwxrwx   0 root         (0) root         (0)     7075 2024-05-31 11:48:53.000000 metalarchivist-0.5.2/src/metalarchivist/export/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 11:49:06.451067 metalarchivist-0.5.2/src/metalarchivist/interface/
--rwxrwxrwx   0 root         (0) root         (0)     1378 2024-05-31 11:48:53.000000 metalarchivist-0.5.2/src/metalarchivist/interface/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     9103 2024-05-31 11:48:53.000000 metalarchivist-0.5.2/src/metalarchivist/interface/album.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 11:49:06.451067 metalarchivist-0.5.2/src/metalarchivist/interface/api/
--rw-rw-rw-   0 root         (0) root         (0)     3514 2024-05-31 11:48:53.000000 metalarchivist-0.5.2/src/metalarchivist/interface/api/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4929 2024-05-31 11:48:53.000000 metalarchivist-0.5.2/src/metalarchivist/interface/api/page.py
--rwxrwxrwx   0 root         (0) root         (0)     8477 2024-05-31 11:48:53.000000 metalarchivist-0.5.2/src/metalarchivist/interface/band.py
--rw-rw-rw-   0 root         (0) root         (0)     7975 2024-05-31 11:48:53.000000 metalarchivist-0.5.2/src/metalarchivist/interface/genre.py
--rw-rw-rw-   0 root         (0) root         (0)     8163 2024-05-31 11:48:53.000000 metalarchivist-0.5.2/src/metalarchivist/interface/label.py
--rwxrwxrwx   0 root         (0) root         (0)      380 2024-05-31 11:48:53.000000 metalarchivist-0.5.2/src/metalarchivist/interface/search.py
--rw-rw-rw-   0 root         (0) root         (0)     7235 2024-05-31 11:48:53.000000 metalarchivist-0.5.2/src/metalarchivist/interface/theme.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 11:49:06.452067 metalarchivist-0.5.2/src/metalarchivist.egg-info/
--rw-r--r--   0 root         (0) root         (0)      702 2024-05-31 11:49:06.000000 metalarchivist-0.5.2/src/metalarchivist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1001 2024-05-31 11:49:06.000000 metalarchivist-0.5.2/src/metalarchivist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 11:49:06.000000 metalarchivist-0.5.2/src/metalarchivist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-05-31 11:49:06.000000 metalarchivist-0.5.2/src/metalarchivist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-31 11:49:06.000000 metalarchivist-0.5.2/src/metalarchivist.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 11:49:06.452067 metalarchivist-0.5.2/src/test/
--rwxrwxrwx   0 root         (0) root         (0)    10767 2024-05-31 11:48:53.000000 metalarchivist-0.5.2/src/test/test_albums.py
--rwxrwxrwx   0 root         (0) root         (0)     4073 2024-05-31 11:48:53.000000 metalarchivist-0.5.2/src/test/test_bands.py
--rwxrwxrwx   0 root         (0) root         (0)     8506 2024-05-31 11:48:53.000000 metalarchivist-0.5.2/src/test/test_genres.py
--rw-rw-rw-   0 root         (0) root         (0)     6166 2024-05-31 11:48:53.000000 metalarchivist-0.5.2/src/test/test_labels.py
--rw-rw-rw-   0 root         (0) root         (0)     4108 2024-05-31 11:48:53.000000 metalarchivist-0.5.2/src/test/test_themes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:30:31.536565 metalarchivist-0.5.3/
+-rwxrwxrwx   0 root         (0) root         (0)      693 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      702 2024-05-31 12:30:31.536565 metalarchivist-0.5.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      113 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      677 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 12:30:31.536565 metalarchivist-0.5.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:30:31.528565 metalarchivist-0.5.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:30:31.529565 metalarchivist-0.5.3/src/metalarchivist/
+-rwxrwxrwx   0 root         (0) root         (0)     3601 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:30:31.532565 metalarchivist-0.5.3/src/metalarchivist/export/
+-rwxrwxrwx   0 root         (0) root         (0)      257 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/export/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3585 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/export/album.py
+-rwxrwxrwx   0 root         (0) root         (0)     3679 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/export/band.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:30:31.532565 metalarchivist-0.5.3/src/metalarchivist/export/data/
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/export/data/user-agents.json
+-rw-rw-rw-   0 root         (0) root         (0)     2685 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/export/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)    10565 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/export/label.py
+-rwxrwxrwx   0 root         (0) root         (0)     7272 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/export/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:30:31.534565 metalarchivist-0.5.3/src/metalarchivist/interface/
+-rwxrwxrwx   0 root         (0) root         (0)     1437 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/interface/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9508 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/interface/album.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:30:31.534565 metalarchivist-0.5.3/src/metalarchivist/interface/api/
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/interface/api/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4929 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/interface/api/page.py
+-rwxrwxrwx   0 root         (0) root         (0)     8477 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/interface/band.py
+-rw-rw-rw-   0 root         (0) root         (0)     7975 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/interface/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)     8163 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/interface/label.py
+-rwxrwxrwx   0 root         (0) root         (0)      380 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/interface/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     7235 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/metalarchivist/interface/theme.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:30:31.536565 metalarchivist-0.5.3/src/metalarchivist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      702 2024-05-31 12:30:31.000000 metalarchivist-0.5.3/src/metalarchivist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1001 2024-05-31 12:30:31.000000 metalarchivist-0.5.3/src/metalarchivist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 12:30:31.000000 metalarchivist-0.5.3/src/metalarchivist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-31 12:30:31.000000 metalarchivist-0.5.3/src/metalarchivist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-31 12:30:31.000000 metalarchivist-0.5.3/src/metalarchivist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 12:30:31.535565 metalarchivist-0.5.3/src/test/
+-rwxrwxrwx   0 root         (0) root         (0)    10359 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/test/test_albums.py
+-rwxrwxrwx   0 root         (0) root         (0)     4073 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/test/test_bands.py
+-rwxrwxrwx   0 root         (0) root         (0)     8506 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/test/test_genres.py
+-rw-rw-rw-   0 root         (0) root         (0)     6166 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/test/test_labels.py
+-rw-rw-rw-   0 root         (0) root         (0)     4108 2024-05-31 12:30:18.000000 metalarchivist-0.5.3/src/test/test_themes.py
```

### Comparing `metalarchivist-0.5.2/LICENSE` & `metalarchivist-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.2/PKG-INFO` & `metalarchivist-0.5.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.5.2
+Version: 0.5.3
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `metalarchivist-0.5.2/pyproject.toml` & `metalarchivist-0.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "metalarchivist"
-version = "0.5.2"
+version = "0.5.3"
 authors = [ { name = "z3c0", email = "z3c0@21337.tech" } ]
 description = "A package for extracting data from metal-archives.com"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [ "rich", "lxml", "urllib3", "pycryptodome" ]
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `metalarchivist-0.5.2/src/metalarchivist/__init__.py` & `metalarchivist-0.5.3/src/metalarchivist/__init__.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.2/src/metalarchivist/export/band.py` & `metalarchivist-0.5.3/src/metalarchivist/export/band.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.2/src/metalarchivist/export/data/user-agents.json` & `metalarchivist-0.5.3/src/metalarchivist/export/data/user-agents.json`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.2/src/metalarchivist/export/genre.py` & `metalarchivist-0.5.3/src/metalarchivist/export/genre.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.2/src/metalarchivist/export/label.py` & `metalarchivist-0.5.3/src/metalarchivist/export/label.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.2/src/metalarchivist/export/util.py` & `metalarchivist-0.5.3/src/metalarchivist/export/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,15 @@
     ROSTER_PAST_PAGE_SIZE = 1000
     LABEL_RELEASES_PAGE_SIZE = 2500
 
     ROOT = 'https://www.metal-archives.com'
     SEARCH = f'{ROOT}/search/advanced/searching/bands'
     
     BAND_LINKS = f'{ROOT}/link/ajax-list/type/band/id'
+    TRACK_LYRICS = f'{ROOT}/release/ajax-view-lyrics/id/'
     
     LABEL = f'{ROOT}/label/ajax-list/json/1/l/'
     LABEL_LINKS = f'{ROOT}/link/ajax-list/type/label/id/'
     ROSTER_CURRENT = f'{ROOT}/label/ajax-bands/nbrPerPage/{ROSTER_CURRENT_PAGE_SIZE}/id/'
     ROSTER_PAST = f'{ROOT}/label/ajax-bands-past/nbrPerPage/{ROSTER_PAST_PAGE_SIZE}/id/'
     LABEL_RELEASES = f'{ROOT}/label/ajax-albums/nbrPerPage/{LABEL_RELEASES_PAGE_SIZE}/id/'
 
@@ -188,14 +189,18 @@
         return os.path.join(cls.BAND_LINKS, str(metallum_id))
     
     @classmethod
     def label_links_query(cls, metallum_id: int) -> str:
         return os.path.join(cls.LABEL_LINKS, str(metallum_id))
     
     @classmethod
+    def track_lyrics_query(cls, metallum_id: str) -> str:
+        return os.path.join(cls.TRACK_LYRICS, metallum_id)
+    
+    @classmethod
     def roster_current_query(cls, metallum_id: int, echo=0, display_start=0, display_length=100) -> str:
         return (f'{os.path.join(cls.ROSTER_CURRENT, str(metallum_id))}'
                 f'?sEcho={echo}&iDisplayStart={display_start}&iDisplayLength={display_length}')
     
     @classmethod
     def roster_past_query(cls, metallum_id: int, echo=0, display_start=0, display_length=100) -> str:
         return (f'{os.path.join(cls.ROSTER_PAST, str(metallum_id))}'
```

### Comparing `metalarchivist-0.5.2/src/metalarchivist/interface/__init__.py` & `metalarchivist-0.5.3/src/metalarchivist/interface/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 
 from .band import (BandProfile, BandLink, 
                    BandExternalLinks, BandGenre)
 
-from .album import AlbumProfile, AlbumLink, AlbumRelease
+from .album import (AlbumProfile, AlbumLink,
+                    AlbumRelease, AlbumTrackLyrics)
 
 from .genre import Subgenres, Genre
 
 from .theme import Themes
 
 from .label import (LabelProfile, LabelRosterMember, 
                     LabelExternalLinks, LabelContainer)
@@ -23,15 +24,15 @@
                        AlbumReleases, BandGenres,
                        LabelRosterMembers)
 
 
 __all__ = ['create_key',
     
            'BandProfile', 'BandLink', 'BandExternalLinks',
-           'AlbumProfile', 'AlbumLink', 
+           'AlbumProfile', 'AlbumLink', 'AlbumTrackLyrics',
            'LabelProfile', 'LabelExternalLinks', 'LabelContainer',
            'Subgenres', 'Genre', 'Themes', 'SearchResults',
            
            'ReleasePages', 'ReleasePage',
            'GenrePages', 'GenrePage',
            'LabelPages', 'LabelPage',
            'LabelRosterPages', 'LabelRosterPage',
```

### Comparing `metalarchivist-0.5.2/src/metalarchivist/interface/album.py` & `metalarchivist-0.5.3/src/metalarchivist/interface/album.py`

 * *Files 6% similar despite different names*

```diff
@@ -127,15 +127,14 @@
     """ A unique track on an album """
     tablerow: InitVar[lxml.etree.ElementBase]
 
     metallum_id: str = field(init=False)
     number: str = field(init=False)
     title: str = field(init=False)
     length: AlbumTrackLength | None = field(init=False)
-    lyrics: str = field(init=False)
     track_key: str = field(init=False)
 
     def __post_init__(self, tablerow: lxml.etree.ElementBase):
         number, title, length, lyrics = tablerow.xpath('./td')
 
         self.metallum_id = metallum_id = number.xpath('./a').pop().attrib['name']
         self.title = title = title.text
@@ -144,14 +143,29 @@
 
         self.number = re.sub(r'\.$', '', number.xpath('./text()').pop())
         self.length = AlbumTrackLength(length.text) if length.text else None
         self.lyrics = lyrics.text
 
 
 @dataclass
+class AlbumTrackLyrics:
+    metallum_id: str
+    html: InitVar[bytes]
+
+    text: str = field(init=False)
+
+    def __post_init__(self, lyrics_html: bytes):
+        wrapped_html = b'<div>' + lyrics_html + b'</div>'
+        lyrics_doc = lxml.html.fragment_fromstring(wrapped_html)
+        lyrics_text = lyrics_doc.xpath('./text()')
+        lyrics_text = list(map(str.strip, lyrics_text))
+        self.text = '\n'.join(lyrics_text)
+
+
+@dataclass
 class AlbumDescription:
     """ Additional information concerning an album """
     release_type: str | None
     release_date: str | None
     catalog_id: str | None
     label: str | None
     media_format: str | None
```

### Comparing `metalarchivist-0.5.2/src/metalarchivist/interface/api/base.py` & `metalarchivist-0.5.3/src/metalarchivist/interface/api/base.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.2/src/metalarchivist/interface/api/page.py` & `metalarchivist-0.5.3/src/metalarchivist/interface/api/page.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.2/src/metalarchivist/interface/band.py` & `metalarchivist-0.5.3/src/metalarchivist/interface/band.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.2/src/metalarchivist/interface/genre.py` & `metalarchivist-0.5.3/src/metalarchivist/interface/genre.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.2/src/metalarchivist/interface/label.py` & `metalarchivist-0.5.3/src/metalarchivist/interface/label.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.2/src/metalarchivist/interface/theme.py` & `metalarchivist-0.5.3/src/metalarchivist/interface/theme.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.2/src/metalarchivist.egg-info/PKG-INFO` & `metalarchivist-0.5.3/src/metalarchivist.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.5.2
+Version: 0.5.3
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `metalarchivist-0.5.2/src/metalarchivist.egg-info/SOURCES.txt` & `metalarchivist-0.5.3/src/metalarchivist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.2/src/test/test_albums.py` & `metalarchivist-0.5.3/src/test/test_albums.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,25 +252,19 @@
         album = self.export.Album.get_profile('https://www.metal-archives.com/albums/Kawir/%CE%9A%CF%85%CE%B4%CE%BF%CE%B9%CE%BC%CE%BF%CF%83/1216552')
         self.assertIsNotNone(album.name)
 
         album = self.export.Album.get_profile('https://www.metal-archives.com/albums/Aamonblut/Black_Candle_Majesty/1239703')
         self.assertIsNotNone(album.tracklist[0].number)
         self.assertEqual(album.tracklist[0].number, '1')
 
-    def test_album_profiles(self):
 
-        self.assertIn('Album', dir(self.export))
+    def test_track_lyrics(self):
+        track_lyrics = self.export.Album.get_track_lyrics('7299894')
+        self.assertIsNotNone(track_lyrics.text)
 
-        albums = self.export.Album.get_profiles(['https://www.metal-archives.com/albums/Urfaust/Untergang/1161736',
-                                                 'https://www.metal-archives.com/albums/Furia/Huta_Luna/1166382',
-                                                 'https://www.metal-archives.com/albums/Hades_Almighty/...Again_Shall_Be/91367'])
-        self.assertIsNotNone(albums)
-
-        album = albums[0]
-        self.assertEqual(album.name, 'Untergang')
 
     # def test_album_themes(self):
     #     metalarchivist = prepare_submodule(Submodule.MODULE)
     #     self.assertIsNotNone(metalarchivist)
 
     #     interface = prepare_submodule(Submodule.IFACE)
     #     self.assertIsNotNone(interface)
```

### Comparing `metalarchivist-0.5.2/src/test/test_bands.py` & `metalarchivist-0.5.3/src/test/test_bands.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.2/src/test/test_genres.py` & `metalarchivist-0.5.3/src/test/test_genres.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.2/src/test/test_labels.py` & `metalarchivist-0.5.3/src/test/test_labels.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.5.2/src/test/test_themes.py` & `metalarchivist-0.5.3/src/test/test_themes.py`

 * *Files identical despite different names*

