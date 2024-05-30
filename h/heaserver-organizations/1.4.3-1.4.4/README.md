# Comparing `tmp/heaserver_organizations-1.4.3.tar.gz` & `tmp/heaserver_organizations-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver_organizations-1.4.3.tar", last modified: Wed May 29 22:42:28 2024, max compression
+gzip compressed data, was "heaserver_organizations-1.4.4.tar", last modified: Thu May 30 21:37:49 2024, max compression
```

## Comparing `heaserver_organizations-1.4.3.tar` & `heaserver_organizations-1.4.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 22:42:28.911460 heaserver_organizations-1.4.3/
--rw-rw-rw-   0        0        0      261 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.3/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.3/.gitignore
--rw-rw-rw-   0        0        0     1663 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.3/Dockerfile
--rw-rw-rw-   0        0        0    11625 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.3/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.3/MANIFEST.in
--rw-rw-rw-   0        0        0     5772 2024-05-29 22:42:28.909459 heaserver_organizations-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     4349 2024-05-29 21:46:35.000000 heaserver_organizations-1.4.3/README.md
--rw-rw-rw-   0        0        0     1749 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.3/RELEASING.md
--rw-rw-rw-   0        0        0      594 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.3/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-05-29 22:42:28.668980 heaserver_organizations-1.4.3/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-05-29 22:42:28.669512 heaserver_organizations-1.4.3/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-29 22:42:28.812252 heaserver_organizations-1.4.3/integrationtests/heaserver/organizationintegrationtest/
--rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.3/integrationtests/heaserver/organizationintegrationtest/__init__.py
--rw-rw-rw-   0        0        0    10980 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.3/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py
--rw-rw-rw-   0        0        0      835 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.3/integrationtests/heaserver/organizationintegrationtest/test_all.py
--rw-rw-rw-   0        0        0    15050 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.3/integrationtests/heaserver/organizationintegrationtest/testcase.py
--rw-rw-rw-   0        0        0      111 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.3/pytest.ini
--rw-rw-rw-   0        0        0      362 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.3/requirements_dev.txt
--rw-rw-rw-   0        0        0     6574 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.3/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-05-29 22:42:28.911460 heaserver_organizations-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1931 2024-05-29 22:41:49.000000 heaserver_organizations-1.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-29 22:42:28.671629 heaserver_organizations-1.4.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-29 22:42:28.670570 heaserver_organizations-1.4.3/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-29 22:42:28.829071 heaserver_organizations-1.4.3/src/heaserver/organization/
--rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.3/src/heaserver/organization/__init__.py
--rw-rw-rw-   0        0        0    52582 2024-05-23 22:35:54.000000 heaserver_organizations-1.4.3/src/heaserver/organization/service.py
-drwxrwxrwx   0        0        0        0 2024-05-29 22:42:28.841800 heaserver_organizations-1.4.3/src/heaserver/organization/wstl/
--rw-rw-rw-   0        0        0    26704 2024-05-29 21:15:39.000000 heaserver_organizations-1.4.3/src/heaserver/organization/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-05-29 22:42:28.907937 heaserver_organizations-1.4.3/src/heaserver_organizations.egg-info/
--rw-rw-rw-   0        0        0     5772 2024-05-29 22:42:28.000000 heaserver_organizations-1.4.3/src/heaserver_organizations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      997 2024-05-29 22:42:28.000000 heaserver_organizations-1.4.3/src/heaserver_organizations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 22:42:28.000000 heaserver_organizations-1.4.3/src/heaserver_organizations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-05-29 22:42:28.000000 heaserver_organizations-1.4.3/src/heaserver_organizations.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2024-05-29 22:42:28.000000 heaserver_organizations-1.4.3/src/heaserver_organizations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-29 22:42:28.000000 heaserver_organizations-1.4.3/src/heaserver_organizations.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-29 22:42:28.672677 heaserver_organizations-1.4.3/tests/
-drwxrwxrwx   0        0        0        0 2024-05-29 22:42:28.672677 heaserver_organizations-1.4.3/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-29 22:42:28.905850 heaserver_organizations-1.4.3/tests/heaserver/organizationtest/
--rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.3/tests/heaserver/organizationtest/__init__.py
--rw-rw-rw-   0        0        0     2214 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.3/tests/heaserver/organizationtest/test_all.py
--rw-rw-rw-   0        0        0     7050 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.3/tests/heaserver/organizationtest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-05-30 21:37:49.736850 heaserver_organizations-1.4.4/
+-rw-rw-rw-   0        0        0      261 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.4/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.4/.gitignore
+-rw-rw-rw-   0        0        0     1663 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.4/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.4/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     6004 2024-05-30 21:37:49.735851 heaserver_organizations-1.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4581 2024-05-30 21:36:00.000000 heaserver_organizations-1.4.4/README.md
+-rw-rw-rw-   0        0        0     1749 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.4/RELEASING.md
+-rw-rw-rw-   0        0        0      594 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.4/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-05-30 21:37:49.558104 heaserver_organizations-1.4.4/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-05-30 21:37:49.558629 heaserver_organizations-1.4.4/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-30 21:37:49.661883 heaserver_organizations-1.4.4/integrationtests/heaserver/organizationintegrationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.4/integrationtests/heaserver/organizationintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0    10980 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.4/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py
+-rw-rw-rw-   0        0        0      835 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.4/integrationtests/heaserver/organizationintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0    15050 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.4/integrationtests/heaserver/organizationintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.4/pytest.ini
+-rw-rw-rw-   0        0        0      362 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.4/requirements_dev.txt
+-rw-rw-rw-   0        0        0     6574 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.4/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 21:37:49.737852 heaserver_organizations-1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1931 2024-05-30 21:36:59.000000 heaserver_organizations-1.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 21:37:49.560741 heaserver_organizations-1.4.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-30 21:37:49.560194 heaserver_organizations-1.4.4/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-30 21:37:49.664851 heaserver_organizations-1.4.4/src/heaserver/organization/
+-rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.4/src/heaserver/organization/__init__.py
+-rw-rw-rw-   0        0        0    53378 2024-05-30 21:23:17.000000 heaserver_organizations-1.4.4/src/heaserver/organization/service.py
+drwxrwxrwx   0        0        0        0 2024-05-30 21:37:49.674881 heaserver_organizations-1.4.4/src/heaserver/organization/wstl/
+-rw-rw-rw-   0        0        0    26704 2024-05-29 22:43:40.000000 heaserver_organizations-1.4.4/src/heaserver/organization/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-05-30 21:37:49.733851 heaserver_organizations-1.4.4/src/heaserver_organizations.egg-info/
+-rw-rw-rw-   0        0        0     6004 2024-05-30 21:37:49.000000 heaserver_organizations-1.4.4/src/heaserver_organizations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      997 2024-05-30 21:37:49.000000 heaserver_organizations-1.4.4/src/heaserver_organizations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 21:37:49.000000 heaserver_organizations-1.4.4/src/heaserver_organizations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-30 21:37:49.000000 heaserver_organizations-1.4.4/src/heaserver_organizations.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2024-05-30 21:37:49.000000 heaserver_organizations-1.4.4/src/heaserver_organizations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-30 21:37:49.000000 heaserver_organizations-1.4.4/src/heaserver_organizations.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 21:37:49.561802 heaserver_organizations-1.4.4/tests/
+drwxrwxrwx   0        0        0        0 2024-05-30 21:37:49.562333 heaserver_organizations-1.4.4/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-30 21:37:49.731881 heaserver_organizations-1.4.4/tests/heaserver/organizationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.4/tests/heaserver/organizationtest/__init__.py
+-rw-rw-rw-   0        0        0     2214 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.4/tests/heaserver/organizationtest/test_all.py
+-rw-rw-rw-   0        0        0     7050 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.4/tests/heaserver/organizationtest/testcase.py
```

### Comparing `heaserver_organizations-1.4.3/Dockerfile` & `heaserver_organizations-1.4.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.3/LICENSE` & `heaserver_organizations-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.3/PKG-INFO` & `heaserver_organizations-1.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-organizations
-Version: 1.4.3
+Version: 1.4.4
 Summary: a service for managing organization information for research laboratories and other research groups
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-organizations,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -30,14 +30,18 @@
 
 # HEA Server Organization
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Organization is a service for managing organization information for research laboratories and other research groups.
 
