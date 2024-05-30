# Comparing `tmp/komootgpx-1.1.2.tar.gz` & `tmp/komootgpx-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "komootgpx-1.1.2.tar", last modified: Thu Dec 29 02:03:47 2022, max compression
+gzip compressed data, was "komootgpx-1.2.0.tar", last modified: Thu May 30 23:34:22 2024, max compression
```

## Comparing `komootgpx-1.1.2.tar` & `komootgpx-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 tim       (1000) tim       (1001)        0 2022-12-29 02:03:47.407395 komootgpx-1.1.2/
--rw-r--r--   0 tim       (1000) tim       (1001)    35149 2022-06-22 21:17:17.000000 komootgpx-1.1.2/LICENSE
--rw-r--r--   0 tim       (1000) tim       (1001)     2299 2022-12-29 02:03:47.407395 komootgpx-1.1.2/PKG-INFO
--rw-r--r--   0 tim       (1000) tim       (1001)     1615 2022-12-29 01:56:52.000000 komootgpx-1.1.2/README.md
-drwxr-xr-x   0 tim       (1000) tim       (1001)        0 2022-12-29 02:03:47.407395 komootgpx-1.1.2/komootgpx/
--rw-r--r--   0 tim       (1000) tim       (1001)       24 2022-12-29 01:20:23.000000 komootgpx-1.1.2/komootgpx/__init__.py
--rw-r--r--   0 tim       (1000) tim       (1001)       79 2022-12-29 01:41:57.000000 komootgpx-1.1.2/komootgpx/__main__.py
--rw-r--r--   0 tim       (1000) tim       (1001)       62 2022-12-29 01:57:08.000000 komootgpx-1.1.2/komootgpx/__version__.py
--rw-r--r--   0 tim       (1000) tim       (1001)     4060 2022-12-29 01:24:04.000000 komootgpx-1.1.2/komootgpx/api.py
--rw-r--r--   0 tim       (1000) tim       (1001)     6338 2022-06-22 21:17:17.000000 komootgpx-1.1.2/komootgpx/gpxcompiler.py
--rw-r--r--   0 tim       (1000) tim       (1001)     4632 2022-12-29 01:52:07.000000 komootgpx-1.1.2/komootgpx/komootgpx.py
--rw-r--r--   0 tim       (1000) tim       (1001)     1254 2022-12-29 01:24:04.000000 komootgpx-1.1.2/komootgpx/utils.py
-drwxr-xr-x   0 tim       (1000) tim       (1001)        0 2022-12-29 02:03:47.407395 komootgpx-1.1.2/komootgpx.egg-info/
--rw-r--r--   0 tim       (1000) tim       (1001)     2299 2022-12-29 02:03:47.000000 komootgpx-1.1.2/komootgpx.egg-info/PKG-INFO
--rw-r--r--   0 tim       (1000) tim       (1001)      379 2022-12-29 02:03:47.000000 komootgpx-1.1.2/komootgpx.egg-info/SOURCES.txt
--rw-r--r--   0 tim       (1000) tim       (1001)        1 2022-12-29 02:03:47.000000 komootgpx-1.1.2/komootgpx.egg-info/dependency_links.txt
--rw-r--r--   0 tim       (1000) tim       (1001)       51 2022-12-29 02:03:47.000000 komootgpx-1.1.2/komootgpx.egg-info/entry_points.txt
--rw-r--r--   0 tim       (1000) tim       (1001)       53 2022-12-29 02:03:47.000000 komootgpx-1.1.2/komootgpx.egg-info/requires.txt
--rw-r--r--   0 tim       (1000) tim       (1001)       10 2022-12-29 02:03:47.000000 komootgpx-1.1.2/komootgpx.egg-info/top_level.txt
--rw-r--r--   0 tim       (1000) tim       (1001)       38 2022-12-29 02:03:47.407395 komootgpx-1.1.2/setup.cfg
--rw-r--r--   0 tim       (1000) tim       (1001)     3623 2022-12-29 01:42:43.000000 komootgpx-1.1.2/setup.py
+drwxr-xr-x   0 tim       (1000) tim       (1001)        0 2024-05-30 23:34:22.699425 komootgpx-1.2.0/
+-rw-r--r--   0 tim       (1000) tim       (1001)    35149 2024-05-30 23:22:31.000000 komootgpx-1.2.0/LICENSE
+-rw-r--r--   0 tim       (1000) tim       (1001)     2514 2024-05-30 23:34:22.699425 komootgpx-1.2.0/PKG-INFO
+-rw-r--r--   0 tim       (1000) tim       (1001)     1672 2024-05-30 23:22:36.000000 komootgpx-1.2.0/README.md
+drwxr-xr-x   0 tim       (1000) tim       (1001)        0 2024-05-30 23:34:22.696092 komootgpx-1.2.0/komootgpx/
+-rw-r--r--   0 tim       (1000) tim       (1001)       24 2024-05-30 23:22:31.000000 komootgpx-1.2.0/komootgpx/__init__.py
+-rw-r--r--   0 tim       (1000) tim       (1001)       79 2024-05-30 23:22:31.000000 komootgpx-1.2.0/komootgpx/__main__.py
+-rw-r--r--   0 tim       (1000) tim       (1001)       63 2024-05-30 23:23:49.000000 komootgpx-1.2.0/komootgpx/__version__.py
+-rw-r--r--   0 tim       (1000) tim       (1001)     3853 2024-05-30 23:22:36.000000 komootgpx-1.2.0/komootgpx/api.py
+-rw-r--r--   0 tim       (1000) tim       (1001)     6338 2024-05-30 23:22:31.000000 komootgpx-1.2.0/komootgpx/gpxcompiler.py
+-rw-r--r--   0 tim       (1000) tim       (1001)     5304 2024-05-30 23:22:36.000000 komootgpx-1.2.0/komootgpx/komootgpx.py
+-rw-r--r--   0 tim       (1000) tim       (1001)     1254 2024-05-30 23:22:31.000000 komootgpx-1.2.0/komootgpx/utils.py
+drwxr-xr-x   0 tim       (1000) tim       (1001)        0 2024-05-30 23:34:22.699425 komootgpx-1.2.0/komootgpx.egg-info/
+-rw-r--r--   0 tim       (1000) tim       (1001)     2514 2024-05-30 23:34:22.000000 komootgpx-1.2.0/komootgpx.egg-info/PKG-INFO
+-rwxrwxrwx   0 tim       (1000) tim       (1001)      379 2024-05-30 23:34:22.000000 komootgpx-1.2.0/komootgpx.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tim       (1000) tim       (1001)        1 2024-05-30 23:34:22.000000 komootgpx-1.2.0/komootgpx.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tim       (1000) tim       (1001)       51 2024-05-30 23:34:22.000000 komootgpx-1.2.0/komootgpx.egg-info/entry_points.txt
+-rwxrwxrwx   0 tim       (1000) tim       (1001)       53 2024-05-30 23:34:22.000000 komootgpx-1.2.0/komootgpx.egg-info/requires.txt
+-rwxrwxrwx   0 tim       (1000) tim       (1001)       10 2024-05-30 23:34:22.000000 komootgpx-1.2.0/komootgpx.egg-info/top_level.txt
+-rw-r--r--   0 tim       (1000) tim       (1001)       38 2024-05-30 23:34:22.699425 komootgpx-1.2.0/setup.cfg
+-rw-r--r--   0 tim       (1000) tim       (1001)     3623 2024-05-30 23:22:31.000000 komootgpx-1.2.0/setup.py
```

### Comparing `komootgpx-1.1.2/LICENSE` & `komootgpx-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `komootgpx-1.1.2/PKG-INFO` & `komootgpx-1.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 Metadata-Version: 2.1
 Name: komootgpx
-Version: 1.1.2
+Version: 1.2.0
 Summary: Download Komoot tracks and highlights as GPX files (including metadata). Supports bulk-download.
 Home-page: https://github.com/thepbone/KomootGPX
 Author: Tim Schneeberger
 Author-email: tim.schneeberger@outlook.de
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet
 Classifier: Topic :: System :: Archiving
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: certifi
+Requires-Dist: chardet
+Requires-Dist: colorama
+Requires-Dist: gpxpy
+Requires-Dist: idna
+Requires-Dist: requests
+Requires-Dist: urllib3
 
 
 # KomootGPX
 Download Komoot tracks and highlights as GPX files with metadata
 
 [Python 3 or later](https://www.python.org/downloads/) is required.
 
 ## Installation
-
+Download from [PyPI](https://pypi.org/project/komootgpx/):
 ```
 pip install komootgpx
 ```
-
 ## Usage
 
 Run script in interactive mode
 ```
 komootgpx
 ```
 ```
