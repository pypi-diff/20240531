# Comparing `tmp/fortiedr-3.6.9.tar.gz` & `tmp/fortiedr-3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortiedr-3.6.9.tar", last modified: Thu May 30 00:29:54 2024, max compression
+gzip compressed data, was "fortiedr-3.7.tar", last modified: Thu May 30 17:01:55 2024, max compression
```

## Comparing `fortiedr-3.6.9.tar` & `fortiedr-3.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:29:54.918597 fortiedr-3.6.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-30 00:29:36.000000 fortiedr-3.6.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-30 00:29:36.000000 fortiedr-3.6.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-30 00:29:54.918597 fortiedr-3.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-30 00:29:36.000000 fortiedr-3.6.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:29:54.914597 fortiedr-3.6.9/fortiedr/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-30 00:29:36.000000 fortiedr-3.6.9/fortiedr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21615 2024-05-30 00:29:36.000000 fortiedr-3.6.9/fortiedr/api_parameters.json
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-30 00:29:36.000000 fortiedr-3.6.9/fortiedr/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-05-30 00:29:36.000000 fortiedr-3.6.9/fortiedr/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)   261160 2024-05-30 00:29:36.000000 fortiedr-3.6.9/fortiedr/fortiedr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 00:29:54.918597 fortiedr-3.6.9/fortiedr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-30 00:29:54.000000 fortiedr-3.6.9/fortiedr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-30 00:29:54.000000 fortiedr-3.6.9/fortiedr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 00:29:54.000000 fortiedr-3.6.9/fortiedr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 00:29:54.000000 fortiedr-3.6.9/fortiedr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-30 00:29:36.000000 fortiedr-3.6.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-30 00:29:36.000000 fortiedr-3.6.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 00:29:54.918597 fortiedr-3.6.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-30 00:29:36.000000 fortiedr-3.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:01:55.647444 fortiedr-3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-30 17:01:51.000000 fortiedr-3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-30 17:01:51.000000 fortiedr-3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-30 17:01:55.647444 fortiedr-3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-30 17:01:51.000000 fortiedr-3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:01:55.647444 fortiedr-3.7/fortiedr/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-30 17:01:51.000000 fortiedr-3.7/fortiedr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21615 2024-05-30 17:01:51.000000 fortiedr-3.7/fortiedr/api_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-30 17:01:51.000000 fortiedr-3.7/fortiedr/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-05-30 17:01:51.000000 fortiedr-3.7/fortiedr/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)   256563 2024-05-30 17:01:51.000000 fortiedr-3.7/fortiedr/fortiedr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:01:55.647444 fortiedr-3.7/fortiedr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-30 17:01:55.000000 fortiedr-3.7/fortiedr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-30 17:01:55.000000 fortiedr-3.7/fortiedr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 17:01:55.000000 fortiedr-3.7/fortiedr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 17:01:55.000000 fortiedr-3.7/fortiedr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-30 17:01:51.000000 fortiedr-3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-30 17:01:51.000000 fortiedr-3.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 17:01:55.647444 fortiedr-3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-30 17:01:51.000000 fortiedr-3.7/setup.py
```

### Comparing `fortiedr-3.6.9/LICENSE` & `fortiedr-3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fortiedr-3.6.9/PKG-INFO` & `fortiedr-3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortiedr
-Version: 3.6.9
+Version: 3.7
 Summary: This Fortiedr module is an open-source Python library that simplifies interaction with the FortiEDR Cloud API.
 Author: Rafael Foster
 Author-email: Rafael Foster <rafaelgfoster@gmail.com>
 Project-URL: Homepage, https://github.com/rafaelfoster/fortiedr
 Project-URL: Issues, https://github.com/rafaelfoster/fortiedr/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fortiedr-3.6.9/README.md` & `fortiedr-3.7/README.md`

 * *Files identical despite different names*

