# Comparing `tmp/botasaurus_requests-4.0.5.tar.gz` & `tmp/botasaurus_requests-4.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botasaurus_requests-4.0.5.tar", last modified: Thu May 16 16:08:58 2024, max compression
+gzip compressed data, was "botasaurus_requests-4.0.7.tar", last modified: Fri May 17 05:57:44 2024, max compression
```

## Comparing `botasaurus_requests-4.0.5.tar` & `botasaurus_requests-4.0.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 16:08:58.065683 botasaurus_requests-4.0.5/
--rw-rw-rw-   0        0        0    11558 2024-05-16 05:34:38.000000 botasaurus_requests-4.0.5/LICENSE
--rw-rw-rw-   0        0        0       14 2024-05-16 05:34:38.000000 botasaurus_requests-4.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0    14770 2024-05-16 16:08:58.064833 botasaurus_requests-4.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      844 2024-05-16 16:06:45.000000 botasaurus_requests-4.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 16:08:58.008049 botasaurus_requests-4.0.5/botasaurus_requests/
--rw-rw-rw-   0        0        0      700 2024-05-16 11:45:50.000000 botasaurus_requests-4.0.5/botasaurus_requests/__init__.py
--rw-rw-rw-   0        0        0     4939 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.5/botasaurus_requests/__main__.py
--rw-rw-rw-   0        0        0       21 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.5/botasaurus_requests/__version__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 16:08:58.059888 botasaurus_requests-4.0.5/botasaurus_requests/bin/
--rw-rw-rw-   0        0        0        0 2024-05-16 05:45:16.000000 botasaurus_requests-4.0.5/botasaurus_requests/bin/__init__.py
--rw-rw-rw-   0        0        0     7338 2024-05-16 13:27:52.000000 botasaurus_requests-4.0.5/botasaurus_requests/cffi.py
--rw-rw-rw-   0        0        0    15963 2024-05-16 12:29:29.000000 botasaurus_requests-4.0.5/botasaurus_requests/client.py
--rw-rw-rw-   0        0        0    16718 2024-05-16 06:48:02.000000 botasaurus_requests-4.0.5/botasaurus_requests/cookies.py
--rw-rw-rw-   0        0        0      767 2024-05-16 06:02:03.000000 botasaurus_requests-4.0.5/botasaurus_requests/exceptions.py
--rw-rw-rw-   0        0        0     6026 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.5/botasaurus_requests/headers.py
--rw-rw-rw-   0        0        0    16753 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.5/botasaurus_requests/parser.py
--rw-rw-rw-   0        0        0    19318 2024-05-16 11:31:13.000000 botasaurus_requests-4.0.5/botasaurus_requests/reqs.py
--rw-rw-rw-   0        0        0     8395 2024-05-16 16:07:08.000000 botasaurus_requests-4.0.5/botasaurus_requests/request_class.py
--rw-rw-rw-   0        0        0       19 2024-05-16 12:29:29.000000 botasaurus_requests-4.0.5/botasaurus_requests/request_functions.py
--rw-rw-rw-   0        0        0     9871 2024-05-16 15:04:13.000000 botasaurus_requests-4.0.5/botasaurus_requests/response.py
--rw-rw-rw-   0        0        0    12167 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.5/botasaurus_requests/session.py
--rw-rw-rw-   0        0        0     4692 2024-05-16 05:45:16.000000 botasaurus_requests-4.0.5/botasaurus_requests/toolbelt.py
-drwxrwxrwx   0        0        0        0 2024-05-16 16:08:58.062134 botasaurus_requests-4.0.5/botasaurus_requests.egg-info/
--rw-rw-rw-   0        0        0    14770 2024-05-16 16:08:57.000000 botasaurus_requests-4.0.5/botasaurus_requests.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      797 2024-05-16 16:08:57.000000 botasaurus_requests-4.0.5/botasaurus_requests.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 16:08:57.000000 botasaurus_requests-4.0.5/botasaurus_requests.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-05-16 16:08:57.000000 botasaurus_requests-4.0.5/botasaurus_requests.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-16 16:08:57.000000 botasaurus_requests-4.0.5/botasaurus_requests.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1008 2024-05-16 16:08:55.000000 botasaurus_requests-4.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       81 2024-05-16 16:08:58.068862 botasaurus_requests-4.0.5/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-24 07:16:00.000000 botasaurus_requests-4.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 05:57:44.081890 botasaurus_requests-4.0.7/
+-rw-rw-rw-   0        0        0    11558 2024-05-16 05:34:38.000000 botasaurus_requests-4.0.7/LICENSE
+-rw-rw-rw-   0        0        0       14 2024-05-16 05:34:38.000000 botasaurus_requests-4.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0    14770 2024-05-17 05:57:44.081890 botasaurus_requests-4.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      844 2024-05-16 16:06:45.000000 botasaurus_requests-4.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 05:57:44.050440 botasaurus_requests-4.0.7/botasaurus_requests/
+-rw-rw-rw-   0        0        0      700 2024-05-16 11:45:50.000000 botasaurus_requests-4.0.7/botasaurus_requests/__init__.py
+-rw-rw-rw-   0        0        0     4295 2024-05-17 05:17:09.000000 botasaurus_requests-4.0.7/botasaurus_requests/__main__.py
+-rw-rw-rw-   0        0        0       21 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.7/botasaurus_requests/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 05:57:44.079705 botasaurus_requests-4.0.7/botasaurus_requests/bin/
+-rw-rw-rw-   0        0        0        0 2024-05-16 05:45:16.000000 botasaurus_requests-4.0.7/botasaurus_requests/bin/__init__.py
+-rw-rw-rw-   0        0        0     7300 2024-05-17 05:18:33.000000 botasaurus_requests-4.0.7/botasaurus_requests/cffi.py
+-rw-rw-rw-   0        0        0    15963 2024-05-16 12:29:29.000000 botasaurus_requests-4.0.7/botasaurus_requests/client.py
+-rw-rw-rw-   0        0        0    16718 2024-05-16 06:48:02.000000 botasaurus_requests-4.0.7/botasaurus_requests/cookies.py
+-rw-rw-rw-   0        0        0      767 2024-05-16 06:02:03.000000 botasaurus_requests-4.0.7/botasaurus_requests/exceptions.py
+-rw-rw-rw-   0        0        0     5913 2024-05-17 05:18:21.000000 botasaurus_requests-4.0.7/botasaurus_requests/headers.py
+-rw-rw-rw-   0        0        0    16753 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.7/botasaurus_requests/parser.py
+-rw-rw-rw-   0        0        0    19318 2024-05-16 11:31:13.000000 botasaurus_requests-4.0.7/botasaurus_requests/reqs.py
+-rw-rw-rw-   0        0        0     8395 2024-05-16 16:07:08.000000 botasaurus_requests-4.0.7/botasaurus_requests/request_class.py
+-rw-rw-rw-   0        0        0       19 2024-05-16 12:29:29.000000 botasaurus_requests-4.0.7/botasaurus_requests/request_functions.py
+-rw-rw-rw-   0        0        0     9871 2024-05-16 15:04:13.000000 botasaurus_requests-4.0.7/botasaurus_requests/response.py
+-rw-rw-rw-   0        0        0    12167 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.7/botasaurus_requests/session.py
+-rw-rw-rw-   0        0        0     4692 2024-05-16 05:45:16.000000 botasaurus_requests-4.0.7/botasaurus_requests/toolbelt.py
+drwxrwxrwx   0        0        0        0 2024-05-17 05:57:44.080701 botasaurus_requests-4.0.7/botasaurus_requests.egg-info/
+-rw-rw-rw-   0        0        0    14770 2024-05-17 05:57:43.000000 botasaurus_requests-4.0.7/botasaurus_requests.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      797 2024-05-17 05:57:43.000000 botasaurus_requests-4.0.7/botasaurus_requests.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 05:57:43.000000 botasaurus_requests-4.0.7/botasaurus_requests.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-05-17 05:57:43.000000 botasaurus_requests-4.0.7/botasaurus_requests.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-17 05:57:43.000000 botasaurus_requests-4.0.7/botasaurus_requests.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1008 2024-05-17 05:57:42.000000 botasaurus_requests-4.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       81 2024-05-17 05:57:44.083382 botasaurus_requests-4.0.7/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-24 07:16:00.000000 botasaurus_requests-4.0.7/setup.py
```

### Comparing `botasaurus_requests-4.0.5/LICENSE` & `botasaurus_requests-4.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.5/PKG-INFO` & `botasaurus_requests-4.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botasaurus_requests
-Version: 4.0.5
+Version: 4.0.7
 Summary: botasaurus_requests is a fork of the requests library with the playwright dependencies removed.
 Author-email: Chetan <chetan@omkar.cloud>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `botasaurus_requests-4.0.5/README.md` & `botasaurus_requests-4.0.7/README.md`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.5/botasaurus_requests/__init__.py` & `botasaurus_requests-4.0.7/botasaurus_requests/__init__.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.5/botasaurus_requests/__main__.py` & `botasaurus_requests-4.0.7/botasaurus_requests/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         raise ValueError('No assets found')
 
     def install(self) -> None:
         filename = super().check_library()
         ver: Version = Version.get_version(filename)
 
         rprint(
-            f'[bright_green]:sparkles: Successfully installed cgo v{ver}! :tada:[/]'
+            f'[bright_green]:sparkles: Successfully installed dependencies v{ver}! :tada:[/]'
         )
 
     def update(self) -> None:
         '''
         Updates the library if needed
         '''
         path = self.path