```

### Comparing `komootgpx-1.1.2/README.md` & `komootgpx-1.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # KomootGPX
 Download Komoot tracks and highlights as GPX files with metadata
 
 [Python 3 or later](https://www.python.org/downloads/) is required.
 
 ## Installation
-
+Download from [PyPI](https://pypi.org/project/komootgpx/):
 ```
 pip install komootgpx
 ```
-
 ## Usage
 
 Run script in interactive mode
 ```
 komootgpx
 ```
 ```
```

### Comparing `komootgpx-1.1.2/komootgpx/api.py` & `komootgpx-1.2.0/komootgpx/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,19 +17,17 @@
 
 class KomootApi:
     def __init__(self):
         self.user_id = ''
         self.token = ''
 
     def __build_header(self):
-        if self.user_id != '' and self.token != '':
-            return {
-                "Authorization": "Basic {0}".format(
-                    base64.b64encode(bytes(self.user_id + ":" + self.token, 'utf-8')).decode())}
-        return {}
+        if self.user_id and self.token:
+            return BasicAuthToken(self.user_id, self.token)
+        return None
 
     @staticmethod
     def __send_request(url, auth, critical=True):
         r = requests.get(url, auth=auth)
         if r.status_code != 200:
             print_error("Error " + str(r.status_code) + ": " + str(r.json()))
             if critical:
@@ -51,53 +49,52 @@
         if not silent:
             print("Fetching tours of user '" + self.user_id + "'...")
 
         results = {}
         has_next_page = True
         current_uri = "https://api.komoot.de/v007/users/" + self.user_id + "/tours/"
         while has_next_page:
-            r = self.__send_request(current_uri,
-                                    BasicAuthToken(self.user_id, self.token))
+            r = self.__send_request(current_uri, self.__build_header())
 
             has_next_page = 'next' in r.json()['_links'] and 'href' in r.json()['_links']['next']
             if has_next_page:
                 current_uri = r.json()['_links']['next']['href']
 
             tours = r.json()['_embedded']['tours']
             for tour in tours:
                 if tourType != "all" and tourType != tour['type']:
                     continue
-                results[tour['id']] = tour['name'] + " (" + tour['sport'] + "; " + str(
-                    int(tour['distance']) / 1000.0) + "km; " + tour['type'] + ")"
+                results[tour['id']] = tour;
 
         print("Found " + str(len(results)) + " tours")
         return results
 
     def print_tours(self, tourType="all"):
         tours = self.fetch_tours(tourType, silent=True)
         print()
-        for tour_id, name in tours.items():
-            print(bcolor.BOLD + bcolor.HEADER + str(tour_id) + bcolor.ENDC + " => " + bcolor.BOLD + name + bcolor.ENDC)
+        for tour_id, tour in tours.items():
+            descr =  tour['name'] + " (" + tour['sport'] + "; " + str(int(tour['distance']) / 1000.0) + "km; " + tour['type'] + ")"
+            print(bcolor.BOLD + bcolor.HEADER + str(tour_id) + bcolor.ENDC + " => " + bcolor.BOLD + descr + bcolor.ENDC)
 
         if len(tours) < 1:
             print_error("No tours found on your profile")
 
     def fetch_tour(self, tour_id):
         print("Fetching tour '" + tour_id + "'...")
 
         r = self.__send_request("https://api.komoot.de/v007/tours/" + tour_id + "?_embedded=coordinates,way_types,"
                                                                                 "surfaces,directions,participants,"
                                                                                 "timeline&directions=v2&fields"
                                                                                 "=timeline&format=coordinate_array"
                                                                                 "&timeline_highlights_fields=tips,"
                                                                                 "recommenders",
-                                BasicAuthToken(self.user_id, self.token))
+                                self.__build_header())
 
         return r.json()
 
     def fetch_highlight_tips(self, highlight_id):
         print("Fetching highlight '" + highlight_id + "'...")
 
         r = self.__send_request("https://api.komoot.de/v007/highlights/" + highlight_id + "/tips/",
-                                BasicAuthToken(self.user_id, self.token), critical=False)
+                                self.__build_header(), critical=False)
 
         return r.json()
