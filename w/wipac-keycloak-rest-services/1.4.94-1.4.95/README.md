# Comparing `tmp/wipac-keycloak-rest-services-1.4.94.tar.gz` & `tmp/wipac-keycloak-rest-services-1.4.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wipac-keycloak-rest-services-1.4.94.tar", last modified: Tue May 28 19:19:31 2024, max compression
+gzip compressed data, was "wipac-keycloak-rest-services-1.4.95.tar", last modified: Fri May 31 16:03:39 2024, max compression
```

## Comparing `wipac-keycloak-rest-services-1.4.94.tar` & `wipac-keycloak-rest-services-1.4.95.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:19:31.627619 wipac-keycloak-rest-services-1.4.94/
--rw-r--r--   0 root         (0) root         (0)     1103 2024-05-28 19:19:28.000000 wipac-keycloak-rest-services-1.4.94/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4149 2024-05-28 19:19:31.627619 wipac-keycloak-rest-services-1.4.94/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3139 2024-05-28 19:19:28.000000 wipac-keycloak-rest-services-1.4.94/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:19:31.623619 wipac-keycloak-rest-services-1.4.94/krs/
--rw-r--r--   0 root         (0) root         (0)      514 2024-05-28 19:19:29.000000 wipac-keycloak-rest-services-1.4.94/krs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20266 2024-05-28 19:19:28.000000 wipac-keycloak-rest-services-1.4.94/krs/apps.py
--rw-r--r--   0 root         (0) root         (0)    16594 2024-05-28 19:19:28.000000 wipac-keycloak-rest-services-1.4.94/krs/bootstrap.py
--rw-r--r--   0 root         (0) root         (0)     3307 2024-05-28 19:19:28.000000 wipac-keycloak-rest-services-1.4.94/krs/email.py
--rw-r--r--   0 root         (0) root         (0)    16899 2024-05-28 19:19:28.000000 wipac-keycloak-rest-services-1.4.94/krs/groups.py
--rw-r--r--   0 root         (0) root         (0)     9038 2024-05-28 19:19:28.000000 wipac-keycloak-rest-services-1.4.94/krs/institutions.py
--rw-r--r--   0 root         (0) root         (0)    22784 2024-05-28 19:19:28.000000 wipac-keycloak-rest-services-1.4.94/krs/ldap.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 19:19:28.000000 wipac-keycloak-rest-services-1.4.94/krs/py.typed
--rw-r--r--   0 root         (0) root         (0)     5722 2024-05-28 19:19:28.000000 wipac-keycloak-rest-services-1.4.94/krs/rabbitmq.py
--rw-r--r--   0 root         (0) root         (0)     2917 2024-05-28 19:19:28.000000 wipac-keycloak-rest-services-1.4.94/krs/token.py
--rw-r--r--   0 root         (0) root         (0)     9039 2024-05-28 19:19:28.000000 wipac-keycloak-rest-services-1.4.94/krs/users.py
--rw-r--r--   0 root         (0) root         (0)     1525 2024-05-28 19:19:28.000000 wipac-keycloak-rest-services-1.4.94/krs/util.py
--rw-r--r--   0 root         (0) root         (0)     2313 2024-05-28 19:19:31.627619 wipac-keycloak-rest-services-1.4.94/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      104 2024-05-28 19:19:28.000000 wipac-keycloak-rest-services-1.4.94/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:19:31.623619 wipac-keycloak-rest-services-1.4.94/wipac_keycloak_rest_services.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4149 2024-05-28 19:19:31.000000 wipac-keycloak-rest-services-1.4.94/wipac_keycloak_rest_services.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      466 2024-05-28 19:19:31.000000 wipac-keycloak-rest-services-1.4.94/wipac_keycloak_rest_services.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 19:19:31.000000 wipac-keycloak-rest-services-1.4.94/wipac_keycloak_rest_services.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      228 2024-05-28 19:19:31.000000 wipac-keycloak-rest-services-1.4.94/wipac_keycloak_rest_services.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2024-05-28 19:19:31.000000 wipac-keycloak-rest-services-1.4.94/wipac_keycloak_rest_services.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 16:03:39.413810 wipac-keycloak-rest-services-1.4.95/
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-05-31 16:03:35.000000 wipac-keycloak-rest-services-1.4.95/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4149 2024-05-31 16:03:39.413810 wipac-keycloak-rest-services-1.4.95/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3139 2024-05-31 16:03:35.000000 wipac-keycloak-rest-services-1.4.95/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 16:03:39.409810 wipac-keycloak-rest-services-1.4.95/krs/
+-rw-r--r--   0 root         (0) root         (0)      514 2024-05-31 16:03:36.000000 wipac-keycloak-rest-services-1.4.95/krs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20266 2024-05-31 16:03:35.000000 wipac-keycloak-rest-services-1.4.95/krs/apps.py
+-rw-r--r--   0 root         (0) root         (0)    16594 2024-05-31 16:03:35.000000 wipac-keycloak-rest-services-1.4.95/krs/bootstrap.py
+-rw-r--r--   0 root         (0) root         (0)     3307 2024-05-31 16:03:35.000000 wipac-keycloak-rest-services-1.4.95/krs/email.py
+-rw-r--r--   0 root         (0) root         (0)    16899 2024-05-31 16:03:35.000000 wipac-keycloak-rest-services-1.4.95/krs/groups.py
+-rw-r--r--   0 root         (0) root         (0)     9038 2024-05-31 16:03:35.000000 wipac-keycloak-rest-services-1.4.95/krs/institutions.py
+-rw-r--r--   0 root         (0) root         (0)    22784 2024-05-31 16:03:35.000000 wipac-keycloak-rest-services-1.4.95/krs/ldap.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 16:03:35.000000 wipac-keycloak-rest-services-1.4.95/krs/py.typed
+-rw-r--r--   0 root         (0) root         (0)     5722 2024-05-31 16:03:35.000000 wipac-keycloak-rest-services-1.4.95/krs/rabbitmq.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2024-05-31 16:03:35.000000 wipac-keycloak-rest-services-1.4.95/krs/token.py
+-rw-r--r--   0 root         (0) root         (0)     9039 2024-05-31 16:03:35.000000 wipac-keycloak-rest-services-1.4.95/krs/users.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2024-05-31 16:03:35.000000 wipac-keycloak-rest-services-1.4.95/krs/util.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2024-05-31 16:03:39.413810 wipac-keycloak-rest-services-1.4.95/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      104 2024-05-31 16:03:35.000000 wipac-keycloak-rest-services-1.4.95/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 16:03:39.413810 wipac-keycloak-rest-services-1.4.95/wipac_keycloak_rest_services.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4149 2024-05-31 16:03:39.000000 wipac-keycloak-rest-services-1.4.95/wipac_keycloak_rest_services.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      466 2024-05-31 16:03:39.000000 wipac-keycloak-rest-services-1.4.95/wipac_keycloak_rest_services.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 16:03:39.000000 wipac-keycloak-rest-services-1.4.95/wipac_keycloak_rest_services.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      228 2024-05-31 16:03:39.000000 wipac-keycloak-rest-services-1.4.95/wipac_keycloak_rest_services.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2024-05-31 16:03:39.000000 wipac-keycloak-rest-services-1.4.95/wipac_keycloak_rest_services.egg-info/top_level.txt
```

### Comparing `wipac-keycloak-rest-services-1.4.94/LICENSE` & `wipac-keycloak-rest-services-1.4.95/LICENSE`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.94/PKG-INFO` & `wipac-keycloak-rest-services-1.4.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-keycloak-rest-services
-Version: 1.4.94
+Version: 1.4.95
 Summary: Services surrounding KeyCloak, that use the REST API to read/update state
 Home-page: https://github.com/WIPACrepo/keycloak-rest-services
 Download-URL: https://pypi.org/project/wipac-keycloak-rest-services/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/keycloak-rest-services/issues
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_dvkrj4l9_/tmpyadb4l7j_TarContainer/0/2", line 94, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wipac-keycloak-rest-services Version: 1.4.94
+Metadata-Version: 2.1 Name: wipac-keycloak-rest-services Version: 1.4.95
 Summary: Services surrounding KeyCloak, that use the REST API to read/update
 state Home-page: https://github.com/WIPACrepo/keycloak-rest-services Download-
 URL: https://pypi.org/project/wipac-keycloak-rest-services/ Author: WIPAC
 Developers Author-email: developers@icecube.wisc.edu License: MIT Project-URL:
 Tracker, https://github.com/WIPACrepo/keycloak-rest-services/issues Project-
 URL: Source, https://github.com/WIPACrepo/keycloak-rest-services Keywords:
 keycloak,rest,tools,utilities Classifier: Development Status :: 5 - Production/
```

