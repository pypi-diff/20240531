# Comparing `tmp/metloom-0.4.3.tar.gz` & `tmp/metloom-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metloom-0.4.3.tar", last modified: Wed May 22 22:32:57 2024, max compression
+gzip compressed data, was "metloom-0.5.0.tar", last modified: Fri May 31 17:28:31 2024, max compression
```

## Comparing `metloom-0.4.3.tar` & `metloom-0.5.0.tar`

### file list

```diff
@@ -1,84 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:32:57.140506 metloom-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-22 22:32:52.000000 metloom-0.4.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-22 22:32:52.000000 metloom-0.4.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-22 22:32:52.000000 metloom-0.4.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-22 22:32:52.000000 metloom-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-22 22:32:52.000000 metloom-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-05-22 22:32:57.140506 metloom-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-05-22 22:32:52.000000 metloom-0.4.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:32:57.128506 metloom-0.4.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-22 22:32:52.000000 metloom-0.4.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-22 22:32:52.000000 metloom-0.4.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-22 22:32:52.000000 metloom-0.4.3/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     5069 2024-05-22 22:32:52.000000 metloom-0.4.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-22 22:32:52.000000 metloom-0.4.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-22 22:32:52.000000 metloom-0.4.3/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-22 22:32:52.000000 metloom-0.4.3/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-22 22:32:52.000000 metloom-0.4.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-22 22:32:52.000000 metloom-0.4.3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-22 22:32:52.000000 metloom-0.4.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 22:32:52.000000 metloom-0.4.3/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-22 22:32:52.000000 metloom-0.4.3/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:32:57.128506 metloom-0.4.3/metloom/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-22 22:32:52.000000 metloom-0.4.3/metloom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-22 22:32:52.000000 metloom-0.4.3/metloom/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-22 22:32:52.000000 metloom-0.4.3/metloom/dataframe_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:32:57.132506 metloom-0.4.3/metloom/pointdata/
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-22 22:32:52.000000 metloom-0.4.3/metloom/pointdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9299 2024-05-22 22:32:52.000000 metloom-0.4.3/metloom/pointdata/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    16704 2024-05-22 22:32:52.000000 metloom-0.4.3/metloom/pointdata/cdec.py
--rw-r--r--   0 runner    (1001) docker     (127)    14252 2024-05-22 22:32:52.000000 metloom-0.4.3/metloom/pointdata/geosphere_austria.py
--rw-r--r--   0 runner    (1001) docker     (127)    13801 2024-05-22 22:32:52.000000 metloom-0.4.3/metloom/pointdata/mesowest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13870 2024-05-22 22:32:52.000000 metloom-0.4.3/metloom/pointdata/snotel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-05-22 22:32:52.000000 metloom-0.4.3/metloom/pointdata/snotel_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-05-22 22:32:52.000000 metloom-0.4.3/metloom/pointdata/usgs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-22 22:32:52.000000 metloom-0.4.3/metloom/request_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-05-22 22:32:52.000000 metloom-0.4.3/metloom/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:32:57.140506 metloom-0.4.3/metloom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-05-22 22:32:57.000000 metloom-0.4.3/metloom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-22 22:32:57.000000 metloom-0.4.3/metloom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 22:32:57.000000 metloom-0.4.3/metloom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-22 22:32:57.000000 metloom-0.4.3/metloom.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 22:32:56.000000 metloom-0.4.3/metloom.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-22 22:32:57.000000 metloom-0.4.3/metloom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 22:32:57.000000 metloom-0.4.3/metloom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-22 22:32:57.140506 metloom-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-22 22:32:52.000000 metloom-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:32:57.136506 metloom-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:32:57.136506 metloom-0.4.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/austria_box.cpg
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/austria_box.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/austria_box.prj
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/austria_box.shp
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/austria_box.shx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:32:57.136506 metloom-0.4.3/tests/data/cdec_mocks/
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/cdec_mocks/raw_tny_locations.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:32:57.140506 metloom-0.4.3/tests/data/geosphere_mocks/
--rw-r--r--   0 runner    (1001) docker     (127)   287245 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/geosphere_mocks/klima_mock.json
--rw-r--r--   0 runner    (1001) docker     (127)   104970 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/geosphere_mocks/meta_mock.json
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/testing.cpg
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/testing.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/testing.prj
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/testing.shp
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/testing.shx
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/triangle.cpg
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/triangle.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/triangle.prj
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/triangle.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/triangle.shp
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/triangle.shx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:32:57.140506 metloom-0.4.3/tests/data/usgs_mocks/
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/usgs_mocks/daily_response.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10027 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/usgs_mocks/hourly_response.json
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/usgs_mocks/platoro_meta.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/data/usgs_mocks/station_search_response.txt
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/shp_to_boxshp.py
--rw-r--r--   0 runner    (1001) docker     (127)    23328 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/test_cdec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6377 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/test_dataframe_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/test_geosphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    13375 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/test_mesowest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/test_point_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    15999 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/test_snotel.py
--rw-r--r--   0 runner    (1001) docker     (127)     9142 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/test_usgs.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-22 22:32:52.000000 metloom-0.4.3/tests/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:28:31.257476 metloom-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-31 17:28:26.000000 metloom-0.5.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-31 17:28:26.000000 metloom-0.5.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-31 17:28:26.000000 metloom-0.5.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-31 17:28:26.000000 metloom-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-31 17:28:26.000000 metloom-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-05-31 17:28:31.257476 metloom-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-05-31 17:28:26.000000 metloom-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:28:31.245476 metloom-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-31 17:28:26.000000 metloom-0.5.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-31 17:28:26.000000 metloom-0.5.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-31 17:28:26.000000 metloom-0.5.0/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5069 2024-05-31 17:28:26.000000 metloom-0.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-31 17:28:26.000000 metloom-0.5.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-31 17:28:26.000000 metloom-0.5.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-31 17:28:26.000000 metloom-0.5.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-31 17:28:26.000000 metloom-0.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-31 17:28:26.000000 metloom-0.5.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-31 17:28:26.000000 metloom-0.5.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-31 17:28:26.000000 metloom-0.5.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-31 17:28:26.000000 metloom-0.5.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:28:31.245476 metloom-0.5.0/metloom/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-31 17:28:26.000000 metloom-0.5.0/metloom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-31 17:28:26.000000 metloom-0.5.0/metloom/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-31 17:28:26.000000 metloom-0.5.0/metloom/dataframe_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:28:31.249476 metloom-0.5.0/metloom/pointdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-31 17:28:26.000000 metloom-0.5.0/metloom/pointdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9823 2024-05-31 17:28:26.000000 metloom-0.5.0/metloom/pointdata/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16704 2024-05-31 17:28:26.000000 metloom-0.5.0/metloom/pointdata/cdec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-05-31 17:28:26.000000 metloom-0.5.0/metloom/pointdata/cues.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14252 2024-05-31 17:28:26.000000 metloom-0.5.0/metloom/pointdata/geosphere_austria.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13801 2024-05-31 17:28:26.000000 metloom-0.5.0/metloom/pointdata/mesowest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18267 2024-05-31 17:28:26.000000 metloom-0.5.0/metloom/pointdata/norway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13870 2024-05-31 17:28:26.000000 metloom-0.5.0/metloom/pointdata/snotel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-05-31 17:28:26.000000 metloom-0.5.0/metloom/pointdata/snotel_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-05-31 17:28:26.000000 metloom-0.5.0/metloom/pointdata/usgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-31 17:28:26.000000 metloom-0.5.0/metloom/request_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13728 2024-05-31 17:28:26.000000 metloom-0.5.0/metloom/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:28:31.257476 metloom-0.5.0/metloom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-05-31 17:28:31.000000 metloom-0.5.0/metloom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-31 17:28:31.000000 metloom-0.5.0/metloom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 17:28:31.000000 metloom-0.5.0/metloom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-31 17:28:31.000000 metloom-0.5.0/metloom.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 17:28:31.000000 metloom-0.5.0/metloom.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-31 17:28:31.000000 metloom-0.5.0/metloom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-31 17:28:31.000000 metloom-0.5.0/metloom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-31 17:28:31.257476 metloom-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-31 17:28:26.000000 metloom-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:28:31.249476 metloom-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:28:31.253476 metloom-0.5.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/austria_box.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/austria_box.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/austria_box.prj
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/austria_box.shp
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/austria_box.shx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:28:31.253476 metloom-0.5.0/tests/data/cdec_mocks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/cdec_mocks/raw_tny_locations.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:28:31.253476 metloom-0.5.0/tests/data/cues_mocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/cues_mocks/daily_response.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/cues_mocks/hourly_response.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:28:31.253476 metloom-0.5.0/tests/data/frost_mocks/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/frost_mocks/box.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/frost_mocks/box.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/frost_mocks/box.prj
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/frost_mocks/box.shp
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/frost_mocks/box.shx
+-rw-r--r--   0 runner    (1001) docker     (127)    54938 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/frost_mocks/hourly_temp.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11372 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/frost_mocks/search.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:28:31.257476 metloom-0.5.0/tests/data/geosphere_mocks/
+-rw-r--r--   0 runner    (1001) docker     (127)   287245 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/geosphere_mocks/klima_mock.json
+-rw-r--r--   0 runner    (1001) docker     (127)   104970 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/geosphere_mocks/meta_mock.json
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/testing.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/testing.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/testing.prj
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/testing.shp
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/testing.shx
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/triangle.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/triangle.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/triangle.prj
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/triangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/triangle.shp
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/triangle.shx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:28:31.257476 metloom-0.5.0/tests/data/usgs_mocks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/usgs_mocks/daily_response.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10027 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/usgs_mocks/hourly_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/usgs_mocks/platoro_meta.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/data/usgs_mocks/station_search_response.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/shp_to_boxshp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23328 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/test_cdec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/test_cues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6377 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/test_dataframe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/test_frost.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11844 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/test_geosphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13375 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/test_mesowest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/test_point_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15999 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/test_snotel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9142 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/test_usgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-31 17:28:26.000000 metloom-0.5.0/tests/test_variables.py
```

### Comparing `metloom-0.4.3/CONTRIBUTING.rst` & `metloom-0.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/HISTORY.rst` & `metloom-0.5.0/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/LICENSE` & `metloom-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/PKG-INFO` & `metloom-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metloom
-Version: 0.4.3
+Version: 0.5.0
 Summary: Location Oriented Observed Meteorology (LOOM)
 Home-page: https://github.com/M3Works/metloom
 Author: M3Works
 Author-email: m3worksllc@gmail.com
 License: BSD license
 Keywords: metloom
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -67,14 +67,16 @@
 * Searching for stations from a datasource within a shapefile
 * Current data sources:
     * `CDEC <https://cdec.water.ca.gov/>`_
     * `SNOTEL <https://www.nrcs.usda.gov/wps/portal/wcc/home/dataAccessHelp/webService/webServiceReference/>`_
     * `MESOWEST <https://developers.synopticdata.com/mesonet/>`_
     * `USGS <https://waterservices.usgs.gov/rest/>`_
     * `GEOSPHERE AUSTRIA <https://data.hub.geosphere.at/dataset/>`_
