# Comparing `tmp/pyguardpoint-1.3.9.tar.gz` & `tmp/pyguardpoint-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyguardpoint-1.3.9.tar", last modified: Tue May 28 15:02:25 2024, max compression
+gzip compressed data, was "pyguardpoint-1.4.0.tar", last modified: Fri May 31 10:38:24 2024, max compression
```

## Comparing `pyguardpoint-1.3.9.tar` & `pyguardpoint-1.4.0.tar`

### file list

```diff
@@ -1,52 +1,56 @@
-drwxr-xr-x   0 johnowen   (501) staff       (20)        0 2024-05-28 15:02:25.141089 pyguardpoint-1.3.9/
--rw-r--r--   0 johnowen   (501) staff       (20)    11357 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/LICENSE.txt
--rw-r--r--   0 johnowen   (501) staff       (20)     8038 2024-05-28 15:02:25.140885 pyguardpoint-1.3.9/PKG-INFO
--rw-r--r--   0 johnowen   (501) staff       (20)     7658 2024-05-28 14:59:56.000000 pyguardpoint-1.3.9/README.rst
-drwxr-xr-x   0 johnowen   (501) staff       (20)        0 2024-05-28 15:02:25.137862 pyguardpoint-1.3.9/pyGuardPoint/
--rw-r--r--   0 johnowen   (501) staff       (20)     8613 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/CustomWebsocketTransport.py
--rw-r--r--   0 johnowen   (501) staff       (20)      342 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/__init__.py
--rw-r--r--   0 johnowen   (501) staff       (20)     1251 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_areas.py
--rw-r--r--   0 johnowen   (501) staff       (20)    11501 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_cardholders.py
--rw-r--r--   0 johnowen   (501) staff       (20)     1340 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_cardholdertypes.py
--rw-r--r--   0 johnowen   (501) staff       (20)     6824 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_cards.py
--rw-r--r--   0 johnowen   (501) staff       (20)     2429 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_controllers.py
--rw-r--r--   0 johnowen   (501) staff       (20)     1302 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_customizedfields.py
--rw-r--r--   0 johnowen   (501) staff       (20)     1860 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_diagnostic.py
--rw-r--r--   0 johnowen   (501) staff       (20)     3857 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_ouputs.py
--rw-r--r--   0 johnowen   (501) staff       (20)     1328 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_personaldetails.py
--rw-r--r--   0 johnowen   (501) staff       (20)     2292 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_readers.py
--rw-r--r--   0 johnowen   (501) staff       (20)     2763 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_scheduledmags.py
--rw-r--r--   0 johnowen   (501) staff       (20)     1524 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_securitygroups.py
--rw-r--r--   0 johnowen   (501) staff       (20)     5432 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/_odata_filter.py
--rw-r--r--   0 johnowen   (501) staff       (20)     1566 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/_str_match_algo.py
-drwxr-xr-x   0 johnowen   (501) staff       (20)        0 2024-05-28 15:02:25.140480 pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/
--rw-r--r--   0 johnowen   (501) staff       (20)        0 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/__init__.py
--rw-r--r--   0 johnowen   (501) staff       (20)     1266 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_areas.py
--rw-r--r--   0 johnowen   (501) staff       (20)    11647 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_cardholders.py
--rw-r--r--   0 johnowen   (501) staff       (20)     1355 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_cardholdertypes.py
--rw-r--r--   0 johnowen   (501) staff       (20)     6900 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_cards.py
--rw-r--r--   0 johnowen   (501) staff       (20)     2527 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_controllers.py
--rw-r--r--   0 johnowen   (501) staff       (20)     1317 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_customizedfields.py
--rw-r--r--   0 johnowen   (501) staff       (20)     1873 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_diagnostic.py
--rw-r--r--   0 johnowen   (501) staff       (20)     3862 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_ouputs.py
--rw-r--r--   0 johnowen   (501) staff       (20)     1343 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_personaldetails.py
--rw-r--r--   0 johnowen   (501) staff       (20)     2319 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_readers.py
--rw-r--r--   0 johnowen   (501) staff       (20)     2763 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_scheduledmags.py
--rw-r--r--   0 johnowen   (501) staff       (20)     1524 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_securitygroups.py
--rw-r--r--   0 johnowen   (501) staff       (20)    12795 2024-05-28 14:49:38.000000 pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/guardpoint_connection_asyncio.py
--rw-r--r--   0 johnowen   (501) staff       (20)     4984 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/guardpoint.py
--rw-r--r--   0 johnowen   (501) staff       (20)     4733 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/guardpoint_asyncio.py
--rw-r--r--   0 johnowen   (501) staff       (20)    11293 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/guardpoint_connection.py
--rw-r--r--   0 johnowen   (501) staff       (20)    20954 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/guardpoint_dataclasses.py
--rw-r--r--   0 johnowen   (501) staff       (20)       97 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/guardpoint_error.py
--rw-r--r--   0 johnowen   (501) staff       (20)     3982 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/guardpoint_threaded.py
--rw-r--r--   0 johnowen   (501) staff       (20)     4245 2024-03-13 09:54:42.000000 pyguardpoint-1.3.9/pyGuardPoint/guardpoint_utils.py
-drwxr-xr-x   0 johnowen   (501) staff       (20)        0 2024-05-28 15:02:25.140677 pyguardpoint-1.3.9/pyGuardPoint.egg-info/
--rw-r--r--   0 johnowen   (501) staff       (20)     8038 2024-05-28 15:02:25.000000 pyguardpoint-1.3.9/pyGuardPoint.egg-info/PKG-INFO
--rw-r--r--   0 johnowen   (501) staff       (20)     1863 2024-05-28 15:02:25.000000 pyguardpoint-1.3.9/pyGuardPoint.egg-info/SOURCES.txt
--rw-r--r--   0 johnowen   (501) staff       (20)        1 2024-05-28 15:02:25.000000 pyguardpoint-1.3.9/pyGuardPoint.egg-info/dependency_links.txt
--rw-r--r--   0 johnowen   (501) staff       (20)        1 2024-05-28 15:02:25.000000 pyguardpoint-1.3.9/pyGuardPoint.egg-info/not-zip-safe
--rw-r--r--   0 johnowen   (501) staff       (20)       56 2024-05-28 15:02:25.000000 pyguardpoint-1.3.9/pyGuardPoint.egg-info/requires.txt
--rw-r--r--   0 johnowen   (501) staff       (20)       13 2024-05-28 15:02:25.000000 pyguardpoint-1.3.9/pyGuardPoint.egg-info/top_level.txt
--rw-r--r--   0 johnowen   (501) staff       (20)       38 2024-05-28 15:02:25.141128 pyguardpoint-1.3.9/setup.cfg
--rw-r--r--   0 johnowen   (501) staff       (20)      610 2024-05-28 14:36:57.000000 pyguardpoint-1.3.9/setup.py
+drwxr-xr-x   0 johnowen   (501) staff       (20)        0 2024-05-31 10:38:24.656224 pyguardpoint-1.4.0/
+-rw-r--r--   0 johnowen   (501) staff       (20)    11357 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/LICENSE.txt
+-rw-r--r--   0 johnowen   (501) staff       (20)    10657 2024-05-31 10:38:24.656036 pyguardpoint-1.4.0/PKG-INFO
+-rw-r--r--   0 johnowen   (501) staff       (20)    10243 2024-05-31 10:37:48.000000 pyguardpoint-1.4.0/README.rst
+drwxr-xr-x   0 johnowen   (501) staff       (20)        0 2024-05-31 10:38:24.651833 pyguardpoint-1.4.0/pyGuardPoint/
+-rw-r--r--   0 johnowen   (501) staff       (20)     8613 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/CustomWebsocketTransport.py
+-rw-r--r--   0 johnowen   (501) staff       (20)      342 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/__init__.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     2361 2024-05-30 09:25:35.000000 pyguardpoint-1.4.0/pyGuardPoint/_guardpoint_alarms.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1251 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/_guardpoint_areas.py
+-rw-r--r--   0 johnowen   (501) staff       (20)    11501 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/_guardpoint_cardholders.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1340 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/_guardpoint_cardholdertypes.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     6824 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/_guardpoint_cards.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     2429 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/_guardpoint_controllers.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1302 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/_guardpoint_customizedfields.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1860 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/_guardpoint_diagnostic.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     3016 2024-05-31 10:23:30.000000 pyguardpoint-1.4.0/pyGuardPoint/_guardpoint_events.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     3857 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/_guardpoint_ouputs.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1328 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/_guardpoint_personaldetails.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     2292 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/_guardpoint_readers.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     2763 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/_guardpoint_scheduledmags.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1524 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/_guardpoint_securitygroups.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     5432 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/_odata_filter.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1566 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/_str_match_algo.py
+drwxr-xr-x   0 johnowen   (501) staff       (20)        0 2024-05-31 10:38:24.655514 pyguardpoint-1.4.0/pyGuardPoint/gp_asyncio/
+-rw-r--r--   0 johnowen   (501) staff       (20)        0 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/gp_asyncio/__init__.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     2388 2024-05-30 09:17:55.000000 pyguardpoint-1.4.0/pyGuardPoint/gp_asyncio/_async_guardpoint_alarms.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1266 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/gp_asyncio/_async_guardpoint_areas.py
+-rw-r--r--   0 johnowen   (501) staff       (20)    11647 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/gp_asyncio/_async_guardpoint_cardholders.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1355 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/gp_asyncio/_async_guardpoint_cardholdertypes.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     6900 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/gp_asyncio/_async_guardpoint_cards.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     2527 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/gp_asyncio/_async_guardpoint_controllers.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1317 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/gp_asyncio/_async_guardpoint_customizedfields.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1873 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/gp_asyncio/_async_guardpoint_diagnostic.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     3043 2024-05-31 10:17:21.000000 pyguardpoint-1.4.0/pyGuardPoint/gp_asyncio/_async_guardpoint_events.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     3862 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/gp_asyncio/_async_guardpoint_ouputs.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1343 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/gp_asyncio/_async_guardpoint_personaldetails.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     2317 2024-05-30 09:17:55.000000 pyguardpoint-1.4.0/pyGuardPoint/gp_asyncio/_async_guardpoint_readers.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     2763 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/gp_asyncio/_async_guardpoint_scheduledmags.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     1524 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/gp_asyncio/_async_guardpoint_securitygroups.py
+-rw-r--r--   0 johnowen   (501) staff       (20)    12795 2024-05-28 14:49:38.000000 pyguardpoint-1.4.0/pyGuardPoint/gp_asyncio/guardpoint_connection_asyncio.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     5090 2024-05-31 10:24:48.000000 pyguardpoint-1.4.0/pyGuardPoint/guardpoint.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     4873 2024-05-30 09:36:02.000000 pyguardpoint-1.4.0/pyGuardPoint/guardpoint_asyncio.py
+-rw-r--r--   0 johnowen   (501) staff       (20)    11293 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/guardpoint_connection.py
+-rw-r--r--   0 johnowen   (501) staff       (20)    23894 2024-05-31 10:17:21.000000 pyguardpoint-1.4.0/pyGuardPoint/guardpoint_dataclasses.py
+-rw-r--r--   0 johnowen   (501) staff       (20)       97 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/guardpoint_error.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     3982 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/guardpoint_threaded.py
+-rw-r--r--   0 johnowen   (501) staff       (20)     4245 2024-03-13 09:54:42.000000 pyguardpoint-1.4.0/pyGuardPoint/guardpoint_utils.py
+drwxr-xr-x   0 johnowen   (501) staff       (20)        0 2024-05-31 10:38:24.655845 pyguardpoint-1.4.0/pyGuardPoint.egg-info/
+-rw-r--r--   0 johnowen   (501) staff       (20)    10657 2024-05-31 10:38:24.000000 pyguardpoint-1.4.0/pyGuardPoint.egg-info/PKG-INFO
+-rw-r--r--   0 johnowen   (501) staff       (20)     2037 2024-05-31 10:38:24.000000 pyguardpoint-1.4.0/pyGuardPoint.egg-info/SOURCES.txt
+-rw-r--r--   0 johnowen   (501) staff       (20)        1 2024-05-31 10:38:24.000000 pyguardpoint-1.4.0/pyGuardPoint.egg-info/dependency_links.txt
+-rw-r--r--   0 johnowen   (501) staff       (20)        1 2024-05-28 15:02:25.000000 pyguardpoint-1.4.0/pyGuardPoint.egg-info/not-zip-safe
+-rw-r--r--   0 johnowen   (501) staff       (20)       75 2024-05-31 10:38:24.000000 pyguardpoint-1.4.0/pyGuardPoint.egg-info/requires.txt
+-rw-r--r--   0 johnowen   (501) staff       (20)       13 2024-05-31 10:38:24.000000 pyguardpoint-1.4.0/pyGuardPoint.egg-info/top_level.txt
+-rw-r--r--   0 johnowen   (501) staff       (20)       38 2024-05-31 10:38:24.656257 pyguardpoint-1.4.0/setup.cfg
+-rw-r--r--   0 johnowen   (501) staff       (20)      632 2024-05-31 10:31:30.000000 pyguardpoint-1.4.0/setup.py
```

### Comparing `pyguardpoint-1.3.9/LICENSE.txt` & `pyguardpoint-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/PKG-INFO` & `pyguardpoint-1.4.0/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: pyGuardPoint
-Version: 1.3.9
-Summary: Python wrapper for GuardPoint 10 Access Control System
-Author: John Owen
-Maintainer-email: sales@sensoraccess.co.uk
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: validators
-Requires-Dist: fuzzywuzzy
-Requires-Dist: cryptography
-Requires-Dist: pysignalr
-Requires-Dist: websockets
-
 pyGuardPoint
 ===============
 
 pyGuardPoint is a Python wrapper for the GuardPoint 10 API, which allows developers to easily integrate with the GuardPoint 10 physical access control system (ACS).
 
 pyGuardPoint aims to provide a pythonic OOP style programming interface to the WebAPI of GuardPoint 10 (GP10), perfect for quickly building proof-of-concepts.
 GuardPoint 10 controls and monitors doors,lifts,readers etc. pyGuardPoint currently focuses more on the management of Cardholders over the monitoring and setup of the physical infrastructure.
