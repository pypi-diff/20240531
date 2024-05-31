# Comparing `tmp/py4web-1.20240529.2.tar.gz` & `tmp/py4web-1.20240530.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py4web-1.20240529.2.tar", last modified: Thu May 30 04:27:01 2024, max compression
+gzip compressed data, was "py4web-1.20240530.1.tar", last modified: Fri May 31 05:26:07 2024, max compression
```

## Comparing `py4web-1.20240529.2.tar` & `py4web-1.20240530.1.tar`

### file list

```diff
@@ -1,74 +1,76 @@
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-30 04:27:01.580757 py4web-1.20240529.2/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3594 2023-05-08 00:39:42.000000 py4web-1.20240529.2/LICENSE.md
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7740 2024-05-30 04:27:01.580757 py4web-1.20240529.2/PKG-INFO
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7168 2024-05-16 06:39:59.000000 py4web-1.20240529.2/README.rst
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-30 04:27:01.547423 py4web-1.20240529.2/py4web/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      736 2024-05-30 04:26:20.000000 py4web-1.20240529.2/py4web/__init__.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-30 04:27:01.567423 py4web-1.20240529.2/py4web/assets/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  2990686 2024-05-30 04:26:54.000000 py4web-1.20240529.2/py4web/assets/py4web.app._dashboard.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   199956 2024-05-30 04:26:54.000000 py4web-1.20240529.2/py4web/assets/py4web.app._default.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  4406167 2024-05-30 04:26:55.000000 py4web-1.20240529.2/py4web/assets/py4web.app._documentation.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5245 2024-05-30 04:26:54.000000 py4web-1.20240529.2/py4web/assets/py4web.app._minimal.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    21891 2024-05-30 04:26:54.000000 py4web-1.20240529.2/py4web/assets/py4web.app._scaffold.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  1394074 2024-05-30 04:26:55.000000 py4web-1.20240529.2/py4web/assets/py4web.app.showcase.zip
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    74468 2024-05-30 04:00:44.000000 py4web-1.20240529.2/py4web/core.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    20424 2024-05-16 06:36:11.000000 py4web-1.20240529.2/py4web/server_adapters.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-30 04:27:01.574090 py4web-1.20240529.2/py4web/utils/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2023-05-08 00:39:45.000000 py4web-1.20240529.2/py4web/utils/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    72776 2024-05-30 04:25:52.000000 py4web-1.20240529.2/py4web/utils/auth.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-30 04:27:01.577423 py4web-1.20240529.2/py4web/utils/auth_plugins/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6440 2024-04-28 19:36:37.000000 py4web-1.20240529.2/py4web/utils/auth_plugins/__init__.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      797 2024-04-28 19:36:37.000000 py4web-1.20240529.2/py4web/utils/auth_plugins/basic_auth_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1480 2024-04-28 19:36:37.000000 py4web-1.20240529.2/py4web/utils/auth_plugins/email_auth_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35452 2024-04-28 19:36:37.000000 py4web-1.20240529.2/py4web/utils/auth_plugins/ldap_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1759 2023-05-08 00:39:45.000000 py4web-1.20240529.2/py4web/utils/auth_plugins/oauth2discord.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      671 2024-05-16 06:36:11.000000 py4web-1.20240529.2/py4web/utils/auth_plugins/oauth2facebook.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      474 2024-04-28 19:36:37.000000 py4web-1.20240529.2/py4web/utils/auth_plugins/oauth2github.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      524 2023-05-08 00:39:45.000000 py4web-1.20240529.2/py4web/utils/auth_plugins/oauth2google.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    11958 2024-04-28 19:36:37.000000 py4web-1.20240529.2/py4web/utils/auth_plugins/oauth2google_scoped.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      489 2023-05-08 00:39:45.000000 py4web-1.20240529.2/py4web/utils/auth_plugins/oauth2okta.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2079 2024-04-28 19:36:37.000000 py4web-1.20240529.2/py4web/utils/auth_plugins/oauth2server.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6091 2024-04-28 19:36:37.000000 py4web-1.20240529.2/py4web/utils/auth_plugins/oauth2wpminiorange.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5051 2024-05-16 06:36:11.000000 py4web-1.20240529.2/py4web/utils/auth_plugins/pam.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      187 2023-05-08 00:39:45.000000 py4web-1.20240529.2/py4web/utils/auth_plugins/pam_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6620 2024-04-28 19:36:37.000000 py4web-1.20240529.2/py4web/utils/auth_plugins/saml2_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2810 2024-05-16 06:36:11.000000 py4web-1.20240529.2/py4web/utils/auth_plugins/x509_auth_plugin.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      857 2023-05-08 00:39:45.000000 py4web-1.20240529.2/py4web/utils/cors.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1628 2024-04-28 19:36:37.000000 py4web-1.20240529.2/py4web/utils/dbstore.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2046 2024-05-08 05:21:14.000000 py4web-1.20240529.2/py4web/utils/downloader.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3097 2024-04-28 19:36:37.000000 py4web-1.20240529.2/py4web/utils/factories.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35896 2024-05-30 04:04:31.000000 py4web-1.20240529.2/py4web/utils/form.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    69806 2024-05-30 01:44:44.000000 py4web-1.20240529.2/py4web/utils/grid.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1629 2024-04-28 19:36:37.000000 py4web-1.20240529.2/py4web/utils/jsonrpc.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    34797 2024-04-28 19:36:37.000000 py4web-1.20240529.2/py4web/utils/mailer.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     9181 2024-04-28 19:36:37.000000 py4web-1.20240529.2/py4web/utils/misc.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      502 2023-05-08 00:39:45.000000 py4web-1.20240529.2/py4web/utils/param.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    18284 2024-04-28 19:36:37.000000 py4web-1.20240529.2/py4web/utils/populate.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1602 2024-04-28 19:36:37.000000 py4web-1.20240529.2/py4web/utils/publisher.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2425 2024-04-28 19:36:37.000000 py4web-1.20240529.2/py4web/utils/recaptcha.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3712 2024-04-28 19:36:37.000000 py4web-1.20240529.2/py4web/utils/security.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      123 2024-05-16 06:36:11.000000 py4web-1.20240529.2/py4web/utils/tags.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6510 2024-05-29 14:24:54.000000 py4web-1.20240529.2/py4web/utils/url_signer.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-30 04:27:01.547423 py4web-1.20240529.2/py4web.egg-info/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7740 2024-05-30 04:27:01.000000 py4web-1.20240529.2/py4web.egg-info/PKG-INFO
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1896 2024-05-30 04:27:01.000000 py4web-1.20240529.2/py4web.egg-info/SOURCES.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2024-05-30 04:27:01.000000 py4web-1.20240529.2/py4web.egg-info/dependency_links.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       43 2024-05-30 04:27:01.000000 py4web-1.20240529.2/py4web.egg-info/entry_points.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      237 2024-05-30 04:27:01.000000 py4web-1.20240529.2/py4web.egg-info/requires.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        7 2024-05-30 04:27:01.000000 py4web-1.20240529.2/py4web.egg-info/top_level.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      925 2024-05-30 04:26:02.000000 py4web-1.20240529.2/pyproject.toml
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      462 2024-05-16 06:49:22.000000 py4web-1.20240529.2/requirements.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       38 2024-05-30 04:27:01.580757 py4web-1.20240529.2/setup.cfg
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-30 04:27:01.580757 py4web-1.20240529.2/tests/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3825 2024-05-27 19:27:23.000000 py4web-1.20240529.2/tests/test_action.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8432 2024-05-27 19:27:23.000000 py4web-1.20240529.2/tests/test_auth.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2067 2024-05-27 19:27:23.000000 py4web-1.20240529.2/tests/test_cache.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1440 2024-05-27 19:27:23.000000 py4web-1.20240529.2/tests/test_fixture.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      731 2024-05-27 19:27:23.000000 py4web-1.20240529.2/tests/test_form.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      677 2024-05-27 19:27:23.000000 py4web-1.20240529.2/tests/test_get_error_snapshot.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1035 2024-05-27 19:27:23.000000 py4web-1.20240529.2/tests/test_json.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      793 2024-05-27 19:27:23.000000 py4web-1.20240529.2/tests/test_main.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5102 2024-05-27 19:27:23.000000 py4web-1.20240529.2/tests/test_session.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      990 2024-05-17 05:35:22.000000 py4web-1.20240529.2/tests/test_tags.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      388 2024-05-27 19:27:23.000000 py4web-1.20240529.2/tests/test_template.py
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      415 2024-05-27 19:27:23.000000 py4web-1.20240529.2/tests/test_url.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-31 05:26:07.743723 py4web-1.20240530.1/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3594 2023-05-08 00:39:42.000000 py4web-1.20240530.1/LICENSE.md
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7740 2024-05-31 05:26:07.743723 py4web-1.20240530.1/PKG-INFO
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7168 2024-05-16 06:39:59.000000 py4web-1.20240530.1/README.rst
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-31 05:26:07.707055 py4web-1.20240530.1/py4web/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      736 2024-05-22 05:46:56.000000 py4web-1.20240530.1/py4web/__init__ (zephyrus's conflicted copy 2024-05-30).py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      736 2024-05-31 05:24:13.000000 py4web-1.20240530.1/py4web/__init__.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-31 05:26:07.727055 py4web-1.20240530.1/py4web/assets/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  2990686 2024-05-31 05:26:00.000000 py4web-1.20240530.1/py4web/assets/py4web.app._dashboard.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)   199956 2024-05-31 05:26:00.000000 py4web-1.20240530.1/py4web/assets/py4web.app._default.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  4406167 2024-05-31 05:26:00.000000 py4web-1.20240530.1/py4web/assets/py4web.app._documentation.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5245 2024-05-31 05:26:00.000000 py4web-1.20240530.1/py4web/assets/py4web.app._minimal.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    21891 2024-05-31 05:26:00.000000 py4web-1.20240530.1/py4web/assets/py4web.app._scaffold.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)  1394074 2024-05-31 05:26:01.000000 py4web-1.20240530.1/py4web/assets/py4web.app.showcase.zip
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    74468 2024-05-30 04:00:44.000000 py4web-1.20240530.1/py4web/core.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    20424 2024-05-16 06:36:11.000000 py4web-1.20240530.1/py4web/server_adapters.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-31 05:26:07.737056 py4web-1.20240530.1/py4web/utils/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2023-05-08 00:39:45.000000 py4web-1.20240530.1/py4web/utils/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    72875 2024-05-30 07:18:21.000000 py4web-1.20240530.1/py4web/utils/auth.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-31 05:26:07.740389 py4web-1.20240530.1/py4web/utils/auth_plugins/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6440 2024-04-28 19:36:37.000000 py4web-1.20240530.1/py4web/utils/auth_plugins/__init__.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      797 2024-04-28 19:36:37.000000 py4web-1.20240530.1/py4web/utils/auth_plugins/basic_auth_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1480 2024-04-28 19:36:37.000000 py4web-1.20240530.1/py4web/utils/auth_plugins/email_auth_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35452 2024-04-28 19:36:37.000000 py4web-1.20240530.1/py4web/utils/auth_plugins/ldap_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1759 2023-05-08 00:39:45.000000 py4web-1.20240530.1/py4web/utils/auth_plugins/oauth2discord.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      671 2024-05-16 06:36:11.000000 py4web-1.20240530.1/py4web/utils/auth_plugins/oauth2facebook.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      474 2024-04-28 19:36:37.000000 py4web-1.20240530.1/py4web/utils/auth_plugins/oauth2github.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      524 2023-05-08 00:39:45.000000 py4web-1.20240530.1/py4web/utils/auth_plugins/oauth2google.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    11958 2024-04-28 19:36:37.000000 py4web-1.20240530.1/py4web/utils/auth_plugins/oauth2google_scoped.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      489 2023-05-08 00:39:45.000000 py4web-1.20240530.1/py4web/utils/auth_plugins/oauth2okta.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2079 2024-04-28 19:36:37.000000 py4web-1.20240530.1/py4web/utils/auth_plugins/oauth2server.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6091 2024-04-28 19:36:37.000000 py4web-1.20240530.1/py4web/utils/auth_plugins/oauth2wpminiorange.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5051 2024-05-16 06:36:11.000000 py4web-1.20240530.1/py4web/utils/auth_plugins/pam.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      187 2023-05-08 00:39:45.000000 py4web-1.20240530.1/py4web/utils/auth_plugins/pam_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6620 2024-04-28 19:36:37.000000 py4web-1.20240530.1/py4web/utils/auth_plugins/saml2_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2810 2024-05-16 06:36:11.000000 py4web-1.20240530.1/py4web/utils/auth_plugins/x509_auth_plugin.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      857 2023-05-08 00:39:45.000000 py4web-1.20240530.1/py4web/utils/cors.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1628 2024-04-28 19:36:37.000000 py4web-1.20240530.1/py4web/utils/dbstore.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2046 2024-05-08 05:21:14.000000 py4web-1.20240530.1/py4web/utils/downloader.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3097 2024-04-28 19:36:37.000000 py4web-1.20240530.1/py4web/utils/factories.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    35896 2024-05-30 04:04:31.000000 py4web-1.20240530.1/py4web/utils/form.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    69783 2024-05-22 05:46:26.000000 py4web-1.20240530.1/py4web/utils/grid (zephyrus's conflicted copy 2024-05-30).py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    69806 2024-05-30 01:44:44.000000 py4web-1.20240530.1/py4web/utils/grid.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1629 2024-04-28 19:36:37.000000 py4web-1.20240530.1/py4web/utils/jsonrpc.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    34797 2024-04-28 19:36:37.000000 py4web-1.20240530.1/py4web/utils/mailer.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     9181 2024-04-28 19:36:37.000000 py4web-1.20240530.1/py4web/utils/misc.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      502 2023-05-08 00:39:45.000000 py4web-1.20240530.1/py4web/utils/param.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)    18284 2024-04-28 19:36:37.000000 py4web-1.20240530.1/py4web/utils/populate.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1602 2024-04-28 19:36:37.000000 py4web-1.20240530.1/py4web/utils/publisher.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2425 2024-04-28 19:36:37.000000 py4web-1.20240530.1/py4web/utils/recaptcha.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3712 2024-04-28 19:36:37.000000 py4web-1.20240530.1/py4web/utils/security.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      123 2024-05-16 06:36:11.000000 py4web-1.20240530.1/py4web/utils/tags.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6510 2024-05-29 14:24:54.000000 py4web-1.20240530.1/py4web/utils/url_signer.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-31 05:26:07.710388 py4web-1.20240530.1/py4web.egg-info/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     7740 2024-05-31 05:26:07.000000 py4web-1.20240530.1/py4web.egg-info/PKG-INFO
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2016 2024-05-31 05:26:07.000000 py4web-1.20240530.1/py4web.egg-info/SOURCES.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2024-05-31 05:26:07.000000 py4web-1.20240530.1/py4web.egg-info/dependency_links.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       43 2024-05-31 05:26:07.000000 py4web-1.20240530.1/py4web.egg-info/entry_points.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      237 2024-05-31 05:26:07.000000 py4web-1.20240530.1/py4web.egg-info/requires.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        7 2024-05-31 05:26:07.000000 py4web-1.20240530.1/py4web.egg-info/top_level.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      925 2024-05-31 05:23:53.000000 py4web-1.20240530.1/pyproject.toml
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      462 2024-05-30 07:14:08.000000 py4web-1.20240530.1/requirements.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       38 2024-05-31 05:26:07.743723 py4web-1.20240530.1/setup.cfg
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-31 05:26:07.743723 py4web-1.20240530.1/tests/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     3825 2024-05-27 19:27:23.000000 py4web-1.20240530.1/tests/test_action.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     8432 2024-05-27 19:27:23.000000 py4web-1.20240530.1/tests/test_auth.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2067 2024-05-27 19:27:23.000000 py4web-1.20240530.1/tests/test_cache.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1440 2024-05-27 19:27:23.000000 py4web-1.20240530.1/tests/test_fixture.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      731 2024-05-27 19:27:23.000000 py4web-1.20240530.1/tests/test_form.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      677 2024-05-27 19:27:23.000000 py4web-1.20240530.1/tests/test_get_error_snapshot.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1035 2024-05-27 19:27:23.000000 py4web-1.20240530.1/tests/test_json.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      793 2024-05-27 19:27:23.000000 py4web-1.20240530.1/tests/test_main.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5102 2024-05-27 19:27:23.000000 py4web-1.20240530.1/tests/test_session.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      990 2024-05-17 05:35:22.000000 py4web-1.20240530.1/tests/test_tags.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      388 2024-05-27 19:27:23.000000 py4web-1.20240530.1/tests/test_template.py
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      415 2024-05-27 19:27:23.000000 py4web-1.20240530.1/tests/test_url.py
```

### Comparing `py4web-1.20240529.2/LICENSE.md` & `py4web-1.20240530.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/PKG-INFO` & `py4web-1.20240530.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4web
-Version: 1.20240529.2
+Version: 1.20240530.1
 Summary: A fast, stable, comprehensive web framework
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/py4web
 Project-URL: Bug Tracker, https://github.com/web2py/py4web/issues
 Project-URL: Documentation, https://py4web.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `py4web-1.20240529.2/README.rst` & `py4web-1.20240530.1/README.rst`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/__init__.py` & `py4web-1.20240530.1/py4web/__init__ (zephyrus's conflicted copy 2024-05-30).py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 __author__ = "Massimo Di Pierro <massimo.dipierro@gmail.com>"
 __license__ = "BSD-3-Clause"
-__version__ = "1.20240529.2"
+__version__ = "1.20240518.3"
 
 
 def _maybe_gevent():
     for arg in sys.argv[1:]:
         if "gevent" in arg.lower():
             from gevent import monkey
```

### Comparing `py4web-1.20240529.2/py4web/assets/py4web.app._dashboard.zip` & `py4web-1.20240530.1/py4web/assets/py4web.app._dashboard.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/assets/py4web.app._default.zip` & `py4web-1.20240530.1/py4web/assets/py4web.app._default.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/assets/py4web.app._documentation.zip` & `py4web-1.20240530.1/py4web/assets/py4web.app._documentation.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/assets/py4web.app._minimal.zip` & `py4web-1.20240530.1/py4web/assets/py4web.app._minimal.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/assets/py4web.app._scaffold.zip` & `py4web-1.20240530.1/py4web/assets/py4web.app._scaffold.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/assets/py4web.app.showcase.zip` & `py4web-1.20240530.1/py4web/assets/py4web.app.showcase.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/core.py` & `py4web-1.20240530.1/py4web/core.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/server_adapters.py` & `py4web-1.20240530.1/py4web/server_adapters.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/utils/auth.py` & `py4web-1.20240530.1/py4web/utils/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -408,15 +408,18 @@
                     Field(
                         "past_passwords_hash",
                         "list:string",
                         writable=False,
                         readable=False,
                     )
                 )
-            db.define_table("auth_user", *(auth_fields + self.extra_auth_user_fields))
+            db.define_table(
+                "auth_user",
+                *(auth_fields + self.extra_auth_user_fields),
+                format=lambda u: f"{u.first_name} {u.last_name}")
 
     @property
     def signature(self):
         """Returns a list of fields for a table signature"""
         now = lambda: datetime.datetime.utcnow()
         user = lambda s=self: s.user_id
         fields = [
```

### Comparing `py4web-1.20240529.2/py4web/utils/auth_plugins/__init__.py` & `py4web-1.20240530.1/py4web/utils/auth_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/utils/auth_plugins/basic_auth_plugin.py` & `py4web-1.20240530.1/py4web/utils/auth_plugins/basic_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/utils/auth_plugins/email_auth_plugin.py` & `py4web-1.20240530.1/py4web/utils/auth_plugins/email_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/utils/auth_plugins/ldap_plugin.py` & `py4web-1.20240530.1/py4web/utils/auth_plugins/ldap_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/utils/auth_plugins/oauth2discord.py` & `py4web-1.20240530.1/py4web/utils/auth_plugins/oauth2discord.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/utils/auth_plugins/oauth2facebook.py` & `py4web-1.20240530.1/py4web/utils/auth_plugins/oauth2facebook.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/utils/auth_plugins/oauth2google.py` & `py4web-1.20240530.1/py4web/utils/auth_plugins/oauth2google.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/utils/auth_plugins/oauth2google_scoped.py` & `py4web-1.20240530.1/py4web/utils/auth_plugins/oauth2google_scoped.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/utils/auth_plugins/oauth2server.py` & `py4web-1.20240530.1/py4web/utils/auth_plugins/oauth2server.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/utils/auth_plugins/oauth2wpminiorange.py` & `py4web-1.20240530.1/py4web/utils/auth_plugins/oauth2wpminiorange.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/utils/auth_plugins/pam.py` & `py4web-1.20240530.1/py4web/utils/auth_plugins/pam.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/utils/auth_plugins/saml2_plugin.py` & `py4web-1.20240530.1/py4web/utils/auth_plugins/saml2_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/utils/auth_plugins/x509_auth_plugin.py` & `py4web-1.20240530.1/py4web/utils/auth_plugins/x509_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/utils/cors.py` & `py4web-1.20240530.1/py4web/utils/cors.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/utils/dbstore.py` & `py4web-1.20240530.1/py4web/utils/dbstore.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/utils/downloader.py` & `py4web-1.20240530.1/py4web/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/utils/factories.py` & `py4web-1.20240530.1/py4web/utils/factories.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/utils/form.py` & `py4web-1.20240530.1/py4web/utils/form.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/utils/grid.py` & `py4web-1.20240530.1/py4web/utils/grid.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/utils/jsonrpc.py` & `py4web-1.20240530.1/py4web/utils/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/utils/mailer.py` & `py4web-1.20240530.1/py4web/utils/mailer.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/utils/misc.py` & `py4web-1.20240530.1/py4web/utils/misc.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/utils/populate.py` & `py4web-1.20240530.1/py4web/utils/populate.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/utils/publisher.py` & `py4web-1.20240530.1/py4web/utils/publisher.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/utils/recaptcha.py` & `py4web-1.20240530.1/py4web/utils/recaptcha.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/utils/security.py` & `py4web-1.20240530.1/py4web/utils/security.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web/utils/url_signer.py` & `py4web-1.20240530.1/py4web/utils/url_signer.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/py4web.egg-info/PKG-INFO` & `py4web-1.20240530.1/py4web.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4web
-Version: 1.20240529.2
+Version: 1.20240530.1
 Summary: A fast, stable, comprehensive web framework
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/py4web
 Project-URL: Bug Tracker, https://github.com/web2py/py4web/issues
 Project-URL: Documentation, https://py4web.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `py4web-1.20240529.2/py4web.egg-info/SOURCES.txt` & `py4web-1.20240530.1/py4web.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.md
 README.rst
 pyproject.toml
 requirements.txt
+py4web/__init__ (zephyrus's conflicted copy 2024-05-30).py
 py4web/__init__.py
 py4web/core.py
 py4web/server_adapters.py
 py4web.egg-info/PKG-INFO
 py4web.egg-info/SOURCES.txt
 py4web.egg-info/dependency_links.txt
 py4web.egg-info/entry_points.txt
@@ -20,14 +21,15 @@
 py4web/utils/__init__.py
 py4web/utils/auth.py
 py4web/utils/cors.py
 py4web/utils/dbstore.py
 py4web/utils/downloader.py
 py4web/utils/factories.py
 py4web/utils/form.py
+py4web/utils/grid (zephyrus's conflicted copy 2024-05-30).py
 py4web/utils/grid.py
 py4web/utils/jsonrpc.py
 py4web/utils/mailer.py
 py4web/utils/misc.py
 py4web/utils/param.py
 py4web/utils/populate.py
 py4web/utils/publisher.py
```

### Comparing `py4web-1.20240529.2/pyproject.toml` & `py4web-1.20240530.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py4web"
-version = "1.20240529.2"
+version = "1.20240530.1"
 authors = [{ name="Massimo Di Pierro", email="massimo.dipierro@gmail.com" },]
 description = "A fast, stable, comprehensive web framework"
 readme = "README.rst"
 requires-python = ">=3.7"
 classifiers = [
       "Programming Language :: Python :: 3",
       "License :: OSI Approved :: BSD License",
```

### Comparing `py4web-1.20240529.2/tests/test_action.py` & `py4web-1.20240530.1/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/tests/test_auth.py` & `py4web-1.20240530.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/tests/test_cache.py` & `py4web-1.20240530.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/tests/test_fixture.py` & `py4web-1.20240530.1/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/tests/test_form.py` & `py4web-1.20240530.1/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/tests/test_get_error_snapshot.py` & `py4web-1.20240530.1/tests/test_get_error_snapshot.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/tests/test_json.py` & `py4web-1.20240530.1/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/tests/test_main.py` & `py4web-1.20240530.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/tests/test_session.py` & `py4web-1.20240530.1/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20240529.2/tests/test_tags.py` & `py4web-1.20240530.1/tests/test_tags.py`

 * *Files identical despite different names*

