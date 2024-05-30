# Comparing `tmp/heaserver_organizations-1.4.5.tar.gz` & `tmp/heaserver_organizations-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver_organizations-1.4.5.tar", last modified: Thu May 30 22:33:28 2024, max compression
+gzip compressed data, was "heaserver_organizations-1.4.6.tar", last modified: Thu May 30 23:40:59 2024, max compression
```

## Comparing `heaserver_organizations-1.4.5.tar` & `heaserver_organizations-1.4.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 22:33:28.132829 heaserver_organizations-1.4.5/
--rw-rw-rw-   0        0        0      261 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.5/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.5/.gitignore
--rw-rw-rw-   0        0        0     1663 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.5/Dockerfile
--rw-rw-rw-   0        0        0    11625 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.5/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.5/MANIFEST.in
--rw-rw-rw-   0        0        0     6138 2024-05-30 22:33:28.131830 heaserver_organizations-1.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     4715 2024-05-30 22:31:03.000000 heaserver_organizations-1.4.5/README.md
--rw-rw-rw-   0        0        0     1749 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.5/RELEASING.md
--rw-rw-rw-   0        0        0      594 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.5/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-05-30 22:33:27.941459 heaserver_organizations-1.4.5/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-05-30 22:33:27.941459 heaserver_organizations-1.4.5/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-30 22:33:28.051718 heaserver_organizations-1.4.5/integrationtests/heaserver/organizationintegrationtest/
--rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.5/integrationtests/heaserver/organizationintegrationtest/__init__.py
--rw-rw-rw-   0        0        0    10980 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.5/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py
--rw-rw-rw-   0        0        0      835 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.5/integrationtests/heaserver/organizationintegrationtest/test_all.py
--rw-rw-rw-   0        0        0    15050 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.5/integrationtests/heaserver/organizationintegrationtest/testcase.py
--rw-rw-rw-   0        0        0      111 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.5/pytest.ini
--rw-rw-rw-   0        0        0      362 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.5/requirements_dev.txt
--rw-rw-rw-   0        0        0     6574 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.5/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-05-30 22:33:28.132829 heaserver_organizations-1.4.5/setup.cfg
--rw-rw-rw-   0        0        0     1931 2024-05-30 22:32:53.000000 heaserver_organizations-1.4.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-30 22:33:27.943456 heaserver_organizations-1.4.5/src/
-drwxrwxrwx   0        0        0        0 2024-05-30 22:33:27.942456 heaserver_organizations-1.4.5/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-30 22:33:28.057719 heaserver_organizations-1.4.5/src/heaserver/organization/
--rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.5/src/heaserver/organization/__init__.py
--rw-rw-rw-   0        0        0    53476 2024-05-30 22:28:05.000000 heaserver_organizations-1.4.5/src/heaserver/organization/service.py
-drwxrwxrwx   0        0        0        0 2024-05-30 22:33:28.067748 heaserver_organizations-1.4.5/src/heaserver/organization/wstl/
--rw-rw-rw-   0        0        0    26704 2024-05-30 21:38:57.000000 heaserver_organizations-1.4.5/src/heaserver/organization/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-05-30 22:33:28.129829 heaserver_organizations-1.4.5/src/heaserver_organizations.egg-info/
--rw-rw-rw-   0        0        0     6138 2024-05-30 22:33:27.000000 heaserver_organizations-1.4.5/src/heaserver_organizations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      997 2024-05-30 22:33:27.000000 heaserver_organizations-1.4.5/src/heaserver_organizations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 22:33:27.000000 heaserver_organizations-1.4.5/src/heaserver_organizations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-05-30 22:33:27.000000 heaserver_organizations-1.4.5/src/heaserver_organizations.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2024-05-30 22:33:27.000000 heaserver_organizations-1.4.5/src/heaserver_organizations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-30 22:33:27.000000 heaserver_organizations-1.4.5/src/heaserver_organizations.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-30 22:33:27.944456 heaserver_organizations-1.4.5/tests/
-drwxrwxrwx   0        0        0        0 2024-05-30 22:33:27.945457 heaserver_organizations-1.4.5/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-30 22:33:28.127676 heaserver_organizations-1.4.5/tests/heaserver/organizationtest/
--rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.5/tests/heaserver/organizationtest/__init__.py
--rw-rw-rw-   0        0        0     2214 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.5/tests/heaserver/organizationtest/test_all.py
--rw-rw-rw-   0        0        0     7050 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.5/tests/heaserver/organizationtest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-05-30 23:40:59.245848 heaserver_organizations-1.4.6/
+-rw-rw-rw-   0        0        0      261 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.6/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.6/.gitignore
+-rw-rw-rw-   0        0        0     1663 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.6/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.6/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     6262 2024-05-30 23:40:59.244844 heaserver_organizations-1.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4839 2024-05-30 23:19:30.000000 heaserver_organizations-1.4.6/README.md
+-rw-rw-rw-   0        0        0     1749 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.6/RELEASING.md
+-rw-rw-rw-   0        0        0      594 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.6/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-05-30 23:40:59.057575 heaserver_organizations-1.4.6/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-05-30 23:40:59.057575 heaserver_organizations-1.4.6/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-30 23:40:59.167844 heaserver_organizations-1.4.6/integrationtests/heaserver/organizationintegrationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.6/integrationtests/heaserver/organizationintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0    10980 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.6/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py
+-rw-rw-rw-   0        0        0      835 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.6/integrationtests/heaserver/organizationintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0    15050 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.6/integrationtests/heaserver/organizationintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.6/pytest.ini
+-rw-rw-rw-   0        0        0      362 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.6/requirements_dev.txt
+-rw-rw-rw-   0        0        0     6574 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.6/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-05-30 23:40:59.245848 heaserver_organizations-1.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     1931 2024-05-30 23:40:11.000000 heaserver_organizations-1.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 23:40:59.060605 heaserver_organizations-1.4.6/src/
+drwxrwxrwx   0        0        0        0 2024-05-30 23:40:59.059604 heaserver_organizations-1.4.6/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-30 23:40:59.170844 heaserver_organizations-1.4.6/src/heaserver/organization/
+-rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.6/src/heaserver/organization/__init__.py
+-rw-rw-rw-   0        0        0    53476 2024-05-30 23:11:08.000000 heaserver_organizations-1.4.6/src/heaserver/organization/service.py
+drwxrwxrwx   0        0        0        0 2024-05-30 23:40:59.181843 heaserver_organizations-1.4.6/src/heaserver/organization/wstl/
+-rw-rw-rw-   0        0        0    26704 2024-05-30 21:38:57.000000 heaserver_organizations-1.4.6/src/heaserver/organization/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-05-30 23:40:59.243858 heaserver_organizations-1.4.6/src/heaserver_organizations.egg-info/
+-rw-rw-rw-   0        0        0     6262 2024-05-30 23:40:59.000000 heaserver_organizations-1.4.6/src/heaserver_organizations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      997 2024-05-30 23:40:59.000000 heaserver_organizations-1.4.6/src/heaserver_organizations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 23:40:59.000000 heaserver_organizations-1.4.6/src/heaserver_organizations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-30 23:40:59.000000 heaserver_organizations-1.4.6/src/heaserver_organizations.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2024-05-30 23:40:59.000000 heaserver_organizations-1.4.6/src/heaserver_organizations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-30 23:40:59.000000 heaserver_organizations-1.4.6/src/heaserver_organizations.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 23:40:59.061573 heaserver_organizations-1.4.6/tests/
+drwxrwxrwx   0        0        0        0 2024-05-30 23:40:59.061573 heaserver_organizations-1.4.6/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-30 23:40:59.241846 heaserver_organizations-1.4.6/tests/heaserver/organizationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.6/tests/heaserver/organizationtest/__init__.py
+-rw-rw-rw-   0        0        0     2214 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.6/tests/heaserver/organizationtest/test_all.py
+-rw-rw-rw-   0        0        0     7050 2024-05-21 23:53:34.000000 heaserver_organizations-1.4.6/tests/heaserver/organizationtest/testcase.py
```

### Comparing `heaserver_organizations-1.4.5/Dockerfile` & `heaserver_organizations-1.4.6/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.5/LICENSE` & `heaserver_organizations-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.5/PKG-INFO` & `heaserver_organizations-1.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-organizations
-Version: 1.4.5
+Version: 1.4.6
 Summary: a service for managing organization information for research laboratories and other research groups
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-organizations,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -22,22 +22,25 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: heaserver~=1.6.0
-Requires-Dist: heaobject~=1.6.1
+Requires-Dist: heaobject~=1.6.2
 
 # HEA Server Organization
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Organization is a service for managing organization information for research laboratories and other research groups.
 