```

### Comparing `komootgpx-1.1.2/komootgpx/gpxcompiler.py` & `komootgpx-1.2.0/komootgpx/gpxcompiler.py`

 * *Files identical despite different names*

### Comparing `komootgpx-1.1.2/komootgpx/komootgpx.py` & `komootgpx-1.2.0/komootgpx/komootgpx.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,52 +25,59 @@
     print('\t{:<2s}, {:<30s} {:<10s}'.format('-D', '--add-date', 'Add date to file name'))
     print(bcolor.OKBLUE + '[Filters]' + bcolor.ENDC)
     print('\t{:<2s}, {:<30s} {:<10s}'.format('-f', '--filter=type', 'Filter by track type (either "planned" or '
                                                                     '"recorded")'))
     print(bcolor.OKBLUE + '[Generator]' + bcolor.ENDC)
     print('\t{:<2s}, {:<30s} {:<10s}'.format('-o', '--output', 'Output directory (default: working directory)'))
     print('\t{:<2s}, {:<30s} {:<10s}'.format('-e', '--no-poi', 'Do not include highlights as POIs'))
+    print('\t{:<2s}, {:<30s} {:<10s}'.format('-s', '--skip-existing', 'Do not download and save GPX if the file already exists, ignored with -d'))
 
 
 def notify_interactive():
     global interactive_info_shown
     interactive_info_shown = True
     if interactive_info_shown:
         print("Interactive mode. Use '--help' for usage details.")
 
 
