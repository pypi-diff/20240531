# Comparing `tmp/zope.testbrowser-6.0.tar.gz` & `tmp/zope.testbrowser-7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.testbrowser-6.0.tar", last modified: Mon Mar 27 11:38:00 2023, max compression
+gzip compressed data, was "zope.testbrowser-7.0.tar", last modified: Fri May 31 08:45:37 2024, max compression
```

## Comparing `zope.testbrowser-6.0.tar` & `zope.testbrowser-7.0.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-27 11:38:00.359291 zope.testbrowser-6.0/
--rw-r--r--   0 mac        (513) staff       (20)    16340 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      804 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)       32 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/COPYRIGHT.rst
--rw-r--r--   0 mac        (513) staff       (20)     2070 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/LICENSE.rst
--rw-r--r--   0 mac        (513) staff       (20)      447 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)    18466 2023-03-27 11:38:00.359445 zope.testbrowser-6.0/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      900 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      946 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/buildout.cfg
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-27 11:38:00.345449 zope.testbrowser-6.0/docs/
--rw-r--r--   0 mac        (513) staff       (20)     6798 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/docs/Makefile
--rw-r--r--   0 mac        (513) staff       (20)      917 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/docs/api.rst
--rw-r--r--   0 mac        (513) staff       (20)     8601 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/docs/conf.py
--rw-r--r--   0 mac        (513) staff       (20)    25998 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/docs/cookies.rst
--rw-r--r--   0 mac        (513) staff       (20)      216 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/docs/index.rst
--rw-r--r--   0 mac        (513) staff       (20)     6719 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/docs/make.bat
--rw-r--r--   0 mac        (513) staff       (20)    50825 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/docs/narrative.rst
--rw-r--r--   0 mac        (513) staff       (20)       45 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/rtd.txt
--rw-r--r--   0 mac        (513) staff       (20)      469 2023-03-27 11:38:00.360248 zope.testbrowser-6.0/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     2925 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-27 11:38:00.338663 zope.testbrowser-6.0/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-27 11:38:00.345858 zope.testbrowser-6.0/src/zope/
--rw-r--r--   0 mac        (513) staff       (20)       56 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-27 11:38:00.351472 zope.testbrowser-6.0/src/zope/testbrowser/
--rw-r--r--   0 mac        (513) staff       (20)      685 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/testbrowser/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)    49033 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/testbrowser/browser.py
--rw-r--r--   0 mac        (513) staff       (20)    14194 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/testbrowser/cookies.py
--rw-r--r--   0 mac        (513) staff       (20)     6005 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/testbrowser/fixed-bugs.txt
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-27 11:38:00.356492 zope.testbrowser-6.0/src/zope/testbrowser/ftests/
--rw-r--r--   0 mac        (513) staff       (20)      632 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/testbrowser/ftests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     6679 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/testbrowser/ftests/controls.html
--rw-r--r--   0 mac        (513) staff       (20)       55 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/testbrowser/ftests/cookies.html
--rw-r--r--   0 mac        (513) staff       (20)     1361 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/testbrowser/ftests/forms.html
--rw-r--r--   0 mac        (513) staff       (20)      112 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/testbrowser/ftests/fragment.html
--rw-r--r--   0 mac        (513) staff       (20)     1168 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/testbrowser/ftests/navigate.html
--rw-r--r--   0 mac        (513) staff       (20)       55 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/testbrowser/ftests/notitle.html
--rw-r--r--   0 mac        (513) staff       (20)      373 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/testbrowser/ftests/oneform.html
--rw-r--r--   0 mac        (513) staff       (20)      426 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/testbrowser/ftests/radio.html
--rw-r--r--   0 mac        (513) staff       (20)      109 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/testbrowser/ftests/simple.html
--rw-r--r--   0 mac        (513) staff       (20)      540 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/testbrowser/ftests/status_lead.html
--rw-r--r--   0 mac        (513) staff       (20)      453 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/testbrowser/ftests/textarea.html
--rw-r--r--   0 mac        (513) staff       (20)     5812 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/testbrowser/ftests/wsgitestapp.py
--rw-r--r--   0 mac        (513) staff       (20)     1506 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/testbrowser/ftests/zope3logo.gif
--rw-r--r--   0 mac        (513) staff       (20)    15906 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/testbrowser/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)      792 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/testbrowser/over_the_wire.txt
--rw-r--r--   0 mac        (513) staff       (20)     1516 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/testbrowser/testing.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-27 11:38:00.358987 zope.testbrowser-6.0/src/zope/testbrowser/tests/
--rw-r--r--   0 mac        (513) staff       (20)        0 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/testbrowser/tests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     2942 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/testbrowser/tests/helper.py
--rw-r--r--   0 mac        (513) staff       (20)      836 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/testbrowser/tests/test_bbb.py
--rw-r--r--   0 mac        (513) staff       (20)    44843 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/testbrowser/tests/test_browser.py
--rw-r--r--   0 mac        (513) staff       (20)     1684 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/testbrowser/tests/test_cookies.py
--rw-r--r--   0 mac        (513) staff       (20)     1363 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/testbrowser/tests/test_doctests.py
--rw-r--r--   0 mac        (513) staff       (20)    14948 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/testbrowser/tests/test_wsgi.py
--rw-r--r--   0 mac        (513) staff       (20)     6731 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/testbrowser/utils.py
--rw-r--r--   0 mac        (513) staff       (20)     5610 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/src/zope/testbrowser/wsgi.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-27 11:38:00.348277 zope.testbrowser-6.0/src/zope.testbrowser.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)    18466 2023-03-27 11:38:00.000000 zope.testbrowser-6.0/src/zope.testbrowser.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     1727 2023-03-27 11:38:00.000000 zope.testbrowser-6.0/src/zope.testbrowser.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-03-27 11:38:00.000000 zope.testbrowser-6.0/src/zope.testbrowser.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2023-03-27 11:38:00.000000 zope.testbrowser-6.0/src/zope.testbrowser.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-03-27 11:38:00.000000 zope.testbrowser-6.0/src/zope.testbrowser.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)      283 2023-03-27 11:38:00.000000 zope.testbrowser-6.0/src/zope.testbrowser.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2023-03-27 11:38:00.000000 zope.testbrowser-6.0/src/zope.testbrowser.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1931 2023-03-27 11:37:59.000000 zope.testbrowser-6.0/tox.ini
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-31 08:45:37.358087 zope.testbrowser-7.0/
+-rw-r--r--   0 jens       (501) staff       (20)      669 2024-05-31 07:35:28.000000 zope.testbrowser-7.0/.readthedocs.yaml
+-rw-r--r--   0 jens       (501) staff       (20)    16462 2024-05-31 08:41:26.000000 zope.testbrowser-7.0/CHANGES.rst
+-rw-r--r--   0 jens       (501) staff       (20)      804 2024-05-31 07:35:28.000000 zope.testbrowser-7.0/CONTRIBUTING.md
+-rw-r--r--   0 jens       (501) staff       (20)       32 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/COPYRIGHT.rst
+-rw-r--r--   0 jens       (501) staff       (20)     2070 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/LICENSE.rst
+-rw-r--r--   0 jens       (501) staff       (20)      462 2024-05-31 07:35:28.000000 zope.testbrowser-7.0/MANIFEST.in
+-rw-r--r--   0 jens       (501) staff       (20)    19504 2024-05-31 08:45:37.357989 zope.testbrowser-7.0/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)     1071 2024-05-31 08:41:07.000000 zope.testbrowser-7.0/README.rst
+-rw-r--r--   0 jens       (501) staff       (20)      946 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/buildout.cfg
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-31 08:45:37.353390 zope.testbrowser-7.0/docs/
+-rw-r--r--   0 jens       (501) staff       (20)     6798 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/docs/Makefile
+-rw-r--r--   0 jens       (501) staff       (20)      917 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/docs/api.rst
+-rw-r--r--   0 jens       (501) staff       (20)     8615 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/docs/conf.py
+-rw-r--r--   0 jens       (501) staff       (20)    25998 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/docs/cookies.rst
+-rw-r--r--   0 jens       (501) staff       (20)      216 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/docs/index.rst
+-rw-r--r--   0 jens       (501) staff       (20)     6719 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/docs/make.bat
+-rw-r--r--   0 jens       (501) staff       (20)    50846 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/docs/narrative.rst
+-rw-r--r--   0 jens       (501) staff       (20)       35 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/docs/requirements.txt
+-rw-r--r--   0 jens       (501) staff       (20)      441 2024-05-31 08:45:37.358329 zope.testbrowser-7.0/setup.cfg
+-rw-r--r--   0 jens       (501) staff       (20)     3052 2024-05-31 08:41:40.000000 zope.testbrowser-7.0/setup.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-31 08:45:37.351102 zope.testbrowser-7.0/src/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-31 08:45:37.353482 zope.testbrowser-7.0/src/zope/
+-rw-r--r--   0 jens       (501) staff       (20)       56 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/__init__.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-31 08:45:37.355353 zope.testbrowser-7.0/src/zope/testbrowser/
+-rw-r--r--   0 jens       (501) staff       (20)      685 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/testbrowser/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)    49033 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/testbrowser/browser.py
+-rw-r--r--   0 jens       (501) staff       (20)    14170 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/testbrowser/cookies.py
+-rw-r--r--   0 jens       (501) staff       (20)     6005 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/testbrowser/fixed-bugs.txt
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-31 08:45:37.356730 zope.testbrowser-7.0/src/zope/testbrowser/ftests/
+-rw-r--r--   0 jens       (501) staff       (20)      632 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/testbrowser/ftests/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)     6679 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/testbrowser/ftests/controls.html
+-rw-r--r--   0 jens       (501) staff       (20)       55 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/testbrowser/ftests/cookies.html
+-rw-r--r--   0 jens       (501) staff       (20)     1361 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/testbrowser/ftests/forms.html
+-rw-r--r--   0 jens       (501) staff       (20)      112 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/testbrowser/ftests/fragment.html
+-rw-r--r--   0 jens       (501) staff       (20)     1168 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/testbrowser/ftests/navigate.html
+-rw-r--r--   0 jens       (501) staff       (20)       55 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/testbrowser/ftests/notitle.html
+-rw-r--r--   0 jens       (501) staff       (20)      373 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/testbrowser/ftests/oneform.html
+-rw-r--r--   0 jens       (501) staff       (20)      426 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/testbrowser/ftests/radio.html
+-rw-r--r--   0 jens       (501) staff       (20)      109 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/testbrowser/ftests/simple.html
+-rw-r--r--   0 jens       (501) staff       (20)      540 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/testbrowser/ftests/status_lead.html
+-rw-r--r--   0 jens       (501) staff       (20)      453 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/testbrowser/ftests/textarea.html
+-rw-r--r--   0 jens       (501) staff       (20)     5812 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/testbrowser/ftests/wsgitestapp.py
+-rw-r--r--   0 jens       (501) staff       (20)     1506 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/testbrowser/ftests/zope3logo.gif
+-rw-r--r--   0 jens       (501) staff       (20)    15906 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/testbrowser/interfaces.py
+-rw-r--r--   0 jens       (501) staff       (20)      752 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/testbrowser/over_the_wire.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1516 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/testbrowser/testing.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-31 08:45:37.357505 zope.testbrowser-7.0/src/zope/testbrowser/tests/
+-rw-r--r--   0 jens       (501) staff       (20)        0 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/testbrowser/tests/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)     1880 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/testbrowser/tests/helper.py
+-rw-r--r--   0 jens       (501) staff       (20)      836 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/testbrowser/tests/test_bbb.py
+-rw-r--r--   0 jens       (501) staff       (20)    44843 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/testbrowser/tests/test_browser.py
+-rw-r--r--   0 jens       (501) staff       (20)     1684 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/testbrowser/tests/test_cookies.py
+-rw-r--r--   0 jens       (501) staff       (20)     1363 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/testbrowser/tests/test_doctests.py
+-rw-r--r--   0 jens       (501) staff       (20)    14948 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/testbrowser/tests/test_wsgi.py
+-rw-r--r--   0 jens       (501) staff       (20)     6731 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/testbrowser/utils.py
+-rw-r--r--   0 jens       (501) staff       (20)     5610 2024-05-31 07:34:08.000000 zope.testbrowser-7.0/src/zope/testbrowser/wsgi.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-31 08:45:37.354233 zope.testbrowser-7.0/src/zope.testbrowser.egg-info/
+-rw-r--r--   0 jens       (501) staff       (20)    19504 2024-05-31 08:45:37.000000 zope.testbrowser-7.0/src/zope.testbrowser.egg-info/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)     1759 2024-05-31 08:45:37.000000 zope.testbrowser-7.0/src/zope.testbrowser.egg-info/SOURCES.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2024-05-31 08:45:37.000000 zope.testbrowser-7.0/src/zope.testbrowser.egg-info/dependency_links.txt
+-rw-r--r--   0 jens       (501) staff       (20)        5 2024-05-31 08:45:37.000000 zope.testbrowser-7.0/src/zope.testbrowser.egg-info/namespace_packages.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2024-05-31 07:35:32.000000 zope.testbrowser-7.0/src/zope.testbrowser.egg-info/not-zip-safe
+-rw-r--r--   0 jens       (501) staff       (20)      322 2024-05-31 08:45:37.000000 zope.testbrowser-7.0/src/zope.testbrowser.egg-info/requires.txt
+-rw-r--r--   0 jens       (501) staff       (20)        5 2024-05-31 08:45:37.000000 zope.testbrowser-7.0/src/zope.testbrowser.egg-info/top_level.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2374 2024-05-31 08:41:07.000000 zope.testbrowser-7.0/tox.ini
```

### Comparing `zope.testbrowser-6.0/CHANGES.rst` & `zope.testbrowser-7.0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 =======
 CHANGES
 =======
 
