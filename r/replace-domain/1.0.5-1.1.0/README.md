# Comparing `tmp/replace_domain-1.0.5.tar.gz` & `tmp/replace_domain-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/replace_domain-1.0.5.tar", last modified: Fri Jul 19 14:31:55 2019, max compression
+gzip compressed data, was "replace_domain-1.1.0.tar", last modified: Fri May 31 16:56:47 2024, max compression
```

## Comparing `replace_domain-1.0.5.tar` & `replace_domain-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 Stephen    (501) staff       (20)        0 2019-07-19 14:31:55.000000 replace_domain-1.0.5/
--rw-r--r--   0 Stephen    (501) staff       (20)      273 2019-07-19 14:31:55.000000 replace_domain-1.0.5/PKG-INFO
-drwxr-xr-x   0 Stephen    (501) staff       (20)        0 2019-07-19 14:31:55.000000 replace_domain-1.0.5/replace_domain/
--rw-r--r--   0 Stephen    (501) staff       (20)       88 2019-07-03 19:45:02.000000 replace_domain-1.0.5/replace_domain/__init__.py
--rw-r--r--   0 Stephen    (501) staff       (20)       22 2019-07-19 14:31:34.000000 replace_domain-1.0.5/replace_domain/_version.py
--rw-r--r--   0 Stephen    (501) staff       (20)     1743 2019-07-19 14:31:34.000000 replace_domain-1.0.5/replace_domain/replace_domain.py
-drwxr-xr-x   0 Stephen    (501) staff       (20)        0 2019-07-19 14:31:55.000000 replace_domain-1.0.5/replace_domain.egg-info/
--rw-r--r--   0 Stephen    (501) staff       (20)      273 2019-07-19 14:31:55.000000 replace_domain-1.0.5/replace_domain.egg-info/PKG-INFO
--rw-r--r--   0 Stephen    (501) staff       (20)      325 2019-07-19 14:31:55.000000 replace_domain-1.0.5/replace_domain.egg-info/SOURCES.txt
--rw-r--r--   0 Stephen    (501) staff       (20)        1 2019-07-19 14:31:55.000000 replace_domain-1.0.5/replace_domain.egg-info/dependency_links.txt
--rw-r--r--   0 Stephen    (501) staff       (20)      123 2019-07-19 14:31:55.000000 replace_domain-1.0.5/replace_domain.egg-info/entry_points.txt
--rw-r--r--   0 Stephen    (501) staff       (20)       10 2019-07-19 14:31:55.000000 replace_domain-1.0.5/replace_domain.egg-info/requires.txt
--rw-r--r--   0 Stephen    (501) staff       (20)       15 2019-07-19 14:31:55.000000 replace_domain-1.0.5/replace_domain.egg-info/top_level.txt
--rw-r--r--   0 Stephen    (501) staff       (20)       38 2019-07-19 14:31:55.000000 replace_domain-1.0.5/setup.cfg
--rw-r--r--   0 Stephen    (501) staff       (20)     1212 2019-07-17 14:07:39.000000 replace_domain-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:56:47.427991 replace_domain-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-31 16:56:47.427991 replace_domain-1.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:56:47.423992 replace_domain-1.1.0/replace_domain/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-31 16:56:38.000000 replace_domain-1.1.0/replace_domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 16:56:38.000000 replace_domain-1.1.0/replace_domain/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-31 16:56:38.000000 replace_domain-1.1.0/replace_domain/replace_domain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:56:47.427991 replace_domain-1.1.0/replace_domain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-31 16:56:47.000000 replace_domain-1.1.0/replace_domain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-31 16:56:47.000000 replace_domain-1.1.0/replace_domain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 16:56:47.000000 replace_domain-1.1.0/replace_domain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-31 16:56:47.000000 replace_domain-1.1.0/replace_domain.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-31 16:56:47.000000 replace_domain-1.1.0/replace_domain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-31 16:56:47.000000 replace_domain-1.1.0/replace_domain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 16:56:47.427991 replace_domain-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-31 16:56:38.000000 replace_domain-1.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `replace_domain-1.0.5/replace_domain/replace_domain.py` & `replace_domain-1.1.0/replace_domain/replace_domain.py`

 * *Files identical despite different names*

### Comparing `replace_domain-1.0.5/setup.py` & `replace_domain-1.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,19 +24,18 @@
 setup(
     name='replace_domain',
     version=get_version('replace_domain'),
     packages=find_packages(),
     install_requires=[
         'looptools',
     ],
-    url='https://github.com/mrstephenneal/Dockerizer',
+    url='https://github.com/sfneal/replace_domain',
     entry_points={
         'console_scripts': [
             'replace_domain = replace_domain.replace_domain:main',
-            'replace-domain = replace_domain.replace_domain:main',
         ]
     },
     license='',
     author='Stephen Neal',
     author_email='stephen@stephenneal.net',
     description='Nginx conf file string replacement.'
 )
```

