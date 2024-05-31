# Comparing `tmp/otc_sphinx_directives-0.2.9.dev1.tar.gz` & `tmp/otc_sphinx_directives-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otc_sphinx_directives-0.2.9.dev1.tar", last modified: Mon Oct 16 08:18:37 2023, max compression
+gzip compressed data, was "otc_sphinx_directives-0.3.0.tar", last modified: Tue Apr  9 08:00:12 2024, max compression
```

## Comparing `otc_sphinx_directives-0.2.9.dev1.tar` & `otc_sphinx_directives-0.3.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 08:18:37.355830 otc_sphinx_directives-0.2.9.dev1/
--rw-r--r--   0 root         (0) root         (0)       50 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/.stestr.conf
--rw-r--r--   0 root         (0) root         (0)      229 2023-10-16 08:18:36.000000 otc_sphinx_directives-0.2.9.dev1/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     2256 2023-10-16 08:18:36.000000 otc_sphinx_directives-0.2.9.dev1/ChangeLog
--rw-r--r--   0 root         (0) root         (0)    11357 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      693 2023-10-16 08:18:37.355830 otc_sphinx_directives-0.2.9.dev1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      110 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 08:18:37.352830 otc_sphinx_directives-0.2.9.dev1/doc/
--rw-r--r--   0 root         (0) root         (0)      394 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/doc/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 08:18:37.352830 otc_sphinx_directives-0.2.9.dev1/doc/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 08:18:37.352830 otc_sphinx_directives-0.2.9.dev1/doc/source/_static/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/doc/source/_static/.placeholder
--rw-r--r--   0 root         (0) root         (0)      899 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/doc/source/_static/ansible.svg
--rw-r--r--   0 root         (0) root         (0)      311 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/doc/source/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 08:18:37.353830 otc_sphinx_directives-0.2.9.dev1/doc/source/examples/
--rw-r--r--   0 root         (0) root         (0)      275 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/doc/source/examples/container_item.rst
--rw-r--r--   0 root         (0) root         (0)      221 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/doc/source/examples/directives_docsportal.rst
--rw-r--r--   0 root         (0) root         (0)      966 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/doc/source/examples/directives_ecs.rst
--rw-r--r--   0 root         (0) root         (0)     1017 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/doc/source/examples/directives_ecs_internal.rst
--rw-r--r--   0 root         (0) root         (0)     1386 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/doc/source/examples/directives_obs.rst
--rw-r--r--   0 root         (0) root         (0)      423 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/doc/source/examples/directives_obs_clean.rst
--rw-r--r--   0 root         (0) root         (0)      191 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/doc/source/examples/index.rst
--rw-r--r--   0 root         (0) root         (0)      118 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/doc/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 08:18:37.354830 otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/
--rw-r--r--   0 root         (0) root         (0)      108 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3748 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/container_item.py
--rw-r--r--   0 root         (0) root         (0)     2383 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/directive_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     3002 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/document_navigator.py
--rw-r--r--   0 root         (0) root         (0)     2993 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/navigator.py
--rw-r--r--   0 root         (0) root         (0)     2513 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/otc_sphinx_directives_setup.py
--rw-r--r--   0 root         (0) root         (0)     3781 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/service_card.py
--rw-r--r--   0 root         (0) root         (0)     2615 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/service_group.py
--rw-r--r--   0 root         (0) root         (0)     2977 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/service_navigator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 08:18:37.355830 otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1767 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/tests/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 08:18:37.351830 otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/tests/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 08:18:37.355830 otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/tests/templates/directive_wrapper/
--rw-r--r--   0 root         (0) root         (0)      791 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/tests/templates/directive_wrapper/conf.py
--rw-r--r--   0 root         (0) root         (0)      250 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/tests/templates/directive_wrapper/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 08:18:37.355830 otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/tests/templates/service_card/
--rw-r--r--   0 root         (0) root         (0)      791 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/tests/templates/service_card/conf.py
--rw-r--r--   0 root         (0) root         (0)      140 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/tests/templates/service_card/index.rst
--rw-r--r--   0 root         (0) root         (0)     2330 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/tests/test_directive_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/tests/test_service_card.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 08:18:37.354830 otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives.egg-info/
--rw-r--r--   0 root         (0) root         (0)      693 2023-10-16 08:18:36.000000 otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1641 2023-10-16 08:18:37.000000 otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       86 2023-10-16 08:18:36.000000 otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-16 08:18:36.000000 otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       47 2023-10-16 08:18:36.000000 otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)       27 2023-10-16 08:18:37.000000 otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-10-16 08:18:37.000000 otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      311 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      586 2023-10-16 08:18:37.355830 otc_sphinx_directives-0.2.9.dev1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      651 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/setup.py
--rw-r--r--   0 root         (0) root         (0)      312 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/test-requirements.txt
--rw-r--r--   0 root         (0) root         (0)     1380 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/tox.ini
--rw-r--r--   0 root         (0) root         (0)      245 2023-10-16 08:15:01.000000 otc_sphinx_directives-0.2.9.dev1/zuul.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 08:00:12.704815 otc_sphinx_directives-0.3.0/
+-rw-r--r--   0 root         (0) root         (0)       50 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/.stestr.conf
+-rw-r--r--   0 root         (0) root         (0)      229 2024-04-09 08:00:12.000000 otc_sphinx_directives-0.3.0/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)     2632 2024-04-09 08:00:12.000000 otc_sphinx_directives-0.3.0/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      688 2024-04-09 08:00:12.704815 otc_sphinx_directives-0.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      110 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 08:00:12.699814 otc_sphinx_directives-0.3.0/doc/
+-rw-r--r--   0 root         (0) root         (0)      394 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/doc/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 08:00:12.700814 otc_sphinx_directives-0.3.0/doc/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 08:00:12.700814 otc_sphinx_directives-0.3.0/doc/source/_static/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/doc/source/_static/.placeholder
+-rw-r--r--   0 root         (0) root         (0)      899 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/doc/source/_static/ansible.svg
+-rw-r--r--   0 root         (0) root         (0)      311 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/doc/source/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 08:00:12.701815 otc_sphinx_directives-0.3.0/doc/source/examples/
+-rw-r--r--   0 root         (0) root         (0)      275 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/doc/source/examples/container_item.rst
+-rw-r--r--   0 root         (0) root         (0)      221 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/doc/source/examples/directives_docsportal.rst
+-rw-r--r--   0 root         (0) root         (0)      966 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/doc/source/examples/directives_ecs.rst
+-rw-r--r--   0 root         (0) root         (0)     1017 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/doc/source/examples/directives_ecs_internal.rst
+-rw-r--r--   0 root         (0) root         (0)     1386 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/doc/source/examples/directives_obs.rst
+-rw-r--r--   0 root         (0) root         (0)      423 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/doc/source/examples/directives_obs_clean.rst
+-rw-r--r--   0 root         (0) root         (0)      191 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/doc/source/examples/index.rst
+-rw-r--r--   0 root         (0) root         (0)      118 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/doc/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 08:00:12.702814 otc_sphinx_directives-0.3.0/otc_sphinx_directives/
+-rw-r--r--   0 root         (0) root         (0)      108 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/otc_sphinx_directives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3748 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/otc_sphinx_directives/container_item.py
+-rw-r--r--   0 root         (0) root         (0)     2383 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/otc_sphinx_directives/directive_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     3228 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/otc_sphinx_directives/document_navigator.py
+-rw-r--r--   0 root         (0) root         (0)     3219 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/otc_sphinx_directives/navigator.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/otc_sphinx_directives/otc_sphinx_directives_setup.py
+-rw-r--r--   0 root         (0) root         (0)     3990 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/otc_sphinx_directives/service_card.py
+-rw-r--r--   0 root         (0) root         (0)     2615 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/otc_sphinx_directives/service_group.py
+-rw-r--r--   0 root         (0) root         (0)     3174 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/otc_sphinx_directives/service_navigator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 08:00:12.703814 otc_sphinx_directives-0.3.0/otc_sphinx_directives/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/otc_sphinx_directives/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1767 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/otc_sphinx_directives/tests/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 08:00:12.698814 otc_sphinx_directives-0.3.0/otc_sphinx_directives/tests/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 08:00:12.704815 otc_sphinx_directives-0.3.0/otc_sphinx_directives/tests/templates/directive_wrapper/
+-rw-r--r--   0 root         (0) root         (0)      791 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/otc_sphinx_directives/tests/templates/directive_wrapper/conf.py
+-rw-r--r--   0 root         (0) root         (0)      250 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/otc_sphinx_directives/tests/templates/directive_wrapper/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 08:00:12.704815 otc_sphinx_directives-0.3.0/otc_sphinx_directives/tests/templates/service_card/
+-rw-r--r--   0 root         (0) root         (0)      791 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/otc_sphinx_directives/tests/templates/service_card/conf.py
+-rw-r--r--   0 root         (0) root         (0)      140 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/otc_sphinx_directives/tests/templates/service_card/index.rst
+-rw-r--r--   0 root         (0) root         (0)     2330 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/otc_sphinx_directives/tests/test_directive_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/otc_sphinx_directives/tests/test_service_card.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 08:00:12.703814 otc_sphinx_directives-0.3.0/otc_sphinx_directives.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      688 2024-04-09 08:00:12.000000 otc_sphinx_directives-0.3.0/otc_sphinx_directives.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-04-09 08:00:12.000000 otc_sphinx_directives-0.3.0/otc_sphinx_directives.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2024-04-09 08:00:12.000000 otc_sphinx_directives-0.3.0/otc_sphinx_directives.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 08:00:12.000000 otc_sphinx_directives-0.3.0/otc_sphinx_directives.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       46 2024-04-09 08:00:12.000000 otc_sphinx_directives-0.3.0/otc_sphinx_directives.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)       27 2024-04-09 08:00:12.000000 otc_sphinx_directives-0.3.0/otc_sphinx_directives.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-09 08:00:12.000000 otc_sphinx_directives-0.3.0/otc_sphinx_directives.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      311 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      586 2024-04-09 08:00:12.704815 otc_sphinx_directives-0.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      651 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)      312 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/test-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     1380 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/tox.ini
+-rw-r--r--   0 root         (0) root         (0)      245 2024-04-09 07:56:40.000000 otc_sphinx_directives-0.3.0/zuul.yaml
```

### Comparing `otc_sphinx_directives-0.2.9.dev1/ChangeLog` & `otc_sphinx_directives-0.3.0/ChangeLog`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,45 @@
 CHANGES
 =======
 
+0.3.0
+-----
+
+* Dark mode pictures (#33)
+
+0.2.16
+------
+
+* icon-svg added to navigator (#32)
+
+0.2.15
+------
+
+* Added icon-svg to document navigator (#31)
+
+0.2.13
+------
+
+* add umn2 (#30)
+
+0.2.12
+------
+
+* blueprints and caf docs added (#29)
+
+0.2.11
+------
+
+* adding new doc type to service card (#28)
+
+0.2.10
+------
+
+* adding new document reference in sphinx directives (#27)
+
 0.2.9.1
 -------
 
 * Added css class to svg icon (#26)
 
 0.2.9
 -----
```