### Comparing `fortiedr-3.6.9/fortiedr/api_parameters.json` & `fortiedr-3.7/fortiedr/api_parameters.json`

 * *Files identical despite different names*

### Comparing `fortiedr-3.6.9/fortiedr/auth.py` & `fortiedr-3.7/fortiedr/auth.py`

 * *Files identical despite different names*

### Comparing `fortiedr-3.6.9/fortiedr/connector.py` & `fortiedr-3.7/fortiedr/connector.py`

 * *Files identical despite different names*

### Comparing `fortiedr-3.6.9/fortiedr/fortiedr.py` & `fortiedr-3.7/fortiedr/fortiedr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,45 +1,18 @@
 
 import os
 import json
 from typing import BinaryIO
 from fortiedr.auth import Auth as fedrAuth
 from fortiedr.connector import FortiEDR_API_GW
 
-version = '3.6.9'
+version = '3.7'
 
 fortiedr_connection = None
 
-class Admin:
-	'''Admin Rest Api Controller'''
-
-	def set_tray_notification_settings(self, enabledPopup: bool = None, enabledTrayNotification: bool = None, message: str = None, organization: str = None) -> tuple[bool, None]:
-		'''
-		Class Admin
-		Description: Update tray notification settings.
-        
-		Args:
-			adminSetTrayNotificationSettingsRequest (Object): Check 'adminSetTrayNotificationSettingsRequest' in the API documentation for further information.
-
-		Returns:
-			bool: Status of the request (True or False). 
-			None: This function does not return any data.
-		'''
-		validate_params("set_tray_notification_settings", locals())
-
-		url = '/api/admin/set-tray-notification-settings'
-
-		adminSetTrayNotificationSettingsRequest = {}
-		if enabledPopup: adminSetTrayNotificationSettingsRequest["enabledPopup"] = enabledPopup
-		if enabledTrayNotification: adminSetTrayNotificationSettingsRequest["enabledTrayNotification"] = enabledTrayNotification
-		if message: adminSetTrayNotificationSettingsRequest["message"] = message
-		if organization: adminSetTrayNotificationSettingsRequest["organization"] = organization
-
-		return fortiedr_connection.send(url, adminSetTrayNotificationSettingsRequest)
-
 class ApplicationControl:
 	'''Application Control Rest Api Controller'''
 
 	def get_applications(self, currentPage: int, organization: str, fileName: str = None, path: str = None, signer: str = None, enabled: bool = None, hash: str = None, operatingSystem: str = None, policyIds: list = None, tag: str = None) -> tuple[bool, None]:
 		'''
 		Class ApplicationControl
 		Description: Get application controls.
@@ -206,73 +179,41 @@
 
 		applicationControlTagCreateRequest = {}
 		if name: applicationControlTagCreateRequest["name"] = name
 		if organization: applicationControlTagCreateRequest["organization"] = organization
 
 		return fortiedr_connection.send(url, applicationControlTagCreateRequest)
 
-class dashboardrestapicontroller:
-	'''Dashboard Rest Api Controller'''
+class Administrator:
+	'''The Administrator module enables administrators to perform administrative operations, such as handling licenses and users.'''
 
-	def most_targeted_items(self, organization: str, itemType: str = None, numOfColumns: int = None, numOfDays: int = None) -> tuple[bool, None]:
+	def set_tray_notification_settings(self, enabledPopup: bool = None, enabledTrayNotification: bool = None, message: str = None, organization: str = None) -> tuple[bool, None]:
 		'''
-		Class dashboardrestapicontroller
-		Description: Returns most targeted devices or most targeted processes, depending on the itemType parameter.
+		Class Admin
+		Description: Update tray notification settings.
         
 		Args:
