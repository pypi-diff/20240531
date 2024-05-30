# Comparing `tmp/heaobject-1.6.1.tar.gz` & `tmp/heaobject-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaobject-1.6.1.tar", last modified: Thu May 23 21:43:23 2024, max compression
+gzip compressed data, was "heaobject-1.6.2.tar", last modified: Thu May 30 23:14:49 2024, max compression
```

## Comparing `heaobject-1.6.1.tar` & `heaobject-1.6.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 21:43:23.833848 heaobject-1.6.1/
--rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:08.000000 heaobject-1.6.1/LICENSE
--rw-rw-rw-   0        0        0     6203 2024-05-23 21:43:23.831848 heaobject-1.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     4697 2024-05-23 21:42:03.000000 heaobject-1.6.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-23 21:43:23.833848 heaobject-1.6.1/setup.cfg
--rw-rw-rw-   0        0        0     2603 2024-05-23 21:42:51.000000 heaobject-1.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 21:43:23.770849 heaobject-1.6.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-23 21:43:23.822847 heaobject-1.6.1/src/heaobject/
--rw-rw-rw-   0        0        0     1247 2023-12-16 22:23:08.000000 heaobject-1.6.1/src/heaobject/__init__.py
--rw-rw-rw-   0        0        0    11351 2024-05-21 22:51:17.000000 heaobject-1.6.1/src/heaobject/account.py
--rw-rw-rw-   0        0        0    15629 2024-04-09 20:34:56.000000 heaobject-1.6.1/src/heaobject/activity.py
--rw-rw-rw-   0        0        0     4030 2023-12-16 22:23:08.000000 heaobject-1.6.1/src/heaobject/aws.py
--rw-rw-rw-   0        0        0     6945 2023-12-16 22:23:08.000000 heaobject-1.6.1/src/heaobject/awss3key.py
--rw-rw-rw-   0        0        0     7587 2024-04-09 20:34:56.000000 heaobject-1.6.1/src/heaobject/bucket.py
--rw-rw-rw-   0        0        0     9988 2024-05-21 22:51:17.000000 heaobject-1.6.1/src/heaobject/data.py
--rw-rw-rw-   0        0        0     2604 2023-12-16 22:23:08.000000 heaobject-1.6.1/src/heaobject/dataadapter.py
--rw-rw-rw-   0        0        0      272 2022-03-11 01:28:08.000000 heaobject-1.6.1/src/heaobject/dataelement.py
--rw-rw-rw-   0        0        0     1601 2022-03-11 01:28:08.000000 heaobject-1.6.1/src/heaobject/datamodel.py
--rw-rw-rw-   0        0        0      430 2022-03-11 01:28:08.000000 heaobject-1.6.1/src/heaobject/datapattern.py
--rw-rw-rw-   0        0        0      238 2023-12-16 22:23:08.000000 heaobject-1.6.1/src/heaobject/datatransform.py
--rw-rw-rw-   0        0        0      353 2023-12-16 22:23:08.000000 heaobject-1.6.1/src/heaobject/error.py
--rw-rw-rw-   0        0        0    22016 2024-04-09 20:34:56.000000 heaobject-1.6.1/src/heaobject/folder.py
--rw-rw-rw-   0        0        0     4566 2024-05-21 22:51:17.000000 heaobject-1.6.1/src/heaobject/keychain.py
--rw-rw-rw-   0        0        0     2859 2024-04-09 20:34:56.000000 heaobject-1.6.1/src/heaobject/mimetype.py
--rw-rw-rw-   0        0        0    11772 2024-05-23 19:02:21.000000 heaobject-1.6.1/src/heaobject/organization.py
--rw-rw-rw-   0        0        0    13108 2024-05-21 22:51:17.000000 heaobject-1.6.1/src/heaobject/person.py
--rw-rw-rw-   0        0        0     5129 2024-04-09 20:34:56.000000 heaobject-1.6.1/src/heaobject/project.py
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:08.000000 heaobject-1.6.1/src/heaobject/py.typed
--rw-rw-rw-   0        0        0      211 2024-04-09 20:34:56.000000 heaobject-1.6.1/src/heaobject/record.py
--rw-rw-rw-   0        0        0    23400 2024-05-21 22:51:17.000000 heaobject-1.6.1/src/heaobject/registry.py
--rw-rw-rw-   0        0        0    80257 2024-04-24 17:43:21.000000 heaobject-1.6.1/src/heaobject/root.py
--rw-rw-rw-   0        0        0      597 2024-04-09 20:34:56.000000 heaobject-1.6.1/src/heaobject/settings.py
--rw-rw-rw-   0        0        0       66 2024-03-26 22:41:59.000000 heaobject-1.6.1/src/heaobject/source.py
--rw-rw-rw-   0        0        0     1165 2023-12-16 22:23:08.000000 heaobject-1.6.1/src/heaobject/source2target.py
--rw-rw-rw-   0        0        0     4074 2024-04-09 20:34:56.000000 heaobject-1.6.1/src/heaobject/storage.py
--rw-rw-rw-   0        0        0    10289 2024-04-18 02:00:20.000000 heaobject-1.6.1/src/heaobject/trash.py
--rw-rw-rw-   0        0        0     1217 2024-05-21 22:51:17.000000 heaobject-1.6.1/src/heaobject/user.py
--rw-rw-rw-   0        0        0      498 2023-12-16 22:23:08.000000 heaobject-1.6.1/src/heaobject/util.py
--rw-rw-rw-   0        0        0     7290 2024-05-21 22:51:17.000000 heaobject-1.6.1/src/heaobject/volume.py
-drwxrwxrwx   0        0        0        0 2024-05-23 21:43:23.830848 heaobject-1.6.1/src/heaobject.egg-info/
--rw-rw-rw-   0        0        0     6203 2024-05-23 21:43:23.000000 heaobject-1.6.1/src/heaobject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      995 2024-05-23 21:43:23.000000 heaobject-1.6.1/src/heaobject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 21:43:23.000000 heaobject-1.6.1/src/heaobject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2024-05-23 21:43:23.000000 heaobject-1.6.1/src/heaobject.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-23 21:43:23.000000 heaobject-1.6.1/src/heaobject.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 23:14:49.893928 heaobject-1.6.2/
+-rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:08.000000 heaobject-1.6.2/LICENSE
+-rw-rw-rw-   0        0        0     6314 2024-05-30 23:14:49.892929 heaobject-1.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4808 2024-05-30 23:13:21.000000 heaobject-1.6.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-30 23:14:49.893928 heaobject-1.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     2603 2024-05-30 23:14:29.000000 heaobject-1.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 23:14:49.835929 heaobject-1.6.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-30 23:14:49.882929 heaobject-1.6.2/src/heaobject/
+-rw-rw-rw-   0        0        0     1247 2023-12-16 22:23:08.000000 heaobject-1.6.2/src/heaobject/__init__.py
+-rw-rw-rw-   0        0        0    11343 2024-05-30 23:08:07.000000 heaobject-1.6.2/src/heaobject/account.py
+-rw-rw-rw-   0        0        0    15629 2024-04-09 20:34:56.000000 heaobject-1.6.2/src/heaobject/activity.py
+-rw-rw-rw-   0        0        0     4030 2023-12-16 22:23:08.000000 heaobject-1.6.2/src/heaobject/aws.py
+-rw-rw-rw-   0        0        0     6945 2023-12-16 22:23:08.000000 heaobject-1.6.2/src/heaobject/awss3key.py
+-rw-rw-rw-   0        0        0     7587 2024-04-09 20:34:56.000000 heaobject-1.6.2/src/heaobject/bucket.py
+-rw-rw-rw-   0        0        0     9988 2024-05-21 22:51:17.000000 heaobject-1.6.2/src/heaobject/data.py
+-rw-rw-rw-   0        0        0     2604 2023-12-16 22:23:08.000000 heaobject-1.6.2/src/heaobject/dataadapter.py
+-rw-rw-rw-   0        0        0      272 2022-03-11 01:28:08.000000 heaobject-1.6.2/src/heaobject/dataelement.py
+-rw-rw-rw-   0        0        0     1601 2022-03-11 01:28:08.000000 heaobject-1.6.2/src/heaobject/datamodel.py
+-rw-rw-rw-   0        0        0      430 2022-03-11 01:28:08.000000 heaobject-1.6.2/src/heaobject/datapattern.py
+-rw-rw-rw-   0        0        0      238 2023-12-16 22:23:08.000000 heaobject-1.6.2/src/heaobject/datatransform.py
+-rw-rw-rw-   0        0        0      353 2023-12-16 22:23:08.000000 heaobject-1.6.2/src/heaobject/error.py
+-rw-rw-rw-   0        0        0    22016 2024-04-09 20:34:56.000000 heaobject-1.6.2/src/heaobject/folder.py
+-rw-rw-rw-   0        0        0     4566 2024-05-21 22:51:17.000000 heaobject-1.6.2/src/heaobject/keychain.py
+-rw-rw-rw-   0        0        0     2859 2024-04-09 20:34:56.000000 heaobject-1.6.2/src/heaobject/mimetype.py
+-rw-rw-rw-   0        0        0    11772 2024-05-23 21:44:05.000000 heaobject-1.6.2/src/heaobject/organization.py
+-rw-rw-rw-   0        0        0    13108 2024-05-21 22:51:17.000000 heaobject-1.6.2/src/heaobject/person.py
+-rw-rw-rw-   0        0        0     5129 2024-04-09 20:34:56.000000 heaobject-1.6.2/src/heaobject/project.py
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:08.000000 heaobject-1.6.2/src/heaobject/py.typed
+-rw-rw-rw-   0        0        0      211 2024-04-09 20:34:56.000000 heaobject-1.6.2/src/heaobject/record.py
+-rw-rw-rw-   0        0        0    23400 2024-05-21 22:51:17.000000 heaobject-1.6.2/src/heaobject/registry.py
+-rw-rw-rw-   0        0        0    80257 2024-04-24 17:43:21.000000 heaobject-1.6.2/src/heaobject/root.py
+-rw-rw-rw-   0        0        0      597 2024-04-09 20:34:56.000000 heaobject-1.6.2/src/heaobject/settings.py
+-rw-rw-rw-   0        0        0       66 2024-03-26 22:41:59.000000 heaobject-1.6.2/src/heaobject/source.py
+-rw-rw-rw-   0        0        0     1165 2023-12-16 22:23:08.000000 heaobject-1.6.2/src/heaobject/source2target.py
+-rw-rw-rw-   0        0        0     4074 2024-04-09 20:34:56.000000 heaobject-1.6.2/src/heaobject/storage.py
+-rw-rw-rw-   0        0        0    10289 2024-04-18 02:00:20.000000 heaobject-1.6.2/src/heaobject/trash.py
+-rw-rw-rw-   0        0        0     1217 2024-05-21 22:51:17.000000 heaobject-1.6.2/src/heaobject/user.py
+-rw-rw-rw-   0        0        0      498 2023-12-16 22:23:08.000000 heaobject-1.6.2/src/heaobject/util.py
+-rw-rw-rw-   0        0        0     7290 2024-05-21 22:51:17.000000 heaobject-1.6.2/src/heaobject/volume.py
+drwxrwxrwx   0        0        0        0 2024-05-30 23:14:49.890929 heaobject-1.6.2/src/heaobject.egg-info/
+-rw-rw-rw-   0        0        0     6314 2024-05-30 23:14:49.000000 heaobject-1.6.2/src/heaobject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      995 2024-05-30 23:14:49.000000 heaobject-1.6.2/src/heaobject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 23:14:49.000000 heaobject-1.6.2/src/heaobject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-05-30 23:14:49.000000 heaobject-1.6.2/src/heaobject.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-30 23:14:49.000000 heaobject-1.6.2/src/heaobject.egg-info/top_level.txt
```

### Comparing `heaobject-1.6.1/LICENSE` & `heaobject-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.1/PKG-INFO` & `heaobject-1.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaobject
-Version: 1.6.1
+Version: 1.6.2
 Summary: Data and other classes that are passed into and out of HEA REST APIs.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -33,14 +33,17 @@
 Requires-Dist: mimetype-description~=0.1.0
 
 # HEA Object Library
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
 
