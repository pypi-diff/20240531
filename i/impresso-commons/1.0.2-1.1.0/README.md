# Comparing `tmp/impresso_commons-1.0.2.tar.gz` & `tmp/impresso_commons-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impresso_commons-1.0.2.tar", last modified: Mon Mar 18 13:43:38 2024, max compression
+gzip compressed data, was "impresso_commons-1.1.0.tar", last modified: Fri May 31 15:26:40 2024, max compression
```

## Comparing `impresso_commons-1.0.2.tar` & `impresso_commons-1.1.0.tar`

### file list

```diff
@@ -1,83 +1,97 @@
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-03-18 13:43:38.106623 impresso_commons-1.0.2/
--rw-r--r--   0 piconti    (502) staff       (20)    34523 2023-10-11 09:13:16.000000 impresso_commons-1.0.2/LICENSE
--rw-r--r--   0 piconti    (502) staff       (20)    43397 2024-03-18 13:43:38.106336 impresso_commons-1.0.2/PKG-INFO
--rw-r--r--   0 piconti    (502) staff       (20)     2279 2024-03-18 11:12:42.000000 impresso_commons-1.0.2/README.md
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-03-18 13:43:38.088462 impresso_commons-1.0.2/impresso_commons/
--rw-r--r--   0 piconti    (502) staff       (20)       22 2024-03-18 11:14:45.000000 impresso_commons-1.0.2/impresso_commons/__init__.py
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-03-18 13:43:38.089741 impresso_commons-1.0.2/impresso_commons/classes/
--rw-r--r--   0 piconti    (502) staff       (20)       54 2023-10-11 09:13:16.000000 impresso_commons-1.0.2/impresso_commons/classes/__init__.py
--rw-r--r--   0 piconti    (502) staff       (20)     5643 2023-10-11 09:13:16.000000 impresso_commons-1.0.2/impresso_commons/classes/contentitem.py
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-03-18 13:43:38.086913 impresso_commons-1.0.2/impresso_commons/data/
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-03-18 13:43:38.094123 impresso_commons-1.0.2/impresso_commons/data/config/
--rw-r--r--   0 piconti    (502) staff       (20)      151 2023-10-11 09:13:16.000000 impresso_commons-1.0.2/impresso_commons/data/config/GDL.json
--rw-r--r--   0 piconti    (502) staff       (20)      120 2023-10-11 09:13:16.000000 impresso_commons-1.0.2/impresso_commons/data/config/JDG.json
--rw-r--r--   0 piconti    (502) staff       (20)       52 2023-12-07 16:24:08.000000 impresso_commons-1.0.2/impresso_commons/data/config/cluster.json
--rw-r--r--   0 piconti    (502) staff       (20)       30 2023-10-11 09:13:16.000000 impresso_commons-1.0.2/impresso_commons/data/config/conf.json
--rw-r--r--   0 piconti    (502) staff       (20)       30 2024-01-19 08:23:03.000000 impresso_commons-1.0.2/impresso_commons/data/config/conf2.json
--rw-r--r--   0 piconti    (502) staff       (20)     1446 2024-02-29 19:07:05.000000 impresso_commons-1.0.2/impresso_commons/data/config/patch_rebuilt_1.json
--rw-r--r--   0 piconti    (502) staff       (20)     2113 2024-03-05 13:29:05.000000 impresso_commons-1.0.2/impresso_commons/data/config/patch_rebuilt_2.json
--rw-r--r--   0 piconti    (502) staff       (20)      981 2024-03-05 13:59:20.000000 impresso_commons-1.0.2/impresso_commons/data/config/patch_rebuilt_3.json
--rw-r--r--   0 piconti    (502) staff       (20)     2627 2024-03-14 14:10:14.000000 impresso_commons-1.0.2/impresso_commons/data/config/patch_rebuilt_4.json
--rw-r--r--   0 piconti    (502) staff       (20)       77 2024-03-15 10:21:24.000000 impresso_commons-1.0.2/impresso_commons/data/config/patch_rebuilt_5.json
--rw-r--r--   0 piconti    (502) staff       (20)      377 2023-10-11 09:13:16.000000 impresso_commons-1.0.2/impresso_commons/data/config/remaining_nps.json
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-03-18 13:43:38.094283 impresso_commons-1.0.2/impresso_commons/data/xmi/
--rw-r--r--   0 piconti    (502) staff       (20)    78982 2023-10-11 09:13:16.000000 impresso_commons-1.0.2/impresso_commons/data/xmi/typesystem.xml
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-03-18 13:43:38.095760 impresso_commons-1.0.2/impresso_commons/images/
--rw-r--r--   0 piconti    (502) staff       (20)        0 2023-10-11 09:13:16.000000 impresso_commons-1.0.2/impresso_commons/images/__init__.py
--rw-r--r--   0 piconti    (502) staff       (20)     3906 2024-01-19 08:23:03.000000 impresso_commons-1.0.2/impresso_commons/images/img_utils.py
--rwxr-xr-x   0 piconti    (502) staff       (20)    19209 2024-01-19 08:23:03.000000 impresso_commons-1.0.2/impresso_commons/images/olive_boxes.py
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-03-18 13:43:38.096938 impresso_commons-1.0.2/impresso_commons/path/
--rw-r--r--   0 piconti    (502) staff       (20)     1346 2023-10-11 09:13:16.000000 impresso_commons-1.0.2/impresso_commons/path/__init__.py
--rw-r--r--   0 piconti    (502) staff       (20)    15654 2024-03-18 11:12:39.000000 impresso_commons-1.0.2/impresso_commons/path/path_fs.py
--rw-r--r--   0 piconti    (502) staff       (20)    17727 2024-03-18 11:12:39.000000 impresso_commons-1.0.2/impresso_commons/path/path_s3.py
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-03-18 13:43:38.098959 impresso_commons-1.0.2/impresso_commons/schemas/
--rw-r--r--   0 piconti    (502) staff       (20)    34523 2024-02-16 09:56:19.000000 impresso_commons-1.0.2/impresso_commons/schemas/LICENSE
--rw-r--r--   0 piconti    (502) staff       (20)     3200 2024-02-16 16:44:24.000000 impresso_commons-1.0.2/impresso_commons/schemas/Makefile
--rw-r--r--   0 piconti    (502) staff       (20)      156 2024-02-16 16:44:24.000000 impresso_commons-1.0.2/impresso_commons/schemas/Pipfile
--rw-r--r--   0 piconti    (502) staff       (20)     1538 2024-02-16 09:56:19.000000 impresso_commons-1.0.2/impresso_commons/schemas/Pipfile.lock
--rw-r--r--   0 piconti    (502) staff       (20)     2721 2024-02-16 16:44:24.000000 impresso_commons-1.0.2/impresso_commons/schemas/README.md
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-03-18 13:43:38.087541 impresso_commons-1.0.2/impresso_commons/schemas/json/
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-03-18 13:43:38.099192 impresso_commons-1.0.2/impresso_commons/schemas/json/entities/
--rw-r--r--   0 piconti    (502) staff       (20)     5414 2024-02-16 16:44:24.000000 impresso_commons-1.0.2/impresso_commons/schemas/json/entities/entities.schema.json
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-03-18 13:43:38.099597 impresso_commons-1.0.2/impresso_commons/schemas/json/language_identification/
--rw-r--r--   0 piconti    (502) staff       (20)     6296 2024-02-16 09:56:19.000000 impresso_commons-1.0.2/impresso_commons/schemas/json/language_identification/language_identification.schema.json
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-03-18 13:43:38.099852 impresso_commons-1.0.2/impresso_commons/schemas/json/linguistic_annotation/
--rw-r--r--   0 piconti    (502) staff       (20)     4645 2024-02-16 09:56:19.000000 impresso_commons-1.0.2/impresso_commons/schemas/json/linguistic_annotation/ling_spacy.schema.json
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-03-18 13:43:38.100608 impresso_commons-1.0.2/impresso_commons/schemas/json/newspaper/
--rw-r--r--   0 piconti    (502) staff       (20)     3663 2024-03-01 16:30:58.000000 impresso_commons-1.0.2/impresso_commons/schemas/json/newspaper/contentitem.schema.json
--rw-r--r--   0 piconti    (502) staff       (20)     5407 2024-03-01 16:30:58.000000 impresso_commons-1.0.2/impresso_commons/schemas/json/newspaper/issue.schema.json
--rw-r--r--   0 piconti    (502) staff       (20)     6742 2024-03-01 16:30:58.000000 impresso_commons-1.0.2/impresso_commons/schemas/json/newspaper/page.schema.json
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-03-18 13:43:38.101110 impresso_commons-1.0.2/impresso_commons/schemas/json/topic_model/
--rw-r--r--   0 piconti    (502) staff       (20)     1587 2023-10-11 09:13:17.000000 impresso_commons-1.0.2/impresso_commons/schemas/json/topic_model/topic_assignment.schema.json
--rw-r--r--   0 piconti    (502) staff       (20)     1390 2023-10-11 09:13:17.000000 impresso_commons-1.0.2/impresso_commons/schemas/json/topic_model/topic_description.schema.json
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-03-18 13:43:38.101334 impresso_commons-1.0.2/impresso_commons/schemas/json/versioning/
--rw-r--r--   0 piconti    (502) staff       (20)    10424 2024-02-16 17:23:29.000000 impresso_commons-1.0.2/impresso_commons/schemas/json/versioning/manifest.schema.json
--rw-r--r--   0 piconti    (502) staff       (20)      106 2024-02-16 16:44:24.000000 impresso_commons-1.0.2/impresso_commons/schemas/requirements.txt
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-03-18 13:43:38.101991 impresso_commons-1.0.2/impresso_commons/text/
--rw-r--r--   0 piconti    (502) staff       (20)        0 2023-11-24 12:18:49.000000 impresso_commons-1.0.2/impresso_commons/text/__init__.py
--rw-r--r--   0 piconti    (502) staff       (20)    11280 2024-03-18 11:12:39.000000 impresso_commons-1.0.2/impresso_commons/text/helpers.py
--rw-r--r--   0 piconti    (502) staff       (20)    24850 2024-03-18 11:12:39.000000 impresso_commons-1.0.2/impresso_commons/text/rebuilder.py
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-03-18 13:43:38.103984 impresso_commons-1.0.2/impresso_commons/utils/
--rw-r--r--   0 piconti    (502) staff       (20)     3764 2023-10-11 09:13:16.000000 impresso_commons-1.0.2/impresso_commons/utils/__init__.py
--rw-r--r--   0 piconti    (502) staff       (20)     1646 2023-10-11 09:13:16.000000 impresso_commons-1.0.2/impresso_commons/utils/config_loader.py
--rw-r--r--   0 piconti    (502) staff       (20)     4589 2024-01-19 08:23:03.000000 impresso_commons-1.0.2/impresso_commons/utils/daskutils.py
--rw-r--r--   0 piconti    (502) staff       (20)    16104 2024-03-18 11:12:42.000000 impresso_commons-1.0.2/impresso_commons/utils/s3.py
--rw-r--r--   0 piconti    (502) staff       (20)     2812 2024-01-19 08:23:03.000000 impresso_commons-1.0.2/impresso_commons/utils/s3_delete.py
--rw-r--r--   0 piconti    (502) staff       (20)     4860 2024-01-19 08:23:03.000000 impresso_commons-1.0.2/impresso_commons/utils/uima.py
--rw-r--r--   0 piconti    (502) staff       (20)     1370 2024-03-18 11:12:39.000000 impresso_commons-1.0.2/impresso_commons/utils/utils.py
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-03-18 13:43:38.104692 impresso_commons-1.0.2/impresso_commons/versioning/
--rw-r--r--   0 piconti    (502) staff       (20)     7778 2024-02-28 18:28:22.000000 impresso_commons-1.0.2/impresso_commons/versioning/manifest_0.py
--rw-r--r--   0 piconti    (502) staff       (20)     5718 2024-02-28 18:33:33.000000 impresso_commons-1.0.2/impresso_commons/versioning/rebuilt_manifest_0.py
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-03-18 13:43:38.105956 impresso_commons-1.0.2/impresso_commons.egg-info/
--rw-r--r--   0 piconti    (502) staff       (20)    43397 2024-03-18 13:43:38.000000 impresso_commons-1.0.2/impresso_commons.egg-info/PKG-INFO
--rw-r--r--   0 piconti    (502) staff       (20)     2440 2024-03-18 13:43:38.000000 impresso_commons-1.0.2/impresso_commons.egg-info/SOURCES.txt
--rw-r--r--   0 piconti    (502) staff       (20)        1 2024-03-18 13:43:38.000000 impresso_commons-1.0.2/impresso_commons.egg-info/dependency_links.txt
--rw-r--r--   0 piconti    (502) staff       (20)      137 2024-03-18 13:43:38.000000 impresso_commons-1.0.2/impresso_commons.egg-info/entry_points.txt
--rw-r--r--   0 piconti    (502) staff       (20)      146 2024-03-18 13:43:38.000000 impresso_commons-1.0.2/impresso_commons.egg-info/requires.txt
--rw-r--r--   0 piconti    (502) staff       (20)       17 2024-03-18 13:43:38.000000 impresso_commons-1.0.2/impresso_commons.egg-info/top_level.txt
--rw-r--r--   0 piconti    (502) staff       (20)     1778 2024-03-18 13:34:24.000000 impresso_commons-1.0.2/pyproject.toml
--rw-r--r--   0 piconti    (502) staff       (20)       38 2024-03-18 13:43:38.106669 impresso_commons-1.0.2/setup.cfg
--rw-r--r--   0 piconti    (502) staff       (20)       36 2023-11-24 08:20:50.000000 impresso_commons-1.0.2/setup.py
-drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-03-18 13:43:38.105415 impresso_commons-1.0.2/tests/
--rw-r--r--   0 piconti    (502) staff       (20)     1756 2024-01-19 08:23:03.000000 impresso_commons-1.0.2/tests/test_path_s3.py
--rw-r--r--   0 piconti    (502) staff       (20)     3145 2023-11-24 08:20:50.000000 impresso_commons-1.0.2/tests/test_rebuilder.py
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-31 15:26:40.135007 impresso_commons-1.1.0/
+-rw-r--r--   0 piconti    (502) staff       (20)    34523 2023-10-11 09:13:16.000000 impresso_commons-1.1.0/LICENSE
+-rw-r--r--   0 piconti    (502) staff       (20)    63907 2024-05-31 15:26:40.134476 impresso_commons-1.1.0/PKG-INFO
+-rw-r--r--   0 piconti    (502) staff       (20)    16024 2024-05-31 15:16:17.000000 impresso_commons-1.1.0/README.md
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-31 15:26:40.108040 impresso_commons-1.1.0/impresso_commons/
+-rw-r--r--   0 piconti    (502) staff       (20)       22 2024-05-30 14:52:49.000000 impresso_commons-1.1.0/impresso_commons/__init__.py
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-31 15:26:40.109715 impresso_commons-1.1.0/impresso_commons/classes/
+-rw-r--r--   0 piconti    (502) staff       (20)       54 2023-10-11 09:13:16.000000 impresso_commons-1.1.0/impresso_commons/classes/__init__.py
+-rw-r--r--   0 piconti    (502) staff       (20)     5643 2023-10-11 09:13:16.000000 impresso_commons-1.1.0/impresso_commons/classes/contentitem.py
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-31 15:26:40.106174 impresso_commons-1.1.0/impresso_commons/data/
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-31 15:26:40.116137 impresso_commons-1.1.0/impresso_commons/data/config/
+-rw-r--r--   0 piconti    (502) staff       (20)      151 2023-10-11 09:13:16.000000 impresso_commons-1.1.0/impresso_commons/data/config/GDL.json
+-rw-r--r--   0 piconti    (502) staff       (20)      120 2023-10-11 09:13:16.000000 impresso_commons-1.1.0/impresso_commons/data/config/JDG.json
+-rw-r--r--   0 piconti    (502) staff       (20)       52 2023-12-07 16:24:08.000000 impresso_commons-1.1.0/impresso_commons/data/config/cluster.json
+-rw-r--r--   0 piconti    (502) staff       (20)       30 2023-10-11 09:13:16.000000 impresso_commons-1.1.0/impresso_commons/data/config/conf.json
+-rw-r--r--   0 piconti    (502) staff       (20)       30 2024-01-19 08:23:03.000000 impresso_commons-1.1.0/impresso_commons/data/config/conf2.json
+-rw-r--r--   0 piconti    (502) staff       (20)     1446 2024-02-29 19:07:05.000000 impresso_commons-1.1.0/impresso_commons/data/config/patch_rebuilt_1.json
+-rw-r--r--   0 piconti    (502) staff       (20)     2113 2024-03-05 13:29:05.000000 impresso_commons-1.1.0/impresso_commons/data/config/patch_rebuilt_2.json
+-rw-r--r--   0 piconti    (502) staff       (20)      981 2024-03-05 13:59:20.000000 impresso_commons-1.1.0/impresso_commons/data/config/patch_rebuilt_3.json
+-rw-r--r--   0 piconti    (502) staff       (20)     2627 2024-03-14 14:10:14.000000 impresso_commons-1.1.0/impresso_commons/data/config/patch_rebuilt_4.json
+-rw-r--r--   0 piconti    (502) staff       (20)       77 2024-03-15 10:21:24.000000 impresso_commons-1.1.0/impresso_commons/data/config/patch_rebuilt_5.json
+-rw-r--r--   0 piconti    (502) staff       (20)     3667 2024-03-25 10:57:27.000000 impresso_commons-1.1.0/impresso_commons/data/config/patch_rebuilt_6.json
+-rw-r--r--   0 piconti    (502) staff       (20)     3292 2024-03-26 16:28:39.000000 impresso_commons-1.1.0/impresso_commons/data/config/patch_rebuilt_7.json
+-rw-r--r--   0 piconti    (502) staff       (20)      959 2024-04-02 15:41:32.000000 impresso_commons-1.1.0/impresso_commons/data/config/patch_rebuilt_8.json
+-rw-r--r--   0 piconti    (502) staff       (20)      377 2024-04-03 11:01:55.000000 impresso_commons-1.1.0/impresso_commons/data/config/patch_rebuilt_9.json
+-rw-r--r--   0 piconti    (502) staff       (20)     9847 2024-03-28 16:14:37.000000 impresso_commons-1.1.0/impresso_commons/data/config/rebuilt_passim.json
+-rw-r--r--   0 piconti    (502) staff       (20)     3512 2024-04-02 09:00:42.000000 impresso_commons-1.1.0/impresso_commons/data/config/rebuilt_passim_1.json
+-rw-r--r--   0 piconti    (502) staff       (20)     1186 2024-04-03 10:53:12.000000 impresso_commons-1.1.0/impresso_commons/data/config/rebuilt_passim_2.json
+-rw-r--r--   0 piconti    (502) staff       (20)      377 2024-04-04 10:15:52.000000 impresso_commons-1.1.0/impresso_commons/data/config/rebuilt_passim_3.json
+-rw-r--r--   0 piconti    (502) staff       (20)      377 2023-10-11 09:13:16.000000 impresso_commons-1.1.0/impresso_commons/data/config/remaining_nps.json
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-31 15:26:40.116298 impresso_commons-1.1.0/impresso_commons/data/xmi/
+-rw-r--r--   0 piconti    (502) staff       (20)    78982 2023-10-11 09:13:16.000000 impresso_commons-1.1.0/impresso_commons/data/xmi/typesystem.xml
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-31 15:26:40.117299 impresso_commons-1.1.0/impresso_commons/images/
+-rw-r--r--   0 piconti    (502) staff       (20)        0 2023-10-11 09:13:16.000000 impresso_commons-1.1.0/impresso_commons/images/__init__.py
+-rw-r--r--   0 piconti    (502) staff       (20)     3906 2024-01-19 08:23:03.000000 impresso_commons-1.1.0/impresso_commons/images/img_utils.py
+-rwxr-xr-x   0 piconti    (502) staff       (20)    19209 2024-01-19 08:23:03.000000 impresso_commons-1.1.0/impresso_commons/images/olive_boxes.py
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-31 15:26:40.118337 impresso_commons-1.1.0/impresso_commons/path/
+-rw-r--r--   0 piconti    (502) staff       (20)     1346 2023-10-11 09:13:16.000000 impresso_commons-1.1.0/impresso_commons/path/__init__.py
+-rw-r--r--   0 piconti    (502) staff       (20)    15548 2024-05-31 10:02:52.000000 impresso_commons-1.1.0/impresso_commons/path/path_fs.py
+-rw-r--r--   0 piconti    (502) staff       (20)    17738 2024-05-31 10:02:40.000000 impresso_commons-1.1.0/impresso_commons/path/path_s3.py
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-31 15:26:40.120276 impresso_commons-1.1.0/impresso_commons/schemas/
+-rw-r--r--   0 piconti    (502) staff       (20)    34523 2024-02-16 09:56:19.000000 impresso_commons-1.1.0/impresso_commons/schemas/LICENSE
+-rw-r--r--   0 piconti    (502) staff       (20)     3200 2024-02-16 16:44:24.000000 impresso_commons-1.1.0/impresso_commons/schemas/Makefile
+-rw-r--r--   0 piconti    (502) staff       (20)      156 2024-02-16 16:44:24.000000 impresso_commons-1.1.0/impresso_commons/schemas/Pipfile
+-rw-r--r--   0 piconti    (502) staff       (20)     1538 2024-02-16 09:56:19.000000 impresso_commons-1.1.0/impresso_commons/schemas/Pipfile.lock
+-rw-r--r--   0 piconti    (502) staff       (20)     2721 2024-02-16 16:44:24.000000 impresso_commons-1.1.0/impresso_commons/schemas/README.md
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-31 15:26:40.106903 impresso_commons-1.1.0/impresso_commons/schemas/json/
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-31 15:26:40.120532 impresso_commons-1.1.0/impresso_commons/schemas/json/entities/
+-rw-r--r--   0 piconti    (502) staff       (20)     5414 2024-02-16 16:44:24.000000 impresso_commons-1.1.0/impresso_commons/schemas/json/entities/entities.schema.json
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-31 15:26:40.120813 impresso_commons-1.1.0/impresso_commons/schemas/json/language_identification/
+-rw-r--r--   0 piconti    (502) staff       (20)     6296 2024-02-16 09:56:19.000000 impresso_commons-1.1.0/impresso_commons/schemas/json/language_identification/language_identification.schema.json
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-31 15:26:40.121096 impresso_commons-1.1.0/impresso_commons/schemas/json/linguistic_annotation/
+-rw-r--r--   0 piconti    (502) staff       (20)     4645 2024-02-16 09:56:19.000000 impresso_commons-1.1.0/impresso_commons/schemas/json/linguistic_annotation/ling_spacy.schema.json
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-31 15:26:40.122058 impresso_commons-1.1.0/impresso_commons/schemas/json/newspaper/
+-rw-r--r--   0 piconti    (502) staff       (20)     3663 2024-03-01 16:30:58.000000 impresso_commons-1.1.0/impresso_commons/schemas/json/newspaper/contentitem.schema.json
+-rw-r--r--   0 piconti    (502) staff       (20)     5407 2024-03-01 16:30:58.000000 impresso_commons-1.1.0/impresso_commons/schemas/json/newspaper/issue.schema.json
+-rw-r--r--   0 piconti    (502) staff       (20)     6742 2024-03-01 16:30:58.000000 impresso_commons-1.1.0/impresso_commons/schemas/json/newspaper/page.schema.json
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-31 15:26:40.122558 impresso_commons-1.1.0/impresso_commons/schemas/json/topic_model/
+-rw-r--r--   0 piconti    (502) staff       (20)     1587 2023-10-11 09:13:17.000000 impresso_commons-1.1.0/impresso_commons/schemas/json/topic_model/topic_assignment.schema.json
+-rw-r--r--   0 piconti    (502) staff       (20)     1390 2023-10-11 09:13:17.000000 impresso_commons-1.1.0/impresso_commons/schemas/json/topic_model/topic_description.schema.json
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-31 15:26:40.122792 impresso_commons-1.1.0/impresso_commons/schemas/json/versioning/
+-rw-r--r--   0 piconti    (502) staff       (20)    10667 2024-04-03 15:35:51.000000 impresso_commons-1.1.0/impresso_commons/schemas/json/versioning/manifest.schema.json
+-rw-r--r--   0 piconti    (502) staff       (20)      106 2024-02-16 16:44:24.000000 impresso_commons-1.1.0/impresso_commons/schemas/requirements.txt
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-31 15:26:40.123528 impresso_commons-1.1.0/impresso_commons/text/
+-rw-r--r--   0 piconti    (502) staff       (20)        0 2023-11-24 12:18:49.000000 impresso_commons-1.1.0/impresso_commons/text/__init__.py
+-rw-r--r--   0 piconti    (502) staff       (20)    11530 2024-05-31 10:03:34.000000 impresso_commons-1.1.0/impresso_commons/text/helpers.py
+-rw-r--r--   0 piconti    (502) staff       (20)    27007 2024-05-31 09:54:50.000000 impresso_commons-1.1.0/impresso_commons/text/rebuilder.py
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-31 15:26:40.125535 impresso_commons-1.1.0/impresso_commons/utils/
+-rw-r--r--   0 piconti    (502) staff       (20)     3764 2023-10-11 09:13:16.000000 impresso_commons-1.1.0/impresso_commons/utils/__init__.py
+-rw-r--r--   0 piconti    (502) staff       (20)     1646 2023-10-11 09:13:16.000000 impresso_commons-1.1.0/impresso_commons/utils/config_loader.py
+-rw-r--r--   0 piconti    (502) staff       (20)     4372 2024-05-31 10:03:54.000000 impresso_commons-1.1.0/impresso_commons/utils/daskutils.py
+-rw-r--r--   0 piconti    (502) staff       (20)    17179 2024-05-31 10:04:23.000000 impresso_commons-1.1.0/impresso_commons/utils/s3.py
+-rw-r--r--   0 piconti    (502) staff       (20)     2812 2024-01-19 08:23:03.000000 impresso_commons-1.1.0/impresso_commons/utils/s3_delete.py
+-rw-r--r--   0 piconti    (502) staff       (20)     4870 2024-05-31 10:04:33.000000 impresso_commons-1.1.0/impresso_commons/utils/uima.py
+-rw-r--r--   0 piconti    (502) staff       (20)     4068 2024-05-31 10:05:08.000000 impresso_commons-1.1.0/impresso_commons/utils/utils.py
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-31 15:26:40.128178 impresso_commons-1.1.0/impresso_commons/versioning/
+-rw-r--r--   0 piconti    (502) staff       (20)        0 2024-05-30 14:52:49.000000 impresso_commons-1.1.0/impresso_commons/versioning/__init__.py
+-rw-r--r--   0 piconti    (502) staff       (20)    12496 2024-05-31 09:53:35.000000 impresso_commons-1.1.0/impresso_commons/versioning/compute_manifest.py
+-rw-r--r--   0 piconti    (502) staff       (20)    46825 2024-05-31 09:56:23.000000 impresso_commons-1.1.0/impresso_commons/versioning/data_manifest.py
+-rw-r--r--   0 piconti    (502) staff       (20)    14043 2024-05-31 09:51:32.000000 impresso_commons-1.1.0/impresso_commons/versioning/data_statistics.py
+-rw-r--r--   0 piconti    (502) staff       (20)    45737 2024-05-31 09:55:56.000000 impresso_commons-1.1.0/impresso_commons/versioning/helpers.py
+-rw-r--r--   0 piconti    (502) staff       (20)     7778 2024-02-28 18:28:22.000000 impresso_commons-1.1.0/impresso_commons/versioning/manifest_0.py
+-rw-r--r--   0 piconti    (502) staff       (20)     5718 2024-02-28 18:33:33.000000 impresso_commons-1.1.0/impresso_commons/versioning/rebuilt_manifest_0.py
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-31 15:26:40.129457 impresso_commons-1.1.0/impresso_commons.egg-info/
+-rw-r--r--   0 piconti    (502) staff       (20)    63907 2024-05-31 15:26:40.000000 impresso_commons-1.1.0/impresso_commons.egg-info/PKG-INFO
+-rw-r--r--   0 piconti    (502) staff       (20)     3078 2024-05-31 15:26:40.000000 impresso_commons-1.1.0/impresso_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 piconti    (502) staff       (20)        1 2024-05-31 15:26:40.000000 impresso_commons-1.1.0/impresso_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 piconti    (502) staff       (20)      137 2024-05-31 15:26:40.000000 impresso_commons-1.1.0/impresso_commons.egg-info/entry_points.txt
+-rw-r--r--   0 piconti    (502) staff       (20)     3896 2024-05-31 15:26:40.000000 impresso_commons-1.1.0/impresso_commons.egg-info/requires.txt
+-rw-r--r--   0 piconti    (502) staff       (20)       17 2024-05-31 15:26:40.000000 impresso_commons-1.1.0/impresso_commons.egg-info/top_level.txt
+-rw-r--r--   0 piconti    (502) staff       (20)     1578 2024-05-30 14:52:49.000000 impresso_commons-1.1.0/pyproject.toml
+-rw-r--r--   0 piconti    (502) staff       (20)     3902 2024-05-30 14:52:49.000000 impresso_commons-1.1.0/requirements.txt
+-rw-r--r--   0 piconti    (502) staff       (20)       38 2024-05-31 15:26:40.135049 impresso_commons-1.1.0/setup.cfg
+-rw-r--r--   0 piconti    (502) staff       (20)       36 2023-11-24 08:20:50.000000 impresso_commons-1.1.0/setup.py
+drwxr-xr-x   0 piconti    (502) staff       (20)        0 2024-05-31 15:26:40.129043 impresso_commons-1.1.0/tests/
+-rw-r--r--   0 piconti    (502) staff       (20)     1756 2024-01-19 08:23:03.000000 impresso_commons-1.1.0/tests/test_path_s3.py
+-rw-r--r--   0 piconti    (502) staff       (20)     3145 2023-11-24 08:20:50.000000 impresso_commons-1.1.0/tests/test_rebuilder.py
```

### Comparing `impresso_commons-1.0.2/LICENSE` & `impresso_commons-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `impresso_commons-1.0.2/PKG-INFO` & `impresso_commons-1.1.0/impresso_commons/schemas/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,728 +1,661 @@
-Metadata-Version: 2.1
-Name: impresso_commons
-Version: 1.0.2
-Summary: Python module highly reusable within impresso.
-Author-email: Maud Ehrmann <maud.ehrmann@epfl.ch>, Matteo Romanello <matteo.romanello@gmail.com>
-License:                     GNU AFFERO GENERAL PUBLIC LICENSE
-                               Version 3, 19 November 2007
-        
-         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
-         Everyone is permitted to copy and distribute verbatim copies
-         of this license document, but changing it is not allowed.
-        
-                                    Preamble
-        
-          The GNU Affero General Public License is a free, copyleft license for
-        software and other kinds of works, specifically designed to ensure
-        cooperation with the community in the case of network server software.
-        
-          The licenses for most software and other practical works are designed
-        to take away your freedom to share and change the works.  By contrast,
-        our General Public Licenses are intended to guarantee your freedom to
-        share and change all versions of a program--to make sure it remains free
-        software for all its users.
-        
-          When we speak of free software, we are referring to freedom, not
-        price.  Our General Public Licenses are designed to make sure that you
-        have the freedom to distribute copies of free software (and charge for
-        them if you wish), that you receive source code or can get it if you
-        want it, that you can change the software or use pieces of it in new
-        free programs, and that you know you can do these things.
-        
-          Developers that use our General Public Licenses protect your rights
-        with two steps: (1) assert copyright on the software, and (2) offer
-        you this License which gives you legal permission to copy, distribute
-        and/or modify the software.
-        
-          A secondary benefit of defending all users' freedom is that
-        improvements made in alternate versions of the program, if they
-        receive widespread use, become available for other developers to
-        incorporate.  Many developers of free software are heartened and
-        encouraged by the resulting cooperation.  However, in the case of
-        software used on network servers, this result may fail to come about.
-        The GNU General Public License permits making a modified version and
-        letting the public access it on a server without ever releasing its
-        source code to the public.
-        
-          The GNU Affero General Public License is designed specifically to
-        ensure that, in such cases, the modified source code becomes available
-        to the community.  It requires the operator of a network server to
-        provide the source code of the modified version running there to the
-        users of that server.  Therefore, public use of a modified version, on
-        a publicly accessible server, gives the public access to the source
-        code of the modified version.
-        
-          An older license, called the Affero General Public License and
-        published by Affero, was designed to accomplish similar goals.  This is
-        a different license, not a version of the Affero GPL, but Affero has
-        released a new version of the Affero GPL which permits relicensing under
-        this license.
-        
-          The precise terms and conditions for copying, distribution and
-        modification follow.
-        
-                               TERMS AND CONDITIONS
-        
-          0. Definitions.
-        
-          "This License" refers to version 3 of the GNU Affero General Public License.
-        
-          "Copyright" also means copyright-like laws that apply to other kinds of
-        works, such as semiconductor masks.
-        
-          "The Program" refers to any copyrightable work licensed under this
-        License.  Each licensee is addressed as "you".  "Licensees" and
-        "recipients" may be individuals or organizations.
-        
-          To "modify" a work means to copy from or adapt all or part of the work
-        in a fashion requiring copyright permission, other than the making of an
-        exact copy.  The resulting work is called a "modified version" of the
-        earlier work or a work "based on" the earlier work.
-        
-          A "covered work" means either the unmodified Program or a work based
-        on the Program.
-        
-          To "propagate" a work means to do anything with it that, without
-        permission, would make you directly or secondarily liable for
-        infringement under applicable copyright law, except executing it on a
-        computer or modifying a private copy.  Propagation includes copying,
-        distribution (with or without modification), making available to the
-        public, and in some countries other activities as well.
-        
-          To "convey" a work means any kind of propagation that enables other
-        parties to make or receive copies.  Mere interaction with a user through
-        a computer network, with no transfer of a copy, is not conveying.
-        
-          An interactive user interface displays "Appropriate Legal Notices"
-        to the extent that it includes a convenient and prominently visible
-        feature that (1) displays an appropriate copyright notice, and (2)
-        tells the user that there is no warranty for the work (except to the
-        extent that warranties are provided), that licensees may convey the
-        work under this License, and how to view a copy of this License.  If
-        the interface presents a list of user commands or options, such as a
-        menu, a prominent item in the list meets this criterion.
-        
-          1. Source Code.
-        
-          The "source code" for a work means the preferred form of the work
-        for making modifications to it.  "Object code" means any non-source
-        form of a work.
-        
-          A "Standard Interface" means an interface that either is an official
-        standard defined by a recognized standards body, or, in the case of
-        interfaces specified for a particular programming language, one that
-        is widely used among developers working in that language.
-        
-          The "System Libraries" of an executable work include anything, other
-        than the work as a whole, that (a) is included in the normal form of
-        packaging a Major Component, but which is not part of that Major
-        Component, and (b) serves only to enable use of the work with that
-        Major Component, or to implement a Standard Interface for which an
-        implementation is available to the public in source code form.  A
-        "Major Component", in this context, means a major essential component
-        (kernel, window system, and so on) of the specific operating system
-        (if any) on which the executable work runs, or a compiler used to
-        produce the work, or an object code interpreter used to run it.
-        
-          The "Corresponding Source" for a work in object code form means all
-        the source code needed to generate, install, and (for an executable
-        work) run the object code and to modify the work, including scripts to
-        control those activities.  However, it does not include the work's
-        System Libraries, or general-purpose tools or generally available free
-        programs which are used unmodified in performing those activities but
-        which are not part of the work.  For example, Corresponding Source
-        includes interface definition files associated with source files for
-        the work, and the source code for shared libraries and dynamically
-        linked subprograms that the work is specifically designed to require,
-        such as by intimate data communication or control flow between those
-        subprograms and other parts of the work.
-        
-          The Corresponding Source need not include anything that users
-        can regenerate automatically from other parts of the Corresponding
-        Source.
-        
-          The Corresponding Source for a work in source code form is that
-        same work.
-        
-          2. Basic Permissions.
-        
-          All rights granted under this License are granted for the term of
-        copyright on the Program, and are irrevocable provided the stated
-        conditions are met.  This License explicitly affirms your unlimited
-        permission to run the unmodified Program.  The output from running a
-        covered work is covered by this License only if the output, given its
-        content, constitutes a covered work.  This License acknowledges your
-        rights of fair use or other equivalent, as provided by copyright law.
-        
-          You may make, run and propagate covered works that you do not
-        convey, without conditions so long as your license otherwise remains
-        in force.  You may convey covered works to others for the sole purpose
-        of having them make modifications exclusively for you, or provide you
-        with facilities for running those works, provided that you comply with
-        the terms of this License in conveying all material for which you do
-        not control copyright.  Those thus making or running the covered works
-        for you must do so exclusively on your behalf, under your direction
-        and control, on terms that prohibit them from making any copies of
-        your copyrighted material outside their relationship with you.
-        
-          Conveying under any other circumstances is permitted solely under
-        the conditions stated below.  Sublicensing is not allowed; section 10
-        makes it unnecessary.
-        
-          3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-        
-          No covered work shall be deemed part of an effective technological
-        measure under any applicable law fulfilling obligations under article
-        11 of the WIPO copyright treaty adopted on 20 December 1996, or
-        similar laws prohibiting or restricting circumvention of such
-        measures.
-        
-          When you convey a covered work, you waive any legal power to forbid
-        circumvention of technological measures to the extent such circumvention
-        is effected by exercising rights under this License with respect to
-        the covered work, and you disclaim any intention to limit operation or
-        modification of the work as a means of enforcing, against the work's
-        users, your or third parties' legal rights to forbid circumvention of
-        technological measures.
-        
-          4. Conveying Verbatim Copies.
-        
-          You may convey verbatim copies of the Program's source code as you
-        receive it, in any medium, provided that you conspicuously and
-        appropriately publish on each copy an appropriate copyright notice;
-        keep intact all notices stating that this License and any
-        non-permissive terms added in accord with section 7 apply to the code;
-        keep intact all notices of the absence of any warranty; and give all
-        recipients a copy of this License along with the Program.
-        
-          You may charge any price or no price for each copy that you convey,
-        and you may offer support or warranty protection for a fee.
-        
-          5. Conveying Modified Source Versions.
-        
-          You may convey a work based on the Program, or the modifications to
-        produce it from the Program, in the form of source code under the
-        terms of section 4, provided that you also meet all of these conditions:
-        
-            a) The work must carry prominent notices stating that you modified
-            it, and giving a relevant date.
-        
-            b) The work must carry prominent notices stating that it is
-            released under this License and any conditions added under section
-            7.  This requirement modifies the requirement in section 4 to
-            "keep intact all notices".
-        
-            c) You must license the entire work, as a whole, under this
-            License to anyone who comes into possession of a copy.  This
-            License will therefore apply, along with any applicable section 7
-            additional terms, to the whole of the work, and all its parts,
-            regardless of how they are packaged.  This License gives no
-            permission to license the work in any other way, but it does not
-            invalidate such permission if you have separately received it.
-        
-            d) If the work has interactive user interfaces, each must display
-            Appropriate Legal Notices; however, if the Program has interactive
-            interfaces that do not display Appropriate Legal Notices, your
-            work need not make them do so.
-        
-          A compilation of a covered work with other separate and independent
-        works, which are not by their nature extensions of the covered work,
-        and which are not combined with it such as to form a larger program,
-        in or on a volume of a storage or distribution medium, is called an
-        "aggregate" if the compilation and its resulting copyright are not
-        used to limit the access or legal rights of the compilation's users
-        beyond what the individual works permit.  Inclusion of a covered work
-        in an aggregate does not cause this License to apply to the other
-        parts of the aggregate.
-        
-          6. Conveying Non-Source Forms.
-        
-          You may convey a covered work in object code form under the terms
-        of sections 4 and 5, provided that you also convey the
-        machine-readable Corresponding Source under the terms of this License,
-        in one of these ways:
-        
-            a) Convey the object code in, or embodied in, a physical product
-            (including a physical distribution medium), accompanied by the
-            Corresponding Source fixed on a durable physical medium
-            customarily used for software interchange.
-        
-            b) Convey the object code in, or embodied in, a physical product
-            (including a physical distribution medium), accompanied by a
-            written offer, valid for at least three years and valid for as
-            long as you offer spare parts or customer support for that product
-            model, to give anyone who possesses the object code either (1) a
-            copy of the Corresponding Source for all the software in the
-            product that is covered by this License, on a durable physical
-            medium customarily used for software interchange, for a price no
-            more than your reasonable cost of physically performing this
-            conveying of source, or (2) access to copy the
-            Corresponding Source from a network server at no charge.
-        
-            c) Convey individual copies of the object code with a copy of the
-            written offer to provide the Corresponding Source.  This
-            alternative is allowed only occasionally and noncommercially, and
-            only if you received the object code with such an offer, in accord
-            with subsection 6b.
-        
-            d) Convey the object code by offering access from a designated
-            place (gratis or for a charge), and offer equivalent access to the
-            Corresponding Source in the same way through the same place at no
-            further charge.  You need not require recipients to copy the
-            Corresponding Source along with the object code.  If the place to
-            copy the object code is a network server, the Corresponding Source
-            may be on a different server (operated by you or a third party)
-            that supports equivalent copying facilities, provided you maintain
-            clear directions next to the object code saying where to find the
-            Corresponding Source.  Regardless of what server hosts the
-            Corresponding Source, you remain obligated to ensure that it is
-            available for as long as needed to satisfy these requirements.
-        
-            e) Convey the object code using peer-to-peer transmission, provided
-            you inform other peers where the object code and Corresponding
-            Source of the work are being offered to the general public at no
-            charge under subsection 6d.
-        
-          A separable portion of the object code, whose source code is excluded
-        from the Corresponding Source as a System Library, need not be
-        included in conveying the object code work.
-        
-          A "User Product" is either (1) a "consumer product", which means any
-        tangible personal property which is normally used for personal, family,
-        or household purposes, or (2) anything designed or sold for incorporation
-        into a dwelling.  In determining whether a product is a consumer product,
-        doubtful cases shall be resolved in favor of coverage.  For a particular
-        product received by a particular user, "normally used" refers to a
-        typical or common use of that class of product, regardless of the status
-        of the particular user or of the way in which the particular user
-        actually uses, or expects or is expected to use, the product.  A product
-        is a consumer product regardless of whether the product has substantial
-        commercial, industrial or non-consumer uses, unless such uses represent
-        the only significant mode of use of the product.
-        
-          "Installation Information" for a User Product means any methods,
-        procedures, authorization keys, or other information required to install
-        and execute modified versions of a covered work in that User Product from
-        a modified version of its Corresponding Source.  The information must
-        suffice to ensure that the continued functioning of the modified object
-        code is in no case prevented or interfered with solely because
-        modification has been made.
-        
-          If you convey an object code work under this section in, or with, or
-        specifically for use in, a User Product, and the conveying occurs as
-        part of a transaction in which the right of possession and use of the
-        User Product is transferred to the recipient in perpetuity or for a
-        fixed term (regardless of how the transaction is characterized), the
-        Corresponding Source conveyed under this section must be accompanied
-        by the Installation Information.  But this requirement does not apply
-        if neither you nor any third party retains the ability to install
-        modified object code on the User Product (for example, the work has
-        been installed in ROM).
-        
-          The requirement to provide Installation Information does not include a
-        requirement to continue to provide support service, warranty, or updates
-        for a work that has been modified or installed by the recipient, or for
-        the User Product in which it has been modified or installed.  Access to a
-        network may be denied when the modification itself materially and
-        adversely affects the operation of the network or violates the rules and
-        protocols for communication across the network.
-        
-          Corresponding Source conveyed, and Installation Information provided,
-        in accord with this section must be in a format that is publicly
-        documented (and with an implementation available to the public in
-        source code form), and must require no special password or key for
-        unpacking, reading or copying.
-        
-          7. Additional Terms.
-        
-          "Additional permissions" are terms that supplement the terms of this
-        License by making exceptions from one or more of its conditions.
-        Additional permissions that are applicable to the entire Program shall
-        be treated as though they were included in this License, to the extent
-        that they are valid under applicable law.  If additional permissions
-        apply only to part of the Program, that part may be used separately
-        under those permissions, but the entire Program remains governed by
-        this License without regard to the additional permissions.
-        
-          When you convey a copy of a covered work, you may at your option
-        remove any additional permissions from that copy, or from any part of
-        it.  (Additional permissions may be written to require their own
-        removal in certain cases when you modify the work.)  You may place
-        additional permissions on material, added by you to a covered work,
-        for which you have or can give appropriate copyright permission.
-        
-          Notwithstanding any other provision of this License, for material you
-        add to a covered work, you may (if authorized by the copyright holders of
-        that material) supplement the terms of this License with terms:
-        
-            a) Disclaiming warranty or limiting liability differently from the
-            terms of sections 15 and 16 of this License; or
-        
-            b) Requiring preservation of specified reasonable legal notices or
-            author attributions in that material or in the Appropriate Legal
-            Notices displayed by works containing it; or
-        
-            c) Prohibiting misrepresentation of the origin of that material, or
-            requiring that modified versions of such material be marked in
-            reasonable ways as different from the original version; or
-        
-            d) Limiting the use for publicity purposes of names of licensors or
-            authors of the material; or
-        
-            e) Declining to grant rights under trademark law for use of some
-            trade names, trademarks, or service marks; or
-        
-            f) Requiring indemnification of licensors and authors of that
-            material by anyone who conveys the material (or modified versions of
-            it) with contractual assumptions of liability to the recipient, for
-            any liability that these contractual assumptions directly impose on
-            those licensors and authors.
-        
-          All other non-permissive additional terms are considered "further
-        restrictions" within the meaning of section 10.  If the Program as you
-        received it, or any part of it, contains a notice stating that it is
-        governed by this License along with a term that is a further
-        restriction, you may remove that term.  If a license document contains
-        a further restriction but permits relicensing or conveying under this
-        License, you may add to a covered work material governed by the terms
-        of that license document, provided that the further restriction does
-        not survive such relicensing or conveying.
-        
-          If you add terms to a covered work in accord with this section, you
-        must place, in the relevant source files, a statement of the
-        additional terms that apply to those files, or a notice indicating
-        where to find the applicable terms.
-        
-          Additional terms, permissive or non-permissive, may be stated in the
-        form of a separately written license, or stated as exceptions;
-        the above requirements apply either way.
-        
-          8. Termination.
-        
-          You may not propagate or modify a covered work except as expressly
-        provided under this License.  Any attempt otherwise to propagate or
-        modify it is void, and will automatically terminate your rights under
-        this License (including any patent licenses granted under the third
-        paragraph of section 11).
-        
-          However, if you cease all violation of this License, then your
-        license from a particular copyright holder is reinstated (a)
-        provisionally, unless and until the copyright holder explicitly and
-        finally terminates your license, and (b) permanently, if the copyright
-        holder fails to notify you of the violation by some reasonable means
-        prior to 60 days after the cessation.
-        
-          Moreover, your license from a particular copyright holder is
-        reinstated permanently if the copyright holder notifies you of the
-        violation by some reasonable means, this is the first time you have
-        received notice of violation of this License (for any work) from that
-        copyright holder, and you cure the violation prior to 30 days after
-        your receipt of the notice.
-        
-          Termination of your rights under this section does not terminate the
-        licenses of parties who have received copies or rights from you under
-        this License.  If your rights have been terminated and not permanently
-        reinstated, you do not qualify to receive new licenses for the same
-        material under section 10.
-        
-          9. Acceptance Not Required for Having Copies.
-        
-          You are not required to accept this License in order to receive or
-        run a copy of the Program.  Ancillary propagation of a covered work
-        occurring solely as a consequence of using peer-to-peer transmission
-        to receive a copy likewise does not require acceptance.  However,
-        nothing other than this License grants you permission to propagate or
-        modify any covered work.  These actions infringe copyright if you do
-        not accept this License.  Therefore, by modifying or propagating a
-        covered work, you indicate your acceptance of this License to do so.
-        
-          10. Automatic Licensing of Downstream Recipients.
-        
-          Each time you convey a covered work, the recipient automatically
-        receives a license from the original licensors, to run, modify and
-        propagate that work, subject to this License.  You are not responsible
-        for enforcing compliance by third parties with this License.
-        
-          An "entity transaction" is a transaction transferring control of an
-        organization, or substantially all assets of one, or subdividing an
-        organization, or merging organizations.  If propagation of a covered
-        work results from an entity transaction, each party to that
-        transaction who receives a copy of the work also receives whatever
-        licenses to the work the party's predecessor in interest had or could
-        give under the previous paragraph, plus a right to possession of the
-        Corresponding Source of the work from the predecessor in interest, if
-        the predecessor has it or can get it with reasonable efforts.
-        
-          You may not impose any further restrictions on the exercise of the
-        rights granted or affirmed under this License.  For example, you may
-        not impose a license fee, royalty, or other charge for exercise of
-        rights granted under this License, and you may not initiate litigation
-        (including a cross-claim or counterclaim in a lawsuit) alleging that
-        any patent claim is infringed by making, using, selling, offering for
-        sale, or importing the Program or any portion of it.
-        
-          11. Patents.
-        
-          A "contributor" is a copyright holder who authorizes use under this
-        License of the Program or a work on which the Program is based.  The
-        work thus licensed is called the contributor's "contributor version".
-        
-          A contributor's "essential patent claims" are all patent claims
-        owned or controlled by the contributor, whether already acquired or
-        hereafter acquired, that would be infringed by some manner, permitted
-        by this License, of making, using, or selling its contributor version,
-        but do not include claims that would be infringed only as a
-        consequence of further modification of the contributor version.  For
-        purposes of this definition, "control" includes the right to grant
-        patent sublicenses in a manner consistent with the requirements of
-        this License.
-        
-          Each contributor grants you a non-exclusive, worldwide, royalty-free
-        patent license under the contributor's essential patent claims, to
-        make, use, sell, offer for sale, import and otherwise run, modify and
-        propagate the contents of its contributor version.
-        
-          In the following three paragraphs, a "patent license" is any express
-        agreement or commitment, however denominated, not to enforce a patent
-        (such as an express permission to practice a patent or covenant not to
-        sue for patent infringement).  To "grant" such a patent license to a
-        party means to make such an agreement or commitment not to enforce a
-        patent against the party.
-        
-          If you convey a covered work, knowingly relying on a patent license,
-        and the Corresponding Source of the work is not available for anyone
-        to copy, free of charge and under the terms of this License, through a
-        publicly available network server or other readily accessible means,
-        then you must either (1) cause the Corresponding Source to be so
-        available, or (2) arrange to deprive yourself of the benefit of the
-        patent license for this particular work, or (3) arrange, in a manner
-        consistent with the requirements of this License, to extend the patent
-        license to downstream recipients.  "Knowingly relying" means you have
-        actual knowledge that, but for the patent license, your conveying the
-        covered work in a country, or your recipient's use of the covered work
-        in a country, would infringe one or more identifiable patents in that
-        country that you have reason to believe are valid.
-        
-          If, pursuant to or in connection with a single transaction or
-        arrangement, you convey, or propagate by procuring conveyance of, a
-        covered work, and grant a patent license to some of the parties
-        receiving the covered work authorizing them to use, propagate, modify
-        or convey a specific copy of the covered work, then the patent license
-        you grant is automatically extended to all recipients of the covered
-        work and works based on it.
-        
-          A patent license is "discriminatory" if it does not include within
-        the scope of its coverage, prohibits the exercise of, or is
-        conditioned on the non-exercise of one or more of the rights that are
-        specifically granted under this License.  You may not convey a covered
-        work if you are a party to an arrangement with a third party that is
-        in the business of distributing software, under which you make payment
-        to the third party based on the extent of your activity of conveying
-        the work, and under which the third party grants, to any of the
-        parties who would receive the covered work from you, a discriminatory
-        patent license (a) in connection with copies of the covered work
-        conveyed by you (or copies made from those copies), or (b) primarily
-        for and in connection with specific products or compilations that
-        contain the covered work, unless you entered into that arrangement,
-        or that patent license was granted, prior to 28 March 2007.
-        
-          Nothing in this License shall be construed as excluding or limiting
-        any implied license or other defenses to infringement that may
-        otherwise be available to you under applicable patent law.
-        
-          12. No Surrender of Others' Freedom.
-        
-          If conditions are imposed on you (whether by court order, agreement or
-        otherwise) that contradict the conditions of this License, they do not
-        excuse you from the conditions of this License.  If you cannot convey a
-        covered work so as to satisfy simultaneously your obligations under this
-        License and any other pertinent obligations, then as a consequence you may
-        not convey it at all.  For example, if you agree to terms that obligate you
-        to collect a royalty for further conveying from those to whom you convey
-        the Program, the only way you could satisfy both those terms and this
-        License would be to refrain entirely from conveying the Program.
-        
-          13. Remote Network Interaction; Use with the GNU General Public License.
-        
-          Notwithstanding any other provision of this License, if you modify the
-        Program, your modified version must prominently offer all users
-        interacting with it remotely through a computer network (if your version
-        supports such interaction) an opportunity to receive the Corresponding
-        Source of your version by providing access to the Corresponding Source
-        from a network server at no charge, through some standard or customary
-        means of facilitating copying of software.  This Corresponding Source
-        shall include the Corresponding Source for any work covered by version 3
-        of the GNU General Public License that is incorporated pursuant to the
-        following paragraph.
-        
-          Notwithstanding any other provision of this License, you have
-        permission to link or combine any covered work with a work licensed
-        under version 3 of the GNU General Public License into a single
-        combined work, and to convey the resulting work.  The terms of this
-        License will continue to apply to the part which is the covered work,
-        but the work with which it is combined will remain governed by version
-        3 of the GNU General Public License.
-        
-          14. Revised Versions of this License.
-        
-          The Free Software Foundation may publish revised and/or new versions of
-        the GNU Affero General Public License from time to time.  Such new versions
-        will be similar in spirit to the present version, but may differ in detail to
-        address new problems or concerns.
-        
-          Each version is given a distinguishing version number.  If the
-        Program specifies that a certain numbered version of the GNU Affero General
-        Public License "or any later version" applies to it, you have the
-        option of following the terms and conditions either of that numbered
-        version or of any later version published by the Free Software
-        Foundation.  If the Program does not specify a version number of the
-        GNU Affero General Public License, you may choose any version ever published
-        by the Free Software Foundation.
-        
-          If the Program specifies that a proxy can decide which future
-        versions of the GNU Affero General Public License can be used, that proxy's
-        public statement of acceptance of a version permanently authorizes you
-        to choose that version for the Program.
-        
-          Later license versions may give you additional or different
-        permissions.  However, no additional obligations are imposed on any
-        author or copyright holder as a result of your choosing to follow a
-        later version.
-        
-          15. Disclaimer of Warranty.
-        
-          THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-        APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-        HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-        OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-        THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-        PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-        IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-        ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-        
-          16. Limitation of Liability.
-        
-          IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-        WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-        THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-        GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-        USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-        DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-        PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-        EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-        SUCH DAMAGES.
-        
-          17. Interpretation of Sections 15 and 16.
-        
-          If the disclaimer of warranty and limitation of liability provided
-        above cannot be given local legal effect according to their terms,
-        reviewing courts shall apply local law that most closely approximates
-        an absolute waiver of all civil liability in connection with the
-        Program, unless a warranty or assumption of liability accompanies a
-        copy of the Program in return for a fee.
-        
-                             END OF TERMS AND CONDITIONS
-        
-                    How to Apply These Terms to Your New Programs
-        
-          If you develop a new program, and you want it to be of the greatest
-        possible use to the public, the best way to achieve this is to make it
-        free software which everyone can redistribute and change under these terms.
-        
-          To do so, attach the following notices to the program.  It is safest
-        to attach them to the start of each source file to most effectively
-        state the exclusion of warranty; and each file should have at least
-        the "copyright" line and a pointer to where the full notice is found.
-        
-            <one line to give the program's name and a brief idea of what it does.>
-            Copyright (C) <year>  <name of author>
-        
-            This program is free software: you can redistribute it and/or modify
-            it under the terms of the GNU Affero General Public License as published
-            by the Free Software Foundation, either version 3 of the License, or
-            (at your option) any later version.
-        
-            This program is distributed in the hope that it will be useful,
-            but WITHOUT ANY WARRANTY; without even the implied warranty of
-            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-            GNU Affero General Public License for more details.
-        
-            You should have received a copy of the GNU Affero General Public License
-            along with this program.  If not, see <https://www.gnu.org/licenses/>.
-        
-        Also add information on how to contact you by electronic and paper mail.
-        
-          If your software can interact with users remotely through a computer
-        network, you should also make sure that it provides a way for users to
-        get its source.  For example, if your program is a web application, its
-        interface could display a "Source" link that leads users to an archive
-        of the code.  There are many ways you could offer source, and different
-        solutions will be better for different programs; see section 13 for the
-        specific requirements.
-        
-          You should also get your employer (if you work as a programmer) or school,
-        if any, to sign a "copyright disclaimer" for the program, if necessary.
-        For more information on this, and how to apply and follow the GNU AGPL, see
-        <https://www.gnu.org/licenses/>.
-        
-Project-URL: Homepage, https://github.com/impresso/impresso-pycommons
-Project-URL: Documentaton, https://impresso-pycommons.readthedocs.io/en/latest/
-Classifier: Programming Language :: Python :: 3
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: dask[complete]
-Requires-Dist: boto3
-Requires-Dist: beautifulsoup4
-Requires-Dist: docopt
-Requires-Dist: deprecated
-Requires-Dist: dkpro-cassis
-Requires-Dist: scikit-build
-Requires-Dist: cmake
-Requires-Dist: opencv-python
-Requires-Dist: numpy
-Requires-Dist: smart_open
-Requires-Dist: jsonlines
-Requires-Dist: s3fs
-Requires-Dist: python-dotenv
-
-# impresso_pycommons
-
-[![Documentation Status](https://readthedocs.org/projects/impresso-pycommons/badge/?version=latest)](https://impresso-pycommons.readthedocs.io/en/latest/?badge=latest)
-[![PyPI version](https://badge.fury.io/py/impresso-commons.svg)](https://badge.fury.io/py/impresso-commons)
-![PyPI - License](https://img.shields.io/pypi/l/impresso-commons)
-
-Python module with bits of code (objects, functions) highly-reusable within the [impresso project](https://impresso-project.ch/).
-
-Please refer to the [documentation](https://impresso-pycommons.readthedocs.io/) for further information on this library.
-
-## Installation
-
-With `pip`:
-
-```bash
-pip install impresso-commons
-```
-
-## Notes
-The library supports configuration of s3 credentials via project-specific local .env files. 
-
-## License
-
-The second project 'impresso - Media Monitoring of the Past II. Beyond Borders: Connecting Historical Newspapers and Radio' is funded by the Swiss National Science Foundation (SNSF) under grant number [CRSII5_213585](https://data.snf.ch/grants/grant/213585) and the Luxembourg National Research Fund under grant No. 17498891.
+                    GNU AFFERO GENERAL PUBLIC LICENSE
+                       Version 3, 19 November 2007
 
-Aiming to develop and consolidate tools to process and explore large-scale collections of historical newspapers and radio archives, and to study the impact of this tooling on historical research practices, _Impresso II_ builds upon the first project – 'impresso - Media Monitoring of the Past' (grant number [CRSII5_173719](http://p3.snf.ch/project-173719), Sinergia program). More information at https://impresso-project.ch.
-
-Copyright (C) 2024  The *impresso* team (contributors to this program: Matteo Romanello, Maud Ehrmann, Alex Flückinger, Edoardo Tarek Hölzl, Pauline Conti).
-
-This program is free software: you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
-
-This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of merchantability or fitness for a particular purpose. See the [GNU Affero General Public License](https://github.com/impresso/impresso-pycommons/blob/master/LICENSE) for more details.
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU Affero General Public License is a free, copyleft license for
+software and other kinds of works, specifically designed to ensure
+cooperation with the community in the case of network server software.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+our General Public Licenses are intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  Developers that use our General Public Licenses protect your rights
+with two steps: (1) assert copyright on the software, and (2) offer
+you this License which gives you legal permission to copy, distribute
+and/or modify the software.
+
+  A secondary benefit of defending all users' freedom is that
+improvements made in alternate versions of the program, if they
+receive widespread use, become available for other developers to
+incorporate.  Many developers of free software are heartened and
+encouraged by the resulting cooperation.  However, in the case of
+software used on network servers, this result may fail to come about.
+The GNU General Public License permits making a modified version and
+letting the public access it on a server without ever releasing its
+source code to the public.
+
+  The GNU Affero General Public License is designed specifically to
+ensure that, in such cases, the modified source code becomes available
+to the community.  It requires the operator of a network server to
+provide the source code of the modified version running there to the
+users of that server.  Therefore, public use of a modified version, on
+a publicly accessible server, gives the public access to the source
+code of the modified version.
+
+  An older license, called the Affero General Public License and
+published by Affero, was designed to accomplish similar goals.  This is
+a different license, not a version of the Affero GPL, but Affero has
+released a new version of the Affero GPL which permits relicensing under
+this license.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU Affero General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Remote Network Interaction; Use with the GNU General Public License.
+
+  Notwithstanding any other provision of this License, if you modify the
+Program, your modified version must prominently offer all users
+interacting with it remotely through a computer network (if your version
+supports such interaction) an opportunity to receive the Corresponding
+Source of your version by providing access to the Corresponding Source
+from a network server at no charge, through some standard or customary
+means of facilitating copying of software.  This Corresponding Source
+shall include the Corresponding Source for any work covered by version 3
+of the GNU General Public License that is incorporated pursuant to the
+following paragraph.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the work with which it is combined will remain governed by version
+3 of the GNU General Public License.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU Affero General Public License from time to time.  Such new versions
+will be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU Affero General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU Affero General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU Affero General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU Affero General Public License as published
+    by the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU Affero General Public License for more details.
+
+    You should have received a copy of the GNU Affero General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If your software can interact with users remotely through a computer
+network, you should also make sure that it provides a way for users to
+get its source.  For example, if your program is a web application, its
+interface could display a "Source" link that leads users to an archive
+of the code.  There are many ways you could offer source, and different
+solutions will be better for different programs; see section 13 for the
+specific requirements.
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU AGPL, see
+<https://www.gnu.org/licenses/>.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `impresso_commons-1.0.2/impresso_commons/classes/contentitem.py` & `impresso_commons-1.1.0/impresso_commons/classes/contentitem.py`

 * *Files identical despite different names*

### Comparing `impresso_commons-1.0.2/impresso_commons/data/config/patch_rebuilt_1.json` & `impresso_commons-1.1.0/impresso_commons/data/config/patch_rebuilt_1.json`

 * *Files identical despite different names*

### Comparing `impresso_commons-1.0.2/impresso_commons/data/config/patch_rebuilt_2.json` & `impresso_commons-1.1.0/impresso_commons/data/config/patch_rebuilt_2.json`

 * *Files identical despite different names*

### Comparing `impresso_commons-1.0.2/impresso_commons/data/config/patch_rebuilt_3.json` & `impresso_commons-1.1.0/impresso_commons/data/config/patch_rebuilt_3.json`

 * *Files identical despite different names*

### Comparing `impresso_commons-1.0.2/impresso_commons/data/config/patch_rebuilt_4.json` & `impresso_commons-1.1.0/impresso_commons/data/config/patch_rebuilt_4.json`

 * *Files identical despite different names*

### Comparing `impresso_commons-1.0.2/impresso_commons/data/xmi/typesystem.xml` & `impresso_commons-1.1.0/impresso_commons/data/xmi/typesystem.xml`

 * *Files identical despite different names*

### Comparing `impresso_commons-1.0.2/impresso_commons/images/img_utils.py` & `impresso_commons-1.1.0/impresso_commons/images/img_utils.py`

 * *Files identical despite different names*

### Comparing `impresso_commons-1.0.2/impresso_commons/images/olive_boxes.py` & `impresso_commons-1.1.0/impresso_commons/images/olive_boxes.py`

 * *Files identical despite different names*

### Comparing `impresso_commons-1.0.2/impresso_commons/path/__init__.py` & `impresso_commons-1.1.0/impresso_commons/path/__init__.py`

 * *Files identical despite different names*

### Comparing `impresso_commons-1.0.2/impresso_commons/path/path_fs.py` & `impresso_commons-1.1.0/impresso_commons/path/path_fs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,23 @@
 """Code for parsing impresso's canonical directory structures."""
 
 import os
 import logging
 from datetime import date, datetime