-			itemType (str): Specifies the type of items.
-			numOfColumns (int): Specifies the number of columns to present.
-			numOfDays (int): Specifies the number of days to present.
-			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+			adminSetTrayNotificationSettingsRequest (Object): Check 'adminSetTrayNotificationSettingsRequest' in the API documentation for further information.
 
 		Returns:
 			bool: Status of the request (True or False). 
 			None: This function does not return any data.
 		'''
-		validate_params("most_targeted_items", locals())
-
-		url = '/api/dashboard/most-targeted-items'
-		url_params = []
-		if itemType:
-			url_params.append('itemType=' + itemType)
-		if numOfColumns:
-			url_params.append('numOfColumns=' + numOfColumns)
-		if numOfDays:
-			url_params.append('numOfDays=' + numOfDays)
-		if organization:
-			url_params.append('organization=' + organization)
-		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.get(url)
+		validate_params("set_tray_notification_settings", locals())
 
-	def unhandled_items(self, organization: str, itemType: str = None) -> tuple[bool, None]:
-		'''
-		Class dashboardrestapicontroller
-		Description: Returns unhandled devices or unhandled processes, depending on the itemType parameter.
-        
-		Args:
-			itemType (str): Specifies the type of items.
-			organization (str): Specifies the name of a specific organization. The value that you specify here must match exactly.
+		url = '/api/admin/set-tray-notification-settings'
 
-		Returns:
-			bool: Status of the request (True or False). 
-			None: This function does not return any data.
-		'''
-		validate_params("unhandled_items", locals())
+		adminSetTrayNotificationSettingsRequest = {}
+		if enabledPopup: adminSetTrayNotificationSettingsRequest["enabledPopup"] = enabledPopup
+		if enabledTrayNotification: adminSetTrayNotificationSettingsRequest["enabledTrayNotification"] = enabledTrayNotification
+		if message: adminSetTrayNotificationSettingsRequest["message"] = message
+		if organization: adminSetTrayNotificationSettingsRequest["organization"] = organization
 
-		url = '/api/dashboard/unhandled-items'
-		url_params = []
-		if itemType:
-			url_params.append('itemType=' + itemType)
-		if organization:
-			url_params.append('organization=' + organization)
-		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.get(url)
+		return fortiedr_connection.send(url, adminSetTrayNotificationSettingsRequest)
 
-class Administrator:
-	'''The Administrator module enables administrators to perform administrative operations, such as handling licenses and users.'''
 
 	def list_collector_installers(self, organization: str = None) -> tuple[bool, None]:
 		'''
 		Class Administrator
 		Description: This API call output the available collectors installers.
         
 		Args:
@@ -2299,65 +2240,14 @@
 		if name:
 			url_params.append('name=' + name)
 		if organization:
 			url_params.append('organization=' + organization)
 		url += '?' + '&'.join(url_params)
 		return fortiedr_connection.send(url)
 