+## Version 1.4.4
+* Return 400 status code when the user lacks permission to update permissions for an organization (those errors were ignored previously).
+* Corrected permissions checking for organization managers and members.
+
 ## Version 1.4.3
 * Send the account ids and group id fields when submitting the members editor form.
 
 ## Version 1.4.2
 * Corrected heaobject.organization.Organization permissions.
 
 ## Version 1.4.1
```

### Comparing `heaserver_organizations-1.4.3/README.md` & `heaserver_organizations-1.4.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # HEA Server Organization
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Organization is a service for managing organization information for research laboratories and other research groups.
 
+## Version 1.4.4
+* Return 400 status code when the user lacks permission to update permissions for an organization (those errors were ignored previously).
+* Corrected permissions checking for organization managers and members.
+
 ## Version 1.4.3
 * Send the account ids and group id fields when submitting the members editor form.
 
 ## Version 1.4.2
 * Corrected heaobject.organization.Organization permissions.
 
 ## Version 1.4.1
```

### Comparing `heaserver_organizations-1.4.3/RELEASING.md` & `heaserver_organizations-1.4.4/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.3/docker-entrypoint.sh` & `heaserver_organizations-1.4.4/docker-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.3/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py` & `heaserver_organizations-1.4.4/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.3/integrationtests/heaserver/organizationintegrationtest/test_all.py` & `heaserver_organizations-1.4.4/integrationtests/heaserver/organizationintegrationtest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.3/integrationtests/heaserver/organizationintegrationtest/testcase.py` & `heaserver_organizations-1.4.4/integrationtests/heaserver/organizationintegrationtest/testcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.3/run-swaggerui.py` & `heaserver_organizations-1.4.4/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.3/setup.py` & `heaserver_organizations-1.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-organizations',
-    version='1.4.3',
+    version='1.4.4',
     description="a service for managing organization information for research laboratories and other research groups",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