@@ -108,16 +94,14 @@
     cardholder.pretty_print()   # Print nicely in the terminal window
 
 To get a list of areas/zones, and count the number of cardholders in each:
 
     gp = GuardPoint(host="sensoraccess.duckdns.org", pwd="password")
 
     areas = gp.get_areas()
-
-    areas = gp.get_areas()
     for area in areas:
         cardholder_count = gp.get_card_holders(count=True, areas=area)
         print(f"Cardholders in {area.name} = {str(cardholder_count)}")
 
 To get a list of security groups:
 
     sec_groups = gp.get_security_groups()
@@ -138,14 +122,79 @@
                       toDateValid=toDateValid)
     gp.add_scheduled_mag(sm)
 
     scheduled_mags = gp.get_scheduled_mags()
     for scheduled_mag in scheduled_mags:
         print(scheduled_mag)
 
+Complete example script using GuardPointAsyncIO to get Access followed by Alarm Events:
+
+    from pyGuardPoint_Build.pyGuardPoint import GuardPointAsyncIO, GuardPointError, GuardPointUnauthorized
+
+    # GuardPoint
+    GP_HOST = 'https://sensoraccess.duckdns.org'
+    # GP_HOST = 'http://localhost/'
+    GP_USER = 'admin'
+    GP_PASS = 'admin'
+    # TLS/SSL secure connection
+    TLS_P12 = "/Users/johnowen/Downloads/MobileGuardDefault.p12"
+    #TLS_P12 = "C:\\Users\\john_\\OneDrive\\Desktop\\MobGuardDefault\\MobileGuardDefault.p12"
+    TLS_P12_PWD = "test"
+
+    if __name__ == "__main__":
+        py_gp_version = version("pyGuardPoint")
+        print("pyGuardPoint Version:" + py_gp_version)
+        py_gp_version_int = int(py_gp_version.replace('.', ''))
+        if py_gp_version_int < 138:
+            print("Please Update pyGuardPoint")
+            print("\t (Within a Terminal Window) Run > 'pip install pyGuardPoint --upgrade'")
+            exit()
+
+        logging.basicConfig(level=logging.DEBUG)
+
+        async def main():
+            gp = GuardPointAsyncIO(host=GP_HOST,
+                                   username=GP_USER,
+                                   pwd=GP_PASS,
+                                   p12_file=TLS_P12,
+                                   p12_pwd=TLS_P12_PWD)
+
+            print(f"\n********* Get Access Events **********")
+            access_events = await gp.get_access_events(limit=3, offset=0)
+
+            for access_event in access_events:
+                print(f"\nAccessEvent:")
+                print(f"\tType: {access_event.type}")
+                print(f"\tjournalUpdateDateTime: {access_event.journalUpdateDateTime}")
+                print(f"\tdateTime: {access_event.dateTime}")
+                print(f"\taccessDeniedCode: {access_event.accessDeniedCode}")
+                print(f"\tisPastEvent: {access_event.isPastEvent}")
+
+            print(f"\n\n********* Get Alarm Events **********")
+            alarm_events = await gp.get_alarm_events(limit=3, offset=0)
+
+            for alarm_event in alarm_events:
+                print(f"\nAlarmEvent:")
+                print(f"\tType: {alarm_event.type}")
+                print(f"\tjournalUpdateDateTime: {alarm_event.journalUpdateDateTime}")
+                print(f"\tdateTime: {alarm_event.dateTime}")
+
+            await gp.close()
+
+        try:
+            asyncio.run(main())
+        except GuardPointError as e:
+            print(f"GuardPointError: {e}")
+        except GuardPointUnauthorized as e:
+            print(f"GuardPointUnauthorized: {e}")
+        except Exception as e:
+            print(f"Exception: {e}")
+
+
+
 GuardPoint servers can be setup with a Signal-R service enabled.
 Once enabled the server will broadcast events to clients listening to events.
 
     try:
         gp = GuardPoint(host=GP_HOST,
                         username=GP_USER,
                         pwd=GP_PASS,
@@ -182,8 +231,8 @@
         print(f"SignalR AuthorizationError")
     except Exception as e:
         print(f"Exception: {str(e)}")
 
 More
 ------------------
 
-The code and further examples can be found at https://github.com/SensorAccess/pyGuardPoint
+The code and further examples can be found at https://github.com/SensorAccess/pyGuardPoint
```

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/CustomWebsocketTransport.py` & `pyguardpoint-1.4.0/pyGuardPoint/CustomWebsocketTransport.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_areas.py` & `pyguardpoint-1.4.0/pyGuardPoint/_guardpoint_areas.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_cardholders.py` & `pyguardpoint-1.4.0/pyGuardPoint/_guardpoint_cardholders.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_cardholdertypes.py` & `pyguardpoint-1.4.0/pyGuardPoint/_guardpoint_cardholdertypes.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_cards.py` & `pyguardpoint-1.4.0/pyGuardPoint/_guardpoint_cards.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_controllers.py` & `pyguardpoint-1.4.0/pyGuardPoint/_guardpoint_controllers.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_customizedfields.py` & `pyguardpoint-1.4.0/pyGuardPoint/_guardpoint_customizedfields.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_diagnostic.py` & `pyguardpoint-1.4.0/pyGuardPoint/_guardpoint_diagnostic.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_ouputs.py` & `pyguardpoint-1.4.0/pyGuardPoint/_guardpoint_ouputs.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_personaldetails.py` & `pyguardpoint-1.4.0/pyGuardPoint/_guardpoint_personaldetails.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_readers.py` & `pyguardpoint-1.4.0/pyGuardPoint/_guardpoint_readers.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_scheduledmags.py` & `pyguardpoint-1.4.0/pyGuardPoint/_guardpoint_scheduledmags.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/_guardpoint_securitygroups.py` & `pyguardpoint-1.4.0/pyGuardPoint/_guardpoint_securitygroups.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/_odata_filter.py` & `pyguardpoint-1.4.0/pyGuardPoint/_odata_filter.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/_str_match_algo.py` & `pyguardpoint-1.4.0/pyGuardPoint/_str_match_algo.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_areas.py` & `pyguardpoint-1.4.0/pyGuardPoint/gp_asyncio/_async_guardpoint_areas.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_cardholders.py` & `pyguardpoint-1.4.0/pyGuardPoint/gp_asyncio/_async_guardpoint_cardholders.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_cardholdertypes.py` & `pyguardpoint-1.4.0/pyGuardPoint/gp_asyncio/_async_guardpoint_cardholdertypes.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_cards.py` & `pyguardpoint-1.4.0/pyGuardPoint/gp_asyncio/_async_guardpoint_cards.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_controllers.py` & `pyguardpoint-1.4.0/pyGuardPoint/gp_asyncio/_async_guardpoint_controllers.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_customizedfields.py` & `pyguardpoint-1.4.0/pyGuardPoint/gp_asyncio/_async_guardpoint_customizedfields.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_diagnostic.py` & `pyguardpoint-1.4.0/pyGuardPoint/gp_asyncio/_async_guardpoint_diagnostic.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_ouputs.py` & `pyguardpoint-1.4.0/pyGuardPoint/gp_asyncio/_async_guardpoint_ouputs.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_personaldetails.py` & `pyguardpoint-1.4.0/pyGuardPoint/gp_asyncio/_async_guardpoint_personaldetails.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_readers.py` & `pyguardpoint-1.4.0/pyGuardPoint/gp_asyncio/_async_guardpoint_readers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import validators
 from ..guardpoint_utils import GuardPointResponse
 from ..guardpoint_dataclasses import Reader
 from ..guardpoint_error import GuardPointError, GuardPointUnauthorized
 
 
 class ReadersAPI:
-    async def get_readers(self, ):
+    async def get_readers(self):
         url = "/odata/API_Readers"
         headers = {
             'Content-Type': 'application/json',
             'Accept': 'application/json'
         }
 
         code, json_body = await self.gp_json_query("GET", headers=headers, url=url)
```

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_scheduledmags.py` & `pyguardpoint-1.4.0/pyGuardPoint/gp_asyncio/_async_guardpoint_scheduledmags.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/_async_guardpoint_securitygroups.py` & `pyguardpoint-1.4.0/pyGuardPoint/gp_asyncio/_async_guardpoint_securitygroups.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/gp_asyncio/guardpoint_connection_asyncio.py` & `pyguardpoint-1.4.0/pyGuardPoint/gp_asyncio/guardpoint_connection_asyncio.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/guardpoint.py` & `pyguardpoint-1.4.0/pyGuardPoint/guardpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import asyncio
 import logging
 
 from pysignalr.client import SignalRClient
 
 from .CustomWebsocketTransport import CustomWebsocketTransport, DEFAULT_PING_INTERVAL, DEFAULT_CONNECTION_TIMEOUT, \
     DEFAULT_MAX_SIZE
+from ._guardpoint_alarms import AlarmsAPI
 from ._guardpoint_cardholdertypes import CardholderTypesAPI
 from ._guardpoint_controllers import ControllersAPI
 from ._guardpoint_diagnostic import DiagnosticAPI
+from ._guardpoint_events import EventsAPI
 from ._guardpoint_ouputs import OutputsAPI
 from ._guardpoint_readers import ReadersAPI
 from ._guardpoint_scheduledmags import ScheduledMagsAPI
 from ._guardpoint_customizedfields import CustomizedFieldsAPI
 from ._guardpoint_personaldetails import PersonalDetailsAPI
 from ._guardpoint_securitygroups import SecurityGroupsAPI
 from .guardpoint_connection import GuardPointConnection, GuardPointAuthType
@@ -35,15 +37,15 @@
     self.task.cancel()
     while not self.task.cancelled():
         sleep(1)'''
 
 
 class GuardPoint(GuardPointConnection, CardsAPI, CardholdersAPI, AreasAPI, SecurityGroupsAPI,
                  CustomizedFieldsAPI, PersonalDetailsAPI, ScheduledMagsAPI, CardholderTypesAPI,
-                 OutputsAPI, DiagnosticAPI, ReadersAPI, ControllersAPI):
+                 OutputsAPI, DiagnosticAPI, ReadersAPI, ControllersAPI, AlarmsAPI, EventsAPI):
     task = None
 
     def __init__(self, **kwargs):
         # Set default values if not present
         host = kwargs.get('host', "localhost")
         port = kwargs.get('port', None)
         url_components = url_parser(host)
```

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/guardpoint_asyncio.py` & `pyguardpoint-1.4.0/pyGuardPoint/guardpoint_asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,27 @@
 from .gp_asyncio._async_guardpoint_scheduledmags import ScheduledMagsAPI
 from .gp_asyncio._async_guardpoint_customizedfields import CustomizedFieldsAPI
 from .gp_asyncio._async_guardpoint_personaldetails import PersonalDetailsAPI
 from .gp_asyncio._async_guardpoint_securitygroups import SecurityGroupsAPI
 from .gp_asyncio._async_guardpoint_cards import CardsAPI
 from .gp_asyncio._async_guardpoint_cardholders import CardholdersAPI
 from .gp_asyncio._async_guardpoint_areas import AreasAPI
+from .gp_asyncio._async_guardpoint_alarms import AlarmsAPI
+from .gp_asyncio._async_guardpoint_events import EventsAPI
 from .gp_asyncio.guardpoint_connection_asyncio import GuardPointConnection, GuardPointAuthType
 
 from .guardpoint_error import GuardPointError, GuardPointUnauthorized
 from .guardpoint_utils import url_parser, ConvertBase64
 
 log = logging.getLogger(__name__)
 
 
 class GuardPointAsyncIO(GuardPointConnection, CardsAPI, CardholdersAPI, AreasAPI, SecurityGroupsAPI,
                         CustomizedFieldsAPI, PersonalDetailsAPI, ScheduledMagsAPI, CardholderTypesAPI,
-                        OutputsAPI, DiagnosticAPI, ReadersAPI, ControllersAPI):
+                        OutputsAPI, DiagnosticAPI, ReadersAPI, ControllersAPI, AlarmsAPI, EventsAPI):
     task = None
 
     def __init__(self, **kwargs):
         # Set default values if not present
         host = kwargs.get('host', "localhost")
         port = kwargs.get('port', None)
         url_components = url_parser(host)
```

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/guardpoint_connection.py` & `pyguardpoint-1.4.0/pyGuardPoint/guardpoint_connection.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/guardpoint_dataclasses.py` & `pyguardpoint-1.4.0/pyGuardPoint/guardpoint_dataclasses.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,14 +43,111 @@
 
 
 class SortAlgorithm(Enum):
     SERVER_DEFAULT = 0,
     FUZZY_MATCH = 1
 
 @dataclass
+class AlarmEvent:
+    additionalSites: any = None
+    additionalSitesNames: any = None
+    alarmUID: str = ""
+    confirmationComments: any = None
+    dateTime: str = ""
+    inputName: str = ""
+    inputUID: str = ""
+    isAcknowledged: bool = False
+    isConfirmed: bool = False
+    isPastEvent: bool = False
+    journalUpdateDateTime: str = ""
+    ownerSiteName: str = ""
+    ownerSiteUID: str = ""
+    type: str = ""
+    uid: str = ""
+    userFirstName: any = None
+    userLastName: any = None
+    userName: any = None
+    userUID: any = None
+
+    def __init__(self, *args, **kwargs):
+        super().__init__()
+        alarm_event_dict = sanitise_args(self, args, kwargs)
+
+        for property_name in alarm_event_dict:
+            if isinstance(alarm_event_dict[property_name], (str, type(None), bool, int)):
+                setattr(self, property_name, alarm_event_dict[property_name])
+
+    def dict(self):
+        alarm_event_dict = {}
+        for k, v in asdict(self).items():
+            if isinstance(v, (list, dict, bool, int)):
+                alarm_event_dict[k] = v
+            elif isinstance(v, type(None)):
+                alarm_event_dict[k] = None
+            else:
+                alarm_event_dict[k] = str(v)
+
+        return alarm_event_dict
+
+@dataclass
+class AccessEvent:
+    accessDeniedCode: str = ""
+    cardCode: str = ""
+    cardholderFirstName: any = None
+    cardholderIdNumber: any = None
+    cardholderLastName: any = None
+    cardholderTypeName: any = None
+    cardholderTypeUID: any = None
+    cardholderUID: str = ""
+    carRegistrationNum: any = None
+    dateTime: str = ""
+    escortCardCode: any = None
+    escortFirstName: any = None
+    escortLastName: any = None
+    escortUID: any = None
+    inOutType: any = None
+    isEscort: bool = False
+    isPastEvent: bool = False
+    isSlave: bool = False
+    journalUpdateDateTime: str = ""
+    logID: int = 0
+    readerFunctionCodes: list = None
+    readerName: str = ""
+    readerUID: str = ""
+    transactionCode: int = 0
+    type: str = ""
+    uid: str = ""
+    ownerSiteUID: str = ""
+    additionalSites: any = None
+    ownerSiteName: str = ""
+    additionalSitesNames: any = None
+    additionalInfo: any = None
+
+    def __init__(self, *args, **kwargs):
+        super().__init__()
+        access_event_dict = sanitise_args(self, args, kwargs)
+
+        for property_name in access_event_dict:
+            if isinstance(access_event_dict[property_name], (str, type(None), bool, int)):
+                setattr(self, property_name, access_event_dict[property_name])
+
+    def dict(self):
+        access_event_dict = {}
+        for k, v in asdict(self).items():
+            if isinstance(v, (list, dict, bool, int)):
+                access_event_dict[k] = v
+            elif isinstance(v, type(None)):
+                access_event_dict[k] = None
+            else:
+                access_event_dict[k] = str(v)
+
+        return access_event_dict
+
+
+@dataclass
 class Controller:
     isActivated: any = None
     uid: str = ""
     address: int = 0
     networkUID: str = ""
     name: str = ""
     isPooling: any = None
@@ -80,14 +177,15 @@
             elif isinstance(v, type(None)):
                 controller_dict[k] = None
             else:
                 controller_dict[k] = str(v)
 
         return controller_dict
 
+
 @dataclass
 class Reader:
     uid: str = ""
     name: str = ""
     description: any = None
     number: int = 0
     controllerUID: str = ""
```

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/guardpoint_threaded.py` & `pyguardpoint-1.4.0/pyGuardPoint/guardpoint_threaded.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/pyGuardPoint/guardpoint_utils.py` & `pyguardpoint-1.4.0/pyGuardPoint/guardpoint_utils.py`

 * *Files identical despite different names*

### Comparing `pyguardpoint-1.3.9/pyGuardPoint.egg-info/PKG-INFO` & `pyguardpoint-1.4.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: pyGuardPoint
-Version: 1.3.9
+Version: 1.4.0
 Summary: Python wrapper for GuardPoint 10 Access Control System
 Author: John Owen
 Maintainer-email: sales@sensoraccess.co.uk
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: validators
 Requires-Dist: fuzzywuzzy
 Requires-Dist: cryptography
 Requires-Dist: pysignalr
 Requires-Dist: websockets
+Requires-Dist: python-Levenshtein
 
 pyGuardPoint
 ===============
 
 pyGuardPoint is a Python wrapper for the GuardPoint 10 API, which allows developers to easily integrate with the GuardPoint 10 physical access control system (ACS).
 
 pyGuardPoint aims to provide a pythonic OOP style programming interface to the WebAPI of GuardPoint 10 (GP10), perfect for quickly building proof-of-concepts.
@@ -108,16 +109,14 @@
     cardholder.pretty_print()   # Print nicely in the terminal window
 
 To get a list of areas/zones, and count the number of cardholders in each:
 
     gp = GuardPoint(host="sensoraccess.duckdns.org", pwd="password")
 
     areas = gp.get_areas()
-
-    areas = gp.get_areas()
     for area in areas:
         cardholder_count = gp.get_card_holders(count=True, areas=area)
         print(f"Cardholders in {area.name} = {str(cardholder_count)}")
 
 To get a list of security groups:
 
     sec_groups = gp.get_security_groups()
@@ -138,14 +137,79 @@
                       toDateValid=toDateValid)
     gp.add_scheduled_mag(sm)
 
     scheduled_mags = gp.get_scheduled_mags()
     for scheduled_mag in scheduled_mags:
         print(scheduled_mag)
 
+Complete example script using GuardPointAsyncIO to get Access followed by Alarm Events:
+
+    from pyGuardPoint_Build.pyGuardPoint import GuardPointAsyncIO, GuardPointError, GuardPointUnauthorized
+
+    # GuardPoint
+    GP_HOST = 'https://sensoraccess.duckdns.org'
+    # GP_HOST = 'http://localhost/'
+    GP_USER = 'admin'
+    GP_PASS = 'admin'
+    # TLS/SSL secure connection
+    TLS_P12 = "/Users/johnowen/Downloads/MobileGuardDefault.p12"
+    #TLS_P12 = "C:\\Users\\john_\\OneDrive\\Desktop\\MobGuardDefault\\MobileGuardDefault.p12"
+    TLS_P12_PWD = "test"
+
+    if __name__ == "__main__":
+        py_gp_version = version("pyGuardPoint")
+        print("pyGuardPoint Version:" + py_gp_version)
+        py_gp_version_int = int(py_gp_version.replace('.', ''))
+        if py_gp_version_int < 138:
+            print("Please Update pyGuardPoint")
+            print("\t (Within a Terminal Window) Run > 'pip install pyGuardPoint --upgrade'")
+            exit()
+
+        logging.basicConfig(level=logging.DEBUG)
+
+        async def main():
+            gp = GuardPointAsyncIO(host=GP_HOST,
+                                   username=GP_USER,
+                                   pwd=GP_PASS,
+                                   p12_file=TLS_P12,
+                                   p12_pwd=TLS_P12_PWD)
+
+            print(f"\n********* Get Access Events **********")
+            access_events = await gp.get_access_events(limit=3, offset=0)
+
+            for access_event in access_events:
+                print(f"\nAccessEvent:")
+                print(f"\tType: {access_event.type}")
+                print(f"\tjournalUpdateDateTime: {access_event.journalUpdateDateTime}")
+                print(f"\tdateTime: {access_event.dateTime}")
+                print(f"\taccessDeniedCode: {access_event.accessDeniedCode}")
+                print(f"\tisPastEvent: {access_event.isPastEvent}")
+
+            print(f"\n\n********* Get Alarm Events **********")
+            alarm_events = await gp.get_alarm_events(limit=3, offset=0)
+
+            for alarm_event in alarm_events:
+                print(f"\nAlarmEvent:")
+                print(f"\tType: {alarm_event.type}")
+                print(f"\tjournalUpdateDateTime: {alarm_event.journalUpdateDateTime}")
+                print(f"\tdateTime: {alarm_event.dateTime}")
+
+            await gp.close()
+
+        try:
+            asyncio.run(main())
+        except GuardPointError as e:
+            print(f"GuardPointError: {e}")
+        except GuardPointUnauthorized as e:
+            print(f"GuardPointUnauthorized: {e}")
+        except Exception as e:
+            print(f"Exception: {e}")
+
+
+
 GuardPoint servers can be setup with a Signal-R service enabled.
 Once enabled the server will broadcast events to clients listening to events.
 
     try:
         gp = GuardPoint(host=GP_HOST,
                         username=GP_USER,
                         pwd=GP_PASS,
```

### Comparing `pyguardpoint-1.3.9/pyGuardPoint.egg-info/SOURCES.txt` & `pyguardpoint-1.4.0/pyGuardPoint.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 LICENSE.txt
 README.rst
 setup.py
 pyGuardPoint/CustomWebsocketTransport.py
 pyGuardPoint/__init__.py
+pyGuardPoint/_guardpoint_alarms.py
 pyGuardPoint/_guardpoint_areas.py
 pyGuardPoint/_guardpoint_cardholders.py
 pyGuardPoint/_guardpoint_cardholdertypes.py
 pyGuardPoint/_guardpoint_cards.py
 pyGuardPoint/_guardpoint_controllers.py
 pyGuardPoint/_guardpoint_customizedfields.py
 pyGuardPoint/_guardpoint_diagnostic.py
+pyGuardPoint/_guardpoint_events.py
 pyGuardPoint/_guardpoint_ouputs.py
 pyGuardPoint/_guardpoint_personaldetails.py
 pyGuardPoint/_guardpoint_readers.py
 pyGuardPoint/_guardpoint_scheduledmags.py
 pyGuardPoint/_guardpoint_securitygroups.py
 pyGuardPoint/_odata_filter.py
 pyGuardPoint/_str_match_algo.py
@@ -27,20 +29,22 @@
 pyGuardPoint.egg-info/PKG-INFO
 pyGuardPoint.egg-info/SOURCES.txt
 pyGuardPoint.egg-info/dependency_links.txt
 pyGuardPoint.egg-info/not-zip-safe
 pyGuardPoint.egg-info/requires.txt
 pyGuardPoint.egg-info/top_level.txt
 pyGuardPoint/gp_asyncio/__init__.py
+pyGuardPoint/gp_asyncio/_async_guardpoint_alarms.py
 pyGuardPoint/gp_asyncio/_async_guardpoint_areas.py
 pyGuardPoint/gp_asyncio/_async_guardpoint_cardholders.py
 pyGuardPoint/gp_asyncio/_async_guardpoint_cardholdertypes.py
 pyGuardPoint/gp_asyncio/_async_guardpoint_cards.py
 pyGuardPoint/gp_asyncio/_async_guardpoint_controllers.py
 pyGuardPoint/gp_asyncio/_async_guardpoint_customizedfields.py
 pyGuardPoint/gp_asyncio/_async_guardpoint_diagnostic.py
+pyGuardPoint/gp_asyncio/_async_guardpoint_events.py
 pyGuardPoint/gp_asyncio/_async_guardpoint_ouputs.py
 pyGuardPoint/gp_asyncio/_async_guardpoint_personaldetails.py
 pyGuardPoint/gp_asyncio/_async_guardpoint_readers.py
 pyGuardPoint/gp_asyncio/_async_guardpoint_scheduledmags.py
 pyGuardPoint/gp_asyncio/_async_guardpoint_securitygroups.py
 pyGuardPoint/gp_asyncio/guardpoint_connection_asyncio.py
```

### Comparing `pyguardpoint-1.3.9/setup.py` & `pyguardpoint-1.4.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 long_description = open('README.rst').read()
 
 setup(name="pyGuardPoint",
       packages=find_packages(),
-      version="1.3.9",
+      version="1.4.0",
       author="John Owen",
       description="Python wrapper for GuardPoint 10 Access Control System",
       long_description_content_type='text/markdown',
       long_description=long_description,
       maintainer_email="sales@sensoraccess.co.uk",
-      install_requires=['validators', 'fuzzywuzzy', 'cryptography', 'pysignalr', 'websockets'],
+      install_requires=['validators', 'fuzzywuzzy', 'cryptography', 'pysignalr', 'websockets', 'python-Levenshtein'],
       #packages=['pyGuardPoint'],
       license_files=('LICENSE.txt',),
       zip_safe=False)
```