+## Version 1.4.6
+* Fixed issue creating new credentials objects without a role when a user is added to an organization.
+
 ## Version 1.4.5
 * Fixed crash when reusing an existing volume and credentials when a user's organization membership has changed.
 
 ## Version 1.4.4
 * Return 400 status code when the user lacks permission to update permissions for an organization (those errors were ignored previously).
 * Corrected permissions checking for organization managers and members.
```

### Comparing `heaserver_organizations-1.4.5/README.md` & `heaserver_organizations-1.4.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # HEA Server Organization
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Organization is a service for managing organization information for research laboratories and other research groups.
 
+## Version 1.4.6
+* Fixed issue creating new credentials objects without a role when a user is added to an organization.
+
 ## Version 1.4.5
 * Fixed crash when reusing an existing volume and credentials when a user's organization membership has changed.
 
 ## Version 1.4.4
 * Return 400 status code when the user lacks permission to update permissions for an organization (those errors were ignored previously).
 * Corrected permissions checking for organization managers and members.
```

### Comparing `heaserver_organizations-1.4.5/RELEASING.md` & `heaserver_organizations-1.4.6/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.5/docker-entrypoint.sh` & `heaserver_organizations-1.4.6/docker-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.5/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py` & `heaserver_organizations-1.4.6/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.5/integrationtests/heaserver/organizationintegrationtest/test_all.py` & `heaserver_organizations-1.4.6/integrationtests/heaserver/organizationintegrationtest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.5/integrationtests/heaserver/organizationintegrationtest/testcase.py` & `heaserver_organizations-1.4.6/integrationtests/heaserver/organizationintegrationtest/testcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.5/run-swaggerui.py` & `heaserver_organizations-1.4.6/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.5/setup.py` & `heaserver_organizations-1.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-organizations',
-    version='1.4.5',
+    version='1.4.6',
     description="a service for managing organization information for research laboratories and other research groups",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.organization'],
     package_data={'heaserver.organization': ['wstl/*.json']},
