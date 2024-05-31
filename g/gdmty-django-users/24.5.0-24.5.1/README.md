# Comparing `tmp/gdmty_django_users-24.5.0.tar.gz` & `tmp/gdmty_django_users-24.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdmty_django_users-24.5.0.tar", last modified: Fri May 10 04:33:08 2024, max compression
+gzip compressed data, was "gdmty_django_users-24.5.1.tar", last modified: Fri May 31 20:10:44 2024, max compression
```

## Comparing `gdmty_django_users-24.5.0.tar` & `gdmty_django_users-24.5.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 04:33:08.703131 gdmty_django_users-24.5.0/
--rw-rw-rw-   0        0        0    35182 2024-03-15 01:06:22.000000 gdmty_django_users-24.5.0/LICENSE
--rw-rw-rw-   0        0        0       51 2024-03-15 01:06:22.000000 gdmty_django_users-24.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0    43714 2024-05-10 04:33:08.703131 gdmty_django_users-24.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     2113 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.0/README.md
--rw-rw-rw-   0        0        0     1527 2024-05-10 04:32:53.000000 gdmty_django_users-24.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-10 04:33:08.703131 gdmty_django_users-24.5.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-10 04:33:08.671486 gdmty_django_users-24.5.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-10 04:33:08.692624 gdmty_django_users-24.5.0/src/gdmty_django_users/
--rw-rw-rw-   0        0        0     1367 2024-05-10 04:32:53.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/__init__.py
--rw-rw-rw-   0        0        0     2477 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/admin.py
--rw-rw-rw-   0        0        0     1048 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/apps.py
--rw-rw-rw-   0        0        0     1437 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/decorators.py
--rw-rw-rw-   0        0        0     2332 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/managers.py
-drwxrwxrwx   0        0        0        0 2024-05-10 04:33:08.703131 gdmty_django_users-24.5.0/src/gdmty_django_users/migrations/
--rw-rw-rw-   0        0        0     3284 2024-05-10 04:28:25.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1333 2024-05-10 04:29:08.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/migrations/0002_alter_user_groups_alter_user_user_permissions_and_more.py
--rw-rw-rw-   0        0        0        0 2024-03-15 01:06:22.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/migrations/__init__.py
--rw-rw-rw-   0        0        0     3204 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/models.py
--rw-rw-rw-   0        0        0     1819 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/permissions.py
--rw-rw-rw-   0        0        0     1763 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/serializers.py
--rw-rw-rw-   0        0        0     1065 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/settings.py
--rw-rw-rw-   0        0        0      910 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/tests.py
--rw-rw-rw-   0        0        0     1756 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/urls.py
--rw-rw-rw-   0        0        0     4811 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/viewsets.py
--rw-rw-rw-   0        0        0     1471 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.0/src/gdmty_django_users/wagtail_forms.py
-drwxrwxrwx   0        0        0        0 2024-05-10 04:33:08.703131 gdmty_django_users-24.5.0/src/gdmty_django_users.egg-info/
--rw-rw-rw-   0        0        0    43714 2024-05-10 04:33:08.000000 gdmty_django_users-24.5.0/src/gdmty_django_users.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      918 2024-05-10 04:33:08.000000 gdmty_django_users-24.5.0/src/gdmty_django_users.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 04:33:08.000000 gdmty_django_users-24.5.0/src/gdmty_django_users.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2024-05-10 04:33:08.000000 gdmty_django_users-24.5.0/src/gdmty_django_users.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-10 04:33:08.000000 gdmty_django_users-24.5.0/src/gdmty_django_users.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 20:10:44.447505 gdmty_django_users-24.5.1/
+-rw-rw-rw-   0        0        0    35182 2024-03-15 01:06:22.000000 gdmty_django_users-24.5.1/LICENSE
+-rw-rw-rw-   0        0        0       51 2024-03-15 01:06:22.000000 gdmty_django_users-24.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    43714 2024-05-31 20:10:44.447505 gdmty_django_users-24.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2113 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.1/README.md
+-rw-rw-rw-   0        0        0     1527 2024-05-31 20:10:28.000000 gdmty_django_users-24.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-31 20:10:44.447505 gdmty_django_users-24.5.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-31 20:10:44.416241 gdmty_django_users-24.5.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-31 20:10:44.431943 gdmty_django_users-24.5.1/src/gdmty_django_users/
+-rw-rw-rw-   0        0        0     1367 2024-05-31 20:10:28.000000 gdmty_django_users-24.5.1/src/gdmty_django_users/__init__.py
+-rw-rw-rw-   0        0        0     2477 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.1/src/gdmty_django_users/admin.py
+-rw-rw-rw-   0        0        0     1048 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.1/src/gdmty_django_users/apps.py
+-rw-rw-rw-   0        0        0     1437 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.1/src/gdmty_django_users/decorators.py
+-rw-rw-rw-   0        0        0     2332 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.1/src/gdmty_django_users/managers.py
+drwxrwxrwx   0        0        0        0 2024-05-31 20:10:44.447505 gdmty_django_users-24.5.1/src/gdmty_django_users/migrations/
+-rw-rw-rw-   0        0        0     3284 2024-05-10 04:28:25.000000 gdmty_django_users-24.5.1/src/gdmty_django_users/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     1333 2024-05-10 04:29:08.000000 gdmty_django_users-24.5.1/src/gdmty_django_users/migrations/0002_alter_user_groups_alter_user_user_permissions_and_more.py
+-rw-rw-rw-   0        0        0        0 2024-03-15 01:06:22.000000 gdmty_django_users-24.5.1/src/gdmty_django_users/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3190 2024-05-31 20:07:38.000000 gdmty_django_users-24.5.1/src/gdmty_django_users/models.py
+-rw-rw-rw-   0        0        0     1819 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.1/src/gdmty_django_users/permissions.py
+-rw-rw-rw-   0        0        0     1763 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.1/src/gdmty_django_users/serializers.py
+-rw-rw-rw-   0        0        0     1065 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.1/src/gdmty_django_users/settings.py
+-rw-rw-rw-   0        0        0      910 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.1/src/gdmty_django_users/tests.py
+-rw-rw-rw-   0        0        0     1756 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.1/src/gdmty_django_users/urls.py
+-rw-rw-rw-   0        0        0     4811 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.1/src/gdmty_django_users/viewsets.py
+-rw-rw-rw-   0        0        0     1471 2024-05-10 04:32:02.000000 gdmty_django_users-24.5.1/src/gdmty_django_users/wagtail_forms.py
+drwxrwxrwx   0        0        0        0 2024-05-31 20:10:44.447505 gdmty_django_users-24.5.1/src/gdmty_django_users.egg-info/
+-rw-rw-rw-   0        0        0    43714 2024-05-31 20:10:44.000000 gdmty_django_users-24.5.1/src/gdmty_django_users.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2024-05-31 20:10:44.000000 gdmty_django_users-24.5.1/src/gdmty_django_users.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 20:10:44.000000 gdmty_django_users-24.5.1/src/gdmty_django_users.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2024-05-31 20:10:44.000000 gdmty_django_users-24.5.1/src/gdmty_django_users.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-31 20:10:44.000000 gdmty_django_users-24.5.1/src/gdmty_django_users.egg-info/top_level.txt
```

### Comparing `gdmty_django_users-24.5.0/LICENSE` & `gdmty_django_users-24.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.0/PKG-INFO` & `gdmty_django_users-24.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdmty-django-users
-Version: 24.5.0
+Version: 24.5.1
 Summary: Extension of Django's AbstractBaseUser for user management, using email as user.
 Author-email: Gobierno de Monterrey <cesar.benjamin@monterrey.gob.mx>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `gdmty_django_users-24.5.0/README.md` & `gdmty_django_users-24.5.1/README.md`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.0/pyproject.toml` & `gdmty_django_users-24.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gdmty-django-users"