### Comparing `otc_sphinx_directives-0.2.9.dev1/LICENSE` & `otc_sphinx_directives-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.9.dev1/PKG-INFO` & `otc_sphinx_directives-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otc_sphinx_directives
-Version: 0.2.9.dev1
+Version: 0.3.0
 Summary: Open Telekom Cloud Sphinx Directives
 Author: Open Telekom Cloud Ecosystem Squad
 Keywords: Sphinx, Sphinx Directives, Open Telekom Cloud
 Classifier: Framework :: Sphinx
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `otc_sphinx_directives-0.2.9.dev1/doc/source/_static/ansible.svg` & `otc_sphinx_directives-0.3.0/doc/source/_static/ansible.svg`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.9.dev1/doc/source/examples/directives_ecs.rst` & `otc_sphinx_directives-0.3.0/doc/source/examples/directives_ecs.rst`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.9.dev1/doc/source/examples/directives_ecs_internal.rst` & `otc_sphinx_directives-0.3.0/doc/source/examples/directives_ecs_internal.rst`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.9.dev1/doc/source/examples/directives_obs.rst` & `otc_sphinx_directives-0.3.0/doc/source/examples/directives_obs.rst`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/container_item.py` & `otc_sphinx_directives-0.3.0/otc_sphinx_directives/container_item.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/directive_wrapper.py` & `otc_sphinx_directives-0.3.0/otc_sphinx_directives/directive_wrapper.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/document_navigator.py` & `otc_sphinx_directives-0.3.0/otc_sphinx_directives/document_navigator.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,15 +70,18 @@
                 title = doc["service_title"]
                 link = doc.get("link")
                 img = v["service_type"]
                 data += (
                     f'<li class="list-group-item"><a href="{link}">'
                     f'<div class="row">'
                     f'<div class="col-2">'
-                    f'<img src="_static/images/services/{img}.svg">'
+                    f'<picture>'
+                    f'<source class="icon-svg" srcSet="_static/images/services/dark/{img}.svg" media="(prefers-color-scheme: dark)" />'
+                    f'<img class="icon-svg" src="_static/images/services/light/{img}.svg">'
+                    f'</picture>'
                     f'</div>'
                     f'<div class="col-10">{title}</div>'
                     f'</div></a></li>'
                 )
 
         data += '</ul></div>'
```

