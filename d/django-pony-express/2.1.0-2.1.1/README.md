# Comparing `tmp/django_pony_express-2.1.0.tar.gz` & `tmp/django_pony_express-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pony_express-2.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_pony_express-2.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_pony_express-2.1.0.tar` & `django_pony_express-2.1.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     2602 2023-12-04 15:24:45.657869 django_pony_express-2.1.0/.ambient-package-update/metadata.py
--rw-r--r--   0        0        0      320 2024-04-11 14:12:18.255023 django_pony_express-2.1.0/.coveragerc
--rw-r--r--   0        0        0      288 2024-04-11 14:12:18.256031 django_pony_express-2.1.0/.editorconfig
--rw-r--r--   0        0        0     2213 2024-04-11 14:16:18.950523 django_pony_express-2.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3137 2023-12-04 15:24:45.661871 django_pony_express-2.1.0/.gitignore
--rw-r--r--   0        0        0      668 2024-04-11 14:16:18.950523 django_pony_express-2.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      773 2024-04-11 14:12:18.259031 django_pony_express-2.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0     1901 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/CHANGES.md
--rw-r--r--   0        0        0    71412 2024-04-11 14:12:18.291569 django_pony_express-2.1.0/LICENSE.md
--rw-r--r--   0        0        0      138 2024-04-11 14:12:18.260033 django_pony_express-2.1.0/MANIFEST.in
--rw-r--r--   0        0        0     6287 2024-04-11 14:12:18.272133 django_pony_express-2.1.0/README.md
--rw-r--r--   0        0        0       85 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/django_pony_express/__init__.py
--rw-r--r--   0        0        0      114 2023-12-04 15:24:45.663888 django_pony_express-2.1.0/django_pony_express/errors.py
--rw-r--r--   0        0        0     2327 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/django_pony_express/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-12-04 15:24:45.663888 django_pony_express-2.1.0/django_pony_express/services/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/django_pony_express/services/asynchronous/__init__.py
--rw-r--r--   0        0        0      724 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/django_pony_express/services/asynchronous/thread.py
--rw-r--r--   0        0        0    12801 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/django_pony_express/services/base.py
--rw-r--r--   0        0        0    10179 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/django_pony_express/services/tests.py
--rw-r--r--   0        0        0      229 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/django_pony_express/settings.py
--rw-r--r--   0        0        0      654 2024-04-11 14:12:18.279570 django_pony_express-2.1.0/docs/Makefile
--rw-r--r--   0        0        0     2825 2024-04-11 14:16:18.951515 django_pony_express-2.1.0/docs/conf.py
--rw-r--r--   0        0        0       32 2023-12-04 15:24:45.665922 django_pony_express-2.1.0/docs/features/changelog.rst
--rw-r--r--   0        0        0     1480 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/docs/features/configuration.md
--rw-r--r--   0        0        0     2789 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/docs/features/factories.md
--rw-r--r--   0        0        0     2750 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/docs/features/internal_api.md
--rw-r--r--   0        0        0     4588 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/docs/features/introduction.md
--rw-r--r--   0        0        0     4912 2023-12-04 15:24:45.665922 django_pony_express-2.1.0/docs/features/tests.md
--rw-r--r--   0        0        0      375 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/docs/index.rst
--rwxr-xr-x   0        0        0      795 2024-04-11 14:12:18.278560 django_pony_express-2.1.0/docs/make.bat
--rw-r--r--   0        0        0      679 2024-04-11 14:16:18.952522 django_pony_express-2.1.0/manage.py
--rw-r--r--   0        0        0     5402 2024-04-11 14:16:18.952522 django_pony_express-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      121 2024-04-11 14:12:18.281561 django_pony_express-2.1.0/scripts/unix/install_requirements.sh
--rw-r--r--   0        0        0       50 2024-04-11 14:12:18.282568 django_pony_express-2.1.0/scripts/unix/publish_to_pypi.sh
--rw-r--r--   0        0        0      121 2024-04-11 14:12:18.284573 django_pony_express-2.1.0/scripts/windows/install_requirements.ps1
--rw-r--r--   0        0        0       50 2024-04-11 14:12:18.285570 django_pony_express-2.1.0/scripts/windows/publish_to_pypi.ps1
--rw-r--r--   0        0        0     1761 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/settings.py
--rw-r--r--   0        0        0      289 2024-04-11 14:12:18.273137 django_pony_express-2.1.0/setup.cfg
--rw-r--r--   0        0        0        0 2023-12-04 15:24:45.665922 django_pony_express-2.1.0/testapp/__init__.py
--rw-r--r--   0        0        0      134 2023-12-04 15:24:45.665922 django_pony_express-2.1.0/testapp/templates/testapp/test_email.html
--rw-r--r--   0        0        0      145 2023-12-04 15:24:45.670166 django_pony_express-2.1.0/testapp/templates/testapp/test_email.txt
--rw-r--r--   0        0        0      137 2023-12-04 15:24:45.670166 django_pony_express-2.1.0/testapp/urls.py
--rw-r--r--   0        0        0        0 2023-12-04 15:24:45.670166 django_pony_express-2.1.0/tests/__init__.py
--rw-r--r--   0        0        0       27 2023-12-04 15:24:45.670166 django_pony_express-2.1.0/tests/files/testfile.txt
--rw-r--r--   0        0        0        0 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/tests/services/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/tests/services/asynchronous/__init__.py
--rw-r--r--   0        0        0      645 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/tests/services/asynchronous/test_thread_email.py
--rw-r--r--   0        0        0        0 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/tests/services/base/__init__.py
--rw-r--r--   0        0        0     3425 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/tests/services/base/test_base_mail_factory.py
--rw-r--r--   0        0        0    15473 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/tests/services/base/test_base_mail_service.py
--rw-r--r--   0        0        0        0 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/tests/services/tests/__init__.py
--rw-r--r--   0        0        0     9609 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/tests/services/tests/test_email_test_service.py
--rw-r--r--   0        0        0     8248 1970-01-01 00:00:00.000000 django_pony_express-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2602 2023-12-04 15:24:45.657869 django_pony_express-2.1.1/.ambient-package-update/metadata.py
+-rw-r--r--   0        0        0      320 2024-04-11 14:12:18.255023 django_pony_express-2.1.1/.coveragerc
+-rw-r--r--   0        0        0      288 2024-04-11 14:12:18.256031 django_pony_express-2.1.1/.editorconfig
+-rw-r--r--   0        0        0     2213 2024-04-11 14:16:18.950523 django_pony_express-2.1.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3137 2023-12-04 15:24:45.661871 django_pony_express-2.1.1/.gitignore
+-rw-r--r--   0        0        0      668 2024-04-11 14:16:18.950523 django_pony_express-2.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      773 2024-04-11 14:12:18.259031 django_pony_express-2.1.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     2020 2024-05-31 15:18:08.467118 django_pony_express-2.1.1/CHANGES.md
+-rw-r--r--   0        0        0    71412 2024-04-11 14:12:18.291569 django_pony_express-2.1.1/LICENSE.md
+-rw-r--r--   0        0        0      138 2024-04-11 14:12:18.260033 django_pony_express-2.1.1/MANIFEST.in
+-rw-r--r--   0        0        0     6287 2024-04-11 14:12:18.272133 django_pony_express-2.1.1/README.md
+-rw-r--r--   0        0        0       85 2024-05-31 15:18:08.362121 django_pony_express-2.1.1/django_pony_express/__init__.py
+-rw-r--r--   0        0        0      114 2023-12-04 15:24:45.663888 django_pony_express-2.1.1/django_pony_express/errors.py
+-rw-r--r--   0        0        0     2327 2024-05-27 15:19:31.530860 django_pony_express-2.1.1/django_pony_express/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-12-04 15:24:45.663888 django_pony_express-2.1.1/django_pony_express/services/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 15:19:31.530860 django_pony_express-2.1.1/django_pony_express/services/asynchronous/__init__.py
+-rw-r--r--   0        0        0      724 2024-05-27 15:19:31.530860 django_pony_express-2.1.1/django_pony_express/services/asynchronous/thread.py
+-rw-r--r--   0        0        0    12799 2024-05-31 15:16:47.267572 django_pony_express-2.1.1/django_pony_express/services/base.py
+-rw-r--r--   0        0        0    10179 2024-05-27 15:19:31.530860 django_pony_express-2.1.1/django_pony_express/services/tests.py
+-rw-r--r--   0        0        0      229 2024-05-27 15:19:31.530860 django_pony_express-2.1.1/django_pony_express/settings.py
+-rw-r--r--   0        0        0      654 2024-04-11 14:12:18.279570 django_pony_express-2.1.1/docs/Makefile
+-rw-r--r--   0        0        0     2825 2024-04-11 14:16:18.951515 django_pony_express-2.1.1/docs/conf.py
+-rw-r--r--   0        0        0       32 2023-12-04 15:24:45.665922 django_pony_express-2.1.1/docs/features/changelog.rst
+-rw-r--r--   0        0        0     1481 2024-05-31 15:16:47.269937 django_pony_express-2.1.1/docs/features/configuration.md
+-rw-r--r--   0        0        0     2789 2024-05-27 15:19:31.530860 django_pony_express-2.1.1/docs/features/factories.md
+-rw-r--r--   0        0        0     2750 2024-05-27 15:19:31.530860 django_pony_express-2.1.1/docs/features/internal_api.md
+-rw-r--r--   0        0        0     4588 2024-05-27 15:19:31.530860 django_pony_express-2.1.1/docs/features/introduction.md
+-rw-r--r--   0        0        0     4912 2023-12-04 15:24:45.665922 django_pony_express-2.1.1/docs/features/tests.md
+-rw-r--r--   0        0        0      375 2024-05-27 15:19:31.530860 django_pony_express-2.1.1/docs/index.rst
+-rwxr-xr-x   0        0        0      795 2024-04-11 14:12:18.278560 django_pony_express-2.1.1/docs/make.bat
+-rw-r--r--   0        0        0      679 2024-04-11 14:16:18.952522 django_pony_express-2.1.1/manage.py
+-rw-r--r--   0        0        0     5402 2024-04-11 14:16:18.952522 django_pony_express-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0      121 2024-04-11 14:12:18.281561 django_pony_express-2.1.1/scripts/unix/install_requirements.sh
+-rw-r--r--   0        0        0       50 2024-04-11 14:12:18.282568 django_pony_express-2.1.1/scripts/unix/publish_to_pypi.sh
+-rw-r--r--   0        0        0      121 2024-04-11 14:12:18.284573 django_pony_express-2.1.1/scripts/windows/install_requirements.ps1
+-rw-r--r--   0        0        0       50 2024-04-11 14:12:18.285570 django_pony_express-2.1.1/scripts/windows/publish_to_pypi.ps1
+-rw-r--r--   0        0        0     1761 2024-05-27 15:19:31.530860 django_pony_express-2.1.1/settings.py
+-rw-r--r--   0        0        0      289 2024-04-11 14:12:18.273137 django_pony_express-2.1.1/setup.cfg
+-rw-r--r--   0        0        0        0 2023-12-04 15:24:45.665922 django_pony_express-2.1.1/testapp/__init__.py
+-rw-r--r--   0        0        0      134 2023-12-04 15:24:45.665922 django_pony_express-2.1.1/testapp/templates/testapp/test_email.html
+-rw-r--r--   0        0        0      145 2023-12-04 15:24:45.670166 django_pony_express-2.1.1/testapp/templates/testapp/test_email.txt
+-rw-r--r--   0        0        0      137 2023-12-04 15:24:45.670166 django_pony_express-2.1.1/testapp/urls.py
+-rw-r--r--   0        0        0        0 2023-12-04 15:24:45.670166 django_pony_express-2.1.1/tests/__init__.py
+-rw-r--r--   0        0        0       27 2023-12-04 15:24:45.670166 django_pony_express-2.1.1/tests/files/testfile.txt
+-rw-r--r--   0        0        0        0 2024-05-27 15:19:31.530860 django_pony_express-2.1.1/tests/services/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 15:19:31.530860 django_pony_express-2.1.1/tests/services/asynchronous/__init__.py
+-rw-r--r--   0        0        0      645 2024-05-27 15:19:31.530860 django_pony_express-2.1.1/tests/services/asynchronous/test_thread_email.py
+-rw-r--r--   0        0        0        0 2024-05-27 15:19:31.530860 django_pony_express-2.1.1/tests/services/base/__init__.py
+-rw-r--r--   0        0        0     3425 2024-05-27 15:19:31.530860 django_pony_express-2.1.1/tests/services/base/test_base_mail_factory.py
+-rw-r--r--   0        0        0    15471 2024-05-31 15:16:47.269937 django_pony_express-2.1.1/tests/services/base/test_base_mail_service.py
+-rw-r--r--   0        0        0        0 2024-05-27 15:19:31.530860 django_pony_express-2.1.1/tests/services/tests/__init__.py
+-rw-r--r--   0        0        0     9609 2024-05-27 15:19:31.530860 django_pony_express-2.1.1/tests/services/tests/test_email_test_service.py
+-rw-r--r--   0        0        0     8248 1970-01-01 00:00:00.000000 django_pony_express-2.1.1/PKG-INFO
```

### Comparing `django_pony_express-2.1.0/.ambient-package-update/metadata.py` & `django_pony_express-2.1.1/.ambient-package-update/metadata.py`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.1.0/.github/workflows/ci.yml` & `django_pony_express-2.1.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.1.0/.gitignore` & `django_pony_express-2.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.1.0/.pre-commit-config.yaml` & `django_pony_express-2.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.1.0/.readthedocs.yaml` & `django_pony_express-2.1.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.1.0/CHANGES.md` & `django_pony_express-2.1.1/CHANGES.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+* *2.1.1* (2024-05-31)
+  * Changed log-level to "info" for successful dispatching
+  * Improved configuration docs
+
 * *2.1.0* (2024-05-27)
   * Added `ThreadEmailService` for simple async sending of emails
   * Added basic logging with privacy configuration to mail class
   * Restructured documentation
   * Restructured unit-tests
   * Minor test improvements
```

