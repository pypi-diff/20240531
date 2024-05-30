# Comparing `tmp/heaserver_organizations-1.4.4.tar.gz` & `tmp/heaserver_organizations-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver_organizations-1.4.4.tar", last modified: Thu May 30 21:37:49 2024, max compression
+gzip compressed data, was "heaserver_organizations-1.4.5.tar", last modified: Thu May 30 22:33:28 2024, max compression
```

## Comparing `heaserver_organizations-1.4.4.tar` & `heaserver_organizations-1.4.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 21:37:49.736850 heaserver_organizations-1.4.4/
--rw-rw-rw-   0        0        0      261 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.4/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.4/.gitignore
--rw-rw-rw-   0        0        0     1663 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.4/Dockerfile
--rw-rw-rw-   0        0        0    11625 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.4/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.4/MANIFEST.in
--rw-rw-rw-   0        0        0     6004 2024-05-30 21:37:49.735851 heaserver_organizations-1.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     4581 2024-05-30 21:36:00.000000 heaserver_organizations-1.4.4/README.md
--rw-rw-rw-   0        0        0     1749 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.4/RELEASING.md
--rw-rw-rw-   0        0        0      594 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.4/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-05-30 21:37:49.558104 heaserver_organizations-1.4.4/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-05-30 21:37:49.558629 heaserver_organizations-1.4.4/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-30 21:37:49.661883 heaserver_organizations-1.4.4/integrationtests/heaserver/organizationintegrationtest/
--rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.4/integrationtests/heaserver/organizationintegrationtest/__init__.py
--rw-rw-rw-   0        0        0    10980 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.4/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py
--rw-rw-rw-   0        0        0      835 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.4/integrationtests/heaserver/organizationintegrationtest/test_all.py
--rw-rw-rw-   0        0        0    15050 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.4/integrationtests/heaserver/organizationintegrationtest/testcase.py
--rw-rw-rw-   0        0        0      111 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.4/pytest.ini
--rw-rw-rw-   0        0        0      362 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.4/requirements_dev.txt
--rw-rw-rw-   0        0        0     6574 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.4/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-05-30 21:37:49.737852 heaserver_organizations-1.4.4/setup.cfg
--rw-rw-rw-   0        0        0     1931 2024-05-30 21:36:59.000000 heaserver_organizations-1.4.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-30 21:37:49.560741 heaserver_organizations-1.4.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-30 21:37:49.560194 heaserver_organizations-1.4.4/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-30 21:37:49.664851 heaserver_organizations-1.4.4/src/heaserver/organization/
--rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.4/src/heaserver/organization/__init__.py
--rw-rw-rw-   0        0        0    53378 2024-05-30 21:23:17.000000 heaserver_organizations-1.4.4/src/heaserver/organization/service.py
-drwxrwxrwx   0        0        0        0 2024-05-30 21:37:49.674881 heaserver_organizations-1.4.4/src/heaserver/organization/wstl/
--rw-rw-rw-   0        0        0    26704 2024-05-29 22:43:40.000000 heaserver_organizations-1.4.4/src/heaserver/organization/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-05-30 21:37:49.733851 heaserver_organizations-1.4.4/src/heaserver_organizations.egg-info/
--rw-rw-rw-   0        0        0     6004 2024-05-30 21:37:49.000000 heaserver_organizations-1.4.4/src/heaserver_organizations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      997 2024-05-30 21:37:49.000000 heaserver_organizations-1.4.4/src/heaserver_organizations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 21:37:49.000000 heaserver_organizations-1.4.4/src/heaserver_organizations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-05-30 21:37:49.000000 heaserver_organizations-1.4.4/src/heaserver_organizations.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2024-05-30 21:37:49.000000 heaserver_organizations-1.4.4/src/heaserver_organizations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-30 21:37:49.000000 heaserver_organizations-1.4.4/src/heaserver_organizations.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-30 21:37:49.561802 heaserver_organizations-1.4.4/tests/
-drwxrwxrwx   0        0        0        0 2024-05-30 21:37:49.562333 heaserver_organizations-1.4.4/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-30 21:37:49.731881 heaserver_organizations-1.4.4/tests/heaserver/organizationtest/
--rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.4/tests/heaserver/organizationtest/__init__.py
--rw-rw-rw-   0        0        0     2214 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.4/tests/heaserver/organizationtest/test_all.py
--rw-rw-rw-   0        0        0     7050 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.4/tests/heaserver/organizationtest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-05-30 22:33:28.132829 heaserver_organizations-1.4.5/
+-rw-rw-rw-   0        0        0      261 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.5/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.5/.gitignore
+-rw-rw-rw-   0        0        0     1663 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.5/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.5/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     6138 2024-05-30 22:33:28.131830 heaserver_organizations-1.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4715 2024-05-30 22:31:03.000000 heaserver_organizations-1.4.5/README.md
+-rw-rw-rw-   0        0        0     1749 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.5/RELEASING.md
+-rw-rw-rw-   0        0        0      594 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.5/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-05-30 22:33:27.941459 heaserver_organizations-1.4.5/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-05-30 22:33:27.941459 heaserver_organizations-1.4.5/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-30 22:33:28.051718 heaserver_organizations-1.4.5/integrationtests/heaserver/organizationintegrationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.5/integrationtests/heaserver/organizationintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0    10980 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.5/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py
+-rw-rw-rw-   0        0        0      835 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.5/integrationtests/heaserver/organizationintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0    15050 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.5/integrationtests/heaserver/organizationintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.5/pytest.ini
+-rw-rw-rw-   0        0        0      362 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.5/requirements_dev.txt
+-rw-rw-rw-   0        0        0     6574 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.5/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 22:33:28.132829 heaserver_organizations-1.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     1931 2024-05-30 22:32:53.000000 heaserver_organizations-1.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 22:33:27.943456 heaserver_organizations-1.4.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-30 22:33:27.942456 heaserver_organizations-1.4.5/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-30 22:33:28.057719 heaserver_organizations-1.4.5/src/heaserver/organization/
+-rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.5/src/heaserver/organization/__init__.py
+-rw-rw-rw-   0        0        0    53476 2024-05-30 22:28:05.000000 heaserver_organizations-1.4.5/src/heaserver/organization/service.py
+drwxrwxrwx   0        0        0        0 2024-05-30 22:33:28.067748 heaserver_organizations-1.4.5/src/heaserver/organization/wstl/
+-rw-rw-rw-   0        0        0    26704 2024-05-30 21:38:57.000000 heaserver_organizations-1.4.5/src/heaserver/organization/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-05-30 22:33:28.129829 heaserver_organizations-1.4.5/src/heaserver_organizations.egg-info/
+-rw-rw-rw-   0        0        0     6138 2024-05-30 22:33:27.000000 heaserver_organizations-1.4.5/src/heaserver_organizations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      997 2024-05-30 22:33:27.000000 heaserver_organizations-1.4.5/src/heaserver_organizations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 22:33:27.000000 heaserver_organizations-1.4.5/src/heaserver_organizations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-30 22:33:27.000000 heaserver_organizations-1.4.5/src/heaserver_organizations.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2024-05-30 22:33:27.000000 heaserver_organizations-1.4.5/src/heaserver_organizations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-30 22:33:27.000000 heaserver_organizations-1.4.5/src/heaserver_organizations.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 22:33:27.944456 heaserver_organizations-1.4.5/tests/
+drwxrwxrwx   0        0        0        0 2024-05-30 22:33:27.945457 heaserver_organizations-1.4.5/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-30 22:33:28.127676 heaserver_organizations-1.4.5/tests/heaserver/organizationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.5/tests/heaserver/organizationtest/__init__.py
+-rw-rw-rw-   0        0        0     2214 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.5/tests/heaserver/organizationtest/test_all.py
+-rw-rw-rw-   0        0        0     7050 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.5/tests/heaserver/organizationtest/testcase.py
```

### Comparing `heaserver_organizations-1.4.4/Dockerfile` & `heaserver_organizations-1.4.5/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.4/LICENSE` & `heaserver_organizations-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.4/PKG-INFO` & `heaserver_organizations-1.4.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-organizations
-Version: 1.4.4
+Version: 1.4.5
 Summary: a service for managing organization information for research laboratories and other research groups
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-organizations,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -30,14 +30,17 @@
 
 # HEA Server Organization
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Organization is a service for managing organization information for research laboratories and other research groups.
 