+7.0 (2024-05-31)
+----------------
+
+- Add support for Python 3.12 and 3.13 as of 3.13b1.
+
+- Drop support for Python 3.7.
+
+
 6.0 (2023-03-27)
 ----------------
 
 - Drop support for Python 2.7, 3.5, 3.6.
 
 - Drop support for deprecated ``python setup.py test``.
```

### Comparing `zope.testbrowser-6.0/CONTRIBUTING.md` & `zope.testbrowser-7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zope.testbrowser-6.0/LICENSE.rst` & `zope.testbrowser-7.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `zope.testbrowser-6.0/PKG-INFO` & `zope.testbrowser-7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,70 @@
 Metadata-Version: 2.1
 Name: zope.testbrowser
-Version: 6.0
+Version: 7.0
 Summary: Programmable browser for functional black-box tests
 Home-page: https://github.com/zopefoundation/zope.testbrowser
 Author: Zope Corporation and Contributors
 Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Project-URL: Documentation, https://zopetestbrowser.readthedocs.io/
 Keywords: headless browser functional tests WSGI HTTP HTML form
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Internet :: WWW/HTTP
-Requires-Python: >=3.7
+Requires-Python: >=3.8
+License-File: LICENSE.rst
+Requires-Dist: setuptools
+Requires-Dist: zope.interface
+Requires-Dist: zope.schema
+Requires-Dist: zope.cachedescriptors
+Requires-Dist: pytz
+Requires-Dist: WebTest>=2.0.30
+Requires-Dist: BeautifulSoup4
+Requires-Dist: SoupSieve>=1.9.0
+Requires-Dist: WSGIProxy2
+Requires-Dist: legacy-cgi; python_version > "3.12"
 Provides-Extra: docs
+Requires-Dist: Sphinx; extra == "docs"
+Requires-Dist: sphinx_rtd_theme; extra == "docs"
+Requires-Dist: repoze.sphinx.autointerface; extra == "docs"
+Requires-Dist: zope.app.wsgi; extra == "docs"
 Provides-Extra: test
-Provides-Extra: test_bbb
+Requires-Dist: zope.testing; extra == "test"
+Requires-Dist: mock; extra == "test"
+Requires-Dist: zope.testrunner; extra == "test"
+Provides-Extra: test-bbb
+Requires-Dist: zope.testbrowser[test]; extra == "test-bbb"
 Provides-Extra: wsgi
-License-File: LICENSE.rst
 
 ``zope.testbrowser`` README
 ===========================
 
 .. image:: https://img.shields.io/pypi/v/zope.testbrowser.svg
         :target: https://pypi.org/project/zope.testbrowser/
         :alt: Latest Version
 
+.. image:: https://img.shields.io/pypi/pyversions/zope.testbrowser.svg
+        :target: https://pypi.org/project/zope.testbrowser/
+        :alt: Supported Python versions
+
 .. image:: https://github.com/zopefoundation/zope.testbrowser/actions/workflows/tests.yml/badge.svg
         :target: https://github.com/zopefoundation/zope.testbrowser/actions/workflows/tests.yml
 
-
 .. image:: https://readthedocs.org/projects/zopetestbrowser/badge/?version=latest
         :target: http://zopetestbrowser.readthedocs.org/en/latest/
         :alt: Documentation Status
 
 ``zope.testbrowser`` provides an easy-to-use programmable web browser
 with special focus on testing.  It is used in Zope, but it's not Zope
 specific at all.  For instance, it can be used to test or otherwise
@@ -51,14 +73,22 @@
 Documentation is available at: https://zopetestbrowser.readthedocs.org
 
 
 =======
 CHANGES
 =======
 
+7.0 (2024-05-31)
+----------------
+
+- Add support for Python 3.12 and 3.13 as of 3.13b1.
+
+- Drop support for Python 3.7.
+
+
 6.0 (2023-03-27)
 ----------------
 
 - Drop support for Python 2.7, 3.5, 3.6.
 
 - Drop support for deprecated ``python setup.py test``.
```

