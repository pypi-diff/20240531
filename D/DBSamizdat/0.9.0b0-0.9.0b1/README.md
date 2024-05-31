# Comparing `tmp/dbsamizdat-0.9.0b0.tar.gz` & `tmp/dbsamizdat-0.9.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbsamizdat-0.9.0b0.tar", last modified: Wed Apr 17 19:50:50 2024, max compression
+gzip compressed data, was "dbsamizdat-0.9.0b1.tar", last modified: Fri Apr 19 15:27:54 2024, max compression
```

## Comparing `dbsamizdat-0.9.0b0.tar` & `dbsamizdat-0.9.0b1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-x---   0 boer      (1000) boer      (1000)        0 2024-04-17 19:50:50.365459 dbsamizdat-0.9.0b0/
--rw-r-----   0 boer      (1000) boer      (1000)    32474 2021-11-20 11:47:56.000000 dbsamizdat-0.9.0b0/LICENSE.txt
--rw-r-----   0 boer      (1000) boer      (1000)       16 2021-11-20 11:47:56.000000 dbsamizdat-0.9.0b0/MANIFEST.in
--rw-r--r--   0 boer      (1000) boer      (1000)    27386 2024-04-17 19:50:50.365459 dbsamizdat-0.9.0b0/PKG-INFO
--rw-r-----   0 boer      (1000) boer      (1000)    26401 2024-04-17 19:37:26.000000 dbsamizdat-0.9.0b0/README.md
--rw-r-----   0 boer      (1000) boer      (1000)       12 2024-04-16 16:04:47.000000 dbsamizdat-0.9.0b0/VERSION
--rw-r-----   0 boer      (1000) boer      (1000)     1374 2024-04-17 19:50:50.366459 dbsamizdat-0.9.0b0/setup.cfg
--rwxr-x---   0 boer      (1000) boer      (1000)       61 2021-11-20 11:47:56.000000 dbsamizdat-0.9.0b0/setup.py
-drwxr-x---   0 boer      (1000) boer      (1000)        0 2024-04-17 19:50:50.362459 dbsamizdat-0.9.0b0/src/
-drwxr-x---   0 boer      (1000) boer      (1000)        0 2024-04-17 19:50:50.365459 dbsamizdat-0.9.0b0/src/DBSamizdat.egg-info/
--rw-r--r--   0 boer      (1000) boer      (1000)    27386 2024-04-17 19:50:50.000000 dbsamizdat-0.9.0b0/src/DBSamizdat.egg-info/PKG-INFO
--rw-r-----   0 boer      (1000) boer      (1000)      741 2024-04-17 19:50:50.000000 dbsamizdat-0.9.0b0/src/DBSamizdat.egg-info/SOURCES.txt
--rw-r-----   0 boer      (1000) boer      (1000)        1 2024-04-17 19:50:50.000000 dbsamizdat-0.9.0b0/src/DBSamizdat.egg-info/dependency_links.txt
--rw-r-----   0 boer      (1000) boer      (1000)       54 2024-04-17 19:50:50.000000 dbsamizdat-0.9.0b0/src/DBSamizdat.egg-info/entry_points.txt
--rw-r-----   0 boer      (1000) boer      (1000)       30 2024-04-17 19:50:50.000000 dbsamizdat-0.9.0b0/src/DBSamizdat.egg-info/requires.txt
--rw-r-----   0 boer      (1000) boer      (1000)       11 2024-04-17 19:50:50.000000 dbsamizdat-0.9.0b0/src/DBSamizdat.egg-info/top_level.txt
--rw-r-----   0 boer      (1000) boer      (1000)        1 2021-11-16 16:18:44.000000 dbsamizdat-0.9.0b0/src/DBSamizdat.egg-info/zip-safe
-drwxr-x---   0 boer      (1000) boer      (1000)        0 2024-04-17 19:50:50.365459 dbsamizdat-0.9.0b0/src/dbsamizdat/
--rw-r-----   0 boer      (1000) boer      (1000)      197 2024-04-16 14:15:40.000000 dbsamizdat-0.9.0b0/src/dbsamizdat/__init__.py
--rw-r-----   0 boer      (1000) boer      (1000)     2018 2024-04-17 19:37:26.000000 dbsamizdat-0.9.0b0/src/dbsamizdat/api.py
--rw-r-----   0 boer      (1000) boer      (1000)     4733 2024-04-17 19:37:26.000000 dbsamizdat-0.9.0b0/src/dbsamizdat/apps.py
--rw-r-----   0 boer      (1000) boer      (1000)     2298 2024-04-17 19:37:26.000000 dbsamizdat-0.9.0b0/src/dbsamizdat/django_api.py
--rw-r-----   0 boer      (1000) boer      (1000)     2997 2024-04-17 19:37:26.000000 dbsamizdat-0.9.0b0/src/dbsamizdat/exceptions.py
--rw-r-----   0 boer      (1000) boer      (1000)     2272 2024-04-16 14:15:40.000000 dbsamizdat-0.9.0b0/src/dbsamizdat/graphvizdot.py
--rw-r-----   0 boer      (1000) boer      (1000)     4937 2024-04-16 14:15:40.000000 dbsamizdat-0.9.0b0/src/dbsamizdat/libdb.py
--rw-r-----   0 boer      (1000) boer      (1000)     4810 2024-04-17 19:37:26.000000 dbsamizdat-0.9.0b0/src/dbsamizdat/libgraph.py
--rw-r-----   0 boer      (1000) boer      (1000)     2094 2024-04-16 14:15:40.000000 dbsamizdat-0.9.0b0/src/dbsamizdat/loader.py
-drwxr-x---   0 boer      (1000) boer      (1000)        0 2024-04-17 19:50:50.362459 dbsamizdat-0.9.0b0/src/dbsamizdat/management/
-drwxr-x---   0 boer      (1000) boer      (1000)        0 2024-04-17 19:50:50.365459 dbsamizdat-0.9.0b0/src/dbsamizdat/management/commands/
--rw-r-----   0 boer      (1000) boer      (1000)      816 2024-04-17 19:37:26.000000 dbsamizdat-0.9.0b0/src/dbsamizdat/management/commands/dbsamizdat.py
--rw-r-----   0 boer      (1000) boer      (1000)      110 2021-11-20 11:47:56.000000 dbsamizdat-0.9.0b0/src/dbsamizdat/models.py
--rwxr-x---   0 boer      (1000) boer      (1000)    16497 2024-04-17 19:37:26.000000 dbsamizdat-0.9.0b0/src/dbsamizdat/runner.py
--rw-r-----   0 boer      (1000) boer      (1000)    12888 2024-04-16 14:15:40.000000 dbsamizdat-0.9.0b0/src/dbsamizdat/samizdat.py
--rw-r-----   0 boer      (1000) boer      (1000)     2881 2024-04-16 14:15:40.000000 dbsamizdat-0.9.0b0/src/dbsamizdat/test_samizdats.py
--rw-r-----   0 boer      (1000) boer      (1000)     1633 2024-04-17 19:37:26.000000 dbsamizdat-0.9.0b0/src/dbsamizdat/util.py
+drwxr-x---   0 boer      (1000) boer      (1000)        0 2024-04-19 15:27:54.368275 dbsamizdat-0.9.0b1/
+-rw-r-----   0 boer      (1000) boer      (1000)    32474 2021-11-20 11:47:56.000000 dbsamizdat-0.9.0b1/LICENSE.txt
+-rw-r-----   0 boer      (1000) boer      (1000)       16 2021-11-20 11:47:56.000000 dbsamizdat-0.9.0b1/MANIFEST.in
+-rw-r--r--   0 boer      (1000) boer      (1000)    27784 2024-04-19 15:27:54.368275 dbsamizdat-0.9.0b1/PKG-INFO
+-rw-r-----   0 boer      (1000) boer      (1000)    26786 2024-04-19 15:17:35.000000 dbsamizdat-0.9.0b1/README.md
+-rw-r-----   0 boer      (1000) boer      (1000)       12 2024-04-19 15:20:19.000000 dbsamizdat-0.9.0b1/VERSION
+-rw-r-----   0 boer      (1000) boer      (1000)     1387 2024-04-19 15:27:54.368275 dbsamizdat-0.9.0b1/setup.cfg
+-rwxr-x---   0 boer      (1000) boer      (1000)       61 2021-11-20 11:47:56.000000 dbsamizdat-0.9.0b1/setup.py
+drwxr-x---   0 boer      (1000) boer      (1000)        0 2024-04-19 15:27:54.365275 dbsamizdat-0.9.0b1/src/
+drwxr-x---   0 boer      (1000) boer      (1000)        0 2024-04-19 15:27:54.367275 dbsamizdat-0.9.0b1/src/DBSamizdat.egg-info/
+-rw-r--r--   0 boer      (1000) boer      (1000)    27784 2024-04-19 15:27:54.000000 dbsamizdat-0.9.0b1/src/DBSamizdat.egg-info/PKG-INFO
+-rw-r-----   0 boer      (1000) boer      (1000)      741 2024-04-19 15:27:54.000000 dbsamizdat-0.9.0b1/src/DBSamizdat.egg-info/SOURCES.txt
+-rw-r-----   0 boer      (1000) boer      (1000)        1 2024-04-19 15:27:54.000000 dbsamizdat-0.9.0b1/src/DBSamizdat.egg-info/dependency_links.txt
+-rw-r-----   0 boer      (1000) boer      (1000)       54 2024-04-19 15:27:54.000000 dbsamizdat-0.9.0b1/src/DBSamizdat.egg-info/entry_points.txt
+-rw-r-----   0 boer      (1000) boer      (1000)       30 2024-04-19 15:27:54.000000 dbsamizdat-0.9.0b1/src/DBSamizdat.egg-info/requires.txt
+-rw-r-----   0 boer      (1000) boer      (1000)       11 2024-04-19 15:27:54.000000 dbsamizdat-0.9.0b1/src/DBSamizdat.egg-info/top_level.txt
+-rw-r-----   0 boer      (1000) boer      (1000)        1 2021-11-16 16:18:44.000000 dbsamizdat-0.9.0b1/src/DBSamizdat.egg-info/zip-safe
+drwxr-x---   0 boer      (1000) boer      (1000)        0 2024-04-19 15:27:54.367275 dbsamizdat-0.9.0b1/src/dbsamizdat/
+-rw-r-----   0 boer      (1000) boer      (1000)      197 2024-04-18 08:52:53.000000 dbsamizdat-0.9.0b1/src/dbsamizdat/__init__.py
+-rw-r-----   0 boer      (1000) boer      (1000)     2018 2024-04-19 12:53:16.000000 dbsamizdat-0.9.0b1/src/dbsamizdat/api.py
+-rw-r-----   0 boer      (1000) boer      (1000)     5035 2024-04-19 15:25:51.000000 dbsamizdat-0.9.0b1/src/dbsamizdat/apps.py
+-rw-r-----   0 boer      (1000) boer      (1000)     2298 2024-04-19 12:53:16.000000 dbsamizdat-0.9.0b1/src/dbsamizdat/django_api.py
+-rw-r-----   0 boer      (1000) boer      (1000)     2997 2024-04-19 12:53:16.000000 dbsamizdat-0.9.0b1/src/dbsamizdat/exceptions.py
+-rw-r-----   0 boer      (1000) boer      (1000)     2272 2024-04-18 08:52:53.000000 dbsamizdat-0.9.0b1/src/dbsamizdat/graphvizdot.py
+-rw-r-----   0 boer      (1000) boer      (1000)     4937 2024-04-19 12:53:16.000000 dbsamizdat-0.9.0b1/src/dbsamizdat/libdb.py
+-rw-r-----   0 boer      (1000) boer      (1000)     4810 2024-04-19 12:53:16.000000 dbsamizdat-0.9.0b1/src/dbsamizdat/libgraph.py
+-rw-r-----   0 boer      (1000) boer      (1000)     2094 2024-04-19 12:53:16.000000 dbsamizdat-0.9.0b1/src/dbsamizdat/loader.py
+drwxr-x---   0 boer      (1000) boer      (1000)        0 2024-04-19 15:27:54.365275 dbsamizdat-0.9.0b1/src/dbsamizdat/management/
+drwxr-x---   0 boer      (1000) boer      (1000)        0 2024-04-19 15:27:54.367275 dbsamizdat-0.9.0b1/src/dbsamizdat/management/commands/
+-rw-r-----   0 boer      (1000) boer      (1000)      816 2024-04-19 12:53:16.000000 dbsamizdat-0.9.0b1/src/dbsamizdat/management/commands/dbsamizdat.py
+-rw-r-----   0 boer      (1000) boer      (1000)      110 2024-04-18 08:52:53.000000 dbsamizdat-0.9.0b1/src/dbsamizdat/models.py
+-rwxr-x---   0 boer      (1000) boer      (1000)    16581 2024-04-19 15:25:57.000000 dbsamizdat-0.9.0b1/src/dbsamizdat/runner.py
+-rw-r-----   0 boer      (1000) boer      (1000)    12888 2024-04-18 08:52:53.000000 dbsamizdat-0.9.0b1/src/dbsamizdat/samizdat.py
+-rw-r-----   0 boer      (1000) boer      (1000)     2881 2024-04-18 08:52:53.000000 dbsamizdat-0.9.0b1/src/dbsamizdat/test_samizdats.py
+-rw-r-----   0 boer      (1000) boer      (1000)     1633 2024-04-19 12:53:16.000000 dbsamizdat-0.9.0b1/src/dbsamizdat/util.py
```

### Comparing `dbsamizdat-0.9.0b0/LICENSE.txt` & `dbsamizdat-0.9.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbsamizdat-0.9.0b0/PKG-INFO` & `dbsamizdat-0.9.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: DBSamizdat
-Version: 0.9.0b0
+Version: 0.9.0b1
 Summary: dbsamizdat — the blissfully naive PostgreSQL database object manager
 Home-page: https://hub.sr.ht/~nullenenenen/DBSamizdat/
 Author: nullenenenen
 Author-email: nullenenenen@gavagai.eu
 License: GPL-3.0+
 Project-URL: Documentation, https://git.sr.ht/~nullenenenen/DBSamizdat/tree/master/item/README.md
 Project-URL: Source, https://git.sr.ht/~nullenenenen/DBSamizdat/
 Keywords: PostgreSQL Django
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Classifier: Topic :: Database
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: psycopg2>=2.8.0
 Requires-Dist: toposort>=1.5
 
 # DBSamizdat
 
 The blissfully naive PostgreSQL database object manager.
 
 For specifics on integrating with the Django web framework, and some examples for integrating with its ORM, see the [Django integration](#django-integration) section further down.
 
 For discussions, questions, bug reports, feature requests, development, and engaging other users, use the [public mailinglist](https://lists.sr.ht/~nullenenenen/dbsamizdat-discuss).
 
-It requires Python 3.6 or later, and is tested for compatibility with PostgreSQL 9.6 and up.
+It requires Python 3.8 or later, and is tested for compatibility with PostgreSQL 10 and up.
 
 ## What it is
 
 DBSamizdat is a lightweight tool that manages code that lives in the database: **views**, **materialized views**, **functions** and **triggers**, and the dependencies between those and other DB objects.
 
 There is a command-line utility, and a library-style API.
 
@@ -338,14 +338,15 @@
 To use the library API functions, load the `django_api` module rather than the `api` module.
 
 ### Extra configuration
 
 The following Django settings are consulted by DBSamizdat, if declared:
 
 - `DBSAMIZDAT_SMART_MIGRATIONS` — a boolean, `False` by default. This has to do with migrations. As Django's migrations are blissfully unaware of your samizdats, things will fail if, for instance, a table column is removed that one of your views selects. The default lets DBSamizdat assume the worst case, so it will simply remove all its DB state before Django's migrations are run, and restore the state afterwards. But if you define this setting as `True`, DBSamizdat will examine the migration plan and to determine the subset of DB state that will need to be dropped and rebuilt following all the migrations. This behaviour can be desirable when you have large or computationally intensive materialized views. But it's not turned on by default, as it's deemed experimental because of reliance on non-public Django APIs. See if it works for you, if not, turn it back off and send a bug report to the mailinglist!
+- `DBSAMIZDAT_PARALLEL_REFRESH_AFTER_MIGRATIONS` ­— a boolean, `False` by default. After migrations, if any materialized views are (re)created, they need to be populated (the first refresh). This can be done parallelized (same as `dbsamizdat refresh --parallel`). When setting this to `True`, it will also switch the syncing from using the "jumbo" transaction style to "checkpoint".
 - `DBSAMIZDAT_MODULES` — an Iterable[str] of module names, eg `["myapp.somesamizdats"]`. Empty, by default. These modules will be loaded ***in addition to*** any autoloaded modules. When you place a module named `dbsamizdat_defs` in a Django app, it will automatically be picked up by DBSamizdat. Think of it as a `models.py`, but for Samizdats. The `DBSAMIZDAT_MODULES` is there for when you want to place some (extra) Samizdat classes elsewhere. Though of course, you could also import those classes from any module into the canonical `dbsamizdat_defs` module.
 
 ### Tips
 
 #### Referencing things nicely
 
 Django allows you to define Model classes that read from a SamizdatView (or SamizdatMaterializedView) rather than a table. For that, set your model's Meta up like so:
```

### Comparing `dbsamizdat-0.9.0b0/README.md` & `dbsamizdat-0.9.0b1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 The blissfully naive PostgreSQL database object manager.
 
 For specifics on integrating with the Django web framework, and some examples for integrating with its ORM, see the [Django integration](#django-integration) section further down.
 
 For discussions, questions, bug reports, feature requests, development, and engaging other users, use the [public mailinglist](https://lists.sr.ht/~nullenenenen/dbsamizdat-discuss).
 
-It requires Python 3.6 or later, and is tested for compatibility with PostgreSQL 9.6 and up.
+It requires Python 3.8 or later, and is tested for compatibility with PostgreSQL 10 and up.
 
 ## What it is
 
 DBSamizdat is a lightweight tool that manages code that lives in the database: **views**, **materialized views**, **functions** and **triggers**, and the dependencies between those and other DB objects.
 
 There is a command-line utility, and a library-style API.
 
@@ -313,14 +313,15 @@
 To use the library API functions, load the `django_api` module rather than the `api` module.
 
 ### Extra configuration
 
 The following Django settings are consulted by DBSamizdat, if declared:
 
 - `DBSAMIZDAT_SMART_MIGRATIONS` — a boolean, `False` by default. This has to do with migrations. As Django's migrations are blissfully unaware of your samizdats, things will fail if, for instance, a table column is removed that one of your views selects. The default lets DBSamizdat assume the worst case, so it will simply remove all its DB state before Django's migrations are run, and restore the state afterwards. But if you define this setting as `True`, DBSamizdat will examine the migration plan and to determine the subset of DB state that will need to be dropped and rebuilt following all the migrations. This behaviour can be desirable when you have large or computationally intensive materialized views. But it's not turned on by default, as it's deemed experimental because of reliance on non-public Django APIs. See if it works for you, if not, turn it back off and send a bug report to the mailinglist!
+- `DBSAMIZDAT_PARALLEL_REFRESH_AFTER_MIGRATIONS` ­— a boolean, `False` by default. After migrations, if any materialized views are (re)created, they need to be populated (the first refresh). This can be done parallelized (same as `dbsamizdat refresh --parallel`). When setting this to `True`, it will also switch the syncing from using the "jumbo" transaction style to "checkpoint".
 - `DBSAMIZDAT_MODULES` — an Iterable[str] of module names, eg `["myapp.somesamizdats"]`. Empty, by default. These modules will be loaded ***in addition to*** any autoloaded modules. When you place a module named `dbsamizdat_defs` in a Django app, it will automatically be picked up by DBSamizdat. Think of it as a `models.py`, but for Samizdats. The `DBSAMIZDAT_MODULES` is there for when you want to place some (extra) Samizdat classes elsewhere. Though of course, you could also import those classes from any module into the canonical `dbsamizdat_defs` module.
 
 ### Tips
 
 #### Referencing things nicely
 
 Django allows you to define Model classes that read from a SamizdatView (or SamizdatMaterializedView) rather than a table. For that, set your model's Meta up like so:
```

### Comparing `dbsamizdat-0.9.0b0/setup.cfg` & `dbsamizdat-0.9.0b1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://hub.sr.ht/~nullenenenen/DBSamizdat/
 keywords = PostgreSQL Django
 license = GPL-3.0+
 license_file = LICENSE.txt
 classifiers = 
-	Development Status :: 4 - Beta
+	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: Developers
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 	Operating System :: OS Independent
 	Topic :: Software Development
 	Topic :: Database
 	Programming Language :: Python :: 3
@@ -25,15 +25,15 @@
 
 [options]
 package_dir = 
 	= src
 packages = 
 	dbsamizdat
 	dbsamizdat.management.commands
-python_requires = >=3.6
+python_requires = >=3.8
 install_requires = 
 	psycopg2 >=2.8.0
 	toposort >=1.5
 zip_safe = True
 include_package_data = True
 
 [options.packages.find]
```

### Comparing `dbsamizdat-0.9.0b0/src/DBSamizdat.egg-info/PKG-INFO` & `dbsamizdat-0.9.0b1/src/DBSamizdat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: DBSamizdat
-Version: 0.9.0b0
+Version: 0.9.0b1
 Summary: dbsamizdat — the blissfully naive PostgreSQL database object manager
 Home-page: https://hub.sr.ht/~nullenenenen/DBSamizdat/
 Author: nullenenenen
 Author-email: nullenenenen@gavagai.eu
 License: GPL-3.0+
 Project-URL: Documentation, https://git.sr.ht/~nullenenenen/DBSamizdat/tree/master/item/README.md
 Project-URL: Source, https://git.sr.ht/~nullenenenen/DBSamizdat/
 Keywords: PostgreSQL Django
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Classifier: Topic :: Database
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: psycopg2>=2.8.0
 Requires-Dist: toposort>=1.5
 
 # DBSamizdat
 
 The blissfully naive PostgreSQL database object manager.
 
 For specifics on integrating with the Django web framework, and some examples for integrating with its ORM, see the [Django integration](#django-integration) section further down.
 
 For discussions, questions, bug reports, feature requests, development, and engaging other users, use the [public mailinglist](https://lists.sr.ht/~nullenenenen/dbsamizdat-discuss).
 
-It requires Python 3.6 or later, and is tested for compatibility with PostgreSQL 9.6 and up.
+It requires Python 3.8 or later, and is tested for compatibility with PostgreSQL 10 and up.
 
 ## What it is
 
 DBSamizdat is a lightweight tool that manages code that lives in the database: **views**, **materialized views**, **functions** and **triggers**, and the dependencies between those and other DB objects.
 
 There is a command-line utility, and a library-style API.
 
@@ -338,14 +338,15 @@
 To use the library API functions, load the `django_api` module rather than the `api` module.
 
 ### Extra configuration
 
 The following Django settings are consulted by DBSamizdat, if declared:
 
 - `DBSAMIZDAT_SMART_MIGRATIONS` — a boolean, `False` by default. This has to do with migrations. As Django's migrations are blissfully unaware of your samizdats, things will fail if, for instance, a table column is removed that one of your views selects. The default lets DBSamizdat assume the worst case, so it will simply remove all its DB state before Django's migrations are run, and restore the state afterwards. But if you define this setting as `True`, DBSamizdat will examine the migration plan and to determine the subset of DB state that will need to be dropped and rebuilt following all the migrations. This behaviour can be desirable when you have large or computationally intensive materialized views. But it's not turned on by default, as it's deemed experimental because of reliance on non-public Django APIs. See if it works for you, if not, turn it back off and send a bug report to the mailinglist!
+- `DBSAMIZDAT_PARALLEL_REFRESH_AFTER_MIGRATIONS` ­— a boolean, `False` by default. After migrations, if any materialized views are (re)created, they need to be populated (the first refresh). This can be done parallelized (same as `dbsamizdat refresh --parallel`). When setting this to `True`, it will also switch the syncing from using the "jumbo" transaction style to "checkpoint".
 - `DBSAMIZDAT_MODULES` — an Iterable[str] of module names, eg `["myapp.somesamizdats"]`. Empty, by default. These modules will be loaded ***in addition to*** any autoloaded modules. When you place a module named `dbsamizdat_defs` in a Django app, it will automatically be picked up by DBSamizdat. Think of it as a `models.py`, but for Samizdats. The `DBSAMIZDAT_MODULES` is there for when you want to place some (extra) Samizdat classes elsewhere. Though of course, you could also import those classes from any module into the canonical `dbsamizdat_defs` module.
 
 ### Tips
 
 #### Referencing things nicely
 
 Django allows you to define Model classes that read from a SamizdatView (or SamizdatMaterializedView) rather than a table. For that, set your model's Meta up like so:
```

### Comparing `dbsamizdat-0.9.0b0/src/DBSamizdat.egg-info/SOURCES.txt` & `dbsamizdat-0.9.0b1/src/DBSamizdat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbsamizdat-0.9.0b0/src/dbsamizdat/api.py` & `dbsamizdat-0.9.0b1/src/dbsamizdat/api.py`

 * *Files identical despite different names*

### Comparing `dbsamizdat-0.9.0b0/src/dbsamizdat/apps.py` & `dbsamizdat-0.9.0b1/src/dbsamizdat/apps.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,27 +11,28 @@
 from .loader import get_samizdats
 from .runner import cmd_sync, cmd_nuke, txstyle, get_cursor
 from .libdb import dbstate_equals_definedstate
 from .util import fqify_node
 
 DBCONN = 'default'  # Only migrations on the default DB connections are supported. For now.
 SMART_MIGRATIONS = getattr(settings, 'DBSAMIZDAT_SMART_MIGRATIONS', False)  # Don't use with custom Operations!
+PARALLEL_REFRESH_AFTER_MIGRATIONS = getattr(settings, 'DBSAMIZDAT_PARALLEL_REFRESH_AFTER_MIGRATIONS', False)
 style = color_style()
 
 
 def get_cmd_args(**kwargs):
     return Namespace(
         printprogress=True,
         verbosity=kwargs['verbosity'],
         dbconn=DBCONN,
-        txdiscipline=txstyle.JUMBO.value,
+        txdiscipline=kwargs.get('txdiscipline', txstyle.JUMBO.value),
         in_django=True,
         samizdatmodules=tuple(),
         log_rather_than_print=not kwargs.get('interactive'),
-        parallel=False,
+        parallel=kwargs.get('parallel', False),
     )
 
 
 def sync(**kwargs):
     cmd_sync(get_cmd_args(**kwargs))
 
 
@@ -106,15 +107,16 @@
     nuke(samizdats=sds_affected, **kwargs)
 
 
 def postmigrate_handler(sender, **kwargs):
     if kwargs['using'] == DBCONN:
         if kwargs.get('interactive'):
             print(style.MIGRATE_HEADING("Syncing DBSamizdat:"))
-        sync(**kwargs)
+        more_kwargs = dict(parallel=True, txdiscipline=txstyle.CHECKPOINT.value) if PARALLEL_REFRESH_AFTER_MIGRATIONS else {}
+        sync(**kwargs, **more_kwargs)
 
 
 class DBSamizdatConfig(AppConfig):
     name = 'dbsamizdat'
 
     def ready(self):
         pre_migrate.connect(premigrate_handler, sender=self)
```

### Comparing `dbsamizdat-0.9.0b0/src/dbsamizdat/django_api.py` & `dbsamizdat-0.9.0b1/src/dbsamizdat/django_api.py`

 * *Files identical despite different names*

### Comparing `dbsamizdat-0.9.0b0/src/dbsamizdat/exceptions.py` & `dbsamizdat-0.9.0b1/src/dbsamizdat/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbsamizdat-0.9.0b0/src/dbsamizdat/graphvizdot.py` & `dbsamizdat-0.9.0b1/src/dbsamizdat/graphvizdot.py`

 * *Files identical despite different names*

### Comparing `dbsamizdat-0.9.0b0/src/dbsamizdat/libdb.py` & `dbsamizdat-0.9.0b1/src/dbsamizdat/libdb.py`

 * *Files identical despite different names*

### Comparing `dbsamizdat-0.9.0b0/src/dbsamizdat/libgraph.py` & `dbsamizdat-0.9.0b1/src/dbsamizdat/libgraph.py`

 * *Files identical despite different names*

### Comparing `dbsamizdat-0.9.0b0/src/dbsamizdat/loader.py` & `dbsamizdat-0.9.0b1/src/dbsamizdat/loader.py`

 * *Files identical despite different names*

### Comparing `dbsamizdat-0.9.0b0/src/dbsamizdat/management/commands/dbsamizdat.py` & `dbsamizdat-0.9.0b1/src/dbsamizdat/management/commands/dbsamizdat.py`

 * *Files identical despite different names*

### Comparing `dbsamizdat-0.9.0b0/src/dbsamizdat/runner.py` & `dbsamizdat-0.9.0b1/src/dbsamizdat/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,27 +166,29 @@
     if excess_dbstate:
         def drops():
             for sd in excess_dbstate:
                 yield 'drop', sd, sd.drop(if_exists=True)  # we don't know the deptree; so they may have vanished through a cascading drop of a previous object
         drain(executor(drops(), args, cursor))
         issame, excess_dbstate, excess_definedstate = dbstate_equals_definedstate(cursor, samizdats)  # again, we don't know the in-db deptree, so we need to re-read DB state as the rug may have been pulled out from under us with cascading drops
     if excess_definedstate:
+        matviews_to_refresh = []
         def creates():
             to_create_ids = {sd.head_id() for sd in excess_definedstate}
             for sd in samizdats:  # iterate in proper creation order
                 if sd.head_id() in to_create_ids:
                     yield 'create', sd, sd.create()
                     yield 'sign', sd, sd.sign(cursor)
+                    if sd.entity_type == entitypes.MATVIEW:
+                        matviews_to_refresh.append(sd)  # queue to populate this matview later
         drain(executor(creates(), args, cursor))
 
         def refreshes(subjects):
             for sd in subjects:
                 yield 'refresh', sd, sd.refresh(concurrent_allowed=False)
 
-        matviews_to_refresh = {sd for sd in excess_definedstate if sd.entity_type == entitypes.MATVIEW}
         if matviews_to_refresh:
             drain = get_executor_drainer(args, max_namelen=max_namelen, parallel=args.parallel)
             if args.parallel:
                 firstlevel, parallelization_callback = prep_refresh_parallel(samizdats, matviews_to_refresh, refreshes)
                 drain(executor(refreshes(firstlevel), args, None, parallelization_callback=parallelization_callback))
             else:
                 drain(executor(refreshes(matviews_to_refresh), args, cursor))
```

### Comparing `dbsamizdat-0.9.0b0/src/dbsamizdat/samizdat.py` & `dbsamizdat-0.9.0b1/src/dbsamizdat/samizdat.py`

 * *Files identical despite different names*

### Comparing `dbsamizdat-0.9.0b0/src/dbsamizdat/test_samizdats.py` & `dbsamizdat-0.9.0b1/src/dbsamizdat/test_samizdats.py`

 * *Files identical despite different names*

### Comparing `dbsamizdat-0.9.0b0/src/dbsamizdat/util.py` & `dbsamizdat-0.9.0b1/src/dbsamizdat/util.py`

 * *Files identical despite different names*