-from smart_open import s3_iter_bucket
 from collections import namedtuple
 import re
-import json
 
 logger = logging.getLogger(__name__)
 
 # a simple data structure to represent input directories
 # a `Document.zip` file is expected to be found in `IssueDir.path`
-IssueDir = namedtuple(
-    "IssueDir", [
-        'journal',
-        'date',
-        'edition',
-        'path'
-    ]
-)
+IssueDir = namedtuple("IssueDir", ["journal", "date", "edition", "path"])
 
 ContentItem = namedtuple(
-    "Item", [
-        'journal',
-        'date',
-        'edition',
-        'number',
-        'path',
-        'type'
-    ]
+    "Item", ["journal", "date", "edition", "number", "path", "type"]
 )
 
 
 KNOWN_JOURNALS = [
     "BDC",
     "CDV",
     "DLE",
@@ -101,26 +85,31 @@
     "MGS",
     "NTS",
     "NZG",
     "SGZ",
     "SRT",
     "WHD",
     "ZBT",
-    "CON", "DTT",
-    "FCT", "GAV",
-    "GAZ", "LLS",
-    "OIZ", "SAX",
-    "SDT", "SMZ",
-    "VDR", "VHT"
-
+    "CON",
+    "DTT",
+    "FCT",
+    "GAV",
+    "GAZ",
+    "LLS",
+    "OIZ",
+    "SAX",
+    "SDT",
+    "SMZ",
+    "VDR",
+    "VHT",
 ]
 
 
 def pair_issue(issue_list1, issue_list2):