@@ -96,20 +96,20 @@
 
         # get the version
         current_ver: Version = Version.get_version(path)
 
         # check if the version is the same as the latest avaliable version
         asset: Asset = self.latest_asset()
         if current_ver >= asset.version:
-            rprint('[bright_green]:sparkles: cgo library up to date! :tada:')
+            rprint('[bright_green]:sparkles: library up to date! :tada:')
             rprint(f'Current version: [green]v{current_ver}\n')
             return
 
         # download updated file
-        rprint(f'Updating cgo library from [red]v{current_ver}[/] => v{asset.version}')
+        rprint(f'Updating dependencies from [red]v{current_ver}[/] => v{asset.version}')
         # download new, remove old
         self.download_file(self.full_path, asset.url)
         try:
             os.remove(os.path.join(self.parent_path, path))
         except OSError:
             rprint('[yellow]Warning: Could not remove outdated library files.')
 
@@ -141,33 +141,9 @@
         headers = library = True
     library and LibraryUpdate().update()
     headers and HeaderUpdate().update()
 
 
 
 
-@cli.command(name='version')
-def version() -> None:
-
-
-    # library path
-    libup = LibraryUpdate()
-    path = libup.path
-    # if the library is not installed
-    if not path:
-        rprint('cgo:\t[red]Not installed!')
-        return
-    # library verion
-    lib_ver = Version.get_version(path)
-    rprint(f'cgo:\t[green]{lib_ver}')
-
-    # check for library updates
-    with Status('Checking for updates...'):
-        latest_ver = libup.latest_asset().version
-        if latest_ver == lib_ver:
-            rprint('\t\t([yellow]Up to date![/])')
-        else:
-            rprint(f'\t\t([yellow]latest = {latest_ver}[/])')
-
-
 if __name__ == '__main__':
     cli()