-	def create_ems_custom_installer(self, osType: str, aggregatorAddress: str = None, aggregatorPort: int = None, citrixPVS: bool = None, collectorGroup: str = None, collectorVersion: str = None, distro: str = None, is64bit: bool = None, organization: str = None, proxy: bool = None, vdi: bool = None) -> tuple[bool, None]:
-		'''
-		Class SystemInventory
-		Description: This API call sends request for creating custom-installer for EMS integration.
-        
-		Args:
-			aggregatorAddress (str): Specifies the aggregator ip or dns address.
-			aggregatorPort (int): Specifies the aggregator port.
-			citrixPVS (bool): Specifies whether the collector installed with citrix in pvs mode.
-			collectorGroup (str): Specifies the requested collector group.
-			collectorVersion (str): Specifies the requested collector version.
-			distro (str): Specifies the Linux distribution. For example: CentOS_6, CentOS_7, CentOS_8, CentOS_9, Amazon, Oracle_6, Oracle_7, Oracle_8, SLES_12, SLES_15, Ubuntu_16.04, Ubuntu_18.04, Ubuntu_20.04, Ubuntu_22.04.
-			is64bit (bool): Specifies the Windows os bit version.
-			organization (str): Specifies the requested organization.
-			osType (str): Specifies the operating system type.
-			proxy (bool): Specifies the system proxy settings (Only applies to Collector versions 3.1 and above).
-			vdi (bool): Specifies the VDI (Virtual Desktop Infrastructure) installation.
-
-		Returns:
-			bool: Status of the request (True or False). 
-			None: This function does not return any data.
-		'''
-		validate_params("create_ems_custom_installer", locals())
-
-		url = '/management-rest/inventory/create-ems-custom-installer'
-		url_params = []
-		if aggregatorAddress:
-			url_params.append('aggregatorAddress=' + aggregatorAddress)
-		if aggregatorPort:
-			url_params.append('aggregatorPort=' + aggregatorPort)
-		if citrixPVS:
-			url_params.append('citrixPVS=' + citrixPVS)
-		if collectorGroup:
-			url_params.append('collectorGroup=' + collectorGroup)
-		if collectorVersion:
-			url_params.append('collectorVersion=' + collectorVersion)
-		if distro:
-			url_params.append('distro=' + distro)
-		if is64bit:
-			url_params.append('is64bit=' + is64bit)
-		if organization:
-			url_params.append('organization=' + organization)
-		if osType:
-			url_params.append('osType=' + osType)
-		if proxy:
-			url_params.append('proxy=' + proxy)
-		if vdi:
-			url_params.append('vdi=' + vdi)
-		url += '?' + '&'.join(url_params)
-		return fortiedr_connection.send(url)
-
 	def delete_collectors(self, cloudAccounts: list = None, cloudProviders: list = None, clusters: list = None, collectorGroups: list = None, collectorGroupsIds: list = None, collectorType: str = None, confirmDeletion: bool = None, deleteAll: bool = None, devices: list = None, devicesIds: list = None, firstSeen: str = None, hasCrashDumps: bool = None, ips: list = None, itemsPerPage: int = None, lastSeenEnd: str = None, lastSeenStart: str = None, loggedUser: str = None, operatingSystems: list = None, organization: str = None, osFamilies: list = None, pageNumber: int = None, showExpired: bool = None, sorting: str = None, states: list = None, strictMode: bool = None, versions: list = None) -> tuple[bool, None]:
 		'''
 		Class SystemInventory
 		Description: This API call deletes a Collector(s).
         
 		Args:
 			cloudAccounts (list): Specifies the list cloud account names.
```

### Comparing `fortiedr-3.6.9/fortiedr.egg-info/PKG-INFO` & `fortiedr-3.7/fortiedr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortiedr
-Version: 3.6.9
+Version: 3.7
 Summary: This Fortiedr module is an open-source Python library that simplifies interaction with the FortiEDR Cloud API.
 Author: Rafael Foster
 Author-email: Rafael Foster <rafaelgfoster@gmail.com>
 Project-URL: Homepage, https://github.com/rafaelfoster/fortiedr
 Project-URL: Issues, https://github.com/rafaelfoster/fortiedr/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fortiedr-3.6.9/pyproject.toml` & `fortiedr-3.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fortiedr"
-version = "3.6.9"
+version = "3.7"
 authors = [
   { name="Rafael Foster", email="rafaelgfoster@gmail.com" }
 ]
 description = "This Fortiedr module is an open-source Python library that simplifies interaction with the FortiEDR Cloud API."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `fortiedr-3.6.9/setup.py` & `fortiedr-3.7/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 cur_dir = os.path.dirname(__file__)
 
 with open(f"{cur_dir}/requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="fortiedr",
-    version="3.6.9",
+    version="3.7",
     description="This Fortiedr module is an open-source Python library that simplifies interaction with the FortiEDR Cloud API.",
     author="Rafael Foster",
     author_email="rafaelgfoster@gmail.com",
     project_urls={
         "GitHub": "https://github.com/rafaelfoster/fortiedr",
     },
     python_requires=">=3.8",
```