```

### Comparing `heaserver_organizations-1.4.3/src/heaserver/organization/service.py` & `heaserver_organizations-1.4.4/src/heaserver/organization/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -890,26 +890,27 @@
     old_dict = await mongoservicelib.get_dict(request, MONGODB_ORGANIZATION_COLLECTION)
     if old_dict is not None:
         old_org = Organization()
         old_org.from_dict(old_dict)
         try:
             new_org = await new_heaobject_from_type(request, Organization)
         except DeserializeException as e:
-            return response.status_bad_request(str(e))
-        if (old_org.admin_ids != new_org.admin_ids or \
-            old_org.manager_ids != new_org.manager_ids or \
-                old_org.member_ids != new_org.member_ids or \
-                    old_org.principal_investigator_id != new_org.principal_investigator_id) and \
-                        not old_org.has_permissions(sub, [Permission.COOWNER]):
-            return response.status_bad_request('You have insufficient permissions to change organization membership')
-        if (old_org.admin_group_ids != new_org.admin_group_ids or \
-            old_org.manager_group_ids != new_org.manager_group_ids or \
-                old_org.member_group_ids != new_org.member_group_ids) and \
-                        not old_org.has_permissions(sub, [Permission.COOWNER]):
-            return response.status_bad_request('You have insufficient permissions to change organization group-membership mappings')
+            raise response.status_bad_request(str(e))
+        if old_org.admin_ids != new_org.admin_ids and old_org.is_attribute_read_only(sub, 'admin_ids'):
+            raise response.status_bad_request("You have insufficient permissions to change this organization's administrators")
+        if old_org.manager_ids != new_org.manager_ids and old_org.is_attribute_read_only(sub, 'manager_ids'):
+            raise response.status_bad_request("You have insufficient permissions to change this organization's managers")
+        if old_org.member_ids != new_org.member_ids and old_org.is_attribute_read_only(sub, 'member_ids'):
+            raise response.status_bad_request("You have insufficient permissions to change this organization's members")
+        if old_org.admin_group_ids != new_org.admin_group_ids and old_org.is_attribute_read_only(sub, 'admin_group_ids'):
+            raise response.status_bad_request("You have insufficient permissions to change this organization's admin group mappings")
+        if old_org.manager_group_ids != new_org.manager_group_ids and old_org.is_attribute_read_only(sub, 'manager_group_ids'):
+            raise response.status_bad_request("You have insufficient permissions to change this organization's manager group mappings")
+        if old_org.member_group_ids != new_org.member_group_ids and old_org.is_attribute_read_only(sub, 'member_group_ids'):
+            raise response.status_bad_request("You have insufficient permissions to change this organization's member group mappings")
 
         person_group_url: str | None = None
         async def get_person_group_url():
             nonlocal person_group_url
             async with Lock():
                 if person_group_url is None:
                     person_group_url = await type_to_resource_url(request, Person)
