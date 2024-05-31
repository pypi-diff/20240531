# Comparing `tmp/pkginfo-1.9.5.tar.gz` & `tmp/pkginfo-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkginfo-1.9.5.tar", last modified: Fri Jan  6 18:05:13 2023, max compression
+gzip compressed data, was "pkginfo-1.9.6.tar", last modified: Sun Jan  8 16:48:17 2023, max compression
```

## Comparing `pkginfo-1.9.5.tar` & `pkginfo-1.9.6.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-06 18:05:13.856269 pkginfo-1.9.5/
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      122 2023-01-03 15:47:49.000000 pkginfo-1.9.5/.bzrignore
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)       61 2022-05-19 14:58:42.000000 pkginfo-1.9.5/.coveragerc
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     9028 2023-01-06 18:04:11.000000 pkginfo-1.9.5/CHANGES.txt
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     1084 2018-08-20 20:05:50.000000 pkginfo-1.9.5/LICENSE.txt
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)       32 2023-01-05 14:54:28.000000 pkginfo-1.9.5/MANIFEST.in
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)    13643 2023-01-06 18:05:13.856269 pkginfo-1.9.5/PKG-INFO
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      528 2018-08-20 20:05:50.000000 pkginfo-1.9.5/README.txt
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      358 2018-08-20 20:05:50.000000 pkginfo-1.9.5/TODO.txt
-drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-06 18:05:13.852269 pkginfo-1.9.5/docs/
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     2367 2018-08-20 20:05:50.000000 pkginfo-1.9.5/docs/Makefile
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     6095 2021-07-09 13:00:42.000000 pkginfo-1.9.5/docs/conf.py
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     5162 2021-07-09 13:01:28.000000 pkginfo-1.9.5/docs/distributions.rst
-drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-06 18:05:13.852269 pkginfo-1.9.5/docs/examples/
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)   335946 2021-11-18 21:32:58.000000 pkginfo-1.9.5/docs/examples/distlib-0.3.1-py2.py3-none-any.whl
-drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-06 18:05:13.852269 pkginfo-1.9.5/docs/examples/mypackage-0.1/
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      318 2018-08-20 20:05:50.000000 pkginfo-1.9.5/docs/examples/mypackage-0.1/PKG-INFO
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)       74 2018-08-20 20:05:50.000000 pkginfo-1.9.5/docs/examples/mypackage-0.1/README.txt
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)       59 2018-08-20 20:05:50.000000 pkginfo-1.9.5/docs/examples/mypackage-0.1/setup.cfg
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      309 2018-08-20 20:05:50.000000 pkginfo-1.9.5/docs/examples/mypackage-0.1/setup.py
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     1816 2018-08-20 20:05:50.000000 pkginfo-1.9.5/docs/examples/mypackage-0.1-cp26-none-linux_x86_64.whl
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      936 2018-08-20 20:05:50.000000 pkginfo-1.9.5/docs/examples/mypackage-0.1-py2.6.egg
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)        0 2021-11-18 21:12:39.000000 pkginfo-1.9.5/docs/examples/mypackage-0.1.bogus
-drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-06 18:05:13.852269 pkginfo-1.9.5/docs/examples/mypackage-0.1.dist-info/
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      308 2013-11-27 21:40:58.000000 pkginfo-1.9.5/docs/examples/mypackage-0.1.dist-info/METADATA
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)    10240 2018-08-20 20:05:50.000000 pkginfo-1.9.5/docs/examples/mypackage-0.1.tar
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      889 2018-08-20 20:05:50.000000 pkginfo-1.9.5/docs/examples/mypackage-0.1.tar.bz2
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      773 2021-11-18 20:25:24.000000 pkginfo-1.9.5/docs/examples/mypackage-0.1.tar.gz
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     2028 2018-08-20 20:05:50.000000 pkginfo-1.9.5/docs/examples/mypackage-0.1.zip
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      955 2018-08-20 20:05:50.000000 pkginfo-1.9.5/docs/examples/nodistinfo-0.1-any.whl
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      955 2018-08-20 20:05:50.000000 pkginfo-1.9.5/docs/examples/nopkginfo-0.1.egg
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      955 2018-08-20 20:05:50.000000 pkginfo-1.9.5/docs/examples/nopkginfo-0.1.zip
-drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-06 18:05:13.852269 pkginfo-1.9.5/docs/examples/testlp1974172/
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      574 2022-05-19 14:36:03.000000 pkginfo-1.9.5/docs/examples/testlp1974172/setup.py
-drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-06 18:05:13.852269 pkginfo-1.9.5/docs/examples/testlp1974172/testlp1974172.egg-info/
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      549 2022-05-19 14:38:01.000000 pkginfo-1.9.5/docs/examples/testlp1974172/testlp1974172.egg-info/PKG-INFO
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      156 2022-05-19 14:38:01.000000 pkginfo-1.9.5/docs/examples/testlp1974172/testlp1974172.egg-info/SOURCES.txt
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)        1 2022-05-19 14:38:01.000000 pkginfo-1.9.5/docs/examples/testlp1974172/testlp1974172.egg-info/dependency_links.txt
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)        1 2022-05-19 14:38:01.000000 pkginfo-1.9.5/docs/examples/testlp1974172/testlp1974172.egg-info/top_level.txt
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     1268 2022-05-19 14:38:01.000000 pkginfo-1.9.5/docs/examples/testlp1974172-0.0.0-py3-none-any.whl
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      551 2018-08-20 20:05:50.000000 pkginfo-1.9.5/docs/index.rst
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      572 2018-08-20 20:05:50.000000 pkginfo-1.9.5/docs/indexes.rst
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     1234 2021-07-09 13:01:59.000000 pkginfo-1.9.5/docs/metadata.rst
-drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-06 18:05:13.852269 pkginfo-1.9.5/pkginfo/
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      266 2018-08-20 20:05:50.000000 pkginfo-1.9.5/pkginfo/__init__.py
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      357 2023-01-03 15:07:02.000000 pkginfo-1.9.5/pkginfo/__init__.pyi
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     1198 2018-08-20 20:05:50.000000 pkginfo-1.9.5/pkginfo/bdist.py
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      247 2023-01-06 15:49:24.000000 pkginfo-1.9.5/pkginfo/bdist.pyi
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     7415 2023-01-03 15:13:01.000000 pkginfo-1.9.5/pkginfo/commandline.py
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     1088 2023-01-06 15:58:28.000000 pkginfo-1.9.5/pkginfo/commandline.pyi
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     1577 2018-08-20 20:05:50.000000 pkginfo-1.9.5/pkginfo/develop.py
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      241 2023-01-06 15:49:06.000000 pkginfo-1.9.5/pkginfo/develop.pyi
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     4627 2023-01-03 15:30:20.000000 pkginfo-1.9.5/pkginfo/distribution.py
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     1691 2023-01-06 15:22:12.000000 pkginfo-1.9.5/pkginfo/distribution.pyi
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      518 2018-08-20 20:05:50.000000 pkginfo-1.9.5/pkginfo/index.py
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      223 2023-01-06 15:51:54.000000 pkginfo-1.9.5/pkginfo/index.pyi
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     2492 2022-11-29 18:32:36.000000 pkginfo-1.9.5/pkginfo/installed.py
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      323 2023-01-06 15:48:58.000000 pkginfo-1.9.5/pkginfo/installed.pyi
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)        0 2023-01-03 15:57:14.000000 pkginfo-1.9.5/pkginfo/py.typed
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     2347 2021-11-18 20:32:59.000000 pkginfo-1.9.5/pkginfo/sdist.py
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      396 2023-01-06 15:50:24.000000 pkginfo-1.9.5/pkginfo/sdist.pyi
-drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-06 18:05:13.856269 pkginfo-1.9.5/pkginfo/tests/
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     1342 2022-11-29 19:55:27.000000 pkginfo-1.9.5/pkginfo/tests/__init__.py
-drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-06 18:05:13.856269 pkginfo-1.9.5/pkginfo/tests/funny/
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)       68 2018-08-20 20:05:50.000000 pkginfo-1.9.5/pkginfo/tests/funny/__init__.py
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)       47 2018-08-20 20:05:50.000000 pkginfo-1.9.5/pkginfo/tests/funny/funny.egg-info
-drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-06 18:05:13.856269 pkginfo-1.9.5/pkginfo/tests/manky/
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      144 2018-08-20 20:05:50.000000 pkginfo-1.9.5/pkginfo/tests/manky/NOT-A-PACKAGE.txt
-drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-06 18:05:13.856269 pkginfo-1.9.5/pkginfo/tests/manky/namespaced/
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      220 2022-05-19 14:17:38.000000 pkginfo-1.9.5/pkginfo/tests/manky/namespaced/__init__.py
-drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-06 18:05:13.856269 pkginfo-1.9.5/pkginfo/tests/manky/namespaced/manky/
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)       51 2018-08-20 20:05:50.000000 pkginfo-1.9.5/pkginfo/tests/manky/namespaced/manky/__init__.py
-drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-06 18:05:13.856269 pkginfo-1.9.5/pkginfo/tests/manky/namespaced.manky-0.1.egg-info/
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)       45 2018-08-20 20:05:50.000000 pkginfo-1.9.5/pkginfo/tests/manky/namespaced.manky-0.1.egg-info/PKG-INFO
-drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-06 18:05:13.856269 pkginfo-1.9.5/pkginfo/tests/silly/
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)       47 2018-08-20 20:05:50.000000 pkginfo-1.9.5/pkginfo/tests/silly/PKG-INFO
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     2279 2018-08-20 20:05:50.000000 pkginfo-1.9.5/pkginfo/tests/test_bdist.py
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)    11722 2022-11-29 19:05:48.000000 pkginfo-1.9.5/pkginfo/tests/test_commandline.py
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      831 2018-08-20 20:05:50.000000 pkginfo-1.9.5/pkginfo/tests/test_develop.py
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)    19377 2022-11-29 20:01:32.000000 pkginfo-1.9.5/pkginfo/tests/test_distribution.py
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     2636 2018-08-20 20:05:50.000000 pkginfo-1.9.5/pkginfo/tests/test_index.py
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     5460 2022-11-29 19:05:52.000000 pkginfo-1.9.5/pkginfo/tests/test_installed.py
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     5481 2022-05-19 15:42:10.000000 pkginfo-1.9.5/pkginfo/tests/test_sdist.py
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     6835 2018-08-20 20:05:50.000000 pkginfo-1.9.5/pkginfo/tests/test_utils.py
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     4443 2022-05-19 14:47:44.000000 pkginfo-1.9.5/pkginfo/tests/test_wheel.py
-drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-06 18:05:13.856269 pkginfo-1.9.5/pkginfo/tests/wonky/
-drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-06 18:05:13.856269 pkginfo-1.9.5/pkginfo/tests/wonky/EGG-INFO/
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)       45 2018-08-20 20:05:50.000000 pkginfo-1.9.5/pkginfo/tests/wonky/EGG-INFO/PKG-INFO
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      144 2018-08-20 20:05:50.000000 pkginfo-1.9.5/pkginfo/tests/wonky/NOT-A-PACKAGE.txt
-drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-06 18:05:13.856269 pkginfo-1.9.5/pkginfo/tests/wonky/namespaced/
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      220 2022-05-19 14:17:56.000000 pkginfo-1.9.5/pkginfo/tests/wonky/namespaced/__init__.py
-drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-06 18:05:13.856269 pkginfo-1.9.5/pkginfo/tests/wonky/namespaced/wonky/
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)       51 2018-08-20 20:05:50.000000 pkginfo-1.9.5/pkginfo/tests/wonky/namespaced/wonky/__init__.py
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     1786 2018-08-20 20:06:26.000000 pkginfo-1.9.5/pkginfo/utils.py
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      175 2023-01-06 15:53:18.000000 pkginfo-1.9.5/pkginfo/utils.pyi
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     1586 2022-11-29 18:43:47.000000 pkginfo-1.9.5/pkginfo/wheel.py
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      263 2023-01-06 15:48:10.000000 pkginfo-1.9.5/pkginfo/wheel.pyi
-drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-06 18:05:13.852269 pkginfo-1.9.5/pkginfo.egg-info/
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)    13643 2023-01-06 18:05:13.000000 pkginfo-1.9.5/pkginfo.egg-info/PKG-INFO
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     2542 2023-01-06 18:05:13.000000 pkginfo-1.9.5/pkginfo.egg-info/SOURCES.txt
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)        1 2023-01-06 18:05:13.000000 pkginfo-1.9.5/pkginfo.egg-info/dependency_links.txt
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)       54 2023-01-06 18:05:13.000000 pkginfo-1.9.5/pkginfo.egg-info/entry_points.txt
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)        1 2018-08-20 20:06:52.000000 pkginfo-1.9.5/pkginfo.egg-info/not-zip-safe
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)       29 2023-01-06 18:05:13.000000 pkginfo-1.9.5/pkginfo.egg-info/requires.txt
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)        8 2023-01-06 18:05:13.000000 pkginfo-1.9.5/pkginfo.egg-info/top_level.txt
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      532 2023-01-06 18:05:13.856269 pkginfo-1.9.5/setup.cfg
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     1837 2023-01-06 18:04:22.000000 pkginfo-1.9.5/setup.py
--rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      810 2023-01-06 15:46:28.000000 pkginfo-1.9.5/tox.ini
+drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-08 16:48:17.641739 pkginfo-1.9.6/
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      122 2023-01-03 15:47:49.000000 pkginfo-1.9.6/.bzrignore
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)       61 2022-05-19 14:58:42.000000 pkginfo-1.9.6/.coveragerc
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     9126 2023-01-08 16:47:37.000000 pkginfo-1.9.6/CHANGES.txt
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     1084 2018-08-20 20:05:50.000000 pkginfo-1.9.6/LICENSE.txt
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)       32 2023-01-05 14:54:28.000000 pkginfo-1.9.6/MANIFEST.in
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)    13778 2023-01-08 16:48:17.641739 pkginfo-1.9.6/PKG-INFO
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      528 2023-01-08 16:40:33.000000 pkginfo-1.9.6/README.txt
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      358 2018-08-20 20:05:50.000000 pkginfo-1.9.6/TODO.txt
+drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-08 16:48:17.637740 pkginfo-1.9.6/docs/
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     2367 2018-08-20 20:05:50.000000 pkginfo-1.9.6/docs/Makefile
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     6095 2021-07-09 13:00:42.000000 pkginfo-1.9.6/docs/conf.py
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     5164 2023-01-08 16:42:32.000000 pkginfo-1.9.6/docs/distributions.rst
+drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-08 16:48:17.637740 pkginfo-1.9.6/docs/examples/
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)   335946 2021-11-18 21:32:58.000000 pkginfo-1.9.6/docs/examples/distlib-0.3.1-py2.py3-none-any.whl
+drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-08 16:48:17.641739 pkginfo-1.9.6/docs/examples/mypackage-0.1/
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      318 2018-08-20 20:05:50.000000 pkginfo-1.9.6/docs/examples/mypackage-0.1/PKG-INFO
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)       74 2018-08-20 20:05:50.000000 pkginfo-1.9.6/docs/examples/mypackage-0.1/README.txt
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)       59 2018-08-20 20:05:50.000000 pkginfo-1.9.6/docs/examples/mypackage-0.1/setup.cfg
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      309 2018-08-20 20:05:50.000000 pkginfo-1.9.6/docs/examples/mypackage-0.1/setup.py
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     1816 2018-08-20 20:05:50.000000 pkginfo-1.9.6/docs/examples/mypackage-0.1-cp26-none-linux_x86_64.whl
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      936 2018-08-20 20:05:50.000000 pkginfo-1.9.6/docs/examples/mypackage-0.1-py2.6.egg
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)        0 2021-11-18 21:12:39.000000 pkginfo-1.9.6/docs/examples/mypackage-0.1.bogus
+drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-08 16:48:17.641739 pkginfo-1.9.6/docs/examples/mypackage-0.1.dist-info/
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      308 2013-11-27 21:40:58.000000 pkginfo-1.9.6/docs/examples/mypackage-0.1.dist-info/METADATA
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)    10240 2018-08-20 20:05:50.000000 pkginfo-1.9.6/docs/examples/mypackage-0.1.tar
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      889 2018-08-20 20:05:50.000000 pkginfo-1.9.6/docs/examples/mypackage-0.1.tar.bz2
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      773 2021-11-18 20:25:24.000000 pkginfo-1.9.6/docs/examples/mypackage-0.1.tar.gz
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     2028 2018-08-20 20:05:50.000000 pkginfo-1.9.6/docs/examples/mypackage-0.1.zip
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      955 2018-08-20 20:05:50.000000 pkginfo-1.9.6/docs/examples/nodistinfo-0.1-any.whl
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      955 2018-08-20 20:05:50.000000 pkginfo-1.9.6/docs/examples/nopkginfo-0.1.egg
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      955 2018-08-20 20:05:50.000000 pkginfo-1.9.6/docs/examples/nopkginfo-0.1.zip
+drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-08 16:48:17.641739 pkginfo-1.9.6/docs/examples/testlp1974172/
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      575 2023-01-08 16:45:05.000000 pkginfo-1.9.6/docs/examples/testlp1974172/setup.py
+drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-08 16:48:17.641739 pkginfo-1.9.6/docs/examples/testlp1974172/testlp1974172.egg-info/
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      549 2022-05-19 14:38:01.000000 pkginfo-1.9.6/docs/examples/testlp1974172/testlp1974172.egg-info/PKG-INFO
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      156 2022-05-19 14:38:01.000000 pkginfo-1.9.6/docs/examples/testlp1974172/testlp1974172.egg-info/SOURCES.txt
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)        1 2022-05-19 14:38:01.000000 pkginfo-1.9.6/docs/examples/testlp1974172/testlp1974172.egg-info/dependency_links.txt
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)        1 2022-05-19 14:38:01.000000 pkginfo-1.9.6/docs/examples/testlp1974172/testlp1974172.egg-info/top_level.txt
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     1268 2022-05-19 14:38:01.000000 pkginfo-1.9.6/docs/examples/testlp1974172-0.0.0-py3-none-any.whl
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      551 2023-01-08 16:42:48.000000 pkginfo-1.9.6/docs/index.rst
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      572 2018-08-20 20:05:50.000000 pkginfo-1.9.6/docs/indexes.rst
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     1234 2021-07-09 13:01:59.000000 pkginfo-1.9.6/docs/metadata.rst
+drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-08 16:48:17.641739 pkginfo-1.9.6/pkginfo/
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      266 2018-08-20 20:05:50.000000 pkginfo-1.9.6/pkginfo/__init__.py
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      357 2023-01-03 15:07:02.000000 pkginfo-1.9.6/pkginfo/__init__.pyi
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     1198 2018-08-20 20:05:50.000000 pkginfo-1.9.6/pkginfo/bdist.py
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      247 2023-01-06 15:49:24.000000 pkginfo-1.9.6/pkginfo/bdist.pyi
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     7415 2023-01-03 15:13:01.000000 pkginfo-1.9.6/pkginfo/commandline.py
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     1088 2023-01-06 15:58:28.000000 pkginfo-1.9.6/pkginfo/commandline.pyi
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     1577 2018-08-20 20:05:50.000000 pkginfo-1.9.6/pkginfo/develop.py
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      241 2023-01-06 15:49:06.000000 pkginfo-1.9.6/pkginfo/develop.pyi
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     4627 2023-01-03 15:30:20.000000 pkginfo-1.9.6/pkginfo/distribution.py
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     1691 2023-01-06 15:22:12.000000 pkginfo-1.9.6/pkginfo/distribution.pyi
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      518 2018-08-20 20:05:50.000000 pkginfo-1.9.6/pkginfo/index.py
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      223 2023-01-06 15:51:54.000000 pkginfo-1.9.6/pkginfo/index.pyi
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     2492 2022-11-29 18:32:36.000000 pkginfo-1.9.6/pkginfo/installed.py
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      323 2023-01-06 15:48:58.000000 pkginfo-1.9.6/pkginfo/installed.pyi
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)        0 2023-01-03 15:57:14.000000 pkginfo-1.9.6/pkginfo/py.typed
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     2347 2021-11-18 20:32:59.000000 pkginfo-1.9.6/pkginfo/sdist.py
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      396 2023-01-06 15:50:24.000000 pkginfo-1.9.6/pkginfo/sdist.pyi
+drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-08 16:48:17.641739 pkginfo-1.9.6/pkginfo/tests/
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     1342 2022-11-29 19:55:27.000000 pkginfo-1.9.6/pkginfo/tests/__init__.py
+drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-08 16:48:17.641739 pkginfo-1.9.6/pkginfo/tests/funny/
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)       68 2018-08-20 20:05:50.000000 pkginfo-1.9.6/pkginfo/tests/funny/__init__.py
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)       47 2018-08-20 20:05:50.000000 pkginfo-1.9.6/pkginfo/tests/funny/funny.egg-info
+drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-08 16:48:17.641739 pkginfo-1.9.6/pkginfo/tests/manky/
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      144 2018-08-20 20:05:50.000000 pkginfo-1.9.6/pkginfo/tests/manky/NOT-A-PACKAGE.txt
+drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-08 16:48:17.641739 pkginfo-1.9.6/pkginfo/tests/manky/namespaced/
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      220 2022-05-19 14:17:38.000000 pkginfo-1.9.6/pkginfo/tests/manky/namespaced/__init__.py
+drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-08 16:48:17.641739 pkginfo-1.9.6/pkginfo/tests/manky/namespaced/manky/
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)       51 2018-08-20 20:05:50.000000 pkginfo-1.9.6/pkginfo/tests/manky/namespaced/manky/__init__.py
+drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-08 16:48:17.641739 pkginfo-1.9.6/pkginfo/tests/manky/namespaced.manky-0.1.egg-info/
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)       45 2018-08-20 20:05:50.000000 pkginfo-1.9.6/pkginfo/tests/manky/namespaced.manky-0.1.egg-info/PKG-INFO
+drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-08 16:48:17.641739 pkginfo-1.9.6/pkginfo/tests/silly/
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)       47 2018-08-20 20:05:50.000000 pkginfo-1.9.6/pkginfo/tests/silly/PKG-INFO
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     2279 2018-08-20 20:05:50.000000 pkginfo-1.9.6/pkginfo/tests/test_bdist.py
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)    11722 2022-11-29 19:05:48.000000 pkginfo-1.9.6/pkginfo/tests/test_commandline.py
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      831 2018-08-20 20:05:50.000000 pkginfo-1.9.6/pkginfo/tests/test_develop.py
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)    19377 2022-11-29 20:01:32.000000 pkginfo-1.9.6/pkginfo/tests/test_distribution.py
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     2636 2018-08-20 20:05:50.000000 pkginfo-1.9.6/pkginfo/tests/test_index.py
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     5460 2022-11-29 19:05:52.000000 pkginfo-1.9.6/pkginfo/tests/test_installed.py
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     5481 2022-05-19 15:42:10.000000 pkginfo-1.9.6/pkginfo/tests/test_sdist.py
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     6835 2018-08-20 20:05:50.000000 pkginfo-1.9.6/pkginfo/tests/test_utils.py
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     4443 2022-05-19 14:47:44.000000 pkginfo-1.9.6/pkginfo/tests/test_wheel.py
+drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-08 16:48:17.641739 pkginfo-1.9.6/pkginfo/tests/wonky/
+drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-08 16:48:17.641739 pkginfo-1.9.6/pkginfo/tests/wonky/EGG-INFO/
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)       45 2018-08-20 20:05:50.000000 pkginfo-1.9.6/pkginfo/tests/wonky/EGG-INFO/PKG-INFO
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      144 2018-08-20 20:05:50.000000 pkginfo-1.9.6/pkginfo/tests/wonky/NOT-A-PACKAGE.txt
+drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-08 16:48:17.641739 pkginfo-1.9.6/pkginfo/tests/wonky/namespaced/
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      220 2022-05-19 14:17:56.000000 pkginfo-1.9.6/pkginfo/tests/wonky/namespaced/__init__.py
+drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-08 16:48:17.641739 pkginfo-1.9.6/pkginfo/tests/wonky/namespaced/wonky/
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)       51 2018-08-20 20:05:50.000000 pkginfo-1.9.6/pkginfo/tests/wonky/namespaced/wonky/__init__.py
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     1786 2018-08-20 20:06:26.000000 pkginfo-1.9.6/pkginfo/utils.py
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      175 2023-01-06 15:53:18.000000 pkginfo-1.9.6/pkginfo/utils.pyi
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     1586 2022-11-29 18:43:47.000000 pkginfo-1.9.6/pkginfo/wheel.py
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      263 2023-01-06 15:48:10.000000 pkginfo-1.9.6/pkginfo/wheel.pyi
+drwxrwxr-x   0 tseaver   (1000) tseaver   (1000)        0 2023-01-08 16:48:17.641739 pkginfo-1.9.6/pkginfo.egg-info/
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)    13778 2023-01-08 16:48:17.000000 pkginfo-1.9.6/pkginfo.egg-info/PKG-INFO
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     2542 2023-01-08 16:48:17.000000 pkginfo-1.9.6/pkginfo.egg-info/SOURCES.txt
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)        1 2023-01-08 16:48:17.000000 pkginfo-1.9.6/pkginfo.egg-info/dependency_links.txt
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)       54 2023-01-08 16:48:17.000000 pkginfo-1.9.6/pkginfo.egg-info/entry_points.txt
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)        1 2018-08-20 20:06:52.000000 pkginfo-1.9.6/pkginfo.egg-info/not-zip-safe
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)       29 2023-01-08 16:48:17.000000 pkginfo-1.9.6/pkginfo.egg-info/requires.txt
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)        8 2023-01-08 16:48:17.000000 pkginfo-1.9.6/pkginfo.egg-info/top_level.txt
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      532 2023-01-08 16:48:17.641739 pkginfo-1.9.6/setup.cfg
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)     1834 2023-01-08 16:47:26.000000 pkginfo-1.9.6/setup.py
+-rw-rw-r--   0 tseaver   (1000) tseaver   (1000)      810 2023-01-06 15:46:28.000000 pkginfo-1.9.6/tox.ini
```

### Comparing `pkginfo-1.9.5/CHANGES.txt` & `pkginfo-1.9.6/CHANGES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 ``pkginfo`` Changelog
 =====================
 