### Comparing `zope.testbrowser-6.0/README.rst` & `zope.testbrowser-7.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 ``zope.testbrowser`` README
 ===========================
 
 .. image:: https://img.shields.io/pypi/v/zope.testbrowser.svg
         :target: https://pypi.org/project/zope.testbrowser/
         :alt: Latest Version
 
+.. image:: https://img.shields.io/pypi/pyversions/zope.testbrowser.svg
+        :target: https://pypi.org/project/zope.testbrowser/
+        :alt: Supported Python versions
+
 .. image:: https://github.com/zopefoundation/zope.testbrowser/actions/workflows/tests.yml/badge.svg
         :target: https://github.com/zopefoundation/zope.testbrowser/actions/workflows/tests.yml
 
-
 .. image:: https://readthedocs.org/projects/zopetestbrowser/badge/?version=latest
         :target: http://zopetestbrowser.readthedocs.org/en/latest/
         :alt: Documentation Status
 
 ``zope.testbrowser`` provides an easy-to-use programmable web browser
 with special focus on testing.  It is used in Zope, but it's not Zope
 specific at all.  For instance, it can be used to test or otherwise
```

### Comparing `zope.testbrowser-6.0/buildout.cfg` & `zope.testbrowser-7.0/buildout.cfg`

 * *Files identical despite different names*

### Comparing `zope.testbrowser-6.0/docs/Makefile` & `zope.testbrowser-7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zope.testbrowser-6.0/docs/api.rst` & `zope.testbrowser-7.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `zope.testbrowser-6.0/docs/conf.py` & `zope.testbrowser-7.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
 #html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+# html_static_path = ['_static']
 
 # Add any extra paths that contain custom files (such as robots.txt or
 # .htaccess) here, relative to this directory. These files are copied
 # directly to the root of the documentation.
 #html_extra_path = []
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
@@ -262,8 +262,8 @@
 #texinfo_show_urls = 'footnote'
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
 #texinfo_no_detailmenu = False
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {'http://docs.python.org/': None}
+intersphinx_mapping = {'python': ('http://docs.python.org/', None)}
```