-def make_gpx(tour_id, api, output_dir, no_poi, add_date):
-    tour = api.fetch_tour(str(tour_id))
-    gpx = GpxCompiler(tour, api, no_poi)
-
+def make_gpx(tour_id, api, output_dir, no_poi, skip_existing, tour, add_date):
     # Example date: 2022-01-02T12:26:41.795+01:00
     # :10 extracts "2022-01-02" from this.
     date_str = tour['date'][:10]+'_' if add_date else ''
 
     path = f"{output_dir}/{date_str}{sanitize_filename(tour['name'])}-{tour_id}.gpx"
+
+    if skip_existing and os.path.exists(path):
+        print_success(f"{tour['name']} skipped - already exists at '{path}'")
+        return
+
+    tour = api.fetch_tour(str(tour_id))
+    gpx = GpxCompiler(tour, api, no_poi)
+
     f = open(path, "w", encoding="utf-8")
     f.write(gpx.generate())
     f.close()
 
     print_success(f"GPX file written to '{path}'")
 
 
 def main(argv):
     tour_selection = ''
     mail = ''
     pwd = ''
     print_tours = False
     no_poi = False
+    skip_existing = False
     add_date = False
     typeFilter = "all"
     output_dir = os.getcwd()
 
     try:
-        opts, args = getopt.getopt(argv, "ahleDo:d:m:p:f:", ["add-date", "list-tours", "make-gpx=", "mail=",
-                                                        "pass=", "filter=", "no-poi", "output=", "make-all"])
+        opts, args = getopt.getopt(argv, "ahlesDo:d:m:p:f:", ["add-date", "list-tours", "make-gpx=", "mail=",
+                                                        "pass=", "filter=", "no-poi", "output=", "skip-existing", "make-all"])
     except getopt.GetoptError:
         usage()
         sys.exit(2)
 
     for opt, arg in opts:
         if opt == '-h':
             usage()
