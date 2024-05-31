# Comparing `tmp/xerenity-0.0.3.tar.gz` & `tmp/xerenity-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xerenity-0.0.3.tar", last modified: Fri May 31 15:38:35 2024, max compression
+gzip compressed data, was "xerenity-0.0.4.tar", last modified: Fri May 31 15:52:32 2024, max compression
```

## Comparing `xerenity-0.0.3.tar` & `xerenity-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:38:35.838785 xerenity-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:38:26.000000 xerenity-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-31 15:38:35.838785 xerenity-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:38:35.838785 xerenity-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-31 15:38:26.000000 xerenity-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:38:35.838785 xerenity-0.0.3/xerenity/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-31 15:38:26.000000 xerenity-0.0.3/xerenity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:38:35.838785 xerenity-0.0.3/xerenity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-31 15:38:35.000000 xerenity-0.0.3/xerenity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-31 15:38:35.000000 xerenity-0.0.3/xerenity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:38:35.000000 xerenity-0.0.3/xerenity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-31 15:38:35.000000 xerenity-0.0.3/xerenity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 15:38:35.000000 xerenity-0.0.3/xerenity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:32.335926 xerenity-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:23.000000 xerenity-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-31 15:52:32.335926 xerenity-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:52:32.335926 xerenity-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-31 15:52:23.000000 xerenity-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:32.331926 xerenity-0.0.4/xerenity/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-31 15:52:23.000000 xerenity-0.0.4/xerenity/Xerenity.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-31 15:52:23.000000 xerenity-0.0.4/xerenity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:32.335926 xerenity-0.0.4/xerenity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-31 15:52:32.000000 xerenity-0.0.4/xerenity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-31 15:52:32.000000 xerenity-0.0.4/xerenity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:52:32.000000 xerenity-0.0.4/xerenity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-31 15:52:32.000000 xerenity-0.0.4/xerenity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 15:52:32.000000 xerenity-0.0.4/xerenity.egg-info/top_level.txt
```

### Comparing `xerenity-0.0.3/setup.py` & `xerenity-0.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 setup(
     name='xerenity',
-    version='0.0.3',
+    version='0.0.4',
     description='Python package for xerenity',
     url='https://xerenity.vercel.app/login',
     author='Andres Velez',
     author_email='svelez@xerenity.co',
     license='BSD 2-clause',
     packages=['xerenity'],
-    install_requires=['supabase>=2.4.4'],
+    install_requires=['supabase>=2.4.4','pandas'],
     classifiers=[
         'Development Status :: 1 - Planning',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: BSD License',
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python :: 3.5',
     ],
```