### Comparing `zope.testbrowser-6.0/docs/cookies.rst` & `zope.testbrowser-7.0/docs/cookies.rst`

 * *Files identical despite different names*

### Comparing `zope.testbrowser-6.0/docs/make.bat` & `zope.testbrowser-7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zope.testbrowser-6.0/docs/narrative.rst` & `zope.testbrowser-7.0/docs/narrative.rst`

 * *Files 0% similar despite different names*

```diff
@@ -241,27 +241,27 @@
 As you can see, the `contents` of the browser does not return any HTTP
 headers.  The headers are accessible via a separate attribute, which is an
 ``http.client.HTTPMessage`` instance (from the Python's standard
 library):
 
 .. doctest::
 
-    >>> from six.moves import http_client
+    >>> import http.client
     >>> browser.open('http://localhost/@@/testbrowser/simple.html')
-    >>> isinstance(browser.headers, http_client.HTTPMessage)
+    >>> isinstance(browser.headers, http.client.HTTPMessage)
     True
 
 The headers can be accessed as a string:
 
 .. doctest::
 
     >>> print(browser.headers)
     ... # doctest: +NORMALIZE_WHITESPACE
     Status: 200 OK
-    Content-Length: 109
+    Content-Length: ...
     Content-Type: text/html; charset=UTF-8
 
 Or as a mapping:
 
 .. doctest::
 
     >>> browser.headers['content-type']
@@ -376,15 +376,15 @@
     '...Message: <em>By Link Text</em>...'
 
 When finding a link by its text, whitespace is normalized.
 
 .. doctest::
 
     >>> browser.open('http://localhost/@@/testbrowser/navigate.html')
-    >>> browser.contents
+    >>> browser.contents.replace('\r', '')
     '...> Link Text \n    with     Whitespace\tNormalization (and parens) </...'
     >>> link = browser.getLink('Link Text with Whitespace Normalization '
     ...                        '(and parens)')
     >>> link
     <Link text='Link Text with Whitespace Normalization (and parens)'...>
     >>> link.text
     'Link Text with Whitespace Normalization (and parens)'
@@ -998,15 +998,15 @@
    :options: +NORMALIZE_WHITESPACE
 
     >>> ctrl = browser.getControl('Text Area Control')
     >>> ctrl
     <Control name='textarea-value' type='textarea'>
     >>> verifyObject(interfaces.IControl, ctrl)
     True
-    >>> ctrl.value
+    >>> ctrl.value.replace('\r', '')
     '        Text inside\n        area!\n      '
     >>> ctrl.value = 'A lot of\n text.'
     >>> ctrl.disabled
     False
     >>> ctrl.multiple
     False
```