```

### Comparing `botasaurus_requests-4.0.5/botasaurus_requests/cffi.py` & `botasaurus_requests-4.0.7/botasaurus_requests/cffi.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from httpx import get, stream
 from orjson import loads
 
 from botasaurus_requests.__version__ import BRIDGE_VERSION
 
 root_dir: Path = Path(os.path.abspath(os.path.dirname(__file__)))
 
-# map machine architecture to cgo binary name
 arch_map = {
     'amd64': 'amd64',
     'x86_64': 'amd64',
     'x86': '386',
     'i686': '386',
     'i386': '386',
     'arm64': 'arm64',
@@ -98,15 +97,15 @@
     def get_releases(self) -> dict:
         resp = get('https://api.github.com/repos/daijro/hrequests/releases')
         if resp.status_code != 200:
             raise ConnectionError(f'Could not connect to GitHub: {resp.text}')
         return loads(resp.content)
 
     def download_library(self):
-        print('Downloading cgo library ...')
+        print('Downloading @request dependencies...')
         releases = self.get_releases()
         for release in releases:
             asset = self.check_assets(release['assets'])
             if asset:
                 url, name = asset
                 break
         else:
```

### Comparing `botasaurus_requests-4.0.5/botasaurus_requests/client.py` & `botasaurus_requests-4.0.7/botasaurus_requests/client.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.5/botasaurus_requests/cookies.py` & `botasaurus_requests-4.0.7/botasaurus_requests/cookies.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.5/botasaurus_requests/exceptions.py` & `botasaurus_requests-4.0.7/botasaurus_requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.5/botasaurus_requests/headers.py` & `botasaurus_requests-4.0.7/botasaurus_requests/headers.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,14 @@
     file_name: str = join(dirname(__file__), "bin", "CR_VERSIONS.json")
 
     @staticmethod
     def get_ver(line: str) -> str:
         return re.sub(r'[^\d\.]', '', line)
 
     def download(self) -> List[str]:
-        print('Downloading Chrome version history...')
         versions: List[str]
         with httpx.stream('GET', self.resource) as r:
             lines = r.iter_lines()
             # search for first version number
             for line in lines:
                 highest_ver = re.search(r'\d+', line)
                 if highest_ver:  # on the first number
@@ -97,15 +96,14 @@
 
 
 class FirefoxVersions(VersionScraper):
     resource: str = 'https://ftp.mozilla.org/pub/firefox/releases/'
     file_name: str = join(dirname(__file__), "bin", "FF_VERSIONS.json")
 
     def download(self) -> List[str]:
-        print('Downloading Firefox version history...')
         resp = httpx.get(self.resource)
         # gather version numbers
         versions: List[str]
         versions = re.findall(r'/pub/firefox/releases/([\d\.]+)/', resp.text)
         versions = sorted(set(versions), key=self.leading_num, reverse=True)
 
         highest_ver: int = self.leading_num(versions[0])
```

### Comparing `botasaurus_requests-4.0.5/botasaurus_requests/parser.py` & `botasaurus_requests-4.0.7/botasaurus_requests/parser.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.5/botasaurus_requests/reqs.py` & `botasaurus_requests-4.0.7/botasaurus_requests/reqs.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.5/botasaurus_requests/request_class.py` & `botasaurus_requests-4.0.7/botasaurus_requests/request_class.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.5/botasaurus_requests/response.py` & `botasaurus_requests-4.0.7/botasaurus_requests/response.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.5/botasaurus_requests/session.py` & `botasaurus_requests-4.0.7/botasaurus_requests/session.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.5/botasaurus_requests/toolbelt.py` & `botasaurus_requests-4.0.7/botasaurus_requests/toolbelt.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.5/botasaurus_requests.egg-info/PKG-INFO` & `botasaurus_requests-4.0.7/botasaurus_requests.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botasaurus_requests
-Version: 4.0.5
+Version: 4.0.7
 Summary: botasaurus_requests is a fork of the requests library with the playwright dependencies removed.
 Author-email: Chetan <chetan@omkar.cloud>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `botasaurus_requests-4.0.5/botasaurus_requests.egg-info/SOURCES.txt` & `botasaurus_requests-4.0.7/botasaurus_requests.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.5/pyproject.toml` & `botasaurus_requests-4.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "botasaurus_requests"
-version="4.0.5"
+version="4.0.7"
 description = "botasaurus_requests is a fork of the requests library with the playwright dependencies removed."
 authors = [
   {name = "Chetan", email = "chetan@omkar.cloud" } # Optional
 ]
 license = {file = "LICENSE"}
 readme = "README.md"
 keywords = [
```