### Comparing `django_pony_express-2.1.0/LICENSE.md` & `django_pony_express-2.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.1.0/README.md` & `django_pony_express-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.1.0/django_pony_express/locale/de/LC_MESSAGES/django.po` & `django_pony_express-2.1.1/django_pony_express/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.1.0/django_pony_express/services/asynchronous/thread.py` & `django_pony_express-2.1.1/django_pony_express/services/asynchronous/thread.py`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.1.0/django_pony_express/services/base.py` & `django_pony_express-2.1.1/django_pony_express/services/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,17 +309,17 @@
         Method to be called by the thread. Enables logging since we won't have any sync return values.
         """
         result = False
         recipients_as_string = " ".join(self.recipient_email_list)
         try:
             result = msg.send()
             if PONY_LOG_RECIPIENTS:
-                self._logger.debug(_('Email "%s" successfully sent to %s.') % (msg.subject, recipients_as_string))
+                self._logger.info(_('Email "%s" successfully sent to %s.') % (msg.subject, recipients_as_string))
             else:
-                self._logger.debug(_('Email "%s" successfully sent.') % msg.subject)
+                self._logger.info(_('Email "%s" successfully sent.') % msg.subject)
         except Exception as e:
             if PONY_LOG_RECIPIENTS:
                 self._logger.error(
                     _('An error occurred sending email "%s" to %s: %s') % (msg.subject, recipients_as_string, str(e))
                 )
             else:
                 self._logger.error(_('An error occurred sending email "%s": %s') % (msg.subject, str(e)))
```

### Comparing `django_pony_express-2.1.0/django_pony_express/services/tests.py` & `django_pony_express-2.1.1/django_pony_express/services/tests.py`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.1.0/docs/Makefile` & `django_pony_express-2.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.1.0/docs/conf.py` & `django_pony_express-2.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.1.0/docs/features/configuration.md` & `django_pony_express-2.1.1/docs/features/configuration.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 Note that in this example, we are only logging to the console.
 
 ```python
 LOGGING = {
     "loggers": {
         "django_pony_express": {
             "handlers": ["console"],
-            "level": "INFO",
+            "level": "DEBUG",
             "propagate": True,
         },
         ...
     },
 }
 ```
```

### Comparing `django_pony_express-2.1.0/docs/features/factories.md` & `django_pony_express-2.1.1/docs/features/factories.md`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.1.0/docs/features/internal_api.md` & `django_pony_express-2.1.1/docs/features/internal_api.md`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.1.0/docs/features/introduction.md` & `django_pony_express-2.1.1/docs/features/introduction.md`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.1.0/docs/features/tests.md` & `django_pony_express-2.1.1/docs/features/tests.md`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.1.0/docs/make.bat` & `django_pony_express-2.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.1.0/manage.py` & `django_pony_express-2.1.1/manage.py`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.1.0/pyproject.toml` & `django_pony_express-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.1.0/settings.py` & `django_pony_express-2.1.1/settings.py`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.1.0/tests/services/asynchronous/test_thread_email.py` & `django_pony_express-2.1.1/tests/services/asynchronous/test_thread_email.py`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.1.0/tests/services/base/test_base_mail_factory.py` & `django_pony_express-2.1.1/tests/services/base/test_base_mail_factory.py`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.1.0/tests/services/base/test_base_mail_service.py` & `django_pony_express-2.1.1/tests/services/base/test_base_mail_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,26 +311,26 @@
     @mock.patch("django_pony_express.services.base.BaseEmailService._logger")
     def test_send_and_log_email_success_privacy_active(self, mock_logger):
         service = BaseEmailService(recipient_email_list=["thomas.aquin@example.com"])
         result = service._send_and_log_email(
             msg=EmailMultiAlternatives(subject="The Pony Express", to=["thomas.aquin@example.com"])
         )
 
-        mock_logger.debug.assert_called_with('Email "The Pony Express" successfully sent.')
+        mock_logger.info.assert_called_with('Email "The Pony Express" successfully sent.')
         self.assertEqual(result, 1)
 
     @mock.patch("django_pony_express.services.base.BaseEmailService._logger")
     @mock.patch("django_pony_express.services.base.PONY_LOG_RECIPIENTS", True)
     def test_send_and_log_success_privacy_inactive(self, mock_logger):
         service = BaseEmailService(recipient_email_list=["thomas.aquin@example.com"])
         result = service._send_and_log_email(
             msg=EmailMultiAlternatives(subject="The Pony Express", to=["thomas.aquin@example.com"])
         )
 
-        mock_logger.debug.assert_called_with('Email "The Pony Express" successfully sent to thomas.aquin@example.com.')
+        mock_logger.info.assert_called_with('Email "The Pony Express" successfully sent to thomas.aquin@example.com.')
         self.assertEqual(result, 1)
 
     @mock.patch.object(EmailMultiAlternatives, "send", side_effect=Exception("Broken pony"))
     @mock.patch("django_pony_express.services.base.BaseEmailService._logger")
     def test_send_and_log_email_failure_privacy_active(self, mock_logger, *args):
         service = BaseEmailService(recipient_email_list=["thomas.aquin@example.com"])
         result = service._send_and_log_email(
```

### Comparing `django_pony_express-2.1.0/tests/services/tests/test_email_test_service.py` & `django_pony_express-2.1.1/tests/services/tests/test_email_test_service.py`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.1.0/PKG-INFO` & `django_pony_express-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pony-express
-Version: 2.1.0
+Version: 2.1.1
 Summary: Class-based emails including a test suite for Django
 Author-email: Ambient Digital <hello@ambient.digital>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
```