-    """ Associates pairs of issues originating from original and canonical repositories.
+    """Associates pairs of issues originating from original and canonical repositories.
 
     :param issue_list1: list of IssueDir
     :type issue_list1: array
     :param issue_list2: list of IssueDir
     :type issue_list2: array
     :return: list containing tuples of issue pairs [(issue1, issue2), (...)]
     :rtype: list
@@ -158,26 +147,27 @@
             sep.join(
                 [
                     dir.journal,
                     str(dir.date.year),
                     str(dir.date.month).zfill(2),
                     str(dir.date.day).zfill(2),
                     dir.edition,
-                    name
+                    name,
                 ]
             ),
-            extension)
+            extension,
+        )
     else:
         return sep.join(
             [
                 dir.journal,
                 str(dir.date.year),
                 str(dir.date.month).zfill(2),
                 str(dir.date.day).zfill(2),
-                dir.edition
+                dir.edition,
             ]
         )
 
 
 def _apply_datefilter(filter_dict, issues, year_only):
     filtered_issues = []
 
@@ -200,22 +190,22 @@
                     for i in issues
                     if i.journal == newspaper and start <= i.date <= end
                 ]
 
         # date filter is not a range
         elif isinstance(dates, list):
             if not dates:
-                filtered_issues += [
-                    i
-                    for i in issues
-                    if i.journal == newspaper
-                ]
+                filtered_issues += [i for i in issues if i.journal == newspaper]
             else:
                 filter_date = [
-                    datetime.strptime(d, "%Y/%m/%d").date().year if year_only else datetime.strptime(d, "%Y/%m/%d").date()
+                    (
+                        datetime.strptime(d, "%Y/%m/%d").date().year
+                        if year_only
+                        else datetime.strptime(d, "%Y/%m/%d").date()
+                    )
                     for d in dates
                 ]
 
                 if year_only:
                     filtered_issues += [
                         i
                         for i in issues
@@ -228,15 +218,15 @@
                         if i.journal == newspaper and i.date in filter_date
                     ]
 
     return filtered_issues
 
 
 def select_issues(config_dict, inp_dir):