@@ -81,14 +88,17 @@
 
         elif opt in ("-l", "--list-tours"):
             print_tours = True
 
         elif opt in ("-e", "--no-poi"):
             no_poi = True
 
+        elif opt in ("-s", "--skip-existing"):
+            skip_existing = True
+
         elif opt in ("-D", "--add-date"):
             add_date = True
 
         elif opt in ("-d", "--make-gpx"):
             tour_selection = str(arg)
 
         elif opt in ("-m", "--mail"):
@@ -99,14 +109,19 @@
 
         elif opt in ("-o", "--output"):
             output_dir = str(arg)
 
         elif opt in ("-a", "--make-all"):
             tour_selection = "all"
 
+    if tour_selection and tour_selection != "all":
+        api = KomootApi()
+        make_gpx(tour_selection, api, output_dir, no_poi, False, None, add_date)
+        return
+
     if mail == "":
         notify_interactive()
         mail = prompt("Enter your mail address (komoot.de)")
 
     if pwd == "":
         notify_interactive()
         pwd = prompt_pass("Enter your password (input hidden)")
@@ -128,17 +143,17 @@
     if tour_selection != "all" and int(tour_selection) not in tours:
         print_error("Unknown tour id selected. These are all available tours on your profile:")
         api.print_tours(typeFilter)
         exit(0)
 
     if tour_selection == "all":
         for x in tours:
-            make_gpx(x, api, output_dir, no_poi, add_date)
+            make_gpx(x, api, output_dir, no_poi, skip_existing, tours[x], add_date)
     else:
-        make_gpx(tour_selection, api, output_dir, no_poi, add_date)
+        make_gpx(tour_selection, api, output_dir, no_poi, skip_existing, tours[tour_selection], add_date)
     print()
 
 
 def entrypoint():
     try:
         return main(sys.argv[1:])
     except KeyboardInterrupt:
```

### Comparing `komootgpx-1.1.2/komootgpx/utils.py` & `komootgpx-1.2.0/komootgpx/utils.py`

 * *Files identical despite different names*

### Comparing `komootgpx-1.1.2/komootgpx.egg-info/PKG-INFO` & `komootgpx-1.2.0/komootgpx.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 Metadata-Version: 2.1
 Name: komootgpx
-Version: 1.1.2
+Version: 1.2.0
 Summary: Download Komoot tracks and highlights as GPX files (including metadata). Supports bulk-download.
 Home-page: https://github.com/thepbone/KomootGPX
 Author: Tim Schneeberger
 Author-email: tim.schneeberger@outlook.de
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet
 Classifier: Topic :: System :: Archiving
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: certifi
+Requires-Dist: chardet
+Requires-Dist: colorama
+Requires-Dist: gpxpy
+Requires-Dist: idna
+Requires-Dist: requests
+Requires-Dist: urllib3
 
 
 # KomootGPX
 Download Komoot tracks and highlights as GPX files with metadata
 
 [Python 3 or later](https://www.python.org/downloads/) is required.
 
 ## Installation
-
+Download from [PyPI](https://pypi.org/project/komootgpx/):
 ```
 pip install komootgpx
 ```
-
 ## Usage
 
 Run script in interactive mode
 ```
 komootgpx
 ```
 ```
```

### Comparing `komootgpx-1.1.2/setup.py` & `komootgpx-1.2.0/setup.py`

 * *Files identical despite different names*

