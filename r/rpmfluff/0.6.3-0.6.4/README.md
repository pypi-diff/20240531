# Comparing `tmp/rpmfluff-0.6.3.tar.gz` & `tmp/rpmfluff-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpmfluff-0.6.3.tar", last modified: Mon Jul 17 07:07:43 2023, max compression
+gzip compressed data, was "rpmfluff-0.6.4.tar", last modified: Fri May 31 09:33:59 2024, max compression
```

## Comparing `rpmfluff-0.6.3.tar` & `rpmfluff-0.6.4.tar`

### file list

```diff
@@ -1,62 +1,26 @@
-drwxr-xr-x   0 jhutar    (1000) jhutar    (1000)        0 2023-07-17 07:07:43.386618 rpmfluff-0.6.3/
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)    17987 2021-01-05 12:37:29.105099 rpmfluff-0.6.3/LICENSE
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)       47 2021-01-05 12:37:29.000000 rpmfluff-0.6.3/MANIFEST.in
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)      614 2023-07-17 07:07:43.385618 rpmfluff-0.6.3/PKG-INFO
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1358 2022-10-19 05:50:02.408222 rpmfluff-0.6.3/README-releng
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     5120 2023-07-17 07:03:42.000000 rpmfluff-0.6.3/README.md
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     6585 2023-07-17 06:59:41.593272 rpmfluff-0.6.3/python-rpmfluff.spec
-drwxr-xr-x   0 jhutar    (1000) jhutar    (1000)        0 2023-07-17 06:56:37.285992 rpmfluff-0.6.3/rpmfluff/
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1647 2021-01-05 12:37:29.106099 rpmfluff-0.6.3/rpmfluff/__init__.py
-drwxr-xr-x   0 jhutar    (1000) jhutar    (1000)        0 2023-07-17 06:57:08.651209 rpmfluff-0.6.3/rpmfluff/__pycache__/
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1225 2022-10-18 19:54:34.604954 rpmfluff-0.6.3/rpmfluff/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1616 2023-07-17 06:57:08.629209 rpmfluff-0.6.3/rpmfluff/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1223 2021-01-05 12:38:12.023582 rpmfluff-0.6.3/rpmfluff/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     6130 2022-10-18 19:54:34.618954 rpmfluff-0.6.3/rpmfluff/__pycache__/check.cpython-310.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)    10140 2023-07-17 06:57:08.636209 rpmfluff-0.6.3/rpmfluff/__pycache__/check.cpython-311.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     6616 2021-01-05 12:40:17.266990 rpmfluff-0.6.3/rpmfluff/__pycache__/check.cpython-39.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1719 2022-10-18 19:54:34.625954 rpmfluff-0.6.3/rpmfluff/__pycache__/make.cpython-310.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2390 2023-07-17 06:57:08.641209 rpmfluff-0.6.3/rpmfluff/__pycache__/make.cpython-311.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1736 2021-01-05 12:40:17.272990 rpmfluff-0.6.3/rpmfluff/__pycache__/make.cpython-39.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)    26585 2022-10-18 19:54:34.631954 rpmfluff-0.6.3/rpmfluff/__pycache__/rpmbuild.cpython-310.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)    47157 2023-07-17 06:57:08.644209 rpmfluff-0.6.3/rpmfluff/__pycache__/rpmbuild.cpython-311.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)    26981 2021-01-05 12:55:19.922105 rpmfluff-0.6.3/rpmfluff/__pycache__/rpmbuild.cpython-39.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)      934 2022-10-18 19:54:34.633954 rpmfluff-0.6.3/rpmfluff/__pycache__/samples.cpython-310.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)      974 2023-07-17 06:57:08.646209 rpmfluff-0.6.3/rpmfluff/__pycache__/samples.cpython-311.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)      932 2021-01-05 12:40:17.277990 rpmfluff-0.6.3/rpmfluff/__pycache__/samples.cpython-39.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2254 2022-10-18 19:54:34.633954 rpmfluff-0.6.3/rpmfluff/__pycache__/sourcefile.cpython-310.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     3748 2023-07-17 06:57:08.646209 rpmfluff-0.6.3/rpmfluff/__pycache__/sourcefile.cpython-311.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2340 2021-01-05 12:40:17.278990 rpmfluff-0.6.3/rpmfluff/__pycache__/sourcefile.cpython-39.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     4018 2022-10-18 19:54:34.634954 rpmfluff-0.6.3/rpmfluff/__pycache__/subpackage.cpython-310.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     5546 2023-07-17 06:57:08.647209 rpmfluff-0.6.3/rpmfluff/__pycache__/subpackage.cpython-311.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     4264 2021-01-05 12:40:17.278990 rpmfluff-0.6.3/rpmfluff/__pycache__/subpackage.cpython-39.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)      981 2022-10-18 19:54:34.634954 rpmfluff-0.6.3/rpmfluff/__pycache__/tarball.cpython-310.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1587 2023-07-17 06:57:08.647209 rpmfluff-0.6.3/rpmfluff/__pycache__/tarball.cpython-311.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)      977 2021-01-05 12:40:17.279990 rpmfluff-0.6.3/rpmfluff/__pycache__/tarball.cpython-39.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)    28331 2022-10-18 19:54:34.639954 rpmfluff-0.6.3/rpmfluff/__pycache__/test.cpython-310.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)    62177 2023-07-17 06:57:08.651209 rpmfluff-0.6.3/rpmfluff/__pycache__/test.cpython-311.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1640 2022-10-18 19:54:34.635954 rpmfluff-0.6.3/rpmfluff/__pycache__/trigger.cpython-310.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2254 2023-07-17 06:57:08.647209 rpmfluff-0.6.3/rpmfluff/__pycache__/trigger.cpython-311.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1636 2021-01-05 12:40:17.279990 rpmfluff-0.6.3/rpmfluff/__pycache__/trigger.cpython-39.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1763 2022-10-18 19:54:34.619954 rpmfluff-0.6.3/rpmfluff/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     3065 2023-07-17 06:57:08.637209 rpmfluff-0.6.3/rpmfluff/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1777 2021-01-05 12:40:17.266990 rpmfluff-0.6.3/rpmfluff/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1350 2022-10-18 19:54:34.640954 rpmfluff-0.6.3/rpmfluff/__pycache__/yumrepobuild.cpython-310.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2221 2023-07-17 06:57:08.651209 rpmfluff-0.6.3/rpmfluff/__pycache__/yumrepobuild.cpython-311.pyc
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     6451 2021-01-05 12:37:29.106099 rpmfluff-0.6.3/rpmfluff/check.py
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2109 2021-01-05 12:37:29.106099 rpmfluff-0.6.3/rpmfluff/make.py
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)    32286 2021-01-05 12:47:10.829641 rpmfluff-0.6.3/rpmfluff/rpmbuild.py
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1532 2021-01-05 12:37:29.107099 rpmfluff-0.6.3/rpmfluff/samples.py
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2367 2021-01-05 12:37:29.107099 rpmfluff-0.6.3/rpmfluff/sourcefile.py
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     3746 2021-01-05 12:37:29.107099 rpmfluff-0.6.3/rpmfluff/subpackage.py
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1443 2021-01-05 12:37:29.107099 rpmfluff-0.6.3/rpmfluff/tarball.py
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)    35573 2023-07-17 06:56:37.285992 rpmfluff-0.6.3/rpmfluff/test.py
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2142 2021-01-05 12:37:29.108099 rpmfluff-0.6.3/rpmfluff/trigger.py
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2496 2021-01-05 12:37:29.108099 rpmfluff-0.6.3/rpmfluff/utils.py
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2035 2021-01-05 12:37:29.108099 rpmfluff-0.6.3/rpmfluff/yumrepobuild.py
-drwxr-xr-x   0 jhutar    (1000) jhutar    (1000)        0 2023-07-17 07:07:43.385618 rpmfluff-0.6.3/rpmfluff.egg-info/
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)      614 2023-07-17 07:07:43.000000 rpmfluff-0.6.3/rpmfluff.egg-info/PKG-INFO
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)      430 2023-07-17 07:07:43.000000 rpmfluff-0.6.3/rpmfluff.egg-info/SOURCES.txt
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)        1 2023-07-17 07:07:43.000000 rpmfluff-0.6.3/rpmfluff.egg-info/dependency_links.txt
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)        9 2023-07-17 07:07:43.000000 rpmfluff-0.6.3/rpmfluff.egg-info/top_level.txt
--rw-r--r--   0 jhutar    (1000) jhutar    (1000)       38 2023-07-17 07:07:43.386618 rpmfluff-0.6.3/setup.cfg
--rwxr-xr-x   0 jhutar    (1000) jhutar    (1000)     1052 2022-10-18 19:55:45.828165 rpmfluff-0.6.3/setup.py
+drwxr-xr-x   0 jhutar    (1000) jhutar    (1000)        0 2024-05-31 09:33:59.527856 rpmfluff-0.6.4/
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)    17987 2021-01-05 12:37:29.000000 rpmfluff-0.6.4/LICENSE
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)       47 2021-01-05 12:37:29.000000 rpmfluff-0.6.4/MANIFEST.in
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)      614 2024-05-31 09:33:59.527856 rpmfluff-0.6.4/PKG-INFO
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     5359 2024-05-31 09:32:02.000000 rpmfluff-0.6.4/README.md
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     6701 2024-05-31 09:28:28.000000 rpmfluff-0.6.4/python-rpmfluff.spec
+drwxr-xr-x   0 jhutar    (1000) jhutar    (1000)        0 2024-05-31 09:33:59.527856 rpmfluff-0.6.4/rpmfluff/
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1647 2021-01-05 12:37:29.000000 rpmfluff-0.6.4/rpmfluff/__init__.py
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     6451 2021-01-05 12:37:29.000000 rpmfluff-0.6.4/rpmfluff/check.py
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2109 2021-01-05 12:37:29.000000 rpmfluff-0.6.4/rpmfluff/make.py
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)    32361 2024-05-31 09:22:43.000000 rpmfluff-0.6.4/rpmfluff/rpmbuild.py
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1532 2021-01-05 12:37:29.000000 rpmfluff-0.6.4/rpmfluff/samples.py
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2367 2021-01-05 12:37:29.000000 rpmfluff-0.6.4/rpmfluff/sourcefile.py
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     3746 2021-01-05 12:37:29.000000 rpmfluff-0.6.4/rpmfluff/subpackage.py
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     1443 2021-01-05 12:37:29.000000 rpmfluff-0.6.4/rpmfluff/tarball.py
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)    35573 2023-07-17 06:56:37.000000 rpmfluff-0.6.4/rpmfluff/test.py
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2142 2021-01-05 12:37:29.000000 rpmfluff-0.6.4/rpmfluff/trigger.py
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2496 2021-01-05 12:37:29.000000 rpmfluff-0.6.4/rpmfluff/utils.py
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)     2035 2021-01-05 12:37:29.000000 rpmfluff-0.6.4/rpmfluff/yumrepobuild.py
+drwxr-xr-x   0 jhutar    (1000) jhutar    (1000)        0 2024-05-31 09:33:59.527856 rpmfluff-0.6.4/rpmfluff.egg-info/
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)      614 2024-05-31 09:33:59.000000 rpmfluff-0.6.4/rpmfluff.egg-info/PKG-INFO
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)      430 2024-05-31 09:33:59.000000 rpmfluff-0.6.4/rpmfluff.egg-info/SOURCES.txt
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)        1 2024-05-31 09:33:59.000000 rpmfluff-0.6.4/rpmfluff.egg-info/dependency_links.txt
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)        9 2024-05-31 09:33:59.000000 rpmfluff-0.6.4/rpmfluff.egg-info/top_level.txt
+-rw-r--r--   0 jhutar    (1000) jhutar    (1000)       38 2024-05-31 09:33:59.527856 rpmfluff-0.6.4/setup.cfg
+-rwxr-xr-x   0 jhutar    (1000) jhutar    (1000)     1052 2022-10-18 19:55:45.000000 rpmfluff-0.6.4/setup.py
```

### Comparing `rpmfluff-0.6.3/LICENSE` & `rpmfluff-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.3/PKG-INFO` & `rpmfluff-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpmfluff
-Version: 0.6.3
+Version: 0.6.4
 Summary: Lightweight way of building RPMs, and sabotaging them
 Home-page: https://pagure.io/rpmfluff
 Author: David Malcolm
 Author-email: dmalcolm@redhat.com
 Maintainer: Jan Hutar
 Maintainer-email: jhutar@redhat.com
 License: GPL-2.0+