### Comparing `otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/navigator.py` & `otc_sphinx_directives-0.3.0/otc_sphinx_directives/navigator.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,15 +71,18 @@
                 title = doc["service_title"]
                 link = doc.get("link")
                 img = v["service_type"]
                 data += (
                     f'<li class="list-group-item"><a href="{link}">'
                     f'<div class="row">'
                     f'<div class="col-2">'
-                    f'<img src="_static/images/services/{img}.svg">'
+                    f'<picture>'
+                    f'<source class="icon-svg" srcSet="_static/images/services/dark/{img}.svg" media="(prefers-color-scheme: dark)" />'
+                    f'<img class="icon-svg" src="_static/images/services/light/{img}.svg">'
+                    f'</picture>'
                     f'</div>'
                     f'<div class="col-10">{title}</div>'
                     f'</div></a></li>'
                 )
 
         data += '</ul></div>'
```

### Comparing `otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/otc_sphinx_directives_setup.py` & `otc_sphinx_directives-0.3.0/otc_sphinx_directives/otc_sphinx_directives_setup.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/service_card.py` & `otc_sphinx_directives-0.3.0/otc_sphinx_directives/service_card.py`

 * *Files 19% similar despite different names*

```diff
@@ -51,30 +51,35 @@
 
 class ServiceCard(Directive):
     node_class = service_card
     option_spec = {
         'service_type': directives.unchanged_required,
         'id': directives.unchanged,
         'api-ref': directives.unchanged,
+        'blueprints': directives.unchanged,
+        'caf': directives.unchanged,
         'dev': directives.unchanged,
         'image-creation-guide': directives.unchanged,
         'tool-guide': directives.unchanged,
         'mycredential': directives.unchanged,
         'public-images': directives.unchanged,
         'sdk-ref': directives.unchanged,
         'operation-guide': directives.unchanged,
         'operation-guide-lts': directives.unchanged,
         'parallel-file-system': directives.unchanged,
         'permissions-configuration-guide': directives.unchanged,
         'permissions': directives.unchanged,
         'swiftapi': directives.unchanged,
         's3api': directives.unchanged,
         'umn': directives.unchanged,
+        'umn2': directives.unchanged,
         'best-practice': directives.unchanged,
-        'environment': directives.unchanged
+        'sqlreference': directives.unchanged,
+        'environment': directives.unchanged,
+        'guidelines': directives.unchanged
     }
 
     has_content = True
 
     def run(self):
         node = self.node_class()
         for k in self.option_spec:
