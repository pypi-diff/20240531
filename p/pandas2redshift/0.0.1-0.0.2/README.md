# Comparing `tmp/pandas2redshift-0.0.1.tar.gz` & `tmp/pandas2redshift-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas2redshift-0.0.1.tar", last modified: Thu May 30 23:28:06 2024, max compression
+gzip compressed data, was "pandas2redshift-0.0.2.tar", last modified: Fri May 31 00:29:49 2024, max compression
```

## Comparing `pandas2redshift-0.0.1.tar` & `pandas2redshift-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jorge     (1000) jorge     (1000)        0 2024-05-30 23:28:06.576927 pandas2redshift-0.0.1/
--rw-r--r--   0 jorge     (1000) jorge     (1000)       17 2024-05-30 23:22:20.000000 pandas2redshift-0.0.1/MANIFEST.in
--rw-r--r--   0 jorge     (1000) jorge     (1000)      210 2024-05-30 23:28:06.576927 pandas2redshift-0.0.1/PKG-INFO
--rw-r--r--   0 jorge     (1000) jorge     (1000)     1831 2024-05-21 18:52:55.000000 pandas2redshift-0.0.1/README.md
-drwxr-xr-x   0 jorge     (1000) jorge     (1000)        0 2024-05-30 23:28:06.576927 pandas2redshift-0.0.1/pandas2redshift/
--rw-r--r--   0 jorge     (1000) jorge     (1000)       30 2024-05-21 18:16:50.000000 pandas2redshift-0.0.1/pandas2redshift/__init__.py
--rw-r--r--   0 jorge     (1000) jorge     (1000)     7997 2024-05-21 18:55:17.000000 pandas2redshift-0.0.1/pandas2redshift/pandas2redshift.py
-drwxr-xr-x   0 jorge     (1000) jorge     (1000)        0 2024-05-30 23:28:06.576927 pandas2redshift-0.0.1/pandas2redshift.egg-info/
--rw-r--r--   0 jorge     (1000) jorge     (1000)      210 2024-05-30 23:28:06.000000 pandas2redshift-0.0.1/pandas2redshift.egg-info/PKG-INFO
--rw-r--r--   0 jorge     (1000) jorge     (1000)      287 2024-05-30 23:28:06.000000 pandas2redshift-0.0.1/pandas2redshift.egg-info/SOURCES.txt
--rw-r--r--   0 jorge     (1000) jorge     (1000)        1 2024-05-30 23:28:06.000000 pandas2redshift-0.0.1/pandas2redshift.egg-info/dependency_links.txt
--rw-r--r--   0 jorge     (1000) jorge     (1000)       49 2024-05-30 23:28:06.000000 pandas2redshift-0.0.1/pandas2redshift.egg-info/requires.txt
--rw-r--r--   0 jorge     (1000) jorge     (1000)       16 2024-05-30 23:28:06.000000 pandas2redshift-0.0.1/pandas2redshift.egg-info/top_level.txt
--rw-r--r--   0 jorge     (1000) jorge     (1000)       38 2024-05-30 23:28:06.576927 pandas2redshift-0.0.1/setup.cfg
--rw-r--r--   0 jorge     (1000) jorge     (1000)      393 2024-05-30 23:26:01.000000 pandas2redshift-0.0.1/setup.py
+drwxr-xr-x   0 jorge     (1000) jorge     (1000)        0 2024-05-31 00:29:49.776933 pandas2redshift-0.0.2/
+-rw-r--r--   0 jorge     (1000) jorge     (1000)       17 2024-05-30 23:22:20.000000 pandas2redshift-0.0.2/MANIFEST.in
+-rw-r--r--   0 jorge     (1000) jorge     (1000)     2541 2024-05-31 00:29:49.776933 pandas2redshift-0.0.2/PKG-INFO
+-rw-r--r--   0 jorge     (1000) jorge     (1000)     1831 2024-05-21 18:52:55.000000 pandas2redshift-0.0.2/README.md
+drwxr-xr-x   0 jorge     (1000) jorge     (1000)        0 2024-05-31 00:29:49.776933 pandas2redshift-0.0.2/pandas2redshift/
+-rw-r--r--   0 jorge     (1000) jorge     (1000)       30 2024-05-21 18:16:50.000000 pandas2redshift-0.0.2/pandas2redshift/__init__.py
+-rw-r--r--   0 jorge     (1000) jorge     (1000)     8015 2024-05-31 00:23:34.000000 pandas2redshift-0.0.2/pandas2redshift/pandas2redshift.py
+drwxr-xr-x   0 jorge     (1000) jorge     (1000)        0 2024-05-31 00:29:49.776933 pandas2redshift-0.0.2/pandas2redshift.egg-info/
+-rw-r--r--   0 jorge     (1000) jorge     (1000)     2541 2024-05-31 00:29:49.000000 pandas2redshift-0.0.2/pandas2redshift.egg-info/PKG-INFO
+-rw-r--r--   0 jorge     (1000) jorge     (1000)      287 2024-05-31 00:29:49.000000 pandas2redshift-0.0.2/pandas2redshift.egg-info/SOURCES.txt
+-rw-r--r--   0 jorge     (1000) jorge     (1000)        1 2024-05-31 00:29:49.000000 pandas2redshift-0.0.2/pandas2redshift.egg-info/dependency_links.txt
+-rw-r--r--   0 jorge     (1000) jorge     (1000)       49 2024-05-31 00:29:49.000000 pandas2redshift-0.0.2/pandas2redshift.egg-info/requires.txt
+-rw-r--r--   0 jorge     (1000) jorge     (1000)       16 2024-05-31 00:29:49.000000 pandas2redshift-0.0.2/pandas2redshift.egg-info/top_level.txt
+-rw-r--r--   0 jorge     (1000) jorge     (1000)       38 2024-05-31 00:29:49.776933 pandas2redshift-0.0.2/setup.cfg
+-rw-r--r--   0 jorge     (1000) jorge     (1000)      568 2024-05-31 00:28:29.000000 pandas2redshift-0.0.2/setup.py
```

### Comparing `pandas2redshift-0.0.1/README.md` & `pandas2redshift-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pandas2redshift-0.0.1/pandas2redshift/pandas2redshift.py` & `pandas2redshift-0.0.2/pandas2redshift/pandas2redshift.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         aws_bucket_root=aws_bucket_root,
     )
 
     BREAK_LINE = "\n" + (4 * " ")
     COPY_QUERY = dedent(
         f"""
             COPY {schema}.{table_name}
-            FROM '{aws_bucket_path}'
+            FROM '{aws_bucket_name}/{aws_bucket_path}'
             {BREAK_LINE.join(query_args)}
             ACCESS_KEY_ID '{aws_access_key}'
             SECRET_ACCESS_KEY '{aws_secret_key}'
         """
     )
 
     conn.execute(COPY_QUERY)
```