+    * `UCSB CUES <https://snow.ucsb.edu/#>`_
+    * `MET NORWAY <https://frost.met.no/index.html>`_
 
 Requirements
 ------------
 python >= 3.7
 
 Install
 -------
```

### Comparing `metloom-0.4.3/README.rst` & `metloom-0.5.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 * Searching for stations from a datasource within a shapefile
 * Current data sources:
     * `CDEC <https://cdec.water.ca.gov/>`_
     * `SNOTEL <https://www.nrcs.usda.gov/wps/portal/wcc/home/dataAccessHelp/webService/webServiceReference/>`_
     * `MESOWEST <https://developers.synopticdata.com/mesonet/>`_
     * `USGS <https://waterservices.usgs.gov/rest/>`_
     * `GEOSPHERE AUSTRIA <https://data.hub.geosphere.at/dataset/>`_
+    * `UCSB CUES <https://snow.ucsb.edu/#>`_
+    * `MET NORWAY <https://frost.met.no/index.html>`_
 
 Requirements
 ------------
 python >= 3.7
 
 Install
 -------
```

### Comparing `metloom-0.4.3/docs/Makefile` & `metloom-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/docs/conf.py` & `metloom-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/docs/installation.rst` & `metloom-0.5.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/docs/make.bat` & `metloom-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/docs/usage.rst` & `metloom-0.5.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/metloom/cli.py` & `metloom-0.5.0/metloom/cli.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/metloom/dataframe_utils.py` & `metloom-0.5.0/metloom/dataframe_utils.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/metloom/pointdata/base.py` & `metloom-0.5.0/metloom/pointdata/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,25 @@
+import copy
 import logging
 from datetime import datetime
 from typing import List
 
 import pandas as pd
 
 import geopandas as gpd
 
 from ..variables import SensorDescription, VariableBase
 
 LOG = logging.getLogger("metloom.pointdata.base")
 
 