```

### Comparing `rpmfluff-0.6.3/README.md` & `rpmfluff-0.6.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 Author: dmalcolm@redhat.com
 
 Homepage: https://pagure.io/rpmfluff
 
 ## News ##
 
+ * 2024-05-31: Explicitly disable debuginfo when not requested, change needed on rawhide by dshea, thank you!
  * 2023-07-17: Remove usage of deprecated rpm.fi by gotmax23 - thanks!
  * 2022-10-18: Change deprecated distutils to setuptools
  * 2020-08-07: Structural changes by msuchy and lots of fixes and improvements by msuchy, dcantrell and tbaeder - thanks!
  * 2019-05-10: Mostly fixes related to rpm changes, thanks ksrot and bcl!
  * 2019-01-31: Fix and new/improved functionality from David Shea (man pages, images, subpackage scriptlets and symlinks properties), thank you!
  * 2018-07-22: BTW we are in pip now, try `pip install rpmfluff`, but fixed small issue with tests for `python3-rpm-4.14.2-0.rc1.1.fc29.2.x86_64` compatibility
  * 2018-02-23: Small fix for Rawhide and executable ELF files - see https://bugzilla.redhat.com/show_bug.cgi?id=1544361
@@ -33,14 +34,15 @@
  * 2008-09-08: Fixed 2 small issues and created 0.2-2 version
  * 2008-09-08: Commited new big bunch of changes by David Malcolm and released version 0.2
  * 2008-07-11: Package renamed to python-rpmfluff, now works on the F9, some more changes
  * 2008-07-08: Initial commit of David Malcolm's code from former Table Cloth project
 
 ## Releases ##
 