-    """ Reads a configuration file and select newspapers/issues to consider
+    """Reads a configuration file and select newspapers/issues to consider
     See config.example.md for explanations.
 
     Usage example:
         if config_file and os.path.isfile(config_file):
             with open(config_file, 'r') as f:
                 config = json.load(f)
                 issues = select_issues(config, inp_dir)
@@ -251,34 +241,52 @@
     """
     # read filters from json configuration (see config.example.json)
     try:
         filter_dict = config_dict.get("newspapers")
         exclude_list = config_dict["exclude_newspapers"]
         year_flag = config_dict["year_only"]
     except KeyError:
-        logger.critical(f"The key [newspapers|exclude_newspapers|year_only] is missing in the config file.")
+        logger.critical(
+            f"The key [newspapers|exclude_newspapers|year_only] is missing in the config file."
+        )
         return
     exclude_flag = False if not exclude_list else True
-    logger.debug(f"got filter_dict: {filter_dict}, "
-                 f"\nexclude_list: {exclude_list}, "
-                 f"\nyear_flag: {year_flag}"
-                 f"\nexclude_flag: {exclude_flag}")
+    logger.debug(
+        f"got filter_dict: {filter_dict}, "
+        f"\nexclude_list: {exclude_list}, "
+        f"\nyear_flag: {year_flag}"
+        f"\nexclude_flag: {exclude_flag}"
+    )
 
     # detect issues to be imported
-    if not filter_dict and not exclude_list:  # todo: remove this case? should be detect issue
-        logger.debug("No positive nor negative filter definition, all issues in {inp_dir} will be considered.")
+    if (
+        not filter_dict and not exclude_list
+    ):  # todo: remove this case? should be detect issue
+        logger.debug(
+            "No positive nor negative filter definition, all issues in {inp_dir} will be considered."
+        )
         issues = detect_issues(inp_dir)
         return issues
     else:
-        filter_newspapers = set(filter_dict.keys()) if not exclude_list else set(exclude_list)
-        logger.debug(f"got filter_newspapers: {filter_newspapers}, with exclude flag: {exclude_flag}")
-        issues = detect_issues(inp_dir, journal_filter=filter_newspapers, exclude=exclude_flag)
+        filter_newspapers = (
+            set(filter_dict.keys()) if not exclude_list else set(exclude_list)
+        )
+        logger.debug(
+            f"got filter_newspapers: {filter_newspapers}, with exclude flag: {exclude_flag}"
+        )
+        issues = detect_issues(
+            inp_dir, journal_filter=filter_newspapers, exclude=exclude_flag
+        )
 
         # apply date filter if not exclusion mode
-        filtered_issues = _apply_datefilter(filter_dict, issues, year_only=year_flag) if not exclude_flag else issues
+        filtered_issues = (
+            _apply_datefilter(filter_dict, issues, year_only=year_flag)
+            if not exclude_flag
+            else issues
+        )
         return filtered_issues
 
 
 def detect_issues(base_dir, journal_filter=None, exclude=False):
     """Parse a directory structure and detect newspaper issues to be imported.
 
     NB: invalid directories are skipped, and a warning message is logged.