+## Version 1.6.2
+* Fixed heaobject.account.AWSAccount.new_credentials() not setting the credentials' role.
+
 ## Version 1.6.1
 * For heaobject.organization.Organization, managers can now modify the manager and member lists.
 
 ## Version 1.6.0
 * Replaced heaobject.keychain.AWSCredentials role_arn attribute with a role attribute on heaobject.keychain.Credentials objects.
 * Added group_ids attribute to heaobject.person.Person.
 * New attributes in heaobject.account.Account: file_system_type, file_system_name.
```

### Comparing `heaobject-1.6.1/README.md` & `heaobject-1.6.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # HEA Object Library
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
 
+## Version 1.6.2
+* Fixed heaobject.account.AWSAccount.new_credentials() not setting the credentials' role.
+
 ## Version 1.6.1
 * For heaobject.organization.Organization, managers can now modify the manager and member lists.
 
 ## Version 1.6.0
 * Replaced heaobject.keychain.AWSCredentials role_arn attribute with a role attribute on heaobject.keychain.Credentials objects.
 * Added group_ids attribute to heaobject.person.Person.
 * New attributes in heaobject.account.Account: file_system_type, file_system_name.
```

### Comparing `heaobject-1.6.1/setup.py` & `heaobject-1.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(name='heaobject',
-                 version='1.6.1',
+                 version='1.6.2',
                  description='Data and other classes that are passed into and out of HEA REST APIs.',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  url='https://risr.hci.utah.edu',
                  author='Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT',
                  author_email='Andrew.Post@hci.utah.edu',
                  python_requires='>=3.10',
```

### Comparing `heaobject-1.6.1/src/heaobject/__init__.py` & `heaobject-1.6.2/src/heaobject/__init__.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.1/src/heaobject/account.py` & `heaobject-1.6.2/src/heaobject/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,16 +175,16 @@
             if role is not None and user.group_ids.count(group.id) > 0:
                 return role
         return None
 
     def new_credentials(self, person: Person, groups: Sequence[Group] | None = None) -> AWSCredentials:
         credentials = AWSCredentials()
         if groups is not None:
-            credentials.role_arn = self.get_role_to_assume(person, groups)
-        if credentials.role_arn is None:
+            credentials.role = self.get_role_to_assume(person, groups)
+        if credentials.role is None:
             raise ValueError('AWS Credentials must have a non-None role attribute')
         credentials.name = f'{person.id}_{self.type}_{self.id}'
         credentials.display_name = f'{self.display_name} - {person.display_name}'
         return credentials
 
 
 class AccountView(AbstractDesktopObject, View):
```

### Comparing `heaobject-1.6.1/src/heaobject/activity.py` & `heaobject-1.6.2/src/heaobject/activity.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.1/src/heaobject/aws.py` & `heaobject-1.6.2/src/heaobject/aws.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.1/src/heaobject/awss3key.py` & `heaobject-1.6.2/src/heaobject/awss3key.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.1/src/heaobject/bucket.py` & `heaobject-1.6.2/src/heaobject/bucket.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.1/src/heaobject/data.py` & `heaobject-1.6.2/src/heaobject/data.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.1/src/heaobject/dataadapter.py` & `heaobject-1.6.2/src/heaobject/dataadapter.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.1/src/heaobject/datamodel.py` & `heaobject-1.6.2/src/heaobject/datamodel.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.1/src/heaobject/folder.py` & `heaobject-1.6.2/src/heaobject/folder.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.1/src/heaobject/keychain.py` & `heaobject-1.6.2/src/heaobject/keychain.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.1/src/heaobject/mimetype.py` & `heaobject-1.6.2/src/heaobject/mimetype.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.1/src/heaobject/organization.py` & `heaobject-1.6.2/src/heaobject/organization.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.1/src/heaobject/person.py` & `heaobject-1.6.2/src/heaobject/person.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.1/src/heaobject/project.py` & `heaobject-1.6.2/src/heaobject/project.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.1/src/heaobject/registry.py` & `heaobject-1.6.2/src/heaobject/registry.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.1/src/heaobject/root.py` & `heaobject-1.6.2/src/heaobject/root.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.1/src/heaobject/settings.py` & `heaobject-1.6.2/src/heaobject/settings.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.1/src/heaobject/source2target.py` & `heaobject-1.6.2/src/heaobject/source2target.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.1/src/heaobject/storage.py` & `heaobject-1.6.2/src/heaobject/storage.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.1/src/heaobject/trash.py` & `heaobject-1.6.2/src/heaobject/trash.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.1/src/heaobject/user.py` & `heaobject-1.6.2/src/heaobject/user.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.1/src/heaobject/volume.py` & `heaobject-1.6.2/src/heaobject/volume.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.1/src/heaobject.egg-info/PKG-INFO` & `heaobject-1.6.2/src/heaobject.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaobject
-Version: 1.6.1
+Version: 1.6.2
 Summary: Data and other classes that are passed into and out of HEA REST APIs.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -33,14 +33,17 @@
 Requires-Dist: mimetype-description~=0.1.0
 
 # HEA Object Library
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
 
+## Version 1.6.2
+* Fixed heaobject.account.AWSAccount.new_credentials() not setting the credentials' role.
+
 ## Version 1.6.1
 * For heaobject.organization.Organization, managers can now modify the manager and member lists.
 
 ## Version 1.6.0
 * Replaced heaobject.keychain.AWSCredentials role_arn attribute with a role attribute on heaobject.keychain.Credentials objects.
 * Added group_ids attribute to heaobject.person.Person.
 * New attributes in heaobject.account.Account: file_system_type, file_system_name.
```

### Comparing `heaobject-1.6.1/src/heaobject.egg-info/SOURCES.txt` & `heaobject-1.6.2/src/heaobject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