```

### Comparing `otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/service_group.py` & `otc_sphinx_directives-0.3.0/otc_sphinx_directives/service_group.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/service_navigator.py` & `otc_sphinx_directives-0.3.0/otc_sphinx_directives/service_navigator.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,18 @@
                 continue
             if environment == "internal" and node['environment'] != "internal":
                 continue
             data += (
                 f'<li class="list-group-item"><a href="{link}">'
                 f'<div class="row">'
                 f'<div class="col-2">'
-                f'<img class="icon-svg" src="_static/images/services/{img}.svg">'
+                f'<picture>'
+                f'<source class="icon-svg" srcSet="_static/images/services/dark/{img}.svg" media="(prefers-color-scheme: dark)" />'
+                f'<img class="icon-svg" src="_static/images/services/light/{img}.svg">'
+                f'</picture>'
                 f'</div>'
                 f'<div class="col-10">{title}</div>'
                 f'</div></a></li>'
             )
 
         data += '</ul></div>'
```

### Comparing `otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/tests/base.py` & `otc_sphinx_directives-0.3.0/otc_sphinx_directives/tests/base.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/tests/templates/directive_wrapper/conf.py` & `otc_sphinx_directives-0.3.0/otc_sphinx_directives/tests/templates/directive_wrapper/conf.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/tests/templates/service_card/conf.py` & `otc_sphinx_directives-0.3.0/otc_sphinx_directives/tests/templates/service_card/conf.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/tests/test_directive_wrapper.py` & `otc_sphinx_directives-0.3.0/otc_sphinx_directives/tests/test_directive_wrapper.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives/tests/test_service_card.py` & `otc_sphinx_directives-0.3.0/otc_sphinx_directives/tests/test_service_card.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives.egg-info/PKG-INFO` & `otc_sphinx_directives-0.3.0/otc_sphinx_directives.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otc-sphinx-directives
-Version: 0.2.9.dev1
+Version: 0.3.0
 Summary: Open Telekom Cloud Sphinx Directives
 Author: Open Telekom Cloud Ecosystem Squad
 Keywords: Sphinx, Sphinx Directives, Open Telekom Cloud
 Classifier: Framework :: Sphinx
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `otc_sphinx_directives-0.2.9.dev1/otc_sphinx_directives.egg-info/SOURCES.txt` & `otc_sphinx_directives-0.3.0/otc_sphinx_directives.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.9.dev1/setup.cfg` & `otc_sphinx_directives-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.9.dev1/setup.py` & `otc_sphinx_directives-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.9.dev1/tox.ini` & `otc_sphinx_directives-0.3.0/tox.ini`

 * *Files identical despite different names*