+## Version 1.4.5
+* Fixed crash when reusing an existing volume and credentials when a user's organization membership has changed.
+
 ## Version 1.4.4
 * Return 400 status code when the user lacks permission to update permissions for an organization (those errors were ignored previously).
 * Corrected permissions checking for organization managers and members.
 
 ## Version 1.4.3
 * Send the account ids and group id fields when submitting the members editor form.
```

### Comparing `heaserver_organizations-1.4.4/README.md` & `heaserver_organizations-1.4.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # HEA Server Organization
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Organization is a service for managing organization information for research laboratories and other research groups.
 
+## Version 1.4.5
+* Fixed crash when reusing an existing volume and credentials when a user's organization membership has changed.
+
 ## Version 1.4.4
 * Return 400 status code when the user lacks permission to update permissions for an organization (those errors were ignored previously).
 * Corrected permissions checking for organization managers and members.
 
 ## Version 1.4.3
 * Send the account ids and group id fields when submitting the members editor form.
```

### Comparing `heaserver_organizations-1.4.4/RELEASING.md` & `heaserver_organizations-1.4.5/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.4/docker-entrypoint.sh` & `heaserver_organizations-1.4.5/docker-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.4/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py` & `heaserver_organizations-1.4.5/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.4/integrationtests/heaserver/organizationintegrationtest/test_all.py` & `heaserver_organizations-1.4.5/integrationtests/heaserver/organizationintegrationtest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.4/integrationtests/heaserver/organizationintegrationtest/testcase.py` & `heaserver_organizations-1.4.5/integrationtests/heaserver/organizationintegrationtest/testcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.4/run-swaggerui.py` & `heaserver_organizations-1.4.5/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.4/setup.py` & `heaserver_organizations-1.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-organizations',
-    version='1.4.4',
+    version='1.4.5',
     description="a service for managing organization information for research laboratories and other research groups",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