@@ -294,21 +302,17 @@
     detected_issues = []
     dir_path, dirs, files = next(os.walk(base_dir))
     # workaround to deal with journal-level folders like: 01_GDL, 02_GDL
     if journal_filter is None:
         journal_dirs = [d for d in dirs if d.split("_")[-1] in KNOWN_JOURNALS]
     else:
         if not exclude:
-            filtrd_journals = list(
-                set(KNOWN_JOURNALS).intersection(journal_filter)
-            )
+            filtrd_journals = list(set(KNOWN_JOURNALS).intersection(journal_filter))
         else:
-            filtrd_journals = list(
-                set(KNOWN_JOURNALS).difference(journal_filter)
-            )
+            filtrd_journals = list(set(KNOWN_JOURNALS).difference(journal_filter))
         journal_dirs = [d for d in dirs if d.split("_")[-1] in filtrd_journals]
 
     for journal in journal_dirs:
         journal_path = os.path.join(base_dir, journal)
         journal = journal.split("_")[-1] if "_" in journal else journal
         dir_path, year_dirs, files = next(os.walk(journal_path))
         # year_dirs = [d for d in dirs if len(d) == 4]
@@ -326,26 +330,22 @@
                     # concerning `edition="a"`: for now, no cases of newspapers
                     # published more than once a day in Olive format (but it
                     # may come later on)
                     try:
                         detected_issue = IssueDir(
                             journal,
                             date(int(year), int(month), int(day)),
-                            'a',
-                            day_path
-                        )
-                        logger.debug("Found an issue: {}".format(
-                            str(detected_issue))
+                            "a",
+                            day_path,
                         )
+                        logger.debug("Found an issue: {}".format(str(detected_issue)))
                         detected_issues.append(detected_issue)
                     except ValueError:
                         logger.warning(
-                            "Path {} is not a valid issue directory".format(
-                                day_path
-                            )
+                            "Path {} is not a valid issue directory".format(day_path)
                         )
     return detected_issues
 
 
 def detect_canonical_issues(base_dir, newspapers):
     """Parse a directory structure and detect newspaper issues to be imported.
 
@@ -386,18 +386,18 @@
                     for edition in edition_dirs:
                         edition_path = os.path.join(day_path, edition)
                         try:
                             detected_issue = IssueDir(
                                 journal,
                                 date(int(year), int(month), int(day)),
                                 edition,
-                                edition_path
+                                edition_path,
                             )
-                            logger.debug("Found an issue: {}".format(
-                                str(detected_issue))
+                            logger.debug(
+                                "Found an issue: {}".format(str(detected_issue))
                             )
                             detected_issues.append(detected_issue)
                         except ValueError:
                             logger.warning(
                                 "Path {} is not a valid issue directory".format(
                                     edition_path
                                 )
@@ -411,15 +411,15 @@
     :param base_dir: the root of the directory structure
     :type base_dir: IssueDir
     :param newspapers: the list of newspapers to consider (acronym blank separated)
     :type newspapers: str
     :return: list of `IssueDir` instances
     :rtype: list
     """
-    #newspapers = [journal.split("_")[-1] if "_" in journal else journal for journal in newspapers]
+    # newspapers = [journal.split("_")[-1] if "_" in journal else journal for journal in newspapers]
 
     detected_issues = []
     dir_path, dirs, files = next(os.walk(base_dir))
     journal_dirs = [d for d in dirs if d == newspapers]
 
     for journal in journal_dirs:
         journal_path = os.path.join(base_dir, journal)
@@ -441,32 +441,32 @@
                                 day_path = os.path.join(month_path, day)
                                 # concerning `edition="a"`: for now, no cases of newspapers
                                 # published more than once a day in Olive format (but it
                                 # may come later on)
                                 detected_issue = IssueDir(
                                     journal,
                                     date(int(year), int(month), int(day)),
-                                    'a',
-                                    day_path
+                                    "a",
+                                    day_path,
                                 )