+ * [rpmfluff-0.6.4.tar.xz](https://releases.pagure.org/rpmfluff/rpmfluff-0.6.4.tar.xz) (MD5: `b00fac91042bb974dcac876082ef1c97`)
  * [rpmfluff-0.6.3.tar.xz](https://releases.pagure.org/rpmfluff/rpmfluff-0.6.3.tar.xz) (MD5: `f62f0e54f1eae70dd0d9926eed0892cb`)
  * [rpmfluff-0.6.2.tar.xz](https://releases.pagure.org/rpmfluff/rpmfluff-0.6.2.tar.xz) (MD5: `be164a407b3ae8c3239c5b9352b946fc`)
  * [rpmfluff-0.5.5.tar.xz](https://releases.pagure.org/rpmfluff/rpmfluff-0.5.5.tar.xz) (MD5: `03ed0d57ab059aa4a3dd5182ae77473c`)
  * [rpmfluff-0.5.4.tar.xz](https://releases.pagure.org/rpmfluff/rpmfluff-0.5.4.tar.xz) (MD5: `dc15e98f125e1a46e47648ff38f627d3`)
  * [rpmfluff-0.5.3.tar.xz](https://releases.pagure.org/rpmfluff/rpmfluff-0.5.3.tar.xz) (MD5: `ae0a846c239a60b71bbbcf4e2c84be72`)
  * [rpmfluff-0.4.2.tar.bz2](https://fedorahosted.org/releases/r/p/rpmfluff/rpmfluff-0.4.2.tar.bz2) (MD5: `e8f4e9607128a2817262761592eb8080`) - [python-rpmfluff-0.4.2-1.fc22.src.rpm](https://fedorahosted.org/releases/r/p/rpmfluff/python-rpmfluff-0.4.2-1.fc22.src.rpm)
  * [rpmfluff-0.4.1.tar.bz2](https://fedorahosted.org/releases/r/p/rpmfluff/rpmfluff-0.4.1.tar.bz2) (MD5: `752be6d7ece44535392583c18e007a2e`) - [python-rpmfluff-0.4.1-1.fc22.src.rpm](https://fedorahosted.org/releases/r/p/rpmfluff/python-rpmfluff-0.4.1-1.fc22.src.rpm)
```

### Comparing `rpmfluff-0.6.3/python-rpmfluff.spec` & `rpmfluff-0.6.4/python-rpmfluff.spec`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 %global modname rpmfluff
 
 Name:          python-%{modname}
-Version:       0.6.3
+Version:       0.6.4
 Release:       1%{?dist}
 Summary:       Lightweight way of building RPMs, and sabotaging them
 
 License:       GPLv2+
 URL:           https://pagure.io/rpmfluff
 Source0:       https://pagure.io/releases/%{modname}/%{modname}-%{version}.tar.xz
 
@@ -49,14 +49,17 @@
 
 %files -n python3-%{modname}
 %license LICENSE
 %doc README.md
 %{python3_sitelib}/*
 
 %changelog
+* Fri May 31 2024 Jan Hutar <jhutar@redhat.com> - 0.6.4-1
+- dshea: Explicitly disable debuginfo when not requested
+
 * Mon Jul 17 2023 Jan Hutar <jhutar@redhat.com> - 0.6.3-1
 - gotmax23: remove usage of deprecated rpm.fi
 
 * Tue Oct 18 2022 Jan Hutar <jhutar@redhat.com> - 0.6.2-1
 - Change deprecated distutils to setuptools
 
 * Wed Aug 12 2020 Jan Hutar <jhutar@redhat.com> - 0.6.1-1
```

### Comparing `rpmfluff-0.6.3/rpmfluff/__init__.py` & `rpmfluff-0.6.4/rpmfluff/__init__.py`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.3/rpmfluff/check.py` & `rpmfluff-0.6.4/rpmfluff/check.py`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.3/rpmfluff/make.py` & `rpmfluff-0.6.4/rpmfluff/make.py`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.3/rpmfluff/rpmbuild.py` & `rpmfluff-0.6.4/rpmfluff/rpmbuild.py`

 * *Files 0% similar despite different names*

```diff
@@ -431,14 +431,16 @@
 
         specFile.write("%files\n")
         specFile.write(self.basePackage.section_files)
         specFile.write("\n")
 
         if self.makeDebugInfo:
             specFile.write("%debug_package\n")
+        else:
+            specFile.write("%global debug_package %{nil}\n")
 
         for sub in self.subPackages:
             specFile.write("%%files %s\n"%sub.suffix)
             specFile.write(sub.section_files)
             specFile.write("\n")
 
         if self.section_changelog:
```

### Comparing `rpmfluff-0.6.3/rpmfluff/samples.py` & `rpmfluff-0.6.4/rpmfluff/samples.py`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.3/rpmfluff/sourcefile.py` & `rpmfluff-0.6.4/rpmfluff/sourcefile.py`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.3/rpmfluff/subpackage.py` & `rpmfluff-0.6.4/rpmfluff/subpackage.py`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.3/rpmfluff/tarball.py` & `rpmfluff-0.6.4/rpmfluff/tarball.py`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.3/rpmfluff/test.py` & `rpmfluff-0.6.4/rpmfluff/test.py`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.3/rpmfluff/trigger.py` & `rpmfluff-0.6.4/rpmfluff/trigger.py`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.3/rpmfluff/utils.py` & `rpmfluff-0.6.4/rpmfluff/utils.py`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.3/rpmfluff/yumrepobuild.py` & `rpmfluff-0.6.4/rpmfluff/yumrepobuild.py`

 * *Files identical despite different names*

### Comparing `rpmfluff-0.6.3/rpmfluff.egg-info/PKG-INFO` & `rpmfluff-0.6.4/rpmfluff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpmfluff
-Version: 0.6.3
+Version: 0.6.4
 Summary: Lightweight way of building RPMs, and sabotaging them
 Home-page: https://pagure.io/rpmfluff
 Author: David Malcolm
 Author-email: dmalcolm@redhat.com
 Maintainer: Jan Hutar
 Maintainer-email: jhutar@redhat.com
 License: GPL-2.0+
```

### Comparing `rpmfluff-0.6.3/setup.py` & `rpmfluff-0.6.4/setup.py`

 * *Files identical despite different names*

