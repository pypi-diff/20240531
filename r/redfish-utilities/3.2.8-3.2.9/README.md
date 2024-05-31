# Comparing `tmp/redfish_utilities-3.2.8.tar.gz` & `tmp/redfish_utilities-3.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redfish_utilities-3.2.8.tar", last modified: Wed Apr 10 18:56:26 2024, max compression
+gzip compressed data, was "redfish_utilities-3.2.9.tar", last modified: Fri May 31 20:40:16 2024, max compression
```

## Comparing `redfish_utilities-3.2.8.tar` & `redfish_utilities-3.2.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:56:26.689970 redfish_utilities-3.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-10 18:56:26.689970 redfish_utilities-3.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:56:26.685970 redfish_utilities-3.2.8/redfish_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/assembly.py
--rw-r--r--   0 runner    (1001) docker     (127)    12926 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/certificates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/event_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    17199 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7306 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)    12226 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    28167 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    24708 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/power_equipment.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/resets.py
--rw-r--r--   0 runner    (1001) docker     (127)    24116 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)    28536 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/systems.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8182 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/redfish_utilities/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:56:26.689970 redfish_utilities-3.2.8/redfish_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-10 18:56:26.000000 redfish_utilities-3.2.8/redfish_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-10 18:56:26.000000 redfish_utilities-3.2.8/redfish_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 18:56:26.000000 redfish_utilities-3.2.8/redfish_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-10 18:56:26.000000 redfish_utilities-3.2.8/redfish_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 18:56:26.000000 redfish_utilities-3.2.8/redfish_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:56:26.689970 redfish_utilities-3.2.8/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     6277 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_assembly.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_bios_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_boot_override.py
--rw-r--r--   0 runner    (1001) docker     (127)     7874 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_certificates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_diagnostic_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_discover.py
--rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_event_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11275 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_manager_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_power_equipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_power_reset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_raw_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_sensor_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_sys_inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_test_event_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/scripts/rf_virtual_media.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 18:56:26.689970 redfish_utilities-3.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-10 18:56:12.000000 redfish_utilities-3.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:40:16.628326 redfish_utilities-3.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-05-31 20:40:16.628326 redfish_utilities-3.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:40:16.620326 redfish_utilities-3.2.9/redfish_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/redfish_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8415 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/redfish_utilities/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/redfish_utilities/assembly.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12884 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/redfish_utilities/certificates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/redfish_utilities/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/redfish_utilities/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8907 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/redfish_utilities/event_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17350 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/redfish_utilities/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7341 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/redfish_utilities/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/redfish_utilities/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29085 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/redfish_utilities/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/redfish_utilities/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/redfish_utilities/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26068 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/redfish_utilities/power_equipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/redfish_utilities/resets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27047 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/redfish_utilities/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29297 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/redfish_utilities/systems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/redfish_utilities/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7861 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/redfish_utilities/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:40:16.624326 redfish_utilities-3.2.9/redfish_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-05-31 20:40:16.000000 redfish_utilities-3.2.9/redfish_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-31 20:40:16.000000 redfish_utilities-3.2.9/redfish_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:40:16.000000 redfish_utilities-3.2.9/redfish_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-31 20:40:16.000000 redfish_utilities-3.2.9/redfish_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-31 20:40:16.000000 redfish_utilities-3.2.9/redfish_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:40:16.624326 redfish_utilities-3.2.9/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     6190 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/scripts/rf_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/scripts/rf_assembly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/scripts/rf_bios_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/scripts/rf_boot_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7936 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/scripts/rf_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/scripts/rf_diagnostic_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/scripts/rf_discover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/scripts/rf_event_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/scripts/rf_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/scripts/rf_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11093 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/scripts/rf_manager_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7343 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/scripts/rf_power_equipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/scripts/rf_power_reset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/scripts/rf_raw_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/scripts/rf_sensor_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/scripts/rf_sys_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/scripts/rf_test_event_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/scripts/rf_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/scripts/rf_virtual_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 20:40:16.628326 redfish_utilities-3.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-05-31 20:40:07.000000 redfish_utilities-3.2.9/setup.py
```

### Comparing `redfish_utilities-3.2.8/LICENSE.md` & `redfish_utilities-3.2.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.8/PKG-INFO` & `redfish_utilities-3.2.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish_utilities
-Version: 3.2.8
+Version: 3.2.9
 Summary: Redfish Utilities
 Home-page: https://github.com/DMTF/Redfish-Tacklebox
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
@@ -17,14 +17,23 @@
 Requires-Dist: XlsxWriter>=1.2.7
 Requires-Dist: requests
 
 # Redfish Tacklebox
 
 Copyright 2019-2024 DMTF.  All rights reserved.
 
+[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md)
+[![PyPI](https://img.shields.io/pypi/v/redfish-utilities)](https://pypi.org/project/redfish-utilities/)
+[![Pulls](https://img.shields.io/docker/pulls/dmtf/redfish-tacklebox?style=flat&logo=docker&label=Pulls)](https://hub.docker.com/r/dmtf/redfish-tacklebox)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat)](https://github.com/psf/black)
+[![Linters](https://github.com/DMTF/Redfish-Tacklebox/actions/workflows/linters.yml/badge.svg)](https://github.com/DMTF/Redfish-Tacklebox/actions/workflows/linters.yml)
+[![Docker](https://github.com/DMTF/Redfish-Tacklebox/actions/workflows/docker.yml/badge.svg)](https://github.com/DMTF/Redfish-Tacklebox/actions/workflows/docker.yml)
+[![GitHub stars](https://img.shields.io/github/stars/DMTF/Redfish-Tacklebox.svg?style=flat-square&label=github%20stars)](https://github.com/DMTF/Redfish-Tacklebox)
+[![GitHub Contributors](https://img.shields.io/github/contributors/DMTF/Redfish-Tacklebox.svg?style=flat-square)](https://github.com/DMTF/Redfish-Tacklebox/graphs/contributors)
+
 ## About
 
 Redfish Tacklebox contains a set of Python3 utilities to perform common management operations with a Redfish service.
 The utilities can be used as part of larger management applications, or be used as standalone command line tools.
 
 ## Installation
 
@@ -38,25 +47,25 @@
 ```
 
 ### Building Docker
 
 * Pull the container from Docker Hub:
 
     ```bash
-    docker pull dmtf/redfish-utilities:latest
+    docker pull dmtf/redfish-tacklebox:latest
     ```
 * Build a container from local source:
 
     ```bash
-    docker build -t dmtf/redfish-utilities:latest .
+    docker build -t dmtf/redfish-tacklebox:latest .
     ```
 * Build a container from GitHub:
 
     ```bash
-    docker build -t dmtf/redfish-utilities:latest https://github.com/DMTF/Redfish-Tacklebox.git
+    docker build -t dmtf/redfish-tacklebox:latest https://github.com/DMTF/Redfish-Tacklebox.git
     ```
 
 ## Requirements
 
 External modules:
 * redfish: https://pypi.python.org/pypi/redfish
 * XlsxWriter: https://pypi.org/project/XlsxWriter
```

### Comparing `redfish_utilities-3.2.8/README.md` & `redfish_utilities-3.2.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 # Redfish Tacklebox
 
 Copyright 2019-2024 DMTF.  All rights reserved.
 
+[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md)
+[![PyPI](https://img.shields.io/pypi/v/redfish-utilities)](https://pypi.org/project/redfish-utilities/)
+[![Pulls](https://img.shields.io/docker/pulls/dmtf/redfish-tacklebox?style=flat&logo=docker&label=Pulls)](https://hub.docker.com/r/dmtf/redfish-tacklebox)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat)](https://github.com/psf/black)
+[![Linters](https://github.com/DMTF/Redfish-Tacklebox/actions/workflows/linters.yml/badge.svg)](https://github.com/DMTF/Redfish-Tacklebox/actions/workflows/linters.yml)
+[![Docker](https://github.com/DMTF/Redfish-Tacklebox/actions/workflows/docker.yml/badge.svg)](https://github.com/DMTF/Redfish-Tacklebox/actions/workflows/docker.yml)
+[![GitHub stars](https://img.shields.io/github/stars/DMTF/Redfish-Tacklebox.svg?style=flat-square&label=github%20stars)](https://github.com/DMTF/Redfish-Tacklebox)
+[![GitHub Contributors](https://img.shields.io/github/contributors/DMTF/Redfish-Tacklebox.svg?style=flat-square)](https://github.com/DMTF/Redfish-Tacklebox/graphs/contributors)
+
 ## About
 
 Redfish Tacklebox contains a set of Python3 utilities to perform common management operations with a Redfish service.
 The utilities can be used as part of larger management applications, or be used as standalone command line tools.
 
 ## Installation
 
@@ -19,25 +28,25 @@
 ```
 
 ### Building Docker
 
 * Pull the container from Docker Hub:
 
     ```bash
-    docker pull dmtf/redfish-utilities:latest
+    docker pull dmtf/redfish-tacklebox:latest
     ```
 * Build a container from local source:
 
     ```bash
-    docker build -t dmtf/redfish-utilities:latest .
+    docker build -t dmtf/redfish-tacklebox:latest .
     ```
 * Build a container from GitHub:
 
     ```bash
-    docker build -t dmtf/redfish-utilities:latest https://github.com/DMTF/Redfish-Tacklebox.git
+    docker build -t dmtf/redfish-tacklebox:latest https://github.com/DMTF/Redfish-Tacklebox.git
     ```
 
 ## Requirements
 
 External modules:
 * redfish: https://pypi.python.org/pypi/redfish
 * XlsxWriter: https://pypi.org/project/XlsxWriter
```

### Comparing `redfish_utilities-3.2.8/redfish_utilities/accounts.py` & `redfish_utilities-3.2.9/redfish_utilities/accounts.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,146 +10,168 @@
 
 Brief : This file contains the definitions and functionalities for managing
         accounts on a Redfish Service
 """
 
 from .messages import verify_response
 
-class RedfishAccountCollectionNotFoundError( Exception ):
+
+class RedfishAccountCollectionNotFoundError(Exception):
     """
     Raised when the Account Service or Account Collection cannot be found
     """
+
     pass
 
-class RedfishAccountNotFoundError( Exception ):
+
+class RedfishAccountNotFoundError(Exception):
     """
     Raised when the Account Service or Account Collection cannot be found
     """
+
     pass
 
-class RedfishAccountNotAddedError( Exception ):
+
+class RedfishAccountNotAddedError(Exception):
     """
     Raised when the requested account was not added
     """
+
     pass
 
-def get_users( context ):
+
+def get_users(context):
     """
     Collects user information from a Redfish service
 
     Args:
         context: The Redfish client object with an open session
 
     Returns:
         A list containing all users
     """
 
     user_list = []
 
     # Go through each Account in the Account Collection
-    account_col = context.get( get_account_collection( context ), None )
+    account_col = context.get(get_account_collection(context), None)
     for account_member in account_col.dict["Members"]:
-        account = context.get( account_member["@odata.id"], None )
+        account = context.get(account_member["@odata.id"], None)
         account_info = {
             "UserName": account.dict["UserName"],
             "RoleId": account.dict["RoleId"],
-            "Locked": account.dict.get( "Locked", False ),
-            "Enabled": account.dict.get( "Enabled", True )
+            "Locked": account.dict.get("Locked", False),
+            "Enabled": account.dict.get("Enabled", True),
         }
 
         # Some implementations always expose "slots" for users; ignore empty slots
-        if account_info["UserName"] == "" and account_info["Enabled"] == False:
+        if account_info["UserName"] == "" and account_info["Enabled"] is False:
             continue
 
-        user_list.append( account_info )
+        user_list.append(account_info)
 
     return user_list
 
-def print_users( user_list ):
+
+def print_users(user_list):
     """
     Prints the user list into a table
 
     Args:
         user_list: The user list to print
     """
 
     user_line_format = "  {:20s} | {:20s} | {:10s} | {:10s}"
-    print( "" )
-    print( user_line_format.format( "Name", "Role", "Locked", "Enabled" ) )
+    print("")
+    print(user_line_format.format("Name", "Role", "Locked", "Enabled"))
     for user in user_list:
-        print( user_line_format.format( user["UserName"], user["RoleId"], str( user["Locked"] ), str( user["Enabled"] ) ) )
-    print( "" )
+        print(user_line_format.format(user["UserName"], user["RoleId"], str(user["Locked"]), str(user["Enabled"])))
+    print("")
+
 
-def add_user( context, user_name, password, role ):
+def add_user(context, user_name, password, role):
     """
     Adds a new user account
 
     Args:
         context: The Redfish client object with an open session
         user_name: The name of the user to add
         password: The password for the new user
         role: The role for the new user
 
     Returns:
         The response of the POST
     """
 
     # Create the new user
-    payload = {
-        "UserName": user_name,
-        "Password": password,
-        "RoleId": role
-    }
-    account_col_uri = get_account_collection( context )
-    response = context.post( account_col_uri, body = payload )
+    payload = {"UserName": user_name, "Password": password, "RoleId": role}
+    account_col_uri = get_account_collection(context)
+    response = context.post(account_col_uri, body=payload)
     if response.status == 405:
         # Some implementations allocate slots for users and don't allow adding in the proper sense
         # Find an empty slot to use
         account_added = False
-        account_col = context.get( account_col_uri )
+        account_col = context.get(account_col_uri)
         for account_member in account_col.dict["Members"]:
-            account = context.get( account_member["@odata.id"] )
-            if account.dict["UserName"] == "" and not account.dict.get( "Enabled", True ):
+            account = context.get(account_member["@odata.id"])
+            if account.dict["UserName"] == "" and not account.dict.get("Enabled", True):
                 # Empty slot found; PATCH it
-                response = context.patch( account_member["@odata.id"], body = payload, headers = { "If-Match": account.getheader( "ETag" ) } )
+                response = context.patch(
+                    account_member["@odata.id"], body=payload, headers={"If-Match": account.getheader("ETag")}
+                )
                 if response.status < 400:
                     # These implementations also might restrict which slots to modify...
                     account_added = True
                     break
         if not account_added:
-            raise RedfishAccountNotAddedError( "Failed to add user '{}'; user may already exist or there is not enough space for the new user".format( user_name ) )
-    verify_response( response )
+            raise RedfishAccountNotAddedError(
+                "Failed to add user '{}'; user may already exist or there is not enough space for the new user".format(
+                    user_name
+                )
+            )
+    verify_response(response)
     return response
 
-def delete_user( context, user_name ):
+
+def delete_user(context, user_name):
     """
     Deletes an existing user account
 
     Args:
         context: The Redfish client object with an open session
         user_name: The name of the user to delete
 
     Returns:
         The response of the DELETE
     """
 
     # Find the user to delete
-    user_uri, user_info = get_user( context, user_name )
+    user_uri, user_info = get_user(context, user_name)
 
     # Delete the user
-    response = context.delete( user_uri )
+    response = context.delete(user_uri)
     if response.status == 405:
         # Some implementations keep slots around and don't allow for deleting in the proper sense
         # Some also do not allow for both Enabled and UserName to be modified simultaneously
-        modify_user( context, user_name, new_enabled = False )
-        return modify_user( context, user_name, new_name = "" )
-    verify_response( response )
+        modify_user(context, user_name, new_enabled=False)
+        return modify_user(context, user_name, new_name="")
+    verify_response(response)
     return response
 
-def modify_user( context, user_name, new_name = None, new_password = None, new_role = None, new_locked = None, new_enabled = None, user_uri = None ):
+
+def modify_user(
+    context,
+    user_name,
+    new_name=None,
+    new_password=None,
+    new_role=None,
+    new_locked=None,
+    new_enabled=None,
+    user_uri=None,
+):
     """
     Modifies an existing user account
 
     Args:
         context: The Redfish client object with an open session
         user_name: The name of the user to modify
         new_name: The new name of the user
@@ -160,15 +182,15 @@
         user_uri: The URI of the user to modify
 
     Returns:
         The response of the PATCH
     """
 
     # Get the current user info
-    user_uri, user_info = get_user( context, user_name , user_uri = user_uri )
+    user_uri, user_info = get_user(context, user_name, user_uri=user_uri)
 
     # Build the payload for the new user
     new_info = {}
     if new_name is not None:
         new_info["UserName"] = new_name
     if new_password is not None:
         new_info["Password"] = new_password
@@ -176,44 +198,46 @@
         new_info["RoleId"] = new_role
     if new_locked is not None:
         new_info["Locked"] = new_locked
     if new_enabled is not None:
         new_info["Enabled"] = new_enabled
 
     # Update the user
-    response = context.patch( user_uri, body = new_info, headers = { "If-Match": user_info.getheader( "ETag" ) } )
-    verify_response( response )
+    response = context.patch(user_uri, body=new_info, headers={"If-Match": user_info.getheader("ETag")})
+    verify_response(response)
     return response
 
-def get_account_collection( context ):
+
+def get_account_collection(context):
     """
     Finds the account collection for the Redfish service
 
     Args:
         context: The Redfish client object with an open session
 
     Returns:
         The URI for the account collection
     """
 
     # Get the Service Root to find the Account Service
-    service_root = context.get( "/redfish/v1" )
+    service_root = context.get("/redfish/v1")
     if "AccountService" not in service_root.dict:
         # No Account Service
-        raise RedfishAccountCollectionNotFoundError( "Service does not contain an Account Service" )
+        raise RedfishAccountCollectionNotFoundError("Service does not contain an Account Service")
 
     # Get the Account Service to find the Account Collection
-    account_service = context.get( service_root.dict["AccountService"]["@odata.id"] )
+    account_service = context.get(service_root.dict["AccountService"]["@odata.id"])
     if "Accounts" not in account_service.dict:
         # No Account Collection
-        raise RedfishAccountCollectionNotFoundError( "Service does not contain an Account Collection" )
+        raise RedfishAccountCollectionNotFoundError("Service does not contain an Account Collection")
 
     return account_service.dict["Accounts"]["@odata.id"]
 
-def get_user( context, user_name, user_uri = None ):
+
+def get_user(context, user_name, user_uri=None):
     """
     Finds a user within the Redfish service
 
     Args:
         context: The Redfish client object with an open session
         user_name: The name of the user to find
         user_uri: The URI of the user to get
@@ -222,28 +246,30 @@
         The URI for the user account
         The contents of the user account resource
     """
 
     avail_users = []
 
     if user_uri is not None:
-        account = context.get( user_uri )
+        account = context.get(user_uri)
         if account.dict["UserName"] == user_name:
             return user_uri, account
 
-    account_col = context.get( get_account_collection( context ) )
-            
+    account_col = context.get(get_account_collection(context))
+
     for account_member in account_col.dict["Members"]:
-        account = context.get( account_member["@odata.id"] )
+        account = context.get(account_member["@odata.id"])
 
         # Some implementations always expose "slots" for users; ignore empty slots
-        if account.dict["UserName"] == "" and not account.dict.get( "Enabled", True ):
+        if account.dict["UserName"] == "" and not account.dict.get("Enabled", True):
             continue
 
-        avail_users.append( account.dict["UserName"] )
+        avail_users.append(account.dict["UserName"])
 
         # Check if the name matches
         if account.dict["UserName"] == user_name:
             return account_member["@odata.id"], account
 
     # No matches found
-    raise RedfishAccountCollectionNotFoundError( "User '{}' is not found; valid users: {}".format( user_name, ", ".join( avail_users ) ) )
+    raise RedfishAccountCollectionNotFoundError(
+        "User '{}' is not found; valid users: {}".format(user_name, ", ".join(avail_users))
+    )
```

### Comparing `redfish_utilities-3.2.8/redfish_utilities/assembly.py` & `redfish_utilities-3.2.9/redfish_utilities/assembly.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,143 +10,168 @@
 
 Brief : This file contains the definitions and functionalities for managing
         assemblies on a Redfish service
 """
 
 from .messages import verify_response
 
-class RedfishAssemblyNotFoundError( Exception ):
+
+class RedfishAssemblyNotFoundError(Exception):
     """
     Raised when an assembly index cannot be found
     """
+
     pass
 
-class RedfishAssemblyNoBinaryDataError( Exception ):
+
+class RedfishAssemblyNoBinaryDataError(Exception):
     """
     Raised when an assembly index does not contain binary data
     """
+
     pass
 
-def get_assembly( context, uri ):
+
+def get_assembly(context, uri):
     """
     Collects assembly information from a Redfish service
 
     Args:
         context: The Redfish client object with an open session
         uri: The URI of the assembly to get
 
     Returns:
         A list containing all assemblies from the URI
     """
 
     # Get the assembly
-    assembly = context.get( uri )
-    verify_response( assembly )
-    return assembly.dict.get( "Assemblies", [] )
+    assembly = context.get(uri)
+    verify_response(assembly)
+    return assembly.dict.get("Assemblies", [])
 
-def print_assembly( assemblies, index = None ):
+
+def print_assembly(assemblies, index=None):
     """
     Prints assembly information into a table
 
     Args:
         assemblies: An array of assembly information to print
         index: If specified, prints only the desired index
     """
 
     assembly_format_header = " {:5s} | {} {}"
     assembly_format = " {:5s} | {}: {}"
-    assembly_properties = [ "Model", "PartNumber", "SparePartNumber", "SKU", "SerialNumber", "Producer", "Vendor",
-                            "ProductionDate", "Version", "EngineeringChangeLevel" ]
+    assembly_properties = [
+        "Model",
+        "PartNumber",
+        "SparePartNumber",
+        "SKU",
+        "SerialNumber",
+        "Producer",
+        "Vendor",
+        "ProductionDate",
+        "Version",
+        "EngineeringChangeLevel",
+    ]
 
     # If an index is specified, isolate to the one index
     if index is not None:
-        if index < 0 or index >= len( assemblies ):
-            raise RedfishAssemblyNotFoundError( "Assembly contains {} entries; index {} is not valid".format( len( assemblies ), index ) )
-        assemblies = [ assemblies[index] ]
+        if index < 0 or index >= len(assemblies):
+            raise RedfishAssemblyNotFoundError(
+                "Assembly contains {} entries; index {} is not valid".format(len(assemblies), index)
+            )
+        assemblies = [assemblies[index]]
 
     # Go through each assembly
     for assembly in assemblies:
         # Print the heading
         heading_details = []
-        state = assembly.get( "Status", {} ).get( "State" )
+        state = assembly.get("Status", {}).get("State")
         if state:
-            heading_details.append( state )
-        health = assembly.get( "Status", {} ).get( "Health" )
+            heading_details.append(state)
+        health = assembly.get("Status", {}).get("Health")
         if health:
-            heading_details.append( health )
-        heading_details = ", ".join( heading_details )
-        if len( heading_details ) != 0:
+            heading_details.append(health)
+        heading_details = ", ".join(heading_details)
+        if len(heading_details) != 0:
             heading_details = "(" + heading_details + ")"
-        print( assembly_format_header.format( assembly["MemberId"], assembly["Name"], heading_details ) )
+        print(assembly_format_header.format(assembly["MemberId"], assembly["Name"], heading_details))
 
         # Print any of the found properties
         for property in assembly_properties:
             if property in assembly:
-                print( assembly_format.format( "", property, assembly[property] ) )
+                print(assembly_format.format("", property, assembly[property]))
+
 
-def download_assembly( context, assemblies, filepath, index = None ):
+def download_assembly(context, assemblies, filepath, index=None):
     """
     Downloads the binary data of an assembly to a file
 
     Args:
         context: The Redfish client object with an open session
         assemblies: An array of assembly information
         filepath: The filepath to download the binary data
         index: The index into the assemblies array to download; if None, perform on index 0 if there's only 1 assembly
     """
 
     # Get the binary data URI
-    binary_data_uri = get_assembly_binary_data_uri( assemblies, index )
+    binary_data_uri = get_assembly_binary_data_uri(assemblies, index)
 
     # Download the data and save it
-    response = context.get( binary_data_uri )
-    verify_response( response )
-    with open( filepath, "wb" ) as binary_file:
-        binary_file.write( response.read )
+    response = context.get(binary_data_uri)
+    verify_response(response)
+    with open(filepath, "wb") as binary_file:
+        binary_file.write(response.read)
 
-def upload_assembly( context, assemblies, filepath, index = None ):
+
+def upload_assembly(context, assemblies, filepath, index=None):
     """
     Uploads the binary data of a file to an assembly
 
     Args:
         context: The Redfish client object with an open session
         assemblies: An array of assembly information
         filepath: The filepath of the binary data to upload
         index: The index into the assemblies array to upload; if None, perform on index 0 if there's only 1 assembly
     """
 
     # Get the binary data URI
-    binary_data_uri = get_assembly_binary_data_uri( assemblies, index )
+    binary_data_uri = get_assembly_binary_data_uri(assemblies, index)
 
     # Upload the binary data
-    with open( filepath, "rb" ) as binary_file:
+    with open(filepath, "rb") as binary_file:
         data = binary_file.read()
-    response = context.put( binary_data_uri, body = data )
-    verify_response( response )
+    response = context.put(binary_data_uri, body=data)
+    verify_response(response)
+
 
-def get_assembly_binary_data_uri( assemblies, index = None ):
+def get_assembly_binary_data_uri(assemblies, index=None):
     """
     Locates the binary data URI for a target assembly
 
     Args:
         assemblies: An array of assembly information
         index: The index into the assemblies array to download; if None, perform on index 0 if there's only 1 assembly
 
     Returns:
         A string containing the binary data URI
     """
 
     # If an index is specified, isolate to the one index
     if index is None:
         index = 0
-        if len( assemblies ) != 1:
-            raise RedfishAssemblyNotFoundError( "Assembly contains {} entries; an index needs to be specified".format( len( assemblies ) ) )
+        if len(assemblies) != 1:
+            raise RedfishAssemblyNotFoundError(
+                "Assembly contains {} entries; an index needs to be specified".format(len(assemblies))
+            )
     else:
-        if index < 0 or index >= len( assemblies ):
-            raise RedfishAssemblyNotFoundError( "Assembly contains {} entries; index {} is not valid".format( len( assemblies ), index ) )
+        if index < 0 or index >= len(assemblies):
+            raise RedfishAssemblyNotFoundError(
+                "Assembly contains {} entries; index {} is not valid".format(len(assemblies), index)
+            )
 
     # Get the binary data URI
-    binary_data_uri = assemblies[index].get( "BinaryDataURI" )
+    binary_data_uri = assemblies[index].get("BinaryDataURI")
     if binary_data_uri is None:
         # No binary data
-        raise RedfishAssemblyNoBinaryDataError( "Assembly index {} does not contain binary data".format( index ) )
+        raise RedfishAssemblyNoBinaryDataError("Assembly index {} does not contain binary data".format(index))
     return binary_data_uri
```

### Comparing `redfish_utilities-3.2.8/redfish_utilities/certificates.py` & `redfish_utilities-3.2.9/redfish_utilities/certificates.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,148 +8,176 @@
 
 File : certificates.py
 
 Brief : This file contains the definitions and functionalities for managing
         certificates on a Redfish service
 """
 
-import os
 from .messages import verify_response
 
-class RedfishCertificateServiceNotFoundError( Exception ):
+
+class RedfishCertificateServiceNotFoundError(Exception):
     """
     Raised when the certificate service cannot be found
     """
+
     pass
 
-class RedfishCertificateLocationsNotFoundError( Exception ):
+
+class RedfishCertificateLocationsNotFoundError(Exception):
     """
     Raised when the certificate locations cannot be found
     """
+
     pass
 
-class RedfishGenerateCSRActionNotFoundError( Exception ):
+
+class RedfishGenerateCSRActionNotFoundError(Exception):
     """
     Raised when the GenerateCSR action cannot be found
     """
+
     pass
 
-class RedfishReplaceCertificateActionNotFoundError( Exception ):
+
+class RedfishReplaceCertificateActionNotFoundError(Exception):
     """
     Raised when the ReplaceCertificate action cannot be found
     """
+
     pass
 
-def get_all_certificates( context ):
+
+def get_all_certificates(context):
     """
     Collects certificate information from a Redfish service
 
     Args:
         context: The Redfish client object with an open session
 
     Returns:
         A list containing all certificates
     """
 
     certificate_list = []
 
     # Get the certificate locations
-    certificate_service = get_certificate_service( context )
+    certificate_service = get_certificate_service(context)
     if "CertificateLocations" not in certificate_service:
-        raise RedfishCertificateLocationsNotFoundError( "Service does not contain certificate locations" )
-    certificate_locations = context.get( certificate_service["CertificateLocations"]["@odata.id"] )
-    verify_response( certificate_locations )
+        raise RedfishCertificateLocationsNotFoundError("Service does not contain certificate locations")
+    certificate_locations = context.get(certificate_service["CertificateLocations"]["@odata.id"])
+    verify_response(certificate_locations)
 
     # Get each member and add it to the response list
-    locations = certificate_locations.dict.get( "Links", {} ).get( "Certificates", [] )
+    locations = certificate_locations.dict.get("Links", {}).get("Certificates", [])
     for certificate_ref in locations:
-        certificate = context.get( certificate_ref["@odata.id"] )
-        verify_response( certificate )
+        certificate = context.get(certificate_ref["@odata.id"])
+        verify_response(certificate)
         certificate_info = {
             "URI": certificate.dict["@odata.id"],
             "Id": certificate.dict["Id"],
-            "Subject": certificate.dict.get( "Subject", {} ),
-            "Issuer": certificate.dict.get( "Issuer", {} ),
-            "ValidNotBefore": certificate.dict.get( "ValidNotBefore" ),
-            "ValidNotAfter": certificate.dict.get( "ValidNotAfter" ),
-            "KeyUsage": certificate.dict.get( "KeyUsage" ),
-            "SerialNumber": certificate.dict.get( "SerialNumber" ),
-            "Fingerprint": certificate.dict.get( "Fingerprint" ),
-            "FingerprintHashAlgorithm": certificate.dict.get( "FingerprintHashAlgorithm" ),
-            "SignatureAlgorithm": certificate.dict.get( "SignatureAlgorithm" ),
-            "CertificateUsageTypes": certificate.dict.get( "CertificateUsageTypes" )
+            "Subject": certificate.dict.get("Subject", {}),
+            "Issuer": certificate.dict.get("Issuer", {}),
+            "ValidNotBefore": certificate.dict.get("ValidNotBefore"),
+            "ValidNotAfter": certificate.dict.get("ValidNotAfter"),
+            "KeyUsage": certificate.dict.get("KeyUsage"),
+            "SerialNumber": certificate.dict.get("SerialNumber"),
+            "Fingerprint": certificate.dict.get("Fingerprint"),
+            "FingerprintHashAlgorithm": certificate.dict.get("FingerprintHashAlgorithm"),
+            "SignatureAlgorithm": certificate.dict.get("SignatureAlgorithm"),
+            "CertificateUsageTypes": certificate.dict.get("CertificateUsageTypes"),
         }
-        certificate_list.append( certificate_info )
+        certificate_list.append(certificate_info)
 
     return certificate_list
 
-def print_certificates( certificate_list, details = False ):
+
+def print_certificates(certificate_list, details=False):
     """
     Prints the certificate list into a table
 
     Args:
         certificate_list: The certificate list to print
         details: True to print all the detailed info
     """
 
     # Go through each certificate
     for certificate in certificate_list:
-        print( "Certificate: {}".format( certificate["URI"] ) )
-        print( "  Subject: {}".format( build_identifier_string( certificate["Subject"] ) ) )
-        print( "  Issuer: {}".format( build_identifier_string( certificate["Issuer"] ) ) )
-        print( "  Valid Not Before: {}, Valid Not After: {}".format( certificate["ValidNotBefore"], certificate["ValidNotAfter"] ) )
+        print("Certificate: {}".format(certificate["URI"]))
+        print("  Subject: {}".format(build_identifier_string(certificate["Subject"])))
+        print("  Issuer: {}".format(build_identifier_string(certificate["Issuer"])))
+        print(
+            "  Valid Not Before: {}, Valid Not After: {}".format(
+                certificate["ValidNotBefore"], certificate["ValidNotAfter"]
+            )
+        )
         if details:
             if certificate["KeyUsage"] is not None:
-                print( "  Key Usage: {}".format( ", ".join( certificate["KeyUsage"] ) ) )
+                print("  Key Usage: {}".format(", ".join(certificate["KeyUsage"])))
             if certificate["CertificateUsageTypes"] is not None:
-                print( "  Certificate Usage: {}".format( ", ".join( certificate["CertificateUsageTypes"] ) ) )
+                print("  Certificate Usage: {}".format(", ".join(certificate["CertificateUsageTypes"])))
             if certificate["SerialNumber"] is not None:
-                print( "  Serial Number: {}".format( certificate["SerialNumber"] ) )
+                print("  Serial Number: {}".format(certificate["SerialNumber"]))
             if certificate["Fingerprint"] is not None:
-                print( "  Fingerprint: {}".format( certificate["Fingerprint"] ) )
+                print("  Fingerprint: {}".format(certificate["Fingerprint"]))
             if certificate["FingerprintHashAlgorithm"] is not None:
-                print( "  Fingerprint Hash Algorithm: {}".format( certificate["FingerprintHashAlgorithm"] ) )
+                print("  Fingerprint Hash Algorithm: {}".format(certificate["FingerprintHashAlgorithm"]))
             if certificate["SignatureAlgorithm"] is not None:
-                print( "  Signature Algorithm: {}".format( certificate["SignatureAlgorithm"] ) )
-        print( "" )
+                print("  Signature Algorithm: {}".format(certificate["SignatureAlgorithm"]))
+        print("")
 
-def get_generate_csr_info( context ):
+
+def get_generate_csr_info(context):
     """
     Finds information about the support for generating CSRs
 
     Args:
         context: The Redfish client object with an open session
 
     Returns:
         The URI of the GenerateCSR action
         A list of parameter requirements from the action info
     """
 
     # Check that there is a GenerateCSR action
-    certificate_service = get_certificate_service( context )
+    certificate_service = get_certificate_service(context)
     if "Actions" not in certificate_service:
-        raise RedfishGenerateCSRActionNotFoundError( "Service does not support the GenerateCSR action" )
+        raise RedfishGenerateCSRActionNotFoundError("Service does not support the GenerateCSR action")
     if "#CertificateService.GenerateCSR" not in certificate_service["Actions"]:
-        raise RedfishGenerateCSRActionNotFoundError( "Service does not support the GenerateCSR action" )
+        raise RedfishGenerateCSRActionNotFoundError("Service does not support the GenerateCSR action")
 
     # Extract the info about the GenerateCSR action
     generate_csr_action = certificate_service["Actions"]["#CertificateService.GenerateCSR"]
     generate_csr_uri = generate_csr_action["target"]
 
     if "@Redfish.ActionInfo" not in generate_csr_action:
         # No action info; due to the action's complexity, don't try to produce a default set of parameters
         generate_csr_parameters = None
     else:
         # Get the action info and its parameter listing
-        action_info = context.get( generate_csr_action["@Redfish.ActionInfo"] )
+        action_info = context.get(generate_csr_action["@Redfish.ActionInfo"])
         generate_csr_parameters = action_info.dict["Parameters"]
 
     return generate_csr_uri, generate_csr_parameters
 
-def generate_csr( context, common_name, organization, organizational_unit, city, state, country, cert_col, email = None, key_pair_alg = None, key_bit_len = None, key_curve_id = None ):
+
+def generate_csr(
+    context,
+    common_name,
+    organization,
+    organizational_unit,
+    city,
+    state,
+    country,
+    cert_col,
+    email=None,
+    key_pair_alg=None,
+    key_bit_len=None,
+    key_curve_id=None,
+):
     """
     Generates a certificate signing request
 
     Args:
         context: The Redfish client object with an open session
         common_name: The common name of the component to secure
         organization: The name of the organization making the request
@@ -164,138 +192,142 @@
         key_curve_id: The curve ID to use with the key if the key pair algorithm supports curves
 
     Returns:
         The response of the action
     """
 
     # Locate the GenerateCSR action
-    generate_csr_uri, generate_csr_parameters = get_generate_csr_info( context )
+    generate_csr_uri, generate_csr_parameters = get_generate_csr_info(context)
 
     # Build the payload
     payload = {
-        "CertificateCollection": { "@odata.id": cert_col },
+        "CertificateCollection": {"@odata.id": cert_col},
         "CommonName": common_name,
         "Organization": organization,
         "OrganizationalUnit": organizational_unit,
         "City": city,
         "State": state,
-        "Country": country
+        "Country": country,
     }
     if email is not None:
         payload["Email"] = email
     if key_pair_alg is not None:
         payload["KeyPairAlgorithm"] = key_pair_alg
     if key_bit_len is not None:
         payload["KeyBitLength"] = key_bit_len
     if key_curve_id is not None:
         payload["KeyCurveId"] = key_curve_id
 
     # Generate a CSR
-    response = context.post( generate_csr_uri, body = payload )
-    verify_response( response )
+    response = context.post(generate_csr_uri, body=payload)
+    verify_response(response)
     return response
 
-def install_certificate( context, destination, cert_file, key_file = None ):
+
+def install_certificate(context, destination, cert_file, key_file=None):
     """
     Replaces an existing certificate with a new certificate
 
     Args:
         context: The Redfish client object with an open session
         destination: The installation URI of the certificate; either a certificate collection to insert, or an existing certificate to replace
         cert_file: The file, and optional path, of the certificate to install
         key_file: The file, and optional path, of the private key for the certificate to install
 
     Returns:
         The response of the operation
     """
 
     # Read the certificate and determine its type
-    with open( cert_file, "r" ):
-         cert_string = cert_file.read()
+    with open(cert_file, "r"):
+        cert_string = cert_file.read()
     cert_type = "PEM"
     if "BEGIN PKCS7" in cert_string:
         cert_type = "PKCS7"
-    elif cert_string.count( "BEGIN CERTIFICATE" ) > 1:
+    elif cert_string.count("BEGIN CERTIFICATE") > 1:
         cert_type = "PEMchain"
 
     # Read the key if needed, and prepend it to the certificate
     if key_file is not None:
-        with open( cert_file, "r" ):
+        with open(cert_file, "r"):
             key_string = key_file.read()
         cert_string = key_string + cert_string
 
     # Build the payload
     payload = {
-        "CertificateUri": { "@odata.id": destination },
+        "CertificateUri": {"@odata.id": destination},
         "CertificateString": cert_string,
-        "CertificateType": cert_type
+        "CertificateType": cert_type,
     }
 
     # Check if the referenced destination is a certificate collection or individual certificate
-    dest_response = context.get( destination )
-    verify_response( dest_response )
+    dest_response = context.get(destination)
+    verify_response(dest_response)
     if dest_response.dict["@odata.type"] == "#CertificateCollection.CertificateCollection":
         # Certificate collection; just perform a POST operation on the collection
-        payload.pop( "CertificateUri" )
+        payload.pop("CertificateUri")
     else:
         # Individual certificate; perform a replacement operation from the certificate service
 
         # Locate the ReplaceCertificate action
-        certificate_service = get_certificate_service( context )
+        certificate_service = get_certificate_service(context)
         if "Actions" not in certificate_service:
-            raise RedfishReplaceCertificateActionNotFoundError( "Service does not support the ReplaceCertificate action" )
+            raise RedfishReplaceCertificateActionNotFoundError("Service does not support the ReplaceCertificate action")
         if "#CertificateService.ReplaceCertificate" not in certificate_service["Actions"]:
-            raise RedfishReplaceCertificateActionNotFoundError( "Service does not support the ReplaceCertificate action" )
+            raise RedfishReplaceCertificateActionNotFoundError("Service does not support the ReplaceCertificate action")
         destination = certificate_service["Actions"]["#CertificateService.ReplaceCertificate"]["target"]
 
     # Install the certificate
-    response = context.post( destination, body = payload )
-    verify_response( response )
+    response = context.post(destination, body=payload)
+    verify_response(response)
     return response
 
-def delete_certificate( context, certificate ):
+
+def delete_certificate(context, certificate):
     """
     Replaces an existing certificate with a new certificate
 
     Args:
         context: The Redfish client object with an open session
         certificate: The URI of the certificate to delete
 
     Returns:
         The response of the operation
     """
 
     # Delete the certificate
-    response = context.delete( certificate )
-    verify_response( response )
+    response = context.delete(certificate)
+    verify_response(response)
     return response
 
-def get_certificate_service( context ):
+
+def get_certificate_service(context):
     """
     Collects the certificate service information from a Redfish service
 
     Args:
         context: The Redfish client object with an open session
 
     Returns:
         An object containing information about the certificate service
     """
 
     # Get the service root to find the certificate service
-    service_root = context.get( "/redfish/v1/" )
+    service_root = context.get("/redfish/v1/")
     if "CertificateService" not in service_root.dict:
         # No event service
-        raise RedfishCertificateServiceNotFoundError( "Service does not contain a certificate service" )
+        raise RedfishCertificateServiceNotFoundError("Service does not contain a certificate service")
 
     # Get the certificate service
-    certificate_service = context.get( service_root.dict["CertificateService"]["@odata.id"] )
-    verify_response( certificate_service )
+    certificate_service = context.get(service_root.dict["CertificateService"]["@odata.id"])
+    verify_response(certificate_service)
     return certificate_service.dict
 
-def build_identifier_string( identifier ):
+
+def build_identifier_string(identifier):
     """
     Creates an identifier string for a subject or issuer object
 
     Args:
         identifier: The identifier object to parse
 
     Returns:
@@ -305,15 +337,15 @@
     field_map = {
         "CommonName": "CN",
         "Organization": "O",
         "OrganizationalUnit": "OU",
         "Country": "C",
         "State": "ST",
         "City": "L",
-        "Email": "emailAddress"
+        "Email": "emailAddress",
     }
 
     strings = []
     for map in field_map:
         if map in identifier and identifier[map] is not None:
-            strings.append( "{}={}".format( field_map[map], identifier[map] ) )
-    return ", ".join( strings )
+            strings.append("{}={}".format(field_map[map], identifier[map]))
+    return ", ".join(strings)
```

### Comparing `redfish_utilities-3.2.8/redfish_utilities/collections.py` & `redfish_utilities-3.2.9/redfish_utilities/collections.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,46 +10,51 @@
 
 Brief : This file contains the definitions and functionalities for performing
         operations with resource collections
 """
 
 from .messages import verify_response
 
-class RedfishCollectionNotFoundError( Exception ):
+
+class RedfishCollectionNotFoundError(Exception):
     """
     Raised when the specified collection is not found (HTTP Status = 404)
     """
+
     pass
 
-class RedfishCollectionMemberNotFoundError( Exception ):
+
+class RedfishCollectionMemberNotFoundError(Exception):
     """
     Raised when the specified member is not found (HTTP Status = 404)
     """
+
     pass
 
-def get_collection_ids( context, collection_uri ):
+
+def get_collection_ids(context, collection_uri):
     """
     Iterates over a collection and returns the identifiers of all members
 
     Args:
         context: The Redfish client object with an open session
         collection_uri: The URI of the collection to process
 
     Returns:
         A list of identifiers of the members of the collection
     """
 
     # Get the collection and iterate through its collection
     avail_members = []
-    collection = context.get( collection_uri )
+    collection = context.get(collection_uri)
     if collection.status == 404:
-        raise RedfishCollectionNotFoundError( "Service does not contain a collection at URI {}".format( collection_uri ) )
-    verify_response( collection )
+        raise RedfishCollectionNotFoundError("Service does not contain a collection at URI {}".format(collection_uri))
+    verify_response(collection)
     while True:
         for member in collection.dict["Members"]:
-            avail_members.append( member["@odata.id"].strip( "/" ).split( "/" )[-1] )
+            avail_members.append(member["@odata.id"].strip("/").split("/")[-1])
         if "Members@odata.nextLink" not in collection.dict:
             break
-        collection = context.get( collection.dict["Members@odata.nextLink"] )
-        verify_response( collection )
+        collection = context.get(collection.dict["Members@odata.nextLink"])
+        verify_response(collection)
 
     return avail_members
```

### Comparing `redfish_utilities-3.2.8/redfish_utilities/config.py` & `redfish_utilities-3.2.9/redfish_utilities/config.py`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.8/redfish_utilities/event_service.py` & `redfish_utilities-3.2.9/redfish_utilities/event_service.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,157 +10,179 @@
 
 Brief : This file contains the definitions and functionalities for managing
         accounts on a Redfish Service
 """
 
 from .messages import verify_response
 
-class RedfishEventServiceNotFoundError( Exception ):
+
+class RedfishEventServiceNotFoundError(Exception):
     """
     Raised when the event service cannot be found
     """
+
     pass
 
-class RedfishEventSubscriptionNotFoundError( Exception ):
+
+class RedfishEventSubscriptionNotFoundError(Exception):
     """
     Raised when the specified event subscription cannot be found
     """
+
     pass
 
-def get_event_service( context ):
+
+def get_event_service(context):
     """
     Collects the event service information from a Redfish service
 
     Args:
         context: The Redfish client object with an open session
 
     Returns:
         An object containing information about the event service
     """
 
     # Get the service root to find the event service
-    service_root = context.get( "/redfish/v1/" )
+    service_root = context.get("/redfish/v1/")
     if "EventService" not in service_root.dict:
         # No event service
-        raise RedfishEventServiceNotFoundError( "Service does not contain an event service" )
+        raise RedfishEventServiceNotFoundError("Service does not contain an event service")
 
     # Get the event service
-    event_service = context.get( service_root.dict["EventService"]["@odata.id"] )
+    event_service = context.get(service_root.dict["EventService"]["@odata.id"])
     return event_service.dict
 
-def print_event_service( service ):
+
+def print_event_service(service):
     """
     Prints the event service information from a Redfish service
 
     Args:
         service: The event service object
     """
 
-    print( "Service Info" )
+    print("Service Info")
 
     # General status
     status = "Enabled"
     if "ServiceEnabled" in service:
         if not service["ServiceEnabled"]:
             status = "Disabled"
     if "Status" in service:
         if "State" in service["Status"]:
             status = service["Status"]["State"]
-    print( "  Status: {}".format( status ) )
+    print("  Status: {}".format(status))
 
     # Delivery retry policy
     retry_policy = ""
     if "DeliveryRetryAttempts" in service:
-        retry_policy += "{} attempts, ".format( service["DeliveryRetryAttempts"] )
+        retry_policy += "{} attempts, ".format(service["DeliveryRetryAttempts"])
     if "DeliveryRetryIntervalSeconds" in service:
-        retry_policy += "{} second intervals, ".format( service["DeliveryRetryIntervalSeconds"] )
-    if len( retry_policy ) > 2:
+        retry_policy += "{} second intervals, ".format(service["DeliveryRetryIntervalSeconds"])
+    if len(retry_policy) > 2:
         retry_policy = retry_policy[:-2]
     else:
         retry_policy = "Unknown/Unspecified"
-    print( "  Delivery Retry Policy: {}".format( retry_policy ) )
+    print("  Delivery Retry Policy: {}".format(retry_policy))
 
     # Subscription methods
-    print( "  Event Types: {}".format( ", ".join( service.get( "EventTypesForSubscription", [ "N/A" ] ) ) ) )
-    print( "  Event Formats: {}".format( ", ".join( service.get( "EventFormatTypes", [ "N/A" ] ) ) ) )
-    print( "  Registries: {}".format( ", ".join( service.get( "RegistryPrefixes", [ "N/A" ] ) ) ) )
-    print( "  Resource Types: {}".format( ", ".join( service.get( "ResourceTypes", [ "N/A" ] ) ) ) )
-    print( "  Include Origin of Condition Supported: {}".format( service.get( "IncludeOriginOfConditionSupported", False ) ) )
+    print("  Event Types: {}".format(", ".join(service.get("EventTypesForSubscription", ["N/A"]))))
+    print("  Event Formats: {}".format(", ".join(service.get("EventFormatTypes", ["N/A"]))))
+    print("  Registries: {}".format(", ".join(service.get("RegistryPrefixes", ["N/A"]))))
+    print("  Resource Types: {}".format(", ".join(service.get("ResourceTypes", ["N/A"]))))
+    print("  Include Origin of Condition Supported: {}".format(service.get("IncludeOriginOfConditionSupported", False)))
 
     # SSE info
-    print( "  SSE URI: {}".format( service.get( "ServerSentEventUri", "Not supported" ) ) )
+    print("  SSE URI: {}".format(service.get("ServerSentEventUri", "Not supported")))
     sse_filters = ""
-    for filter in service.get( "SSEFilterPropertiesSupported", {} ):
+    for filter in service.get("SSEFilterPropertiesSupported", {}):
         if filter == "EventType":
             # This style is deprecated
             continue
         if service["SSEFilterPropertiesSupported"][filter]:
-            sse_filters += "{}, ".format( filter )
-    if len( sse_filters ) > 2:
+            sse_filters += "{}, ".format(filter)
+    if len(sse_filters) > 2:
         sse_filters = sse_filters[:-2]
     else:
         sse_filters = "Unknown/Unspecified"
-    print( "  SSE Filter Parameters: {}".format( sse_filters ) )
+    print("  SSE Filter Parameters: {}".format(sse_filters))
+
 
-def get_event_subscriptions( context ):
+def get_event_subscriptions(context):
     """
     Collects the event subscription information from a Redfish service
 
     Args:
         context: The Redfish client object with an open session
 
     Returns:
         A list containing all event subscriptions
     """
 
     # Get the event service
-    event_service = get_event_service( context )
+    event_service = get_event_service(context)
     if "Subscriptions" not in event_service:
         # No subscriptions
-        raise RedfishEventServiceNotFoundError( "Service does not contain a subscription collection" )
+        raise RedfishEventServiceNotFoundError("Service does not contain a subscription collection")
 
     # Get each of the event subscriptions
     subscriptions = []
-    subscription_col = context.get( event_service["Subscriptions"]["@odata.id"] )
+    subscription_col = context.get(event_service["Subscriptions"]["@odata.id"])
     for subscription_member in subscription_col.dict["Members"]:
-        subscription = context.get( subscription_member["@odata.id"] )
-        subscriptions.append( subscription.dict )
+        subscription = context.get(subscription_member["@odata.id"])
+        subscriptions.append(subscription.dict)
     return subscriptions
 
-def print_event_subscriptions( subscriptions ):
+
+def print_event_subscriptions(subscriptions):
     """
     Prints the event subscription information from a Redfish service
 
     Args:
         subscriptions: An array of event subscription objects
     """
 
     subscription_line_format = "  {:36s} | {}: {}"
 
-    print( "Subscription Info" )
+    print("Subscription Info")
 
-    if len( subscriptions ) == 0:
-        print( "  No subscriptions" )
+    if len(subscriptions) == 0:
+        print("  No subscriptions")
         return
 
     for subscription in subscriptions:
-        print( subscription_line_format.format( subscription["Id"], "Destination", subscription.get( "Destination", "N/A" ) ) )
-        print( subscription_line_format.format( "", "State", subscription.get( "Status", {} ).get( "State", "Enabled" ) ) )
+        print(
+            subscription_line_format.format(subscription["Id"], "Destination", subscription.get("Destination", "N/A"))
+        )
+        print(subscription_line_format.format("", "State", subscription.get("Status", {}).get("State", "Enabled")))
         if "Context" in subscription:
-            print( subscription_line_format.format( "", "Context", subscription["Context"] ) )
-        print( subscription_line_format.format( "", "Event Format", subscription.get( "EventFormatType", "Event" ) ) )
+            print(subscription_line_format.format("", "Context", subscription["Context"]))
+        print(subscription_line_format.format("", "Event Format", subscription.get("EventFormatType", "Event")))
         if "EventTypes" in subscription:
-            print( subscription_line_format.format( "", "Event Types", ", ".join(subscription["EventTypes"] ) ) )
+            print(subscription_line_format.format("", "Event Types", ", ".join(subscription["EventTypes"])))
         if "RegistryPrefixes" in subscription:
-            print( subscription_line_format.format( "", "Registries", ", ".join( subscription["RegistryPrefixes"] ) ) )
+            print(subscription_line_format.format("", "Registries", ", ".join(subscription["RegistryPrefixes"])))
         if "ResourceTypes" in subscription:
-            print( subscription_line_format.format( "", "Resource Types", ", ".join( subscription["ResourceTypes"] ) ) )
+            print(subscription_line_format.format("", "Resource Types", ", ".join(subscription["ResourceTypes"])))
 
-def create_event_subscription( context, destination, format = None, client_context = None, expand = None, resource_types = None,
-    registries = None, message_ids = None, origins = None, subordinate_resources = None, event_types = None ):
+
+def create_event_subscription(
+    context,
+    destination,
+    format=None,
+    client_context=None,
+    expand=None,
+    resource_types=None,
+    registries=None,
+    message_ids=None,
+    origins=None,
+    subordinate_resources=None,
+    event_types=None,
+):
     """
     Creates an event subscription
 
     Args:
         context: The Redfish client object with an open session
         destination: The event subscription destination
         format: The format of the event payloads
@@ -174,24 +196,21 @@
         event_types: The event types for the subscription; this method for subscriptions has been deprecated for other controls
 
     Returns:
         The response of the POST
     """
 
     # Get the event service
-    event_service = get_event_service( context )
+    event_service = get_event_service(context)
     if "Subscriptions" not in event_service:
         # No subscriptions
-        raise RedfishEventServiceNotFoundError( "Service does not contain a subscription collection" )
+        raise RedfishEventServiceNotFoundError("Service does not contain a subscription collection")
 
     # Form the POST request
-    payload = {
-        "Destination": destination,
-        "Protocol": "Redfish"
-    }
+    payload = {"Destination": destination, "Protocol": "Redfish"}
     if format is not None:
         payload["EventFormatType"] = format
     if client_context is not None:
         payload["Context"] = client_context
     if expand is not None:
         payload["IncludeOriginOfCondition"] = expand
     if resource_types is not None:
@@ -204,35 +223,36 @@
         payload["OriginResources"] = origins
     if subordinate_resources is not None:
         payload["SubordinateResources"] = subordinate_resources
     if event_types is not None:
         payload["EventTypes"] = event_types
 
     # Create the subscription
-    response = context.post( event_service["Subscriptions"]["@odata.id"], body = payload )
-    verify_response( response )
+    response = context.post(event_service["Subscriptions"]["@odata.id"], body=payload)
+    verify_response(response)
     return response
 
-def delete_event_subscription( context, id ):
+
+def delete_event_subscription(context, id):
     """
     Deletes an event subscription
 
     Args:
         context: The Redfish client object with an open session
         id: The identifier for the subscription
 
     Returns:
         The response of the DELETE
     """
 
     # Get the current subscriptions
-    subscriptions = get_event_subscriptions( context )
+    subscriptions = get_event_subscriptions(context)
 
     # Find the matching subscription and delete it
     for subscription in subscriptions:
         if subscription["Id"] == id:
-            response = context.delete( subscription["@odata.id"] )
-            verify_response( response )
+            response = context.delete(subscription["@odata.id"])
+            verify_response(response)
             return response
 
     # No matches found
-    raise RedfishEventSubscriptionNotFoundError( "Service does not contain an event subscription called {}".format( id ) )
+    raise RedfishEventSubscriptionNotFoundError("Service does not contain an event subscription called {}".format(id))
```

### Comparing `redfish_utilities-3.2.8/redfish_utilities/inventory.py` & `redfish_utilities-3.2.9/redfish_utilities/inventory.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,21 +14,24 @@
 
 import warnings
 import xlsxwriter
 from .collections import get_collection_ids
 from .messages import verify_response
 from . import config
 
-class RedfishChassisNotFoundError( Exception ):
+
+class RedfishChassisNotFoundError(Exception):
     """
     Raised when a matching chassis cannot be found
     """
+
     pass
 
-def get_system_inventory( context ):
+
+def get_system_inventory(context):
     """
     Walks a Redfish service for system component information, such as drives,
     processors, and memory
 
     Args:
         context: The Redfish client object with an open session
 
@@ -37,16 +40,16 @@
     """
 
     chassis_uri_pattern = "/redfish/v1/Chassis/{}"
     inventory_list = []
 
     # Get the set of chassis instances to initialize the structure
     try:
-        chassis_ids = get_chassis_ids( context )
-    except:
+        chassis_ids = get_chassis_ids(context)
+    except Exception:
         # No chassis instances
         return inventory_list
 
     # Set up the inventory list based on the chassis instances found
     # This is done prior to cataloging anything since depending on how links are used, some devices might point back to a chassis instance not yet cataloged
     for chassis_id in chassis_ids:
         chassis_instance = {
@@ -54,84 +57,91 @@
             "Chassis": [],
             "Processors": [],
             "Memory": [],
             "Drives": [],
             "PCIeDevices": [],
             "StorageControllers": [],
             "NetworkAdapters": [],
-            "Switches": []
+            "Switches": [],
         }
-        inventory_list.append( chassis_instance )
+        inventory_list.append(chassis_instance)
 
     # Go through each chassis and catalog the results
     for chassis_id in chassis_ids:
-        chassis_uri = chassis_uri_pattern.format( chassis_id )
-        chassis = context.get( chassis_uri )
+        chassis_uri = chassis_uri_pattern.format(chassis_id)
+        chassis = context.get(chassis_uri)
         try:
-            verify_response( chassis )
-        except:
+            verify_response(chassis)
+        except Exception:
             if config.__workarounds__:
-                warnings.warn( "Could not access '{}'.  Contact your vendor.  Skipping...".format( chassis_uri ) )
+                warnings.warn("Could not access '{}'.  Contact your vendor.  Skipping...".format(chassis_uri))
                 continue
             else:
                 raise
-        catalog_resource( context, chassis.dict, inventory_list, chassis_id )
+        catalog_resource(context, chassis.dict, inventory_list, chassis_id)
 
     return inventory_list
 
-def catalog_array( context, resource, name, inventory, chassis_id ):
+
+def catalog_array(context, resource, name, inventory, chassis_id):
     """
     Catalogs an array of resources for the inventory list
 
     Args:
         context: The Redfish client object with an open session
         resource: The resource with the array
         name: The name of the property of the array
         inventory: The inventory to update
         chassis_id: The identifier for the chassis being scanned
     """
 
     if name in resource:
         for member in resource[name]:
-            member_res = context.get( member["@odata.id"] )
+            member_res = context.get(member["@odata.id"])
             try:
-                verify_response( member_res )
-            except:
+                verify_response(member_res)
+            except Exception:
                 if config.__workarounds__:
-                    warnings.warn( "Could not access '{}'.  Contact your vendor.  Skipping...".format( member["@odata.id"] ) )
+                    warnings.warn(
+                        "Could not access '{}'.  Contact your vendor.  Skipping...".format(member["@odata.id"])
+                    )
                     continue
                 else:
                     raise
-            catalog_resource( context, member_res.dict, inventory, chassis_id )
+            catalog_resource(context, member_res.dict, inventory, chassis_id)
+
 
-def catalog_collection( context, resource, name, inventory, chassis_id ):
+def catalog_collection(context, resource, name, inventory, chassis_id):
     """
     Catalogs a collection of resources for the inventory list
 
     Args:
         context: The Redfish client object with an open session
         resource: The resource with the array
         name: The name of the property of the collection
         inventory: The inventory to update
         chassis_id: The identifier for the chassis being scanned
     """
 
     if name in resource:
-        collection = context.get( resource[name]["@odata.id"] )
+        collection = context.get(resource[name]["@odata.id"])
         try:
-            verify_response( collection )
-        except:
+            verify_response(collection)
+        except Exception:
             if config.__workarounds__:
-                warnings.warn( "Could not access '{}'.  Contact your vendor.  Skipping...".format( resource[name]["@odata.id"] ) )
+                warnings.warn(
+                    "Could not access '{}'.  Contact your vendor.  Skipping...".format(resource[name]["@odata.id"])
+                )
                 return
             else:
                 raise
-        catalog_array( context, collection.dict, "Members", inventory, chassis_id )
+        catalog_array(context, collection.dict, "Members", inventory, chassis_id)
 
-def catalog_resource( context, resource, inventory, chassis_id ):
+
+def catalog_resource(context, resource, inventory, chassis_id):
     """
     Catalogs a resource for the inventory list
 
     Args:
         context: The Redfish client object with an open session
         resource: The resource to catalog
         inventory: The inventory to update
@@ -139,153 +149,153 @@
     """
 
     resource_type = resource["@odata.type"].rsplit(".")[-1]
 
     # Based on the resource type, see if anything needs to be cataloged within it
     if resource_type == "Chassis":
         # Catalog all of the components within the chassis
-        catalog_collection( context, resource, "NetworkAdapters", inventory, chassis_id )
-        catalog_collection( context, resource, "Drives", inventory, chassis_id )
-        catalog_collection( context, resource, "PCIeDevices", inventory, chassis_id )
-        catalog_collection( context, resource, "Memory", inventory, chassis_id )
+        catalog_collection(context, resource, "NetworkAdapters", inventory, chassis_id)
+        catalog_collection(context, resource, "Drives", inventory, chassis_id)
+        catalog_collection(context, resource, "PCIeDevices", inventory, chassis_id)
+        catalog_collection(context, resource, "Memory", inventory, chassis_id)
         if "Links" in resource:
-            catalog_array( context, resource["Links"], "Drives", inventory, chassis_id )
-            catalog_array( context, resource["Links"], "PCIeDevices", inventory, chassis_id )
-            catalog_array( context, resource["Links"], "Switches", inventory, chassis_id )
-            catalog_array( context, resource["Links"], "ComputerSystems", inventory, chassis_id )
+            catalog_array(context, resource["Links"], "Drives", inventory, chassis_id)
+            catalog_array(context, resource["Links"], "PCIeDevices", inventory, chassis_id)
+            catalog_array(context, resource["Links"], "Switches", inventory, chassis_id)
+            catalog_array(context, resource["Links"], "ComputerSystems", inventory, chassis_id)
     elif resource_type == "ComputerSystem":
         # Catalog all of the components within the system
-        catalog_collection( context, resource, "Processors", inventory, chassis_id )
-        catalog_collection( context, resource, "Memory", inventory, chassis_id )
-        catalog_collection( context, resource, "SimpleStorage", inventory, chassis_id )
-        catalog_collection( context, resource, "Storage", inventory, chassis_id )
+        catalog_collection(context, resource, "Processors", inventory, chassis_id)
+        catalog_collection(context, resource, "Memory", inventory, chassis_id)
+        catalog_collection(context, resource, "SimpleStorage", inventory, chassis_id)
+        catalog_collection(context, resource, "Storage", inventory, chassis_id)
         # The system itself does not get cataloged (the chassis representation should cover this)
         return
     elif resource_type == "Storage":
         # Catalog the drives and storage controllers in the storage subsystem
-        catalog_array( context, resource, "Drives", inventory, chassis_id )
+        catalog_array(context, resource, "Drives", inventory, chassis_id)
         if "StorageControllers" in resource:
-            for index, controller in enumerate( resource["StorageControllers"] ):
+            for index, controller in enumerate(resource["StorageControllers"]):
                 controller["@odata.type"] = "#StorageController.StorageController"
                 controller["Id"] = controller["MemberId"]
-                catalog_resource( context, controller, inventory, chassis_id )
+                catalog_resource(context, controller, inventory, chassis_id)
         # The storage subsystem itself does not get cataloged
         return
     elif resource_type == "SimpleStorage":
         # If there is a full storage representation of this resource, skip it
         if "Links" in resource:
             if "Storage" in resource["Links"]:
                 return
 
         # Catalog the devices (as drives)
         if "Devices" in resource:
-            for index, drive in enumerate( resource["Devices"] ):
-                drive["@odata.id"] = "{}#/Devices/{}".format( resource["@odata.id"], index )
+            for index, drive in enumerate(resource["Devices"]):
+                drive["@odata.id"] = "{}#/Devices/{}".format(resource["@odata.id"], index)
                 drive["@odata.type"] = "#Drive.Drive"
                 drive["Id"] = drive["Name"]
-                catalog_resource( context, drive, inventory, chassis_id )
+                catalog_resource(context, drive, inventory, chassis_id)
         # The simple storage subsystem itself does not get cataloged
         return
 
     # If the resource has a pointer back to chassis, use the identifier in the link for cataloging
     if "Links" in resource:
         if "Chassis" in resource["Links"]:
-            if isinstance( resource["Links"]["Chassis"], dict ):
-                chassis_id = resource["Links"]["Chassis"]["@odata.id"].strip( "/" ).split( "/" )[-1]
+            if isinstance(resource["Links"]["Chassis"], dict):
+                chassis_id = resource["Links"]["Chassis"]["@odata.id"].strip("/").split("/")[-1]
 
     # Determine the location property
     location_prop = "Location"
     if resource_type == "Drive":
         location_prop = "PhysicalLocation"
 
     # Pull out all relevant properties for the catalog
     catalog = {
         "Uri": resource["@odata.id"],
-        "PartNumber": resource.get( "PartNumber", None ),
-        "SerialNumber": resource.get( "SerialNumber", None ),
-        "Manufacturer": resource.get( "Manufacturer", None ),
-        "Model": resource.get( "Model", None ),
-        "SKU": resource.get( "SKU", None ),
-        "AssetTag": resource.get( "AssetTag", None ),
+        "PartNumber": resource.get("PartNumber", None),
+        "SerialNumber": resource.get("SerialNumber", None),
+        "Manufacturer": resource.get("Manufacturer", None),
+        "Model": resource.get("Model", None),
+        "SKU": resource.get("SKU", None),
+        "AssetTag": resource.get("AssetTag", None),
         "Label": None,
         "State": None,
-        "Description": None
+        "Description": None,
     }
     # For nested properties, need to protect against malformed payloads to avoid exceptions
     try:
-        catalog["Label"] = resource.get( location_prop, {} ).get( "PartLocation", {} ).get( "ServiceLabel", None )
-    except:
+        catalog["Label"] = resource.get(location_prop, {}).get("PartLocation", {}).get("ServiceLabel", None)
+    except Exception:
         pass
     try:
-        catalog["State"] = resource.get( "Status", {} ).get( "State", None )
-    except:
+        catalog["State"] = resource.get("Status", {}).get("State", None)
+    except Exception:
         pass
     # Ensure all fields are strings
     for item in catalog:
-        if not isinstance( catalog[item], str ):
+        if not isinstance(catalog[item], str):
             catalog[item] = None
 
     # If no label was found, build a default name
     if catalog["Label"] is None:
         catalog["Label"] = resource_type + ": " + resource["Id"]
 
     # Build a string description of the component based on other properties
     entry_tag = None
     prop_list = []
     if resource_type == "Chassis":
         entry_tag = "Chassis"
-        prop_list = [ "Model" ]
+        prop_list = ["Model"]
     elif resource_type == "Processor":
         entry_tag = "Processors"
         if catalog["Model"] is not None:
-            prop_list = [ "Model" ]
+            prop_list = ["Model"]
         else:
-            prop_list = [ "Manufacturer", "ProcessorArchitecture", "ProcessorType", "TotalCores", "MaxSpeedMHz" ]
+            prop_list = ["Manufacturer", "ProcessorArchitecture", "ProcessorType", "TotalCores", "MaxSpeedMHz"]
     elif resource_type == "Memory":
         entry_tag = "Memory"
-        prop_list = [ "Manufacturer", "CapacityMiB", "MemoryDeviceType", "MemoryType" ]
+        prop_list = ["Manufacturer", "CapacityMiB", "MemoryDeviceType", "MemoryType"]
     elif resource_type == "Drive":
         entry_tag = "Drives"
-        prop_list = [ "Manufacturer", "CapacityBytes", "Protocol", "MediaType" ]
+        prop_list = ["Manufacturer", "CapacityBytes", "Protocol", "MediaType"]
     elif resource_type == "PCIeDevice":
         entry_tag = "PCIeDevices"
-        prop_list = [ "Manufacturer", "Model", "DeviceType", "PCIeInterface" ]
+        prop_list = ["Manufacturer", "Model", "DeviceType", "PCIeInterface"]
     elif resource_type == "StorageController":
         entry_tag = "StorageControllers"
-        prop_list = [ "Manufacturer", "SpeedGbps", "SupportedDeviceProtocols" ]
+        prop_list = ["Manufacturer", "SpeedGbps", "SupportedDeviceProtocols"]
     elif resource_type == "NetworkAdapter":
         entry_tag = "NetworkAdapters"
-        prop_list = [ "Manufacturer", "Model" ]
+        prop_list = ["Manufacturer", "Model"]
     elif resource_type == "Switch":
         entry_tag = "Switches"
-        prop_list = [ "Manufacturer", "Model" ]
+        prop_list = ["Manufacturer", "Model"]
     if entry_tag is None:
         # No handling set up for this resource type
         # Should not happen; check the types against the possible lists
         return
 
     # Based on the listed properties for the resource type, build the description string
     if catalog["State"] != "Absent":
         description_str = ""
         for prop in prop_list:
-            if resource.get( prop, None ) is not None:
+            if resource.get(prop, None) is not None:
                 prop_val = resource[prop]
                 # Some properties require refinement
                 if prop == "TotalCores":
-                    prop_val = str( prop_val ) + " Cores"
+                    prop_val = str(prop_val) + " Cores"
                 elif prop == "MaxSpeedMHz":
-                    prop_val = "@ " + str( prop_val ) + "MHz"
+                    prop_val = "@ " + str(prop_val) + "MHz"
                 elif prop == "CapacityMiB":
-                    prop_val = str( prop_val ) + "MB"
+                    prop_val = str(prop_val) + "MB"
                 elif prop == "CapacityBytes":
-                    prop_val = str( int( prop_val / ( 2 ** 30 ) ) ) + "GB"
+                    prop_val = str(int(prop_val / (2**30))) + "GB"
                 elif prop == "SpeedGbps":
-                    prop_val = str( prop_val ) + "Gbps"
+                    prop_val = str(prop_val) + "Gbps"
                 elif prop == "SupportedDeviceProtocols":
-                    prop_val = "/".join( prop_val ) + " Controller"
+                    prop_val = "/".join(prop_val) + " Controller"
                 elif prop == "DeviceType":
                     prop_val = prop_val + " PCIe Device"
                 elif prop == "PCIeInterface":
                     if "MaxPCIeType" in prop_val:
                         prop_val = "@" + " " + prop_val["MaxPCIeType"]
                     else:
                         continue
@@ -307,17 +317,18 @@
         # No matching spot to put this entry in the inventory
         return
     # Check if this is a new entry
     for item in inventory_instance[entry_tag]:
         if item["Uri"] == resource["@odata.id"]:
             return
 
-    inventory_instance[entry_tag].append( catalog )
+    inventory_instance[entry_tag].append(catalog)
+
 
-def print_system_inventory( inventory_list, details = False, skip_absent = False ):
+def print_system_inventory(inventory_list, details=False, skip_absent=False):
     """
     Prints the system inventory list into a table
 
     Args:
         inventory_list: The inventory list to print
         details: True to print all of the detailed info
         skip_absent: True to skip printing absent components
@@ -325,90 +336,110 @@
 
     inventory_line_format = "  {:35s} | {}"
     inventory_line_format_detail = "  {:35s} | {}: {}"
     inventory_line_format_empty = "  {:35s} | Not Present"
 
     # Go through each chassis instance
     for chassis in inventory_list:
-        print( "'" + chassis["ChassisName"] + "' Inventory" )
-        print( inventory_line_format.format( "Name", "Description" ) )
+        print("'" + chassis["ChassisName"] + "' Inventory")
+        print(inventory_line_format.format("Name", "Description"))
 
         # Go through each component type in the chassis
-        type_list = [ "Chassis", "Processors", "Memory", "Drives", "PCIeDevices", "StorageControllers", "NetworkAdapters", "Switches" ]
+        type_list = [
+            "Chassis",
+            "Processors",
+            "Memory",
+            "Drives",
+            "PCIeDevices",
+            "StorageControllers",
+            "NetworkAdapters",
+            "Switches",
+        ]
         for inv_type in type_list:
             # Go through each component and prints its info
             for item in chassis[inv_type]:
                 if item["State"] == "Absent":
                     if not skip_absent:
-                        print( inventory_line_format_empty.format( item["Label"][:35] ) )
+                        print(inventory_line_format_empty.format(item["Label"][:35]))
                 else:
-                    print( inventory_line_format.format( item["Label"][:35], item["Description"] ) )
+                    print(inventory_line_format.format(item["Label"][:35], item["Description"]))
 
                     if details:
-                        detail_list = [ "Manufacturer", "Model", "SKU", "PartNumber", "SerialNumber", "AssetTag" ]
+                        detail_list = ["Manufacturer", "Model", "SKU", "PartNumber", "SerialNumber", "AssetTag"]
                         for detail in detail_list:
                             if item[detail] is not None:
-                                print( inventory_line_format_detail.format( "", detail, item[detail] ) )
-        print( "" )
+                                print(inventory_line_format_detail.format("", detail, item[detail]))
+        print("")
 
-def write_system_inventory( inventory_list, file_name ):
+
+def write_system_inventory(inventory_list, file_name):
     """
     Write the system inventory list into a spreadsheet
 
     Args:
         inventory_list: The inventory list to write to an Excel spreadsheet
         file_name: The name of the file for the spreadsheet
     """
 
     # Excel workbook to save data extracted and parsed
-    workbook = xlsxwriter.Workbook( "./{}.xlsx".format( file_name ) )
+    workbook = xlsxwriter.Workbook("./{}.xlsx".format(file_name))
 
-    worksheet = workbook.add_worksheet( "Device Inventory" )
-    cell_header_format = workbook.add_format( { 'bold': True, 'bg_color': 'yellow' } )
-    cell_name_format = workbook.add_format( { 'bold': True } )
+    worksheet = workbook.add_worksheet("Device Inventory")
+    cell_header_format = workbook.add_format({"bold": True, "bg_color": "yellow"})
+    cell_name_format = workbook.add_format({"bold": True})
 
     column = 0
     row = 0
 
     # Adds header to Excel file
-    header = [ "NAME", "DESCRIPTION", "MANUFACTURER", "MODEL", "SKU", "PART NUMBER", "SERIAL NUMBER", "ASSET TAG" ]
+    header = ["NAME", "DESCRIPTION", "MANUFACTURER", "MODEL", "SKU", "PART NUMBER", "SERIAL NUMBER", "ASSET TAG"]
     for column_title in header:
-        worksheet.write( row, column, column_title, cell_header_format )
+        worksheet.write(row, column, column_title, cell_header_format)
         column += 1
     row = 1
 
     for chassis in inventory_list:
         # Go through each component type in the chassis
-        type_list = [ "Chassis", "Processors", "Memory", "Drives", "PCIeDevices", "StorageControllers", "NetworkAdapters", "Switches" ]
+        type_list = [
+            "Chassis",
+            "Processors",
+            "Memory",
+            "Drives",
+            "PCIeDevices",
+            "StorageControllers",
+            "NetworkAdapters",
+            "Switches",
+        ]
         for inv_type in type_list:
             # Go through each component and prints its info
             for item in chassis[inv_type]:
                 column = 0
-                worksheet.write( row, column, inv_type, cell_name_format )
+                worksheet.write(row, column, inv_type, cell_name_format)
                 column += 1
-                detail_list = [ "Description", "Manufacturer", "Model", "SKU", "PartNumber", "SerialNumber", "AssetTag" ]
+                detail_list = ["Description", "Manufacturer", "Model", "SKU", "PartNumber", "SerialNumber", "AssetTag"]
                 for detail in detail_list:
-                    worksheet.write( row, column, item[detail] )
+                    worksheet.write(row, column, item[detail])
                     column += 1
                 row += 1
 
     workbook.close()
 
-def get_chassis_ids( context ):
+
+def get_chassis_ids(context):
     """
     Finds the chassis collection and returns all of the member's identifiers
 
     Args:
         context: The Redfish client object with an open session
 
     Returns:
         A list of identifiers of the members of the chassis collection
     """
 
     # Get the service root to find the chassis collection
-    service_root = context.get( "/redfish/v1/" )
+    service_root = context.get("/redfish/v1/")
     if "Chassis" not in service_root.dict:
         # No chassis collection
-        raise RedfishChassisNotFoundError( "Service does not contain a chassis collection" )
+        raise RedfishChassisNotFoundError("Service does not contain a chassis collection")
 
     # Get the chassis collection and iterate through its collection
-    return get_collection_ids( context, service_root.dict["Chassis"]["@odata.id"] )
+    return get_collection_ids(context, service_root.dict["Chassis"]["@odata.id"])
```

### Comparing `redfish_utilities-3.2.8/redfish_utilities/licenses.py` & `redfish_utilities-3.2.9/redfish_utilities/licenses.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,206 +13,235 @@
 """
 
 import base64
 import os
 from .collections import get_collection_ids
 from .messages import verify_response
 
-class RedfishLicenseServiceNotFoundError( Exception ):
+
+class RedfishLicenseServiceNotFoundError(Exception):
     """
     Raised when the license service cannot be found
     """
+
     pass
 
-class RedfishLicenseCollectionNotFoundError( Exception ):
+
+class RedfishLicenseCollectionNotFoundError(Exception):
     """
     Raised when the license collection cannot be found
     """
+
     pass
 
-class RedfishLicenseNotFoundError( Exception ):
+
+class RedfishLicenseNotFoundError(Exception):
     """
     Raised when a specific license cannot be found
     """
+
     pass
 
-class RedfishInstallLicenseNotFoundError( Exception ):
+
+class RedfishInstallLicenseNotFoundError(Exception):
     """
     Raised when the license service does not contain the Install action
     """
+
     pass
 
-def get_licenses( context ):
+
+def get_licenses(context):
     """
     Collects license information from a Redfish service
 
     Args:
         context: The Redfish client object with an open session
 
     Returns:
         A list containing all licenses
     """
 
     license_list = []
-    license_collection = get_license_collection( context )
+    license_collection = get_license_collection(context)
 
     # Get the identifiers of the collection
-    license_col = get_collection_ids( context, license_collection )
+    license_col = get_collection_ids(context, license_collection)
 
     # Get each member and add it to the response list
     for license_id in license_col:
-        license = context.get( license_collection + "/" + license_id )
-        verify_response( license )
-        license_list.append( license.dict )
+        license = context.get(license_collection + "/" + license_id)
+        verify_response(license)
+        license_list.append(license.dict)
 
     return license_list
 
-def print_licenses( license_list, details = False ):
+
+def print_licenses(license_list, details=False):
     """
     Prints the license list into a table
 
     Args:
         license_list: The license list to print
         details: True to print all the detailed info
     """
 
     license_format = "  {:30s} | {}"
     license_format_detail = "  {:30s} | {}: {}"
     info_properties = [
-        { "Format": "{}", "Property": "EntitlementId" },
-        { "Format": "Installed on {}", "Property": "InstallDate" },
-        { "Format": "Expires on {}", "Property": "ExpirationDate" }
+        {"Format": "{}", "Property": "EntitlementId"},
+        {"Format": "Installed on {}", "Property": "InstallDate"},
+        {"Format": "Expires on {}", "Property": "ExpirationDate"},
+    ]
+    detail_list = [
+        "Description",
+        "LicenseType",
+        "LicenseOrigin",
+        "Removable",
+        "Manufacturer",
+        "SKU",
+        "PartNumber",
+        "SerialNumber",
+        "AuthorizationScope",
+        "MaxAuthorizedDevices",
+        "RemainingUseCount",
     ]
-    detail_list = [ "Description", "LicenseType", "LicenseOrigin", "Removable", "Manufacturer", "SKU", "PartNumber",
-                    "SerialNumber", "AuthorizationScope", "MaxAuthorizedDevices", "RemainingUseCount" ]
 
-    print( "" )
-    print( license_format.format( "License", "Details" ) )
+    print("")
+    print(license_format.format("License", "Details"))
 
     # Go through each license
     for license in license_list:
         info_list = []
         # Build the general info string
         for info in info_properties:
             if info["Property"] in license:
-                info_string = info["Format"].format( license[info["Property"]] )
+                info_string = info["Format"].format(license[info["Property"]])
             else:
                 if info["Property"] == "EntitlementId":
                     # Fallback to ensure there is always something to show
                     info_string = "License " + license["Id"]
-            info_list.append( info_string )
+            info_list.append(info_string)
 
         # Print the license info
-        print( license_format.format( license["Id"], ", ".join( info_list ) ) )
+        print(license_format.format(license["Id"], ", ".join(info_list)))
 
         # Print details if requested
         if details:
             for detail in detail_list:
                 if detail in license:
-                    print( license_format_detail.format( "", detail, license[detail] ) )
+                    print(license_format_detail.format("", detail, license[detail]))
 
-    print( "" )
+    print("")
 
-def install_license( context, license_path ):
+
+def install_license(context, license_path):
     """
     Installs a new license
 
     Args:
         context: The Redfish client object with an open session
         license_path: The filepath or URI of the license to install
 
     Returns:
         The response of the operation
     """
 
     # Get the license service
-    license_service = get_license_service( context )
+    license_service = get_license_service(context)
 
     # Determine which installation method to use based on the provided license path
-    if os.path.isfile( license_path ):
+    if os.path.isfile(license_path):
         # Local file; perform via a POST to the license collection
         if "Licenses" not in license_service:
-            raise RedfishLicenseCollectionNotFoundError( "The license service does not contain a license collection" )
+            raise RedfishLicenseCollectionNotFoundError("The license service does not contain a license collection")
         install_uri = license_service["Licenses"]["@odata.id"]
 
         # Read in the file and convert it to a Base64-encoded string
-        with open( license_path, "rb") as file:
+        with open(license_path, "rb") as file:
             license_file = file.read()
-        payload = { "LicenseString": base64.b64encode(license_file).decode( "utf-8" ) }
+        payload = {"LicenseString": base64.b64encode(license_file).decode("utf-8")}
     else:
         # Remote file; perform via a POST to the Install action
         if "Actions" not in license_service:
-            raise RedfishInstallLicenseNotFoundError( "The license service does not contain actions")
+            raise RedfishInstallLicenseNotFoundError("The license service does not contain actions")
         if "#LicenseService.Install" not in license_service["Actions"]:
-            raise RedfishInstallLicenseNotFoundError( "The license service does not contain the Install action" )
+            raise RedfishInstallLicenseNotFoundError("The license service does not contain the Install action")
         install_uri = license_service["Actions"]["#LicenseService.Install"]["target"]
 
-        payload = { "LicenseFileURI": license_path }
+        payload = {"LicenseFileURI": license_path}
 
     # Install the license
-    response = context.post( install_uri, body = payload )
-    verify_response( response )
+    response = context.post(install_uri, body=payload)
+    verify_response(response)
     return response
 
-def delete_license( context, license_id ):
+
+def delete_license(context, license_id):
     """
     Deletes a license
 
     Args:
         context: The Redfish client object with an open session
         license_id: The identifier of the license to delete
 
     Returns:
         The response of the operation
     """
 
     # Get the identifiers of the collection
     license_collection = get_license_collection(context)
-    avail_licenses = get_collection_ids( context, license_collection )
+    avail_licenses = get_collection_ids(context, license_collection)
     if license_id not in avail_licenses:
-        raise RedfishLicenseNotFoundError( "License service does not contain the license '{}'; available licenses: {}".format( license_id, ", ".join( avail_licenses ) ) )
+        raise RedfishLicenseNotFoundError(
+            "License service does not contain the license '{}'; available licenses: {}".format(
+                license_id, ", ".join(avail_licenses)
+            )
+        )
 
     # Delete the requested license
-    response = context.delete( license_collection + "/" + license_id )
-    verify_response( response )
+    response = context.delete(license_collection + "/" + license_id)
+    verify_response(response)
     return response
 
-def get_license_service( context ):
+
+def get_license_service(context):
     """
     Collects the license service information from a Redfish service
 
     Args:
         context: The Redfish client object with an open session
 
     Returns:
         An object containing information about the license service
     """
 
     # Get the service root to find the license service
-    service_root = context.get( "/redfish/v1/" )
+    service_root = context.get("/redfish/v1/")
     if "LicenseService" not in service_root.dict:
         # No event service
-        raise RedfishLicenseServiceNotFoundError( "Service does not contain a license service" )
+        raise RedfishLicenseServiceNotFoundError("Service does not contain a license service")
 
     # Get the license service
-    license_service = context.get( service_root.dict["LicenseService"]["@odata.id"] )
-    verify_response( license_service )
+    license_service = context.get(service_root.dict["LicenseService"]["@odata.id"])
+    verify_response(license_service)
     return license_service.dict
 
-def get_license_collection( context ):
+
+def get_license_collection(context):
     """
     Finds the license collection for the Redfish service
 
     Args:
         context: The Redfish client object with an open session
 
     Returns:
         The URI for the license collection
     """
 
     # Get the license service to find the license collection
-    license_service = get_license_service( context )
+    license_service = get_license_service(context)
     if "Licenses" not in license_service:
         # No license collection
-        raise RedfishLicenseCollectionNotFoundError( "Service does not contain a license collection" )
+        raise RedfishLicenseCollectionNotFoundError("Service does not contain a license collection")
 
-    return license_service["Licenses"]["@odata.id"]
+    return license_service["Licenses"]["@odata.id"]
```

### Comparing `redfish_utilities-3.2.8/redfish_utilities/logs.py` & `redfish_utilities-3.2.9/redfish_utilities/logs.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,145 +13,187 @@
 """
 
 import shutil
 
 from .messages import verify_response
 from enum import Enum
 
-class RedfishLogServiceNotFoundError( Exception ):
+
+class RedfishLogServiceNotFoundError(Exception):
     """
     Raised when a matching log service cannot be found
     """
+
     pass
 
-class RedfishClearLogNotFoundError( Exception ):
+
+class RedfishClearLogNotFoundError(Exception):
     """
     Raised when a log service does not contain the clear log action
     """
+
     pass
 
-class RedfishCollectDiagnosticDataNotFoundError( Exception ):
+
+class RedfishCollectDiagnosticDataNotFoundError(Exception):
     """
     Raised when a log service does not contain the collect diagnostic data action
     """
+
     pass
 
-class RedfishDiagnosticDataNotFoundError( Exception ):
+
+class RedfishDiagnosticDataNotFoundError(Exception):
     """
     Raised when the requested diagnostic data cannot be found
     """
+
     pass
 
-class log_container( Enum ):
+
+class log_container(Enum):
     """
     Types of resources that contain log services
     """
+
     MANAGER = "Managers"
     CHASSIS = "Chassis"
     SYSTEM = "Systems"
 
-class diagnostic_data_types( Enum ):
+
+class diagnostic_data_types(Enum):
     """
     Types of diagnostic data that can be requested
     """
+
     MANAGER = "Manager"
     PRE_OS = "PreOS"
     OS = "OS"
     OEM = "OEM"
 
-    def __str__( self ):
+    def __str__(self):
         return self.value
 
-def get_log_entries( context, container_type = log_container.MANAGER, container_id = None, log_service_id = None ):
+
+def get_log_entries(context, container_type=log_container.MANAGER, container_id=None, log_service_id=None):
     """
     Finds the log entries of a log service matching the given ID
 
     Args:
         context: The Redfish client object with an open session
         container_type: The type of resource containing the log service (manager, system, or chassis)
         container_id: The container instance with the log service; if None, perform on the only container
         log_service_id: The log service with the logs; if None, perform on the only log service
 
     Returns:
         An array of log entries
     """
 
-    log_service = get_log_service( context, container_type, container_id, log_service_id )
+    log_service = get_log_service(context, container_type, container_id, log_service_id)
 
     # Read in the log entries
     log_entries = []
-    log_entry_col = context.get( log_service.dict["Entries"]["@odata.id"] )
-    log_entries.extend( log_entry_col.dict["Members"] )
+    log_entry_col = context.get(log_service.dict["Entries"]["@odata.id"])
+    log_entries.extend(log_entry_col.dict["Members"])
 
     # If a next link is provided, iterate over it and add to the log entry list
     while "Members@odata.nextLink" in log_entry_col.dict:
-        log_entry_col = context.get( log_entry_col.dict["Members@odata.nextLink"] )
-        log_entries.extend( log_entry_col.dict["Members"] )
+        log_entry_col = context.get(log_entry_col.dict["Members@odata.nextLink"])
+        log_entries.extend(log_entry_col.dict["Members"])
 
     return log_entries
 
-def print_log_entries( log_entries, details = False ):
+
+def print_log_entries(log_entries, details=False):
     """
     Prints a set of log entries in a table
 
     Args:
         log_entries: The log entries to print
         details: Flag indicating if details should be displayed
     """
 
     # Set up templates
     console_size = shutil.get_terminal_size(fallback=(80, 24))
     message_size = console_size.columns - 38
     entry_line_format = "  {:5s} | {:25s} | {}"
     detail_line_format = "  {:33s} | {}: {}"
-    detail_list = [ "Severity", "EntryType", "OemRecordFormat", "EntryCode", "OemLogEntryCode", "SensorType", "OemSensorType",
-        "GeneratorId", "SensorNumber", "EventType", "EventId", "EventGroupId", "MessageId", "MessageArgs" ]
-    print( entry_line_format.format( "Id", "Timestamp", "Message" ) )
+    detail_list = [
+        "Severity",
+        "EntryType",
+        "OemRecordFormat",
+        "EntryCode",
+        "OemLogEntryCode",
+        "SensorType",
+        "OemSensorType",
+        "GeneratorId",
+        "SensorNumber",
+        "EventType",
+        "EventId",
+        "EventGroupId",
+        "MessageId",
+        "MessageArgs",
+    ]
+    print(entry_line_format.format("Id", "Timestamp", "Message"))
 
     # Go through each entry and print the info
     for entry in log_entries:
         timestamp_property = "Created"
         if "EventTimestamp" in entry:
             timestamp_property = "EventTimestamp"
-        print( entry_line_format.format( entry["Id"], entry.get( timestamp_property, "Unknown" ), entry["Message"].replace( "\n", "; " )[:message_size] ) )
+        print(
+            entry_line_format.format(
+                entry["Id"],
+                entry.get(timestamp_property, "Unknown"),
+                entry["Message"].replace("\n", "; ")[:message_size],
+            )
+        )
         if details:
             for detail in detail_list:
                 if detail in entry:
-                    print( detail_line_format.format( "", detail, entry[detail] ) )
+                    print(detail_line_format.format("", detail, entry[detail]))
 
-def clear_log_entries( context, container_type = log_container.MANAGER, container_id = None, log_service_id = None ):
+
+def clear_log_entries(context, container_type=log_container.MANAGER, container_id=None, log_service_id=None):
     """
     Clears the log entries of a log service matching the given ID
 
     Args:
         context: The Redfish client object with an open session
         container_type: The type of resource containing the log service (manager, system, or chassis)
         container_id: The container instance with the log service; if None, perform on the only container
         log_service_id: The log service with the logs; if None, perform on the only log service
 
     Returns:
         The response of the action
     """
 
-    log_service = get_log_service( context, container_type, container_id, log_service_id )
+    log_service = get_log_service(context, container_type, container_id, log_service_id)
 
     # Find the ClearLog action
     if "Actions" not in log_service.dict:
-        raise RedfishClearLogNotFoundError( "Log service does not support ClearLog" )
+        raise RedfishClearLogNotFoundError("Log service does not support ClearLog")
     if "#LogService.ClearLog" not in log_service.dict["Actions"]:
-        raise RedfishClearLogNotFoundError( "Log service does not support ClearLog" )
+        raise RedfishClearLogNotFoundError("Log service does not support ClearLog")
     clear_uri = log_service.dict["Actions"]["#LogService.ClearLog"]["target"]
 
     # Clear the log
-    response = context.post( clear_uri, body = {} )
-    verify_response( response )
+    response = context.post(clear_uri, body={})
+    verify_response(response)
     return response
 
-def collect_diagnostic_data( context, container_type = log_container.MANAGER, container_id = None, log_service_id = None,
-    diagnostic_data_type = None, oem_data_type = None ):
+
+def collect_diagnostic_data(
+    context,
+    container_type=log_container.MANAGER,
+    container_id=None,
+    log_service_id=None,
+    diagnostic_data_type=None,
+    oem_data_type=None,
+):
     """
     Performs diagnostic data collection of a log service matching the given ID
 
     Args:
         context: The Redfish client object with an open session
         container_type: The type of resource containing the log service (manager, system, or chassis)
         container_id: The container instance with the log service; if None, perform on the only container
@@ -159,122 +201,147 @@
         diagnostic_data_type: The type of diagnostic data to collect (manager, pre OS, OS, OEM)
         oem_data_type: The type of OEM data to collect
 
     Returns:
         The response of the action
     """
 
-    log_service = get_log_service( context, container_type, container_id, log_service_id )
+    log_service = get_log_service(context, container_type, container_id, log_service_id)
 
     # Find the ClearLog action
     if "Actions" not in log_service.dict:
-        raise RedfishCollectDiagnosticDataNotFoundError( "Log service does not support CollectDiagnosticData" )
+        raise RedfishCollectDiagnosticDataNotFoundError("Log service does not support CollectDiagnosticData")
     if "#LogService.CollectDiagnosticData" not in log_service.dict["Actions"]:
-        raise RedfishCollectDiagnosticDataNotFoundError( "Log service does not support CollectDiagnosticData" )
+        raise RedfishCollectDiagnosticDataNotFoundError("Log service does not support CollectDiagnosticData")
     collect_uri = log_service.dict["Actions"]["#LogService.CollectDiagnosticData"]["target"]
 
     # Collect diagnostic data
     if diagnostic_data_type is None:
         diagnostic_data_type = diagnostic_data_types.MANAGER
-    payload = { "DiagnosticDataType": diagnostic_data_type.value }
+    payload = {"DiagnosticDataType": diagnostic_data_type.value}
     if oem_data_type is not None and diagnostic_data_type == diagnostic_data_types.OEM:
         # Only include OEMDiagnosticDataType if the OEM type is requested
         payload["OEMDiagnosticDataType"] = oem_data_type
-    response = context.post( collect_uri, body = payload )
-    verify_response( response )
+    response = context.post(collect_uri, body=payload)
+    verify_response(response)
     return response
 
-def download_diagnostic_data( context, collect_response ):
+
+def download_diagnostic_data(context, collect_response):
     """
     Downloads the diagnostic data based on the response from the collect action
 
     Args:
         context: The Redfish client object with an open session
         collect_response: The response object from the collect diagnostic data action
 
     Returns:
         The name of the file downloaded from the service
         An array of bytes containing the file contents
     """
 
     # Follow the Location header to the log entry
-    entry_uri = collect_response.getheader( "Location" )
+    entry_uri = collect_response.getheader("Location")
     if entry_uri is None:
-        raise RedfishDiagnosticDataNotFoundError( "The response to collecting diagnostic data does not contain a location for the data" )
+        raise RedfishDiagnosticDataNotFoundError(
+            "The response to collecting diagnostic data does not contain a location for the data"
+        )
 
     # Get the log entry
-    response = context.get( entry_uri )
+    response = context.get(entry_uri)
     if "AdditionalDataURI" not in response.dict:
-        raise RedfishDiagnosticDataNotFoundError( "The log entry for the collected data does not contain an additional data link" )
+        raise RedfishDiagnosticDataNotFoundError(
+            "The log entry for the collected data does not contain an additional data link"
+        )
 
     # Download the file
-    filename = response.dict["AdditionalDataURI"].split( "/" )[-1]
-    response = context.get( response.dict["AdditionalDataURI"] )
-    return filename, response._http_response.content     # TODO: May need to push support in python-redfish-library to have a proper method of getting raw content
+    filename = response.dict["AdditionalDataURI"].split("/")[-1]
+    response = context.get(response.dict["AdditionalDataURI"])
+    return (
+        filename,
+        response._http_response.content,
+    )  # TODO: May need to push support in python-redfish-library to have a proper method of getting raw content
+
 
-def get_log_service( context, container_type = log_container.MANAGER, container_id = None, log_service_id = None ):
+def get_log_service(context, container_type=log_container.MANAGER, container_id=None, log_service_id=None):
     """
     Finds a log service matching the given ID and returns its resource
 
     Args:
         context: The Redfish client object with an open session
         container_type: The type of resource containing the log service (manager, system, or chassis)
         container_id: The container instance to locate; if None, perform on the only container
         log_service_id: The log service to locate; if None, perform on the only log service
 
     Returns:
         The log service resource
     """
 
     # Get the Service Root to find the resource collection
-    service_root = context.get( "/redfish/v1/" )
+    service_root = context.get("/redfish/v1/")
     if container_type.value not in service_root.dict:
         # No resource collection
-        raise RedfishLogServiceNotFoundError( "Service does not contain a {} collection".format( container_type.value ) )
+        raise RedfishLogServiceNotFoundError("Service does not contain a {} collection".format(container_type.value))
 
     # Get the resource collection and iterate through its collection to find the matching container instance
     avail_resources = []
-    resource_col = context.get( service_root.dict[container_type.value]["@odata.id"] )
+    resource_col = context.get(service_root.dict[container_type.value]["@odata.id"])
     if container_id is None:
-        if len( resource_col.dict["Members"] ) == 1:
-            resource = context.get( resource_col.dict["Members"][0]["@odata.id"] )
+        if len(resource_col.dict["Members"]) == 1:
+            resource = context.get(resource_col.dict["Members"][0]["@odata.id"])
             container_id = resource.dict["Id"]
         else:
             for resource_member in resource_col.dict["Members"]:
-                resource = context.get( resource_member["@odata.id"] )
-                avail_resources.append( resource.dict["Id"] )
-            raise RedfishLogServiceNotFoundError( "Service does not contain exactly one resource in {}; a target container needs to be specified: {}".format( container_type.value, ", ".join( avail_resources ) ) )
+                resource = context.get(resource_member["@odata.id"])
+                avail_resources.append(resource.dict["Id"])
+            raise RedfishLogServiceNotFoundError(
+                "Service does not contain exactly one resource in {}; a target container needs to be specified: {}".format(
+                    container_type.value, ", ".join(avail_resources)
+                )
+            )
     else:
         container_found = False
         for resource_member in resource_col.dict["Members"]:
-            resource = context.get( resource_member["@odata.id"] )
-            avail_resources.append( resource.dict["Id"] )
+            resource = context.get(resource_member["@odata.id"])
+            avail_resources.append(resource.dict["Id"])
             if resource.dict["Id"] == container_id:
                 container_found = True
                 break
         if not container_found:
-            raise RedfishLogServiceNotFoundError( "Service does not contain a resource in {} called {}; valid resources: {}".format( container_type.value, container_id, ", ".join( avail_resources ) ) )
+            raise RedfishLogServiceNotFoundError(
+                "Service does not contain a resource in {} called {}; valid resources: {}".format(
+                    container_type.value, container_id, ", ".join(avail_resources)
+                )
+            )
 
     # Go through the container to find the log service collection
     if "LogServices" not in resource.dict:
         # No log services
-        raise RedfishLogServiceNotFoundError( "{} does not contain a log service collection".format( container_id ) )
+        raise RedfishLogServiceNotFoundError("{} does not contain a log service collection".format(container_id))
 
     # Get the log service collection and iterate through its collection
     avail_logs = []
-    log_serv_col = context.get( resource.dict["LogServices"]["@odata.id"] )
+    log_serv_col = context.get(resource.dict["LogServices"]["@odata.id"])
     if log_service_id is None:
-        if len( log_serv_col.dict["Members"] ) == 1:
-            return context.get( log_serv_col.dict["Members"][0]["@odata.id"] )
+        if len(log_serv_col.dict["Members"]) == 1:
+            return context.get(log_serv_col.dict["Members"][0]["@odata.id"])
         else:
             for log_serv_member in log_serv_col.dict["Members"]:
-                log_serv = context.get( log_serv_member["@odata.id"] )
-                avail_logs.append( log_serv.dict["Id"] )
-            raise RedfishLogServiceNotFoundError( "{} does not contain exactly one log service; a target log service needs to be specified: {}".format( container_id, ", ".join( avail_logs ) ) )
+                log_serv = context.get(log_serv_member["@odata.id"])
+                avail_logs.append(log_serv.dict["Id"])
+            raise RedfishLogServiceNotFoundError(
+                "{} does not contain exactly one log service; a target log service needs to be specified: {}".format(
+                    container_id, ", ".join(avail_logs)
+                )
+            )
     else:
         for log_serv_member in log_serv_col.dict["Members"]:
-            log_serv = context.get( log_serv_member["@odata.id"] )
-            avail_logs.append( log_serv.dict["Id"] )
+            log_serv = context.get(log_serv_member["@odata.id"])
+            avail_logs.append(log_serv.dict["Id"])
             if log_serv.dict["Id"] == log_service_id:
                 return log_serv
 
-    raise RedfishLogServiceNotFoundError( "{} does not contain a log service called {}; valid log services: {}".format( container_id, log_service_id, ", ".join( avail_logs ) ) )
+    raise RedfishLogServiceNotFoundError(
+        "{} does not contain a log service called {}; valid log services: {}".format(
+            container_id, log_service_id, ", ".join(avail_logs)
+        )
+    )
```

### Comparing `redfish_utilities-3.2.8/redfish_utilities/managers.py` & `redfish_utilities-3.2.9/redfish_utilities/managers.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,65 +14,77 @@
 
 import sys
 from .collections import get_collection_ids
 from .messages import verify_response
 from .resets import reset_types
 from .resets import reset_to_defaults_types
 
-class RedfishManagerNotFoundError( Exception ):
+
+class RedfishManagerNotFoundError(Exception):
     """
     Raised when a matching manager cannot be found
     """
+
     pass
 
-class RedfishManagerNetworkProtocolNotFoundError( Exception ):
+
+class RedfishManagerNetworkProtocolNotFoundError(Exception):
     """
     Raised when a matching manager does not contain network protocol information
     """
+
     pass
 
-class RedfishManagerEthIntNotFoundError( Exception ):
+
+class RedfishManagerEthIntNotFoundError(Exception):
     """
     Raised when a matching Ethernet interface cannot be found
     """
+
     pass
 
-class RedfishManagerResetNotFoundError( Exception ):
+
+class RedfishManagerResetNotFoundError(Exception):
     """
     Raised when the Reset action cannot be found
     """
+
     pass
 
-class RedfishManagerResetToDefaultsNotFoundError( Exception ):
+
+class RedfishManagerResetToDefaultsNotFoundError(Exception):
     """
     Raised when the ResetToDefaults action cannot be found
     """
+
     pass
 
-def get_manager_ids( context ):
+
+def get_manager_ids(context):
     """
     Finds the manager collection and returns all of the member's identifiers
 
     Args:
         context: The Redfish client object with an open session
 
     Returns:
         A list of identifiers of the members of the manager collection
     """
 
     # Get the service root to find the manager collection
-    service_root = context.get( "/redfish/v1/" )
+    service_root = context.get("/redfish/v1/")
     if "Managers" not in service_root.dict:
         # No manager collection
-        raise RedfishManagerNotFoundError( "The service does not contain a manager collection" )
+        raise RedfishManagerNotFoundError("The service does not contain a manager collection")
 
     # Get the manager collection and iterate through its collection
-    return get_collection_ids( context, service_root.dict["Managers"]["@odata.id"] )
+    return get_collection_ids(context, service_root.dict["Managers"]["@odata.id"])
+
 
-def get_manager( context, manager_id = None ):
+def get_manager(context, manager_id=None):
     """
     Finds a manager matching the given identifier and returns its resource
 
     Args:
         context: The Redfish client object with an open session
         manager_id: The manager to locate; if None, perform on the only manager
 
@@ -81,138 +93,163 @@
     """
 
     manager_uri_pattern = "/redfish/v1/Managers/{}"
     avail_managers = None
 
     # If given an identifier, get the manager directly
     if manager_id is not None:
-        manager = context.get( manager_uri_pattern.format( manager_id ) )
+        manager = context.get(manager_uri_pattern.format(manager_id))
     # No identifier given; see if there's exactly one member
     else:
-        avail_managers = get_manager_ids( context )
-        if len( avail_managers ) == 1:
-            manager = context.get( manager_uri_pattern.format( avail_managers[0] ) )
+        avail_managers = get_manager_ids(context)
+        if len(avail_managers) == 1:
+            manager = context.get(manager_uri_pattern.format(avail_managers[0]))
         else:
-            raise RedfishManagerNotFoundError( "The service does not contain exactly one manager; a target manager needs to be specified: {}".format( ", ".join( avail_managers ) ) )
+            raise RedfishManagerNotFoundError(
+                "The service does not contain exactly one manager; a target manager needs to be specified: {}".format(
+                    ", ".join(avail_managers)
+                )
+            )
 
     # Check the response and return the manager if the response is good
     if manager.status == 404:
         if avail_managers is None:
-            avail_managers = get_manager_ids( context )
-        raise RedfishManagerNotFoundError( "The service does not contain a manager called {}; valid managers: {}".format( manager_id, ", ".join( avail_managers ) ) )
-    verify_response( manager )
+            avail_managers = get_manager_ids(context)
+        raise RedfishManagerNotFoundError(
+            "The service does not contain a manager called {}; valid managers: {}".format(
+                manager_id, ", ".join(avail_managers)
+            )
+        )
+    verify_response(manager)
     return manager
 
-def set_manager( context, manager_id = None, date_time = None, date_time_offset = None ):
+
+def set_manager(context, manager_id=None, date_time=None, date_time_offset=None):
     """
     Finds a manager matching the given identifier and sets one or more properties
 
     Args:
         context: The Redfish client object with an open session
         manager_id: The manager to locate; if None, perform on the only manager
         date_time: The date-time value to set
         date_time_offset: The date-time offset value to set
 
     Returns:
         The response of the PATCH
     """
 
     # Locate the manager
-    manager = get_manager( context, manager_id )
+    manager = get_manager(context, manager_id)
 
     # Build the payload
     payload = {}
     if date_time is not None:
         payload["DateTime"] = date_time
     if date_time_offset is not None:
         payload["DateTimeOffset"] = date_time_offset
 
     # Update the manager
     headers = None
-    etag = manager.getheader( "ETag" )
+    etag = manager.getheader("ETag")
     if etag is not None:
-        headers = { "If-Match": etag }
-    response = context.patch( manager.dict["@odata.id"], body = payload, headers = headers )
-    verify_response( response )
+        headers = {"If-Match": etag}
+    response = context.patch(manager.dict["@odata.id"], body=payload, headers=headers)
+    verify_response(response)
     return response
 
-def print_manager( manager ):
+
+def print_manager(manager):
     """
     Prints the manager info
 
     Args:
         manager: The manager info to print
     """
 
     manager_line_format = "  {}: {}"
-    manager_properties = [ "Status", "ManagerType", "PowerState", "FirmwareVersion", "DateTime", "DateTimeLocalOffset", "LastResetTime",
-        "UUID", "ServiceEntryPointUUID", "Manufacturer", "Model", "PartNumber", "SparePartNumber", "SerialNumber" ]
-    print( "Manager {} Info".format( manager.dict["Id"] ) )
+    manager_properties = [
+        "Status",
+        "ManagerType",
+        "PowerState",
+        "FirmwareVersion",
+        "DateTime",
+        "DateTimeLocalOffset",
+        "LastResetTime",
+        "UUID",
+        "ServiceEntryPointUUID",
+        "Manufacturer",
+        "Model",
+        "PartNumber",
+        "SparePartNumber",
+        "SerialNumber",
+    ]
+    print("Manager {} Info".format(manager.dict["Id"]))
     for property in manager_properties:
         if property in manager.dict:
             prop_val = manager.dict[property]
-            if isinstance( prop_val, list ):
-                prop_val = ", ".join( prop_val )
+            if isinstance(prop_val, list):
+                prop_val = ", ".join(prop_val)
             elif property == "Status":
-                prop_val = "State: {}, Health: {}".format( prop_val.get( "State", "N/A" ), prop_val.get( "Health", "N/A" ) )
-            print( manager_line_format.format( property, prop_val ) )
-    print( "" )
+                prop_val = "State: {}, Health: {}".format(prop_val.get("State", "N/A"), prop_val.get("Health", "N/A"))
+            print(manager_line_format.format(property, prop_val))
+    print("")
+
 
-def get_manager_reset_info( context, manager_id = None, manager = None ):
+def get_manager_reset_info(context, manager_id=None, manager=None):
     """
     Finds a manager matching the given ID and returns its reset info
 
     Args:
         context: The Redfish client object with an open session
         manager_id: The manager to locate; if None, perform on the only manager
         manager: Existing manager resource to inspect for reset info
 
     Returns:
         The URI of the Reset action
         A list of parameter requirements from the action info
     """
 
     if manager is None:
-        manager = get_manager( context, manager_id )
+        manager = get_manager(context, manager_id)
 
     # Check that there is a Reset action
     if "Actions" not in manager.dict:
-        raise RedfishManagerResetNotFoundError( "Manager {} does not support the Reset action".format( manager.dict["Id"] ) )
+        raise RedfishManagerResetNotFoundError(
+            "Manager {} does not support the Reset action".format(manager.dict["Id"])
+        )
     if "#Manager.Reset" not in manager.dict["Actions"]:
-        raise RedfishManagerResetNotFoundError( "Manager {} does not support the Reset action".format( manager.dict["Id"] ) )
+        raise RedfishManagerResetNotFoundError(
+            "Manager {} does not support the Reset action".format(manager.dict["Id"])
+        )
 
     # Extract the info about the Reset action
     reset_action = manager.dict["Actions"]["#Manager.Reset"]
     reset_uri = reset_action["target"]
 
     if "@Redfish.ActionInfo" not in reset_action:
         # No action info; need to build this manually based on other annotations
 
         # Default parameter requirements
         reset_parameters = [
-            {
-                "Name": "ResetType",
-                "Required": False,
-                "DataType": "String",
-                "AllowableValues": reset_types
-            }
+            {"Name": "ResetType", "Required": False, "DataType": "String", "AllowableValues": reset_types}
         ]
 
         # Get the AllowableValues from annotations
         for param in reset_parameters:
             if param["Name"] + "@Redfish.AllowableValues" in reset_action:
                 param["AllowableValues"] = reset_action[param["Name"] + "@Redfish.AllowableValues"]
     else:
         # Get the action info and its parameter listing
-        action_info = context.get( reset_action["@Redfish.ActionInfo"] )
+        action_info = context.get(reset_action["@Redfish.ActionInfo"])
         reset_parameters = action_info.dict["Parameters"]
 
     return reset_uri, reset_parameters
 
-def manager_reset( context, manager_id = None, reset_type = None ):
+
+def manager_reset(context, manager_id=None, reset_type=None):
     """
     Finds a manager matching the given ID and performs a reset
 
     Args:
         context: The Redfish client object with an open session
         manager_id: The manager to locate; if None, perform on the only manager
         reset_type: The type of reset to perform; if None, perform one of the common resets
@@ -221,18 +258,18 @@
         The response of the action
     """
 
     # Check that the values themselves are supported by the schema
     reset_type_values = reset_types
     if reset_type is not None:
         if reset_type not in reset_type_values:
-            raise ValueError( "{} is not an allowable reset type ({})".format( reset_type, ", ".join( reset_type_values ) ) )
+            raise ValueError("{} is not an allowable reset type ({})".format(reset_type, ", ".join(reset_type_values)))
 
     # Locate the reset action
-    reset_uri, reset_parameters = get_manager_reset_info( context, manager_id )
+    reset_uri, reset_parameters = get_manager_reset_info(context, manager_id)
 
     # Build the payload
     if reset_type is None:
         for param in reset_parameters:
             if param["Name"] == "ResetType":
                 if "GracefulRestart" in param["AllowableValues"]:
                     reset_type = "GracefulRestart"
@@ -242,80 +279,81 @@
                     reset_type = "PowerCycle"
 
     payload = {}
     if reset_type is not None:
         payload["ResetType"] = reset_type
 
     # Reset the manager
-    response = context.post( reset_uri, body = payload )
+    response = context.post(reset_uri, body=payload)
     try:
-        verify_response( response )
+        verify_response(response)
     except Exception as e:
         additional_message = ""
         if response.status == 400:
             # Append the list of valid reset types to 400 Bad Request responses
             additional_message = "\nNo supported reset types listed"
             for param in reset_parameters:
                 if param["Name"] == "ResetType" and "AllowableValues" in param:
-                    additional_message = "\nSupported reset types: {}".format( ", ".join( param["AllowableValues"] ) )
-        raise type( e )( str( e ) + additional_message ).with_traceback( sys.exc_info()[2] )
+                    additional_message = "\nSupported reset types: {}".format(", ".join(param["AllowableValues"]))
+        raise type(e)(str(e) + additional_message).with_traceback(sys.exc_info()[2])
     return response
 
-def get_manager_reset_to_defaults_info( context, manager_id = None, manager = None ):
+
+def get_manager_reset_to_defaults_info(context, manager_id=None, manager=None):
     """
     Finds a manager matching the given ID and returns its reset-to-defaults info
 
     Args:
         context: The Redfish client object with an open session
         manager_id: The manager to locate; if None, perform on the only manager
         manager: Existing manager resource to inspect for reset info
 
     Returns:
         The URI of the Reset action
         A list of parameter requirements from the action info
     """
 
     if manager is None:
-        manager = get_manager( context, manager_id )
+        manager = get_manager(context, manager_id)
 
     # Check that there is a Reset action
     if "Actions" not in manager.dict:
-        raise RedfishManagerResetToDefaultsNotFoundError( "Manager {} does not support the ResetToDefaults action".format( manager.dict["Id"] ) )
+        raise RedfishManagerResetToDefaultsNotFoundError(
+            "Manager {} does not support the ResetToDefaults action".format(manager.dict["Id"])
+        )
     if "#Manager.ResetToDefaults" not in manager.dict["Actions"]:
-        raise RedfishManagerResetToDefaultsNotFoundError( "Manager {} does not support the ResetToDefaults action".format( manager.dict["Id"] ) )
+        raise RedfishManagerResetToDefaultsNotFoundError(
+            "Manager {} does not support the ResetToDefaults action".format(manager.dict["Id"])
+        )
 
     # Extract the info about the ResetToDefaults action
     reset_action = manager.dict["Actions"]["#Manager.ResetToDefaults"]
     reset_uri = reset_action["target"]
 
     if "@Redfish.ActionInfo" not in reset_action:
         # No action info; need to build this manually based on other annotations
 
         # Default parameter requirements
         reset_parameters = [
-            {
-                "Name": "ResetType",
-                "Required": True,
-                "DataType": "String",
-                "AllowableValues": reset_to_defaults_types
-            }
+            {"Name": "ResetType", "Required": True, "DataType": "String", "AllowableValues": reset_to_defaults_types}
         ]
 
         # Get the AllowableValues from annotations
         for param in reset_parameters:
             if param["Name"] + "@Redfish.AllowableValues" in reset_action:
                 param["AllowableValues"] = reset_action[param["Name"] + "@Redfish.AllowableValues"]
     else:
         # Get the action info and its parameter listing
-        action_info = context.get( reset_action["@Redfish.ActionInfo"] )
+        action_info = context.get(reset_action["@Redfish.ActionInfo"])
         reset_parameters = action_info.dict["Parameters"]
 
     return reset_uri, reset_parameters
 
-def manager_reset_to_defaults( context, manager_id = None, reset_type = None ):
+
+def manager_reset_to_defaults(context, manager_id=None, reset_type=None):
     """
     Finds a manager matching the given ID and performs a reset-to-defaults
 
     Args:
         context: The Redfish client object with an open session
         manager_id: The manager to locate; if None, perform on the only manager
         reset_type: The type of reset to perform; if None, perform one of the common resets
@@ -324,18 +362,20 @@
         The response of the action
     """
 
     # Check that the values themselves are supported by the schema
     reset_to_default_type_values = reset_to_defaults_types
     if reset_type is not None:
         if reset_type not in reset_to_default_type_values:
-            raise ValueError( "{} is not an allowable reset type ({})".format( reset_type, ", ".join( reset_to_default_type_values ) ) )
+            raise ValueError(
+                "{} is not an allowable reset type ({})".format(reset_type, ", ".join(reset_to_default_type_values))
+            )
 
     # Locate the reset action
-    reset_uri, reset_parameters = get_manager_reset_to_defaults_info( context, manager_id )
+    reset_uri, reset_parameters = get_manager_reset_to_defaults_info(context, manager_id)
 
     # Build the payload
     if reset_type is None:
         for param in reset_parameters:
             if param["Name"] == "ResetType":
                 if "PreserveNetworkAndUsers" in param["AllowableValues"]:
                     reset_type = "PreserveNetworkAndUsers"
@@ -345,143 +385,179 @@
                     reset_type = "ResetAll"
 
     payload = {}
     if reset_type is not None:
         payload["ResetType"] = reset_type
 
     # Reset the manager to defaults
-    response = context.post( reset_uri, body = payload )
+    response = context.post(reset_uri, body=payload)
     try:
-        verify_response( response )
+        verify_response(response)
     except Exception as e:
         additional_message = ""
         if response.status == 400:
             # Append the list of valid reset types to 400 Bad Request responses
             additional_message = "\nNo supported reset types listed"
             for param in reset_parameters:
                 if param["Name"] == "ResetType" and "AllowableValues" in param:
-                    additional_message = "\nSupported reset types: {}".format( ", ".join( param["AllowableValues"] ) )
-        raise type( e )( str( e ) + additional_message ).with_traceback( sys.exc_info()[2] )
+                    additional_message = "\nSupported reset types: {}".format(", ".join(param["AllowableValues"]))
+        raise type(e)(str(e) + additional_message).with_traceback(sys.exc_info()[2])
     return response
 
-def get_manager_network_protocol( context, manager_id = None ):
+
+def get_manager_network_protocol(context, manager_id=None):
     """
     Finds the network protocol information for a manager and returns its resource
 
     Args:
         context: The Redfish client object with an open session
         manager_id: The manager to locate; if None, perform on the only manager
 
     Returns:
         The ManagerNetworkProtocol resource
     """
     # Get the manager to find its network protocol information
-    manager = get_manager( context, manager_id )
+    manager = get_manager(context, manager_id)
     if "NetworkProtocol" not in manager.dict:
         # No network protocol information
-        raise RedfishManagerNetworkProtocolNotFoundError( "Manager {} does not contain network protocol information".format( manager.dict["Id"] ) )
+        raise RedfishManagerNetworkProtocolNotFoundError(
+            "Manager {} does not contain network protocol information".format(manager.dict["Id"])
+        )
 
     # Get the network protocol information
-    response = context.get( manager.dict["NetworkProtocol"]["@odata.id"] )
-    verify_response( response )
+    response = context.get(manager.dict["NetworkProtocol"]["@odata.id"])
+    verify_response(response)
     return response
 
-def set_manager_network_protocol( context, manager_id = None, network_protocol = None ):
+
+def set_manager_network_protocol(context, manager_id=None, network_protocol=None):
     """
     Sets network protocol settings for a manager
 
     Args:
         context: The Redfish client object with an open session
         manager_id: The manager to locate; if None, perform on the only manager
         network_protocol: The network protocol settings to apply
 
     Returns:
         The response of the PATCH
     """
     # Get the manager to find its network protocol information
-    manager = get_manager( context, manager_id )
+    manager = get_manager(context, manager_id)
     if "NetworkProtocol" not in manager.dict:
         # No network protocol information
-        raise RedfishManagerNetworkProtocolNotFoundError( "Manager {} does not contain network protocol information".format( manager.dict["Id"] ) )
+        raise RedfishManagerNetworkProtocolNotFoundError(
+            "Manager {} does not contain network protocol information".format(manager.dict["Id"])
+        )
 
     # Get the current network protocol information
-    response = context.get( manager.dict["NetworkProtocol"]["@odata.id"] )
-    verify_response( response )
+    response = context.get(manager.dict["NetworkProtocol"]["@odata.id"])
+    verify_response(response)
     headers = None
-    etag = response.getheader( "ETag" )
+    etag = response.getheader("ETag")
     if etag is not None:
-        headers = { "If-Match": etag }
+        headers = {"If-Match": etag}
 
     # Set the network protocol information
     if network_protocol is None:
         network_protocol = {}
-    response = context.patch( manager.dict["NetworkProtocol"]["@odata.id"], body = network_protocol, headers = headers )
-    verify_response( response )
+    response = context.patch(manager.dict["NetworkProtocol"]["@odata.id"], body=network_protocol, headers=headers)
+    verify_response(response)
     return response
 
-def print_manager_network_protocol( network_protocol ):
+
+def print_manager_network_protocol(network_protocol):
     """
     Prints the manager network protocol information
 
     Args:
         network_protocol: The manager network protocol information to print
     """
 
-    network_protocol_properties = [ "HTTP", "HTTPS", "SSDP", "SSH", "Telnet", "KVMIP", "NTP", "RDP", "RFB",
-                                    "VirtualMedia", "IPMI", "SNMP", "DHCP", "DHCPv6" ]
+    network_protocol_properties = [
+        "HTTP",
+        "HTTPS",
+        "SSDP",
+        "SSH",
+        "Telnet",
+        "KVMIP",
+        "NTP",
+        "RDP",
+        "RFB",
+        "VirtualMedia",
+        "IPMI",
+        "SNMP",
+        "DHCP",
+        "DHCPv6",
+    ]
     network_protocol_line_format = "  {:16s} | {:8s} | {:6s} | {}"
-    print( "Manager Network Protocol Info" )
-    print( "" )
-    print( network_protocol_line_format.format( "Protocol", "Enabled", "Port", "Other Settings" ) )
+    print("Manager Network Protocol Info")
+    print("")
+    print(network_protocol_line_format.format("Protocol", "Enabled", "Port", "Other Settings"))
 
     for property in network_protocol_properties:
         if property in network_protocol.dict:
             other_str = ""
             if property == "SSDP":
                 # For SSDP, extract the NOTIFY settings
                 other_str = []
                 if "NotifyIPv6Scope" in network_protocol.dict[property]:
-                    other_str.append( "NOTIFY IPv6 Scope: {}".format( network_protocol.dict[property]["NotifyIPv6Scope"] ) )
+                    other_str.append("NOTIFY IPv6 Scope: {}".format(network_protocol.dict[property]["NotifyIPv6Scope"]))
                 if "NotifyTTL" in network_protocol.dict[property]:
-                    other_str.append( "NOTIFY TTL: {}".format( network_protocol.dict[property]["NotifyTTL"] ) )
+                    other_str.append("NOTIFY TTL: {}".format(network_protocol.dict[property]["NotifyTTL"]))
                 if "NotifyMulticastIntervalSeconds" in network_protocol.dict[property]:
-                    other_str.append( "NOTIFY ALIVE Interval: {}".format( network_protocol.dict[property]["NotifyMulticastIntervalSeconds"] ) )
-                other_str = ", ".join( other_str )
+                    other_str.append(
+                        "NOTIFY ALIVE Interval: {}".format(
+                            network_protocol.dict[property]["NotifyMulticastIntervalSeconds"]
+                        )
+                    )
+                other_str = ", ".join(other_str)
             if property == "NTP":
                 # For NTP, extract the servers; need to skip "empty" slots potentially
                 if "NTPServers" in network_protocol.dict[property]:
                     other_str = []
                     for server in network_protocol.dict[property]["NTPServers"]:
-                        if isinstance( server, str ):
-                            other_str.append( server )
-                    other_str = "NTP Servers: " + ", ".join( other_str )
-            print( network_protocol_line_format.format( property, str( network_protocol.dict[property].get( "ProtocolEnabled", "" ) ), str( network_protocol.dict[property].get( "Port", "" ) ), other_str ) )
+                        if isinstance(server, str):
+                            other_str.append(server)
+                    other_str = "NTP Servers: " + ", ".join(other_str)
+            print(
+                network_protocol_line_format.format(
+                    property,
+                    str(network_protocol.dict[property].get("ProtocolEnabled", "")),
+                    str(network_protocol.dict[property].get("Port", "")),
+                    other_str,
+                )
+            )
+
 
-def get_manager_ethernet_interface_ids( context, manager_id = None ):
+def get_manager_ethernet_interface_ids(context, manager_id=None):
     """
     Finds the Ethernet interface collection for a manager and returns all of the member's identifiers
 
     Args:
         context: The Redfish client object with an open session
         manager_id: The manager to locate; if None, perform on the only manager
 
     Returns:
         A list of identifiers of the members of the Ethernet interface collection
     """
 
     # Get the manager to find its Ethernet interface collection
-    manager = get_manager( context, manager_id )
+    manager = get_manager(context, manager_id)
     if "EthernetInterfaces" not in manager.dict:
         # No Ethernet interface collection
-        raise RedfishManagerEthIntNotFoundError( "Manager {} does not contain an Ethernet interface collection".format( manager.dict["Id"] ) )
+        raise RedfishManagerEthIntNotFoundError(
+            "Manager {} does not contain an Ethernet interface collection".format(manager.dict["Id"])
+        )
 
     # Get the Ethernet interface collection and iterate through its collection
-    return get_collection_ids( context, manager.dict["EthernetInterfaces"]["@odata.id"] )
+    return get_collection_ids(context, manager.dict["EthernetInterfaces"]["@odata.id"])
 
-def get_manager_ethernet_interface( context, manager_id = None, interface_id = None ):
+
+def get_manager_ethernet_interface(context, manager_id=None, interface_id=None):
     """
     Finds an Ethernet interface for a manager matching the given identifiers and returns its resource
 
     Args:
         context: The Redfish client object with an open session
         manager_id: The manager to locate; if None, perform on the only manager
         interface_id: The Ethernet interface to locate; if None, perform on the only Ethernet interface
@@ -491,37 +567,56 @@
     """
 
     interface_uri_pattern = "/redfish/v1/Managers/{}/EthernetInterfaces/{}"
     avail_interfaces = None
 
     # Get the manager identifier in order to build the full URI later
     if manager_id is None:
-        manager = get_manager( context, None )
+        manager = get_manager(context, None)
         manager_id = manager.dict["Id"]
 
     # If given an identifier, get the Ethernet interface directly
     if interface_id is not None:
-        interface = context.get( interface_uri_pattern.format( manager_id, interface_id ) )
+        interface = context.get(interface_uri_pattern.format(manager_id, interface_id))
     # No identifier given; see if there's exactly one member
     else:
-        avail_interfaces = get_manager_ethernet_interface_ids( context, manager_id )
-        if len( avail_interfaces ) == 1:
-            interface = context.get( interface_uri_pattern.format( manager_id, avail_interfaces[0] ) )
+        avail_interfaces = get_manager_ethernet_interface_ids(context, manager_id)
+        if len(avail_interfaces) == 1:
+            interface = context.get(interface_uri_pattern.format(manager_id, avail_interfaces[0]))
         else:
-            raise RedfishManagerEthIntNotFoundError( "Manager {} does not contain exactly one Ethernet interface; a target Ethernet interface needs to be specified: {}".format( manager_id, ", ".join( avail_interfaces ) ) )
+            raise RedfishManagerEthIntNotFoundError(
+                "Manager {} does not contain exactly one Ethernet interface; a target Ethernet interface needs to be specified: {}".format(
+                    manager_id, ", ".join(avail_interfaces)
+                )
+            )
 
     # Check the response and return the Ethernet interface if the response is good
     if interface.status == 404:
         if avail_interfaces is None:
-            avail_interfaces = get_manager_ethernet_interface_ids( context, manager_id )
-        raise RedfishManagerEthIntNotFoundError( "Manager {} does not contain an Ethernet interface called {}; valid Ethernet interfaces: {}".format( manager_id, interface_id, ", ".join( avail_interfaces ) ) )
-    verify_response( interface )
+            avail_interfaces = get_manager_ethernet_interface_ids(context, manager_id)
+        raise RedfishManagerEthIntNotFoundError(
+            "Manager {} does not contain an Ethernet interface called {}; valid Ethernet interfaces: {}".format(
+                manager_id, interface_id, ", ".join(avail_interfaces)
+            )
+        )
+    verify_response(interface)
     return interface
 
-def set_manager_ethernet_interface( context, manager_id = None, interface_id = None, vlan = None, ipv4_addresses = None, dhcpv4 = None, ipv6_addresses = None, ipv6_gateways = None, dhcpv6 = None ):
+
+def set_manager_ethernet_interface(
+    context,
+    manager_id=None,
+    interface_id=None,
+    vlan=None,
+    ipv4_addresses=None,
+    dhcpv4=None,
+    ipv6_addresses=None,
+    ipv6_gateways=None,
+    dhcpv6=None,
+):
     """
     Finds an Ethernet interface matching the given ID and updates specified properties
 
     Args:
         context: The Redfish client object with an open session
         manager_id: The manager to locate; if None, perform on the only manager
         interface_id: The Ethernet interface to locate; if None, perform on the only interface
@@ -533,15 +628,15 @@
         dhcpv6: An object containing new DHCPv6 settings for the interface
 
     Returns:
         The response of the PATCH
     """
 
     # Locate the interface
-    interface = get_manager_ethernet_interface( context, manager_id, interface_id )
+    interface = get_manager_ethernet_interface(context, manager_id, interface_id)
 
     # Update the interface based on the request parameters
     payload = {}
     if vlan is not None:
         payload["VLAN"] = vlan
     if ipv4_addresses is not None:
         if "IPv4StaticAddresses" in interface.dict:
@@ -554,97 +649,139 @@
     if ipv6_addresses is not None:
         payload["IPv6StaticAddresses"] = ipv6_addresses
     if ipv6_gateways is not None:
         payload["IPv6StaticDefaultGateways"] = ipv6_gateways
     if dhcpv6 is not None:
         payload["DHCPv6"] = dhcpv6
     headers = None
-    etag = interface.getheader( "ETag" )
+    etag = interface.getheader("ETag")
     if etag is not None:
-        headers = { "If-Match": etag }
-    response = context.patch( interface.dict["@odata.id"], body = payload, headers = headers )
-    verify_response( response )
+        headers = {"If-Match": etag}
+    response = context.patch(interface.dict["@odata.id"], body=payload, headers=headers)
+    verify_response(response)
     return response
 
-def print_manager_ethernet_interface( interface ):
+
+def print_manager_ethernet_interface(interface):
     """
     Prints the Ethernet interface info
 
     Args:
         interface: The Ethernet interface info to print
     """
 
     interface_line_format = "  {}: {}"
-    interface_properties = [ "Status", "InterfaceEnabled", "LinkStatus", "MACAddress", "PermanentMACAddress", "SpeedMbps", "AutoNeg", "FullDuplex",
-        "MTUSize", "HostName", "FQDN", "NameServers", "StaticNameServers" ]
-    print( "Ethernet Interface {} Info".format( interface.dict["Id"] ) )
+    interface_properties = [
+        "Status",
+        "InterfaceEnabled",
+        "LinkStatus",
+        "MACAddress",
+        "PermanentMACAddress",
+        "SpeedMbps",
+        "AutoNeg",
+        "FullDuplex",
+        "MTUSize",
+        "HostName",
+        "FQDN",
+        "NameServers",
+        "StaticNameServers",
+    ]
+    print("Ethernet Interface {} Info".format(interface.dict["Id"]))
     for property in interface_properties:
         if property in interface.dict:
             prop_val = interface.dict[property]
-            if isinstance( prop_val, list ):
-                prop_val = ", ".join( prop_val )
+            if isinstance(prop_val, list):
+                prop_val = ", ".join(prop_val)
             elif property == "Status":
-                prop_val = "State: {}, Health: {}".format( prop_val.get( "State", "N/A" ), prop_val.get( "Health", "N/A" ) )
-            print( interface_line_format.format( property, prop_val ) )
-    print( "" )
+                prop_val = "State: {}, Health: {}".format(prop_val.get("State", "N/A"), prop_val.get("Health", "N/A"))
+            print(interface_line_format.format(property, prop_val))
+    print("")
 
     if "VLAN" in interface.dict:
-        print( "  VLAN Info" )
-        print( "    Enabled: {}".format( interface.dict["VLAN"].get( "VLANEnable", False ) ) )
-        print( "    ID: {}".format( interface.dict["VLAN"].get( "VLANId", "N/A" ) ) )
-        print( "    Priority: {}".format( interface.dict["VLAN"].get( "VLANPriority", "N/A" ) ) )
-        print( "" )
+        print("  VLAN Info")
+        print("    Enabled: {}".format(interface.dict["VLAN"].get("VLANEnable", False)))
+        print("    ID: {}".format(interface.dict["VLAN"].get("VLANId", "N/A")))
+        print("    Priority: {}".format(interface.dict["VLAN"].get("VLANPriority", "N/A")))
+        print("")
 
-    print( "  IPv4 Info" )
+    print("  IPv4 Info")
     if "DHCPv4" in interface.dict:
-        print( "    DHCP Enabled: {}".format( interface.dict["DHCPv4"]["DHCPEnabled"] ) )
+        print("    DHCP Enabled: {}".format(interface.dict["DHCPv4"]["DHCPEnabled"]))
     if "IPv4Addresses" in interface.dict:
-        print( "    Assigned Addresses" )
-        for i, address in enumerate( interface.dict["IPv4Addresses"] ):
+        print("    Assigned Addresses")
+        for i, address in enumerate(interface.dict["IPv4Addresses"]):
             if address is None:
-                print( "      Empty" )
+                print("      Empty")
             elif i == 0:
-                print( "      {}: {}, {}, {}".format( address.get( "Address", "N/A" ), address.get( "SubnetMask", "N/A" ), address.get( "Gateway", "N/A" ), address.get( "AddressOrigin", "N/A" ) ) )
+                print(
+                    "      {}: {}, {}, {}".format(
+                        address.get("Address", "N/A"),
+                        address.get("SubnetMask", "N/A"),
+                        address.get("Gateway", "N/A"),
+                        address.get("AddressOrigin", "N/A"),
+                    )
+                )
             else:
-                print( "      {}: {}, {}".format( address.get( "Address", "N/A" ), address.get( "SubnetMask", "N/A" ), address.get( "AddressOrigin", "N/A" ) ) )
+                print(
+                    "      {}: {}, {}".format(
+                        address.get("Address", "N/A"),
+                        address.get("SubnetMask", "N/A"),
+                        address.get("AddressOrigin", "N/A"),
+                    )
+                )
     if "IPv4StaticAddresses" in interface.dict:
-        print( "    Static Addresses" )
-        for i, address in enumerate( interface.dict["IPv4StaticAddresses"] ):
+        print("    Static Addresses")
+        for i, address in enumerate(interface.dict["IPv4StaticAddresses"]):
             if address is None:
-                print( "       Empty" )
+                print("       Empty")
             elif i == 0:
-                print( "      {}: {}, {}".format( address.get( "Address", "N/A" ), address.get( "SubnetMask", "N/A" ), address.get( "Gateway", "N/A" ) ) )
+                print(
+                    "      {}: {}, {}".format(
+                        address.get("Address", "N/A"), address.get("SubnetMask", "N/A"), address.get("Gateway", "N/A")
+                    )
+                )
             else:
-                print( "      {}: {}".format( address["Address"], address["SubnetMask"] ) )
-    print( "" )
+                print("      {}: {}".format(address["Address"], address["SubnetMask"]))
+    print("")
 
-    print( "  IPv6 Info" )
+    print("  IPv6 Info")
     if "DHCPv6" in interface.dict:
-        print( "    DHCP Mode: {}".format( interface.dict["DHCPv6"]["OperatingMode"] ) )
+        print("    DHCP Mode: {}".format(interface.dict["DHCPv6"]["OperatingMode"]))
     if "IPv6Addresses" in interface.dict:
-        print( "    Assigned Addresses" )
+        print("    Assigned Addresses")
         for address in interface.dict["IPv6Addresses"]:
-            print( "      {}/{}: {}, {}".format( address.get( "Address", "N/A" ), address.get( "PrefixLength", "N/A" ), address.get( "AddressOrigin", "N/A" ), address.get( "AddressState", "N/A" ) ) )
+            print(
+                "      {}/{}: {}, {}".format(
+                    address.get("Address", "N/A"),
+                    address.get("PrefixLength", "N/A"),
+                    address.get("AddressOrigin", "N/A"),
+                    address.get("AddressState", "N/A"),
+                )
+            )
     if "IPv6StaticAddresses" in interface.dict:
-        print( "    Static Addresses" )
+        print("    Static Addresses")
         for address in interface.dict["IPv6StaticAddresses"]:
             if address is None:
-                print( "      Empty" )
+                print("      Empty")
             else:
-                print( "      {}/{}".format( address.get( "Address", "N/A" ), address.get( "PrefixLength", "N/A" ) ) )
+                print("      {}/{}".format(address.get("Address", "N/A"), address.get("PrefixLength", "N/A")))
     if "IPv6StaticDefaultGateways" in interface.dict:
-        print( "    Static Default Gateways" )
+        print("    Static Default Gateways")
         for address in interface.dict["IPv6StaticDefaultGateways"]:
             if address is None:
-                print( "      Empty" )
+                print("      Empty")
             else:
-                print( "      {}/{}".format( address.get( "Address", "N/A" ), address.get( "PrefixLength", "N/A" ) ) )
+                print("      {}/{}".format(address.get("Address", "N/A"), address.get("PrefixLength", "N/A")))
     if "IPv6DefaultGateway" in interface.dict:
-        print( "    Default Gateway: {}".format( interface.dict["IPv6DefaultGateway"] ) )
+        print("    Default Gateway: {}".format(interface.dict["IPv6DefaultGateway"]))
     if "IPv6AddressPolicyTable" in interface.dict:
-        print( "    Address Policy Table" )
+        print("    Address Policy Table")
         for policy in interface.dict["IPv6AddressPolicyTable"]:
             if policy is None:
-                print( "      Empty" )
+                print("      Empty")
             else:
-                print( "      Prefix: {}, Prec: {}, Label: {}".format( policy.get( "Prefix", "N/A" ), policy.get( "Precedence", "N/A" ), policy.get( "Label", "N/A" ) ) )
-    print( "" )
+                print(
+                    "      Prefix: {}, Prec: {}, Label: {}".format(
+                        policy.get("Prefix", "N/A"), policy.get("Precedence", "N/A"), policy.get("Label", "N/A")
+                    )
+                )
+    print("")
```

### Comparing `redfish_utilities-3.2.8/redfish_utilities/messages.py` & `redfish_utilities-3.2.9/redfish_utilities/messages.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,44 +8,55 @@
 
 File : messages.py
 
 Brief : This file contains the definitions and functionalities for interacting
         with Messages for a given Redfish service
 """
 
-from redfish.messages import *
+from redfish.messages import (
+    get_messages_detail,
+    get_error_messages,
+    search_message,
+    RedfishPasswordChangeRequiredError,
+    RedfishOperationFailedError,
+)
 
-def verify_response( response ):
+
+def verify_response(response):
     """
     Verifies a response and raises an exception if there was a failure
 
     Args:
         response: The response to verify
     """
 
     if response.status >= 400:
-        messages_detail = get_messages_detail( response )
-        exception_string = get_error_messages( messages_detail )
-        message_item = search_message( messages_detail, "Base", "PasswordChangeRequired" )
-        if not message_item is None:
-            raise RedfishPasswordChangeRequiredError( "Operation failed: HTTP {}\n{}".format( response.status, exception_string ), message_item["MessageArgs"][0] )
+        messages_detail = get_messages_detail(response)
+        exception_string = get_error_messages(messages_detail)
+        message_item = search_message(messages_detail, "Base", "PasswordChangeRequired")
+        if message_item is not None:
+            raise RedfishPasswordChangeRequiredError(
+                "Operation failed: HTTP {}\n{}".format(response.status, exception_string),
+                message_item["MessageArgs"][0],
+            )
         else:
-            raise RedfishOperationFailedError( "Operation failed: HTTP {}\n{}".format( response.status, exception_string ) )
+            raise RedfishOperationFailedError("Operation failed: HTTP {}\n{}".format(response.status, exception_string))
 
     return
 
-def print_error_payload( response ):
+
+def print_error_payload(response):
     """
     Prints an error payload, which can also be used for action responses
 
     Args:
         response: The response to print
     """
 
     try:
-        print( get_error_messages( response ) )
-    except:
+        print(get_error_messages(response))
+    except Exception:
         # No response body
         if response.status >= 400:
-            print( "Failed" )
+            print("Failed")
         else:
-            print( "Success" )
+            print("Success")
```

### Comparing `redfish_utilities-3.2.8/redfish_utilities/misc.py` & `redfish_utilities-3.2.9/redfish_utilities/misc.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,41 +7,45 @@
 Miscellaneous
 
 File : misc.py
 
 Brief : Miscellaneous functions with common script logic
 """
 
-import sys
 
-def logout( context, ignore_error = False ):
+def logout(context, ignore_error=False):
     """
     Performs a logout of the service and allows for exceptions to be ignored
 
     Args:
         context: The Redfish client object with an open session
         ignore_error: Indicates if exceptions during logout are ignored
     """
 
     if context is not None:
         try:
             context.logout()
-        except Exception as e:
+        except Exception:
             if ignore_error:
                 pass
             else:
                 raise
     return
 
-def print_password_change_required_and_logout( context, args ):
+
+def print_password_change_required_and_logout(context, args):
     """
     Common help text when handling password change required conditions
 
     Args:
         context: The Redfish client object with an open session
         args: The argparse object from the calling script
     """
 
-    print( "Password change required.  To set a new password, run the following:" )
-    print( "rf_accounts.py -r {} -u {} -p <old password> --setpassword {} <new password>".format( args.rhost, args.user, args.user ) )
-    logout( context, ignore_error = True )  # Some services do not allow session logout in this condition
+    print("Password change required.  To set a new password, run the following:")
+    print(
+        "rf_accounts.py -r {} -u {} -p <old password> --setpassword {} <new password>".format(
+            args.rhost, args.user, args.user
+        )
+    )
+    logout(context, ignore_error=True)  # Some services do not allow session logout in this condition
     return
```

### Comparing `redfish_utilities-3.2.8/redfish_utilities/power_equipment.py` & `redfish_utilities-3.2.9/redfish_utilities/power_equipment.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,71 +12,80 @@
         with the power equipment for a given Redfish service
 """
 
 from .collections import get_collection_ids
 from .messages import verify_response
 from enum import Enum
 
-class RedfishPowerEquipmentNotFoundError( Exception ):
+
+class RedfishPowerEquipmentNotFoundError(Exception):
     """
     Raised when the requested power equipment is not represented in the service
     """
+
     pass
 
-class RedfishPowerEquipmentElectricalNotFoundError( Exception ):
+
+class RedfishPowerEquipmentElectricalNotFoundError(Exception):
     """
     Raised when the requested power equipment does not contain the desired electrical component
     """
+
     pass
 
-class power_equipment_types( Enum ):
+
+class power_equipment_types(Enum):
     """
     Types of power equipment that can be managed
     """
+
     FLOOR_PDU = "FloorPDU"
     RACK_PDU = "RackPDU"
     SWITCHGEAR = "Switchgear"
     TRANSFER_SWITCH = "TransferSwitch"
     POWER_SHELF = "PowerShelf"
     ELECTRICAL_BUS = "ElectricalBus"
 
-    def __str__( self ):
+    def __str__(self):
         return self.value
 
     @property
-    def plural( self ):
+    def plural(self):
         if self.value == "FloorPDU" or self.value == "RackPDU":
             return self.value + "s"
         if self.value == "TransferSwitch" or self.value == "ElectricalBus":
             return self.value + "es"
         if self.value == "PowerShelf":
             return "PowerShelves"
         return self.value
 
-class power_equipment_electrical_types( Enum ):
+
+class power_equipment_electrical_types(Enum):
     """
     Types of electrical components found on power equipment
     """
+
     OUTLET = "Outlet"
     MAINS = "Mains"
     BRANCH = "Branch"
     FEEDER = "Feeder"
     SUBFEED = "Subfeed"
 
-    def __str__( self ):
+    def __str__(self):
         return self.value
 
     @property
-    def plural( self ):
+    def plural(self):
         if self.value == "Mains":
             return self.value
         if self.value == "Branch":
             return self.value + "es"
         return self.value + "s"
 
+
 voltage_type_strings = {
     "AC100To127V": "100 V to 127 V AC",
     "AC100To240V": "100 V to 240 V AC",
     "AC100To277V": "100 V to 277 V AC",
     "AC120V": "120 V AC",
     "AC200To240V": "200 V to 240 V AC",
     "AC200To277V": "200 V to 277 V AC",
@@ -87,24 +96,24 @@
     "AC277V": "277 V AC",
     "AC277AndDC380V": "277 V AC/380 V DC",
     "AC400V": "400 V AC",
     "AC480V": "480 V AC",
     "DC48V": "48 V DC",
     "DC240V": "240 V DC",
     "DC380V": "380 V DC",
-    "DCNeg48V": "-48 V DC"
+    "DCNeg48V": "-48 V DC",
 }
 
 phase_wiring_type_strings = {
     "OnePhase3Wire": "1 Phase, 3 Wire",
     "TwoPhase3Wire": "2 Phase, 3 Wire",
     "OneOrTwoPhase3Wire": "1 or 2 Phase, 3 Wire",
     "TwoPhase4Wire": "2 Phase, 4 Wire",
     "ThreePhase4Wire": "3 Phase, 4 Wire",
-    "ThreePhase5Wire": "3 Phase, 5 Wire"
+    "ThreePhase5Wire": "3 Phase, 5 Wire",
 }
 
 receptical_type_strings = {
     "BS_1363_Type_G": "BS 1363 Type G (250V; 13A)",
     "BusConnection": "Electrical bus connection",
     "CEE_7_Type_E": "CEE 7/7 Type E (250V; 16A)",
     "CEE_7_Type_F": "CEE 7/7 Type F (250V; 16A)",
@@ -113,15 +122,15 @@
     "NEMA_5_15R": "NEMA 5-15R (120V; 15A)",
     "NEMA_5_20R": "NEMA 5-20R (120V; 20A)",
     "NEMA_L5_20R": "NEMA L5-20R (120V; 20A)",
     "NEMA_L5_30R": "NEMA L5-30R (120V; 30A)",
     "NEMA_L6_20R": "NEMA L6-20R (250V; 20A)",
     "NEMA_L6_30R": "NEMA L6-30R (250V; 30A)",
     "SEV_1011_TYPE_12": "SEV 1011 Type 12 (250V; 10A)",
-    "SEV_1011_TYPE_23": "SEV 1011 Type 23 (250V; 16A)"
+    "SEV_1011_TYPE_23": "SEV 1011 Type 23 (250V; 16A)",
 }
 
 plug_type_strings = {
     "California_CS8265": "California Standard CS8265 (Single-phase 250V; 50A; 2P3W)",
     "California_CS8365": "California Standard CS8365 (Three-phase 250V; 50A; 3P4W)",
     "Field_208V_3P4W_60A": "Field-wired; Three-phase 200-250V; 60A; 3P4W",
     "Field_400V_3P5W_32A": "Field-wired; Three-phase 200-240/346-415V; 32A; 3P5W",
@@ -148,113 +157,137 @@
     "NEMA_L22_20P": "NEMA L22-20P (Three-phase 277/480V; 20A; 3P5W)",
     "NEMA_L22_30P": "NEMA L22-30P (Three-phase 277/480V; 30A; 3P5W)",
     "NEMA_L5_15P": "NEMA L5-15P (Single-phase 125V; 15A; 1P3W)",
     "NEMA_L5_20P": "NEMA L5-20P (Single-phase 125V; 20A; 1P3W)",
     "NEMA_L5_30P": "NEMA L5-30P (Single-phase 125V; 30A; 1P3W)",
     "NEMA_L6_15P": "NEMA L6-15P (Single-phase 250V; 15A; 2P3W)",
     "NEMA_L6_20P": "NEMA L6-20P (Single-phase 250V; 20A; 2P3W)",
-    "NEMA_L6_30P": "NEMA L6-30P (Single-phase 250V; 30A; 2P3W)"
+    "NEMA_L6_30P": "NEMA L6-30P (Single-phase 250V; 30A; 2P3W)",
 }
 
 line_measurement_strings = {
     "Line1ToLine2": "L1-L2",
     "Line1ToNeutral": "L1-N",
     "Line2ToLine3": "L2-L3",
     "Line2ToNeutral": "L2-N",
     "Line3ToLine1": "L3-L1",
     "Line3ToNeutral": "L3-N",
     "Line1": "L1",
     "Line2": "L2",
     "Line3": "L3",
-    "Neutral": "N"
+    "Neutral": "N",
 }
 
-def get_power_equipment_ids( context ):
+
+def get_power_equipment_ids(context):
     """
     Finds the power equipment and returns all power equipment identifiers
 
     Args:
         context: The Redfish client object with an open session
 
     Returns:
         A dictionary containing lists of identifiers for each type of power equipment
     """
 
     # Get the service root to find the power equipment
-    service_root = context.get( "/redfish/v1/" )
+    service_root = context.get("/redfish/v1/")
     if "PowerEquipment" not in service_root.dict:
         # No power equipment
-        raise RedfishPowerEquipmentNotFoundError( "The service does not contain any power equipment" )
+        raise RedfishPowerEquipmentNotFoundError("The service does not contain any power equipment")
 
     # Get the power equipment sets
-    power_equipment = context.get( service_root.dict["PowerEquipment"]["@odata.id"] )
-    verify_response( power_equipment )
+    power_equipment = context.get(service_root.dict["PowerEquipment"]["@odata.id"])
+    verify_response(power_equipment)
 
     # Build up the lists of identifiers from the power equipment
     power_equipment_identifiers = {}
     for equip_type in power_equipment_types:
         power_equipment_identifiers[equip_type.plural] = []
         if equip_type.plural in power_equipment.dict:
             # Get the collection identifiers for this power equipment type
-            power_equipment_identifiers[equip_type.plural] = get_collection_ids( context, power_equipment.dict[equip_type.plural]["@odata.id"])
+            power_equipment_identifiers[equip_type.plural] = get_collection_ids(
+                context, power_equipment.dict[equip_type.plural]["@odata.id"]
+            )
 
     return power_equipment_identifiers
 
-def get_power_equipment_summary( context ):
+
+def get_power_equipment_summary(context):
     """
     Gets a summary of all power equipment
 
     Args:
         context: The Redfish client object with an open session
 
     Returns:
         A dictionary containing lists of summary info for each type of power equipment
     """
 
     # Get the equipment identifiers
-    power_equipment_identifiers = get_power_equipment_ids( context )
+    power_equipment_identifiers = get_power_equipment_ids(context)
 
     # Build up the lists of summary info from the discovered identifiers
     power_equipment_summary = {}
     for equipment_type in power_equipment_types:
         power_equipment_summary[equipment_type.plural] = []
         if equipment_type.plural in power_equipment_identifiers:
             for equip in power_equipment_identifiers[equipment_type.plural]:
                 # Get the equipment info
-                equipment = get_power_equipment( context, equipment_type, equip )
+                equipment = get_power_equipment(context, equipment_type, equip)
                 summary = {
-                    "Id": equipment["Info"].dict.get( "Id" ),
-                    "Model": equipment["Info"].dict.get( "Model" ),
-                    "SerialNumber": equipment["Info"].dict.get( "SerialNumber" ),
-                    "State": equipment["Info"].dict.get( "Status", {} ).get( "State" ),
-                    "Health": equipment["Info"].dict.get( "Status", {} ).get( "Health" )
+                    "Id": equipment["Info"].dict.get("Id"),
+                    "Model": equipment["Info"].dict.get("Model"),
+                    "SerialNumber": equipment["Info"].dict.get("SerialNumber"),
+                    "State": equipment["Info"].dict.get("Status", {}).get("State"),
+                    "Health": equipment["Info"].dict.get("Status", {}).get("Health"),
                 }
-                power_equipment_summary[equipment_type.plural].append( summary )
+                power_equipment_summary[equipment_type.plural].append(summary)
 
     return power_equipment_summary
 
-def print_power_equipment_summary( power_equipment_summary ):
+
+def print_power_equipment_summary(power_equipment_summary):
     """
     Prints the power equipment summary into a table
 
     Args:
         power_equipment_summary: The power equipment summary to print
     """
 
     summary_line_format = "  {:16s} | {:16s} | {:16s} | {:12s} | {:8s}"
 
     for equipment_type in power_equipment_summary:
-        if len( power_equipment_summary[equipment_type] ):
-            print( equipment_type )
-            print( summary_line_format.format( "Id", "Model", "Serial Number", "State", "Health" ) )
+        if len(power_equipment_summary[equipment_type]):
+            print(equipment_type)
+            print(summary_line_format.format("Id", "Model", "Serial Number", "State", "Health"))
             for equipment in power_equipment_summary[equipment_type]:
-                print( summary_line_format.format( equipment["Id"], equipment["Model"], equipment["SerialNumber"], equipment["State"], equipment["Health"] ) )
-            print( "" )
-
-def get_power_equipment( context, power_equipment_type, power_equipment_id = None, get_metrics = False, get_outlets = False, get_mains = False, get_branches = False, get_feeders = False, get_subfeeds = False ):
+                print(
+                    summary_line_format.format(
+                        equipment["Id"],
+                        equipment["Model"],
+                        equipment["SerialNumber"],
+                        equipment["State"],
+                        equipment["Health"],
+                    )
+                )
+            print("")
+
+
+def get_power_equipment(
+    context,
+    power_equipment_type,
+    power_equipment_id=None,
+    get_metrics=False,
+    get_outlets=False,
+    get_mains=False,
+    get_branches=False,
+    get_feeders=False,
+    get_subfeeds=False,
+):
     """
     Finds a power equipment matching the given identifier and returns its resource
 
     Args:
         context: The Redfish client object with an open session
         power_equipment_type: The power equipment type to get; see power_equipment_types enumeration
         power_equipment_id: The power equipment to locate; if None, perform on the only power equipment
@@ -267,101 +300,139 @@
 
     Returns:
         A dictionary containing the power equipment resource and optional subordinate resources
     """
 
     power_equipment_uri_pattern = "/redfish/v1/PowerEquipment/" + power_equipment_type.plural + "/{}"
     avail_power_equipment = None
-    power_equipment = {
-        "Info": None
-    }
+    power_equipment = {"Info": None}
 
     # If given an identifier, get the power equipment directly
     if power_equipment_id is not None:
-        power_equipment["Info"] = context.get( power_equipment_uri_pattern.format( power_equipment_id ) )
+        power_equipment["Info"] = context.get(power_equipment_uri_pattern.format(power_equipment_id))
     # No identifier given; see if there's exactly one member
     else:
-        all_power_equipment = get_power_equipment_ids( context )
+        all_power_equipment = get_power_equipment_ids(context)
         if power_equipment_type.plural not in all_power_equipment:
-            raise RedfishPowerEquipmentNotFoundError( "The service does not contain any {}".format( power_equipment_type.plural ) )
+            raise RedfishPowerEquipmentNotFoundError(
+                "The service does not contain any {}".format(power_equipment_type.plural)
+            )
         avail_power_equipment = all_power_equipment[power_equipment_type.plural]
-        if len( avail_power_equipment ) == 1:
-            power_equipment["Info"] = context.get( power_equipment_uri_pattern.format( avail_power_equipment[0] ) )
+        if len(avail_power_equipment) == 1:
+            power_equipment["Info"] = context.get(power_equipment_uri_pattern.format(avail_power_equipment[0]))
         else:
-            raise RedfishPowerEquipmentNotFoundError( "The service contains multiple {}; a target power equipment needs to be specified: {}".format( power_equipment_type.plural, ", ".join( avail_power_equipment ) ) )
+            raise RedfishPowerEquipmentNotFoundError(
+                "The service contains multiple {}; a target power equipment needs to be specified: {}".format(
+                    power_equipment_type.plural, ", ".join(avail_power_equipment)
+                )
+            )
 
     # Check the response and return the manager if the response is good
     if power_equipment["Info"].status == 404:
         if avail_power_equipment is None:
-            all_equipment = get_power_equipment_ids( context )
+            all_equipment = get_power_equipment_ids(context)
             if power_equipment_type.plural not in all_equipment:
-                raise RedfishPowerEquipmentNotFoundError( "The service does not contain any {}".format( power_equipment_type.plural ) )
+                raise RedfishPowerEquipmentNotFoundError(
+                    "The service does not contain any {}".format(power_equipment_type.plural)
+                )
             avail_equipment = all_equipment[power_equipment_type.plural]
-        raise RedfishPowerEquipmentNotFoundError( "The service does not contain any {} called {}; valid {}: {}".format( power_equipment_type.plural, power_equipment_id, power_equipment_type.plural, ", ".join( avail_equipment ) ) )
-    verify_response( power_equipment["Info"] )
+        raise RedfishPowerEquipmentNotFoundError(
+            "The service does not contain any {} called {}; valid {}: {}".format(
+                power_equipment_type.plural, power_equipment_id, power_equipment_type.plural, ", ".join(avail_equipment)
+            )
+        )
+    verify_response(power_equipment["Info"])
 
     # Get each of the subordinate resources requested by the caller
     resource_grabber = [
-        { "Property": "Metrics", "Parameter": get_metrics, "Collection": False },
-        { "Property": "Outlets", "Parameter": get_outlets, "Collection": True },
-        { "Property": "Mains", "Parameter": get_mains, "Collection": True },
-        { "Property": "Branches", "Parameter": get_branches, "Collection": True },
-        { "Property": "Feeders", "Parameter": get_feeders, "Collection": True },
-        { "Property": "Subfeeds", "Parameter": get_subfeeds, "Collection": True }
+        {"Property": "Metrics", "Parameter": get_metrics, "Collection": False},
+        {"Property": "Outlets", "Parameter": get_outlets, "Collection": True},
+        {"Property": "Mains", "Parameter": get_mains, "Collection": True},
+        {"Property": "Branches", "Parameter": get_branches, "Collection": True},
+        {"Property": "Feeders", "Parameter": get_feeders, "Collection": True},
+        {"Property": "Subfeeds", "Parameter": get_subfeeds, "Collection": True},
     ]
     for resource in resource_grabber:
         power_equipment[resource["Property"]] = None
         if resource["Parameter"] and resource["Property"] in power_equipment["Info"].dict:
             if resource["Collection"]:
                 power_equipment[resource["Property"]] = []
-                collection = get_collection_ids( context, power_equipment["Info"].dict[resource["Property"]]["@odata.id"] )
+                collection = get_collection_ids(
+                    context, power_equipment["Info"].dict[resource["Property"]]["@odata.id"]
+                )
                 for member_id in collection:
-                    member = context.get( power_equipment["Info"].dict[resource["Property"]]["@odata.id"] + "/" + member_id )
-                    verify_response( member )
-                    power_equipment[resource["Property"]].append( member )
+                    member = context.get(
+                        power_equipment["Info"].dict[resource["Property"]]["@odata.id"] + "/" + member_id
+                    )
+                    verify_response(member)
+                    power_equipment[resource["Property"]].append(member)
             else:
-                power_equipment[resource["Property"]] = context.get( power_equipment["Info"].dict[resource["Property"]]["@odata.id"] )
-                verify_response( power_equipment[resource["Property"]] )
+                power_equipment[resource["Property"]] = context.get(
+                    power_equipment["Info"].dict[resource["Property"]]["@odata.id"]
+                )
+                verify_response(power_equipment[resource["Property"]])
 
     return power_equipment
 
-def print_power_equipment( power_equipment ):
+
+def print_power_equipment(power_equipment):
     """
     Prints the power equipment info
 
     Args:
         power_equipment: The power equipment info to print
     """
 
     power_equipment_line_format = "  {}: {}"
-    print( "{} {} Info".format( power_equipment["Info"].dict["EquipmentType"], power_equipment["Info"].dict["Id"] ) )
+    print("{} {} Info".format(power_equipment["Info"].dict["EquipmentType"], power_equipment["Info"].dict["Id"]))
 
-    print( "" )
-    power_equipment_properties = [ "Status", "EquipmentType", "Model", "Manufacturer", "PartNumber", "SerialNumber", "Version", "FirmwareVersion", "ProductionDate", "AssetTag", "UserLabel" ]
+    print("")
+    power_equipment_properties = [
+        "Status",
+        "EquipmentType",
+        "Model",
+        "Manufacturer",
+        "PartNumber",
+        "SerialNumber",
+        "Version",
+        "FirmwareVersion",
+        "ProductionDate",
+        "AssetTag",
+        "UserLabel",
+    ]
     for property in power_equipment_properties:
         if property in power_equipment["Info"].dict:
             prop_val = power_equipment["Info"].dict[property]
-            if isinstance( prop_val, list ):
-                prop_val = ", ".join( prop_val )
+            if isinstance(prop_val, list):
+                prop_val = ", ".join(prop_val)
             elif property == "Status":
-                prop_val = "State: {}, Health: {}".format( prop_val.get( "State", "N/A" ), prop_val.get( "Health", "N/A" ) )
-            print( power_equipment_line_format.format( property, prop_val ) )
+                prop_val = "State: {}, Health: {}".format(prop_val.get("State", "N/A"), prop_val.get("Health", "N/A"))
+            print(power_equipment_line_format.format(property, prop_val))
     if power_equipment["Metrics"]:
-        power_equipment_properties = [ ( "PowerWatts", "Power", "W" ), ( "EnergykWh", "Energy", "kWh" ), ( "TemperatureCelsius", "Temperature", "C" ),
-            ( "HumidityPercent", "Humidity", "%" ), ( "PowerLoadPercent", "PowerLoad", "%" ), ( "AbsoluteHumidity", "AbsoluteHumidity", "g/m^3" ) ]
+        power_equipment_properties = [
+            ("PowerWatts", "Power", "W"),
+            ("EnergykWh", "Energy", "kWh"),
+            ("TemperatureCelsius", "Temperature", "C"),
+            ("HumidityPercent", "Humidity", "%"),
+            ("PowerLoadPercent", "PowerLoad", "%"),
+            ("AbsoluteHumidity", "AbsoluteHumidity", "g/m^3"),
+        ]
         for property in power_equipment_properties:
             if property[0] in power_equipment["Metrics"].dict:
                 if power_equipment["Metrics"].dict[property[0]]["Reading"] is None:
                     prop_val = "Unavailable"
                 else:
-                    prop_val = str( power_equipment["Metrics"].dict[property[0]]["Reading"] ) + " " + property[2]
-                print( power_equipment_line_format.format( property[1], prop_val ) )
-    print( "" )
+                    prop_val = str(power_equipment["Metrics"].dict[property[0]]["Reading"]) + " " + property[2]
+                print(power_equipment_line_format.format(property[1], prop_val))
+    print("")
+
 
-def get_power_equipment_electrical( context, power_equipment_type, power_equipment_electrical_type, power_equipment_id = None, electrical_id = None ):
+def get_power_equipment_electrical(
+    context, power_equipment_type, power_equipment_electrical_type, power_equipment_id=None, electrical_id=None
+):
     """
     Finds an outlet or circuit for an instance of power equipment and returns its resource
 
     Args:
         context: The Redfish client object with an open session
         power_equipment_type: The power equipment type to get; see power_equipment_types enumeration
         power_equipment_electrical_type: The electrical type to get; see power_equipment_electrical_types enumeration
@@ -369,133 +440,210 @@
         electrical_id: The outlet or circuit to locate; if None, perform on the only outlet or circuit
 
     Returns:
         The outlet or circuit resource
     """
 
     # Get the power equipment
-    power_equipment = get_power_equipment( context, power_equipment_type, power_equipment_id )
+    power_equipment = get_power_equipment(context, power_equipment_type, power_equipment_id)
 
     # Check that the power equipment has the desired electrical component type
     if power_equipment_electrical_type.plural not in power_equipment["Info"].dict:
-        raise RedfishPowerEquipmentElectricalNotFoundError( "{} {} does not contain any {}".format( power_equipment_type.plural, power_equipment["Info"].dict["Id"], power_equipment_electrical_type.plural ) )
-
-    power_equipment_electrical_uri_pattern = power_equipment["Info"].dict[power_equipment_electrical_type.plural]["@odata.id"] + "/{}"
+        raise RedfishPowerEquipmentElectricalNotFoundError(
+            "{} {} does not contain any {}".format(
+                power_equipment_type.plural, power_equipment["Info"].dict["Id"], power_equipment_electrical_type.plural
+            )
+        )
+
+    power_equipment_electrical_uri_pattern = (
+        power_equipment["Info"].dict[power_equipment_electrical_type.plural]["@odata.id"] + "/{}"
+    )
     avail_electrical = None
 
     # If given an identifier, get the outlet or circuit directly
     if electrical_id is not None:
-        electrical = context.get( power_equipment_electrical_uri_pattern.format( electrical_id ) )
+        electrical = context.get(power_equipment_electrical_uri_pattern.format(electrical_id))
     # No identifier given; see if there's exactly one member
     else:
-        avail_electrical = get_collection_ids( context, power_equipment["Info"].dict[power_equipment_electrical_type.plural]["@odata.id"] )
-        if len( avail_electrical ) == 1:
-            electrical = context.get( power_equipment_electrical_uri_pattern.format( avail_electrical[0] ) )
+        avail_electrical = get_collection_ids(
+            context, power_equipment["Info"].dict[power_equipment_electrical_type.plural]["@odata.id"]
+        )
+        if len(avail_electrical) == 1:
+            electrical = context.get(power_equipment_electrical_uri_pattern.format(avail_electrical[0]))
         else:
-            raise RedfishPowerEquipmentElectricalNotFoundError( "{} {} contains multiple {}; a target component needs to be specified: {}".format( power_equipment_type.plural, power_equipment["Info"].dict["Id"], power_equipment_electrical_type.plural, ", ".join( avail_electrical ) ) )
+            raise RedfishPowerEquipmentElectricalNotFoundError(
+                "{} {} contains multiple {}; a target component needs to be specified: {}".format(
+                    power_equipment_type.plural,
+                    power_equipment["Info"].dict["Id"],
+                    power_equipment_electrical_type.plural,
+                    ", ".join(avail_electrical),
+                )
+            )
 
     # Check the response and return the manager if the response is good
     if electrical.status == 404:
         if avail_electrical is None:
-            avail_electrical = get_collection_ids( context, power_equipment["Info"].dict[power_equipment_electrical_type.plural]["@odata.id"] )
-        raise RedfishPowerEquipmentNotFoundError( "{} {} does not contain any {} called {}; valid {}: {}".format( power_equipment_type.plural, power_equipment["Info"].dict["Id"], power_equipment_electrical_type.plural, electrical_id, power_equipment_electrical_type.plural, ", ".join( avail_electrical ) ) )
-    verify_response( electrical )
+            avail_electrical = get_collection_ids(
+                context, power_equipment["Info"].dict[power_equipment_electrical_type.plural]["@odata.id"]
+            )
+        raise RedfishPowerEquipmentNotFoundError(
+            "{} {} does not contain any {} called {}; valid {}: {}".format(
+                power_equipment_type.plural,
+                power_equipment["Info"].dict["Id"],
+                power_equipment_electrical_type.plural,
+                electrical_id,
+                power_equipment_electrical_type.plural,
+                ", ".join(avail_electrical),
+            )
+        )
+    verify_response(electrical)
     return electrical
 
-def print_power_equipment_electrical( electrical ):
+
+def print_power_equipment_electrical(electrical):
     """
     Prints the outlet or circuit info
 
     Args:
         electrical: The outlet or circuit to print
     """
 
     electrical_line_format = "  {}: {}"
     poly_phase_line_format = "    {:5s}: {}"
     if "#Outlet." in electrical.dict["@odata.type"]:
-        print( "Outlet {} Info".format( electrical.dict["Id"] ) )
+        print("Outlet {} Info".format(electrical.dict["Id"]))
     else:
-        print( "{} {} Info".format( electrical.dict["CircuitType"], electrical.dict["Id"] ) )
+        print("{} {} Info".format(electrical.dict["CircuitType"], electrical.dict["Id"]))
 
-    print( "" )
+    print("")
     # Display the simple properties
-    electrical_properties = [ "Status", "CircuitType", "CriticalCircuit", "ElectricalContext", "PhaseWiringType", "VoltageType",
-        "OutletType", "PlugType", "NominalVoltage", "RatedCurrentAmps", "BreakerState", "PowerState" ]
+    electrical_properties = [
+        "Status",
+        "CircuitType",
+        "CriticalCircuit",
+        "ElectricalContext",
+        "PhaseWiringType",
+        "VoltageType",
+        "OutletType",
+        "PlugType",
+        "NominalVoltage",
+        "RatedCurrentAmps",
+        "BreakerState",
+        "PowerState",
+    ]
     for property in electrical_properties:
         if property in electrical.dict:
             prop_val = electrical.dict[property]
-            if isinstance( prop_val, list ):
-                prop_val = ", ".join( prop_val )
+            if isinstance(prop_val, list):
+                prop_val = ", ".join(prop_val)
             elif property == "PhaseWiringType":
-                prop_val = str( phase_wiring_type_strings.get( prop_val, prop_val ) )
+                prop_val = str(phase_wiring_type_strings.get(prop_val, prop_val))
             elif property == "NominalVoltage":
-                prop_val = str( voltage_type_strings.get( prop_val, prop_val ) )
+                prop_val = str(voltage_type_strings.get(prop_val, prop_val))
             elif property == "OutletType":
-                prop_val = str( receptical_type_strings.get( prop_val, prop_val ) )
+                prop_val = str(receptical_type_strings.get(prop_val, prop_val))
             elif property == "PlugType":
-                prop_val = str( plug_type_strings.get( prop_val, prop_val ) )
+                prop_val = str(plug_type_strings.get(prop_val, prop_val))
             elif property == "Status":
-                prop_val = "State: {}, Health: {}".format( prop_val.get( "State", "N/A" ), prop_val.get( "Health", "N/A" ) )
+                prop_val = "State: {}, Health: {}".format(prop_val.get("State", "N/A"), prop_val.get("Health", "N/A"))
             else:
-                prop_val = str( prop_val )
-            print( electrical_line_format.format( property, prop_val ) )
+                prop_val = str(prop_val)
+            print(electrical_line_format.format(property, prop_val))
     # Display the embedded metrics
-    electrical_properties = [ ( "Voltage", "Voltage", "V" ), ( "CurrentAmps", "Current", "A" ), ( "PowerWatts", "Power", "W" ),
-        ( "EnergykWh", "Energy", "kWh" ), ( "FrequencyHz", "Frequency", "Hz" ), ( "PowerLoadPercent", "PowerLoad", "%" ),
-        ( "UnbalancedVoltagePercent", "UnbalancedVoltage", "%" ), ( "UnbalancedCurrentPercent", "UnbalancedCurrent", "%" ) ]
+    electrical_properties = [
+        ("Voltage", "Voltage", "V"),
+        ("CurrentAmps", "Current", "A"),
+        ("PowerWatts", "Power", "W"),
+        ("EnergykWh", "Energy", "kWh"),
+        ("FrequencyHz", "Frequency", "Hz"),
+        ("PowerLoadPercent", "PowerLoad", "%"),
+        ("UnbalancedVoltagePercent", "UnbalancedVoltage", "%"),
+        ("UnbalancedCurrentPercent", "UnbalancedCurrent", "%"),
+    ]
     for property in electrical_properties:
         if property[0] in electrical.dict:
             if electrical.dict[property[0]]["Reading"] is None:
                 prop_val = "Unavailable"
             else:
-                prop_val = str( electrical.dict[property[0]]["Reading"] ) + " " + property[2]
-            print( electrical_line_format.format( property[1], prop_val ) )
+                prop_val = str(electrical.dict[property[0]]["Reading"]) + " " + property[2]
+            print(electrical_line_format.format(property[1], prop_val))
 
         poly_phase_name = "PolyPhase" + property[0]
         if poly_phase_name in electrical.dict:
             if property[0] not in electrical.dict:
-                print( electrical_line_format.format( property[1], "" ) )
+                print(electrical_line_format.format(property[1], ""))
             for poly_phase in electrical.dict[poly_phase_name]:
                 if electrical.dict[poly_phase_name][poly_phase]["Reading"] is None:
                     prop_val = "Unavailable"
                 else:
-                    prop_val = "{:7.2f}".format( electrical.dict["PolyPhase" + property[0]][poly_phase]["Reading"] ) + " " + property[2]
-                print( poly_phase_line_format.format( line_measurement_strings.get( poly_phase, poly_phase ), prop_val ) )
-    print( "" )
+                    prop_val = (
+                        "{:7.2f}".format(electrical.dict["PolyPhase" + property[0]][poly_phase]["Reading"])
+                        + " "
+                        + property[2]
+                    )
+                print(poly_phase_line_format.format(line_measurement_strings.get(poly_phase, poly_phase), prop_val))
+    print("")
+
 
-def print_power_equipment_electrical_summary( power_equipment, electrical_type, print_heading ):
+def print_power_equipment_electrical_summary(power_equipment, electrical_type, print_heading):
     """
     Prints the circuit/outlet summary for an instance of power equipment
 
     Args:
         power_equipment: The power equipment info to print
         electrical_type: The type of electrical info to print
         print_heading: Indicates if the tabling heading should be printed
     """
 
     if not power_equipment[electrical_type.plural]:
         if print_heading:
-            print( "{} {} does not contain any {}".format( power_equipment["Info"].dict["EquipmentType"], power_equipment["Info"].dict["Id"], electrical_type.plural ) )
+            print(
+                "{} {} does not contain any {}".format(
+                    power_equipment["Info"].dict["EquipmentType"],
+                    power_equipment["Info"].dict["Id"],
+                    electrical_type.plural,
+                )
+            )
         return
 
     electrical_line_format = "  {:16s} | {:18s} | {:20s} | {:12s} | {:12s} | {:12s} | {:12s}"
     if print_heading:
-        print( "{} {} {}".format( power_equipment["Info"].dict["EquipmentType"], power_equipment["Info"].dict["Id"], electrical_type.plural ) )
-        print( "" )
-    print( electrical_line_format.format( electrical_type.value + " Id", "Nominal Voltage", "Phase Wiring", "State", "Voltage (V)", "Current (A)", "Power (W)" ) )
+        print(
+            "{} {} {}".format(
+                power_equipment["Info"].dict["EquipmentType"],
+                power_equipment["Info"].dict["Id"],
+                electrical_type.plural,
+            )
+        )
+        print("")
+    print(
+        electrical_line_format.format(
+            electrical_type.value + " Id",
+            "Nominal Voltage",
+            "Phase Wiring",
+            "State",
+            "Voltage (V)",
+            "Current (A)",
+            "Power (W)",
+        )
+    )
     for item in power_equipment[electrical_type.plural]:
         if "PolyPhaseVoltage" in item.dict:
             voltage = "Polyphase"
         else:
-            voltage = str( item.dict.get( "Voltage", {} ).get( "Reading", "---" ) )
+            voltage = str(item.dict.get("Voltage", {}).get("Reading", "---"))
         if "PolyPhaseCurrentAmps" in item.dict:
             current = "Polyphase"
         else:
-            current = str( item.dict.get( "CurrentAmps", {} ).get( "Reading", "---" ) )
-        voltage_type = item.dict.get( "NominalVoltage", "---" )
-        voltage_type = voltage_type_strings.get( voltage_type, voltage_type )
-        phase_wiring_type = item.dict.get( "PhaseWiringType", "---" )
-        phase_wiring_type = phase_wiring_type_strings.get( phase_wiring_type, phase_wiring_type )
-        state = str( item.dict.get( "Status", {} ).get( "State", "---" ) )
-        power = str( item.dict.get( "PowerWatts", {} ).get( "Reading", "---" ) )
-        print( electrical_line_format.format( item.dict["Id"], voltage_type, phase_wiring_type, state, voltage, current, power ) )
-    print( "" )
+            current = str(item.dict.get("CurrentAmps", {}).get("Reading", "---"))
+        voltage_type = item.dict.get("NominalVoltage", "---")
+        voltage_type = voltage_type_strings.get(voltage_type, voltage_type)
+        phase_wiring_type = item.dict.get("PhaseWiringType", "---")
+        phase_wiring_type = phase_wiring_type_strings.get(phase_wiring_type, phase_wiring_type)
+        state = str(item.dict.get("Status", {}).get("State", "---"))
+        power = str(item.dict.get("PowerWatts", {}).get("Reading", "---"))
+        print(
+            electrical_line_format.format(
+                item.dict["Id"], voltage_type, phase_wiring_type, state, voltage, current, power
+            )
+        )
+    print("")
```

### Comparing `redfish_utilities-3.2.8/redfish_utilities/sensors.py` & `redfish_utilities-3.2.9/redfish_utilities/sensors.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,237 +8,349 @@
 
 File : sensors.py
 
 Brief : This file contains the definitions and functionalities for scanning a
         Redfish service's Power and Thermal properties for sensor readings
 """
 
-def get_sensors( context , use_id = False ):
+
+def get_sensors(context, use_id=False):
     """
     Walks a Redfish service for sensor information
 
     Args:
         context: The Redfish client object with an open session
         use_id: Indicates whether to construct names from 'Id' property values
 
     Returns:
         A list containing all sensor readings
     """
 
     sensor_list = []
 
     # Get the service root to find the chassis collection
-    service_root = context.get( "/redfish/v1/" )
+    service_root = context.get("/redfish/v1/")
     if "Chassis" not in service_root.dict:
         # No chassis collection
         return sensor_list
 
     # Get the chassis collection and iterate through its collection
-    chassis_col = context.get( service_root.dict["Chassis"]["@odata.id"] )
+    chassis_col = context.get(service_root.dict["Chassis"]["@odata.id"])
     for chassis_member in chassis_col.dict["Members"]:
-        chassis = context.get( chassis_member["@odata.id"] )
+        chassis = context.get(chassis_member["@odata.id"])
 
         chassis_name = "Chassis " + chassis.dict["Id"]
         if use_id is False and "Name" in chassis.dict:
             chassis_name = chassis.dict["Name"]
 
         # Get the chassis status
-        chassis_instance = {
-            "ChassisName": chassis_name,
-            "Readings": []
-        }
-        sensor_list.append( chassis_instance )
-        get_discrete_status( "State", chassis.dict, chassis_instance["Readings"] )
+        chassis_instance = {"ChassisName": chassis_name, "Readings": []}
+        sensor_list.append(chassis_instance)
+        get_discrete_status("State", chassis.dict, chassis_instance["Readings"])
 
         # If the chassis contains any of the newer power/thermal models, scan based on the common sensor model
-        if "EnvironmentMetrics" in chassis.dict or "PowerSubsystem" in chassis.dict or "ThermalSubsystem" in chassis.dict or "Sensors" in chassis.dict:
+        if (
+            "EnvironmentMetrics" in chassis.dict
+            or "PowerSubsystem" in chassis.dict
+            or "ThermalSubsystem" in chassis.dict
+            or "Sensors" in chassis.dict
+        ):
             # Get readings from the EnvironmentMetrics resource if available
             if "EnvironmentMetrics" in chassis.dict:
-                environment = context.get( chassis.dict["EnvironmentMetrics"]["@odata.id"] )
-                get_excerpt_status( chassis_instance["ChassisName"], "TemperatureCelsius", "Cel", environment.dict, chassis_instance["Readings"] )
-                get_excerpt_status( chassis_instance["ChassisName"], "HumidityPercent", "%", environment.dict, chassis_instance["Readings"] )
-                get_excerpt_status( chassis_instance["ChassisName"], "PowerWatts", "W", environment.dict, chassis_instance["Readings"] )
-                get_excerpt_status( chassis_instance["ChassisName"], "EnergykWh", "kW.h", environment.dict, chassis_instance["Readings"] )
-                get_excerpt_status( chassis_instance["ChassisName"], "PowerLoadPercent", "%", environment.dict, chassis_instance["Readings"] )
-                get_excerpt_status( chassis_instance["ChassisName"], "DewPointCelsius", "Cel", environment.dict, chassis_instance["Readings"] )
+                environment = context.get(chassis.dict["EnvironmentMetrics"]["@odata.id"])
+                get_excerpt_status(
+                    chassis_instance["ChassisName"],
+                    "TemperatureCelsius",
+                    "Cel",
+                    environment.dict,
+                    chassis_instance["Readings"],
+                )
+                get_excerpt_status(
+                    chassis_instance["ChassisName"],
+                    "HumidityPercent",
+                    "%",
+                    environment.dict,
+                    chassis_instance["Readings"],
+                )
+                get_excerpt_status(
+                    chassis_instance["ChassisName"], "PowerWatts", "W", environment.dict, chassis_instance["Readings"]
+                )
+                get_excerpt_status(
+                    chassis_instance["ChassisName"], "EnergykWh", "kW.h", environment.dict, chassis_instance["Readings"]
+                )
+                get_excerpt_status(
+                    chassis_instance["ChassisName"],
+                    "PowerLoadPercent",
+                    "%",
+                    environment.dict,
+                    chassis_instance["Readings"],
+                )
+                get_excerpt_status(
+                    chassis_instance["ChassisName"],
+                    "DewPointCelsius",
+                    "Cel",
+                    environment.dict,
+                    chassis_instance["Readings"],
+                )
 
             # Get readings from the PowerSubsystem resource if available
             if "PowerSubsystem" in chassis.dict:
-                power = context.get( chassis.dict["PowerSubsystem"]["@odata.id"] )
+                power = context.get(chassis.dict["PowerSubsystem"]["@odata.id"])
 
                 # Add information for each power supply reported
                 if "PowerSupplies" in power.dict:
-                    power_supplies = context.get( power.dict["PowerSupplies"]["@odata.id"] )
+                    power_supplies = context.get(power.dict["PowerSupplies"]["@odata.id"])
                     for power_supply_member in power_supplies.dict["Members"]:
-                        power_supply = context.get( power_supply_member["@odata.id"] )
+                        power_supply = context.get(power_supply_member["@odata.id"])
                         power_supply_name = "Power Supply " + power_supply.dict["Id"]
                         if use_id is False and "Name" in power_supply.dict:
                             power_supply_name = power_supply.dict["Name"]
-                        get_discrete_status( power_supply_name + " State", power_supply.dict, chassis_instance["Readings"] )
+                        get_discrete_status(
+                            power_supply_name + " State", power_supply.dict, chassis_instance["Readings"]
+                        )
                         if "Metrics" in power_supply.dict:
-                            metrics = context.get( power_supply.dict["Metrics"]["@odata.id"] )
-                            get_excerpt_status( power_supply_name, "InputVoltage", "V", metrics.dict, chassis_instance["Readings"] )
-                            get_excerpt_status( power_supply_name, "InputCurrentAmps", "A", metrics.dict, chassis_instance["Readings"] )
-                            get_excerpt_status( power_supply_name, "InputPowerWatts", "W", metrics.dict, chassis_instance["Readings"] )
-                            get_excerpt_status( power_supply_name, "EnergykWh", "kW.h", metrics.dict, chassis_instance["Readings"] )
-                            get_excerpt_status( power_supply_name, "FrequencyHz", "Hz", metrics.dict, chassis_instance["Readings"] )
-                            get_excerpt_status( power_supply_name, "OutputPowerWatts", "W", metrics.dict, chassis_instance["Readings"] )
-                            get_excerpt_status( power_supply_name, "RailVoltage", "V", metrics.dict, chassis_instance["Readings"] )
-                            get_excerpt_status( power_supply_name, "RailCurrentAmps", "A", metrics.dict, chassis_instance["Readings"] )
-                            get_excerpt_status( power_supply_name, "RailPowerWatts", "W", metrics.dict, chassis_instance["Readings"] )
-                            get_excerpt_status( power_supply_name, "TemperatureCelsius", "Cel", metrics.dict, chassis_instance["Readings"] )
-                            get_excerpt_status( power_supply_name, "FanSpeedPercent", "%", metrics.dict, chassis_instance["Readings"] )
+                            metrics = context.get(power_supply.dict["Metrics"]["@odata.id"])
+                            get_excerpt_status(
+                                power_supply_name, "InputVoltage", "V", metrics.dict, chassis_instance["Readings"]
+                            )
+                            get_excerpt_status(
+                                power_supply_name, "InputCurrentAmps", "A", metrics.dict, chassis_instance["Readings"]
+                            )
+                            get_excerpt_status(
+                                power_supply_name, "InputPowerWatts", "W", metrics.dict, chassis_instance["Readings"]
+                            )
+                            get_excerpt_status(
+                                power_supply_name, "EnergykWh", "kW.h", metrics.dict, chassis_instance["Readings"]
+                            )
+                            get_excerpt_status(
+                                power_supply_name, "FrequencyHz", "Hz", metrics.dict, chassis_instance["Readings"]
+                            )
+                            get_excerpt_status(
+                                power_supply_name, "OutputPowerWatts", "W", metrics.dict, chassis_instance["Readings"]
+                            )
+                            get_excerpt_status(
+                                power_supply_name, "RailVoltage", "V", metrics.dict, chassis_instance["Readings"]
+                            )
+                            get_excerpt_status(
+                                power_supply_name, "RailCurrentAmps", "A", metrics.dict, chassis_instance["Readings"]
+                            )
+                            get_excerpt_status(
+                                power_supply_name, "RailPowerWatts", "W", metrics.dict, chassis_instance["Readings"]
+                            )
+                            get_excerpt_status(
+                                power_supply_name,
+                                "TemperatureCelsius",
+                                "Cel",
+                                metrics.dict,
+                                chassis_instance["Readings"],
+                            )
+                            get_excerpt_status(
+                                power_supply_name, "FanSpeedPercent", "%", metrics.dict, chassis_instance["Readings"]
+                            )
 
                 # Add information for each battery reported
                 if "Batteries" in power.dict:
-                    batteries = context.get( power.dict["Batteries"]["@odata.id"] )
+                    batteries = context.get(power.dict["Batteries"]["@odata.id"])
                     for battery_member in batteries.dict["Members"]:
-                        battery = context.get( battery_member["@odata.id"] )
+                        battery = context.get(battery_member["@odata.id"])
                         battery_name = "Battery " + battery.dict["Id"]
                         if use_id is False and "Name" in battery.dict:
                             battery_name = battery.dict["Name"]
-                        get_discrete_status( battery_name + " State", battery.dict, chassis_instance["Readings"] )
-                        get_excerpt_status( battery_name, "StateOfHealthPercent", "%", battery.dict, chassis_instance["Readings"])
+                        get_discrete_status(battery_name + " State", battery.dict, chassis_instance["Readings"])
+                        get_excerpt_status(
+                            battery_name, "StateOfHealthPercent", "%", battery.dict, chassis_instance["Readings"]
+                        )
                         if "Metrics" in battery.dict:
-                            metrics = context.get( battery.dict["Metrics"]["@odata.id"] )
-                            get_excerpt_status( battery_name, "InputVoltage", "V", metrics.dict, chassis_instance["Readings"] )
-                            get_excerpt_status( battery_name, "InputCurrentAmps", "A", metrics.dict, chassis_instance["Readings"] )
-                            get_excerpt_status( battery_name, "OutputVoltages", "V", metrics.dict, chassis_instance["Readings"] )
-                            get_excerpt_status( battery_name, "OutputCurrentAmps", "A", metrics.dict, chassis_instance["Readings"] )
-                            get_excerpt_status( battery_name, "StoredEnergyWattHours", "W.h", metrics.dict, chassis_instance["Readings"] )
-                            get_excerpt_status( battery_name, "StoredChargeAmpHours", "A.h", metrics.dict, chassis_instance["Readings"] )
-                            get_excerpt_status( battery_name, "TemperatureCelsius", "Cel", metrics.dict, chassis_instance["Readings"] )
-                            get_excerpt_status( battery_name, "ChargePercent", "%", metrics.dict, chassis_instance["Readings"] )
-                            get_excerpt_status( battery_name, "CellVoltages", "V", metrics.dict, chassis_instance["Readings"] )
+                            metrics = context.get(battery.dict["Metrics"]["@odata.id"])
+                            get_excerpt_status(
+                                battery_name, "InputVoltage", "V", metrics.dict, chassis_instance["Readings"]
+                            )
+                            get_excerpt_status(
+                                battery_name, "InputCurrentAmps", "A", metrics.dict, chassis_instance["Readings"]
+                            )
+                            get_excerpt_status(
+                                battery_name, "OutputVoltages", "V", metrics.dict, chassis_instance["Readings"]
+                            )
+                            get_excerpt_status(
+                                battery_name, "OutputCurrentAmps", "A", metrics.dict, chassis_instance["Readings"]
+                            )
+                            get_excerpt_status(
+                                battery_name, "StoredEnergyWattHours", "W.h", metrics.dict, chassis_instance["Readings"]
+                            )
+                            get_excerpt_status(
+                                battery_name, "StoredChargeAmpHours", "A.h", metrics.dict, chassis_instance["Readings"]
+                            )
+                            get_excerpt_status(
+                                battery_name, "TemperatureCelsius", "Cel", metrics.dict, chassis_instance["Readings"]
+                            )
+                            get_excerpt_status(
+                                battery_name, "ChargePercent", "%", metrics.dict, chassis_instance["Readings"]
+                            )
+                            get_excerpt_status(
+                                battery_name, "CellVoltages", "V", metrics.dict, chassis_instance["Readings"]
+                            )
 
                 # Add information for each of the redundancy groups reported
                 if "PowerSupplyRedundancy" in power.dict:
-                    for i, redundancy in enumerate( power.dict["PowerSupplyRedundancy"] ):
-                        redundancy_name = "Power Supply Redundancy " + str( i )
+                    for i, redundancy in enumerate(power.dict["PowerSupplyRedundancy"]):
+                        redundancy_name = "Power Supply Redundancy " + str(i)
                         if use_id is False and "Name" in redundancy:
                             redundancy_name = redundancy["Name"]
-                        get_discrete_status( redundancy_name, redundancy, chassis_instance["Readings"] )
+                        get_discrete_status(redundancy_name, redundancy, chassis_instance["Readings"])
 
             # Get readings from the ThermalSubsystem resource if available
             if "ThermalSubsystem" in chassis.dict:
-                thermal = context.get( chassis.dict["ThermalSubsystem"]["@odata.id"] )
+                thermal = context.get(chassis.dict["ThermalSubsystem"]["@odata.id"])
 
                 # Add overall thermal metrics
                 if "ThermalMetrics" in thermal.dict:
-                    metrics = context.get( thermal.dict["ThermalMetrics"]["@odata.id"] )
+                    metrics = context.get(thermal.dict["ThermalMetrics"]["@odata.id"])
                     if "TemperatureSummaryCelsius" in metrics.dict:
-                        get_excerpt_status( chassis_instance["ChassisName"], "Internal", "Cel", metrics.dict["TemperatureSummaryCelsius"], chassis_instance["Readings"] )
-                        get_excerpt_status( chassis_instance["ChassisName"], "Intake", "Cel", metrics.dict["TemperatureSummaryCelsius"], chassis_instance["Readings"] )
-                        get_excerpt_status( chassis_instance["ChassisName"], "Exhaust", "Cel", metrics.dict["TemperatureSummaryCelsius"], chassis_instance["Readings"] )
-                        get_excerpt_status( chassis_instance["ChassisName"], "Ambient", "Cel", metrics.dict["TemperatureSummaryCelsius"], chassis_instance["Readings"] )
+                        get_excerpt_status(
+                            chassis_instance["ChassisName"],
+                            "Internal",
+                            "Cel",
+                            metrics.dict["TemperatureSummaryCelsius"],
+                            chassis_instance["Readings"],
+                        )
+                        get_excerpt_status(
+                            chassis_instance["ChassisName"],
+                            "Intake",
+                            "Cel",
+                            metrics.dict["TemperatureSummaryCelsius"],
+                            chassis_instance["Readings"],
+                        )
+                        get_excerpt_status(
+                            chassis_instance["ChassisName"],
+                            "Exhaust",
+                            "Cel",
+                            metrics.dict["TemperatureSummaryCelsius"],
+                            chassis_instance["Readings"],
+                        )
+                        get_excerpt_status(
+                            chassis_instance["ChassisName"],
+                            "Ambient",
+                            "Cel",
+                            metrics.dict["TemperatureSummaryCelsius"],
+                            chassis_instance["Readings"],
+                        )
 
                 # Add information for each fan reported
                 if "Fans" in thermal.dict:
-                    fans = context.get( thermal.dict["Fans"]["@odata.id"] )
+                    fans = context.get(thermal.dict["Fans"]["@odata.id"])
                     for fan_member in fans.dict["Members"]:
-                        fan = context.get( fan_member["@odata.id"] )
+                        fan = context.get(fan_member["@odata.id"])
                         fan_name = "Fan " + fan.dict["Id"]
                         if use_id is False and "Name" in fan.dict:
                             fan_name = fan.dict["Name"]
-                        get_discrete_status( fan_name + " State", fan.dict, chassis_instance["Readings"] )
-                        get_excerpt_status( fan_name, "SpeedPercent", "%", fan.dict, chassis_instance["Readings"])
+                        get_discrete_status(fan_name + " State", fan.dict, chassis_instance["Readings"])
+                        get_excerpt_status(fan_name, "SpeedPercent", "%", fan.dict, chassis_instance["Readings"])
 
                 # Add information for each of the redundancy groups reported
                 if "FanRedundancy" in thermal.dict:
-                    for i, redundancy in enumerate( thermal.dict["FanRedundancy"] ):
-                        redundancy_name = "Fan Redundancy " + str( i )
+                    for i, redundancy in enumerate(thermal.dict["FanRedundancy"]):
+                        redundancy_name = "Fan Redundancy " + str(i)
                         if use_id is False and "Name" in redundancy:
                             redundancy_name = redundancy["Name"]
-                        get_discrete_status( redundancy_name, redundancy, chassis_instance["Readings"] )
+                        get_discrete_status(redundancy_name, redundancy, chassis_instance["Readings"])
 
             # Get all sensor readings if available
             if "Sensors" in chassis.dict:
-                sensors = context.get( chassis.dict["Sensors"]["@odata.id"] )
+                sensors = context.get(chassis.dict["Sensors"]["@odata.id"])
                 for sensor_member in sensors.dict["Members"]:
-                    sensor = context.get( sensor_member["@odata.id"] )
-                    get_sensor_status( sensor.dict, chassis_instance["Readings"] , use_id = use_id)
+                    sensor = context.get(sensor_member["@odata.id"])
+                    get_sensor_status(sensor.dict, chassis_instance["Readings"], use_id=use_id)
 
         # Older power/thermal models
         else:
             # Get readings from the Power resource if available
             if "Power" in chassis.dict:
-                power = context.get( chassis.dict["Power"]["@odata.id"] )
+                power = context.get(chassis.dict["Power"]["@odata.id"])
 
                 # Add information for each power supply reported
                 if "PowerSupplies" in power.dict:
                     for power_supply in power.dict["PowerSupplies"]:
                         power_supply_name = "Power Supply " + power_supply["MemberId"]
                         if use_id is False and "Name" in power_supply:
                             power_supply_name = power_supply["Name"]
-                        get_discrete_status( power_supply_name + " State", power_supply, chassis_instance["Readings"] )
-                        get_analog_status_small( power_supply_name, "ReadingVolts", "V", power_supply, chassis_instance["Readings"] )
-                        get_analog_status_small( power_supply_name, "LineInputVoltage", "V", power_supply, chassis_instance["Readings"] )
-                        get_analog_status_small( power_supply_name, "PowerCapacityWatts", "W", power_supply, chassis_instance["Readings"] )
-                        get_analog_status_small( power_supply_name, "LastPowerOutputWatts", "W", power_supply, chassis_instance["Readings"] )
+                        get_discrete_status(power_supply_name + " State", power_supply, chassis_instance["Readings"])
+                        get_analog_status_small(
+                            power_supply_name, "ReadingVolts", "V", power_supply, chassis_instance["Readings"]
+                        )
+                        get_analog_status_small(
+                            power_supply_name, "LineInputVoltage", "V", power_supply, chassis_instance["Readings"]
+                        )
+                        get_analog_status_small(
+                            power_supply_name, "PowerCapacityWatts", "W", power_supply, chassis_instance["Readings"]
+                        )
+                        get_analog_status_small(
+                            power_supply_name, "LastPowerOutputWatts", "W", power_supply, chassis_instance["Readings"]
+                        )
 
                 # Add information for each of the voltages reported
                 if "Voltages" in power.dict:
                     for voltage in power.dict["Voltages"]:
                         voltage_name = "Voltage " + voltage["MemberId"]
                         if use_id is False and "Name" in voltage:
                             voltage_name = voltage["Name"]
-                        get_analog_status_full( voltage_name, voltage, chassis_instance["Readings"] )
+                        get_analog_status_full(voltage_name, voltage, chassis_instance["Readings"])
 
                 # Add information for each of the redundancy groups reported
                 if "Redundancy" in power.dict:
-                    for i, redundancy in enumerate( power.dict["Redundancy"] ):
-                        redundancy_name = "Power Supply Redundancy " + str( i )
+                    for i, redundancy in enumerate(power.dict["Redundancy"]):
+                        redundancy_name = "Power Supply Redundancy " + str(i)
                         if use_id is False and "Name" in redundancy:
                             redundancy_name = redundancy["Name"]
-                        get_discrete_status( redundancy_name, redundancy, chassis_instance["Readings"] )
+                        get_discrete_status(redundancy_name, redundancy, chassis_instance["Readings"])
 
             # Get readings from the Thermal resource if available
             if "Thermal" in chassis.dict:
-                thermal = context.get( chassis.dict["Thermal"]["@odata.id"] )
+                thermal = context.get(chassis.dict["Thermal"]["@odata.id"])
 
                 # Add information for each of the temperatures reported
                 if "Temperatures" in thermal.dict:
                     for temperature in thermal.dict["Temperatures"]:
                         temperature_name = "Temperature " + temperature["MemberId"]
                         if use_id is False and "Name" in temperature:
                             temperature_name = temperature["Name"]
-                        get_analog_status_full( temperature_name, temperature, chassis_instance["Readings"] )
+                        get_analog_status_full(temperature_name, temperature, chassis_instance["Readings"])
 
                 # Add information for each of the fans reported
                 if "Fans" in thermal.dict:
                     for fan in thermal.dict["Fans"]:
                         fan_name = "Fan " + fan["MemberId"]
                         if use_id is False and "Name" in fan:
                             fan_name = fan["Name"]
-                        get_analog_status_full( fan_name, fan, chassis_instance["Readings"] )
+                        get_analog_status_full(fan_name, fan, chassis_instance["Readings"])
 
                 # Add information for each of the redundancy groups reported
                 if "Redundancy" in thermal.dict:
-                    for i, redundancy in enumerate( thermal.dict["Redundancy"] ):
-                        redundancy_name = "Fan Redundancy " + str( i )
+                    for i, redundancy in enumerate(thermal.dict["Redundancy"]):
+                        redundancy_name = "Fan Redundancy " + str(i)
                         if use_id is False and "Name" in redundancy:
                             redundancy_name = redundancy["Name"]
-                        get_discrete_status( redundancy_name, redundancy, chassis_instance["Readings"] )
+                        get_discrete_status(redundancy_name, redundancy, chassis_instance["Readings"])
 
     return sensor_list
 
-def get_discrete_status( name, object, readings ):
+
+def get_discrete_status(name, object, readings):
     """
     Builds the status reading based on the Status property
 
     Args:
         name: The name to apply to the reading
         object: The object to parse
         readings: The list of readings to update
     """
 
     if "Status" not in object:
         # Do not produce a dummy reading if Status is not found
         return
-    state, health = get_status( object )
+    state, health = get_status(object)
 
     reading = {
         "Name": name,
         "Reading": state,
         "Units": None,
         "State": state,
         "Health": health,
@@ -247,27 +359,28 @@
         "LowerCaution": None,
         "UpperCaution": None,
         "UpperCritical": None,
         "UpperFatal": None,
         "PhysicalContext": None,
     }
 
-    readings.append( reading )
+    readings.append(reading)
 
-def get_analog_status_full( name, object, readings ):
+
+def get_analog_status_full(name, object, readings):
     """
     Builds a full analog reading based on the the contents of an object
 
     Args:
         name: The name to apply to the reading
         object: The object to parse
         readings: The list of readings to update
     """
 
-    state, health = get_status( object )
+    state, health = get_status(object)
     units = None
 
     if "ReadingCelsius" in object:
         reading_val = object["ReadingCelsius"]
         units = "Cel"
     elif "ReadingVolts" in object:
         reading_val = object["ReadingVolts"]
@@ -287,26 +400,27 @@
 
     reading = {
         "Name": name,
         "Reading": reading_val,
         "Units": units,
         "State": state,
         "Health": health,
-        "LowerFatal": object.get( "LowerThresholdFatal", None ),
-        "LowerCritical": object.get( "LowerThresholdCritical", None ),
-        "LowerCaution": object.get( "LowerThresholdNonCritical", None ),
-        "UpperCaution": object.get( "UpperThresholdNonCritical", None ),
-        "UpperCritical": object.get( "UpperThresholdCritical", None ),
-        "UpperFatal": object.get( "UpperThresholdFatal", None ),
-        "PhysicalContext": object.get( "PhysicalContext", None ),
+        "LowerFatal": object.get("LowerThresholdFatal", None),
+        "LowerCritical": object.get("LowerThresholdCritical", None),
+        "LowerCaution": object.get("LowerThresholdNonCritical", None),
+        "UpperCaution": object.get("UpperThresholdNonCritical", None),
+        "UpperCritical": object.get("UpperThresholdCritical", None),
+        "UpperFatal": object.get("UpperThresholdFatal", None),
+        "PhysicalContext": object.get("PhysicalContext", None),
     }
 
-    readings.append( reading )
+    readings.append(reading)
+
 
-def get_analog_status_small( name, field, units, object, readings ):
+def get_analog_status_small(name, field, units, object, readings):
     """
     Builds an analog reading without thresholds based on a single field
 
     Args:
         name: The name to apply to the reading
         field: The field with the reading
         units: The units of measure for the reading
@@ -314,120 +428,123 @@
         readings: The list of readings to update
     """
 
     if field not in object:
         return
 
     reading = {
-        "Name": "{} {}".format( name, field ),
+        "Name": "{} {}".format(name, field),
         "Reading": object[field],
         "Units": units,
         "State": None,
         "Health": None,
         "LowerFatal": None,
         "LowerCritical": None,
         "LowerCaution": None,
         "UpperCaution": None,
         "UpperCritical": None,
         "UpperFatal": None,
         "PhysicalContext": None,
     }
 
-    readings.append( reading )
+    readings.append(reading)
 
-def get_excerpt_status( name, field, units, object, readings ):
+
+def get_excerpt_status(name, field, units, object, readings):
     """
     Builds an analog reading based on an excerpt
 
     Args:
         name: The name to apply to the reading
         field: The field with the reading
         units: The units of measure for the reading
         object: The object to parse
         readings: The list of readings to update
     """
 
     if field not in object:
         return
 
-    if isinstance( object[field], list ):
-        for i, item in enumerate( object[field] ):
+    if isinstance(object[field], list):
+        for i, item in enumerate(object[field]):
             if "DataSourceUri" not in item:
                 reading = {
-                    "Name": "{} {} {}".format( name, field, i ),
-                    "Reading": item.get( "Reading", None ),
+                    "Name": "{} {} {}".format(name, field, i),
+                    "Reading": item.get("Reading", None),
                     "Units": units,
                     "State": None,
                     "Health": None,
                     "LowerFatal": None,
                     "LowerCritical": None,
                     "LowerCaution": None,
                     "UpperCaution": None,
                     "UpperCritical": None,
                     "UpperFatal": None,
                     "PhysicalContext": None,
                 }
-                readings.append( reading )
+                readings.append(reading)
     else:
         if "DataSourceUri" not in object[field]:
             reading = {
-                "Name": "{} {}".format( name, field ),
-                "Reading": object[field].get( "Reading", None ),
+                "Name": "{} {}".format(name, field),
+                "Reading": object[field].get("Reading", None),
                 "Units": units,
                 "State": None,
                 "Health": None,
                 "LowerFatal": None,
                 "LowerCritical": None,
                 "LowerCaution": None,
                 "UpperCaution": None,
                 "UpperCritical": None,
                 "UpperFatal": None,
                 "PhysicalContext": None,
             }
-            readings.append( reading )
+            readings.append(reading)
+
 
-def get_sensor_status( sensor, readings , use_id = False ):
+def get_sensor_status(sensor, readings, use_id=False):
     """
     Builds an analog reading from a sensor
 
     Args:
         sensor: The sensor
         readings: The list of readings to update
         use_id: Indicates whether to construct names from 'Id' property values
     """
 
-    state, health = get_status( sensor )
-    units = sensor.get( "ReadingUnits", None )
-    reading_val = sensor.get( "Reading", None )
+    state, health = get_status(sensor)
+    units = sensor.get("ReadingUnits", None)
+    reading_val = sensor.get("Reading", None)
     if reading_val is None:
         reading_val = state
 
-    sensor_name = sensor.get( "Name", None )
+    sensor_name = sensor.get("Name", None)
     name = "Sensor " + sensor["Id"]
     if use_id is False and name is not None:
         name = sensor_name
 
     reading = {
         "Name": name,
         "Reading": reading_val,
         "Units": units,
         "State": state,
         "Health": health,
-        "LowerFatal": sensor.get( "Thresholds", {} ).get( "LowerFatal", {} ).get( "Reading", None ),
-        "LowerCritical": sensor.get( "Thresholds", {} ).get( "LowerCritical", {} ).get( "Reading", None ),
-        "LowerCaution": sensor.get( "Thresholds", {} ).get( "LowerCaution", {} ).get( "Reading", None ),
-        "UpperCaution": sensor.get( "Thresholds", {} ).get( "UpperCaution", {} ).get( "Reading", None ),
-        "UpperCritical": sensor.get( "Thresholds", {} ).get( "UpperCritical", {} ).get( "Reading", None ),
-        "UpperFatal": sensor.get( "Thresholds", {} ).get( "UpperFatal", {} ).get( "Reading", None ),
-        "PhysicalContext": sensor.get( "PhysicalContext", None),
+        "LowerFatal": sensor.get("Thresholds", {}).get("LowerFatal", {}).get("Reading", None),
+        "LowerCritical": sensor.get("Thresholds", {}).get("LowerCritical", {}).get("Reading", None),
+        "LowerCaution": sensor.get("Thresholds", {}).get("LowerCaution", {}).get("Reading", None),
+        "UpperCaution": sensor.get("Thresholds", {}).get("UpperCaution", {}).get("Reading", None),
+        "UpperCritical": sensor.get("Thresholds", {}).get("UpperCritical", {}).get("Reading", None),
+        "UpperFatal": sensor.get("Thresholds", {}).get("UpperFatal", {}).get("Reading", None),
+        "PhysicalContext": sensor.get("PhysicalContext", None),
     }
 
-    readings.append( reading )
+    readings.append(reading)
 
-def get_status( object ):
+
+def get_status(object):
     """
     Gets the lower status information
 
     Args:
         object: The object containing the Status property
 
     Returns:
@@ -435,58 +552,74 @@
         The health within Status (None if not found)
     """
 
     state = None
     health = None
 
     if "Status" in object:
-        state = object["Status"].get( "State", None )
-        health = object["Status"].get( "Health", None )
+        state = object["Status"].get("State", None)
+        health = object["Status"].get("Health", None)
 
     return state, health
 
-def print_sensors( sensor_list ):
+
+def print_sensors(sensor_list):
     """
     Prints the sensor list into a table
 
     Args:
         sensor_list: The sensor list to print
     """
 
     sensor_line_format = "  {:25s} | {:10s} | {:8s} | {:8s} | {:8s} | {:8s} | {:8s} | {:8s} | {:8s} | {:32s}"
 
     # Go through each chassis object in the list
     for chassis in sensor_list:
 
-        print( "Chassis '" + chassis["ChassisName"] + "' Status" )
-        print( sensor_line_format.format( "Sensor", "Reading", "Health", "LF", "LC", "LNC", "UNC", "UC", "UF", "PhysicalContext" ) )
+        print("Chassis '" + chassis["ChassisName"] + "' Status")
+        print(
+            sensor_line_format.format(
+                "Sensor", "Reading", "Health", "LF", "LC", "LNC", "UNC", "UC", "UF", "PhysicalContext"
+            )
+        )
 
         # Go through each reading in the chassis
         for reading in chassis["Readings"]:
 
             # Sanitize the data for printing; use a new object to not modify the original reading data
             reading_pr = {}
             for item in reading:
                 if item == "Name":
                     reading_pr["Name"] = reading["Name"][:25]
                 elif item == "Reading":
                     if reading["Reading"] is None:
                         reading_pr["Reading"] = "Unknown"
                     else:
-                        reading_pr["Reading"] = str( reading["Reading"] )
+                        reading_pr["Reading"] = str(reading["Reading"])
                         if reading["Units"] is not None:
                             reading_pr["Reading"] = reading_pr["Reading"] + reading["Units"]
                     reading_pr["Reading"] = reading_pr["Reading"][:10]
                 elif item == "Units":
                     if reading["Units"] is None:
                         reading_pr["Units"] = ""
                 else:
                     if reading[item] is None:
                         reading_pr[item] = "N/A"
                     else:
-                        reading_pr[item] = str( reading[item] )
+                        reading_pr[item] = str(reading[item])
 
             # Print it
-            print( sensor_line_format.format( reading_pr["Name"], reading_pr["Reading"], reading_pr["Health"],
-                reading_pr["LowerFatal"], reading_pr["LowerCritical"], reading_pr["LowerCaution"],
-                reading_pr["UpperCaution"], reading_pr["UpperCritical"], reading_pr["UpperFatal"], reading_pr["PhysicalContext"] ) )
-        print( "" )
+            print(
+                sensor_line_format.format(
+                    reading_pr["Name"],
+                    reading_pr["Reading"],
+                    reading_pr["Health"],
+                    reading_pr["LowerFatal"],
+                    reading_pr["LowerCritical"],
+                    reading_pr["LowerCaution"],
+                    reading_pr["UpperCaution"],
+                    reading_pr["UpperCritical"],
+                    reading_pr["UpperFatal"],
+                    reading_pr["PhysicalContext"],
+                )
+            )
+        print("")
```

### Comparing `redfish_utilities-3.2.8/redfish_utilities/systems.py` & `redfish_utilities-3.2.9/redfish_utilities/systems.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,76 +15,93 @@
 import warnings
 import sys
 from .collections import get_collection_ids
 from .messages import verify_response
 from .resets import reset_types
 from . import config
 
-class RedfishSystemNotFoundError( Exception ):
+
+class RedfishSystemNotFoundError(Exception):
     """
     Raised when a matching system cannot be found
     """
+
     pass
 
-class RedfishSystemResetNotFoundError( Exception ):
+
+class RedfishSystemResetNotFoundError(Exception):
     """
     Raised when the reset action cannot be found
     """
+
     pass
 
-class RedfishSystemBootNotFoundError( Exception ):
+
+class RedfishSystemBootNotFoundError(Exception):
     """
     Raised when the boot object cannot be found
     """
+
     pass
-class RedfishSystemBiosNotFoundError( Exception ):
+
+
+class RedfishSystemBiosNotFoundError(Exception):
     """
     Raised when the BIOS resource cannot be found
     """
+
     pass
 
-class RedfishSystemBiosInvalidSettingsError( Exception ):
+
+class RedfishSystemBiosInvalidSettingsError(Exception):
     """
     Raised when the BIOS resource contains a settings object, but it's not rendered properly
     """
+
     pass
 
-class RedfishVirtualMediaNotFoundError( Exception ):
+
+class RedfishVirtualMediaNotFoundError(Exception):
     """
     Raised when a system does not have any virtual media available
     """
+
     pass
 
-class RedfishNoAcceptableVirtualMediaError( Exception ):
+
+class RedfishNoAcceptableVirtualMediaError(Exception):
     """
     Raised when a system does not have virtual media available that meets criteria
     """
+
     pass
 
-def get_system_ids( context ):
+
+def get_system_ids(context):
     """
     Finds the system collection and returns all of the member's identifiers
 
     Args:
         context: The Redfish client object with an open session
 
     Returns:
         A list of identifiers of the members of the system collection
     """
 
     # Get the service root to find the system collection
-    service_root = context.get( "/redfish/v1/" )
+    service_root = context.get("/redfish/v1/")
     if "Systems" not in service_root.dict:
         # No system collection
-        raise RedfishSystemNotFoundError( "Service does not contain a system collection" )
+        raise RedfishSystemNotFoundError("Service does not contain a system collection")
 
     # Get the system collection and iterate through its collection
-    return get_collection_ids( context, service_root.dict["Systems"]["@odata.id"] )
+    return get_collection_ids(context, service_root.dict["Systems"]["@odata.id"])
 
-def get_system( context, system_id = None ):
+
+def get_system(context, system_id=None):
     """
     Finds a system matching the given identifier and returns its resource
 
     Args:
         context: The Redfish client object with an open session
         system_id: The system to locate; if None, perform on the only system
 
@@ -93,77 +110,103 @@
     """
 
     system_uri_pattern = "/redfish/v1/Systems/{}"
     avail_systems = None
 
     # If given an identifier, get the system directly
     if system_id is not None:
-        system = context.get( system_uri_pattern.format( system_id ) )
+        system = context.get(system_uri_pattern.format(system_id))
     # No identifier given; see if there's exactly one member
     else:
-        avail_systems = get_system_ids( context )
-        if len( avail_systems ) == 1:
-            system = context.get( system_uri_pattern.format( avail_systems[0] ) )
+        avail_systems = get_system_ids(context)
+        if len(avail_systems) == 1:
+            system = context.get(system_uri_pattern.format(avail_systems[0]))
         else:
-            raise RedfishSystemNotFoundError( "Service does not contain exactly one system; a target system needs to be specified: {}".format( ", ".join( avail_systems ) ) )
+            raise RedfishSystemNotFoundError(
+                "Service does not contain exactly one system; a target system needs to be specified: {}".format(
+                    ", ".join(avail_systems)
+                )
+            )
 
     # Check the response and return the system if the response is good
     if system.status == 404:
         if avail_systems is None:
-            avail_systems = get_system_ids( context )
-        raise RedfishSystemNotFoundError( "Service does not contain a system called {}; valid systems: {}".format( system_id, ", ".join( avail_systems ) ) )
-    verify_response( system )
+            avail_systems = get_system_ids(context)
+        raise RedfishSystemNotFoundError(
+            "Service does not contain a system called {}; valid systems: {}".format(system_id, ", ".join(avail_systems))
+        )
+    verify_response(system)
     return system
 
-def get_system_boot( context, system_id = None ):
+
+def get_system_boot(context, system_id=None):
     """
     Finds a system matching the given ID and returns its Boot object
 
     Args:
         context: The Redfish client object with an open session
         system_id: The system to locate; if None, perform on the only system
 
     Returns:
         The Boot object from the given system
     """
 
-    system = get_system( context, system_id )
-    boot_obj = system.dict.get( "Boot" )
+    system = get_system(context, system_id)
+    boot_obj = system.dict.get("Boot")
 
     if config.__workarounds__:
         # Try getting boot information from the settings resource
-        settings_uris = [ "Settings", "SD" ]
+        settings_uris = ["Settings", "SD"]
         for setting_ext in settings_uris:
-            system_settings = context.get( system.dict["@odata.id"] + "/" + setting_ext )
+            system_settings = context.get(system.dict["@odata.id"] + "/" + setting_ext)
             if system_settings.status == 200:
                 if "Boot" in system_settings.dict:
                     if boot_obj is None:
                         # Boot property only exists in settings, which is not expected
-                        warnings.warn( "System '{}' only reports boot information in the settings resource.  Contact your vendor.".format( system_id ) )
+                        warnings.warn(
+                            "System '{}' only reports boot information in the settings resource.  Contact your vendor.".format(
+                                system_id
+                            )
+                        )
                         boot_obj = system_settings.dict["Boot"]
                     else:
                         # Check the boot override properties; these are expected to only be in the active resource
-                        boot_override_props = [ "BootSourceOverrideTarget", "BootSourceOverrideEnabled", "BootSourceOverrideMode", "UefiTargetBootSourceOverride", "BootNext" ]
+                        boot_override_props = [
+                            "BootSourceOverrideTarget",
+                            "BootSourceOverrideEnabled",
+                            "BootSourceOverrideMode",
+                            "UefiTargetBootSourceOverride",
+                            "BootNext",
+                        ]
                         boot_ov_found = False
                         for prop in boot_override_props:
                             if prop in system_settings.dict["Boot"]:
                                 # Boot override property found; copy it over
                                 boot_ov_found = True
                                 boot_obj[prop] = system_settings.dict["Boot"][prop]
                                 if prop + "@Redfish.AllowableValues" in system_settings.dict["Boot"]:
-                                    boot_obj[prop + "@Redfish.AllowableValues"] = system_settings.dict["Boot"][prop + "@Redfish.AllowableValues"]
+                                    boot_obj[prop + "@Redfish.AllowableValues"] = system_settings.dict["Boot"][
+                                        prop + "@Redfish.AllowableValues"
+                                    ]
                         if boot_ov_found:
-                            warnings.warn( "System '{}' contains one or more boot override properties in the settings resource.  Contact your vendor.".format( system_id ) )
+                            warnings.warn(
+                                "System '{}' contains one or more boot override properties in the settings resource.  Contact your vendor.".format(
+                                    system_id
+                                )
+                            )
                 break
 
     if boot_obj is None:
-        raise RedfishSystemBootNotFoundError( "System '{}' does not contain the boot object".format( system.dict["Id"] ) )
+        raise RedfishSystemBootNotFoundError("System '{}' does not contain the boot object".format(system.dict["Id"]))
     return boot_obj
 
-def set_system_boot( context, system_id = None, ov_target = None, ov_enabled = None, ov_mode = None, ov_uefi_target = None, ov_boot_next = None ):
+
+def set_system_boot(
+    context, system_id=None, ov_target=None, ov_enabled=None, ov_mode=None, ov_uefi_target=None, ov_boot_next=None
+):
     """
     Finds a system matching the given ID and updates its Boot object
 
     Args:
         context: The Redfish client object with an open session
         system_id: The system to locate; if None, perform on the only system
         ov_target: The override target (BootSourceOverrideTarget)
@@ -173,147 +216,178 @@
         ov_boot_next: The UEFI boot next for override (BootNext)
 
     Returns:
         The response of the PATCH
     """
 
     # Check that the values themselves are supported by the schema
-    ov_target_values = [ "None", "Pxe", "Floppy", "Cd", "Usb", "Hdd", "BiosSetup", "Utilities", "Diags",
-                         "UefiShell", "UefiTarget", "SDCard", "UefiHttp", "RemoteDrive", "UefiBootNext" ]
+    ov_target_values = [
+        "None",
+        "Pxe",
+        "Floppy",
+        "Cd",
+        "Usb",
+        "Hdd",
+        "BiosSetup",
+        "Utilities",
+        "Diags",
+        "UefiShell",
+        "UefiTarget",
+        "SDCard",
+        "UefiHttp",
+        "RemoteDrive",
+        "UefiBootNext",
+    ]
     if ov_target is not None:
         if ov_target not in ov_target_values:
-            raise ValueError( "{} is not an allowable override target ({})".format( ov_target, ", ".join( ov_target_values ) ) )
-    ov_enabled_values = [ "Disabled", "Once", "Continuous" ]
+            raise ValueError(
+                "{} is not an allowable override target ({})".format(ov_target, ", ".join(ov_target_values))
+            )
+    ov_enabled_values = ["Disabled", "Once", "Continuous"]
     if ov_enabled is not None:
         if ov_enabled not in ov_enabled_values:
-            raise ValueError( "{} is not an allowable override enabled ({})".format( ov_enabled, ", ".join( ov_enabled_values ) ) )
-    ov_mode_values = [ "Legacy", "UEFI" ]
+            raise ValueError(
+                "{} is not an allowable override enabled ({})".format(ov_enabled, ", ".join(ov_enabled_values))
+            )
+    ov_mode_values = ["Legacy", "UEFI"]
     if ov_mode is not None:
         if ov_mode not in ov_mode_values:
-            raise ValueError( "{} is not an allowable override mode ({})".format( ov_mode, ", ".join( ov_mode_values ) ) )
+            raise ValueError("{} is not an allowable override mode ({})".format(ov_mode, ", ".join(ov_mode_values)))
 
     # Locate the system
-    system = get_system( context, system_id )
+    system = get_system(context, system_id)
 
     # Build the payload
-    payload = { "Boot": {} }
+    payload = {"Boot": {}}
     if ov_target is not None:
         payload["Boot"]["BootSourceOverrideTarget"] = ov_target
     if ov_enabled is not None:
         payload["Boot"]["BootSourceOverrideEnabled"] = ov_enabled
     if ov_mode is not None:
         payload["Boot"]["BootSourceOverrideMode"] = ov_mode
     if ov_uefi_target is not None:
         payload["Boot"]["UefiTargetBootSourceOverride"] = ov_uefi_target
     if ov_boot_next is not None:
         payload["Boot"]["BootNext"] = ov_boot_next
 
     # Update the system
     headers = None
-    etag = system.getheader( "ETag" )
+    etag = system.getheader("ETag")
     if etag is not None:
-        headers = { "If-Match": etag }
-    response = context.patch( system.dict["@odata.id"], body = payload, headers = headers )
+        headers = {"If-Match": etag}
+    response = context.patch(system.dict["@odata.id"], body=payload, headers=headers)
 
     # Attempt workarounds if needed
     if config.__workarounds__ and response.status >= 400:
         # Try directing the request to the settings resource
-        settings_uris = [ "Settings", "SD" ]
+        settings_uris = ["Settings", "SD"]
         for setting_ext in settings_uris:
-            system_settings = context.get( system.dict["@odata.id"] + "/" + setting_ext )
+            system_settings = context.get(system.dict["@odata.id"] + "/" + setting_ext)
             if system_settings.status == 200:
                 headers = None
-                etag = system_settings.getheader( "ETag" )
+                etag = system_settings.getheader("ETag")
                 if etag is not None:
-                    headers = { "If-Match": etag }
-                settings_response = context.patch( system.dict["@odata.id"] + "/" + setting_ext, body = payload, headers = headers )
+                    headers = {"If-Match": etag}
+                settings_response = context.patch(
+                    system.dict["@odata.id"] + "/" + setting_ext, body=payload, headers=headers
+                )
                 if settings_response.status < 400:
                     # Workaround successful; swap out the response object to return
-                    warnings.warn( "System '{}' incorrectly required applying the boot override configuration to the settings resource.  Contact your vendor.".format( system_id ) )
+                    warnings.warn(
+                        "System '{}' incorrectly required applying the boot override configuration to the settings resource.  Contact your vendor.".format(
+                            system_id
+                        )
+                    )
                     response = settings_response
                     break
 
-    verify_response( response )
+    verify_response(response)
     return response
 
-def print_system_boot( boot ):
+
+def print_system_boot(boot):
     """
     Prints the contents of a Boot object
 
     Args:
         boot: The Boot object to print
     """
 
-    print( "" )
+    print("")
 
-    print( "Boot Override Settings:" )
-    boot_properties = [ "BootSourceOverrideTarget", "BootSourceOverrideEnabled", "BootSourceOverrideMode", "UefiTargetBootSourceOverride", "BootNext" ]
-    boot_strings = [ "Target", "Enabled", "Mode", "UEFI Target", "Boot Next" ]
-    for index, boot_property in enumerate( boot_properties ):
+    print("Boot Override Settings:")
+    boot_properties = [
+        "BootSourceOverrideTarget",
+        "BootSourceOverrideEnabled",
+        "BootSourceOverrideMode",
+        "UefiTargetBootSourceOverride",
+        "BootNext",
+    ]
+    boot_strings = ["Target", "Enabled", "Mode", "UEFI Target", "Boot Next"]
+    for index, boot_property in enumerate(boot_properties):
         if boot_property in boot:
-            out_string = "  {}: {}".format( boot_strings[index], boot[boot_property] )
+            out_string = "  {}: {}".format(boot_strings[index], boot[boot_property])
             allow_string = ""
             if boot_property + "@Redfish.AllowableValues" in boot:
-                allow_string = "; Allowable Values: {}".format( ", ".join( boot[boot_property + "@Redfish.AllowableValues"] ) )
-            print( out_string + allow_string )
+                allow_string = "; Allowable Values: {}".format(
+                    ", ".join(boot[boot_property + "@Redfish.AllowableValues"])
+                )
+            print(out_string + allow_string)
 
-    print( "" )
+    print("")
 
-def get_system_reset_info( context, system_id = None, system = None ):
+
+def get_system_reset_info(context, system_id=None, system=None):
     """
     Finds a system matching the given ID and returns its reset info
 
     Args:
         context: The Redfish client object with an open session
         system_id: The system to locate; if None, perform on the only system
         system: Existing system resource to inspect for reset info
 
     Returns:
         The URI of the Reset action
         A list of parameter requirements from the Action Info
     """
 
     if system is None:
-        system = get_system( context, system_id )
+        system = get_system(context, system_id)
 
     # Check that there is a Reset action
     if "Actions" not in system.dict:
-        raise RedfishSystemResetNotFoundError( "System '{}' does not support the reset action".format( system.dict["Id"] ) )
+        raise RedfishSystemResetNotFoundError("System '{}' does not support the reset action".format(system.dict["Id"]))
     if "#ComputerSystem.Reset" not in system.dict["Actions"]:
-        raise RedfishSystemResetNotFoundError( "System '{}' does not support the reset action".format( system.dict["Id"] ) )
+        raise RedfishSystemResetNotFoundError("System '{}' does not support the reset action".format(system.dict["Id"]))
 
     # Extract the info about the Reset action
     reset_action = system.dict["Actions"]["#ComputerSystem.Reset"]
     reset_uri = reset_action["target"]
 
     if "@Redfish.ActionInfo" not in reset_action:
         # No action info; need to build this manually based on other annotations
 
         # Default parameter requirements
         reset_parameters = [
-            {
-                "Name": "ResetType",
-                "Required": False,
-                "DataType": "String",
-                "AllowableValues": reset_types
-            }
+            {"Name": "ResetType", "Required": False, "DataType": "String", "AllowableValues": reset_types}
         ]
 
         # Get the AllowableValues from annotations
         for param in reset_parameters:
             if param["Name"] + "@Redfish.AllowableValues" in reset_action:
                 param["AllowableValues"] = reset_action[param["Name"] + "@Redfish.AllowableValues"]
     else:
         # Get the action info and its parameter listing
-        action_info = context.get( reset_action["@Redfish.ActionInfo"] )
+        action_info = context.get(reset_action["@Redfish.ActionInfo"])
         reset_parameters = action_info.dict["Parameters"]
 
     return reset_uri, reset_parameters
 
-def system_reset( context, system_id = None, reset_type = None ):
+
+def system_reset(context, system_id=None, reset_type=None):
     """
     Finds a system matching the given ID and performs a reset
 
     Args:
         context: The Redfish client object with an open session
         system_id: The system to locate; if None, perform on the only system
         reset_type: The type of reset to perform; if None, perform one of the common resets
@@ -322,18 +396,18 @@
         The response of the action
     """
 
     # Check that the values themselves are supported by the schema
     reset_type_values = reset_types
     if reset_type is not None:
         if reset_type not in reset_type_values:
-            raise ValueError( "{} is not an allowable reset type ({})".format( reset_type, ", ".join( reset_type_values ) ) )
+            raise ValueError("{} is not an allowable reset type ({})".format(reset_type, ", ".join(reset_type_values)))
 
     # Locate the reset action
-    reset_uri, reset_parameters = get_system_reset_info( context, system_id )
+    reset_uri, reset_parameters = get_system_reset_info(context, system_id)
 
     # Build the payload
     if reset_type is None:
         for param in reset_parameters:
             if param["Name"] == "ResetType":
                 if "GracefulRestart" in param["AllowableValues"]:
                     reset_type = "GracefulRestart"
@@ -343,72 +417,77 @@
                     reset_type = "PowerCycle"
 
     payload = {}
     if reset_type is not None:
         payload["ResetType"] = reset_type
 
     # Reset the system
-    response = context.post( reset_uri, body = payload )
+    response = context.post(reset_uri, body=payload)
     try:
-        verify_response( response )
+        verify_response(response)
     except Exception as e:
         additional_message = ""
         if response.status == 400:
             # Append the list of valid reset types to 400 Bad Request responses
             additional_message = "\nNo supported reset types listed"
             for param in reset_parameters:
                 if param["Name"] == "ResetType" and "AllowableValues" in param:
-                    additional_message = "\nSupported reset types: {}".format( ", ".join( param["AllowableValues"] ) )
-        raise type( e )( str( e ) + additional_message ).with_traceback( sys.exc_info()[2] )
+                    additional_message = "\nSupported reset types: {}".format(", ".join(param["AllowableValues"]))
+        raise type(e)(str(e) + additional_message).with_traceback(sys.exc_info()[2])
     return response
 
-def get_virtual_media( context, system_id = None ):
+
+def get_virtual_media(context, system_id=None):
     """
     Finds the system matching the given ID and gets its virtual media
 
     Args:
         context: The Redfish client object with an open session
         system_id: The system to locate; if None, perform on the only system
 
     Returns:
         An array of dictionaries of the virtual media instances
     """
 
     # Get the virtual media collection
-    virtual_media_collection = get_virtual_media_collection( context, system_id = system_id )
+    virtual_media_collection = get_virtual_media_collection(context, system_id=system_id)
 
     # Iterate through the members and pull out each of the instances
     virtual_media_list = []
     for member in virtual_media_collection.dict["Members"]:
-        virtual_media = context.get( member["@odata.id"] )
-        virtual_media_list.append( virtual_media.dict )
+        virtual_media = context.get(member["@odata.id"])
+        virtual_media_list.append(virtual_media.dict)
     return virtual_media_list
 
-def print_virtual_media( virtual_media_list ):
+
+def print_virtual_media(virtual_media_list):
     """
     Prints the virtual media list into a table
 
     Args:
         virtual_media_list: The virtual media list to print
     """
 
     virtual_media_line_format = "  {:20s} | {}: {}"
-    virtual_media_properties = [ "Image", "MediaTypes", "ConnectedVia", "Inserted", "WriteProtected" ]
-    print( "" )
+    virtual_media_properties = ["Image", "MediaTypes", "ConnectedVia", "Inserted", "WriteProtected"]
+    print("")
     for virtual_media in virtual_media_list:
-        print( virtual_media_line_format.format( virtual_media["Id"], "ImageName", virtual_media.get( "ImageName", "" ) ) )
+        print(virtual_media_line_format.format(virtual_media["Id"], "ImageName", virtual_media.get("ImageName", "")))
         for property in virtual_media_properties:
             if property in virtual_media:
                 prop_val = virtual_media[property]
-                if isinstance( prop_val, list ):
-                    prop_val = ", ".join( prop_val )
-                print( virtual_media_line_format.format( "", property, prop_val ) )
-        print( "" )
+                if isinstance(prop_val, list):
+                    prop_val = ", ".join(prop_val)
+                print(virtual_media_line_format.format("", property, prop_val))
+        print("")
 
-def insert_virtual_media( context, image, system_id = None, media_id = None, media_types = None, inserted = None, write_protected = None ):
+
+def insert_virtual_media(
+    context, image, system_id=None, media_id=None, media_types=None, inserted=None, write_protected=None
+):
     """
     Finds the system matching the given ID and inserts virtual media
 
     Args:
         context: The Redfish client object with an open session
         image: The URI of the media to insert
         system_id: The system to locate; if None, perform on the only system
@@ -419,28 +498,28 @@
 
     Returns:
         The response of the insert operation
     """
 
     # Set up acceptable media types based on the image URI if not specified
     if media_types is None:
-        if image.lower().endswith( ".iso" ):
-            media_types = [ "CD", "DVD" ]
-        elif image.lower().endswith( ".img" ):
-            media_types = [ "USBStick" ]
-        elif image.lower().endswith( ".bin" ):
-            media_types = [ "USBStick" ]
+        if image.lower().endswith(".iso"):
+            media_types = ["CD", "DVD"]
+        elif image.lower().endswith(".img"):
+            media_types = ["USBStick"]
+        elif image.lower().endswith(".bin"):
+            media_types = ["USBStick"]
 
     # Get the virtual media collection
-    virtual_media_collection = get_virtual_media_collection( context, system_id = system_id )
+    virtual_media_collection = get_virtual_media_collection(context, system_id=system_id)
 
     # Scan the virtual media for an appropriate slot
     match = False
     for member in virtual_media_collection.dict["Members"]:
-        media = context.get( member["@odata.id"] )
+        media = context.get(member["@odata.id"])
         if media.dict["Image"] is not None:
             # In use; move on
             continue
 
         # Check for a match
         if media_id is not None:
             if media.dict["Id"] == media_id:
@@ -455,238 +534,257 @@
                 for type in media_types:
                     if type in media.dict["MediaTypes"]:
                         # Acceptable media type found
                         match = True
 
         # If a match was found, attempt to insert the media
         if match:
-            payload = {
-                "Image": image
-            }
+            payload = {"Image": image}
             if inserted:
                 payload["Inserted"] = inserted
             if write_protected:
                 payload["WriteProtected"] = write_protected
             try:
                 # Preference for using the InsertMedia action
-                response = context.post( media.dict["Actions"]["#VirtualMedia.InsertMedia"]["target"], body = payload )
-            except:
+                response = context.post(media.dict["Actions"]["#VirtualMedia.InsertMedia"]["target"], body=payload)
+            except Exception:
                 # Fallback to PATCH method
                 if "Inserted" not in payload:
                     payload["Inserted"] = True
                 headers = None
-                etag = media.getheader( "ETag" )
+                etag = media.getheader("ETag")
                 if etag is not None:
-                    headers = { "If-Match": etag }
-                response = context.patch( media.dict["@odata.id"], body = payload, headers = headers )
-            verify_response( response )
+                    headers = {"If-Match": etag}
+                response = context.patch(media.dict["@odata.id"], body=payload, headers=headers)
+            verify_response(response)
             return response
 
     # No matches found
     if media_id is not None:
-        reason = "'{}' not found or is already in use".format( media_id )
+        reason = "'{}' not found or is already in use".format(media_id)
     elif media_types is not None:
-        reason = "No available slots of types {}".format( ", ".join( media_types ) )
+        reason = "No available slots of types {}".format(", ".join(media_types))
     else:
         reason = "No available slots"
-    raise RedfishNoAcceptableVirtualMediaError( "No acceptable virtual media: {}".format( reason ) )
+    raise RedfishNoAcceptableVirtualMediaError("No acceptable virtual media: {}".format(reason))
+
 
-def eject_virtual_media( context, media_id, system_id = None ):
+def eject_virtual_media(context, media_id, system_id=None):
     """
     Finds the system matching the given ID and ejects virtual media
 
     Args:
         context: The Redfish client object with an open session
         media_id: The virtual media instance to eject
         system_id: The system to locate; if None, perform on the only system
 
     Returns:
         The response of the eject operation
     """
 
     # Get the virtual media collection
-    virtual_media_collection = get_virtual_media_collection( context, system_id = system_id )
+    virtual_media_collection = get_virtual_media_collection(context, system_id=system_id)
 
     # Scan the virtual media for the selected slot
     for member in virtual_media_collection.dict["Members"]:
-        media = context.get( member["@odata.id"] )
+        media = context.get(member["@odata.id"])
         if media.dict["Id"] == media_id:
             # Found the selected slot; eject it
             try:
                 # Preference for using the EjectMedia action
-                response = context.post( media.dict["Actions"]["#VirtualMedia.EjectMedia"]["target"], body = {} )
-            except:
+                response = context.post(media.dict["Actions"]["#VirtualMedia.EjectMedia"]["target"], body={})
+            except Exception:
                 # Fallback to PATCH method
-                payload = {
-                    "Image": None,
-                    "Inserted": False
-                }
+                payload = {"Image": None, "Inserted": False}
                 headers = None
-                etag = media.getheader( "ETag" )
+                etag = media.getheader("ETag")
                 if etag is not None:
-                    headers = { "If-Match": etag }
-                response = context.patch( media.dict["@odata.id"], body = payload, headers = headers )
-            verify_response( response )
+                    headers = {"If-Match": etag}
+                response = context.patch(media.dict["@odata.id"], body=payload, headers=headers)
+            verify_response(response)
             return response
 
     # No matches found
-    raise RedfishNoAcceptableVirtualMediaError( "No acceptable virtual media: '{}' not found".format( media_id ) )
+    raise RedfishNoAcceptableVirtualMediaError("No acceptable virtual media: '{}' not found".format(media_id))
 
-def get_virtual_media_collection( context, system_id = None ):
+
+def get_virtual_media_collection(context, system_id=None):
     """
     Finds the system matching the given ID and gets its virtual media collection
 
     Args:
         context: The Redfish client object with an open session
         system_id: The system to locate; if None, perform on the only system
 
     Returns:
         The virtual media collection
     """
 
     # Locate the system
-    system = get_system( context, system_id )
+    system = get_system(context, system_id)
 
     # Check if there is a VirtualMediaCollection; if not, try the older location in the Manager resource
     virtual_media_uri = None
     if "VirtualMedia" in system.dict:
         virtual_media_uri = system.dict["VirtualMedia"]["@odata.id"]
     else:
         if "Links" in system.dict:
             if "ManagedBy" in system.dict["Links"]:
                 for manager in system.dict["Links"]["ManagedBy"]:
-                    manager_resp = context.get( manager["@odata.id"] )
+                    manager_resp = context.get(manager["@odata.id"])
                     if "VirtualMedia" in manager_resp.dict:
                         # Get the first manager that contains virtual media
                         virtual_media_uri = manager_resp.dict["VirtualMedia"]["@odata.id"]
                         break
     if virtual_media_uri is None:
-        raise RedfishVirtualMediaNotFoundError( "System '{}' does not support virtual media".format( system.dict["Id"] ) )
+        raise RedfishVirtualMediaNotFoundError("System '{}' does not support virtual media".format(system.dict["Id"]))
 
     # Get the VirtualMediaCollection
-    return context.get( virtual_media_uri )
+    return context.get(virtual_media_uri)
+
 
-def get_system_bios( context, system_id = None ):
+def get_system_bios(context, system_id=None):
     """
     Finds a system matching the given ID and gets the BIOS settings
 
     Args:
         context: The Redfish client object with an open session
         system_id: The system to locate; if None, perform on the only system
 
     Returns:
         A dictionary of the current BIOS attributes
         A dictionary of the BIOS attributes on the next reset
     """
 
     # Locate the system
-    system = get_system( context, system_id )
+    system = get_system(context, system_id)
 
     # Get the Bios resource
     if "Bios" not in system.dict:
-        raise RedfishSystemBiosNotFoundError( "System '{}' does not support representing BIOS".format( system.dict["Id"] ) )
-    bios = context.get( system.dict["Bios"]["@odata.id"] )
+        raise RedfishSystemBiosNotFoundError("System '{}' does not support representing BIOS".format(system.dict["Id"]))
+    bios = context.get(system.dict["Bios"]["@odata.id"])
     current_settings = bios.dict["Attributes"]
     future_settings = bios.dict["Attributes"]
 
     # Get the Settings object if present
     if "@Redfish.Settings" in bios.dict:
         try:
-            bios_settings = get_system_bios_settings( context, bios, system.dict["Id"] )
+            bios_settings = get_system_bios_settings(context, bios, system.dict["Id"])
             future_settings = bios_settings.dict["Attributes"]
-        except:
+        except Exception:
             if config.__workarounds__:
-                warnings.warn( "System '{}' BIOS resource contains the settings term, but no 'SettingsObject'.  Contact your vendor.  Workarounds exhausted for reading the settings data and falling back on using the active attributes.".format( system_id ) )
+                warnings.warn(
+                    "System '{}' BIOS resource contains the settings term, but no 'SettingsObject'.  Contact your vendor.  Workarounds exhausted for reading the settings data and falling back on using the active attributes.".format(
+                        system_id
+                    )
+                )
             else:
                 raise
 
     return current_settings, future_settings
 
-def set_system_bios( context, settings, system_id = None ):
+
+def set_system_bios(context, settings, system_id=None):
     """
     Finds a system matching the given ID and sets the BIOS settings
 
     Args:
         context: The Redfish client object with an open session
         settings: The settings to apply to the system
         system_id: The system to locate; if None, perform on the only system
 
     Returns:
         The response of the PATCH
     """
 
     # Locate the system
-    system = get_system( context, system_id )
+    system = get_system(context, system_id)
 
     # Get the BIOS resource and determine if the settings need to be applied to the resource itself or the settings object
     if "Bios" not in system.dict:
-        raise RedfishSystemBiosNotFoundError( "System '{}' does not support representing BIOS".format( system.dict["Id"] ) )
+        raise RedfishSystemBiosNotFoundError("System '{}' does not support representing BIOS".format(system.dict["Id"]))
     bios_uri = system.dict["Bios"]["@odata.id"]
-    bios = context.get( bios_uri )
-    etag = bios.getheader( "ETag" )
+    bios = context.get(bios_uri)
+    etag = bios.getheader("ETag")
     if "@Redfish.Settings" in bios.dict:
-        bios_settings = get_system_bios_settings( context, bios, system.dict["Id"] )
+        bios_settings = get_system_bios_settings(context, bios, system.dict["Id"])
         bios_uri = bios_settings.dict["@odata.id"]
-        etag = bios_settings.getheader( "ETag" )
+        etag = bios_settings.getheader("ETag")
 
     # Update the settings
-    payload = { "Attributes": settings }
+    payload = {"Attributes": settings}
     headers = None
     if etag is not None:
-        headers = { "If-Match": etag }
-    response = context.patch( bios_uri, body = payload, headers = headers )
-    verify_response( response )
+        headers = {"If-Match": etag}
+    response = context.patch(bios_uri, body=payload, headers=headers)
+    verify_response(response)
     return response
 
-def get_system_bios_settings( context, bios, system_id ):
+
+def get_system_bios_settings(context, bios, system_id):
     """
     Gets the settings resource for BIOS
 
     Args:
         context: The Redfish client object with an open session
         bios: The BIOS resource
         system_id: The system identifier
 
     Returns:
         The Settings resource for BIOS
     """
 
     if "SettingsObject" in bios.dict["@Redfish.Settings"]:
-        bios_settings = context.get( bios.dict["@Redfish.Settings"]["SettingsObject"]["@odata.id"] )
+        bios_settings = context.get(bios.dict["@Redfish.Settings"]["SettingsObject"]["@odata.id"])
     else:
         if config.__workarounds__:
-            warnings.warn( "System '{}' BIOS resource contains the settings term, but no 'SettingsObject'.  Contact your vendor.  Attempting workarounds...".format( system_id ) )
-            settings_uris = [ "Settings", "SD" ]
+            warnings.warn(
+                "System '{}' BIOS resource contains the settings term, but no 'SettingsObject'.  Contact your vendor.  Attempting workarounds...".format(
+                    system_id
+                )
+            )
+            settings_uris = ["Settings", "SD"]
             for setting_ext in settings_uris:
-                bios_settings = context.get( bios.dict["@odata.id"] + "/" + setting_ext )
+                bios_settings = context.get(bios.dict["@odata.id"] + "/" + setting_ext)
                 if bios_settings.status == 200:
                     break
             try:
-                verify_response( bios_settings )
-            except:
-                raise RedfishSystemBiosInvalidSettingsError( "System '{}' BIOS resource contains the settings term, but no 'SettingsObject'.  Workarounds exhausted.  Contact your vendor.".format( system_id ) ) from None
+                verify_response(bios_settings)
+            except Exception:
+                raise RedfishSystemBiosInvalidSettingsError(
+                    "System '{}' BIOS resource contains the settings term, but no 'SettingsObject'.  Workarounds exhausted.  Contact your vendor.".format(
+                        system_id
+                    )
+                ) from None
         else:
-            raise RedfishSystemBiosInvalidSettingsError( "System '{}' BIOS resource contains the settings term, but no 'SettingsObject'.  Contact your vendor, or retry with the '__workarounds__' flag.".format( system_id ) )
+            raise RedfishSystemBiosInvalidSettingsError(
+                "System '{}' BIOS resource contains the settings term, but no 'SettingsObject'.  Contact your vendor, or retry with the '__workarounds__' flag.".format(
+                    system_id
+                )
+            )
 
     return bios_settings
 
-def print_system_bios( current_settings, future_settings ):
+
+def print_system_bios(current_settings, future_settings):
     """
     Prints the system BIOS settings into a table
 
     Args:
         current_settings: A dictionary of the current BIOS attributes
         future_settings: A dictionary of the BIOS attributes on the next reset
     """
 
-    print( "" )
-    print( "BIOS Settings:" )
+    print("")
+    print("BIOS Settings:")
 
     bios_line_format = "  {:30s} | {:30s} | {:30s}"
-    print( bios_line_format.format( "Attribute Name", "Current Setting", "Future Setting" ) )
-    for attribute, value in sorted( current_settings.items() ):
+    print(bios_line_format.format("Attribute Name", "Current Setting", "Future Setting"))
+    for attribute, value in sorted(current_settings.items()):
         if attribute in future_settings:
-            print( bios_line_format.format( attribute, str( current_settings[attribute] ), str( future_settings[attribute] ) ) )
+            print(bios_line_format.format(attribute, str(current_settings[attribute]), str(future_settings[attribute])))
         else:
-            print( bios_line_format.format( attribute, str( current_settings[attribute] ), str( current_settings[attribute] ) ) )
+            print(
+                bios_line_format.format(attribute, str(current_settings[attribute]), str(current_settings[attribute]))
+            )
 
-    print( "" )
+    print("")
```

### Comparing `redfish_utilities-3.2.8/redfish_utilities/tasks.py` & `redfish_utilities-3.2.9/redfish_utilities/tasks.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 Brief : This file contains the definitions and functionalities for interacting
         with Tasks for a given Redfish service
 """
 
 import sys
 import time
 
-def poll_task_monitor( context, response ):
+
+def poll_task_monitor(context, response):
     """
     Monitors a task monitor until it's complete and prints out progress
     NOTE: This call will block until the task is complete
 
     Args:
         context: The Redfish client object with an open session
         response: The initial response from the operation that produced the task
@@ -35,34 +36,34 @@
     # Poll the task until completion
     task_monitor = response
     while task_monitor.is_processing:
         # Print the progress
         task_state = None
         task_percent = None
         try:
-            task_state = task_monitor.dict.get( "TaskState", None )
-            task_percent = task_monitor.dict.get( "PercentComplete", None )
-        except:
+            task_state = task_monitor.dict.get("TaskState", None)
+            task_percent = task_monitor.dict.get("PercentComplete", None)
+        except Exception:
             # 202 responses are allowed to not have a response body
             pass
         if task_state is None:
             task_state = "Running"
         if task_percent is None:
-            progress_str = "Task is {}\r".format( task_state )
+            progress_str = "Task is {}\r".format(task_state)
         else:
-            progress_str = "Task is {}: {}% complete\r".format( task_state, task_percent )
-        sys.stdout.write( "\x1b[2K" )
-        sys.stdout.write( progress_str )
+            progress_str = "Task is {}: {}% complete\r".format(task_state, task_percent)
+        sys.stdout.write("\x1b[2K")
+        sys.stdout.write(progress_str)
         sys.stdout.flush()
 
         # Sleep for the requested time
         retry_time = response.retry_after
         if retry_time is None:
             retry_time = 1
-        time.sleep( retry_time )
+        time.sleep(retry_time)
 
         # Check the monitor for an update
-        task_monitor = response.monitor( context )
-    sys.stdout.write( "\x1b[2K" )
-    print( "Task is Done!" )
+        task_monitor = response.monitor(context)
+    sys.stdout.write("\x1b[2K")
+    print("Task is Done!")
 
     return task_monitor
```

### Comparing `redfish_utilities-3.2.8/redfish_utilities/update.py` & `redfish_utilities-3.2.9/redfish_utilities/update.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,107 +11,96 @@
 Brief : This file contains the definitions and functionalities for interacting
         with the UpdateService for a given Redfish service
 """
 
 import json
 import os
 import errno
-import math
 from .messages import verify_response
 from enum import Enum
 
-class RedfishUpdateServiceNotFoundError( Exception ):
+
+class RedfishUpdateServiceNotFoundError(Exception):
     """
     Raised when the update service or an update action cannot be found
     """
+
     pass
 
-class operation_apply_times( Enum ):
+
+class operation_apply_times(Enum):
     """
     Values for operation apply time settings
     """
+
     IMMEDIATE = "Immediate"
     ON_RESET = "OnReset"
     AT_MAINTENANCE_WINDOW_START = "AtMaintenanceWindowStart"
     AT_MAINTENANCE_WINDOW_ON_RESET = "InMaintenanceWindowOnReset"
     ON_START_UPDATE_REQUEST = "OnStartUpdateRequest"
 
-    def __str__( self ):
+    def __str__(self):
         return self.value
 
-def get_simple_update_info( context ):
+
+def get_simple_update_info(context):
     """
     Locates the SimpleUpdate action and collects its information
 
     Args:
         context: The Redfish client object with an open session
 
     Returns:
         The URI of the SimpleUpdate action
         A list of parameter requirements from the action info
     """
 
     # Get the update service
-    update_service = get_update_service( context )
+    update_service = get_update_service(context)
 
     # Check that there is a SimpleUpdate action
     if "Actions" not in update_service.dict:
-        raise RedfishUpdateServiceNotFoundError( "Service does not support SimpleUpdate" )
+        raise RedfishUpdateServiceNotFoundError("Service does not support SimpleUpdate")
     if "#UpdateService.SimpleUpdate" not in update_service.dict["Actions"]:
-        raise RedfishUpdateServiceNotFoundError( "Service does not support SimpleUpdate" )
+        raise RedfishUpdateServiceNotFoundError("Service does not support SimpleUpdate")
 
     # Extract the info about the SimpleUpdate action
     simple_update_action = update_service.dict["Actions"]["#UpdateService.SimpleUpdate"]
     simple_update_uri = simple_update_action["target"]
 
     if "@Redfish.ActionInfo" not in simple_update_action:
         # No action info; need to build this manually based on other annotations
 
         # Default parameter requirements
         simple_update_parameters = [
-            {
-                "Name": "ImageURI",
-                "Required": True,
-                "DataType": "String"
-            },
+            {"Name": "ImageURI", "Required": True, "DataType": "String"},
             {
                 "Name": "TransferProtocol",
                 "Required": False,
                 "DataType": "String",
-                "AllowableValues": [ "CIFS", "FTP", "SFTP", "HTTP", "HTTPS", "NSF", "SCP", "TFTP", "OEM", "NFS" ]
-            },
-            {
-                "Name": "Targets",
-                "Required": False,
-                "DateType": "StringArray"
+                "AllowableValues": ["CIFS", "FTP", "SFTP", "HTTP", "HTTPS", "NSF", "SCP", "TFTP", "OEM", "NFS"],
             },
-            {
-                "Name": "Username",
-                "Required": False,
-                "DataType": "String"
-            },
-            {
-                "Name": "Password",
-                "Required": False,
-                "DataType": "String"
-            }
+            {"Name": "Targets", "Required": False, "DateType": "StringArray"},
+            {"Name": "Username", "Required": False, "DataType": "String"},
+            {"Name": "Password", "Required": False, "DataType": "String"},
         ]
 
         # Get the allowable values from annotations
         for param in simple_update_parameters:
             if param["Name"] + "@Redfish.AllowableValues" in simple_update_action:
                 param["AllowableValues"] = simple_update_action[param["Name"] + "@Redfish.AllowableValues"]
     else:
         # Get the action info and its parameter listing
-        action_info = context.get( simple_update_action["@Redfish.ActionInfo"] )
+        action_info = context.get(simple_update_action["@Redfish.ActionInfo"])
         simple_update_parameters = action_info.dict["Parameters"]
 
     return simple_update_uri, simple_update_parameters
 
-def simple_update( context, image_uri, protocol = None, targets = None, username = None, password = None, apply_time = None ):
+
+def simple_update(context, image_uri, protocol=None, targets=None, username=None, password=None, apply_time=None):
     """
     Performs a SimpleUpdate request
 
     Args:
         context: The Redfish client object with an open session
         image_uri: The image URI for the update
         protocol: The transfer protocol for the update
@@ -121,56 +110,56 @@
         apply_time: The apply time for the update
 
     Returns:
         The response from the request
     """
 
     # Get the SimpleUpdate info
-    uri, params = get_simple_update_info( context )
+    uri, params = get_simple_update_info(context)
 
     # Build the request body
-    body = {
-        "ImageURI": image_uri
-    }
+    body = {"ImageURI": image_uri}
     if protocol is not None:
         body["TransferProtocol"] = protocol
     if targets is not None:
         body["Targets"] = targets
     if username is not None:
         body["Username"] = username
     if password is not None:
         body["Password"] = password
     if apply_time is not None:
         body["@Redfish.OperationApplyTime"] = apply_time.value
 
-    response = context.post( uri, body = body )
-    verify_response( response )
+    response = context.post(uri, body=body)
+    verify_response(response)
     return response
 
-def get_size( file_path, unit = 'bytes' ):
+
+def get_size(file_path, unit="bytes"):
     """
     Determines the size of a local file
 
     Args:
         file_path: The path to the file
         unit: The units to apply to the return value
 
     Returns:
         The size of the file in the specified units
     """
 
-    file_size = os.path.getsize( file_path )
-    exponents_map = { 'bytes': 0, 'kb': 1, 'mb': 2, 'gb': 3 }
+    file_size = os.path.getsize(file_path)
+    exponents_map = {"bytes": 0, "kb": 1, "mb": 2, "gb": 3}
     if unit not in exponents_map:
-        raise ValueError( "Must select from ['bytes', 'kb', 'mb', 'gb']" )
+        raise ValueError("Must select from ['bytes', 'kb', 'mb', 'gb']")
     else:
         size = file_size / 1024 ** exponents_map[unit]
-        return round( size, 3 )
-    
-def multipart_push_update( context, image_path, targets = None, timeout = None, apply_time = None ):
+        return round(size, 3)
+
+
+def multipart_push_update(context, image_path, targets=None, timeout=None, apply_time=None):
     """
     Performs an HTTP Multipart push update request
 
     Args:
         context: The Redfish client object with an open session
         image_path: The filepath to the image for the update
         targets: The targets receiving the update
@@ -178,63 +167,70 @@
         apply_time: The apply time for the update
 
     Returns:
         The response from the request
     """
 
     # Ensure the file exists
-    if os.path.isfile( image_path ) is False:
-        raise FileNotFoundError( errno.ENOENT, os.strerror( errno.ENOENT ), image_path )
+    if os.path.isfile(image_path) is False:
+        raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), image_path)
 
     # If no update is specified, determine an appropriate timeout to apply
     if timeout is None:
         """TODO: See what a 'reasonable' timeout is when accounting for slow networks
         for now, keeping the timeout conservative (2 seconds per MB)
         timeout = 5
         file_size = get_size( image_path, "mb" )
 
         if file_size >= 16:
             timeout = math.ceil( ( 5 / 16 ) * file_size )
         """
         timeout = 30
-        file_size = get_size( image_path, "mb" )
+        file_size = get_size(image_path, "mb")
         if file_size >= 15:
             timeout = 2 * file_size
 
     # Get the update service
-    update_service = get_update_service( context )
+    update_service = get_update_service(context)
     if "MultipartHttpPushUri" not in update_service.dict:
-        raise RedfishUpdateServiceNotFoundError( "Service does not support MultipartHttpPushUri" )
+        raise RedfishUpdateServiceNotFoundError("Service does not support MultipartHttpPushUri")
 
     # Build the request body
     update_parameters = {}
     if targets is not None:
         update_parameters["Targets"] = targets
     if apply_time is not None:
         update_parameters["@Redfish.OperationApplyTime"] = apply_time.value
     body = {
-        "UpdateParameters": ( None, json.dumps( update_parameters ), "application/json" ),
-        "UpdateFile": ( image_path.split( os.path.sep )[-1], open( image_path, "rb" ), "application/octet-stream" )
+        "UpdateParameters": (None, json.dumps(update_parameters), "application/json"),
+        "UpdateFile": (image_path.split(os.path.sep)[-1], open(image_path, "rb"), "application/octet-stream"),
     }
 
-    response = context.post( update_service.dict["MultipartHttpPushUri"], body = body, headers = { "Content-Type": "multipart/form-data" }, timeout = timeout, max_retry = 3 )
-    verify_response( response )
+    response = context.post(
+        update_service.dict["MultipartHttpPushUri"],
+        body=body,
+        headers={"Content-Type": "multipart/form-data"},
+        timeout=timeout,
+        max_retry=3,
+    )
+    verify_response(response)
     return response
 
-def get_update_service( context ):
+
+def get_update_service(context):
     """
     Locates and gets the UpdateService resource
 
     Args:
         context: The Redfish client object with an open session
 
     Returns:
         The UpdateService resource
     """
 
     # Get the Service Root to find the Update Service
-    service_root = context.get( "/redfish/v1/" )
+    service_root = context.get("/redfish/v1/")
     if "UpdateService" not in service_root.dict:
         # No Update Service
-        raise RedfishUpdateServiceNotFoundError( "Service does not have an UpdateService" )
+        raise RedfishUpdateServiceNotFoundError("Service does not have an UpdateService")
 
-    return context.get( service_root.dict["UpdateService"]["@odata.id"] )
+    return context.get(service_root.dict["UpdateService"]["@odata.id"])
```

### Comparing `redfish_utilities-3.2.8/redfish_utilities.egg-info/PKG-INFO` & `redfish_utilities-3.2.9/redfish_utilities.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish_utilities
-Version: 3.2.8
+Version: 3.2.9
 Summary: Redfish Utilities
 Home-page: https://github.com/DMTF/Redfish-Tacklebox
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
@@ -17,14 +17,23 @@
 Requires-Dist: XlsxWriter>=1.2.7
 Requires-Dist: requests
 
 # Redfish Tacklebox
 
 Copyright 2019-2024 DMTF.  All rights reserved.
 
+[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md)
+[![PyPI](https://img.shields.io/pypi/v/redfish-utilities)](https://pypi.org/project/redfish-utilities/)
+[![Pulls](https://img.shields.io/docker/pulls/dmtf/redfish-tacklebox?style=flat&logo=docker&label=Pulls)](https://hub.docker.com/r/dmtf/redfish-tacklebox)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat)](https://github.com/psf/black)
+[![Linters](https://github.com/DMTF/Redfish-Tacklebox/actions/workflows/linters.yml/badge.svg)](https://github.com/DMTF/Redfish-Tacklebox/actions/workflows/linters.yml)
+[![Docker](https://github.com/DMTF/Redfish-Tacklebox/actions/workflows/docker.yml/badge.svg)](https://github.com/DMTF/Redfish-Tacklebox/actions/workflows/docker.yml)
+[![GitHub stars](https://img.shields.io/github/stars/DMTF/Redfish-Tacklebox.svg?style=flat-square&label=github%20stars)](https://github.com/DMTF/Redfish-Tacklebox)
+[![GitHub Contributors](https://img.shields.io/github/contributors/DMTF/Redfish-Tacklebox.svg?style=flat-square)](https://github.com/DMTF/Redfish-Tacklebox/graphs/contributors)
+
 ## About
 
 Redfish Tacklebox contains a set of Python3 utilities to perform common management operations with a Redfish service.
 The utilities can be used as part of larger management applications, or be used as standalone command line tools.
 
 ## Installation
 
@@ -38,25 +47,25 @@
 ```
 
 ### Building Docker
 
 * Pull the container from Docker Hub:
 
     ```bash
-    docker pull dmtf/redfish-utilities:latest
+    docker pull dmtf/redfish-tacklebox:latest
     ```
 * Build a container from local source:
 
     ```bash
-    docker build -t dmtf/redfish-utilities:latest .
+    docker build -t dmtf/redfish-tacklebox:latest .
     ```
 * Build a container from GitHub:
 
     ```bash
-    docker build -t dmtf/redfish-utilities:latest https://github.com/DMTF/Redfish-Tacklebox.git
+    docker build -t dmtf/redfish-tacklebox:latest https://github.com/DMTF/Redfish-Tacklebox.git
     ```
 
 ## Requirements
 
 External modules:
 * redfish: https://pypi.python.org/pypi/redfish
 * XlsxWriter: https://pypi.org/project/XlsxWriter
```

### Comparing `redfish_utilities-3.2.8/redfish_utilities.egg-info/SOURCES.txt` & `redfish_utilities-3.2.9/redfish_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redfish_utilities-3.2.8/scripts/rf_accounts.py` & `redfish_utilities-3.2.9/scripts/rf_accounts.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,109 +17,133 @@
 import redfish
 import redfish_utilities
 import traceback
 import sys
 from redfish.messages import RedfishPasswordChangeRequiredError
 
 # Get the input arguments
-argget = argparse.ArgumentParser( description = "A tool to manage user accounts on a Redfish service" )
-argget.add_argument( "--user", "-u", type = str, required = True, help = "The user name for authentication" )
-argget.add_argument( "--password", "-p",  type = str, required = True, help = "The password for authentication" )
-argget.add_argument( "--rhost", "-r", type = str, required = True, help = "The address of the Redfish service (with scheme)" )
-argget.add_argument( "--add", "-add", type = str, nargs = 3, metavar = ( "name", "password", "role" ), help = "Adds a new user account" )
-argget.add_argument( "--delete", "-delete", type = str, help = "Deletes a user account with the given name" )
-argget.add_argument( "--setname", "-setname", type = str, nargs = 2, metavar = ( "old_name", "new_name" ) , help = "Sets a user account to a new name" )
-argget.add_argument( "--setpassword", "-setpassword", type = str, nargs = 2, metavar = ( "name", "new_password" ), help = "Sets a user account to a new password" )
-argget.add_argument( "--setrole", "-setrole", type = str, nargs = 2, metavar = ( "name", "new_role" ), help = "Sets a user account to a new role" )
-argget.add_argument( "--enable", "-enable", type = str, help = "Enables a user account with the given name" )
-argget.add_argument( "--disable", "-disable", type = str, help = "Disabled a user account with the given name" )
-argget.add_argument( "--unlock", "-unlock", type = str, help = "Unlocks a user account with the given name" )
-argget.add_argument( "--debug", action = "store_true", help = "Creates debug file showing HTTP traces and exceptions" )
+argget = argparse.ArgumentParser(description="A tool to manage user accounts on a Redfish service")
+argget.add_argument("--user", "-u", type=str, required=True, help="The user name for authentication")
+argget.add_argument("--password", "-p", type=str, required=True, help="The password for authentication")
+argget.add_argument("--rhost", "-r", type=str, required=True, help="The address of the Redfish service (with scheme)")
+argget.add_argument(
+    "--add", "-add", type=str, nargs=3, metavar=("name", "password", "role"), help="Adds a new user account"
+)
+argget.add_argument("--delete", "-delete", type=str, help="Deletes a user account with the given name")
+argget.add_argument(
+    "--setname",
+    "-setname",
+    type=str,
+    nargs=2,
+    metavar=("old_name", "new_name"),
+    help="Sets a user account to a new name",
+)
+argget.add_argument(
+    "--setpassword",
+    "-setpassword",
+    type=str,
+    nargs=2,
+    metavar=("name", "new_password"),
+    help="Sets a user account to a new password",
+)
+argget.add_argument(
+    "--setrole", "-setrole", type=str, nargs=2, metavar=("name", "new_role"), help="Sets a user account to a new role"
+)
+argget.add_argument("--enable", "-enable", type=str, help="Enables a user account with the given name")
+argget.add_argument("--disable", "-disable", type=str, help="Disabled a user account with the given name")
+argget.add_argument("--unlock", "-unlock", type=str, help="Unlocks a user account with the given name")
+argget.add_argument("--debug", action="store_true", help="Creates debug file showing HTTP traces and exceptions")
 args = argget.parse_args()
 
 if args.debug:
-    log_file = "rf_accounts-{}.log".format( datetime.datetime.now().strftime( "%Y-%m-%d-%H%M%S" ) )
+    log_file = "rf_accounts-{}.log".format(datetime.datetime.now().strftime("%Y-%m-%d-%H%M%S"))
     log_format = "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
-    logger = redfish.redfish_logger( log_file, log_format, logging.DEBUG )
-    logger.info( "rf_accounts Trace" )
+    logger = redfish.redfish_logger(log_file, log_format, logging.DEBUG)
+    logger.info("rf_accounts Trace")
 
 # Set up the Redfish object
 user_uri = None
 redfish_obj = None
 try:
-    redfish_obj = redfish.redfish_client( base_url = args.rhost, username = args.user, password = args.password, timeout = 15, max_retry = 3 )
-    redfish_obj.login( auth = "session" )
+    redfish_obj = redfish.redfish_client(
+        base_url=args.rhost, username=args.user, password=args.password, timeout=15, max_retry=3
+    )
+    redfish_obj.login(auth="session")
 except RedfishPasswordChangeRequiredError as e:
     if args.setpassword is None:
-        redfish_utilities.print_password_change_required_and_logout( redfish_obj, args )
-        sys.exit( 1 )
+        redfish_utilities.print_password_change_required_and_logout(redfish_obj, args)
+        sys.exit(1)
     else:
         user_uri = e.args[1]
         if args.setpassword[0] == args.user:
             # The user is requesting to change their own password
             # Allow the request to go through directly, and log out
             exit_code = 0
             try:
-                print( "Changing password of user '{}'".format( args.setpassword[0] ) )
-                redfish_utilities.modify_user( redfish_obj, args.setpassword[0], new_password = args.setpassword[1], user_uri = user_uri )
+                print("Changing password of user '{}'".format(args.setpassword[0]))
+                redfish_utilities.modify_user(
+                    redfish_obj, args.setpassword[0], new_password=args.setpassword[1], user_uri=user_uri
+                )
             except Exception as e:
                 if args.debug:
-                    logger.error( "Caught exception:\n\n{}\n".format( traceback.format_exc() ) )
+                    logger.error("Caught exception:\n\n{}\n".format(traceback.format_exc()))
                 exit_code = 1
-                print( e )
+                print(e)
             finally:
                 # Log out
-                redfish_utilities.logout( redfish_obj, ignore_error = True )    # Some services do not allow session logout in this condition
-            sys.exit( exit_code )
+                redfish_utilities.logout(
+                    redfish_obj, ignore_error=True
+                )  # Some services do not allow session logout in this condition
+            sys.exit(exit_code)
         else:
-            redfish_utilities.print_password_change_required_and_logout( redfish_obj, args )
-            sys.exit( 1 )
-except Exception as e:
+            redfish_utilities.print_password_change_required_and_logout(redfish_obj, args)
+            sys.exit(1)
+except Exception:
     raise
 
 exit_code = 0
 try:
     print_accounts = True
     if args.add is not None:
-        print( "Adding new user '{}'".format( args.add[0] ) )
-        redfish_utilities.add_user( redfish_obj, args.add[0], args.add[1], args.add[2] )
+        print("Adding new user '{}'".format(args.add[0]))
+        redfish_utilities.add_user(redfish_obj, args.add[0], args.add[1], args.add[2])
         print_accounts = False
     if args.delete is not None:
-        print( "Deleting user '{}'".format( args.delete ) )
-        redfish_utilities.delete_user( redfish_obj, args.delete )
+        print("Deleting user '{}'".format(args.delete))
+        redfish_utilities.delete_user(redfish_obj, args.delete)
         print_accounts = False
     if args.setname is not None:
-        print( "Changing name of user '{}' to '{}'".format( args.setname[0], args.setname[1] ) )
-        redfish_utilities.modify_user( redfish_obj, args.setname[0], new_name = args.setname[1] )
+        print("Changing name of user '{}' to '{}'".format(args.setname[0], args.setname[1]))
+        redfish_utilities.modify_user(redfish_obj, args.setname[0], new_name=args.setname[1])
         print_accounts = False
     if args.setpassword is not None:
-        print( "Changing password of user '{}'".format( args.setpassword[0] ) )
-        redfish_utilities.modify_user( redfish_obj, args.setpassword[0], new_password = args.setpassword[1] )
+        print("Changing password of user '{}'".format(args.setpassword[0]))
+        redfish_utilities.modify_user(redfish_obj, args.setpassword[0], new_password=args.setpassword[1])
         print_accounts = False
     if args.setrole is not None:
-        print( "Changing role of user '{}' to '{}'".format( args.setrole[0], args.setrole[1] ) )
-        redfish_utilities.modify_user( redfish_obj, args.setrole[0], new_role = args.setrole[1] )
+        print("Changing role of user '{}' to '{}'".format(args.setrole[0], args.setrole[1]))
+        redfish_utilities.modify_user(redfish_obj, args.setrole[0], new_role=args.setrole[1])
         print_accounts = False
     if args.enable is not None:
-        print( "Enabling user '{}'".format( args.enable ) )
-        redfish_utilities.modify_user( redfish_obj, args.enable, new_enabled = True )
+        print("Enabling user '{}'".format(args.enable))
+        redfish_utilities.modify_user(redfish_obj, args.enable, new_enabled=True)
         print_accounts = False
     if args.disable is not None:
-        print( "Disabling user '{}'".format( args.disable ) )
-        redfish_utilities.modify_user( redfish_obj, args.disable, new_enabled = False )
+        print("Disabling user '{}'".format(args.disable))
+        redfish_utilities.modify_user(redfish_obj, args.disable, new_enabled=False)
         print_accounts = False
     if args.unlock is not None:
-        print( "Unlocking user '{}'".format( args.unlock ) )
-        redfish_utilities.modify_user( redfish_obj, args.unlock, new_locked = False )
+        print("Unlocking user '{}'".format(args.unlock))
+        redfish_utilities.modify_user(redfish_obj, args.unlock, new_locked=False)
         print_accounts = False
     if print_accounts:
-        user_list = redfish_utilities.get_users( redfish_obj )
-        redfish_utilities.print_users( user_list )
+        user_list = redfish_utilities.get_users(redfish_obj)
+        redfish_utilities.print_users(user_list)
 except Exception as e:
     if args.debug:
-        logger.error( "Caught exception:\n\n{}\n".format( traceback.format_exc() ) )
+        logger.error("Caught exception:\n\n{}\n".format(traceback.format_exc()))
     exit_code = 1
-    print( e )
+    print(e)
 finally:
     # Log out
-    redfish_utilities.logout( redfish_obj )
-sys.exit( exit_code )
+    redfish_utilities.logout(redfish_obj)
+sys.exit(exit_code)
```

### Comparing `redfish_utilities-3.2.8/scripts/rf_assembly.py` & `redfish_utilities-3.2.9/scripts/rf_assembly.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,63 +17,69 @@
 import redfish
 import redfish_utilities
 import traceback
 import sys
 from redfish.messages import RedfishPasswordChangeRequiredError
 
 # Get the input arguments
-argget = argparse.ArgumentParser( description = "A tool to manage assemblies on a Redfish service" )
-argget.add_argument( "--user", "-u", type = str, required = True, help = "The user name for authentication" )
-argget.add_argument( "--password", "-p",  type = str, required = True, help = "The password for authentication" )
-argget.add_argument( "--rhost", "-r", type = str, required = True, help = "The address of the Redfish service (with scheme)" )
-argget.add_argument( "--assembly", "-a", type = str, required = True, help = "The URI of the target assembly" )
-argget.add_argument( "--index", "-i", type = int, help = "The target assembly index" )
-argget.add_argument( "--debug", action = "store_true", help = "Creates debug file showing HTTP traces and exceptions" )
-subparsers = argget.add_subparsers( dest = "command" )
-info_argget = subparsers.add_parser( "info", help = "Displays information about the an assembly" )
-download_argget = subparsers.add_parser( "download", help = "Downloads assembly data to a file" )
-download_argget.add_argument( "--file", "-f", type = str, required = True, help = "The file, and optional path, to save the assembly data" )
-upload_argget = subparsers.add_parser( "upload", help = "Uploads assembly data from a file" )
-upload_argget.add_argument( "--file", "-f", type = str, required = True, help = "The file, and optional path, containing the assembly data to upload" )
+argget = argparse.ArgumentParser(description="A tool to manage assemblies on a Redfish service")
+argget.add_argument("--user", "-u", type=str, required=True, help="The user name for authentication")
+argget.add_argument("--password", "-p", type=str, required=True, help="The password for authentication")
+argget.add_argument("--rhost", "-r", type=str, required=True, help="The address of the Redfish service (with scheme)")
+argget.add_argument("--assembly", "-a", type=str, required=True, help="The URI of the target assembly")
+argget.add_argument("--index", "-i", type=int, help="The target assembly index")
+argget.add_argument("--debug", action="store_true", help="Creates debug file showing HTTP traces and exceptions")
+subparsers = argget.add_subparsers(dest="command")
+info_argget = subparsers.add_parser("info", help="Displays information about the an assembly")
+download_argget = subparsers.add_parser("download", help="Downloads assembly data to a file")
+download_argget.add_argument(
+    "--file", "-f", type=str, required=True, help="The file, and optional path, to save the assembly data"
+)
+upload_argget = subparsers.add_parser("upload", help="Uploads assembly data from a file")
+upload_argget.add_argument(
+    "--file", "-f", type=str, required=True, help="The file, and optional path, containing the assembly data to upload"
+)
 args = argget.parse_args()
 
 if args.index and args.index < 0:
-    print( "rf_assembly.py: error: the assembly index cannot be negative" )
-    sys.exit( 1 )
+    print("rf_assembly.py: error: the assembly index cannot be negative")
+    sys.exit(1)
 
 if args.debug:
-    log_file = "rf_assembly-{}.log".format( datetime.datetime.now().strftime( "%Y-%m-%d-%H%M%S" ) )
+    log_file = "rf_assembly-{}.log".format(datetime.datetime.now().strftime("%Y-%m-%d-%H%M%S"))
     log_format = "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
-    logger = redfish.redfish_logger( log_file, log_format, logging.DEBUG )
-    logger.info( "rf_assembly Trace" )
+    logger = redfish.redfish_logger(log_file, log_format, logging.DEBUG)
+    logger.info("rf_assembly Trace")
 
 # Set up the Redfish object
 redfish_obj = None
 try:
-    redfish_obj = redfish.redfish_client( base_url = args.rhost, username = args.user, password = args.password, timeout = 15, max_retry = 3 )
-    redfish_obj.login( auth = "session" )
-except RedfishPasswordChangeRequiredError as e:
-    redfish_utilities.print_password_change_required_and_logout( redfish_obj, args )
-    sys.exit( 1 )
-except Exception as e:
+    redfish_obj = redfish.redfish_client(
+        base_url=args.rhost, username=args.user, password=args.password, timeout=15, max_retry=3
+    )
+    redfish_obj.login(auth="session")
+except RedfishPasswordChangeRequiredError:
+    redfish_utilities.print_password_change_required_and_logout(redfish_obj, args)
+    sys.exit(1)
+except Exception:
     raise
 
 exit_code = 0
 try:
-    assembly_info = redfish_utilities.get_assembly( redfish_obj, args.assembly )
+    assembly_info = redfish_utilities.get_assembly(redfish_obj, args.assembly)
     if args.command == "download":
-        print( "Saving data to '{}'...".format( args.file ) )
-        redfish_utilities.download_assembly( redfish_obj, assembly_info, args.file, args.index )
+        print("Saving data to '{}'...".format(args.file))
+        redfish_utilities.download_assembly(redfish_obj, assembly_info, args.file, args.index)
     elif args.command == "upload":
-        print( "Writing data from '{}'...".format( args.file) )
-        redfish_utilities.upload_assembly( redfish_obj, assembly_info, args.file, args.index )
+        print("Writing data from '{}'...".format(args.file))
+        redfish_utilities.upload_assembly(redfish_obj, assembly_info, args.file, args.index)
     else:
-        redfish_utilities.print_assembly( assembly_info, args.index )
+        redfish_utilities.print_assembly(assembly_info, args.index)
 except Exception as e:
     if args.debug:
-        logger.error( "Caught exception:\n\n{}\n".format( traceback.format_exc() ) )
+        logger.error("Caught exception:\n\n{}\n".format(traceback.format_exc()))
     exit_code = 1
-    print( e )
+    print(e)
 finally:
     # Log out
-    redfish_utilities.logout( redfish_obj )
-sys.exit( exit_code )
+    redfish_utilities.logout(redfish_obj)
+sys.exit(exit_code)
```

### Comparing `redfish_utilities-3.2.8/scripts/rf_bios_settings.py` & `redfish_utilities-3.2.9/scripts/rf_bios_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,77 +17,93 @@
 import redfish
 import redfish_utilities
 import traceback
 import sys
 from redfish.messages import RedfishPasswordChangeRequiredError
 
 # Get the input arguments
-argget = argparse.ArgumentParser( description = "A tool to manager BIOS settings for a system" )
-argget.add_argument( "--user", "-u", type = str, required = True, help = "The user name for authentication" )
-argget.add_argument( "--password", "-p",  type = str, required = True, help = "The password for authentication" )
-argget.add_argument( "--rhost", "-r", type = str, required = True, help = "The address of the Redfish service (with scheme)" )
-argget.add_argument( "--system", "-s", type = str, help = "The ID of the system to manage" )
-argget.add_argument( "--attribute", "-a", type = str, nargs = 2, metavar = ( "name", "value" ), action = "append", help = "Sets a BIOS attribute to a new value; can be supplied multiple times to set multiple attributes" )
-argget.add_argument( "--workaround", "-workaround", action = "store_true", help = "Indicates if workarounds should be attempted for non-conformant services", default = False )
-argget.add_argument( "--debug", action = "store_true", help = "Creates debug file showing HTTP traces and exceptions" )
+argget = argparse.ArgumentParser(description="A tool to manager BIOS settings for a system")
+argget.add_argument("--user", "-u", type=str, required=True, help="The user name for authentication")
+argget.add_argument("--password", "-p", type=str, required=True, help="The password for authentication")
+argget.add_argument("--rhost", "-r", type=str, required=True, help="The address of the Redfish service (with scheme)")
+argget.add_argument("--system", "-s", type=str, help="The ID of the system to manage")
+argget.add_argument(
+    "--attribute",
+    "-a",
+    type=str,
+    nargs=2,
+    metavar=("name", "value"),
+    action="append",
+    help="Sets a BIOS attribute to a new value; can be supplied multiple times to set multiple attributes",
+)
+argget.add_argument(
+    "--workaround",
+    "-workaround",
+    action="store_true",
+    help="Indicates if workarounds should be attempted for non-conformant services",
+    default=False,
+)
+argget.add_argument("--debug", action="store_true", help="Creates debug file showing HTTP traces and exceptions")
 args = argget.parse_args()
 
 if args.workaround:
     redfish_utilities.config.__workarounds__ = True
 
 if args.debug:
-    log_file = "rf_bios_settings-{}.log".format( datetime.datetime.now().strftime( "%Y-%m-%d-%H%M%S" ) )
+    log_file = "rf_bios_settings-{}.log".format(datetime.datetime.now().strftime("%Y-%m-%d-%H%M%S"))
     log_format = "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
-    logger = redfish.redfish_logger( log_file, log_format, logging.DEBUG )
-    logger.info( "rf_bios_settings Trace" )
+    logger = redfish.redfish_logger(log_file, log_format, logging.DEBUG)
+    logger.info("rf_bios_settings Trace")
 
 # Set up the Redfish object
 redfish_obj = None
 try:
-    redfish_obj = redfish.redfish_client( base_url = args.rhost, username = args.user, password = args.password, timeout = 15, max_retry = 3 )
-    redfish_obj.login( auth = "session" )
-except RedfishPasswordChangeRequiredError as e:
-    redfish_utilities.print_password_change_required_and_logout( redfish_obj, args )
-    sys.exit( 1 )
-except Exception as e:
+    redfish_obj = redfish.redfish_client(
+        base_url=args.rhost, username=args.user, password=args.password, timeout=15, max_retry=3
+    )
+    redfish_obj.login(auth="session")
+except RedfishPasswordChangeRequiredError:
+    redfish_utilities.print_password_change_required_and_logout(redfish_obj, args)
+    sys.exit(1)
+except Exception:
     raise
 
 exit_code = 0
 try:
     # Get the BIOS settings
-    current_settings, future_settings = redfish_utilities.get_system_bios( redfish_obj, args.system )
+    current_settings, future_settings = redfish_utilities.get_system_bios(redfish_obj, args.system)
 
     if args.attribute is not None:
         new_settings = {}
         for attribute in args.attribute:
             # Based on the current settings, determine the appropriate data type for the new setting
             new_value = attribute[1]
             if attribute[0] in current_settings:
-                if isinstance( current_settings[attribute[0]], bool ):
+                if isinstance(current_settings[attribute[0]], bool):
                     # Boolean; convert from a string
                     if new_value.lower() == "true":
                         new_value = True
                     else:
                         new_value = False
-                elif isinstance( current_settings[attribute[0]], ( int, float ) ):
+                elif isinstance(current_settings[attribute[0]], (int, float)):
                     # Integer or float; go by the user input to determine how to convert since the current value may be truncated
                     try:
-                        new_value = int( new_value )
-                    except:
-                        new_value = float( new_value )
+                        new_value = int(new_value)
+                    except Exception:
+                        new_value = float(new_value)
 
             # Set the specified attribute to the new value
             new_settings[attribute[0]] = new_value
-            print( "Setting {} to {}...".format( attribute[0], attribute[1] ) )
-        redfish_utilities.set_system_bios( redfish_obj, new_settings, args.system )
+            print("Setting {} to {}...".format(attribute[0], attribute[1]))
+        redfish_utilities.set_system_bios(redfish_obj, new_settings, args.system)
     else:
         # Print the BIOS settings
-        redfish_utilities.print_system_bios( current_settings, future_settings )
+        redfish_utilities.print_system_bios(current_settings, future_settings)
 except Exception as e:
     if args.debug:
-        logger.error( "Caught exception:\n\n{}\n".format( traceback.format_exc() ) )
+        logger.error("Caught exception:\n\n{}\n".format(traceback.format_exc()))
     exit_code = 1
-    print( e )
+    print(e)
 finally:
     # Log out
-    redfish_utilities.logout( redfish_obj )
-sys.exit( exit_code )
+    redfish_utilities.logout(redfish_obj)
+sys.exit(exit_code)
```

### Comparing `redfish_utilities-3.2.8/scripts/rf_boot_override.py` & `redfish_utilities-3.2.9/scripts/rf_boot_override.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,83 +18,105 @@
 import redfish
 import redfish_utilities
 import traceback
 import sys
 from redfish.messages import RedfishPasswordChangeRequiredError
 
 # Get the input arguments
-argget = argparse.ArgumentParser( description = "A tool to perform a one time boot override of a system" )
-argget.add_argument( "--user", "-u", type = str, required = True, help = "The user name for authentication" )
-argget.add_argument( "--password", "-p",  type = str, required = True, help = "The password for authentication" )
-argget.add_argument( "--rhost", "-r", type = str, required = True, help = "The address of the Redfish service (with scheme)" )
-argget.add_argument( "--system", "-s", type = str, help = "The ID of the system to set" )
-argget.add_argument( "--info", "-info", action = "store_true", help = "Indicates if boot information should be reported" )
-argget.add_argument( "--target", "-t", type = str, help = "The target boot device; if this argument is omitted the tool will display the current boot settings" )
-argget.add_argument( "--uefi", "-uefi", type = str, help = "If target is 'UefiTarget', the UEFI Device Path of the device to boot.  If target is 'UefiBootNext', the UEFI Boot Option string of the device to boot." )
-argget.add_argument( "--mode", "-m", type = str, help = "The requested boot mode ('UEFI' or 'Legacy')" )
-argget.add_argument( "--reset", "-reset", action = "store_true", help = "Signifies that the system is reset after the boot override is set" )
-argget.add_argument( "--workaround", "-workaround", action = "store_true", help = "Indicates if workarounds should be attempted for non-conformant services", default = False )
-argget.add_argument( "--debug", action = "store_true", help = "Creates debug file showing HTTP traces and exceptions" )
+argget = argparse.ArgumentParser(description="A tool to perform a one time boot override of a system")
+argget.add_argument("--user", "-u", type=str, required=True, help="The user name for authentication")
+argget.add_argument("--password", "-p", type=str, required=True, help="The password for authentication")
+argget.add_argument("--rhost", "-r", type=str, required=True, help="The address of the Redfish service (with scheme)")
+argget.add_argument("--system", "-s", type=str, help="The ID of the system to set")
+argget.add_argument("--info", "-info", action="store_true", help="Indicates if boot information should be reported")
+argget.add_argument(
+    "--target",
+    "-t",
+    type=str,
+    help="The target boot device; if this argument is omitted the tool will display the current boot settings",
+)
+argget.add_argument(
+    "--uefi",
+    "-uefi",
+    type=str,
+    help="If target is 'UefiTarget', the UEFI Device Path of the device to boot.  If target is 'UefiBootNext', the UEFI Boot Option string of the device to boot.",
+)
+argget.add_argument("--mode", "-m", type=str, help="The requested boot mode ('UEFI' or 'Legacy')")
+argget.add_argument(
+    "--reset", "-reset", action="store_true", help="Signifies that the system is reset after the boot override is set"
+)
+argget.add_argument(
+    "--workaround",
+    "-workaround",
+    action="store_true",
+    help="Indicates if workarounds should be attempted for non-conformant services",
+    default=False,
+)
+argget.add_argument("--debug", action="store_true", help="Creates debug file showing HTTP traces and exceptions")
 args = argget.parse_args()
 
 # Verify the combination of arguments is correct
 if args.target is None:
     args.info = True
     if args.uefi or args.mode or args.reset:
-        argget.error( "Cannot use '--uefi', '--mode', or '--reset' without '--target'" )
+        argget.error("Cannot use '--uefi', '--mode', or '--reset' without '--target'")
 
 if args.workaround:
     redfish_utilities.config.__workarounds__ = True
 
 if args.debug:
-    log_file = "rf_boot_override-{}.log".format( datetime.datetime.now().strftime( "%Y-%m-%d-%H%M%S" ) )
+    log_file = "rf_boot_override-{}.log".format(datetime.datetime.now().strftime("%Y-%m-%d-%H%M%S"))
     log_format = "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
-    logger = redfish.redfish_logger( log_file, log_format, logging.DEBUG )
-    logger.info( "rf_boot_override Trace" )
+    logger = redfish.redfish_logger(log_file, log_format, logging.DEBUG)
+    logger.info("rf_boot_override Trace")
 
 # Set up the Redfish object
 redfish_obj = None
 try:
-    redfish_obj = redfish.redfish_client( base_url = args.rhost, username = args.user, password = args.password, timeout = 15, max_retry = 3 )
-    redfish_obj.login( auth = "session" )
-except RedfishPasswordChangeRequiredError as e:
-    redfish_utilities.print_password_change_required_and_logout( redfish_obj, args )
-    sys.exit( 1 )
-except Exception as e:
+    redfish_obj = redfish.redfish_client(
+        base_url=args.rhost, username=args.user, password=args.password, timeout=15, max_retry=3
+    )
+    redfish_obj.login(auth="session")
+except RedfishPasswordChangeRequiredError:
+    redfish_utilities.print_password_change_required_and_logout(redfish_obj, args)
+    sys.exit(1)
+except Exception:
     raise
 
 exit_code = 0
 try:
     if args.info:
-        boot = redfish_utilities.get_system_boot( redfish_obj, args.system )
-        redfish_utilities.print_system_boot( boot )
+        boot = redfish_utilities.get_system_boot(redfish_obj, args.system)
+        redfish_utilities.print_system_boot(boot)
     else:
         # Build and send the boot request based on the arguments given
         uefi_target = None
         boot_next = None
         boot_enable = "Once"
         if args.target == "UefiTarget":
             uefi_target = args.uefi
         if args.target == "UefiBootNext":
             boot_next = args.uefi
         if args.target == "None":
-            print( "Disabling one time boot..." )
+            print("Disabling one time boot...")
             boot_enable = "Disabled"
         else:
-            print( "Setting a one time boot for {}...".format( args.target ) )
-        redfish_utilities.set_system_boot( redfish_obj, args.system, args.target, boot_enable, args.mode, uefi_target, boot_next )
+            print("Setting a one time boot for {}...".format(args.target))
+        redfish_utilities.set_system_boot(
+            redfish_obj, args.system, args.target, boot_enable, args.mode, uefi_target, boot_next
+        )
 
         # Reset the system if requested
         if args.reset:
-            print( "Resetting the system..." )
-            response = redfish_utilities.system_reset( redfish_obj, args.system )
-            response = redfish_utilities.poll_task_monitor( redfish_obj, response )
-            redfish_utilities.verify_response( response )
+            print("Resetting the system...")
+            response = redfish_utilities.system_reset(redfish_obj, args.system)
+            response = redfish_utilities.poll_task_monitor(redfish_obj, response)
+            redfish_utilities.verify_response(response)
 except Exception as e:
     if args.debug:
-        logger.error( "Caught exception:\n\n{}\n".format( traceback.format_exc() ) )
+        logger.error("Caught exception:\n\n{}\n".format(traceback.format_exc()))
     exit_code = 1
-    print( e )
+    print(e)
 finally:
     # Log out
-    redfish_utilities.logout( redfish_obj )
-sys.exit( exit_code )
+    redfish_utilities.logout(redfish_obj)
+sys.exit(exit_code)
```

### Comparing `redfish_utilities-3.2.8/scripts/rf_diagnostic_data.py` & `redfish_utilities-3.2.9/scripts/rf_diagnostic_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,84 +18,114 @@
 import redfish
 import redfish_utilities
 import traceback
 import sys
 from redfish.messages import RedfishPasswordChangeRequiredError
 
 # Get the input arguments
-argget = argparse.ArgumentParser( description = "A tool to collect diagnostic data from a log service on a Redfish service" )
-argget.add_argument( "--user", "-u", type = str, required = True, help = "The user name for authentication" )
-argget.add_argument( "--password", "-p",  type = str, required = True, help = "The password for authentication" )
-argget.add_argument( "--rhost", "-r", type = str, required = True, help = "The address of the Redfish service (with scheme)" )
-argget.add_argument( "--manager", "-m", type = str, nargs = "?", default = False, help = "The ID of the manager containing the log service" )
-argget.add_argument( "--system", "-s", type = str, nargs = "?", default = False, help = "The ID of the system containing the log service" )
-argget.add_argument( "--chassis", "-c", type = str, nargs = "?", default = False, help = "The ID of the chassis containing the log service" )
-argget.add_argument( "--log", "-l", type = str, help = "The ID of the log service" )
-argget.add_argument( "--type", "-type", type = redfish_utilities.diagnostic_data_types, help = "The type of diagnostic data to collect; defaults to 'Manager' if not specified", choices = redfish_utilities.diagnostic_data_types, default = redfish_utilities.diagnostic_data_types.MANAGER )
-argget.add_argument( "--oemtype", "-oemtype", type = str, help = "The OEM-specific type of diagnostic data to collect; this option should only be used if the requested type is 'OEM'" )
-argget.add_argument( "--directory", "-d", type = str, help = "The directory to save the diagnostic data; defaults to the current directory if not specified", default = "." )
-argget.add_argument( "--debug", action = "store_true", help = "Creates debug file showing HTTP traces and exceptions" )
+argget = argparse.ArgumentParser(
+    description="A tool to collect diagnostic data from a log service on a Redfish service"
+)
+argget.add_argument("--user", "-u", type=str, required=True, help="The user name for authentication")
+argget.add_argument("--password", "-p", type=str, required=True, help="The password for authentication")
+argget.add_argument("--rhost", "-r", type=str, required=True, help="The address of the Redfish service (with scheme)")
+argget.add_argument(
+    "--manager", "-m", type=str, nargs="?", default=False, help="The ID of the manager containing the log service"
+)
+argget.add_argument(
+    "--system", "-s", type=str, nargs="?", default=False, help="The ID of the system containing the log service"
+)
+argget.add_argument(
+    "--chassis", "-c", type=str, nargs="?", default=False, help="The ID of the chassis containing the log service"
+)
+argget.add_argument("--log", "-l", type=str, help="The ID of the log service")
+argget.add_argument(
+    "--type",
+    "-type",
+    type=redfish_utilities.diagnostic_data_types,
+    help="The type of diagnostic data to collect; defaults to 'Manager' if not specified",
+    choices=redfish_utilities.diagnostic_data_types,
+    default=redfish_utilities.diagnostic_data_types.MANAGER,
+)
+argget.add_argument(
+    "--oemtype",
+    "-oemtype",
+    type=str,
+    help="The OEM-specific type of diagnostic data to collect; this option should only be used if the requested type is 'OEM'",
+)
+argget.add_argument(
+    "--directory",
+    "-d",
+    type=str,
+    help="The directory to save the diagnostic data; defaults to the current directory if not specified",
+    default=".",
+)
+argget.add_argument("--debug", action="store_true", help="Creates debug file showing HTTP traces and exceptions")
 args = argget.parse_args()
 
 # Determine the target log service based on the inputs
 # Effectively if the user gives multiple targets, some will be ignored
 container_type = redfish_utilities.log_container.MANAGER
 container_id = None
-if args.manager != False:
+if args.manager is not False:
     container_type = redfish_utilities.log_container.MANAGER
     container_id = args.manager
-elif args.system != False:
+elif args.system is not False:
     container_type = redfish_utilities.log_container.SYSTEM
     container_id = args.system
-elif args.chassis != False:
+elif args.chassis is not False:
     container_type = redfish_utilities.log_container.CHASSIS
     container_id = args.chassis
 
 if args.debug:
-    log_file = "rf_diagnostic_data-{}.log".format( datetime.datetime.now().strftime( "%Y-%m-%d-%H%M%S" ) )
+    log_file = "rf_diagnostic_data-{}.log".format(datetime.datetime.now().strftime("%Y-%m-%d-%H%M%S"))
     log_format = "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
-    logger = redfish.redfish_logger( log_file, log_format, logging.DEBUG )
-    logger.info( "rf_diagnostic_data Trace" )
+    logger = redfish.redfish_logger(log_file, log_format, logging.DEBUG)
+    logger.info("rf_diagnostic_data Trace")
 
 # Set up the Redfish object
 redfish_obj = None
 try:
-    redfish_obj = redfish.redfish_client( base_url = args.rhost, username = args.user, password = args.password, timeout = 15, max_retry = 3 )
-    redfish_obj.login( auth = "session" )
-except RedfishPasswordChangeRequiredError as e:
-    redfish_utilities.print_password_change_required_and_logout( redfish_obj, args )
-    sys.exit( 1 )
-except Exception as e:
+    redfish_obj = redfish.redfish_client(
+        base_url=args.rhost, username=args.user, password=args.password, timeout=15, max_retry=3
+    )
+    redfish_obj.login(auth="session")
+except RedfishPasswordChangeRequiredError:
+    redfish_utilities.print_password_change_required_and_logout(redfish_obj, args)
+    sys.exit(1)
+except Exception:
     raise
 
 exit_code = 0
 try:
-    print( "Collecting diagnostic data..." )
-    response = redfish_utilities.collect_diagnostic_data( redfish_obj, container_type, container_id, args.log, args.type, args.oemtype )
-    response = redfish_utilities.poll_task_monitor( redfish_obj, response )
-    filename, data = redfish_utilities.download_diagnostic_data( redfish_obj, response )
+    print("Collecting diagnostic data...")
+    response = redfish_utilities.collect_diagnostic_data(
+        redfish_obj, container_type, container_id, args.log, args.type, args.oemtype
+    )
+    response = redfish_utilities.poll_task_monitor(redfish_obj, response)
+    filename, data = redfish_utilities.download_diagnostic_data(redfish_obj, response)
 
     # Save the file
-    if not os.path.isdir( args.directory ):
-        os.makedirs( args.directory )
-    path = os.path.join( args.directory, filename )
-    name_parts = filename.split( ".", 1 )
+    if not os.path.isdir(args.directory):
+        os.makedirs(args.directory)
+    path = os.path.join(args.directory, filename)
+    name_parts = filename.split(".", 1)
     file_check = 0
-    if len( name_parts ) == 1:
-        name_parts.append( "" )
-    while os.path.isfile( path ):
+    if len(name_parts) == 1:
+        name_parts.append("")
+    while os.path.isfile(path):
         # If the file already exists, build a new file name with a counter
         file_check = file_check + 1
-        filename = "{}({}).{}".format( name_parts[0], file_check, name_parts[1] )
-        path = os.path.join( args.directory, filename )
-    with open( path, "wb" ) as file:
-        file.write( data )
-    print( "Saved diagnostic data to '{}'".format( path ) )
+        filename = "{}({}).{}".format(name_parts[0], file_check, name_parts[1])
+        path = os.path.join(args.directory, filename)
+    with open(path, "wb") as file:
+        file.write(data)
+    print("Saved diagnostic data to '{}'".format(path))
 except Exception as e:
     if args.debug:
-        logger.error( "Caught exception:\n\n{}\n".format( traceback.format_exc() ) )
+        logger.error("Caught exception:\n\n{}\n".format(traceback.format_exc()))
     exit_code = 1
-    print( e )
+    print(e)
 finally:
     # Log out
-    redfish_utilities.logout( redfish_obj )
-sys.exit( exit_code )
+    redfish_utilities.logout(redfish_obj)
+sys.exit(exit_code)
```

### Comparing `redfish_utilities-3.2.8/scripts/rf_discover.py` & `redfish_utilities-3.2.9/scripts/rf_discover.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,33 +13,33 @@
 
 import argparse
 import re
 import redfish
 import sys
 
 # No arguments, but having help text is useful
-argget = argparse.ArgumentParser( description = "A tool to discover Redfish services" )
+argget = argparse.ArgumentParser(description="A tool to discover Redfish services")
 args = argget.parse_args()
 
 # Invoke the discovery routine for SSDP and print the responses
 services = redfish.discover_ssdp()
-if len( services ) == 0:
-    print( "No Redfish services discovered" )
-    sys.exit( 1 )
+if len(services) == 0:
+    print("No Redfish services discovered")
+    sys.exit(1)
 else:
-    print( "Redfish services:" )
+    print("Redfish services:")
 
 # Go through each discovered service and print out basic info
 for service in services:
     # Try to get the Product property from the service root for each service
     # If found, print the UUID, service root pointer, and the Product
     # If not, just print the UUID and service root pointer
     try:
         # Need to strip off /redfish/v1 from the SSDP response to use the URL with the library
-        groups = re.search( r"^(.+)\/redfish\/v1\/?$", services[service] )
-        url = groups.group( 1 )
-        redfish_obj = redfish.redfish_client( base_url = url, timeout = 15, max_retry = 3 )
-        print( "{}: {} ({})".format( service, services[service], redfish_obj.root["Product"] ) )
-    except:
-        print( "{}: {}".format( service, services[service] ) )
+        groups = re.search(r"^(.+)\/redfish\/v1\/?$", services[service])
+        url = groups.group(1)
+        redfish_obj = redfish.redfish_client(base_url=url, timeout=15, max_retry=3)
+        print("{}: {} ({})".format(service, services[service], redfish_obj.root["Product"]))
+    except Exception:
+        print("{}: {}".format(service, services[service]))
 
-sys.exit( 0 )
+sys.exit(0)
```

### Comparing `redfish_utilities-3.2.8/scripts/rf_licenses.py` & `redfish_utilities-3.2.9/scripts/rf_licenses.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,65 +17,71 @@
 import redfish
 import redfish_utilities
 import traceback
 import sys
 from redfish.messages import RedfishPasswordChangeRequiredError
 
 # Get the input arguments
-argget = argparse.ArgumentParser( description = "A tool to manage licenses on a Redfish service" )
-argget.add_argument( "--user", "-u", type = str, required = True, help = "The user name for authentication" )
-argget.add_argument( "--password", "-p",  type = str, required = True, help = "The password for authentication" )
-argget.add_argument( "--rhost", "-r", type = str, required = True, help = "The address of the Redfish service (with scheme)" )
-argget.add_argument( "--debug", action = "store_true", help = "Creates debug file showing HTTP traces and exceptions" )
-subparsers = argget.add_subparsers( dest = "command" )
-info_argget = subparsers.add_parser( "info", help = "Displays information about the licenses installed on the service" )
-info_argget.add_argument( "--details", "-details", action = "store_true", help = "Indicates if the full details of each license should be shown" )
-install_argget = subparsers.add_parser( "install", help = "Installs a new license" )
-install_argget.add_argument( "--license", "-l", type = str, required = True, help = "The filepath or URI to the license to install" )
-delete_argget = subparsers.add_parser( "delete", help = "Deletes a license" )
-delete_argget.add_argument( "--license", "-l", type = str, required = True, help = "The identifier of the license to delete" )
+argget = argparse.ArgumentParser(description="A tool to manage licenses on a Redfish service")
+argget.add_argument("--user", "-u", type=str, required=True, help="The user name for authentication")
+argget.add_argument("--password", "-p", type=str, required=True, help="The password for authentication")
+argget.add_argument("--rhost", "-r", type=str, required=True, help="The address of the Redfish service (with scheme)")
+argget.add_argument("--debug", action="store_true", help="Creates debug file showing HTTP traces and exceptions")
+subparsers = argget.add_subparsers(dest="command")
+info_argget = subparsers.add_parser("info", help="Displays information about the licenses installed on the service")
+info_argget.add_argument(
+    "--details", "-details", action="store_true", help="Indicates if the full details of each license should be shown"
+)
+install_argget = subparsers.add_parser("install", help="Installs a new license")
+install_argget.add_argument(
+    "--license", "-l", type=str, required=True, help="The filepath or URI to the license to install"
+)
+delete_argget = subparsers.add_parser("delete", help="Deletes a license")
+delete_argget.add_argument("--license", "-l", type=str, required=True, help="The identifier of the license to delete")
 args = argget.parse_args()
 
 if args.debug:
-    log_file = "rf_licenses-{}.log".format( datetime.datetime.now().strftime( "%Y-%m-%d-%H%M%S" ) )
+    log_file = "rf_licenses-{}.log".format(datetime.datetime.now().strftime("%Y-%m-%d-%H%M%S"))
     log_format = "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
-    logger = redfish.redfish_logger( log_file, log_format, logging.DEBUG )
-    logger.info( "rf_licenses Trace" )
+    logger = redfish.redfish_logger(log_file, log_format, logging.DEBUG)
+    logger.info("rf_licenses Trace")
 
 # Set up the Redfish object
 redfish_obj = None
 try:
-    redfish_obj = redfish.redfish_client( base_url = args.rhost, username = args.user, password = args.password, timeout = 15, max_retry = 3 )
-    redfish_obj.login( auth = "session" )
-except RedfishPasswordChangeRequiredError as e:
-    redfish_utilities.print_password_change_required_and_logout( redfish_obj, args )
-    sys.exit( 1 )
-except Exception as e:
+    redfish_obj = redfish.redfish_client(
+        base_url=args.rhost, username=args.user, password=args.password, timeout=15, max_retry=3
+    )
+    redfish_obj.login(auth="session")
+except RedfishPasswordChangeRequiredError:
+    redfish_utilities.print_password_change_required_and_logout(redfish_obj, args)
+    sys.exit(1)
+except Exception:
     raise
 
 exit_code = 0
 try:
     if args.command == "install":
-        print( "Installing license '{}'...".format( args.license ) )
-        response = redfish_utilities.install_license( redfish_obj, args.license )
-        response = redfish_utilities.poll_task_monitor( redfish_obj, response )
-        redfish_utilities.verify_response( response )
+        print("Installing license '{}'...".format(args.license))
+        response = redfish_utilities.install_license(redfish_obj, args.license)
+        response = redfish_utilities.poll_task_monitor(redfish_obj, response)
+        redfish_utilities.verify_response(response)
     elif args.command == "delete":
-        print( "Deleting license '{}'...".format( args.license ) )
-        response = redfish_utilities.delete_license( redfish_obj, args.license )
-        response = redfish_utilities.poll_task_monitor( redfish_obj, response )
-        redfish_utilities.verify_response( response )
+        print("Deleting license '{}'...".format(args.license))
+        response = redfish_utilities.delete_license(redfish_obj, args.license)
+        response = redfish_utilities.poll_task_monitor(redfish_obj, response)
+        redfish_utilities.verify_response(response)
     else:
-        licenses = redfish_utilities.get_licenses( redfish_obj )
+        licenses = redfish_utilities.get_licenses(redfish_obj)
         if args.command == "info":
-            redfish_utilities.print_licenses( licenses, details = args.details )
+            redfish_utilities.print_licenses(licenses, details=args.details)
         else:
-            redfish_utilities.print_licenses( licenses )
+            redfish_utilities.print_licenses(licenses)
 except Exception as e:
     if args.debug:
-        logger.error( "Caught exception:\n\n{}\n".format( traceback.format_exc() ) )
+        logger.error("Caught exception:\n\n{}\n".format(traceback.format_exc()))
     exit_code = 1
-    print( e )
+    print(e)
 finally:
     # Log out
-    redfish_utilities.logout( redfish_obj )
-sys.exit( exit_code )
+    redfish_utilities.logout(redfish_obj)
+sys.exit(exit_code)
```

### Comparing `redfish_utilities-3.2.8/scripts/rf_logs.py` & `redfish_utilities-3.2.9/scripts/rf_logs.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,76 +14,88 @@
 import argparse
 import datetime
 import logging
 import redfish
 import redfish_utilities
 import traceback
 import sys
+from signal import signal, SIGPIPE, SIG_DFL
 from redfish.messages import RedfishPasswordChangeRequiredError
 
 # Get the input arguments
-argget = argparse.ArgumentParser( description = "A tool to manage logs on a Redfish service" )
-argget.add_argument( "--user", "-u", type = str, required = True, help = "The user name for authentication" )
-argget.add_argument( "--password", "-p",  type = str, required = True, help = "The password for authentication" )
-argget.add_argument( "--rhost", "-r", type = str, required = True, help = "The address of the Redfish service (with scheme)" )
-argget.add_argument( "--manager", "-m", type = str, nargs = "?", default = False, help = "The ID of the manager containing the log service" )
-argget.add_argument( "--system", "-s", type = str, nargs = "?", default = False, help = "The ID of the system containing the log service" )
-argget.add_argument( "--chassis", "-c", type = str, nargs = "?", default = False, help = "The ID of the chassis containing the log service" )
-argget.add_argument( "--log", "-l", type = str, help = "The ID of the resource containing the log service" )
-argget.add_argument( "--details", "-details", action = "store_true", help = "Indicates details to be shown for each log entry" )
-argget.add_argument( "--clear", "-clear", action = "store_true", help = "Indicates if the log should be cleared" )
-argget.add_argument( "--debug", action = "store_true", help = "Creates debug file showing HTTP traces and exceptions" )
+argget = argparse.ArgumentParser(description="A tool to manage logs on a Redfish service")
+argget.add_argument("--user", "-u", type=str, required=True, help="The user name for authentication")
+argget.add_argument("--password", "-p", type=str, required=True, help="The password for authentication")
+argget.add_argument("--rhost", "-r", type=str, required=True, help="The address of the Redfish service (with scheme)")
+argget.add_argument(
+    "--manager", "-m", type=str, nargs="?", default=False, help="The ID of the manager containing the log service"
+)
+argget.add_argument(
+    "--system", "-s", type=str, nargs="?", default=False, help="The ID of the system containing the log service"
+)
+argget.add_argument(
+    "--chassis", "-c", type=str, nargs="?", default=False, help="The ID of the chassis containing the log service"
+)
+argget.add_argument("--log", "-l", type=str, help="The ID of the resource containing the log service")
+argget.add_argument(
+    "--details", "-details", action="store_true", help="Indicates details to be shown for each log entry"
+)
+argget.add_argument("--clear", "-clear", action="store_true", help="Indicates if the log should be cleared")
+argget.add_argument("--debug", action="store_true", help="Creates debug file showing HTTP traces and exceptions")
 args = argget.parse_args()
 
 # Determine the target log service based on the inputs
 # Effectively if the user gives multiple targets, some will be ignored
 container_type = redfish_utilities.log_container.MANAGER
 container_id = None
-if args.manager != False:
+if args.manager is not False:
     container_type = redfish_utilities.log_container.MANAGER
     container_id = args.manager
-elif args.system != False:
+elif args.system is not False:
     container_type = redfish_utilities.log_container.SYSTEM
     container_id = args.system
-elif args.chassis != False:
+elif args.chassis is not False:
     container_type = redfish_utilities.log_container.CHASSIS
     container_id = args.chassis
 
 if args.debug:
-    log_file = "rf_logs-{}.log".format( datetime.datetime.now().strftime( "%Y-%m-%d-%H%M%S" ) )
+    log_file = "rf_logs-{}.log".format(datetime.datetime.now().strftime("%Y-%m-%d-%H%M%S"))
     log_format = "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
-    logger = redfish.redfish_logger( log_file, log_format, logging.DEBUG )
-    logger.info( "rf_logs Trace" )
+    logger = redfish.redfish_logger(log_file, log_format, logging.DEBUG)
+    logger.info("rf_logs Trace")
 
 # Set up the Redfish object
 redfish_obj = None
 try:
-    redfish_obj = redfish.redfish_client( base_url = args.rhost, username = args.user, password = args.password, timeout = 30, max_retry = 3 )
-    redfish_obj.login( auth = "session" )
-except RedfishPasswordChangeRequiredError as e:
-    redfish_utilities.print_password_change_required_and_logout( redfish_obj, args )
-    sys.exit( 1 )
-except Exception as e:
+    redfish_obj = redfish.redfish_client(
+        base_url=args.rhost, username=args.user, password=args.password, timeout=30, max_retry=3
+    )
+    redfish_obj.login(auth="session")
+except RedfishPasswordChangeRequiredError:
+    redfish_utilities.print_password_change_required_and_logout(redfish_obj, args)
+    sys.exit(1)
+except Exception:
     raise
 
 exit_code = 0
 try:
     # Either clear the logs or get/print the logs
     if args.clear:
         # Clear log was requested
-        print( "Clearing the log..." )
-        response = redfish_utilities.clear_log_entries( redfish_obj, container_type, container_id, args.log )
-        response = redfish_utilities.poll_task_monitor( redfish_obj, response )
-        redfish_utilities.verify_response( response )
+        print("Clearing the log...")
+        response = redfish_utilities.clear_log_entries(redfish_obj, container_type, container_id, args.log)
+        response = redfish_utilities.poll_task_monitor(redfish_obj, response)
+        redfish_utilities.verify_response(response)
     else:
         # Print log was requested
-        log_entries = redfish_utilities.get_log_entries( redfish_obj, container_type, container_id, args.log )
-        redfish_utilities.print_log_entries( log_entries, args.details )
+        log_entries = redfish_utilities.get_log_entries(redfish_obj, container_type, container_id, args.log)
+        signal(SIGPIPE, SIG_DFL)
+        redfish_utilities.print_log_entries(log_entries, args.details)
 except Exception as e:
     if args.debug:
-        logger.error( "Caught exception:\n\n{}\n".format( traceback.format_exc() ) )
+        logger.error("Caught exception:\n\n{}\n".format(traceback.format_exc()))
     exit_code = 1
-    print( e )
+    print(e)
 finally:
     # Log out
-    redfish_utilities.logout( redfish_obj )
-sys.exit( exit_code )
+    redfish_utilities.logout(redfish_obj)
+sys.exit(exit_code)
```

### Comparing `redfish_utilities-3.2.8/scripts/rf_manager_config.py` & `redfish_utilities-3.2.9/scripts/rf_manager_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,177 +17,213 @@
 import redfish
 import redfish_utilities
 import traceback
 import sys
 from redfish.messages import RedfishPasswordChangeRequiredError
 
 # Get the input arguments
-argget = argparse.ArgumentParser( description = "A tool to manage managers in a service" )
-argget.add_argument( "--user", "-u", type = str, required = True, help = "The user name for authentication" )
-argget.add_argument( "--password", "-p",  type = str, required = True, help = "The password for authentication" )
-argget.add_argument( "--rhost", "-r", type = str, required = True, help = "The address of the Redfish service (with scheme)" )
-argget.add_argument( "--manager", "-m", type = str, help = "The ID of the manager to target" )
-argget.add_argument( "--debug", action = "store_true", help = "Creates debug file showing HTTP traces and exceptions" )
-subparsers = argget.add_subparsers( dest = "command" )
-info_argget = subparsers.add_parser( "info", help = "Displays information about a manager" )
-reset_argget = subparsers.add_parser( "reset", help = "Resets a manager" )
-reset_argget.add_argument( "--type", "-t", type = str, help = "The type of power/reset operation to perform", choices = redfish_utilities.reset_types )
-reset_argget.add_argument( "--info", "-info", action = "store_true", help = "Indicates if reset information should be reported" )
-getnet_argget = subparsers.add_parser( "getnet", help = "Displays information about an Ethernet interface" )
-getnet_argget.add_argument( "--id", "-i", type = str, help = "The identifier of the Ethernet interface to display" )
-setnet_argget = subparsers.add_parser( "setnet", help = "Configures an Ethernet interface" )
-setnet_argget.add_argument( "--id", "-i", type = str, help = "The identifier of the Ethernet interface to configure" )
-setnet_argget.add_argument( "--ipv4address", "-ipv4address", type = str, help = "The static IPv4 address to set" )
-setnet_argget.add_argument( "--ipv4netmask", "-ipv4netmask", type = str, help = "The static IPv4 subnet mask to set" )
-setnet_argget.add_argument( "--ipv4gateway", "-ipv4gateway", type = str, help = "The static IPv4 gateway to set" )
-setnet_argget.add_argument( "--dhcpv4", "-dhcpv4", type = str, help = "The DHCPv4 configuration to set", choices = [ "On", "Off" ] )
-setnet_argget.add_argument( "--ipv6addresses", "-ipv6addresses", type = str, nargs = '+', help = "The static IPv6 addresses to set with prefix length" )
-setnet_argget.add_argument( "--ipv6gateways", "-ipv6gateways", type = str, nargs = '+', help = "The static IPv6 default gateways to set with prefix length" )
-setnet_argget.add_argument( "--dhcpv6", "-dhcpv6", type = str, help = "The DHCPv6 configuration to set", choices = [ "Stateful", "Stateless", "Disabled", "Enabled" ] )
-setnet_argget.add_argument( "--vlan", "-vlan", type = str, help = "The VLAN enabled configuration to set", choices = [ "On", "Off" ] )
-setnet_argget.add_argument( "--vlanid", "-vlanid", type = int, help = "The VLAN ID to set" )
-setnet_argget.add_argument( "--vlanpriority", "-vlanpriority", type = int, help = "The VLAN priority to set" )
-reset_to_defaults_argget = subparsers.add_parser( "resettodefaults", help = "Resets a manager to default settings" )
-reset_to_defaults_argget.add_argument( "--type", "-t", type = str, help = "The type of reset-to-defaults operation to perform", choices = redfish_utilities.reset_to_defaults_types )
-reset_to_defaults_argget.add_argument( "--info", "-info", action = "store_true", help = "Indicates if reset-to-defaults information should be reported" )
-set_time_argget = subparsers.add_parser( "settime", help = "Sets the date-time on a manager" )
-set_time_argget.add_argument( "--datetime", "-dt", type = str, help = "The date-time value to set" )
-set_time_argget.add_argument( "--offset", "-o", type = str, help = "The date-time offset value to set" )
-getprotocol_argget = subparsers.add_parser( "getprotocol", help = "Displays network protocol information about a manager" )
-setprotocol_argget = subparsers.add_parser( "setprotocol", help = "Configures network protocol settings on a manager" )
-setprotocol_argget.add_argument( "--protocol", "-prot", type = str, required = True, help = "The protocol to set" )
-setprotocol_argget.add_argument( "--enable", "-en", action = "store_true", help = "Enable the selected protocol" )
-setprotocol_argget.add_argument( "--disable", "-dis", action = "store_true", help = "Disable the selected protocol" )
-setprotocol_argget.add_argument( "--port", "-port", type = int, help = "The port number to assign the protocol" )
+argget = argparse.ArgumentParser(description="A tool to manage managers in a service")
+argget.add_argument("--user", "-u", type=str, required=True, help="The user name for authentication")
+argget.add_argument("--password", "-p", type=str, required=True, help="The password for authentication")
+argget.add_argument("--rhost", "-r", type=str, required=True, help="The address of the Redfish service (with scheme)")
+argget.add_argument("--manager", "-m", type=str, help="The ID of the manager to target")
+argget.add_argument("--debug", action="store_true", help="Creates debug file showing HTTP traces and exceptions")
+subparsers = argget.add_subparsers(dest="command")
+info_argget = subparsers.add_parser("info", help="Displays information about a manager")
+reset_argget = subparsers.add_parser("reset", help="Resets a manager")
+reset_argget.add_argument(
+    "--type", "-t", type=str, help="The type of power/reset operation to perform", choices=redfish_utilities.reset_types
+)
+reset_argget.add_argument(
+    "--info", "-info", action="store_true", help="Indicates if reset information should be reported"
+)
+getnet_argget = subparsers.add_parser("getnet", help="Displays information about an Ethernet interface")
+getnet_argget.add_argument("--id", "-i", type=str, help="The identifier of the Ethernet interface to display")
+setnet_argget = subparsers.add_parser("setnet", help="Configures an Ethernet interface")
+setnet_argget.add_argument("--id", "-i", type=str, help="The identifier of the Ethernet interface to configure")
+setnet_argget.add_argument("--ipv4address", "-ipv4address", type=str, help="The static IPv4 address to set")
+setnet_argget.add_argument("--ipv4netmask", "-ipv4netmask", type=str, help="The static IPv4 subnet mask to set")
+setnet_argget.add_argument("--ipv4gateway", "-ipv4gateway", type=str, help="The static IPv4 gateway to set")
+setnet_argget.add_argument(
+    "--dhcpv4", "-dhcpv4", type=str, help="The DHCPv4 configuration to set", choices=["On", "Off"]
+)
+setnet_argget.add_argument(
+    "--ipv6addresses", "-ipv6addresses", type=str, nargs="+", help="The static IPv6 addresses to set with prefix length"
+)
+setnet_argget.add_argument(
+    "--ipv6gateways",
+    "-ipv6gateways",
+    type=str,
+    nargs="+",
+    help="The static IPv6 default gateways to set with prefix length",
+)
+setnet_argget.add_argument(
+    "--dhcpv6",
+    "-dhcpv6",
+    type=str,
+    help="The DHCPv6 configuration to set",
+    choices=["Stateful", "Stateless", "Disabled", "Enabled"],
+)
+setnet_argget.add_argument(
+    "--vlan", "-vlan", type=str, help="The VLAN enabled configuration to set", choices=["On", "Off"]
+)
+setnet_argget.add_argument("--vlanid", "-vlanid", type=int, help="The VLAN ID to set")
+setnet_argget.add_argument("--vlanpriority", "-vlanpriority", type=int, help="The VLAN priority to set")
+reset_to_defaults_argget = subparsers.add_parser("resettodefaults", help="Resets a manager to default settings")
+reset_to_defaults_argget.add_argument(
+    "--type",
+    "-t",
+    type=str,
+    help="The type of reset-to-defaults operation to perform",
+    choices=redfish_utilities.reset_to_defaults_types,
+)
+reset_to_defaults_argget.add_argument(
+    "--info", "-info", action="store_true", help="Indicates if reset-to-defaults information should be reported"
+)
+set_time_argget = subparsers.add_parser("settime", help="Sets the date-time on a manager")
+set_time_argget.add_argument("--datetime", "-dt", type=str, help="The date-time value to set")
+set_time_argget.add_argument("--offset", "-o", type=str, help="The date-time offset value to set")
+getprotocol_argget = subparsers.add_parser("getprotocol", help="Displays network protocol information about a manager")
+setprotocol_argget = subparsers.add_parser("setprotocol", help="Configures network protocol settings on a manager")
+setprotocol_argget.add_argument("--protocol", "-prot", type=str, required=True, help="The protocol to set")
+setprotocol_argget.add_argument("--enable", "-en", action="store_true", help="Enable the selected protocol")
+setprotocol_argget.add_argument("--disable", "-dis", action="store_true", help="Disable the selected protocol")
+setprotocol_argget.add_argument("--port", "-port", type=int, help="The port number to assign the protocol")
 args = argget.parse_args()
 
 if args.debug:
-    log_file = "rf_manager_config-{}.log".format( datetime.datetime.now().strftime( "%Y-%m-%d-%H%M%S" ) )
+    log_file = "rf_manager_config-{}.log".format(datetime.datetime.now().strftime("%Y-%m-%d-%H%M%S"))
     log_format = "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
-    logger = redfish.redfish_logger( log_file, log_format, logging.DEBUG )
-    logger.info( "rf_manager_config Trace" )
+    logger = redfish.redfish_logger(log_file, log_format, logging.DEBUG)
+    logger.info("rf_manager_config Trace")
 
 # Set up the Redfish object
 redfish_obj = None
 try:
-    redfish_obj = redfish.redfish_client( base_url = args.rhost, username = args.user, password = args.password, timeout = 15, max_retry = 3 )
-    redfish_obj.login( auth = "session" )
-except RedfishPasswordChangeRequiredError as e:
-    redfish_utilities.print_password_change_required_and_logout( redfish_obj, args )
-    sys.exit( 1 )
-except Exception as e:
+    redfish_obj = redfish.redfish_client(
+        base_url=args.rhost, username=args.user, password=args.password, timeout=15, max_retry=3
+    )
+    redfish_obj.login(auth="session")
+except RedfishPasswordChangeRequiredError:
+    redfish_utilities.print_password_change_required_and_logout(redfish_obj, args)
+    sys.exit(1)
+except Exception:
     raise
 
 exit_code = 0
 try:
     if args.command == "reset":
         if args.info:
-            reset_uri, reset_parameters = redfish_utilities.get_manager_reset_info( redfish_obj, args.manager )
+            reset_uri, reset_parameters = redfish_utilities.get_manager_reset_info(redfish_obj, args.manager)
             printed_reset_types = False
             for param in reset_parameters:
                 if param["Name"] == "ResetType" and "AllowableValues" in param:
-                    print( "Supported reset types: {}".format( ", ".join( param["AllowableValues"] ) ) )
+                    print("Supported reset types: {}".format(", ".join(param["AllowableValues"])))
                     printed_reset_types = True
             if not printed_reset_types:
-                print( "No reset information found" )
+                print("No reset information found")
         else:
-            print( "Resetting the manager..." )
-            response = redfish_utilities.manager_reset( redfish_obj, args.manager, args.type )
-            response = redfish_utilities.poll_task_monitor( redfish_obj, response )
-            redfish_utilities.verify_response( response )
+            print("Resetting the manager...")
+            response = redfish_utilities.manager_reset(redfish_obj, args.manager, args.type)
+            response = redfish_utilities.poll_task_monitor(redfish_obj, response)
+            redfish_utilities.verify_response(response)
     elif args.command == "resettodefaults":
         if args.info:
-            reset_uri, reset_parameters = redfish_utilities.get_manager_reset_to_defaults_info( redfish_obj, args.manager )
+            reset_uri, reset_parameters = redfish_utilities.get_manager_reset_to_defaults_info(
+                redfish_obj, args.manager
+            )
             printed_reset_types = False
             for param in reset_parameters:
                 if param["Name"] == "ResetType" and "AllowableValues" in param:
-                    print( "Supported reset types: {}".format( ", ".join( param["AllowableValues"] ) ) )
+                    print("Supported reset types: {}".format(", ".join(param["AllowableValues"])))
                     printed_reset_types = True
             if not printed_reset_types:
-                print( "No reset information found" )
+                print("No reset information found")
         else:
-            print( "Resetting the manager to defaults..." )
-            response = redfish_utilities.manager_reset_to_defaults( redfish_obj, args.manager, args.type )
-            response = redfish_utilities.poll_task_monitor( redfish_obj, response )
-            redfish_utilities.verify_response( response )
+            print("Resetting the manager to defaults...")
+            response = redfish_utilities.manager_reset_to_defaults(redfish_obj, args.manager, args.type)
+            response = redfish_utilities.poll_task_monitor(redfish_obj, response)
+            redfish_utilities.verify_response(response)
     elif args.command == "settime":
-        redfish_utilities.set_manager( redfish_obj, args.manager, args.datetime, args.offset )
+        redfish_utilities.set_manager(redfish_obj, args.manager, args.datetime, args.offset)
     elif args.command == "getnet":
-        interface = redfish_utilities.get_manager_ethernet_interface( redfish_obj, args.manager, args.id )
-        redfish_utilities.print_manager_ethernet_interface( interface )
+        interface = redfish_utilities.get_manager_ethernet_interface(redfish_obj, args.manager, args.id)
+        redfish_utilities.print_manager_ethernet_interface(interface)
     elif args.command == "setnet":
         vlan = {}
         if args.vlan == "On":
             vlan["VLANEnable"] = True
         elif args.vlan == "Off":
             vlan["VLANEnable"] = False
         if args.vlanid is not None:
             vlan["VLANId"] = args.vlanid
         if args.vlanpriority is not None:
             vlan["VLANPriority"] = args.vlanpriority
-        if len( vlan ) == 0:
+        if len(vlan) == 0:
             vlan = None
-        ipv4_addresses = [ {} ]
+        ipv4_addresses = [{}]
         if args.ipv4address is not None:
             ipv4_addresses[0]["Address"] = args.ipv4address
         if args.ipv4netmask is not None:
             ipv4_addresses[0]["SubnetMask"] = args.ipv4netmask
         if args.ipv4gateway is not None:
             ipv4_addresses[0]["Gateway"] = args.ipv4gateway
-        if len( ipv4_addresses[0] ) == 0:
+        if len(ipv4_addresses[0]) == 0:
             ipv4_addresses = None
         dhcpv4 = None
         if args.dhcpv4 == "On":
-            dhcpv4 = { "DHCPEnabled": True }
+            dhcpv4 = {"DHCPEnabled": True}
         elif args.dhcpv4 == "Off":
-            dhcpv4 = { "DHCPEnabled": False }
+            dhcpv4 = {"DHCPEnabled": False}
         dhcpv6 = None
         ipv6_addresses = None
         if args.ipv6addresses is not None:
             ipv6_addresses = []
             for address in args.ipv6addresses:
                 if address == "None":
-                    ipv6_addresses.append( None )
+                    ipv6_addresses.append(None)
                 elif address == "{}":
-                    ipv6_addresses.append( {} )
+                    ipv6_addresses.append({})
                 else:
-                    ipv6_addresses.append( { "Address": address.split( "/" )[0], "PrefixLength": int( address.split( "/" )[1] ) } )
+                    ipv6_addresses.append(
+                        {"Address": address.split("/")[0], "PrefixLength": int(address.split("/")[1])}
+                    )
         ipv6_gateways = None
         if args.ipv6gateways is not None:
             ipv6_gateways = []
             for address in args.ipv6gateways:
                 if address == "None":
-                    ipv6_gateways.append( None )
+                    ipv6_gateways.append(None)
                 elif address == "{}":
-                    ipv6_gateways.append( {} )
+                    ipv6_gateways.append({})
                 else:
-                    ipv6_gateways.append( { "Address": address.split( "/" )[0], "PrefixLength": int( address.split( "/" )[1] ) } )
+                    ipv6_gateways.append({"Address": address.split("/")[0], "PrefixLength": int(address.split("/")[1])})
         if args.dhcpv6 is not None:
-            dhcpv6 = { "OperatingMode": args.dhcpv6 }
-        redfish_utilities.set_manager_ethernet_interface( redfish_obj, args.manager, args.id, vlan, ipv4_addresses, dhcpv4, ipv6_addresses, ipv6_gateways, dhcpv6 )
+            dhcpv6 = {"OperatingMode": args.dhcpv6}
+        redfish_utilities.set_manager_ethernet_interface(
+            redfish_obj, args.manager, args.id, vlan, ipv4_addresses, dhcpv4, ipv6_addresses, ipv6_gateways, dhcpv6
+        )
     elif args.command == "getprotocol":
-        network_protocol = redfish_utilities.get_manager_network_protocol( redfish_obj, args.manager )
-        redfish_utilities.print_manager_network_protocol( network_protocol )
+        network_protocol = redfish_utilities.get_manager_network_protocol(redfish_obj, args.manager)
+        redfish_utilities.print_manager_network_protocol(network_protocol)
     elif args.command == "setprotocol":
-        network_protocol_setting = {
-            args.protocol: {}
-        }
+        network_protocol_setting = {args.protocol: {}}
         if args.enable:
             network_protocol_setting[args.protocol]["ProtocolEnabled"] = True
         elif args.disable:
             network_protocol_setting[args.protocol]["ProtocolEnabled"] = False
         if args.port:
             network_protocol_setting[args.protocol]["Port"] = args.port
-        print( "Configuring {}...".format( args.protocol ) )
-        redfish_utilities.set_manager_network_protocol( redfish_obj, args.manager, network_protocol_setting )
+        print("Configuring {}...".format(args.protocol))
+        redfish_utilities.set_manager_network_protocol(redfish_obj, args.manager, network_protocol_setting)
     else:
-        manager = redfish_utilities.get_manager( redfish_obj, args.manager )
-        redfish_utilities.print_manager( manager )
+        manager = redfish_utilities.get_manager(redfish_obj, args.manager)
+        redfish_utilities.print_manager(manager)
 except Exception as e:
     if args.debug:
-        logger.error( "Caught exception:\n\n{}\n".format( traceback.format_exc() ) )
+        logger.error("Caught exception:\n\n{}\n".format(traceback.format_exc()))
     exit_code = 1
-    print( e )
+    print(e)
 finally:
     # Log out
-    redfish_utilities.logout( redfish_obj )
-sys.exit( exit_code )
+    redfish_utilities.logout(redfish_obj)
+sys.exit(exit_code)
```

### Comparing `redfish_utilities-3.2.8/scripts/rf_power_equipment.py` & `redfish_utilities-3.2.9/scripts/rf_power_equipment.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,85 +17,160 @@
 import redfish
 import redfish_utilities
 import traceback
 import sys
 from redfish.messages import RedfishPasswordChangeRequiredError
 
 # Get the input arguments
-argget = argparse.ArgumentParser( description = "A tool to manage power equipment" )
-argget.add_argument( "--user", "-u", type = str, required = True, help = "The user name for authentication" )
-argget.add_argument( "--password", "-p",  type = str, required = True, help = "The password for authentication" )
-argget.add_argument( "--rhost", "-r", type = str, required = True, help = "The address of the Redfish service (with scheme)" )
-argget.add_argument( "--debug", action = "store_true", help = "Creates debug file showing HTTP traces and exceptions" )
-subparsers = argget.add_subparsers( dest = "command" )
-list_argget = subparsers.add_parser( "list", help = "Displays a list of the available power equipment" )
-status_argget = subparsers.add_parser( "status", help = "Displays the status of an instance of power equipment" )
-status_argget.add_argument( "--type", "-t", type = redfish_utilities.power_equipment_types, required = True, help = "The type of power equipment to get", choices = redfish_utilities.power_equipment_types )
-status_argget.add_argument( "--equipment", "-pe", type = str, help = "The identifier of the power equipment to get" )
-outletsummary_argget = subparsers.add_parser( "outlets", help = "Displays the outlet summary of an instance of power equipment" )
-outletsummary_argget.add_argument( "--type", "-t", type = redfish_utilities.power_equipment_types, required = True, help = "The type of power equipment to get", choices = redfish_utilities.power_equipment_types )
-outletsummary_argget.add_argument( "--equipment", "-pe", type = str, help = "The identifier of the power equipment to get" )
-outlet_info_argget = subparsers.add_parser( "outletinfo", help = "Displays the status of an outlet for an instance of power equipment" )
-outlet_info_argget.add_argument( "--type", "-t", type = redfish_utilities.power_equipment_types, required = True, help = "The type of power equipment to get", choices = redfish_utilities.power_equipment_types )
-outlet_info_argget.add_argument( "--equipment", "-pe", type = str, help = "The identifier of the power equipment to get" )
-outlet_info_argget.add_argument( "--outlet", "-o", type = str, help = "The identifier of the outlet to get" )
-mains_info_argget = subparsers.add_parser( "mainsinfo", help = "Displays the status of a mains circuit for an instance of power equipment" )
-mains_info_argget.add_argument( "--type", "-t", type = redfish_utilities.power_equipment_types, required = True, help = "The type of power equipment to get", choices = redfish_utilities.power_equipment_types )
-mains_info_argget.add_argument( "--equipment", "-pe", type = str, help = "The identifier of the power equipment to get" )
-mains_info_argget.add_argument( "--mains", "-m", type = str, help = "The identifier of the mains circuit to get" )
-branch_info_argget = subparsers.add_parser( "branchinfo", help = "Displays the status of a branch circuit for an instance of power equipment" )
-branch_info_argget.add_argument( "--type", "-t", type = redfish_utilities.power_equipment_types, required = True, help = "The type of power equipment to get", choices = redfish_utilities.power_equipment_types )
-branch_info_argget.add_argument( "--equipment", "-pe", type = str, help = "The identifier of the power equipment to get" )
-branch_info_argget.add_argument( "--branch", "-b", type = str, help = "The identifier of the branch circuit to get" )
+argget = argparse.ArgumentParser(description="A tool to manage power equipment")
+argget.add_argument("--user", "-u", type=str, required=True, help="The user name for authentication")
+argget.add_argument("--password", "-p", type=str, required=True, help="The password for authentication")
+argget.add_argument("--rhost", "-r", type=str, required=True, help="The address of the Redfish service (with scheme)")
+argget.add_argument("--debug", action="store_true", help="Creates debug file showing HTTP traces and exceptions")
+subparsers = argget.add_subparsers(dest="command")
+list_argget = subparsers.add_parser("list", help="Displays a list of the available power equipment")
+status_argget = subparsers.add_parser("status", help="Displays the status of an instance of power equipment")
+status_argget.add_argument(
+    "--type",
+    "-t",
+    type=redfish_utilities.power_equipment_types,
+    required=True,
+    help="The type of power equipment to get",
+    choices=redfish_utilities.power_equipment_types,
+)
+status_argget.add_argument("--equipment", "-pe", type=str, help="The identifier of the power equipment to get")
+outletsummary_argget = subparsers.add_parser(
+    "outlets", help="Displays the outlet summary of an instance of power equipment"
+)
+outletsummary_argget.add_argument(
+    "--type",
+    "-t",
+    type=redfish_utilities.power_equipment_types,
+    required=True,
+    help="The type of power equipment to get",
+    choices=redfish_utilities.power_equipment_types,
+)
+outletsummary_argget.add_argument("--equipment", "-pe", type=str, help="The identifier of the power equipment to get")
+outlet_info_argget = subparsers.add_parser(
+    "outletinfo", help="Displays the status of an outlet for an instance of power equipment"
+)
+outlet_info_argget.add_argument(
+    "--type",
+    "-t",
+    type=redfish_utilities.power_equipment_types,
+    required=True,
+    help="The type of power equipment to get",
+    choices=redfish_utilities.power_equipment_types,
+)
+outlet_info_argget.add_argument("--equipment", "-pe", type=str, help="The identifier of the power equipment to get")
+outlet_info_argget.add_argument("--outlet", "-o", type=str, help="The identifier of the outlet to get")
+mains_info_argget = subparsers.add_parser(
+    "mainsinfo", help="Displays the status of a mains circuit for an instance of power equipment"
+)
+mains_info_argget.add_argument(
+    "--type",
+    "-t",
+    type=redfish_utilities.power_equipment_types,
+    required=True,
+    help="The type of power equipment to get",
+    choices=redfish_utilities.power_equipment_types,
+)
+mains_info_argget.add_argument("--equipment", "-pe", type=str, help="The identifier of the power equipment to get")
+mains_info_argget.add_argument("--mains", "-m", type=str, help="The identifier of the mains circuit to get")
+branch_info_argget = subparsers.add_parser(
+    "branchinfo", help="Displays the status of a branch circuit for an instance of power equipment"
+)
+branch_info_argget.add_argument(
+    "--type",
+    "-t",
+    type=redfish_utilities.power_equipment_types,
+    required=True,
+    help="The type of power equipment to get",
+    choices=redfish_utilities.power_equipment_types,
+)
+branch_info_argget.add_argument("--equipment", "-pe", type=str, help="The identifier of the power equipment to get")
+branch_info_argget.add_argument("--branch", "-b", type=str, help="The identifier of the branch circuit to get")
 args = argget.parse_args()
 
 if args.debug:
-    log_file = "rf_power_equipment-{}.log".format( datetime.datetime.now().strftime( "%Y-%m-%d-%H%M%S" ) )
+    log_file = "rf_power_equipment-{}.log".format(datetime.datetime.now().strftime("%Y-%m-%d-%H%M%S"))
     log_format = "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
-    logger = redfish.redfish_logger( log_file, log_format, logging.DEBUG )
-    logger.info( "rf_power_equipment Trace" )
+    logger = redfish.redfish_logger(log_file, log_format, logging.DEBUG)
+    logger.info("rf_power_equipment Trace")
 
 # Set up the Redfish object
 redfish_obj = None
 try:
-    redfish_obj = redfish.redfish_client( base_url = args.rhost, username = args.user, password = args.password, timeout = 15, max_retry = 3 )
-    redfish_obj.login( auth = "session" )
-except RedfishPasswordChangeRequiredError as e:
-    redfish_utilities.print_password_change_required_and_logout( redfish_obj, args )
-    sys.exit( 1 )
-except Exception as e:
+    redfish_obj = redfish.redfish_client(
+        base_url=args.rhost, username=args.user, password=args.password, timeout=15, max_retry=3
+    )
+    redfish_obj.login(auth="session")
+except RedfishPasswordChangeRequiredError:
+    redfish_utilities.print_password_change_required_and_logout(redfish_obj, args)
+    sys.exit(1)
+except Exception:
     raise
 
 exit_code = 0
 try:
     if args.command == "status":
-        power_equipment = redfish_utilities.get_power_equipment( redfish_obj, args.type, args.equipment, get_metrics = True,
-            get_mains = True, get_branches = True, get_feeders = True, get_subfeeds = True )
-        redfish_utilities.print_power_equipment( power_equipment )
-        circuit_types = [ redfish_utilities.power_equipment_electrical_types.MAINS, redfish_utilities.power_equipment_electrical_types.BRANCH,
-            redfish_utilities.power_equipment_electrical_types.FEEDER, redfish_utilities.power_equipment_electrical_types.SUBFEED ]
+        power_equipment = redfish_utilities.get_power_equipment(
+            redfish_obj,
+            args.type,
+            args.equipment,
+            get_metrics=True,
+            get_mains=True,
+            get_branches=True,
+            get_feeders=True,
+            get_subfeeds=True,
+        )
+        redfish_utilities.print_power_equipment(power_equipment)
+        circuit_types = [
+            redfish_utilities.power_equipment_electrical_types.MAINS,
+            redfish_utilities.power_equipment_electrical_types.BRANCH,
+            redfish_utilities.power_equipment_electrical_types.FEEDER,
+            redfish_utilities.power_equipment_electrical_types.SUBFEED,
+        ]
         for circuit_type in circuit_types:
-            redfish_utilities.print_power_equipment_electrical_summary( power_equipment, circuit_type, False )
+            redfish_utilities.print_power_equipment_electrical_summary(power_equipment, circuit_type, False)
     elif args.command == "outlets":
-        power_equipment = redfish_utilities.get_power_equipment( redfish_obj, args.type, args.equipment, get_outlets = True )
-        redfish_utilities.print_power_equipment_electrical_summary( power_equipment, redfish_utilities.power_equipment_electrical_types.OUTLET, True )
+        power_equipment = redfish_utilities.get_power_equipment(
+            redfish_obj, args.type, args.equipment, get_outlets=True
+        )
+        redfish_utilities.print_power_equipment_electrical_summary(
+            power_equipment, redfish_utilities.power_equipment_electrical_types.OUTLET, True
+        )
     elif args.command == "outletinfo":
-        outlet = redfish_utilities.get_power_equipment_electrical( redfish_obj, args.type, redfish_utilities.power_equipment_electrical_types.OUTLET, args.equipment, args.outlet )
-        redfish_utilities.print_power_equipment_electrical( outlet )
+        outlet = redfish_utilities.get_power_equipment_electrical(
+            redfish_obj,
+            args.type,
+            redfish_utilities.power_equipment_electrical_types.OUTLET,
+            args.equipment,
+            args.outlet,
+        )
+        redfish_utilities.print_power_equipment_electrical(outlet)
     elif args.command == "mainsinfo":
-        mains = redfish_utilities.get_power_equipment_electrical( redfish_obj, args.type, redfish_utilities.power_equipment_electrical_types.MAINS, args.equipment, args.mains )
-        redfish_utilities.print_power_equipment_electrical( mains )
+        mains = redfish_utilities.get_power_equipment_electrical(
+            redfish_obj, args.type, redfish_utilities.power_equipment_electrical_types.MAINS, args.equipment, args.mains
+        )
+        redfish_utilities.print_power_equipment_electrical(mains)
     elif args.command == "branchinfo":
-        mains = redfish_utilities.get_power_equipment_electrical( redfish_obj, args.type, redfish_utilities.power_equipment_electrical_types.BRANCH, args.equipment, args.branch )
-        redfish_utilities.print_power_equipment_electrical( mains )
+        mains = redfish_utilities.get_power_equipment_electrical(
+            redfish_obj,
+            args.type,
+            redfish_utilities.power_equipment_electrical_types.BRANCH,
+            args.equipment,
+            args.branch,
+        )
+        redfish_utilities.print_power_equipment_electrical(mains)
     else:
-        power_equipment = redfish_utilities.get_power_equipment_summary( redfish_obj )
-        redfish_utilities.print_power_equipment_summary( power_equipment )
+        power_equipment = redfish_utilities.get_power_equipment_summary(redfish_obj)
+        redfish_utilities.print_power_equipment_summary(power_equipment)
 except Exception as e:
     if args.debug:
-        logger.error( "Caught exception:\n\n{}\n".format( traceback.format_exc() ) )
+        logger.error("Caught exception:\n\n{}\n".format(traceback.format_exc()))
     exit_code = 1
-    print( e )
+    print(e)
 finally:
     # Log out
-    redfish_utilities.logout( redfish_obj )
-sys.exit( exit_code )
+    redfish_utilities.logout(redfish_obj)
+sys.exit(exit_code)
```

### Comparing `redfish_utilities-3.2.8/scripts/rf_power_reset.py` & `redfish_utilities-3.2.9/scripts/rf_power_reset.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,64 +17,70 @@
 import redfish
 import redfish_utilities
 import traceback
 import sys
 from redfish.messages import RedfishPasswordChangeRequiredError
 
 # Get the input arguments
-argget = argparse.ArgumentParser( description = "A tool to perform a power/reset operation of a system" )
-argget.add_argument( "--user", "-u", type = str, required = True, help = "The user name for authentication" )
-argget.add_argument( "--password", "-p",  type = str, required = True, help = "The password for authentication" )
-argget.add_argument( "--rhost", "-r", type = str, required = True, help = "The address of the Redfish service (with scheme)" )
-argget.add_argument( "--system", "-s", type = str, help = "The ID of the system to reset" )
-argget.add_argument( "--type", "-t", type = str, help = "The type of power/reset operation to perform", choices = redfish_utilities.reset_types )
-argget.add_argument( "--info", "-info", action = "store_true", help = "Indicates if reset and power information should be reported" )
-argget.add_argument( "--debug", action = "store_true", help = "Creates debug file showing HTTP traces and exceptions" )
+argget = argparse.ArgumentParser(description="A tool to perform a power/reset operation of a system")
+argget.add_argument("--user", "-u", type=str, required=True, help="The user name for authentication")
+argget.add_argument("--password", "-p", type=str, required=True, help="The password for authentication")
+argget.add_argument("--rhost", "-r", type=str, required=True, help="The address of the Redfish service (with scheme)")
+argget.add_argument("--system", "-s", type=str, help="The ID of the system to reset")
+argget.add_argument(
+    "--type", "-t", type=str, help="The type of power/reset operation to perform", choices=redfish_utilities.reset_types
+)
+argget.add_argument(
+    "--info", "-info", action="store_true", help="Indicates if reset and power information should be reported"
+)
+argget.add_argument("--debug", action="store_true", help="Creates debug file showing HTTP traces and exceptions")
 args = argget.parse_args()
 
 if args.debug:
-    log_file = "rf_power_reset-{}.log".format( datetime.datetime.now().strftime( "%Y-%m-%d-%H%M%S" ) )
+    log_file = "rf_power_reset-{}.log".format(datetime.datetime.now().strftime("%Y-%m-%d-%H%M%S"))
     log_format = "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
-    logger = redfish.redfish_logger( log_file, log_format, logging.DEBUG )
-    logger.info( "rf_power_reset Trace" )
+    logger = redfish.redfish_logger(log_file, log_format, logging.DEBUG)
+    logger.info("rf_power_reset Trace")
 
 # Set up the Redfish object
 redfish_obj = None
 try:
-    redfish_obj = redfish.redfish_client( base_url = args.rhost, username = args.user, password = args.password, timeout = 15, max_retry = 3 )
-    redfish_obj.login( auth = "session" )
-except RedfishPasswordChangeRequiredError as e:
-    redfish_utilities.print_password_change_required_and_logout( redfish_obj, args )
-    sys.exit( 1 )
-except Exception as e:
+    redfish_obj = redfish.redfish_client(
+        base_url=args.rhost, username=args.user, password=args.password, timeout=15, max_retry=3
+    )
+    redfish_obj.login(auth="session")
+except RedfishPasswordChangeRequiredError:
+    redfish_utilities.print_password_change_required_and_logout(redfish_obj, args)
+    sys.exit(1)
+except Exception:
     raise
 
 exit_code = 0
 try:
     if args.info:
-        system_info = redfish_utilities.get_system( redfish_obj, args.system )
-        reset_uri, reset_parameters = redfish_utilities.get_system_reset_info( redfish_obj, args.system, system_info )
+        system_info = redfish_utilities.get_system(redfish_obj, args.system)
+        reset_uri, reset_parameters = redfish_utilities.get_system_reset_info(redfish_obj, args.system, system_info)
         printed_reset_types = False
         for param in reset_parameters:
             if param["Name"] == "ResetType" and "AllowableValues" in param:
-                print( "Supported reset types: {}".format( ", ".join( param["AllowableValues"] ) ) )
+                print("Supported reset types: {}".format(", ".join(param["AllowableValues"])))
                 printed_reset_types = True
         if not printed_reset_types:
-            print( "No reset information found" )
+            print("No reset information found")
         if "PowerState" in system_info.dict:
-            print( "Current power state: {}".format( system_info.dict["PowerState"] ) )
+            print("Current power state: {}".format(system_info.dict["PowerState"]))
         else:
-            print( "No power state information found" )
+            print("No power state information found")
     else:
-        print( "Resetting the system..." )
-        response = redfish_utilities.system_reset( redfish_obj, args.system, args.type )
-        response = redfish_utilities.poll_task_monitor( redfish_obj, response )
-        redfish_utilities.verify_response( response )
+        print("Resetting the system...")
+        response = redfish_utilities.system_reset(redfish_obj, args.system, args.type)
+        response = redfish_utilities.poll_task_monitor(redfish_obj, response)
+        redfish_utilities.verify_response(response)
 except Exception as e:
     if args.debug:
-        logger.error( "Caught exception:\n\n{}\n".format( traceback.format_exc() ) )
+        logger.error("Caught exception:\n\n{}\n".format(traceback.format_exc()))
     exit_code = 1
-    print( e )
+    print(e)
 finally:
     # Log out
-    redfish_utilities.logout( redfish_obj )
-sys.exit( exit_code )
+    redfish_utilities.logout(redfish_obj)
+sys.exit(exit_code)
```

### Comparing `redfish_utilities-3.2.8/scripts/rf_raw_request.py` & `redfish_utilities-3.2.9/scripts/rf_raw_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
 import argparse
 import json
 import os
 import redfish
 import redfish_utilities
 import sys
-import re
 from redfish.messages import RedfishPasswordChangeRequiredError
 
-def ifmatch_header( redfish_obj, path, headers = None ):
+
+def ifmatch_header(redfish_obj, path, headers=None):
     """
     Generates If-Match header for PATCH and PUT operations
 
     Args:
         redfish_obj: The Redfish client object with an open session
         path: The URI of the resource
         headers: Dictionary of HTTP headers to provide in the request
@@ -32,89 +32,112 @@
     Returns:
         Updated dictionary of HTTP headers with If-Match, if an ETag was found
     """
 
     if headers is None:
         headers = {}
     try:
-        response = redfish_obj.get( path )
-        etag = response.getheader( "ETag" )
+        response = redfish_obj.get(path)
+        etag = response.getheader("ETag")
         if etag is not None:
             headers["If-Match"] = etag
     except Exception:
         pass
     return headers
 
+
 # Get the input arguments
-argget = argparse.ArgumentParser( description = "A tool perform a raw request to a Redfish service" )
-argget.add_argument( "--user", "-u", type = str, required = True, help = "The user name for authentication" )
-argget.add_argument( "--password", "-p",  type = str, required = True, help = "The password for authentication" )
-argget.add_argument( "--rhost", "-r", type = str, required = True, help = "The address of the Redfish service (with scheme)" )
-argget.add_argument( "--method", "-m", type = str, required = False, help = "The HTTP method to perform; performs GET if not specified", default = "GET", choices = [ "GET", "HEAD", "POST", "PATCH", "PUT", "DELETE" ] )
-argget.add_argument( "--request", "-req", type = str, required = True, help = "The URI for the request" )
-argget.add_argument( "--body", "-b", type = str, required = False, help = "The body to provide with the request; can be a JSON string for a JSON request, a filename to send binary data, or an unstructured string" )
-argget.add_argument( "--verbose", "-v", action = "store_true", help = "Indicates if HTTP response codes and headers are displayed", default = False )
+argget = argparse.ArgumentParser(description="A tool perform a raw request to a Redfish service")
+argget.add_argument("--user", "-u", type=str, required=True, help="The user name for authentication")
+argget.add_argument("--password", "-p", type=str, required=True, help="The password for authentication")
+argget.add_argument("--rhost", "-r", type=str, required=True, help="The address of the Redfish service (with scheme)")
+argget.add_argument(
+    "--method",
+    "-m",
+    type=str,
+    required=False,
+    help="The HTTP method to perform; performs GET if not specified",
+    default="GET",
+    choices=["GET", "HEAD", "POST", "PATCH", "PUT", "DELETE"],
+)
+argget.add_argument("--request", "-req", type=str, required=True, help="The URI for the request")
+argget.add_argument(
+    "--body",
+    "-b",
+    type=str,
+    required=False,
+    help="The body to provide with the request; can be a JSON string for a JSON request, a filename to send binary data, or an unstructured string",
+)
+argget.add_argument(
+    "--verbose",
+    "-v",
+    action="store_true",
+    help="Indicates if HTTP response codes and headers are displayed",
+    default=False,
+)
 args = argget.parse_args()
 
 # Connect to the service
 redfish_obj = None
 try:
-    redfish_obj = redfish.redfish_client( base_url = args.rhost, username = args.user, password = args.password, timeout = 15, max_retry = 3 )
-    redfish_obj.login( auth = "session" )
-except RedfishPasswordChangeRequiredError as e:
-    redfish_utilities.print_password_change_required_and_logout( redfish_obj, args )
-    sys.exit( 1 )
-except Exception as e:
+    redfish_obj = redfish.redfish_client(
+        base_url=args.rhost, username=args.user, password=args.password, timeout=15, max_retry=3
+    )
+    redfish_obj.login(auth="session")
+except RedfishPasswordChangeRequiredError:
+    redfish_utilities.print_password_change_required_and_logout(redfish_obj, args)
+    sys.exit(1)
+except Exception:
     raise
 
 # Encode the body
 # If the body argument points to a file, load the file
-if args.body is not None and os.path.isfile( args.body ):
-    with open( args.body, mode="rb" ) as file:
+if args.body is not None and os.path.isfile(args.body):
+    with open(args.body, mode="rb") as file:
         body = file.read()
 else:
     # Not a file; either JSON or a raw string
     try:
-        body = json.loads( args.body )
-    except:
+        body = json.loads(args.body)
+    except Exception:
         body = args.body
 if body is None:
     # Default case if nothing resolves (empty JSON object)
     body = {}
 
 headers = {}
 # Perform the requested operation
 if args.method == "HEAD":
-    resp = redfish_obj.head( args.request )
+    resp = redfish_obj.head(args.request)
 elif args.method == "POST":
-    resp = redfish_obj.post( args.request, body = body )
+    resp = redfish_obj.post(args.request, body=body)
 elif args.method == "PATCH":
-    headers = ifmatch_header( redfish_obj, args.request, headers = headers )
-    resp = redfish_obj.patch( args.request, body = body, headers = headers )
+    headers = ifmatch_header(redfish_obj, args.request, headers=headers)
+    resp = redfish_obj.patch(args.request, body=body, headers=headers)
 elif args.method == "PUT":
-    headers = ifmatch_header( redfish_obj, args.request, headers = headers )
-    resp = redfish_obj.put( args.request, body = body, headers = headers )
+    headers = ifmatch_header(redfish_obj, args.request, headers=headers)
+    resp = redfish_obj.put(args.request, body=body, headers=headers)
 elif args.method == "DELETE":
-    resp = redfish_obj.delete( args.request )
+    resp = redfish_obj.delete(args.request)
 else:
-    resp = redfish_obj.get( args.request )
+    resp = redfish_obj.get(args.request)
 
 # Print HTTP status and headers
 if args.verbose:
-    print( "HTTP {}".format( resp.status ) )
+    print("HTTP {}".format(resp.status))
     for header in resp.getheaders():
-        print( "{}: {}".format( header[0], header[1] ) )
+        print("{}: {}".format(header[0], header[1]))
     print()
 
 # Print the response
 if resp.status != 204:
     try:
-        print( json.dumps( resp.dict, sort_keys = True, indent = 4, separators = ( ",", ": " ) ) )
-    except:
+        print(json.dumps(resp.dict, sort_keys=True, indent=4, separators=(",", ": ")))
+    except Exception:
         # The response is either malformed JSON or not JSON at all
-        print( resp.text )
+        print(resp.text)
 else:
-    print( "No response body" )
+    print("No response body")
 
 # Log out
-redfish_utilities.logout( redfish_obj )
-sys.exit( 0 )
+redfish_utilities.logout(redfish_obj)
+sys.exit(0)
```

### Comparing `redfish_utilities-3.2.8/scripts/rf_sensor_list.py` & `redfish_utilities-3.2.9/scripts/rf_sensor_list.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,52 +17,54 @@
 import redfish
 import redfish_utilities
 import traceback
 import sys
 from redfish.messages import RedfishPasswordChangeRequiredError
 
 # Get the input arguments
-argget = argparse.ArgumentParser( description = "A tool to walk a Redfish service and list sensor info" )
-argget.add_argument( "--user", "-u", type = str, required = True, help = "The user name for authentication" )
-argget.add_argument( "--password", "-p",  type = str, required = True, help = "The password for authentication" )
-argget.add_argument( "--rhost", "-r", type = str, required = True, help = "The address of the Redfish service (with scheme)" )
-argget.add_argument( "--id", "-i",  action = "store_true", help = "Construct sensor names using 'Id' values" )
-argget.add_argument( "--name", "-n",  action = "store_true", help = "Construct sensor names using 'Name' values" )
-argget.add_argument( "--debug", action = "store_true", help = "Creates debug file showing HTTP traces and exceptions" )
+argget = argparse.ArgumentParser(description="A tool to walk a Redfish service and list sensor info")
+argget.add_argument("--user", "-u", type=str, required=True, help="The user name for authentication")
+argget.add_argument("--password", "-p", type=str, required=True, help="The password for authentication")
+argget.add_argument("--rhost", "-r", type=str, required=True, help="The address of the Redfish service (with scheme)")
+argget.add_argument("--id", "-i", action="store_true", help="Construct sensor names using 'Id' values")
+argget.add_argument("--name", "-n", action="store_true", help="Construct sensor names using 'Name' values")
+argget.add_argument("--debug", action="store_true", help="Creates debug file showing HTTP traces and exceptions")
 args = argget.parse_args()
 
 if args.debug:
-    log_file = "rf_sensor_list-{}.log".format( datetime.datetime.now().strftime( "%Y-%m-%d-%H%M%S" ) )
+    log_file = "rf_sensor_list-{}.log".format(datetime.datetime.now().strftime("%Y-%m-%d-%H%M%S"))
     log_format = "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
-    logger = redfish.redfish_logger( log_file, log_format, logging.DEBUG )
-    logger.info( "rf_sensor_list Trace" )
+    logger = redfish.redfish_logger(log_file, log_format, logging.DEBUG)
+    logger.info("rf_sensor_list Trace")
 
 # Set up the Redfish object
 redfish_obj = None
 try:
-    redfish_obj = redfish.redfish_client( base_url = args.rhost, username = args.user, password = args.password, timeout = 15, max_retry = 3 )
-    redfish_obj.login( auth = "session" )
-except RedfishPasswordChangeRequiredError as e:
-    redfish_utilities.print_password_change_required_and_logout( redfish_obj, args )
-    sys.exit( 1 )
-except Exception as e:
+    redfish_obj = redfish.redfish_client(
+        base_url=args.rhost, username=args.user, password=args.password, timeout=15, max_retry=3
+    )
+    redfish_obj.login(auth="session")
+except RedfishPasswordChangeRequiredError:
+    redfish_utilities.print_password_change_required_and_logout(redfish_obj, args)
+    sys.exit(1)
+except Exception:
     raise
 
 exit_code = 0
 try:
     use_id = False
     if args.id:
         use_id = True
     if args.name:
         use_id = False
     # Get and print the sensor info
-    sensors = redfish_utilities.get_sensors( redfish_obj , use_id)
-    redfish_utilities.print_sensors( sensors )
+    sensors = redfish_utilities.get_sensors(redfish_obj, use_id)
+    redfish_utilities.print_sensors(sensors)
 except Exception as e:
     if args.debug:
-        logger.error( "Caught exception:\n\n{}\n".format( traceback.format_exc() ) )
+        logger.error("Caught exception:\n\n{}\n".format(traceback.format_exc()))
     exit_code = 1
-    print( e )
+    print(e)
 finally:
     # Log out
-    redfish_utilities.logout( redfish_obj )
-sys.exit( exit_code )
+    redfish_utilities.logout(redfish_obj)
+sys.exit(exit_code)
```

### Comparing `redfish_utilities-3.2.8/scripts/rf_sys_inventory.py` & `redfish_utilities-3.2.9/scripts/rf_sys_inventory.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,55 +18,74 @@
 import redfish
 import redfish_utilities
 import traceback
 import sys
 from redfish.messages import RedfishPasswordChangeRequiredError
 
 # Get the input arguments
-argget = argparse.ArgumentParser( description = "A tool to walk a Redfish service and list component information" )
-argget.add_argument( "--user", "-u", type = str, required = True, help = "The user name for authentication" )
-argget.add_argument( "--password", "-p",  type = str, required = True, help = "The password for authentication" )
-argget.add_argument( "--rhost", "-r", type = str, required = True, help = "The address of the Redfish service (with scheme)" )
-argget.add_argument( "--details", "-details", action = "store_true", help = "Indicates if the full details of each component should be shown" )
-argget.add_argument( "--noabsent", "-noabsent", action = "store_true", help = "Indicates if absent devices should be skipped" )
-argget.add_argument( "--write", "-w", nargs = "?", const = "Device_Inventory", type = str, help = "Indicates if the inventory should be written to a spreadsheet and what the file name should be if given" )
-argget.add_argument( "--workaround", "-workaround", action = "store_true", help = "Indicates if workarounds should be attempted for non-conformant services", default = False )
-argget.add_argument( "--debug", action = "store_true", help = "Creates debug file showing HTTP traces and exceptions" )
+argget = argparse.ArgumentParser(description="A tool to walk a Redfish service and list component information")
+argget.add_argument("--user", "-u", type=str, required=True, help="The user name for authentication")
+argget.add_argument("--password", "-p", type=str, required=True, help="The password for authentication")
+argget.add_argument("--rhost", "-r", type=str, required=True, help="The address of the Redfish service (with scheme)")
+argget.add_argument(
+    "--details", "-details", action="store_true", help="Indicates if the full details of each component should be shown"
+)
+argget.add_argument(
+    "--noabsent", "-noabsent", action="store_true", help="Indicates if absent devices should be skipped"
+)
+argget.add_argument(
+    "--write",
+    "-w",
+    nargs="?",
+    const="Device_Inventory",
+    type=str,
+    help="Indicates if the inventory should be written to a spreadsheet and what the file name should be if given",
+)
+argget.add_argument(
+    "--workaround",
+    "-workaround",
+    action="store_true",
+    help="Indicates if workarounds should be attempted for non-conformant services",
+    default=False,
+)
+argget.add_argument("--debug", action="store_true", help="Creates debug file showing HTTP traces and exceptions")
 args = argget.parse_args()
 
 if args.workaround:
     redfish_utilities.config.__workarounds__ = True
 
 if args.debug:
-    log_file = "rf_sys_inventory-{}.log".format( datetime.datetime.now().strftime( "%Y-%m-%d-%H%M%S" ) )
+    log_file = "rf_sys_inventory-{}.log".format(datetime.datetime.now().strftime("%Y-%m-%d-%H%M%S"))
     log_format = "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
-    logger = redfish.redfish_logger( log_file, log_format, logging.DEBUG )
-    logger.info( "rf_sys_inventory Trace" )
+    logger = redfish.redfish_logger(log_file, log_format, logging.DEBUG)
+    logger.info("rf_sys_inventory Trace")
 
 # Set up the Redfish object
 redfish_obj = None
 try:
-    redfish_obj = redfish.redfish_client( base_url = args.rhost, username = args.user, password = args.password, timeout = 15, max_retry = 3 )
-    redfish_obj.login( auth = "session" )
-except RedfishPasswordChangeRequiredError as e:
-    redfish_utilities.print_password_change_required_and_logout( redfish_obj, args )
-    sys.exit( 1 )
-except Exception as e:
+    redfish_obj = redfish.redfish_client(
+        base_url=args.rhost, username=args.user, password=args.password, timeout=15, max_retry=3
+    )
+    redfish_obj.login(auth="session")
+except RedfishPasswordChangeRequiredError:
+    redfish_utilities.print_password_change_required_and_logout(redfish_obj, args)
+    sys.exit(1)
+except Exception:
     raise
 
 exit_code = 0
 try:
     # Get and print the system inventory
-    inventory = redfish_utilities.get_system_inventory( redfish_obj )
-    redfish_utilities.print_system_inventory( inventory, args.details, args.noabsent )
+    inventory = redfish_utilities.get_system_inventory(redfish_obj)
+    redfish_utilities.print_system_inventory(inventory, args.details, args.noabsent)
 
     if args.write:
-        redfish_utilities.write_system_inventory( inventory, args.write )
+        redfish_utilities.write_system_inventory(inventory, args.write)
 except Exception as e:
     if args.debug:
-        logger.error( "Caught exception:\n\n{}\n".format( traceback.format_exc() ) )
+        logger.error("Caught exception:\n\n{}\n".format(traceback.format_exc()))
     exit_code = 1
-    print( e )
+    print(e)
 finally:
     # Log out
-    redfish_utilities.logout( redfish_obj )
-sys.exit( exit_code )
+    redfish_utilities.logout(redfish_obj)
+sys.exit(exit_code)
```

### Comparing `redfish_utilities-3.2.8/scripts/rf_test_event_listener.py` & `redfish_utilities-3.2.9/scripts/rf_test_event_listener.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,53 +13,74 @@
 """
 
 import argparse
 import json
 import requests
 from datetime import datetime
 
-event_headers = {
-    "Content-Type": "application/json"
-}
+event_headers = {"Content-Type": "application/json"}
 
 event_payload = {
     "@odata.type": "#Event.v1_7_0.Event",
     "Id": "1",
     "Name": "Sample Event",
     "Context": "Sample Event for Listener",
     "Events": [
         {
             "EventType": "Other",
             "EventId": "1",
             "Severity": "OK",
             "MessageSeverity": "OK",
             "Message": "Test message.",
-            "MessageId": "Resource.1.3.TestMessage"
+            "MessageId": "Resource.1.3.TestMessage",
         }
-    ]
+    ],
 }
 
-argget = argparse.ArgumentParser( description = "A tool to help verify a Redfish event listener" )
-argget.add_argument( "--listener", "-l", type = str, required = True, help = "The absolute URI of the Redfish event listener (with scheme)" )
-argget.add_argument( "--file", "-file", type = str, help = "The filepath to a JSON file containing the event payload; if this argument is specified, all other arguments controlling the event data is ignored" )
-argget.add_argument( "--id", "-id", type = str, help = "The value to specify in the Id property of the event" )
-argget.add_argument( "--name", "-name", type = str, help = "The value to specify in the Name property of the event" )
-argget.add_argument( "--context", "-context", type = str, help = "The value to specify in the Context property of the event" )
-argget.add_argument( "--eventtype", "-eventtype", type = str, help = "The value to specify in the EventType property of the event" )
-argget.add_argument( "--eventid", "-eventid", type = str, help = "The value to specify in the EventId property of the event" )
-argget.add_argument( "--severity", "-severity", type = str, help = "The value to specify in the Severity property of the event" )
-argget.add_argument( "--message", "-message", type = str, help = "The value to specify in the Message property of the event" )
-argget.add_argument( "--messageid", "-messageid", type = str, help = "The value to specify in the MessageId property of the event" )
-argget.add_argument( "--timestamp", "-timestamp", type = str, help = "The value to specify in the EventTimestamp property of the event" )
-argget.add_argument( "--header", "-header", type = str, nargs = 2, metavar = ( "name", "value" ), action = "append", help = "Name-value pairs of HTTP headers to provide with the request" )
+argget = argparse.ArgumentParser(description="A tool to help verify a Redfish event listener")
+argget.add_argument(
+    "--listener", "-l", type=str, required=True, help="The absolute URI of the Redfish event listener (with scheme)"
+)
+argget.add_argument(
+    "--file",
+    "-file",
+    type=str,
+    help="The filepath to a JSON file containing the event payload; if this argument is specified, all other arguments controlling the event data is ignored",
+)
+argget.add_argument("--id", "-id", type=str, help="The value to specify in the Id property of the event")
+argget.add_argument("--name", "-name", type=str, help="The value to specify in the Name property of the event")
+argget.add_argument("--context", "-context", type=str, help="The value to specify in the Context property of the event")
+argget.add_argument(
+    "--eventtype", "-eventtype", type=str, help="The value to specify in the EventType property of the event"
+)
+argget.add_argument("--eventid", "-eventid", type=str, help="The value to specify in the EventId property of the event")
+argget.add_argument(
+    "--severity", "-severity", type=str, help="The value to specify in the Severity property of the event"
+)
+argget.add_argument("--message", "-message", type=str, help="The value to specify in the Message property of the event")
+argget.add_argument(
+    "--messageid", "-messageid", type=str, help="The value to specify in the MessageId property of the event"
+)
+argget.add_argument(
+    "--timestamp", "-timestamp", type=str, help="The value to specify in the EventTimestamp property of the event"
+)
+argget.add_argument(
+    "--header",
+    "-header",
+    type=str,
+    nargs=2,
+    metavar=("name", "value"),
+    action="append",
+    help="Name-value pairs of HTTP headers to provide with the request",
+)
 args = argget.parse_args()
 
 # Update the event payload based on the specified arguments
 if args.file:
-    with open( args.file ) as json_file:
+    with open(args.file) as json_file:
         event_payload = json.load(json_file)
 else:
     if args.id:
         event_payload["Id"] = args.id
     if args.name:
         event_payload["Name"] = args.name
     if args.context:
@@ -74,17 +95,17 @@
     if args.message:
         event_payload["Events"][0]["Message"] = args.message
     if args.messageid:
         event_payload["Events"][0]["MessageId"] = args.messageid
     if args.timestamp:
         event_payload["Events"][0]["EventTimestamp"] = args.timestamp
     else:
-        event_payload["Events"][0]["EventTimestamp"] = datetime.now().replace( microsecond = 0 ).astimezone().isoformat()
+        event_payload["Events"][0]["EventTimestamp"] = datetime.now().replace(microsecond=0).astimezone().isoformat()
 
 # Update the HTTP headers based on the specified arguments
 if args.header:
     for header in args.header:
         event_headers[header[0]] = header[1]
 
 # Send the request
-response = requests.post( args.listener, json = event_payload, headers = event_headers, timeout = 15, verify = False )
-print( "Listener responded with {} {}".format( response.status_code, response.reason ) )
+response = requests.post(args.listener, json=event_payload, headers=event_headers, timeout=15, verify=False)
+print("Listener responded with {} {}".format(response.status_code, response.reason))
```

### Comparing `redfish_utilities-3.2.8/scripts/rf_update.py` & `redfish_utilities-3.2.9/scripts/rf_update.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,152 +22,171 @@
 import socket
 import sys
 import threading
 import time
 import traceback
 from redfish.messages import RedfishPasswordChangeRequiredError
 
-if sys.version_info > ( 3, ):
+if sys.version_info > (3,):
     import http.server
 else:
     import SimpleHTTPServer
     import SocketServer
 
 WEB_SERVER_PORT = 8888
 WEB_SERVER_FOLDER = "rf_update_server"
 
-def local_web_server( filepath ):
+
+def local_web_server(filepath):
     """
     Creates a web server to host the image file
 
     Args:
         filepath: The filepath for the image
     """
 
     # Create a temporary folder and move the file to the folder
     try:
-        shutil.rmtree( WEB_SERVER_FOLDER )
-    except:
+        shutil.rmtree(WEB_SERVER_FOLDER)
+    except Exception:
         pass
-    os.mkdir( WEB_SERVER_FOLDER )
-    shutil.copy( filepath, WEB_SERVER_FOLDER )
-    os.chdir( WEB_SERVER_FOLDER )
+    os.mkdir(WEB_SERVER_FOLDER)
+    shutil.copy(filepath, WEB_SERVER_FOLDER)
+    os.chdir(WEB_SERVER_FOLDER)
 
     # Create a web server and host it out of the temporary folder
-    if sys.version_info > ( 3, ):
+    if sys.version_info > (3,):
         handler = http.server.SimpleHTTPRequestHandler
-        httpd = http.server.HTTPServer( ( "", WEB_SERVER_PORT ), handler )
+        httpd = http.server.HTTPServer(("", WEB_SERVER_PORT), handler)
     else:
         handler = SimpleHTTPServer.SimpleHTTPRequestHandler
-        httpd = SocketServer.TCPServer( ( "", WEB_SERVER_PORT ), handler )
+        httpd = SocketServer.TCPServer(("", WEB_SERVER_PORT), handler)
     httpd.serve_forever()
 
     return
 
-def print_error_payload( response ):
+
+def print_error_payload(response):
     """
     Prints an error payload, which can also be used for action responses
 
     Args:
         response: The response to print
     """
 
     try:
-        print(redfish_utilities.get_error_messages( response ) )
-    except:
+        print(redfish_utilities.get_error_messages(response))
+    except Exception:
         # No response body
         if response.status >= 400:
-            print( "Failed" )
+            print("Failed")
         else:
-            print( "Success" )
+            print("Success")
+
 
 # Get the input arguments
-argget = argparse.ArgumentParser( description = "A tool to perform an update with a Redfish service" )
-argget.add_argument( "--user", "-u", type = str, required = True, help = "The user name for authentication" )
-argget.add_argument( "--password", "-p",  type = str, required = True, help = "The password for authentication" )
-argget.add_argument( "--rhost", "-r", type = str, required = True, help = "The address of the Redfish service (with scheme)" )
-argget.add_argument( "--image", "-i", type = str, required = True, help = "The URI or filepath of the image" )
-argget.add_argument( "--target", "-t", type = str, help = "The target resource to apply the image" )
-argget.add_argument( "--applytime", "-at", type = redfish_utilities.operation_apply_times, help = "The apply time for the update", choices = redfish_utilities.operation_apply_times )
-argget.add_argument( "--debug", action = "store_true", help = "Creates debug file showing HTTP traces and exceptions" )
+argget = argparse.ArgumentParser(description="A tool to perform an update with a Redfish service")
+argget.add_argument("--user", "-u", type=str, required=True, help="The user name for authentication")
+argget.add_argument("--password", "-p", type=str, required=True, help="The password for authentication")
+argget.add_argument("--rhost", "-r", type=str, required=True, help="The address of the Redfish service (with scheme)")
+argget.add_argument("--image", "-i", type=str, required=True, help="The URI or filepath of the image")
+argget.add_argument("--target", "-t", type=str, help="The target resource to apply the image")
+argget.add_argument(
+    "--applytime",
+    "-at",
+    type=redfish_utilities.operation_apply_times,
+    help="The apply time for the update",
+    choices=redfish_utilities.operation_apply_times,
+)
+argget.add_argument("--debug", action="store_true", help="Creates debug file showing HTTP traces and exceptions")
 args = argget.parse_args()
 
 if args.debug:
-    log_file = "rf_update-{}.log".format( datetime.datetime.now().strftime( "%Y-%m-%d-%H%M%S" ) )
+    log_file = "rf_update-{}.log".format(datetime.datetime.now().strftime("%Y-%m-%d-%H%M%S"))
     log_format = "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
-    logger = redfish.redfish_logger( log_file, log_format, logging.DEBUG )
-    logger.info( "rf_update Trace" )
+    logger = redfish.redfish_logger(log_file, log_format, logging.DEBUG)
+    logger.info("rf_update Trace")
 
 # Set up the Redfish object
 redfish_obj = None
 try:
-    redfish_obj = redfish.redfish_client( base_url = args.rhost, username = args.user, password = args.password, timeout = 15, max_retry = 3 )
-    redfish_obj.login( auth = "session" )
-except RedfishPasswordChangeRequiredError as e:
-    redfish_utilities.print_password_change_required_and_logout( redfish_obj, args )
-    sys.exit( 1 )
-except Exception as e:
+    redfish_obj = redfish.redfish_client(
+        base_url=args.rhost, username=args.user, password=args.password, timeout=15, max_retry=3
+    )
+    redfish_obj.login(auth="session")
+except RedfishPasswordChangeRequiredError:
+    redfish_utilities.print_password_change_required_and_logout(redfish_obj, args)
+    sys.exit(1)
+except Exception:
     raise
 
 start_path = os.getcwd()
 targets = None
 if args.target is not None:
-    targets = [ args.target ]
+    targets = [args.target]
 exit_code = 0
 try:
     # Determine what path to use to perform the update
-    update_service = redfish_utilities.get_update_service( redfish_obj )
-    if os.path.isfile( args.image ):
+    update_service = redfish_utilities.get_update_service(redfish_obj)
+    if os.path.isfile(args.image):
         # Local image; see if we can push the image directly
         if "MultipartHttpPushUri" in update_service.dict:
             # Perform a multipart push update
-            print( "Pushing the image to the service directly; depending on the size of the image, this can take a few minutes..." )
-            response = redfish_utilities.multipart_push_update( redfish_obj, args.image, targets = targets, apply_time = args.applytime )
+            print(
+                "Pushing the image to the service directly; depending on the size of the image, this can take a few minutes..."
+            )
+            response = redfish_utilities.multipart_push_update(
+                redfish_obj, args.image, targets=targets, apply_time=args.applytime
+            )
         else:
             # Host a local web server and perform a SimpleUpdate for the local image
-            web_server_thread = threading.Thread( target = local_web_server, args=( args.image, ) )
-            web_server_thread.setDaemon( True )
+            web_server_thread = threading.Thread(target=local_web_server, args=(args.image,))
+            web_server_thread.setDaemon(True)
             web_server_thread.start()
             # Wait for the server to start up
-            time.sleep( 3 )
+            time.sleep(3)
 
             # Build the proper image URI for the call based on how the web server will be hosting it
             # TODO: Find a better way of getting your own IP address
             # socket.gethostbyname( socket.gethostname() ) returns 127.0.0.1 on many systems
             # This will open a socket with the target, and pulls the address of the socket
-            groups = re.search( "^(https?)://([^:]+)(:(\d+))?$", args.rhost )
-            s = socket.socket( socket.AF_INET, socket.SOCK_DGRAM )
-            remote_port = groups.group( 4 )
+            groups = re.search("^(https?)://([^:]+)(:(\d+))?$", args.rhost)
+            s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+            remote_port = groups.group(4)
             if remote_port is None:
                 remote_port = "80"
-                if groups.group( 1 ) == "https":
+                if groups.group(1) == "https":
                     remote_port = "443"
-            s.connect( ( groups.group(2), int( remote_port ) ) )
-            image_uri = "http://{}:{}/{}".format( s.getsockname()[0], WEB_SERVER_PORT, args.image.rsplit( os.path.sep, 1 )[-1] )
+            s.connect((groups.group(2), int(remote_port)))
+            image_uri = "http://{}:{}/{}".format(
+                s.getsockname()[0], WEB_SERVER_PORT, args.image.rsplit(os.path.sep, 1)[-1]
+            )
             s.close()
-            response = redfish_utilities.simple_update( redfish_obj, image_uri, targets = targets, apply_time = args.applytime )
+            response = redfish_utilities.simple_update(
+                redfish_obj, image_uri, targets=targets, apply_time=args.applytime
+            )
     else:
         # Remote image; always use SimpleUpdate
-        response = redfish_utilities.simple_update( redfish_obj, args.image, targets = targets, apply_time = args.applytime )
+        response = redfish_utilities.simple_update(redfish_obj, args.image, targets=targets, apply_time=args.applytime)
 
     # Monitor the response
-    print( "Update initiated..." )
-    response = redfish_utilities.poll_task_monitor( redfish_obj, response )
+    print("Update initiated...")
+    response = redfish_utilities.poll_task_monitor(redfish_obj, response)
 
     # Display the results
-    print( "" )
-    print_error_payload( response )
+    print("")
+    print_error_payload(response)
 except Exception as e:
     if args.debug:
-        logger.error( "Caught exception:\n\n{}\n".format( traceback.format_exc() ) )
+        logger.error("Caught exception:\n\n{}\n".format(traceback.format_exc()))
     exit_code = 1
-    print( e )
+    print(e)
 finally:
     # Log out and cleanup
-    os.chdir( start_path )
+    os.chdir(start_path)
     try:
-        shutil.rmtree( WEB_SERVER_FOLDER )
-    except:
+        shutil.rmtree(WEB_SERVER_FOLDER)
+    except Exception:
         pass
     # Log out
-    redfish_utilities.logout( redfish_obj )
-sys.exit( exit_code )
+    redfish_utilities.logout(redfish_obj)
+sys.exit(exit_code)
```

### Comparing `redfish_utilities-3.2.8/scripts/rf_virtual_media.py` & `redfish_utilities-3.2.9/scripts/rf_virtual_media.py`

 * *Files 27% similar despite different names*

```diff
@@ -17,62 +17,82 @@
 import redfish
 import redfish_utilities
 import traceback
 import sys
 from redfish.messages import RedfishPasswordChangeRequiredError
 
 # Get the input arguments
-argget = argparse.ArgumentParser( description = "A tool to manage virtual media of a system" )
-argget.add_argument( "--user", "-u", type = str, required = True, help = "The user name for authentication" )
-argget.add_argument( "--password", "-p",  type = str, required = True, help = "The password for authentication" )
-argget.add_argument( "--rhost", "-r", type = str, required = True, help = "The address of the Redfish service (with scheme)" )
-argget.add_argument( "--system", "-s", type = str, help = "The ID of the system containing the virtual media" )
-argget.add_argument( "--debug", action = "store_true", help = "Creates debug file showing HTTP traces and exceptions" )
-subparsers = argget.add_subparsers( dest = "command" )
-info_argget = subparsers.add_parser( "info", help = "Displays information about the virtual media for a system" )
-insert_argget = subparsers.add_parser( "insert", help = "Inserts virtual media for a system" )
-insert_argget.add_argument( "--image", "-image", type = str, required = True, help = "The URI of the image to insert" )
-insert_argget.add_argument( "--id", "-i", type = str, help = "The identifier of the virtual media instance to insert" )
-insert_argget.add_argument( "--notinserted", "-notinserted", action = "store_false", help = "Indicates if the media is to be marked as not inserted for the system", default = None )
-insert_argget.add_argument( "--writable", "-writable", action = "store_false", help = "Indicates if the media is to be marked as writable for the system", default = None )
-insert_argget.add_argument( "--mediatypes", "-mt", type = str, nargs = '+', help = "A list of acceptable media types for the virtual media" )
-eject_argget = subparsers.add_parser( "eject", help = "Ejects virtual media from a system" )
-eject_argget.add_argument( "--id", "-i", type = str, required = True, help = "The identifier of the virtual media instance to eject" )
+argget = argparse.ArgumentParser(description="A tool to manage virtual media of a system")
+argget.add_argument("--user", "-u", type=str, required=True, help="The user name for authentication")
+argget.add_argument("--password", "-p", type=str, required=True, help="The password for authentication")
+argget.add_argument("--rhost", "-r", type=str, required=True, help="The address of the Redfish service (with scheme)")
+argget.add_argument("--system", "-s", type=str, help="The ID of the system containing the virtual media")
+argget.add_argument("--debug", action="store_true", help="Creates debug file showing HTTP traces and exceptions")
+subparsers = argget.add_subparsers(dest="command")
+info_argget = subparsers.add_parser("info", help="Displays information about the virtual media for a system")
+insert_argget = subparsers.add_parser("insert", help="Inserts virtual media for a system")
+insert_argget.add_argument("--image", "-image", type=str, required=True, help="The URI of the image to insert")
+insert_argget.add_argument("--id", "-i", type=str, help="The identifier of the virtual media instance to insert")
+insert_argget.add_argument(
+    "--notinserted",
+    "-notinserted",
+    action="store_false",
+    help="Indicates if the media is to be marked as not inserted for the system",
+    default=None,
+)
+insert_argget.add_argument(
+    "--writable",
+    "-writable",
+    action="store_false",
+    help="Indicates if the media is to be marked as writable for the system",
+    default=None,
+)
+insert_argget.add_argument(
+    "--mediatypes", "-mt", type=str, nargs="+", help="A list of acceptable media types for the virtual media"
+)
+eject_argget = subparsers.add_parser("eject", help="Ejects virtual media from a system")
+eject_argget.add_argument(
+    "--id", "-i", type=str, required=True, help="The identifier of the virtual media instance to eject"
+)
 args = argget.parse_args()
 
 if args.debug:
-    log_file = "rf_virtual_media-{}.log".format( datetime.datetime.now().strftime( "%Y-%m-%d-%H%M%S" ) )
+    log_file = "rf_virtual_media-{}.log".format(datetime.datetime.now().strftime("%Y-%m-%d-%H%M%S"))
     log_format = "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
-    logger = redfish.redfish_logger( log_file, log_format, logging.DEBUG )
-    logger.info( "rf_virtual_media Trace" )
+    logger = redfish.redfish_logger(log_file, log_format, logging.DEBUG)
+    logger.info("rf_virtual_media Trace")
 
 # Set up the Redfish object
 redfish_obj = None
 try:
-    redfish_obj = redfish.redfish_client( base_url = args.rhost, username = args.user, password = args.password, timeout = 15, max_retry = 3 )
-    redfish_obj.login( auth = "session" )
-except RedfishPasswordChangeRequiredError as e:
-    redfish_utilities.print_password_change_required_and_logout( redfish_obj, args )
-    sys.exit( 1 )
-except Exception as e:
+    redfish_obj = redfish.redfish_client(
+        base_url=args.rhost, username=args.user, password=args.password, timeout=15, max_retry=3
+    )
+    redfish_obj.login(auth="session")
+except RedfishPasswordChangeRequiredError:
+    redfish_utilities.print_password_change_required_and_logout(redfish_obj, args)
+    sys.exit(1)
+except Exception:
     raise
 
 exit_code = 0
 try:
     if args.command == "insert":
-        print( "Inserting '{}'".format( args.image ) )
-        redfish_utilities.insert_virtual_media( redfish_obj, args.image, args.system, args.id, args.mediatypes, args.notinserted, args.writable )
+        print("Inserting '{}'".format(args.image))
+        redfish_utilities.insert_virtual_media(
+            redfish_obj, args.image, args.system, args.id, args.mediatypes, args.notinserted, args.writable
+        )
     elif args.command == "eject":
-        print( "Ejecting '{}'".format( args.id ) )
-        redfish_utilities.eject_virtual_media (redfish_obj, args.id, args.system )
+        print("Ejecting '{}'".format(args.id))
+        redfish_utilities.eject_virtual_media(redfish_obj, args.id, args.system)
     else:
-        virtual_media = redfish_utilities.get_virtual_media( redfish_obj, args.system )
-        redfish_utilities.print_virtual_media( virtual_media )
+        virtual_media = redfish_utilities.get_virtual_media(redfish_obj, args.system)
+        redfish_utilities.print_virtual_media(virtual_media)
 except Exception as e:
     if args.debug:
-        logger.error( "Caught exception:\n\n{}\n".format( traceback.format_exc() ) )
+        logger.error("Caught exception:\n\n{}\n".format(traceback.format_exc()))
     exit_code = 1
-    print( e )
+    print(e)
 finally:
     # Log out
-    redfish_utilities.logout( redfish_obj )
-sys.exit( exit_code )
+    redfish_utilities.logout(redfish_obj)
+sys.exit(exit_code)
```

### Comparing `redfish_utilities-3.2.8/setup.py` & `redfish_utilities-3.2.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,69 +2,73 @@
 # Copyright Notice:
 # Copyright 2019-2022 DMTF. All rights reserved.
 # License: BSD 3-Clause License. For full text see link: https://github.com/DMTF/Redfish-Tacklebox/blob/main/LICENSE.md
 
 from setuptools import setup
 from setuptools import Command as _Command
 from codecs import open
-import sys
 import os
 
+
 class Pyinstaller(_Command):
-    description: 'Pyinstaller'
+    description: "Pyinstaller"
     user_options = []
+
     def __init__(self, dist, **kw):
         super().__init__(dist, **kw)
         self.flags = ""
         self.scripts = []
         self.packages = []
         if not os.path.exists("./dist"):
             os.mkdir("dist")
         if not os.path.exists("./spec"):
             os.mkdir("spec")
+
     def initialize_options(self):
         self.flags = ""
         self.scripts = []
         self.packages = []
 
     def finalize_options(self):
         self.flags = "--specpath ./spec"
         self.scripts = self.distribution.scripts
         self.packages = self.distribution.packages
         for package in self.packages:
-            self.flags = "{} --collect-all {}".format(self.flags,package)
+            self.flags = "{} --collect-all {}".format(self.flags, package)
 
     def pyinstaller(self, target):
         if os.system("pyinstaller --onefile {} {}".format(target, self.flags)):
             raise Exception("PyInstaller failed!")
+
     def run(self):
         for scripts in self.scripts:
             self.pyinstaller(scripts)
 
-with open( "README.md", "r", "utf-8" ) as f:
+
+with open("README.md", "r", "utf-8") as f:
     long_description = f.read()
 
 setup(
-    name = "redfish_utilities",
-    version = "3.2.8",
-    description = "Redfish Utilities",
-    long_description = long_description,
-    long_description_content_type = "text/markdown",
-    author = "DMTF, https://www.dmtf.org/standards/feedback",
-    license = "BSD 3-clause \"New\" or \"Revised License\"",
-    classifiers = [
+    name="redfish_utilities",
+    version="3.2.9",
+    description="Redfish Utilities",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    author="DMTF, https://www.dmtf.org/standards/feedback",
+    license='BSD 3-clause "New" or "Revised License"',
+    classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: BSD License",
         "Programming Language :: Python :: 3",
-        "Topic :: Communications"
+        "Topic :: Communications",
     ],
-    keywords = "Redfish",
-    url = "https://github.com/DMTF/Redfish-Tacklebox",
-    packages = [ "redfish_utilities" ],
-    scripts = [
+    keywords="Redfish",
+    url="https://github.com/DMTF/Redfish-Tacklebox",
+    packages=["redfish_utilities"],
+    scripts=[
         "scripts/rf_accounts.py",
         "scripts/rf_assembly.py",
         "scripts/rf_bios_settings.py",
         "scripts/rf_boot_override.py",
         "scripts/rf_certificates.py",
         "scripts/rf_diagnostic_data.py",
         "scripts/rf_discover.py",
@@ -75,14 +79,12 @@
         "scripts/rf_power_equipment.py",
         "scripts/rf_power_reset.py",
         "scripts/rf_raw_request.py",
         "scripts/rf_sensor_list.py",
         "scripts/rf_sys_inventory.py",
         "scripts/rf_test_event_listener.py",
         "scripts/rf_update.py",
-        "scripts/rf_virtual_media.py"
+        "scripts/rf_virtual_media.py",
     ],
-    install_requires = [ "redfish>=3.2.1", "XlsxWriter>=1.2.7", "requests" ],
-    cmdclass={
-        'pyinstaller': Pyinstaller
-    }
+    install_requires=["redfish>=3.2.1", "XlsxWriter>=1.2.7", "requests"],
+    cmdclass={"pyinstaller": Pyinstaller},
 )
```