### Comparing `wipac-keycloak-rest-services-1.4.94/README.md` & `wipac-keycloak-rest-services-1.4.95/README.md`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.94/krs/__init__.py` & `wipac-keycloak-rest-services-1.4.95/krs/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "1.4.94"
+__version__ = "1.4.95"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `wipac-keycloak-rest-services-1.4.94/krs/apps.py` & `wipac-keycloak-rest-services-1.4.95/krs/apps.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.94/krs/bootstrap.py` & `wipac-keycloak-rest-services-1.4.95/krs/bootstrap.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.94/krs/email.py` & `wipac-keycloak-rest-services-1.4.95/krs/email.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.94/krs/groups.py` & `wipac-keycloak-rest-services-1.4.95/krs/groups.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.94/krs/institutions.py` & `wipac-keycloak-rest-services-1.4.95/krs/institutions.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.94/krs/ldap.py` & `wipac-keycloak-rest-services-1.4.95/krs/ldap.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.94/krs/rabbitmq.py` & `wipac-keycloak-rest-services-1.4.95/krs/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.94/krs/token.py` & `wipac-keycloak-rest-services-1.4.95/krs/token.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.94/krs/users.py` & `wipac-keycloak-rest-services-1.4.95/krs/users.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.94/krs/util.py` & `wipac-keycloak-rest-services-1.4.95/krs/util.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.94/setup.cfg` & `wipac-keycloak-rest-services-1.4.95/setup.cfg`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.94/wipac_keycloak_rest_services.egg-info/PKG-INFO` & `wipac-keycloak-rest-services-1.4.95/wipac_keycloak_rest_services.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-keycloak-rest-services
-Version: 1.4.94
+Version: 1.4.95
 Summary: Services surrounding KeyCloak, that use the REST API to read/update state
 Home-page: https://github.com/WIPACrepo/keycloak-rest-services
 Download-URL: https://pypi.org/project/wipac-keycloak-rest-services/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/keycloak-rest-services/issues
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_dvkrj4l9_/tmpyadb4l7j_TarContainer/0/20", line 94, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wipac-keycloak-rest-services Version: 1.4.94
+Metadata-Version: 2.1 Name: wipac-keycloak-rest-services Version: 1.4.95
 Summary: Services surrounding KeyCloak, that use the REST API to read/update
 state Home-page: https://github.com/WIPACrepo/keycloak-rest-services Download-
 URL: https://pypi.org/project/wipac-keycloak-rest-services/ Author: WIPAC
 Developers Author-email: developers@icecube.wisc.edu License: MIT Project-URL:
 Tracker, https://github.com/WIPACrepo/keycloak-rest-services/issues Project-
 URL: Source, https://github.com/WIPACrepo/keycloak-rest-services Keywords:
 keycloak,rest,tools,utilities Classifier: Development Status :: 5 - Production/
```