@@ -920,25 +921,25 @@
             nonlocal group_url
             async with Lock():
                 if group_url is None:
                     group_url = await type_to_resource_url(request, Group)
                 return group_url
 
         async def add_and_delete(old_group_ids: list[str], new_group_ids: list[str], user_ids: list[str]):
-            added_groups = set(new_group_ids).difference(old_group_ids)
+            added_group_id_strs = set(new_group_ids).difference(old_group_ids)
             deleted_group_id_strs = set(old_group_ids).difference(new_group_ids)
-            groups = [await client.get(request.app, URL(await get_group_url()) / group_id_str, Group) for group_id_str in deleted_group_id_strs]
+            groups = await gather(*[client.get(request.app, URL(await get_group_url()) / group_id_str, Group) for group_id_str in deleted_group_id_strs])
             for group in groups:
                 if group.group_type != GroupType.ORGANIZATION:
                     deleted_group_id_strs.remove(group.id)
             coros = []
             for user_id in user_ids:
                 coros.append(_update_group_membership(request,
                                                     user_id,
-                                                    added_groups,
+                                                    added_group_id_strs,
                                                     deleted_group_id_strs,
                                                     get_person_group_url))
             await gather(*coros)
 
         await gather(
             add_and_delete(old_org.member_group_ids,
                            new_org.member_group_ids,
@@ -994,14 +995,16 @@
             changed.old_account_ids = []
             changed.new_account_ids = new_org.account_ids
             changed.group_ids = group_ids
             changed.user_id = user_id
             changed.new_organization_display_name = new_org.display_name
             coros.append(_update_volumes_and_credentials(request, changed))
         await gather(*coros)
+    else:
+        raise response.status_not_found()
 
 
 async def _update_volumes_and_credentials(request: web.Request, changed: _OrganizationPermissionsChanged):
     logger = logging.getLogger(__name__)
     logger.debug('Updating volumes and credentials %s', changed)
     app = request.app
     sub = request.headers.get(SUB, NONE_USER)
@@ -1034,49 +1037,54 @@
         async def accounts_needing_updates_coro():
             logger.debug('Updating credentials for accounts %s for person %s', accounts_needing_updates, person.id)
             awaitables_: list[Awaitable] = []
             volumes_to_update = await client.get_all_list(app, volume_url, Volume,
                                                     query_params=_account_query_params(accounts_needing_updates),
                                                     headers=_sub_header)
             volumes_for_current_user = [v for v in volumes_to_update if v.has_permissions(person.id, RESTPermissionGroup.GETTER_PERMS)]
-            awaitables_.append(gather(*[_update_volume_and_credentials(request, account_view_url, volume, credential_id, person, groups,
-                                                          changed.new_organization_display_name) \
-                        for volume, credential_id in ((volume, volume.credential_id) for volume in volumes_for_current_user)]))
+            awaitables_.extend(_update_volume_and_credentials(request, account_view_url, volume, credential_id, person, groups,
+                                                          changed.new_organization_display_name, volume_url) \
+                        for volume, credential_id in ((volume, volume.credential_id) for volume in volumes_for_current_user))
             accounts_missing_a_volume = accounts_needing_updates.difference(v.account_id for v in volumes_for_current_user)
+            account_views_by_account_id: dict[str, AccountView] = {}
             for acct_id in accounts_missing_a_volume:
                 logger.warn('Replacing missing volume for account %s for user %s', acct_id, person.id)
-                account_view = await client.get(app, account_view_url / acct_id, AccountView, headers=acct_headers)
-                awaitable = _new_volume_and_credentials(request, account_view, person, groups, changed.new_organization_display_name)
-                awaitables_.append(awaitable)
+                async def replace_missing_volume(account_id):
+                    if (account_view := account_views_by_account_id.get(account_id)) is None:
+                        account_view = await client.get(app, account_view_url / account_id, AccountView, headers=acct_headers)
+                        account_views_by_account_id[account_id] = account_view
+                    await _new_volume_and_credentials(request, account_view, person, groups, changed.new_organization_display_name, volume_url)
+                awaitables_.append(replace_missing_volume(acct_id))
             await gather(*awaitables_)
         awaitables.append(accounts_needing_updates_coro())
 
     if added_accounts := set(changed.new_account_ids).difference(changed.old_account_ids):
         async def added_accounts_coro():
             logger.debug('Creating new volumes and credentials for accounts %s for user %s', added_accounts, person.id)
             awaitables_: list[Awaitable] = []
             async for account_view in client.get_all(app, account_view_url, AccountView,
                                                     query_params=_account_query_params(added_accounts),
                                                     headers=acct_headers):
-                awaitable = _new_volume_and_credentials(request, account_view, person, groups, changed.new_organization_display_name)
+                awaitable = _new_volume_and_credentials(request, account_view, person, groups, changed.new_organization_display_name, volume_url)
                 awaitables_.append(awaitable)
             await gather(*awaitables_)
         awaitables.append(added_accounts_coro())
     await gather(*awaitables)
 
 def _account_query_params(account_ids: Sequence[str]) -> MultiDict[str, str]:
     return MultiDict(('account_id', account_id) for account_id in account_ids)
 
 async def _update_volume_and_credentials(request: web.Request,
                                          account_view_url: URL,
                                          volume: Volume,
                                          credential_id: str,
                                          person: Person,
                                          groups: Sequence[Group],
-                                         organization_display_name: str | None):
+                                         organization_display_name: str | None,
+                                         volume_url: URL):
     logger = logging.getLogger(__name__)
     sub = request.headers.get(SUB, NONE_USER)
     app = request.app
     credentials_url = URL(await client.get_resource_url(app, volume.credential_type_name))
     credential, account_view = await gather(
         client.get(app,
                    credentials_url / credential_id,
@@ -1112,15 +1120,14 @@
     else:
         credential.role = actual_account.get_role_to_assume(person, groups)
         credential.display_name = _credentials_display_name(actual_account, organization_display_name)
         credential.expiration = None
         credential.temporary = True
         credential.name = f'{person.id}_{actual_account.type}_{actual_account.id}'
         await client.put(app, credentials_url / credential.id, credential, headers=_sub_header)
-    volume_url = URL(await client.get_resource_url(app, Volume))
     await client.put(app, volume_url / volume.id, volume, headers=_sub_header)
 
 async def _delete_volume_and_credentials(app: web.Application,
                                          volume_url: URL,
                                          volume: Volume,
                                          credential_id: str):
     try:
@@ -1131,20 +1138,20 @@
         if e.status != 404:
             raise e
 
 async def _new_volume_and_credentials(request: web.Request,
                                       account_view: AccountView,
                                       person: Person,
                                       groups: Sequence[Group],
-                                      organization_display_name: str | None) -> Awaitable[None]:
+                                      organization_display_name: str | None,
+                                      volume_url: URL):
     sub = request.headers.get(SUB, NONE_USER)
     app = request.app
-    volumes_url = URL(await client.get_resource_url(app, Volume))
     volume_name = _volume_name(account_view, person)
-    volume = await client.get(app, volumes_url / 'byname' / volume_name, Volume, headers=_sub_header)
+    volume = await client.get(app, volume_url / 'byname' / volume_name, Volume, headers=_sub_header)
     if volume is None or volume.owner != CREDENTIALS_MANAGER_USER:
         volume = Volume()
         volume_exists = False
         volume.owner = CREDENTIALS_MANAGER_USER
         share = ShareImpl()
         share.user = person.id
         share.add_permission(Permission.VIEWER)
@@ -1172,46 +1179,43 @@
         existing_credentials.name = new_credentials.name
         existing_credentials.display_name = _credentials_display_name(actual_account, organization_display_name)
         existing_credentials.temporary = True
         existing_credentials.expiration = None
         await client.put(app, credentials_url / existing_credentials.id, existing_credentials, headers=_sub_header)
     else:
         new_credential_url = await client.post(app, credentials_url, new_credentials, headers=_sub_header)
-        id_ = new_credential_url[new_credential_url.rindex('/') + 1:]
-        volume.credential_id = (await client.get(app,
-                                                credentials_url / id_,
-                                                type(new_credentials), headers=_sub_header)).id
+        volume.credential_id = new_credential_url[new_credential_url.rindex('/') + 1:]
     volume.credential_type_name = new_credentials.type
     if volume_exists:
-        await client.put(app, volumes_url / volume.id, volume, headers=_sub_header)
+        await client.put(app, volume_url / volume.id, volume, headers=_sub_header)
     else:
-        await client.post(app, volumes_url, volume, headers=_sub_header)
+        await client.post(app, volume_url, volume, headers=_sub_header)
 
 def _volume_display_name(account_view):
     return f'{account_view.type_display_name} {account_view.display_name}'
 
 def _volume_name(account_view, person):
     return f'{person.id}_{account_view.id}'
 
 def _credentials_display_name(account: AWSAccount, organization_display_name: str | None):
     return f'{account.display_name} - {organization_display_name}'
 
 async def _update_group_membership(request: web.Request,
                                    user: str,
-                                   added_groups: list[str],
-                                   deleted_groups: list[str],
-                                   group_url_getter: Callable[[], Coroutine[None, None, str]]):
+                                   added_group_ids: Sequence[str],
+                                   deleted_group_ids: Sequence[str],
+                                   group_url_getter: Callable[[], Coroutine[None, None, None]]):
     coros = []
     group_url = URL(await group_url_getter())
     async def delete(deleted_group):
         try:
             await client.delete(request.app, group_url / user / 'groups' / deleted_group, headers={SUB: CREDENTIALS_MANAGER_USER})
         except ClientResponseError as e:
             if e.status != 404:
                 raise e
-    for deleted_group in deleted_groups:
-        coros.append(delete(deleted_group))
-    for added_group in added_groups:
+    for deleted_group_id in deleted_group_ids:
+        coros.append(delete(deleted_group_id))
+    for added_group_id in added_group_ids:
         group = Group()
-        group.id = added_group
+        group.id = added_group_id
         coros.append(client.post(request.app, group_url / user / 'groups', group, headers={SUB: CREDENTIALS_MANAGER_USER}))
     await gather(*coros)
```

### Comparing `heaserver_organizations-1.4.3/src/heaserver/organization/wstl/all.json` & `heaserver_organizations-1.4.4/src/heaserver/organization/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.3/src/heaserver_organizations.egg-info/PKG-INFO` & `heaserver_organizations-1.4.4/src/heaserver_organizations.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-organizations
-Version: 1.4.3
+Version: 1.4.4
 Summary: a service for managing organization information for research laboratories and other research groups
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-organizations,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -30,14 +30,18 @@
 
 # HEA Server Organization
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Organization is a service for managing organization information for research laboratories and other research groups.
 
+## Version 1.4.4
+* Return 400 status code when the user lacks permission to update permissions for an organization (those errors were ignored previously).
+* Corrected permissions checking for organization managers and members.
+
 ## Version 1.4.3
 * Send the account ids and group id fields when submitting the members editor form.
 
 ## Version 1.4.2
 * Corrected heaobject.organization.Organization permissions.
 
 ## Version 1.4.1
```

### Comparing `heaserver_organizations-1.4.3/src/heaserver_organizations.egg-info/SOURCES.txt` & `heaserver_organizations-1.4.4/src/heaserver_organizations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.3/tests/heaserver/organizationtest/test_all.py` & `heaserver_organizations-1.4.4/tests/heaserver/organizationtest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.3/tests/heaserver/organizationtest/testcase.py` & `heaserver_organizations-1.4.4/tests/heaserver/organizationtest/testcase.py`

 * *Files identical despite different names*