-                                logger.debug("Found an issue: {}".format(
-                                    str(detected_issue))
+                                logger.debug(
+                                    "Found an issue: {}".format(str(detected_issue))
                                 )
                                 detected_issues.append(detected_issue)
     return detected_issues
 
 
 def check_filenaming(file_basename):
-    """ Checks whether a filename complies with our naming convention (GDL-1900-01-10-a-p0001)
+    """Checks whether a filename complies with our naming convention (GDL-1900-01-10-a-p0001)
 
     :param file_basename: page file (txt or image)
     :type file_basename: str
     """
     page_pattern = re.compile(r"^[A-Z]+-\d{4}-\d{2}-\d{2}-[a-z]-p\d{4}$")
     return page_pattern.match(file_basename)
 
 
 def get_issueshortpath(issuedir):
-    """ Returns short version of issue dir path"""
+    """Returns short version of issue dir path"""
 
     path = issuedir.path
-    return path[path.index(issuedir.journal):]
+    return path[path.index(issuedir.journal) :]
```

### Comparing `impresso_commons-1.0.2/impresso_commons/path/path_s3.py` & `impresso_commons-1.1.0/impresso_commons/path/path_s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import os
 import json
 import logging
 import warnings
 from datetime import date
 from collections import namedtuple
+from typing import Optional, Union
 
 from dask.diagnostics import ProgressBar
 import dask.bag as db
 
 from impresso_commons.path import id2IssueDir
 from impresso_commons.utils.s3 import get_s3_client, get_s3_versions, fixed_s3fs_glob
 from impresso_commons.utils.s3 import IMPRESSO_STORAGEOPT
@@ -187,15 +188,15 @@
         logger.error("Provide either a prefix or a config but not both")
         return None
 
     # check which kind of object to build, issue or content_item
     suffix = "issue.json" if item_type == "issue" else ".json"
 
     # collect keys using pagination
-    logger.info(f"Start collecting key from s3 (not parallel)")
+    logger.info("Start collecting key from s3 (not parallel)")
     if filter_config is None:
         keys = _list_bucket_paginator(
             bucket_name, prefix, accept_key=lambda key: key.endswith(suffix)
         )
     else:
         keys = _list_bucket_paginator_filter(
             bucket_name,
@@ -290,22 +291,22 @@
 
 def read_s3_issues(newspaper, year, input_bucket):
 
     def add_version(issue):
         issue["s3_version"] = None
         return issue
 
-    issue_path_ons3 = (
+    issue_path_on_s3 = (
         f"{input_bucket}/{newspaper}/issues/{newspaper}-{year}-issues.jsonl.bz2"
     )
     issues = (
-        db.read_text(issue_path_ons3, storage_options=IMPRESSO_STORAGEOPT)
-        .map(lambda x: json.loads(x))
+        db.read_text(issue_path_on_s3, storage_options=IMPRESSO_STORAGEOPT)
+        .map(json.loads)
         .map(add_version)
-        .map(lambda x: (id2IssueDir(x["id"], issue_path_ons3), x))
+        .map(lambda x: (id2IssueDir(x["id"], issue_path_on_s3), x))
         .compute()
     )
     return issues
 
 
 def list_newspapers(
     bucket_name: str,
@@ -355,16 +356,16 @@
 
     return newspapers
 
 
 def list_files(
     bucket_name: str,
     file_type: str = "issues",
-    newspapers_filter: list[str] | None = None,
-) -> tuple[list[str] | None, list[str] | None]:
+    newspapers_filter: Optional[list[str]] = None,
+) -> tuple[Optional[list[str]], Optional[list[str]]]:
     """List the canonical files located in a given S3 bucket.
 
     Note:
         adapted from https://github.com/impresso/impresso-data-sanitycheck/tree/master/sanity_check/contents/s3_data.py
 
     Args:
         bucket_name (str): S3 bucket name.
@@ -395,17 +396,15 @@
         suffix = ""
 
     if file_type in ["issues", "both"]:
         issue_files = [
             file
             for np in newspapers
             if newspapers_filter is not None and np in newspapers_filter
-            for file in fixed_s3fs_glob(
-                f"{os.path.join(bucket_name, f'{np}/issues/*')}"
-            )
+            for file in fixed_s3fs_glob(os.path.join(bucket_name, f"{np}/issues/*"))
         ]
         print(f"{bucket_name} contains {len(issue_files)} .bz2 issue files {suffix}")
     if file_type in ["pages", "both"]:
         page_files = [
             file
             for np in newspapers
             if newspapers_filter is not None and np in newspapers_filter
@@ -416,16 +415,16 @@
     return issue_files, page_files
 
 
 def fetch_files(
     bucket_name: str,
     compute: bool = True,
     file_type: str = "issues",
-    newspapers_filter: list[str] | None = None,
-) -> tuple[db.core.Bag | list[str] | None, db.core.Bag | list[str] | None]:
+    newspapers_filter: Optional[list[str]] = None,
+) -> tuple[Union[db.core.Bag, list[str], None], Union[db.core.Bag, list[str], None]]:
     """Fetch issue and/or page canonical JSON files from an s3 bucket.
 
     If compute=True, the output will be a list of the contents of all files in the
     bucket for the specified newspapers and type of files.
     If compute=False, the output will remain in a distributed dask.bag.
 
     Based on file_type, the issue files, page files or both will be returned.
```

### Comparing `impresso_commons-1.0.2/impresso_commons/schemas/Makefile` & `impresso_commons-1.1.0/impresso_commons/schemas/Makefile`

 * *Files identical despite different names*

### Comparing `impresso_commons-1.0.2/impresso_commons/schemas/Pipfile.lock` & `impresso_commons-1.1.0/impresso_commons/schemas/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `impresso_commons-1.0.2/impresso_commons/schemas/README.md` & `impresso_commons-1.1.0/impresso_commons/schemas/README.md`

 * *Files identical despite different names*

### Comparing `impresso_commons-1.0.2/impresso_commons/schemas/json/entities/entities.schema.json` & `impresso_commons-1.1.0/impresso_commons/schemas/json/entities/entities.schema.json`

 * *Files identical despite different names*

### Comparing `impresso_commons-1.0.2/impresso_commons/schemas/json/language_identification/language_identification.schema.json` & `impresso_commons-1.1.0/impresso_commons/schemas/json/language_identification/language_identification.schema.json`

 * *Files identical despite different names*

### Comparing `impresso_commons-1.0.2/impresso_commons/schemas/json/linguistic_annotation/ling_spacy.schema.json` & `impresso_commons-1.1.0/impresso_commons/schemas/json/linguistic_annotation/ling_spacy.schema.json`

 * *Files identical despite different names*

### Comparing `impresso_commons-1.0.2/impresso_commons/schemas/json/newspaper/contentitem.schema.json` & `impresso_commons-1.1.0/impresso_commons/schemas/json/newspaper/contentitem.schema.json`

 * *Files identical despite different names*

### Comparing `impresso_commons-1.0.2/impresso_commons/schemas/json/newspaper/issue.schema.json` & `impresso_commons-1.1.0/impresso_commons/schemas/json/newspaper/issue.schema.json`

 * *Files identical despite different names*

### Comparing `impresso_commons-1.0.2/impresso_commons/schemas/json/newspaper/page.schema.json` & `impresso_commons-1.1.0/impresso_commons/schemas/json/newspaper/page.schema.json`

 * *Files identical despite different names*

### Comparing `impresso_commons-1.0.2/impresso_commons/schemas/json/topic_model/topic_assignment.schema.json` & `impresso_commons-1.1.0/impresso_commons/schemas/json/topic_model/topic_assignment.schema.json`

 * *Files identical despite different names*

### Comparing `impresso_commons-1.0.2/impresso_commons/schemas/json/topic_model/topic_description.schema.json` & `impresso_commons-1.1.0/impresso_commons/schemas/json/topic_model/topic_description.schema.json`

 * *Files identical despite different names*

### Comparing `impresso_commons-1.0.2/impresso_commons/schemas/json/versioning/manifest.schema.json` & `impresso_commons-1.1.0/impresso_commons/schemas/json/versioning/manifest.schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999935611263736%*

 * *Differences: {"'definitions'": "{'media_statistics': {'properties': {'nps_stats': {'properties': {'lang_fd': "*

 * *                  "OrderedDict([('type', 'object'), ('description', 'Frequency dict with the "*

 * *                  "occurences of each lang identified in the data.')]), 'text_reuse_clusters': "*

 * *                  "OrderedDict([('type', 'integer'), ('description', 'Number of text-reuse "*

 * *                  "clusters indentified in the data.')]), delete: ['ne_links']}}}}}"}*

```diff
@@ -55,30 +55,34 @@
                             "description": "Number of images present in the data.",
                             "type": "integer"
                         },
                         "issues": {
                             "description": "Number of issues present in the data.",
                             "type": "integer"
                         },
+                        "lang_fd": {
+                            "description": "Frequency dict with the occurences of each lang identified in the data.",
+                            "type": "object"
+                        },
                         "ne_entities": {
                             "description": "Number of unique named entities present in the data.",
                             "type": "integer"
                         },
-                        "ne_links": {
-                            "description": "Number of named-entity links present in the data.",
-                            "type": "integer"
-                        },
                         "ne_mentions": {
                             "description": "Number of named-entity mentions present in the data.",
                             "type": "integer"
                         },
                         "pages": {
                             "description": "Number of pages present in the data.",
                             "type": "integer"
                         },
+                        "text_reuse_clusters": {
+                            "description": "Number of text-reuse clusters indentified in the data.",
+                            "type": "integer"
+                        },
                         "titles": {
                             "description": "Number of newspaper titles included in the data.",
                             "type": "integer"
                         },
                         "topics": {
                             "description": "Number of topics extracted from the data.",
                             "type": "integer"
```

### Comparing `impresso_commons-1.0.2/impresso_commons/text/helpers.py` & `impresso_commons-1.1.0/impresso_commons/text/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """Helper functions for the text `rebuilder.py` script."""
 
 import json
 import logging
 import os
-from typing import Any
-
-from dask import bag as db
+from typing import Any, Optional, Union
 
 from impresso_commons.utils.s3 import (
     IMPRESSO_STORAGEOPT,
     alternative_read_text,
     get_s3_resource,
     get_s3_versions,
 )
 
 logger = logging.getLogger(__name__)
 
 IIIF_ENDPOINT_BASE_2_SUFFIX = {
-    "https://ub-sipi.ub.unibas.ch/impresso": "max/0/default.jpg",  # suffix for SWA data
-    "https://scriptorium.bcu-lausanne.ch/api": "450,/0/default.jpg",  # suffix for BCUL data
+    # suffix for SWA data
+    "https://ub-sipi.ub.unibas.ch/impresso": "max/0/default.jpg",
+    # suffix for BCUL data, sometimes 300 can be replaced by larger values
+    "https://scriptorium.bcu-lausanne.ch/api": "300,/0/default.jpg",
 }
 
 WHITESPACE_RULES = {
     "fr": {
         "pct_no_ws_before": [".", ",", ")", "]", "}", "°", "...", ".-", "%"],
         "pct_no_ws_after": ["(", "[", "{"],
         "pct_no_ws_before_after": ["'", "-"],
@@ -87,30 +87,30 @@
     if s3_client is None:
         s3_client = get_s3_resource()
 
     content_object = s3_client.Object(bucket_name, issue.path)
     file_content = content_object.get()["Body"].read().decode("utf-8")
     issue_json = json.loads(file_content)
     issue_json["s3_version"] = get_s3_versions(bucket_name, issue.path)[0][0]
-    logger.info("Read JSON of {}".format(issue))
+    logger.info("Read JSON of %s", issue)
     return (issue, issue_json)
 
 
 def read_page(page_key, bucket_name, s3_client):
     """Read the data from S3 for a given newspaper pages."""
 
     try:
         content_object = s3_client.Object(bucket_name, page_key)
         file_content = content_object.get()["Body"].read().decode("utf-8")
         page_json = json.loads(file_content)
         page_json["s3v"] = get_s3_versions(bucket_name, page_key)[0][0]
-        logger.info("Read page {} from bucket {}".format(page_key, bucket_name))
+        logger.info("Read page %s from bucket %s", page_key, bucket_name)
         return page_json
     except Exception as e:
-        logger.error(f"There was a problem reading {page_key}: {e}")
+        logger.error("There was a problem reading %s: %s", page_key, e)
         return None
 
 
 def read_issue_pages(issue, issue_json, bucket=None):
     """Read all pages of a given issue from S3 in parallel."""
     newspaper = issue.journal
     year = issue.date.year
@@ -121,20 +121,14 @@
     )
 
     pages = [
         json.loads(page)
         for page in alternative_read_text(filename, IMPRESSO_STORAGEOPT)
     ]
 
-    """
-    pages = db.read_text(
-        filename,
-        storage_options=IMPRESSO_STORAGEOPT
-    ).map(lambda x: json.loads(x)).compute()
-    """
     print(filename)
     issue_json["pp"] = pages
     del pages
     return (issue, issue_json)
 
 
 def rejoin_articles(issue, issue_json):
@@ -161,16 +155,19 @@
                     if page_no_string in page["id"]
                 ][0]
                 pages.append(issue_json["pp"][page_idx])
             except IndexError:
                 article["has_problem"] = True
                 articles.append(article)
                 logger.error(
-                    f"Page {page_no_string} not found for item {art_id}"
-                    f"Issue {issue_json['id']} has pages {page_ids}"
+                    "Page %s not found for item %s. Issue %s has pages %s",
+                    page_no_string,
+                    art_id,
+                    issue_json["id"],
+                    page_ids,
                 )
                 continue
 
         regions_by_page = []
         for page in pages:
             regions_by_page.append(
                 [
@@ -191,26 +188,26 @@
     return articles
 
 
 def pages_to_article(article, pages):
     """Return all text regions belonging to a given article."""
     try:
         art_id = article["m"]["id"]
-        print("Extracting text regions for article {}".format(art_id))
+        print("Extracting text regions for article %s", art_id)
         regions_by_page = []
         for page in pages:
             regions_by_page.append(
                 [region for region in page["r"] if region["pOf"] == art_id]
             )
         convert_coords = [page["cc"] for page in pages]
         article["m"]["cc"] = sum(convert_coords) / len(convert_coords) == 1.0
         article["has_problem"] = False
         article["pprr"] = regions_by_page
         return article
-    except Exception as e:
+    except Exception:
         article["has_problem"] = True
         return article
 
 
 def text_apply_breaks(fulltext, breaks):
     """Apply breaks to the text returned by `rebuild_for_solr`.
 
@@ -234,15 +231,15 @@
         start = br
 
     text.append(fulltext[start:])
 
     return text
 
 
-def get_iiif_and_coords(ci: dict[str, Any]) -> tuple[str | None, str | None]:
+def get_iiif_and_coords(ci: dict[str, Any]) -> tuple[Optional[str], Optional[str]]:
     """Fetch the iiif link and image coordinates from CI metadata.
 
     Adapts to the various cases currently present in the canonical data, see
     https://github.com/impresso/impresso-text-acquisition/issues/117.
 
     Args:
         ci (dict[str, Any]): Content item to retrieve the information from.
@@ -285,60 +282,72 @@
     iiif, coords = get_iiif_and_coords(content_item)
     if iiif:
         # recover the url base to which the image suffix should be appended
         uri_base, old_suffix = os.path.split(iiif)
 
         # SWA and BCUL data have a different image suffix than other endpoints
         for iiif_base, iiif_suffix in IIIF_ENDPOINT_BASE_2_SUFFIX.items():
-            img_suffix = iiif_suffix if uri_base in iiif_base else img_suffix
+            img_suffix = iiif_suffix if iiif_base in uri_base else img_suffix
 
         if old_suffix == "default.jpg":
             # iiif was already constructed according to needs.
             if coords in iiif and img_suffix in iiif:
                 return iiif
             # uri was already of image, but not correct.
             uri_base = "/".join(uri_base.split("/")[:-3])
         elif old_suffix != "info.json":
-            logger.warning(
+            warn_msg = (
                 f"Unexpected iiif url suffix: {old_suffix} "
                 f"for CI with id: {content_item['id']}."
             )
+            logger.warning(warn_msg)
 
         # reconstruct the final image link
         return os.path.join(uri_base, coords, img_suffix)
     return None
 
 
 def insert_whitespace(
-    token: str, next_t: str | None, prev_t: str | None, lang: str | None
+    token: str,
+    next_t: Optional[str],
+    prev_t: Optional[str],
+    lang: Optional[str],
 ) -> bool:
     """Determine whether a whitespace should be inserted after a token.
 
     Args:
         token (str): Current token.
         next_t (str): Following token.
         prev_t (str): Previous token.
         lang (str): Language of text.
 
     Returns:
         bool: Whether a whitespace should be inserted after the `token`.
     """
+    # if current token text is None, previous token's whitespace rule applies
+    if token is None or len(token) == 0:
+        return False
+
     wsrules = WHITESPACE_RULES[lang if lang in WHITESPACE_RULES else "other"]
 
     insert_ws = True
 
     if (
         token in wsrules["pct_no_ws_before_after"]
         or next_t in wsrules["pct_no_ws_before_after"]
     ):
         insert_ws = False
 
     # the first char of the next token is punctuation.
-    elif next_t is not None and next_t[0] in wsrules["pct_no_ws_before"]:
-        insert_ws = False
+    elif next_t is not None and len(next_t) != 0:
+        if (
+            next_t in wsrules["pct_no_ws_before"]
+            or next_t[0] in wsrules["pct_no_ws_before"]
+        ):
+            insert_ws = False
 
     # the last char of current token is punctuation.
     elif token in wsrules["pct_no_ws_after"] or token[-1] in wsrules["pct_no_ws_after"]:
         insert_ws = False
 
     elif token in wsrules["pct_number"] and prev_t is not None and next_t is not None:
         if prev_t.isdigit() and next_t.isdigit():
```

### Comparing `impresso_commons-1.0.2/impresso_commons/text/rebuilder.py` & `impresso_commons-1.1.0/impresso_commons/text/rebuilder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 """Functions and CLI to rebuild text from impresso's canonical format.
 For EPFL members, this script can be scaled by running it using Runai, 
 as documented on https://github.com/impresso/impresso-infrastructure/blob/main/howtos/runai.md.
 
 Usage:
-    rebuilder.py rebuild_articles --input-bucket=<b> --log-file=<f> --output-dir=<od> --filter-config=<fc> [--format=<fo> --scheduler=<sch> --output-bucket=<ob> --verbose --clear --languages=<lgs> --nworkers=<nw>]
+    rebuilder.py rebuild_articles --input-bucket=<b> --log-file=<f> --output-dir=<od> --filter-config=<fc> [--format=<fo> --scheduler=<sch> --output-bucket=<ob> --verbose --clear --languages=<lgs> --nworkers=<nw> --git-repo=<gr> --temp-dir=<tp> --prev-manifest=<pm>]
 
 Options:
 
 --input-bucket=<b>  S3 bucket where canonical JSON data will be read from
 --output-bucket=<ob>  Rebuilt data will be uploaded to the specified s3 bucket (otherwise no upload)
 --log-file=<f>  Path to log file
 --scheduler=<sch>  Tell dask to use an existing scheduler (otherwise it'll create one)
 --filter-config=<fc>  A JSON configuration file specifying which newspaper issues will be rebuilt
 --verbose  Set logging level to DEBUG (by default is INFO)
 --clear  Remove output directory before and after rebuilding
---format=<fo>  stuff
---nworkers=<nw>  number of workers for (local) dask client
+--format=<fo>  Rebuilt format to use (can be "solr" or "passim")
+--languages=<lgs>  Languages to filter the articles to rebuild on.
+--nworkers=<nw>  number of workers for (local) Dask client.
+--git-repo=<gr>   Local path to the "impresso-text-acquisition" git directory (including it).
+--temp-dir=<tp>  Temporary directory in which to clone the impresso-data-release git repository.
+--prev-manifest=<pm>  Optional S3 path to the previous manifest to use for the manifest generation.
 """  # noqa: E501
 
+import sys
 import traceback
 import datetime
 import json
 import pathlib
 import logging
 import os
 import shutil
 import signal
-from typing import Any
+from typing import Any, Optional
+import git
 
 import dask.bag as db
 import jsonlines
 from dask.distributed import Client, progress
 from docopt import docopt
 from smart_open import smart_open
 
@@ -41,14 +47,17 @@
     rejoin_articles,
     reconstruct_iiif_link,
     insert_whitespace,
 )
 from impresso_commons.utils import Timer, timestamp
 from impresso_commons.utils.s3 import get_s3_resource
 
+from impresso_commons.versioning.data_manifest import DataManifest
+from impresso_commons.versioning.helpers import compute_stats_in_rebuilt_bag
+
 logger = logging.getLogger(__name__)
 
 
 TYPE_MAPPINGS = {
     "article": "ar",
     "ar": "ar",
     "advertisement": "ad",
@@ -59,15 +68,15 @@
     "death_notice": "ob",
     "weather": "w",
 }
 # TODO KB data: add familial announcement?
 
 
 def rebuild_text(
-    page: list[dict], language: str | None, string: str | None = None
+    page: list[dict], language: Optional[str], string: Optional[str] = None
 ) -> tuple[str, dict[list], dict[list]]:
     """Rebuild the text of an article for Solr ingestion.
 
     If `string` is not `None`, then the rebuilt text is appended to it.
 
     Args:
         page (list[dict]): Newspaper page conforming to the impresso JSON pages schema.
@@ -84,48 +93,51 @@
     offsets = {"line": [], "para": [], "region": []}
 
     if string is None:
         string = ""
 
     # in order to be able to keep line break information
     # we iterate over a list of lists (lines of tokens)
-    for region_n, region in enumerate(page):
+    for region in page:
 
         if len(string) > 0:
             offsets["region"].append(len(string))
 
         coordinates["regions"].append(region["c"])
 
-        for i, para in enumerate(region["p"]):
+        for para in region["p"]:
 
             if len(string) > 0:
                 offsets["para"].append(len(string))
 
             for line in para["l"]:
 
                 for n, token in enumerate(line["t"]):
                     region = {}
+                    if "c" not in token:
+                        print(f"'c' was not present in token: {token}, line: {line}")
+                        continue
                     region["c"] = token["c"]
                     region["s"] = len(string)
 
                     if "hy" in token:
                         region["l"] = len(token["tx"][:-1]) - 1
                         region["hy1"] = True
                     elif "nf" in token:
                         region["l"] = len(token["nf"])
                         region["hy2"] = True
 
-                        token_text = token["nf"]
+                        token_text = token["nf"] if token["nf"] is not None else ""
                     else:
                         if token["tx"]:
                             region["l"] = len(token["tx"])
                         else:
                             region["l"] = 0
 
-                        token_text = token["tx"]
+                        token_text = token["tx"] if token["tx"] is not None else ""
 
                     # don't add the tokens corresponding to the first part of a hyphenated word
                     if "hy" not in token:
                         next_token = (
                             line["t"][n + 1]["tx"] if n != len(line["t"]) - 1 else None
                         )
                         ws = insert_whitespace(
@@ -146,15 +158,15 @@
 
                     coordinates["tokens"].append(region)
 
     return (string, coordinates, offsets)
 
 
 def rebuild_text_passim(
-    page: list[dict], language: str | None, string: str | None = None
+    page: list[dict], language: Optional[str], string: Optional[str] = None
 ) -> tuple[str, list[dict]]:
     """The text rebuilding function from pages for passim.
 
     If `string` is not `None`, then the rebuilt text is appended to it.
 
     Args:
         page (list[dict]): Newspaper page conforming to the impresso JSON pages schema.
@@ -169,24 +181,30 @@
 
     if string is None:
         string = ""
 
     # in order to be able to keep line break information
     # we iterate over a list of lists (lines of tokens)
 
-    for region_n, region in enumerate(page):
+    for region in page:
 
-        for i, para in enumerate(region["p"]):
+        for para in region["p"]:
 
             for line in para["l"]:
 
                 for n, token in enumerate(line["t"]):
 
                     region_string = ""
 
+                    if "c" not in token:
+                        # if the coordniates are missing, they should be skipped
+                        logger.debug("Missing 'c' in token %s", token)
+                        print(f"Missing 'c' in token {token}")
+                        continue
+
                     # each page region is a token
                     output_region = {
                         "start": None,
                         "length": None,
                         "coords": {
                             "x": token["c"][0],
                             "y": token["c"][1],
@@ -198,15 +216,15 @@
                     if len(string) == 0:
                         output_region["start"] = 0
                     else:
                         output_region["start"] = len(string)
 
                     # if token is the last in a line
                     if n == len(line["t"]) - 1:
-                        tmp = "{}\n".format(token["tx"])
+                        tmp = f"{token['tx']}\n"
                         region_string += tmp
                     else:
                         ws = insert_whitespace(
                             token["tx"],
                             next_t=line["t"][n + 1]["tx"],
                             prev_t=line["t"][n - 1]["tx"] if n != 0 else None,
                             lang=language,
@@ -237,16 +255,15 @@
 
     article_id = content_item["m"]["id"]
     logger.debug("Started rebuilding article %s", article_id)
 
     issue_id = "-".join(article_id.split("-")[:-1])
 
     page_file_names = {
-        p: "{}-p{}.json".format(issue_id, str(p).zfill(4))
-        for p in content_item["m"]["pp"]
+        p: f"{issue_id}-p{str(p).zfill(4)}.json" for p in content_item["m"]["pp"]
     }
 
     year, month, day, _, ci_num = article_id.split("-")[1:]
     d = datetime.date(int(year), int(month), int(day))
 
     raw_type = content_item["m"]["tp"]
 
@@ -323,25 +340,22 @@
 
     Args:
         content_item (dict[str, Any]): The content-item to rebuilt using its metadata.
 
     Returns:
         dict[str, Any]: The rebuilt content-item built for passim.
     """
-    np, date, edition, ci_type, ci_number, ext = parse_canonical_filename(
-        content_item["m"]["id"]
-    )
+    np, date, _, _, _, _ = parse_canonical_filename(content_item["m"]["id"])
 
     article_id = content_item["m"]["id"]
     logger.debug("Started rebuilding article %s", article_id)
     issue_id = "-".join(article_id.split("-")[:-1])
 
     page_file_names = {
-        p: "{}-p{}.json".format(issue_id, str(p).zfill(4))
-        for p in content_item["m"]["pp"]
+        p: f"{issue_id}-p{str(p).zfill(4)}.json" for p in content_item["m"]["pp"]
     }
 
     article_lang = content_item["m"]["l"] if "l" in content_item["m"] else None
 
     passim_document = {
         "series": np,
         "date": f"{date[0]}-{date[1]}-{date[2]}",
@@ -393,35 +407,37 @@
         `sort_key` is expected to be the concatenation of newspaper ID and year
         (e.g. GDL-1900).
     """
 
     newspaper, year = key.split("-")
     filename = f"{newspaper}-{year}.jsonl.bz2"
     filepath = os.path.join(output_dir, filename)
-    logger.info(f"Compressing {len(json_files)} JSON files into {filepath}")
+    logger.info("Compressing %s JSON files into %s", len(json_files), filepath)
     print(f"Compressing {len(json_files)} JSON files into {filepath}")
 
     with smart_open(filepath, "wb") as fout:
         writer = jsonlines.Writer(fout)
 
         for json_file in json_files:
-            with open(json_file, "r") as inpf:
+            with open(json_file, "r", encoding="utf-8") as inpf:
                 reader = jsonlines.Reader(inpf)
                 articles = list(reader)
                 writer.write_all(articles)
-            logger.info(f"Written {len(articles)} docs from {json_file} to {filepath}")
+            logger.info(
+                "Written %s docs from %s to %s", len(articles), json_file, filepath
+            )
 
         writer.close()
 
     for json_file in json_files:
         os.remove(json_file)
 
     temp_dir = os.path.dirname(json_files[0])
     os.rmdir(temp_dir)
-    logger.info(f"Removed temporary directory and files in {temp_dir}")
+    logger.info("Removed temporary directory and files in %s", temp_dir)
 
     return (key, filepath)
 
 
 def upload(sort_key, filepath, bucket_name=None):
     """Uploads a file to a given S3 bucket.
 
@@ -437,25 +453,29 @@
     .. note::
 
         `sort_key` is expected to be the concatenation of newspaper ID and year
         (e.g. GDL-1900).
     """
     # create connection with bucket
     # copy contents to s3 key
-    newspaper, year = sort_key.split("-")
-    key_name = "{}/{}".format(newspaper, os.path.basename(filepath))
+    newspaper, _ = sort_key.split("-")
+    key_name = f"{newspaper}/{os.path.basename(filepath)}"
+    if "/" in bucket_name:
+        # if the provided bucket also contains a partition, add it to the key name
+        bucket_name, partition = bucket_name.split("/")
+        key_name = f"{partition}/{key_name}"
     s3 = get_s3_resource()
     try:
         bucket = s3.Bucket(bucket_name)
         bucket.upload_file(filepath, key_name)
-        logger.info(f"Uploaded {filepath} to {key_name}")
+        logger.info("Uploaded %s to %s", filepath, key_name)
         return True, filepath
     except Exception as e:
         logger.error(e)
-        logger.error(f"The upload of {filepath} failed with error {e}")
+        logger.error("The upload of %s failed with error %s", filepath, e)
         return False, filepath
 
 
 def cleanup(upload_success, filepath):
     """Removes a file if it has been successfully uploaded to S3.
     :param upload_success: whether the upload was successful
     :type upload_success: bool
@@ -488,20 +508,20 @@
 
     :param article: input article
     :type article: dict
     :return: `True` or `False`
     :rtype: boolean
     """
     if article["has_problem"]:
-        logger.warning(f"Article {article['m']['id']} won't be rebuilt.")
+        logger.warning("Article %s won't be rebuilt.", article["m"]["id"])
     return not article["has_problem"]
 
 
 def rebuild_issues(
-    issues, input_bucket, output_dir, dask_client, format="solr", filter_language=None
+    issues, input_bucket, output_dir, dask_client, _format="solr", filter_language=None
 ):
     """Rebuild a set of newspaper issues into a given format.
 
     :param issues: issues to rebuild
     :type issues: list of `IssueDir` objects
     :param input_bucket: name of input s3 bucket
     :type input_bucket: str
@@ -515,84 +535,85 @@
         if not os.path.exists(path):
             pathlib.Path(path).mkdir(parents=True, exist_ok=True)
         else:
             for f in os.listdir(path):
                 os.remove(os.path.join(path, f))
 
     # determine which rebuild function to apply
-    if format == "solr":
+    if _format == "solr":
         rebuild_function = rebuild_for_solr
-    elif format == "passim":
+    elif _format == "passim":
         rebuild_function = rebuild_for_passim
     else:
         raise NotImplementedError
 
     # create a temporary output directory named after newspaper and year
     # e.g. IMP-1994
-    issue, issue_json = issues[0]
+    issue, _ = issues[0]
     key = f"{issue.journal}-{issue.date.year}"
     issue_dir = os.path.join(output_dir, key)
     mkdir(issue_dir)
 
-    print("Fleshing out articles by issue...")  # warning about large graph comes here
+    # warning about large graph comes here
+    print("Fleshing out articles by issue...")
     issues_bag = db.from_sequence(issues, partition_size=3)
 
     faulty_issues = (
         issues_bag.filter(lambda i: len(i[1]["pp"]) == 0)
         .map(lambda i: i[1])
         .pluck("id")
         .compute()
     )
-    logger.debug(f"Issues with no pages (will be skipped): {faulty_issues}")
-    print(f"Issues with no pages (will be skipped): {faulty_issues}")
+    msg = f"Issues with no pages (will be skipped): {faulty_issues}"
+    logger.debug(msg)
+    print(msg)
     del faulty_issues
-    logger.debug(f"Number of partitions: {issues_bag.npartitions}")
-    print(f"Number of partitions: {issues_bag.npartitions}")
+    msg = f"Number of partitions: {issues_bag.npartitions}"
+    logger.debug(msg)
+    print(msg)
 
     articles_bag = (
         issues_bag.filter(lambda i: len(i[1]["pp"]) > 0)
         .starmap(read_issue_pages, bucket=input_bucket)
         .starmap(rejoin_articles)
         .flatten()
         .persist()
     )
 
     faulty_articles_n = (
         articles_bag.filter(_article_has_problem).pluck("m").pluck("id").compute()
     )
-    logger.debug(f"Skipped articles: {faulty_articles_n}")
-    print(f"Skipped articles: {faulty_articles_n}")
+    msg = f"Skipped articles: {faulty_articles_n}"
+    logger.debug(msg)
+    print(msg)
     del faulty_articles_n
 
     articles_bag = (
         articles_bag.filter(_article_without_problem).map(rebuild_function).persist()
     )
 
     def has_language(ci):
         if "lg" not in ci:
             return False
-        else:
-            return ci["lg"] in filter_language
+        return ci["lg"] in filter_language
 
     if filter_language:
         filtered_articles = articles_bag.filter(has_language).persist()
         print(filtered_articles.count().compute())
-        result = filtered_articles.map(json.dumps).to_textfiles(
-            "{}/*.json".format(issue_dir)
-        )
+        stats_for_issues = compute_stats_in_rebuilt_bag(filtered_articles, key)
+        result = filtered_articles.map(json.dumps).to_textfiles(f"{issue_dir}/*.json")
     else:
-        result = articles_bag.map(json.dumps).to_textfiles(
-            "{}/*.json".format(issue_dir)
-        )
+        stats_for_issues = compute_stats_in_rebuilt_bag(articles_bag, key)
+        result = articles_bag.map(json.dumps).to_textfiles(f"{issue_dir}/*.json")
 
     dask_client.cancel(issues_bag)
     logger.info("done.")
     print("done.")
 
-    return (key, result)
+    return (key, result, stats_for_issues)
 
 
 def init_logging(level, file):
     """Initialises the root logger.
 
     :param level: desired level of logging (default: logging.INFO)
     :type level: int
@@ -619,129 +640,156 @@
     handler.setFormatter(formatter)
     root_logger.addHandler(handler)
     root_logger.info("Logger successfully initialised")
 
     return root_logger
 
 
-def main():
+def main() -> None:
 
-    def signal_handler(*args):
+    def signal_handler():
         # Handle any cleanup here
         print(
             "SIGINT or CTRL-C detected. Exiting gracefully"
             " and shutting down the dask local cluster"
         )
         client.shutdown()
-        exit(0)
+        sys.exit(0)
 
     arguments = docopt(__doc__)
     clear_output = arguments["--clear"]
     bucket_name = f's3://{arguments["--input-bucket"]}'
     output_bucket_name = arguments["--output-bucket"]
     outp_dir = arguments["--output-dir"]
     filter_config_file = arguments["--filter-config"]
     output_format = arguments["--format"]
     scheduler = arguments["--scheduler"]
     log_file = arguments["--log-file"]
     nworkers = arguments["--nworkers"] if arguments["--nworkers"] else 8
     log_level = logging.DEBUG if arguments["--verbose"] else logging.INFO
     languages = arguments["--languages"]
+    repo_path = arguments["--git-repo"]
+    temp_dir = arguments["--temp-dir"]
+    prev_manifest_path = (
+        arguments["--prev-manifest"] if arguments["--prev-manifest"] else None
+    )
 
     signal.signal(signal.SIGINT, signal_handler)
 
     if languages:
         languages = languages.split(",")
 
     init_logging(log_level, log_file)
 
     # clean output directory if existing
     if outp_dir is not None and os.path.exists(outp_dir):
         if clear_output is not None and clear_output:
             shutil.rmtree(outp_dir)
             os.mkdir(outp_dir)
 
-    with open(filter_config_file, "r") as file:
+    with open(filter_config_file, "r", encoding="utf-8") as file:
         config = json.load(file)
 
     # start the dask local cluster
     if scheduler is None:
         client = Client(n_workers=nworkers, threads_per_worker=1)
     else:
-        cluster = None
         client = Client(scheduler)
-    logger.info(f"Dask local cluster: {client}")
-    print(f"Dask local cluster: {client}")
+
+    dask_cluster_msg = f"Dask local cluster: {client}"
+    logger.info(dask_cluster_msg)
+    print(dask_cluster_msg)
+
+    # the created manifest is not the same based on the output format
+    data_stage = "rebuilt" if output_format == "solr" else "passim"
+
+    # initialize manifest
+    manifest = DataManifest(
+        data_stage=data_stage,
+        s3_output_bucket=output_bucket_name,
+        s3_input_bucket=bucket_name,
+        git_repo=git.Repo(repo_path),
+        temp_dir=temp_dir,
+        previous_mft_path=prev_manifest_path if prev_manifest_path != "" else None,
+    )
+    titles = set()
 
     if arguments["rebuild_articles"]:
 
         try:
             for n, batch in enumerate(config):
                 rebuilt_issues = []
-                logger.info(f"Processing batch {n + 1}/{len(config)} [{batch}]")
-                print(f"Processing batch {n + 1}/{len(config)} [{batch}]")
+                proc_b_msg = f"Processing batch {n + 1}/{len(config)} [{batch}]"
+                logger.info(proc_b_msg)
+                print(proc_b_msg)
                 newspaper = list(batch.keys())[0]
                 start_year, end_year = batch[newspaper]
 
                 for year in range(start_year, end_year):
-                    logger.info(f"Processing year {year}")
-                    logger.info("Retrieving issues...")
-                    print(f"Processing year {year}")
-                    print("Retrieving issues...")
+                    proc_year_msg = f"Processing year {year} \nRetrieving issues..."
+                    logger.info(proc_year_msg)
+                    print(proc_year_msg)
+
                     try:
                         input_issues = read_s3_issues(newspaper, year, bucket_name)
                     except FileNotFoundError:
-                        logger.info(f"{newspaper}-{year} not found in {bucket_name}")
-                        print(f"{newspaper}-{year} not found in {bucket_name}")
+                        fnf_msg = f"{newspaper}-{year} not found in {bucket_name}"
+                        logger.info(fnf_msg)
+                        print(fnf_msg)
                         continue
 
-                    issue_key, json_files = rebuild_issues(
+                    issue_key, json_files, year_stats = rebuild_issues(
                         issues=input_issues,
                         input_bucket=bucket_name,
                         output_dir=outp_dir,
                         dask_client=client,
-                        format=output_format,
+                        _format=output_format,
                         filter_language=languages,
                     )
                     rebuilt_issues.append((issue_key, json_files))
                     del input_issues
-                logger.info(
-                    (
-                        f"Uploading {len(rebuilt_issues)} rebuilt bz2files "
-                        f"to {output_bucket_name}"
-                    )
-                )
-                print(
-                    (
-                        f"Uploading {len(rebuilt_issues)} rebuilt bz2files "
-                        f"to {output_bucket_name}"
-                    )
+
+                    logger.debug("year_stats: %s", year_stats)
+                    manifest.add_by_title_year(newspaper, year, year_stats[0])
+                    titles.add(newspaper)
+
+                msg = (
+                    f"Uploading {len(rebuilt_issues)} rebuilt bz2files "
+                    f"to {output_bucket_name}"
                 )
+                logger.info(msg)
+                print(msg)
+
                 b = (
                     db.from_sequence(rebuilt_issues)
                     .starmap(compress, output_dir=outp_dir)
                     .starmap(upload, bucket_name=output_bucket_name)
                     .starmap(cleanup)
                 )
                 future = b.persist()
                 progress(future)
                 # clear memory of objects once computations are done
                 client.restart()
-                print(f"Restarted client after finishing processing batch {n + 1}")
-                logger.info(
-                    f"Restarted client after finishing processing batch {n + 1}"
-                )
+                rstrt_msg = f"Restarted client after finishing processing batch {n + 1}"
+                print(rstrt_msg)
+                logger.info(rstrt_msg)
 
         except Exception as e:
             traceback.print_tb(e.__traceback__)
             print(e)
             client.shutdown()
         finally:
             client.shutdown()
 
+        manifest_note = f"Rebuilt of newspaper articles for {list(titles)}."
+        manifest.append_to_notes(manifest_note)
+        # finalize and compute the manifest
+        manifest.compute(export_to_git_and_s3=False)
+        manifest.validate_and_export_manifest(push_to_git=False)
+
         logger.info("---------- Done ----------")
         print("---------- Done ----------")
 
     elif arguments["rebuild_pages"]:
         print("\nFunction not yet implemented (sorry!).\n")
```

### Comparing `impresso_commons-1.0.2/impresso_commons/utils/__init__.py` & `impresso_commons-1.1.0/impresso_commons/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `impresso_commons-1.0.2/impresso_commons/utils/config_loader.py` & `impresso_commons-1.1.0/impresso_commons/utils/config_loader.py`

 * *Files identical despite different names*

### Comparing `impresso_commons-1.0.2/impresso_commons/utils/daskutils.py` & `impresso_commons-1.1.0/impresso_commons/utils/daskutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 Usage:
     daskutils.py partition --config-file=<cf> --nb-partitions=<p> [--log-file=<f> --verbose]
 
 Options:
     --config-file=<cf>  json configuration dict specifying various arguments
 """
 
+import os
 import logging
 import docopt
-import os
 
 from dask.diagnostics import ProgressBar
 import dask.bag as db
 import numpy as np
 
 from impresso_commons.utils import init_logger
-from impresso_commons.utils import Timer, user_confirmation
+from impresso_commons.utils import Timer
 from impresso_commons.path.path_s3 import s3_filter_archives
 from impresso_commons.utils.s3 import get_bucket, read_jsonlines, readtext_jsonlines
 from impresso_commons.utils.s3 import IMPRESSO_STORAGEOPT
 from impresso_commons.utils.config_loader import PartitionerConfig
 
 __author__ = "maudehrmann"
 
@@ -36,20 +36,22 @@
     grouped_items = bag.groupby(lambda x: np.random.randint(500), npartitions=nbpart)
     items = grouped_items.map(lambda x: x[1]).flatten()
     path = os.path.join(path, "*.jsonl.bz2")
     with ProgressBar():
         items.to_textfiles(path)
 
 
-def create_even_partitions(bucket,
-                           config_newspapers,
-                           output_dir,
-                           local_fs=False,
-                           keep_full=False,
-                           nb_partition=500):
+def create_even_partitions(
+    bucket,
+    config_newspapers,
+    output_dir,
+    local_fs=False,
+    keep_full=False,
+    nb_partition=500,
+):
     """Convert yearly bz2 archives to even bz2 archives, i.e. partitions.
 
     Enables efficient (distributed) processing, bypassing the size discrepancies of newspaper archives.
     N.B.: in resulting partitions articles are all shuffled.
     Warning: consider well the config_newspapers as it decides what will be in the partitions and loaded in memory.
 
     :param bucket: name of the bucket where the files to partition are
@@ -64,40 +66,42 @@
     t = Timer()
 
     # set the output
     if local_fs:
         os.makedirs(output_dir, exist_ok=True)
         path = os.path.join(output_dir, "*.jsonl.bz2")
     else:
-        path = f'{output_dir}/*.jsonl.gz'
+        path = f"{output_dir}/*.jsonl.gz"
     logger.info(f"Will write partitions to {path}")
 
     # collect (yearly) keys & load in bag
     bz2_keys = s3_filter_archives(bucket.name, config=config_newspapers)
     bag_bz2_keys = db.from_sequence(bz2_keys)
 
     # read and filter lines (1 elem = list of lines, or articles, from a key)
     if keep_full is False:
-        bag_items = bag_bz2_keys.map(readtext_jsonlines, bucket_name=bucket.name).flatten()
+        bag_items = bag_bz2_keys.map(
+            readtext_jsonlines, bucket_name=bucket.name
+        ).flatten()
     else:
         bag_items = bag_bz2_keys.map(read_jsonlines, bucket_name=bucket.name).flatten()
 
     # repartition evenly
-    grouped_items = bag_items.groupby(lambda x: np.random.randint(1000), npartitions=nb_partition)
+    grouped_items = bag_items.groupby(
+        lambda x: np.random.randint(1000), npartitions=nb_partition
+    )
     items = grouped_items.map(lambda x: x[1]).flatten()
 
     # write partitions
     with ProgressBar():
         # items.compute()
         # if local_fs:
         #     items.to_textfiles(path)
         # else:
-        items.to_textfiles(path,
-                           storage_options=IMPRESSO_STORAGEOPT,
-                           compute=True)
+        items.to_textfiles(path, storage_options=IMPRESSO_STORAGEOPT, compute=True)
 
     logger.info(f"Partitioning done in {t.stop()}.")
 
 
 def main(args):
     # get args
     config_file = args["--config-file"]
@@ -112,18 +116,20 @@
 
     config = PartitionerConfig.from_json(config_file)
 
     bucket = get_bucket(config.bucket_name, create=False)
     logger.info(f"Retrieved bucket: {bucket.name}")
 
     if args["partition"] is True:
-        create_even_partitions(bucket,
-                               config.newspapers,
-                               config.output_dir,
-                               local_fs=config.local_fs,
-                               keep_full=config.keep_full,
-                               nb_partition=int(nb_partitions))
+        create_even_partitions(
+            bucket,
+            config.newspapers,
+            config.output_dir,
+            local_fs=config.local_fs,
+            keep_full=config.keep_full,
+            nb_partition=int(nb_partitions),
+        )
 
 
 if __name__ == "__main__":
     arguments = docopt.docopt(__doc__)
     main(arguments)
```

### Comparing `impresso_commons-1.0.2/impresso_commons/utils/s3.py` & `impresso_commons-1.1.0/impresso_commons/utils/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 
 """
 
 import os
 import logging
 import json
 import warnings
-
-import boto3
 import bz2
+from typing import Union
+import boto3
 from smart_open.s3 import iter_bucket
 from smart_open import open as s_open
 from dotenv import load_dotenv
+import botocore
 
 from impresso_commons.utils import _get_cores
 
-
 logger = logging.getLogger(__name__)
 
 
 def get_storage_options():
     # load environment variables from local .env files
     load_dotenv()
     return {
@@ -392,17 +392,20 @@
                     or k == "pp"
                     or k == "lg"
                     or k == "t"
                 }
                 yield json.dumps(article_reduced)
 
 
-def upload(partition_name, newspaper_prefix, bucket_name=None):
+def upload(partition_name, newspaper_prefix=None, bucket_name=None):
 
-    key_name = os.path.join("/", newspaper_prefix, partition_name.split("/")[-1])
+    if newspaper_prefix is not None:
+        key_name = os.path.join("/", newspaper_prefix, partition_name.split("/")[-1])
+    else:
+        key_name = partition_name.split("/")[-1]
     s3 = get_s3_resource()
     try:
         bucket = s3.Bucket(bucket_name)
         logger.info(bucket.name)
         bucket.upload_file(partition_name, key_name)
         logger.info(f"Uploaded {partition_name} to {key_name}")
         return True, partition_name
@@ -465,15 +468,17 @@
         )  # prepend bucket-name as it is necessary for s3fs
         for o in boto3_bucket.objects.filter(Prefix=base_path)
         if o.key.endswith(suffix_path)
     ]
     return filenames
 
 
-def alternative_read_text(s3_key, s3_credentials):
+def alternative_read_text(
+    s3_key: str, s3_credentials: dict, line_by_line: bool = True
+) -> Union[list[str], str]:
     """Read from S3 a line-separated text file (e.g. `*.jsonl.bz2`).
 
     Note:
         The reason for this function is a bug in `dask.bag.read_text()`
         which breaks on buckets having >= 1000 keys.
         It raises a `FileNotFoundError`.
     """
@@ -483,11 +488,38 @@
         aws_secret_access_key=s3_credentials["secret"],
     )
     s3_endpoint = s3_credentials["client_kwargs"]["endpoint_url"]
     transport_params = {
         "client": session.client("s3", endpoint_url=s3_endpoint),
     }
 
-    with s_open(s3_key, "r", transport_params=transport_params) as infile:
-        lines = infile.readlines()
+    if line_by_line:
+        with s_open(s3_key, "r", transport_params=transport_params) as infile:
+            text = infile.readlines()
+    else:
+        with s_open(s3_key, "r", transport_params=transport_params) as infile:
+            text = infile.read()
+
+    return text
+
 
-    return lines
+def get_s3_object_size(bucket_name, key):
+    """
+    Get the size of an object (key) in an S3 bucket.
+
+    Args:
+        bucket_name (str): The name of the S3 bucket.
+        key (str): The key (object) whose size you want to retrieve.
+
+    Returns:
+        int: The size of the object in bytes, or None if the object doesn't exist.
+    """
+    s3_client = get_s3_client()
+
+    try:
+        # Get the object metadata to retrieve its size
+        response = s3_client.head_object(Bucket=bucket_name, Key=key)
+        size = response["ContentLength"]
+        return int(size)
+    except botocore.exceptions.ClientError as err:
+        logger.error(f"Error: {err} for {key} in {bucket_name}")
+        return None
```

### Comparing `impresso_commons-1.0.2/impresso_commons/utils/s3_delete.py` & `impresso_commons-1.1.0/impresso_commons/utils/s3_delete.py`

 * *Files identical despite different names*

### Comparing `impresso_commons-1.0.2/impresso_commons/utils/uima.py` & `impresso_commons-1.1.0/impresso_commons/utils/uima.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Utility functions to export data in Apache UIMA XMI format."""
 
 import os
 import json
-from typing import Dict, Tuple, List
+from typing import Dict, List
 
 from dask import bag as db
-from cassis import load_cas_from_xmi, load_typesystem, Cas
+from cassis import load_typesystem, Cas
 
 
 from impresso_commons.utils.s3 import IMPRESSO_STORAGEOPT
 from impresso_commons.classes import ContentItem
 from impresso_commons.images.olive_boxes import get_iiif_url
 
-IMPRESSO_IIIF_ENDPOINT = 'https://dhlabsrv17.epfl.ch/iiif_impresso/'
+IMPRESSO_IIIF_ENDPOINT = "https://dhlabsrv17.epfl.ch/iiif_impresso/"
 # IMPRESSO_IIIF_ENDPOINT = 'http://pub.cl.uzh.ch/service/iiif_impresso'
 
 
 def compute_image_links(
     ci: ContentItem,
     padding: int = 20,
     iiif_endpoint: str = IMPRESSO_IIIF_ENDPOINT,
@@ -41,75 +41,79 @@
         start_offset = break_offset
 
         tokens = ci.get_coordinates(start, end)
 
         if len(tokens) == 0:
             continue
 
-        page_id = tokens[0]['page_id']
+        page_id = tokens[0]["page_id"]
 
-        if 'hy1' in tokens[0] and len(tokens) > 1:
+        if "hy1" in tokens[0] and len(tokens) > 1:
             first_token = tokens[1]
         else:
             first_token = tokens[0]
 
         last_token = tokens[-1]
 
         if line_n + 1 < len(ci.lines):
             next_offset = ci.lines[line_n + 1]
             next_line_tokens = ci.get_coordinates(start_offset, next_offset)
 
-            if len(next_line_tokens) > 0 and 'hy1' in next_line_tokens[0]:
+            if len(next_line_tokens) > 0 and "hy1" in next_line_tokens[0]:
                 last_token = next_line_tokens[0]
             else:
                 last_token = tokens[-1]
 
         # compute box coordinates of line
-        x1, y1, w1, h1 = first_token['coords']
-        x2, y2, w2, h2 = last_token['coords']
+        x1, y1, w1, h1 = first_token["coords"]
+        x2, y2, w2, h2 = last_token["coords"]
         x3, y3, w3, h3 = x1, y1 - padding, w2 + (x2 - x1), h1 + padding
         box = " ".join([str(coord) for coord in [x3, y3, w3, h3]])
         if iiif_links is None:
             iiif_link = get_iiif_url(page_id, box, IMPRESSO_IIIF_ENDPOINT, pct)
         else:
-            iiif_link = get_iiif_url(page_id, box, iiif_manifest_uri=iiif_links[page_id], pct=pct)
+            iiif_link = get_iiif_url(
+                page_id, box, iiif_manifest_uri=iiif_links[page_id], pct=pct
+            )
         image_links.append((iiif_link, start, end))
 
     return image_links
 
 
 def get_iiif_links(contentitems: List[ContentItem], canonical_bucket: str):
     """Retrieves from S3 IIIF links for a set of canonical pages where the input content items are found."""
 
     # derive the IDs of all issues involved
-    issue_ids = set(["-".join(ci.id.split('-')[:-1]) for ci in contentitems])
+    issue_ids = set(["-".join(ci.id.split("-")[:-1]) for ci in contentitems])
 
     # reconstruct S3 links to canonical pages
     page_files = [
         os.path.join(
             canonical_bucket,
-            issue_id.split('-')[0],
+            issue_id.split("-")[0],
             "pages",
             f"{issue_id.split('-')[0]}-{issue_id.split('-')[1]}",
             f"{issue_id}-pages.jsonl.bz2",
         )
         for issue_id in issue_ids
     ]
 
     iiif_links = (
         db.read_text(page_files, storage_options=IMPRESSO_STORAGEOPT)
         .map(json.loads)
-        .map(lambda x: (x['id'], x['iiif']))
+        .map(lambda x: (x["id"], x["iiif"]))
         .compute()
     )
 
     return {page_id: iiif_link for page_id, iiif_link in iiif_links}
 
 
-def rebuilt2xmi(ci, output_dir, typesystem_path, iiif_mappings, pct_coordinates=False) -> str:
+def rebuilt2xmi(
+    ci, output_dir, typesystem_path, iiif_mappings, pct_coordinates=False
+) -> str:
     """
     Converts a rebuilt ContentItem into Apache UIMA/XMI format.
 
     The resulting file will be named after the content item's ID, adding
     the `.xmi` extension.
 
     :param ci: the content item to be converted
@@ -122,18 +126,18 @@
     """
 
     with open(typesystem_path, "rb") as f:
         typesystem = load_typesystem(f)
 
     cas = Cas(typesystem=typesystem)
     cas.sofa_string = ci.fulltext
-    cas.sofa_mime = 'text/plain'
+    cas.sofa_mime = "text/plain"
 
-    sentType = 'de.tudarmstadt.ukp.dkpro.core.api.segmentation.type.Sentence'
-    imgLinkType = 'webanno.custom.ImpressoImages'
+    sentType = "de.tudarmstadt.ukp.dkpro.core.api.segmentation.type.Sentence"
+    imgLinkType = "webanno.custom.ImpressoImages"
     Sentence = typesystem.get_type(sentType)
     ImageLink = typesystem.get_type(imgLinkType)
 
     # create sentence-level annotations
     start_offset = 0
     for break_offset in ci.lines:
         start = start_offset
@@ -143,10 +147,10 @@
 
     iiif_links = compute_image_links(ci, iiif_links=iiif_mappings, pct=pct_coordinates)
 
     # inject the IIIF links into
     for iiif_link, start, end in iiif_links:
         cas.add_annotation(ImageLink(begin=start, end=end, link=iiif_link))
 
-    outfile_path = os.path.join(output_dir, f'{ci.id}.xmi')
+    outfile_path = os.path.join(output_dir, f"{ci.id}.xmi")
     cas.to_xmi(outfile_path, pretty_print=True)
     return outfile_path
```

### Comparing `impresso_commons-1.0.2/impresso_commons/versioning/manifest_0.py` & `impresso_commons-1.1.0/impresso_commons/versioning/manifest_0.py`

 * *Files identical despite different names*

### Comparing `impresso_commons-1.0.2/impresso_commons/versioning/rebuilt_manifest_0.py` & `impresso_commons-1.1.0/impresso_commons/versioning/rebuilt_manifest_0.py`

 * *Files identical despite different names*

### Comparing `impresso_commons-1.0.2/impresso_commons.egg-info/SOURCES.txt` & `impresso_commons-1.1.0/impresso_commons.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
+requirements.txt
 setup.py
 impresso_commons/__init__.py
 impresso_commons.egg-info/PKG-INFO
 impresso_commons.egg-info/SOURCES.txt
 impresso_commons.egg-info/dependency_links.txt
 impresso_commons.egg-info/entry_points.txt
 impresso_commons.egg-info/requires.txt
@@ -17,14 +18,22 @@
 impresso_commons/data/config/conf.json
 impresso_commons/data/config/conf2.json
 impresso_commons/data/config/patch_rebuilt_1.json
 impresso_commons/data/config/patch_rebuilt_2.json
 impresso_commons/data/config/patch_rebuilt_3.json
 impresso_commons/data/config/patch_rebuilt_4.json
 impresso_commons/data/config/patch_rebuilt_5.json
+impresso_commons/data/config/patch_rebuilt_6.json
+impresso_commons/data/config/patch_rebuilt_7.json
+impresso_commons/data/config/patch_rebuilt_8.json
+impresso_commons/data/config/patch_rebuilt_9.json
+impresso_commons/data/config/rebuilt_passim.json
+impresso_commons/data/config/rebuilt_passim_1.json
+impresso_commons/data/config/rebuilt_passim_2.json
+impresso_commons/data/config/rebuilt_passim_3.json
 impresso_commons/data/config/remaining_nps.json
 impresso_commons/data/xmi/typesystem.xml
 impresso_commons/images/__init__.py
 impresso_commons/images/img_utils.py
 impresso_commons/images/olive_boxes.py
 impresso_commons/path/__init__.py
 impresso_commons/path/path_fs.py
@@ -50,11 +59,16 @@
 impresso_commons/utils/__init__.py
 impresso_commons/utils/config_loader.py
 impresso_commons/utils/daskutils.py
 impresso_commons/utils/s3.py
 impresso_commons/utils/s3_delete.py
 impresso_commons/utils/uima.py
 impresso_commons/utils/utils.py
+impresso_commons/versioning/__init__.py
+impresso_commons/versioning/compute_manifest.py
+impresso_commons/versioning/data_manifest.py
+impresso_commons/versioning/data_statistics.py
+impresso_commons/versioning/helpers.py
 impresso_commons/versioning/manifest_0.py
 impresso_commons/versioning/rebuilt_manifest_0.py
 tests/test_path_s3.py
 tests/test_rebuilder.py
```

### Comparing `impresso_commons-1.0.2/pyproject.toml` & `impresso_commons-1.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools>=68.2.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "impresso_commons"
 authors = [
     {name="Maud Ehrmann", email="maud.ehrmann@epfl.ch"},
     {name="Matteo Romanello", email="matteo.romanello@gmail.com"}
@@ -19,40 +19,25 @@
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-dynamic = ["version"]
+dynamic = ["version","dependencies"]
+
 
-dependencies = [
-    "dask[complete]",
-    "boto3",
-    "beautifulsoup4",
-    "docopt",
-    "deprecated",
-    "dkpro-cassis",
-    "scikit-build",
-    "cmake",
-    "opencv-python",
-    "numpy",
-    "smart_open",
-    "jsonlines",
-    "s3fs",
-    "python-dotenv"
-]
 
 [project.urls]
 Homepage = "https://github.com/impresso/impresso-pycommons"
 Documentaton = "https://impresso-pycommons.readthedocs.io/en/latest/" 
 
 [tool.setuptools.dynamic]
 version = {attr = "impresso_commons.__version__"}
-
+dependencies = {file = ["requirements.txt"]}
 [tool.setuptools.packages.find]
 include = ["impresso_commons*"]
 namespaces = false
 
 [tool.setuptools.package-data]
 impresso_commons = [
     "data/xmi/*.xml",
```

### Comparing `impresso_commons-1.0.2/tests/test_path_s3.py` & `impresso_commons-1.1.0/tests/test_path_s3.py`

 * *Files identical despite different names*

### Comparing `impresso_commons-1.0.2/tests/test_rebuilder.py` & `impresso_commons-1.1.0/tests/test_rebuilder.py`

 * *Files identical despite different names*