-    install_requires=['heaserver~=1.6.0', 'heaobject~=1.6.1'],
+    install_requires=['heaserver~=1.6.0', 'heaobject~=1.6.2'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
         'Environment :: Web Environment',
```

### Comparing `heaserver_organizations-1.4.5/src/heaserver/organization/service.py` & `heaserver_organizations-1.4.6/src/heaserver/organization/service.py`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.5/src/heaserver/organization/wstl/all.json` & `heaserver_organizations-1.4.6/src/heaserver/organization/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.5/src/heaserver_organizations.egg-info/PKG-INFO` & `heaserver_organizations-1.4.6/src/heaserver_organizations.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-organizations
-Version: 1.4.5
+Version: 1.4.6
 Summary: a service for managing organization information for research laboratories and other research groups
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-organizations,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -22,22 +22,25 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: heaserver~=1.6.0
-Requires-Dist: heaobject~=1.6.1
+Requires-Dist: heaobject~=1.6.2
 
 # HEA Server Organization
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Organization is a service for managing organization information for research laboratories and other research groups.
 
+## Version 1.4.6
+* Fixed issue creating new credentials objects without a role when a user is added to an organization.
+
 ## Version 1.4.5
 * Fixed crash when reusing an existing volume and credentials when a user's organization membership has changed.
 
 ## Version 1.4.4
 * Return 400 status code when the user lacks permission to update permissions for an organization (those errors were ignored previously).
 * Corrected permissions checking for organization managers and members.
```

### Comparing `heaserver_organizations-1.4.5/src/heaserver_organizations.egg-info/SOURCES.txt` & `heaserver_organizations-1.4.6/src/heaserver_organizations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.5/tests/heaserver/organizationtest/test_all.py` & `heaserver_organizations-1.4.6/tests/heaserver/organizationtest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.4.5/tests/heaserver/organizationtest/testcase.py` & `heaserver_organizations-1.4.6/tests/heaserver/organizationtest/testcase.py`

 * *Files identical despite different names*