+class DataValidationError(RuntimeError):
+    pass
+
+
 class PointDataCollection:
     """
     Iterator class for a collection of PointData objects.
     This allows conversion to a GeoDataFrame
     """
 
     def __init__(self, points: List[object] = None):
@@ -246,21 +251,32 @@
         if gdf is None:
             return
         assert isinstance(gdf, gpd.GeoDataFrame)
         columns = gdf.columns
         index_names = gdf.index.names
         # check for required indexes
         for ei in cls.EXPECTED_INDICES:
-            assert ei in index_names
-        # check for expected columns
-        expected_columns = cls.EXPECTED_COLUMNS
-        if "measurementDate" in columns:
-            expected_columns = expected_columns + ["measurementDate"]
-        for column in cls.EXPECTED_COLUMNS:
-            assert column in columns
+            if ei not in index_names:
+                raise DataValidationError(
+                    f"{ei} was expected, but not found as an"
+                    f" index of the final dataframe"
+                )
+        # check for expected columns - avoid modifying at class level
+        expected_columns = copy.deepcopy(cls.EXPECTED_COLUMNS)
+        possible_extras = ["measurementDate", "quality_code"]
+        for pe in possible_extras:
+            if pe in columns:
+                expected_columns += [pe]
+        for column in expected_columns:
+            if column not in columns:
+                raise DataValidationError(
+                    f"{column} was expected, but not found as a"
+                    f" column of the final dataframe"
+                )
+
         remaining_columns = [c for c in columns if c not in expected_columns]
         # make sure all variables have a units column as well
         for rc in remaining_columns:
             if "_units" not in rc:
                 assert f"{rc}_units" in remaining_columns
 
     def __repr__(self):