### Comparing `zope.testbrowser-6.0/setup.py` & `zope.testbrowser-7.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,54 +25,56 @@
 
 long_description = (README + '\n\n' + CHANGES)
 
 tests_require = ['zope.testing', 'mock', 'zope.testrunner']
 
 setup(
     name='zope.testbrowser',
-    version='6.0',
+    version='7.0',
     url='https://github.com/zopefoundation/zope.testbrowser',
     license='ZPL 2.1',
     project_urls={
         'Documentation': 'https://zopetestbrowser.readthedocs.io/',
     },
     description='Programmable browser for functional black-box tests',
     author='Zope Corporation and Contributors',
     author_email='zope-dev@zope.dev',
     long_description=long_description,
     classifiers=[
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Zope Public License',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
+        'Programming Language :: Python :: 3.13',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Topic :: Software Development :: Testing',
         'Topic :: Internet :: WWW/HTTP',
     ],
     keywords='headless browser functional tests WSGI HTTP HTML form',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     namespace_packages=['zope'],
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     install_requires=[
         'setuptools',
         'zope.interface',
         'zope.schema',
         'zope.cachedescriptors',
         'pytz',
         'WebTest >= 2.0.30',
         'BeautifulSoup4',
         'SoupSieve >= 1.9.0',
         'WSGIProxy2',
+        'legacy-cgi; python_version > "3.12"',  # WebOb uses the cgi module
     ],
     extras_require={
         'docs': [
             'Sphinx',
             'sphinx_rtd_theme',
             'repoze.sphinx.autointerface',
             'zope.app.wsgi',
```

### Comparing `zope.testbrowser-6.0/src/zope/testbrowser/__init__.py` & `zope.testbrowser-7.0/src/zope/testbrowser/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.testbrowser-6.0/src/zope/testbrowser/browser.py` & `zope.testbrowser-7.0/src/zope/testbrowser/browser.py`

 * *Files identical despite different names*

### Comparing `zope.testbrowser-6.0/src/zope/testbrowser/cookies.py` & `zope.testbrowser-7.0/src/zope/testbrowser/cookies.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import time
 import urllib.parse
 import urllib.request
 from collections.abc import MutableMapping
 from urllib.parse import quote as url_quote
 
 import pytz
+
 import zope.interface
 
 from zope.testbrowser import interfaces
 from zope.testbrowser import utils
 
 
 # Cookies class helpers
@@ -197,16 +198,14 @@
 
     def keys(self):
         return [ck.name for ck in self._get_cookies()]
 
     def __iter__(self):
         return (ck.name for ck in self._get_cookies())
 
-    iterkeys = __iter__
-
     def iterinfo(self, key=None):
         return (self._getinfo(ck) for ck in self._get_cookies(key))
 
     def iteritems(self):
         return ((ck.name, ck.value) for ck in self._get_cookies())
 
     def has_key(self, key):
```

### Comparing `zope.testbrowser-6.0/src/zope/testbrowser/fixed-bugs.txt` & `zope.testbrowser-7.0/src/zope/testbrowser/fixed-bugs.txt`

 * *Files identical despite different names*

### Comparing `zope.testbrowser-6.0/src/zope/testbrowser/ftests/__init__.py` & `zope.testbrowser-7.0/src/zope/testbrowser/ftests/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.testbrowser-6.0/src/zope/testbrowser/ftests/controls.html` & `zope.testbrowser-7.0/src/zope/testbrowser/ftests/controls.html`

 * *Files identical despite different names*

### Comparing `zope.testbrowser-6.0/src/zope/testbrowser/ftests/forms.html` & `zope.testbrowser-7.0/src/zope/testbrowser/ftests/forms.html`

 * *Files identical despite different names*

### Comparing `zope.testbrowser-6.0/src/zope/testbrowser/ftests/navigate.html` & `zope.testbrowser-7.0/src/zope/testbrowser/ftests/navigate.html`

 * *Files identical despite different names*

### Comparing `zope.testbrowser-6.0/src/zope/testbrowser/ftests/status_lead.html` & `zope.testbrowser-7.0/src/zope/testbrowser/ftests/status_lead.html`

 * *Files identical despite different names*

### Comparing `zope.testbrowser-6.0/src/zope/testbrowser/ftests/wsgitestapp.py` & `zope.testbrowser-7.0/src/zope/testbrowser/ftests/wsgitestapp.py`

 * *Files identical despite different names*

### Comparing `zope.testbrowser-6.0/src/zope/testbrowser/ftests/zope3logo.gif` & `zope.testbrowser-7.0/src/zope/testbrowser/ftests/zope3logo.gif`

 * *Files identical despite different names*

### Comparing `zope.testbrowser-6.0/src/zope/testbrowser/interfaces.py` & `zope.testbrowser-7.0/src/zope/testbrowser/interfaces.py`

 * *Files identical despite different names*

### Comparing `zope.testbrowser-6.0/src/zope/testbrowser/testing.py` & `zope.testbrowser-7.0/src/zope/testbrowser/testing.py`

 * *Files identical despite different names*

### Comparing `zope.testbrowser-6.0/src/zope/testbrowser/tests/test_bbb.py` & `zope.testbrowser-7.0/src/zope/testbrowser/tests/test_bbb.py`

 * *Files identical despite different names*

### Comparing `zope.testbrowser-6.0/src/zope/testbrowser/tests/test_browser.py` & `zope.testbrowser-7.0/src/zope/testbrowser/tests/test_browser.py`

 * *Files identical despite different names*

### Comparing `zope.testbrowser-6.0/src/zope/testbrowser/tests/test_cookies.py` & `zope.testbrowser-7.0/src/zope/testbrowser/tests/test_cookies.py`

 * *Files identical despite different names*

### Comparing `zope.testbrowser-6.0/src/zope/testbrowser/tests/test_doctests.py` & `zope.testbrowser-7.0/src/zope/testbrowser/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `zope.testbrowser-6.0/src/zope/testbrowser/tests/test_wsgi.py` & `zope.testbrowser-7.0/src/zope/testbrowser/tests/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `zope.testbrowser-6.0/src/zope/testbrowser/utils.py` & `zope.testbrowser-7.0/src/zope/testbrowser/utils.py`

 * *Files identical despite different names*

### Comparing `zope.testbrowser-6.0/src/zope/testbrowser/wsgi.py` & `zope.testbrowser-7.0/src/zope/testbrowser/wsgi.py`

 * *Files identical despite different names*

### Comparing `zope.testbrowser-6.0/src/zope.testbrowser.egg-info/PKG-INFO` & `zope.testbrowser-7.0/src/zope.testbrowser.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,70 @@
 Metadata-Version: 2.1
 Name: zope.testbrowser
-Version: 6.0
+Version: 7.0
 Summary: Programmable browser for functional black-box tests
 Home-page: https://github.com/zopefoundation/zope.testbrowser
 Author: Zope Corporation and Contributors
 Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Project-URL: Documentation, https://zopetestbrowser.readthedocs.io/
 Keywords: headless browser functional tests WSGI HTTP HTML form
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Internet :: WWW/HTTP
-Requires-Python: >=3.7
+Requires-Python: >=3.8
+License-File: LICENSE.rst
+Requires-Dist: setuptools
+Requires-Dist: zope.interface
+Requires-Dist: zope.schema
+Requires-Dist: zope.cachedescriptors
+Requires-Dist: pytz
+Requires-Dist: WebTest>=2.0.30
+Requires-Dist: BeautifulSoup4
+Requires-Dist: SoupSieve>=1.9.0
+Requires-Dist: WSGIProxy2
+Requires-Dist: legacy-cgi; python_version > "3.12"
 Provides-Extra: docs
+Requires-Dist: Sphinx; extra == "docs"
+Requires-Dist: sphinx_rtd_theme; extra == "docs"
+Requires-Dist: repoze.sphinx.autointerface; extra == "docs"
+Requires-Dist: zope.app.wsgi; extra == "docs"
 Provides-Extra: test
-Provides-Extra: test_bbb
+Requires-Dist: zope.testing; extra == "test"
+Requires-Dist: mock; extra == "test"
+Requires-Dist: zope.testrunner; extra == "test"
+Provides-Extra: test-bbb
+Requires-Dist: zope.testbrowser[test]; extra == "test-bbb"
 Provides-Extra: wsgi
-License-File: LICENSE.rst
 
 ``zope.testbrowser`` README
 ===========================
 
 .. image:: https://img.shields.io/pypi/v/zope.testbrowser.svg
         :target: https://pypi.org/project/zope.testbrowser/
         :alt: Latest Version
 
+.. image:: https://img.shields.io/pypi/pyversions/zope.testbrowser.svg
+        :target: https://pypi.org/project/zope.testbrowser/
+        :alt: Supported Python versions
+
 .. image:: https://github.com/zopefoundation/zope.testbrowser/actions/workflows/tests.yml/badge.svg
         :target: https://github.com/zopefoundation/zope.testbrowser/actions/workflows/tests.yml
 
-
 .. image:: https://readthedocs.org/projects/zopetestbrowser/badge/?version=latest
         :target: http://zopetestbrowser.readthedocs.org/en/latest/
         :alt: Documentation Status
 
 ``zope.testbrowser`` provides an easy-to-use programmable web browser
 with special focus on testing.  It is used in Zope, but it's not Zope
 specific at all.  For instance, it can be used to test or otherwise
@@ -51,14 +73,22 @@
 Documentation is available at: https://zopetestbrowser.readthedocs.org
 
 
 =======
 CHANGES
 =======
 
+7.0 (2024-05-31)
+----------------
+
+- Add support for Python 3.12 and 3.13 as of 3.13b1.
+
+- Drop support for Python 3.7.
+
+
 6.0 (2023-03-27)
 ----------------
 
 - Drop support for Python 2.7, 3.5, 3.6.
 
 - Drop support for deprecated ``python setup.py test``.
```

### Comparing `zope.testbrowser-6.0/src/zope.testbrowser.egg-info/SOURCES.txt` & `zope.testbrowser-7.0/src/zope.testbrowser.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
+.readthedocs.yaml
 CHANGES.rst
 CONTRIBUTING.md
 COPYRIGHT.rst
 LICENSE.rst
 MANIFEST.in
 README.rst
 buildout.cfg
-rtd.txt
 setup.cfg
 setup.py
 tox.ini
 docs/Makefile
 docs/api.rst
 docs/conf.py
 docs/cookies.rst
 docs/index.rst
 docs/make.bat
 docs/narrative.rst
+docs/requirements.txt
 src/zope/__init__.py
 src/zope.testbrowser.egg-info/PKG-INFO
 src/zope.testbrowser.egg-info/SOURCES.txt
 src/zope.testbrowser.egg-info/dependency_links.txt
 src/zope.testbrowser.egg-info/namespace_packages.txt
 src/zope.testbrowser.egg-info/not-zip-safe
 src/zope.testbrowser.egg-info/requires.txt
```

### Comparing `zope.testbrowser-6.0/tox.ini` & `zope.testbrowser-7.0/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,68 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/pure-python
 [tox]
 minversion = 3.18
 envlist =
+    release-check
     lint
-    py37
     py38
     py39
     py310
     py311
+    py312
+    py313
     pypy3
     docs
     coverage
 
 [testenv]
 usedevelop = true
+package = wheel
+wheel_build_env = .pkg
+pip_pre = py313: true
 deps =
+    setuptools < 69
+    Sphinx
 setenv =
     ZOPE_INTERFACE_STRICT_IRO=1
+    py312: VIRTUALENV_PIP=23.1.2
+    py312: PIP_REQUIRE_VIRTUALENV=0
 commands =
     zope-testrunner --test-path=src {posargs:-vc}
     sphinx-build -b doctest -d {envdir}/.cache/doctrees docs {envdir}/.cache/doctest
 extras =
     test
     docs
+[testenv:release-check]
+description = ensure that the distribution is ready to release
+basepython = python3
+skip_install = true
+deps =
+    twine
+    build
+    check-manifest
+    check-python-versions >= 0.20.0
+    wheel
+commands_pre =
+commands =
+    check-manifest
+    check-python-versions --only setup.py,tox.ini,.github/workflows/tests.yml
+    python -m build --sdist --no-isolation
+    twine check dist/*
 
 [testenv:lint]
 basepython = python3
 skip_install = true
+deps =
+    isort
+    flake8
 commands =
     isort --check-only --diff {toxinidir}/src {toxinidir}/setup.py
     flake8 src setup.py
-    check-manifest
-    check-python-versions
-deps =
-    check-manifest
-    check-python-versions >= 0.19.1
-    wheel
-    flake8
-    isort
 
 [testenv:isort-apply]
 basepython = python3
 skip_install = true
 commands_pre =
 deps =
     isort
@@ -59,29 +79,29 @@
 
 [testenv:coverage]
 basepython = python3
 allowlist_externals =
     mkdir
 deps =
     coverage
-    coverage-python-version
+    Sphinx
 commands =
     mkdir -p {toxinidir}/parts/htmlcov
     coverage run -m zope.testrunner --test-path=src {posargs:-vc}
     coverage run -a -m sphinx -b doctest -d {envdir}/.cache/doctrees docs {envdir}/.cache/doctest
     coverage html --ignore-errors
-    coverage report --ignore-errors --show-missing --fail-under=70
+    coverage report --show-missing --fail-under=70
 
 [coverage:run]
 branch = True
-plugins = coverage_python_version
 source = zope.testbrowser
 
 [coverage:report]
 precision = 2
+ignore_errors = True
 exclude_lines =
     pragma: no cover
     pragma: nocover
     except ImportError:
     raise NotImplementedError
     if __name__ == '__main__':
     self.fail
```