```

### Comparing `heaserver_organizations-1.4.4/src/heaserver/organization/service.py` & `heaserver_organizations-1.4.5/src/heaserver/organization/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1165,14 +1165,17 @@
     volume.file_system_name = account_view.file_system_name
     account_url_str = await client.get_resource_url(app, account_view.actual_object_type_name)
     actual_account = await client.get(app, URL(account_url_str) / account_view.actual_object_id, type_or_obj=Account,
                                       headers={SUB: sub, hdrs.AUTHORIZATION: request.headers[hdrs.AUTHORIZATION]})
     new_credentials = actual_account.new_credentials(person, groups)
     new_credentials.display_name = _credentials_display_name(actual_account, organization_display_name)
     new_credentials.owner = CREDENTIALS_MANAGER_USER
+    share = ShareImpl()
+    share.user = person.id
+    share.add_permission(Permission.VIEWER)
     new_credentials.add_share(share)
     new_credentials.temporary = True
     credentials_url = URL(await client.get_resource_url(app, type(new_credentials)))
     existing_credentials = await client.get(app, credentials_url / 'byname' / new_credentials.name,
                                             type(new_credentials), headers=_sub_header)
     if existing_credentials is not None and existing_credentials.owner == CREDENTIALS_MANAGER_USER:
         volume.credential_id = existing_credentials.id
```

### Comparing `heaserver_organizations-1.4.4/src/heaserver/organization/wstl/all.json` & `heaserver_organizations-1.4.5/src/heaserver/organization/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.4/src/heaserver_organizations.egg-info/PKG-INFO` & `heaserver_organizations-1.4.5/src/heaserver_organizations.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-organizations
-Version: 1.4.4
+Version: 1.4.5
 Summary: a service for managing organization information for research laboratories and other research groups
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-organizations,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -30,14 +30,17 @@
 
 # HEA Server Organization
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Organization is a service for managing organization information for research laboratories and other research groups.
 
+## Version 1.4.5
+* Fixed crash when reusing an existing volume and credentials when a user's organization membership has changed.
+
 ## Version 1.4.4
 * Return 400 status code when the user lacks permission to update permissions for an organization (those errors were ignored previously).
 * Corrected permissions checking for organization managers and members.
 
 ## Version 1.4.3
 * Send the account ids and group id fields when submitting the members editor form.
```

### Comparing `heaserver_organizations-1.4.4/src/heaserver_organizations.egg-info/SOURCES.txt` & `heaserver_organizations-1.4.5/src/heaserver_organizations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.4/tests/heaserver/organizationtest/test_all.py` & `heaserver_organizations-1.4.5/tests/heaserver/organizationtest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.4/tests/heaserver/organizationtest/testcase.py` & `heaserver_organizations-1.4.5/tests/heaserver/organizationtest/testcase.py`

 * *Files identical despite different names*