+1.9.6 (2023-01-08)
+------------------
+
+- Fix various typos in docs / docstrings.  LP #2002232.
+
 1.9.5 (2023-01-06)
 ------------------
 
 - Add stricter typing checks, matching those used in 'twine'.
 
 - Fix typing errors / gaps reported from 'twine' CI failure.  LP #2002104.
 
@@ -18,15 +23,15 @@
 
 - Added stub files for Python typing support;  verify using 'mypy'. LP #1876591.
 
 1.9.2 (2022-11-29)
 ------------------
 
 - Drop "universal" wheel support (should be redundant with
-  'python_requires >= 3.6', but just in case.  LP #1998258.
+  'python_requires >= 3.6', but just in case).  LP #1998258.
 
 1.9.1 (2022-11-29)
 ------------------
 
 - Restore a deprecated alias for the '_must_decode' helper function, moved
   from 'pkginfo._compat.must_decode' to 'pkginfo.distribution._must_decode'
   in 1.90.
@@ -274,15 +279,15 @@
   which module was used for parsing.
 
 - Remove bogus testing dependency on ``zope.testing``.
 
 - Add tests that the "environment markers" spelled out in the approved
   PEP 345 are captured.
 
-- Add ``Project-URL`` for ``1.2`` PKG-INFO metdata (defined in the accepted
+- Add ``Project-URL`` for ``1.2`` PKG-INFO metadata (defined in the accepted
   version of PEP 345).
 
 
 0.5 (2009-09-11)
 ----------------
 
 - Marked package as non-zip-safe.
```

### Comparing `pkginfo-1.9.5/LICENSE.txt` & `pkginfo-1.9.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/PKG-INFO` & `pkginfo-1.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 Metadata-Version: 2.1
 Name: pkginfo
-Version: 1.9.5
-Summary: Query metadatdata from sdists / bdists / installed packages.
+Version: 1.9.6
+Summary: Query metadata from sdists / bdists / installed packages.
 Home-page: https://code.launchpad.net/~tseaver/pkginfo/trunk
 Author: Tres Seaver, Agendaless Consulting
 Author-email: tseaver@agendaless.com
 License: MIT
 Description: ``pkginfo`` README
         ==================
         
         This package provides an API for querying the distutils metadata written in
-        the ``PKG-INFO`` file inside a source distriubtion (an ``sdist``) or a
+        the ``PKG-INFO`` file inside a source distribution (an ``sdist``) or a
         binary distribution (e.g., created by running ``bdist_egg``).  It can
         also query the ``EGG-INFO`` directory of an installed distribution, and
         the ``*.egg-info`` stored in a "development checkout"
         (e.g, created by running ``setup.py develop``).
         
         
         Please see the `pkginfo docs <http://packages.python.org/pkginfo>`_
         for detailed documentation.
         
         
         ``pkginfo`` Changelog
         =====================
         
+        1.9.6 (2023-01-08)
+        ------------------
+        
+        - Fix various typos in docs / docstrings.  LP #2002232.
+        
         1.9.5 (2023-01-06)
         ------------------
         
         - Add stricter typing checks, matching those used in 'twine'.
         
         - Fix typing errors / gaps reported from 'twine' CI failure.  LP #2002104.
         
@@ -41,15 +46,15 @@
         
         - Added stub files for Python typing support;  verify using 'mypy'. LP #1876591.
         
         1.9.2 (2022-11-29)
         ------------------
         
         - Drop "universal" wheel support (should be redundant with
-          'python_requires >= 3.6', but just in case.  LP #1998258.
+          'python_requires >= 3.6', but just in case).  LP #1998258.
         
         1.9.1 (2022-11-29)
         ------------------
         
         - Restore a deprecated alias for the '_must_decode' helper function, moved
           from 'pkginfo._compat.must_decode' to 'pkginfo.distribution._must_decode'
           in 1.90.
@@ -297,15 +302,15 @@
           which module was used for parsing.
         
         - Remove bogus testing dependency on ``zope.testing``.
         
         - Add tests that the "environment markers" spelled out in the approved
           PEP 345 are captured.
         
-        - Add ``Project-URL`` for ``1.2`` PKG-INFO metdata (defined in the accepted
+        - Add ``Project-URL`` for ``1.2`` PKG-INFO metadata (defined in the accepted
           version of PEP 345).
         
         
         0.5 (2009-09-11)
         ----------------
         
         - Marked package as non-zip-safe.
```

### Comparing `pkginfo-1.9.5/README.txt` & `pkginfo-1.9.6/README.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ``pkginfo`` README
 ==================
 
 This package provides an API for querying the distutils metadata written in
-the ``PKG-INFO`` file inside a source distriubtion (an ``sdist``) or a
+the ``PKG-INFO`` file inside a source distribution (an ``sdist``) or a
 binary distribution (e.g., created by running ``bdist_egg``).  It can
 also query the ``EGG-INFO`` directory of an installed distribution, and
 the ``*.egg-info`` stored in a "development checkout"
 (e.g, created by running ``setup.py develop``).
 
 
 Please see the `pkginfo docs <http://packages.python.org/pkginfo>`_
```

### Comparing `pkginfo-1.9.5/docs/Makefile` & `pkginfo-1.9.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/docs/conf.py` & `pkginfo-1.9.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/docs/distributions.rst` & `pkginfo-1.9.6/docs/distributions.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Distribution Types
 ==================
 
 The fundamental abstraction provided by this pacakge is the ``Distribution``
 base class.  Implementations exist for specific cases:  source distributions,
-binary distributions, installed pakcages, and development checkouts.
+binary distributions, installed packages, and development checkouts.
 
 .. doctest::
 
   >>> from pkginfo import Distribution
   >>> from pkginfo import SDist
   >>> assert issubclass(SDist, Distribution)
   >>> from pkginfo import UnpackedSDist
@@ -28,15 +28,15 @@
 archive, which should have been created via the ``sdist`` command from
 distutils:
 
 .. doctest::
 
   >>> mypackage = SDist('docs/examples/mypackage-0.1.tar.gz')
 
-After creation, the ``SDist`` instance will have attributes corrsponding
+After creation, the ``SDist`` instance will have attributes corresponding
 the the fields defined in the PEP corresponding to the metadata version,
 lower-cased and transliterated into valid Python identifiers by mapping
 hyphens to underscores.  E.g.:
 
 .. doctest::
 
   >>> print(mypackage.metadata_version)
@@ -52,15 +52,15 @@
 .. doctest::
 
   >>> print(mypackage.keywords)
   None
 
 Fields which are marked "multiple use" under the PEP map onto sequences;
 their names are pluralized to indicate the sequence.  "Multiple use" fields
-with no occurences in the ``PKG-INFO`` file will map onto an empty sequence:
+with no occurrences in the ``PKG-INFO`` file will map onto an empty sequence:
 
 .. doctest::
 
   >>> print(list(mypackage.supported_platforms))
   []
 
 See `Metadata Versions <metadata.html>`_ for an example with a non-empty,
@@ -78,15 +78,15 @@
   >>> mypackage = UnpackedSDist('docs/examples/mypackage-0.1')
   >>> print(mypackage.name)
   mypackage
   >>> myotherpackage = UnpackedSDist('docs/examples/mypackage-0.1/setup.py')
   >>> print(myotherpackage.name)
   mypackage
 
-``UnpackedSDist`` objects are most useful in conjuction with distutils to
+``UnpackedSDist`` objects are most useful in conjunction with distutils to
 produce sdists that want complex behavior for determining what metadata to use;
 these sdists normally break when installed with ``pip``, because metadata in an
 sdist is regenerated when pip installed. You can achieve this in your
 `setup.py` as follows:
 
 .. code::
 
@@ -143,15 +143,15 @@
   ...    direct = Installed(pkginfo)
 
 After that, they have the same metadata as other ``Distribution`` objects,
 assuming that the package on which they were based has a discoverable
 '.egg-info' file / directory.  To be discoverable, the '.egg-info' must
 either be located inside the package (e.g., created via ``setup.py develop``
 under setuptools), or adjacent to the package (e.g., created via
-``setup.py instlall``).
+``setup.py install``).
 
 
 Introspecting Development Checkouts
 -----------------------------------
 
 ``Develop`` objects are created from a path to a checkout containing
 a ``PKG-iNFO`` file, e.g., created by running ``setup.py develop`` under
```

### Comparing `pkginfo-1.9.5/docs/examples/distlib-0.3.1-py2.py3-none-any.whl` & `pkginfo-1.9.6/docs/examples/distlib-0.3.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/docs/examples/mypackage-0.1-cp26-none-linux_x86_64.whl` & `pkginfo-1.9.6/docs/examples/mypackage-0.1-cp26-none-linux_x86_64.whl`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/docs/examples/mypackage-0.1-py2.6.egg` & `pkginfo-1.9.6/docs/examples/mypackage-0.1-py2.6.egg`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/docs/examples/mypackage-0.1.tar` & `pkginfo-1.9.6/docs/examples/mypackage-0.1.tar`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/docs/examples/mypackage-0.1.tar.bz2` & `pkginfo-1.9.6/docs/examples/mypackage-0.1.tar.bz2`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/docs/examples/mypackage-0.1.tar.gz` & `pkginfo-1.9.6/docs/examples/mypackage-0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/docs/examples/mypackage-0.1.zip` & `pkginfo-1.9.6/docs/examples/mypackage-0.1.zip`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/docs/examples/nodistinfo-0.1-any.whl` & `pkginfo-1.9.6/docs/examples/nodistinfo-0.1-any.whl`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/docs/examples/nopkginfo-0.1.egg` & `pkginfo-1.9.6/docs/examples/nopkginfo-0.1.egg`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/docs/examples/nopkginfo-0.1.zip` & `pkginfo-1.9.6/docs/examples/nopkginfo-0.1.zip`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/docs/examples/testlp1974172/setup.py` & `pkginfo-1.9.6/docs/examples/testlp1974172/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 DESCRIPTION = f"""\
 Package: {NAME}
 ==============================
 
 This distribution exists to allow testing wheels with the description
 in the "body" of the metadata, rather than in a header.
 
-We make it long enough here, and with enough embeded markup, to try to
+We make it long enough here, and with enough embedded markup, to try to
 trigger that feature during wheel build.
 
 See also:
 
 - https://bugs.launchpad.net/pkginfo/+bug/1885458
 - https://peps.python.org/pep-0566/#description
 """
```

### Comparing `pkginfo-1.9.5/docs/examples/testlp1974172/testlp1974172.egg-info/PKG-INFO` & `pkginfo-1.9.6/docs/examples/testlp1974172/testlp1974172.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/docs/examples/testlp1974172-0.0.0-py3-none-any.whl` & `pkginfo-1.9.6/docs/examples/testlp1974172-0.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/docs/index.rst` & `pkginfo-1.9.6/docs/index.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 :mod:`pkginfo` documentation
 ============================
 
 This package provides an API for querying the distutils metadata written in
-the ``PKG-INFO`` file inside a source distriubtion (an ``sdist``) or a
+the ``PKG-INFO`` file inside a source distribution (an ``sdist``) or a
 binary distribution (e.g., created by running ``bdist_egg`` or
 ``bdist_wheel``).  It can also query the ``EGG-INFO`` directory of an
 installed distribution, and the ``*.egg-info`` stored in a "development
 checkout" (e.g, created by running ``setup.py develop``).
 
 Contents:
```

### Comparing `pkginfo-1.9.5/docs/indexes.rst` & `pkginfo-1.9.6/docs/indexes.rst`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/docs/metadata.rst` & `pkginfo-1.9.6/docs/metadata.rst`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/pkginfo/bdist.py` & `pkginfo-1.9.6/pkginfo/bdist.py`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/pkginfo/commandline.py` & `pkginfo-1.9.6/pkginfo/commandline.py`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/pkginfo/commandline.pyi` & `pkginfo-1.9.6/pkginfo/commandline.pyi`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/pkginfo/develop.py` & `pkginfo-1.9.6/pkginfo/develop.py`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/pkginfo/distribution.py` & `pkginfo-1.9.6/pkginfo/distribution.py`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/pkginfo/distribution.pyi` & `pkginfo-1.9.6/pkginfo/distribution.pyi`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/pkginfo/index.py` & `pkginfo-1.9.6/pkginfo/index.py`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/pkginfo/installed.py` & `pkginfo-1.9.6/pkginfo/installed.py`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/pkginfo/sdist.py` & `pkginfo-1.9.6/pkginfo/sdist.py`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/pkginfo/tests/__init__.py` & `pkginfo-1.9.6/pkginfo/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/pkginfo/tests/test_bdist.py` & `pkginfo-1.9.6/pkginfo/tests/test_bdist.py`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/pkginfo/tests/test_commandline.py` & `pkginfo-1.9.6/pkginfo/tests/test_commandline.py`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/pkginfo/tests/test_develop.py` & `pkginfo-1.9.6/pkginfo/tests/test_develop.py`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/pkginfo/tests/test_distribution.py` & `pkginfo-1.9.6/pkginfo/tests/test_distribution.py`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/pkginfo/tests/test_index.py` & `pkginfo-1.9.6/pkginfo/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/pkginfo/tests/test_installed.py` & `pkginfo-1.9.6/pkginfo/tests/test_installed.py`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/pkginfo/tests/test_sdist.py` & `pkginfo-1.9.6/pkginfo/tests/test_sdist.py`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/pkginfo/tests/test_utils.py` & `pkginfo-1.9.6/pkginfo/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/pkginfo/tests/test_wheel.py` & `pkginfo-1.9.6/pkginfo/tests/test_wheel.py`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/pkginfo/utils.py` & `pkginfo-1.9.6/pkginfo/utils.py`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/pkginfo/wheel.py` & `pkginfo-1.9.6/pkginfo/wheel.py`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/pkginfo.egg-info/PKG-INFO` & `pkginfo-1.9.6/pkginfo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 Metadata-Version: 2.1
 Name: pkginfo
-Version: 1.9.5
-Summary: Query metadatdata from sdists / bdists / installed packages.
+Version: 1.9.6
+Summary: Query metadata from sdists / bdists / installed packages.
 Home-page: https://code.launchpad.net/~tseaver/pkginfo/trunk
 Author: Tres Seaver, Agendaless Consulting
 Author-email: tseaver@agendaless.com
 License: MIT
 Description: ``pkginfo`` README
         ==================
         
         This package provides an API for querying the distutils metadata written in
-        the ``PKG-INFO`` file inside a source distriubtion (an ``sdist``) or a
+        the ``PKG-INFO`` file inside a source distribution (an ``sdist``) or a
         binary distribution (e.g., created by running ``bdist_egg``).  It can
         also query the ``EGG-INFO`` directory of an installed distribution, and
         the ``*.egg-info`` stored in a "development checkout"
         (e.g, created by running ``setup.py develop``).
         
         
         Please see the `pkginfo docs <http://packages.python.org/pkginfo>`_
         for detailed documentation.
         
         
         ``pkginfo`` Changelog
         =====================
         
+        1.9.6 (2023-01-08)
+        ------------------
+        
+        - Fix various typos in docs / docstrings.  LP #2002232.
+        
         1.9.5 (2023-01-06)
         ------------------
         
         - Add stricter typing checks, matching those used in 'twine'.
         
         - Fix typing errors / gaps reported from 'twine' CI failure.  LP #2002104.
         
@@ -41,15 +46,15 @@
         
         - Added stub files for Python typing support;  verify using 'mypy'. LP #1876591.
         
         1.9.2 (2022-11-29)
         ------------------
         
         - Drop "universal" wheel support (should be redundant with
-          'python_requires >= 3.6', but just in case.  LP #1998258.
+          'python_requires >= 3.6', but just in case).  LP #1998258.
         
         1.9.1 (2022-11-29)
         ------------------
         
         - Restore a deprecated alias for the '_must_decode' helper function, moved
           from 'pkginfo._compat.must_decode' to 'pkginfo.distribution._must_decode'
           in 1.90.
@@ -297,15 +302,15 @@
           which module was used for parsing.
         
         - Remove bogus testing dependency on ``zope.testing``.
         
         - Add tests that the "environment markers" spelled out in the approved
           PEP 345 are captured.
         
-        - Add ``Project-URL`` for ``1.2`` PKG-INFO metdata (defined in the accepted
+        - Add ``Project-URL`` for ``1.2`` PKG-INFO metadata (defined in the accepted
           version of PEP 345).
         
         
         0.5 (2009-09-11)
         ----------------
         
         - Marked package as non-zip-safe.
```

### Comparing `pkginfo-1.9.5/pkginfo.egg-info/SOURCES.txt` & `pkginfo-1.9.6/pkginfo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/setup.cfg` & `pkginfo-1.9.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `pkginfo-1.9.5/setup.py` & `pkginfo-1.9.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 README = open(os.path.join(here, 'README.txt')).read()
 CHANGES = open(os.path.join(here, 'CHANGES.txt')).read()
 
 setup(
     name='pkginfo',
-    version='1.9.5',
-    description='Query metadatdata from sdists / bdists / installed packages.',
+    version='1.9.6',
+    description='Query metadata from sdists / bdists / installed packages.',
     platforms=['Unix', 'Windows'],
     long_description='\n\n'.join([README, CHANGES]),
     keywords='distribution sdist installed metadata',
     url='https://code.launchpad.net/~tseaver/pkginfo/trunk',
     author='Tres Seaver, Agendaless Consulting',
     author_email='tseaver@agendaless.com',
     license='MIT',
```

### Comparing `pkginfo-1.9.5/tox.ini` & `pkginfo-1.9.6/tox.ini`

 * *Files identical despite different names*