-version = "24.5.0"
+version = "24.5.1"
 description = "Extension of Django's AbstractBaseUser for user management, using email as user."
 readme = "README.md"
 authors = [{ name="Gobierno de Monterrey", email="cesar.benjamin@monterrey.gob.mx" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
     "Programming Language :: Python",
@@ -31,15 +31,15 @@
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 "Homepage" = "https://github.com/gobiernodigitalmonterrey/gdmty-django-users"
 "Bug Tracker" = "https://github.com/gobiernodigitalmonterrey/gdmty-django-users/issues"
 
 [tool.bumpver]
-current_version = "24.5.0"
+current_version = "24.5.1"
 version_pattern = "MAJOR.MINOR.PATCH[-PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = true
```

### Comparing `gdmty_django_users-24.5.0/src/gdmty_django_users/__init__.py` & `gdmty_django_users-24.5.1/src/gdmty_django_users/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Package: gdmty_django_users
 PyPi: https://pypi.org/project/gdmty-django-users/
 License: GNU Affero General Public License v3 or later (AGPLv3+)
 
 """
 
 __title__ = "gdmty_django_users"
-__version__ = "24.5.0"
+__version__ = "24.5.1"
 __description__ = "Django module for Users models and permission adding reCAPTCHA token verification."
 __url__ = "https://github.com/SIGAMty/gdmty-django-recaptcha-enterprise"
 __author__ = "César Benjamín"
 __author_email__ = "mathereall@gmail.com"
 __license__ = "GNU Affero General Public License v3 or later (AGPLv3+)"
 __keywords__ = ["django", "users"]
 VERSION = __version__
```

### Comparing `gdmty_django_users-24.5.0/src/gdmty_django_users/admin.py` & `gdmty_django_users-24.5.1/src/gdmty_django_users/admin.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.0/src/gdmty_django_users/apps.py` & `gdmty_django_users-24.5.1/src/gdmty_django_users/apps.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.0/src/gdmty_django_users/decorators.py` & `gdmty_django_users-24.5.1/src/gdmty_django_users/decorators.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.0/src/gdmty_django_users/managers.py` & `gdmty_django_users-24.5.1/src/gdmty_django_users/managers.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.0/src/gdmty_django_users/migrations/0001_initial.py` & `gdmty_django_users-24.5.1/src/gdmty_django_users/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.0/src/gdmty_django_users/migrations/0002_alter_user_groups_alter_user_user_permissions_and_more.py` & `gdmty_django_users-24.5.1/src/gdmty_django_users/migrations/0002_alter_user_groups_alter_user_user_permissions_and_more.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.0/src/gdmty_django_users/models.py` & `gdmty_django_users-24.5.1/src/gdmty_django_users/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,22 +47,22 @@
 
     objects = CustomUserManager()
 
     groups = models.ManyToManyField(
         OriginalGroup,
         verbose_name=_('groups'),
         blank=True,
-        related_name='custom_user_set',  # TODO: Add a related_name here
+        related_name='user_set',  # TODO: Add a related_name here
         related_query_name='user',
     )
     user_permissions = models.ManyToManyField(
         Permission,
         verbose_name=_('user permissions'),
         blank=True,
-        related_name='custom_user_set',  # TODO: Add a related_name here
+        related_name='user_set',  # TODO: Add a related_name here
         related_query_name='user',
     )
 
     @property
     def id(self):
         return self.pk
```

### Comparing `gdmty_django_users-24.5.0/src/gdmty_django_users/permissions.py` & `gdmty_django_users-24.5.1/src/gdmty_django_users/permissions.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.0/src/gdmty_django_users/serializers.py` & `gdmty_django_users-24.5.1/src/gdmty_django_users/serializers.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.0/src/gdmty_django_users/settings.py` & `gdmty_django_users-24.5.1/src/gdmty_django_users/settings.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.0/src/gdmty_django_users/tests.py` & `gdmty_django_users-24.5.1/src/gdmty_django_users/tests.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.0/src/gdmty_django_users/urls.py` & `gdmty_django_users-24.5.1/src/gdmty_django_users/urls.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.0/src/gdmty_django_users/viewsets.py` & `gdmty_django_users-24.5.1/src/gdmty_django_users/viewsets.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.0/src/gdmty_django_users/wagtail_forms.py` & `gdmty_django_users-24.5.1/src/gdmty_django_users/wagtail_forms.py`

 * *Files identical despite different names*

### Comparing `gdmty_django_users-24.5.0/src/gdmty_django_users.egg-info/PKG-INFO` & `gdmty_django_users-24.5.1/src/gdmty_django_users.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdmty-django-users
-Version: 24.5.0
+Version: 24.5.1
 Summary: Extension of Django's AbstractBaseUser for user management, using email as user.
 Author-email: Gobierno de Monterrey <cesar.benjamin@monterrey.gob.mx>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `gdmty_django_users-24.5.0/src/gdmty_django_users.egg-info/SOURCES.txt` & `gdmty_django_users-24.5.1/src/gdmty_django_users.egg-info/SOURCES.txt`

 * *Files identical despite different names*