```

### Comparing `metloom-0.4.3/metloom/pointdata/cdec.py` & `metloom-0.5.0/metloom/pointdata/cdec.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/metloom/pointdata/geosphere_austria.py` & `metloom-0.5.0/metloom/pointdata/geosphere_austria.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/metloom/pointdata/mesowest.py` & `metloom-0.5.0/metloom/pointdata/mesowest.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/metloom/pointdata/snotel.py` & `metloom-0.5.0/metloom/pointdata/snotel.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/metloom/pointdata/snotel_client.py` & `metloom-0.5.0/metloom/pointdata/snotel_client.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/metloom/pointdata/usgs.py` & `metloom-0.5.0/metloom/pointdata/usgs.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/metloom/request_utils.py` & `metloom-0.5.0/metloom/request_utils.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/metloom/variables.py` & `metloom-0.5.0/metloom/variables.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,23 @@
 
     code: str = "-1"  # code used within the applicable API
     name: str = "basename"  # desired name for the sensor
     description: str = None  # description of the sensor
     accumulated: bool = False  # whether or not the data is accumulated
 
 
+@dataclass(eq=True, frozen=True)
+class InstrumentDescription(SensorDescription):
+    """
+    Extend the Sensor Description to include instrument
+    """
+    # description of the specific instrument for the variable
+    instrument: str = None
+
+
 class VariableBase:
     """
     Base class to store all variables for a specific datasource. Each
     datasource should implement the class. The goal is that the variables
     are synonymous across implementations.(i.e. PRECIPITATION should have the
     same meaning in each implementation).
     Additionally, variables with the same meaning should have the same
@@ -246,7 +255,94 @@
     TEMP = SensorDescription("t7", "Air temperature 2m on observation date")
     SNOWDEPTH = SensorDescription(
         "schnee", "Snowdepth"
     )
     PRECIPITATION = SensorDescription(
         "nied", "Precipitation Total", accumulated=True
     )
+
+
+class CuesLevel1Variables(VariableBase):
+    """
+    Variables for CUES level1 data
+    https://snow.ucsb.edu/index.php/query-db/
+
+    Some variables report back with multiple instruments. See `UPSHORTWAVE`
+    and `UPSHORTWAVE2` for two instrument specific implementations
+    of the same variable.
+
+    """
+    TEMP = InstrumentDescription("air temperature", "AIR TEMP")
+    RH = InstrumentDescription("RH", "RELATIVE HUMIDITY")
+    LASERSNOWDEPTH = InstrumentDescription("laser snow depth", "LASER SNOWDEPTH")
+    SNOWDEPTH = InstrumentDescription("snow depth", "SNOWDEPTH")
+    NEWSNOWDEPTH = InstrumentDescription("new snow depth", "NEW SNOWDEPTH")
+    SWE = InstrumentDescription("Snow Pillow (DWR) SWE", "SWE")
+    # PRECIPITATION = InstrumentDescription(
+    #     "nied", "Precipitation Total", accumulated=True
+    # )
+    TEMPSURFSNOW = InstrumentDescription(
+        "snow surface temperature", "SNOW SURFACE TEMPERATURE"
+    )
+    DOWNSHORTWAVE = InstrumentDescription(
+        "downward looking solar radiation", "DOWNWARD SHORTWAVE RADIATION",
+    )
+    UPSHORTWAVE = InstrumentDescription(
+        "upward looking solar radiation", "UPWARD SHORTWAVE RADIATION",
+        instrument="Eppley Lab precision spectral pyranometer"
+    )
+    UPSHORTWAVE2 = InstrumentDescription(
+        "upward looking solar radiation", "UPWARD SHORTWAVE RADIATION 2",
+        instrument="uplooking Sunshine pyranometer  direct and diffus"
+    )
+    DOWNSHORTWAVEIR = InstrumentDescription(
+        "downward looking near-IR radiation",
+        "DOWNWARD NIR SHORTWAVE RADIATION",
+    )
+    UPSHORTWAVEIR = InstrumentDescription(
+        "upward looking near-IR radiation",
+        "UPWARD NIR SHORTWAVE RADIATION",
+    )
+
+
+class MetNorwayVariables(VariableBase):
+    """
+    See https://frost.met.no/concepts2.html#calculationmethod
+    for explanation of variable naming.
+    All available variables are
+    https://frost.met.no/elementtable
+    """
+    TEMP = SensorDescription(
+        "air_temperature", "AIR TEMP",
+        "Air temperature (default 2 m above ground), present value"
+    )
+    TEMPAVG = SensorDescription(
+        "best_estimate_mean(air_temperature P1D)", "AVG AIR TEMP",
+        "Homogenised daily mean temperature."
+        " The mean is an arithmetic mean of 24 hourly values (00-00 UTC),"
+    )
+    SNOWDEPTH = SensorDescription(
+        "surface_snow_thickness", "SNOWDEPTH",
+        "The depth of the snow is measured in cm from the ground to the top of"
+        " the snow cover. (Code=-1 means 'no snow'"
+        " and can be presented as '.')"
+    )
+    # SWE is only available as regional and interpolated datasets, so
+    # metloom will NOT return data
+    SWE = SensorDescription(
+        "liquid_water_content_of_surface_snow", "SWE",
+        "Snow water equivalent is a measure of the amount of water obtained"
+        " if the snow is melted (as height in mm of a water column)"
+    )
+    PRECIPITATIONACCUM = SensorDescription(
+        "accumulated(precipitation_amount)", "ACCUMULATED PRECIPITATION",
+        "Total precipitation amount in gauge"
+        " (accumulated since last emptying). Timing for emptying and"
+        " algoritm for calculating the precipitation"
+        " amount depends on sensortype"
+    )
+    PRECIPITATION = SensorDescription(
+        "precipitation_amount", "PRECIPITATION",
+        "Tipping bucket. The gauge tips for every 0.1 mm."
+        " Each tip is registered along with the time stamp for the tip."
+        " This is the basis for calcutation of precipitation sum per minute"
+    )
```

### Comparing `metloom-0.4.3/metloom.egg-info/PKG-INFO` & `metloom-0.5.0/metloom.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metloom
-Version: 0.4.3
+Version: 0.5.0
 Summary: Location Oriented Observed Meteorology (LOOM)
 Home-page: https://github.com/M3Works/metloom
 Author: M3Works
 Author-email: m3worksllc@gmail.com
 License: BSD license
 Keywords: metloom
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -67,14 +67,16 @@
 * Searching for stations from a datasource within a shapefile
 * Current data sources:
     * `CDEC <https://cdec.water.ca.gov/>`_
     * `SNOTEL <https://www.nrcs.usda.gov/wps/portal/wcc/home/dataAccessHelp/webService/webServiceReference/>`_
     * `MESOWEST <https://developers.synopticdata.com/mesonet/>`_
     * `USGS <https://waterservices.usgs.gov/rest/>`_
     * `GEOSPHERE AUSTRIA <https://data.hub.geosphere.at/dataset/>`_
+    * `UCSB CUES <https://snow.ucsb.edu/#>`_
+    * `MET NORWAY <https://frost.met.no/index.html>`_
 
 Requirements
 ------------
 python >= 3.7
 
 Install
 -------
```

### Comparing `metloom-0.4.3/metloom.egg-info/SOURCES.txt` & `metloom-0.5.0/metloom.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -29,23 +29,27 @@
 metloom.egg-info/entry_points.txt
 metloom.egg-info/not-zip-safe
 metloom.egg-info/requires.txt
 metloom.egg-info/top_level.txt
 metloom/pointdata/__init__.py
 metloom/pointdata/base.py
 metloom/pointdata/cdec.py
+metloom/pointdata/cues.py
 metloom/pointdata/geosphere_austria.py
 metloom/pointdata/mesowest.py
+metloom/pointdata/norway.py
 metloom/pointdata/snotel.py
 metloom/pointdata/snotel_client.py
 metloom/pointdata/usgs.py
 tests/__init__.py
 tests/shp_to_boxshp.py
 tests/test_cdec.py
+tests/test_cues.py
 tests/test_dataframe_utils.py
+tests/test_frost.py
 tests/test_geosphere.py
 tests/test_mesowest.py
 tests/test_point_data.py
 tests/test_snotel.py
 tests/test_usgs.py
 tests/test_variables.py
 tests/data/austria_box.cpg
@@ -61,13 +65,22 @@
 tests/data/triangle.cpg
 tests/data/triangle.dbf
 tests/data/triangle.prj
 tests/data/triangle.py
 tests/data/triangle.shp
 tests/data/triangle.shx
 tests/data/cdec_mocks/raw_tny_locations.csv
+tests/data/cues_mocks/daily_response.txt
+tests/data/cues_mocks/hourly_response.txt
+tests/data/frost_mocks/box.cpg
+tests/data/frost_mocks/box.dbf
+tests/data/frost_mocks/box.prj
+tests/data/frost_mocks/box.shp
+tests/data/frost_mocks/box.shx
+tests/data/frost_mocks/hourly_temp.json
+tests/data/frost_mocks/search.json
 tests/data/geosphere_mocks/klima_mock.json
 tests/data/geosphere_mocks/meta_mock.json
 tests/data/usgs_mocks/daily_response.txt
 tests/data/usgs_mocks/hourly_response.json
 tests/data/usgs_mocks/platoro_meta.txt
 tests/data/usgs_mocks/station_search_response.txt
```

### Comparing `metloom-0.4.3/setup.py` & `metloom-0.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     include_package_data=True,
     keywords='metloom',
     name='metloom',
     packages=find_packages(include=['metloom', 'metloom.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/M3Works/metloom',
-    version='0.4.3',
+    version='0.5.0',
     zip_safe=False,
 )
```

### Comparing `metloom-0.4.3/tests/data/cdec_mocks/raw_tny_locations.csv` & `metloom-0.5.0/tests/data/cdec_mocks/raw_tny_locations.csv`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/tests/data/geosphere_mocks/klima_mock.json` & `metloom-0.5.0/tests/data/geosphere_mocks/klima_mock.json`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/tests/data/geosphere_mocks/meta_mock.json` & `metloom-0.5.0/tests/data/geosphere_mocks/meta_mock.json`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/tests/data/usgs_mocks/daily_response.txt` & `metloom-0.5.0/tests/data/usgs_mocks/daily_response.txt`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/tests/data/usgs_mocks/hourly_response.json` & `metloom-0.5.0/tests/data/usgs_mocks/hourly_response.json`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/tests/data/usgs_mocks/platoro_meta.txt` & `metloom-0.5.0/tests/data/usgs_mocks/platoro_meta.txt`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/tests/data/usgs_mocks/station_search_response.txt` & `metloom-0.5.0/tests/data/usgs_mocks/station_search_response.txt`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/tests/shp_to_boxshp.py` & `metloom-0.5.0/tests/shp_to_boxshp.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/tests/test_cdec.py` & `metloom-0.5.0/tests/test_cdec.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/tests/test_dataframe_utils.py` & `metloom-0.5.0/tests/test_dataframe_utils.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/tests/test_geosphere.py` & `metloom-0.5.0/tests/test_geosphere.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/tests/test_mesowest.py` & `metloom-0.5.0/tests/test_mesowest.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/tests/test_point_data.py` & `metloom-0.5.0/tests/test_point_data.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/tests/test_snotel.py` & `metloom-0.5.0/tests/test_snotel.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/tests/test_usgs.py` & `metloom-0.5.0/tests/test_usgs.py`

 * *Files identical despite different names*

### Comparing `metloom-0.4.3/tests/test_variables.py` & `metloom-0.5.0/tests/test_variables.py`

 * *Files identical despite different names*

