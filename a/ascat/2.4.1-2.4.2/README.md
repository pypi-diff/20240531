# Comparing `tmp/ascat-2.4.1.tar.gz` & `tmp/ascat-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascat-2.4.1.tar", last modified: Tue May 28 09:09:29 2024, max compression
+gzip compressed data, was "ascat-2.4.2.tar", last modified: Fri May 31 13:08:48 2024, max compression
```

## Comparing `ascat-2.4.1.tar` & `ascat-2.4.2.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.922756 ascat-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-28 09:09:19.000000 ascat-2.4.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.886756 ascat-2.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.890756 ascat-2.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-28 09:09:19.000000 ascat-2.4.1/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-28 09:09:19.000000 ascat-2.4.1/.github/workflows/upload_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-28 09:09:19.000000 ascat-2.4.1/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-28 09:09:19.000000 ascat-2.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-28 09:09:19.000000 ascat-2.4.1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-28 09:09:19.000000 ascat-2.4.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-28 09:09:19.000000 ascat-2.4.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-05-28 09:09:19.000000 ascat-2.4.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-28 09:09:19.000000 ascat-2.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-05-28 09:09:29.922756 ascat-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-05-28 09:09:19.000000 ascat-2.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.898756 ascat-2.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.902756 ascat-2.4.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/ascat_bufr_format.rst
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9929 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/docs_env.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/license.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.902756 ascat-2.4.1/docs/org/
--rw-r--r--   0 runner    (1001) docker     (127)    33620 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/org/xarray_readers_tutorial.org
--rw-r--r--   0 runner    (1001) docker     (127)    92416 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_cgls_swi_ts.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_cgls_swi_ts.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.902756 ascat-2.4.1/docs/read_cgls_swi_ts_files/
--rw-r--r--   0 runner    (1001) docker     (127)    65951 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_cgls_swi_ts_files/read_cgls_swi_ts_7_0.png
--rw-r--r--   0 runner    (1001) docker     (127)   578048 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_eumetsat.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    35677 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_eumetsat.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.902756 ascat-2.4.1/docs/read_eumetsat_files/
--rw-r--r--   0 runner    (1001) docker     (127)    99279 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_eumetsat_files/read_eumetsat_19_0.png
--rw-r--r--   0 runner    (1001) docker     (127)   151416 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_eumetsat_files/read_eumetsat_5_0.png
--rw-r--r--   0 runner    (1001) docker     (127)   151239 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_eumetsat_files/read_eumetsat_8_0.png
--rw-r--r--   0 runner    (1001) docker     (127)   719257 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_cdr.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_cdr.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.902756 ascat-2.4.1/docs/read_hsaf_cdr_files/
--rw-r--r--   0 runner    (1001) docker     (127)    68510 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_10_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    77447 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_12_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    78359 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_15_1.png
--rw-r--r--   0 runner    (1001) docker     (127)   162796 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_18_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    78897 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_21_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    65970 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_8_1.png
--rw-r--r--   0 runner    (1001) docker     (127)  1256504 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_nrt.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11409 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_nrt.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.906756 ascat-2.4.1/docs/read_hsaf_nrt_files/
--rw-r--r--   0 runner    (1001) docker     (127)   173484 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_0.png
--rw-r--r--   0 runner    (1001) docker     (127)   168175 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_1.png
--rw-r--r--   0 runner    (1001) docker     (127)   165841 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_2.png
--rw-r--r--   0 runner    (1001) docker     (127)   171571 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_3.png
--rw-r--r--   0 runner    (1001) docker     (127)    33102 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_16_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    31452 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_18_0.png
--rw-r--r--   0 runner    (1001) docker     (127)   186561 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_7_0.png
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1289682 2024-05-28 09:09:19.000000 ascat-2.4.1/docs/xarray_readers_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-28 09:09:19.000000 ascat-2.4.1/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-28 09:09:19.000000 ascat-2.4.1/environment_win.yml
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-28 09:09:19.000000 ascat-2.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-28 09:09:29.922756 ascat-2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-28 09:09:19.000000 ascat-2.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.886756 ascat-2.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.906756 ascat-2.4.1/src/ascat/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.910756 ascat-2.4.1/src/ascat/aggregate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/aggregate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/aggregate/aggregators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/aggregate/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     7019 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/cgls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.910756 ascat-2.4.1/src/ascat/download/
--rw-r--r--   0 runner    (1001) docker     (127)    20661 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/download/connectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/download/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.910756 ascat-2.4.1/src/ascat/eumetsat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/eumetsat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16171 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/eumetsat/level1.py
--rw-r--r--   0 runner    (1001) docker     (127)    11671 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/eumetsat/level2.py
--rw-r--r--   0 runner    (1001) docker     (127)    29708 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/file_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     9481 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/h_saf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.910756 ascat-2.4.1/src/ascat/read_native/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21703 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/bufr.py
--rw-r--r--   0 runner    (1001) docker     (127)    13374 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/cdr.py
--rw-r--r--   0 runner    (1001) docker     (127)    73255 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/eps_native.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.918756 ascat-2.4.1/src/ascat/read_native/formats/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/ccsds.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps.dtd
--rw-r--r--   0 runner    (1001) docker     (127)    67604 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    34467 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszf_13.1.xml
--rw-r--r--   0 runner    (1001) docker     (127)    63559 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.4.xml
--rw-r--r--   0 runner    (1001) docker     (127)    63563 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.4m.xml
--rw-r--r--   0 runner    (1001) docker     (127)    66425 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.5.xml
--rw-r--r--   0 runner    (1001) docker     (127)    66555 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.6.xml
--rw-r--r--   0 runner    (1001) docker     (127)    39840 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszf_7.0.xml
--rw-r--r--   0 runner    (1001) docker     (127)    37290 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszf_9.0.xml
--rw-r--r--   0 runner    (1001) docker     (127)    36662 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszo_13.1.xml
--rw-r--r--   0 runner    (1001) docker     (127)    68252 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.4.xml
--rw-r--r--   0 runner    (1001) docker     (127)    68256 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.4m.xml
--rw-r--r--   0 runner    (1001) docker     (127)    71118 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.5.xml
--rw-r--r--   0 runner    (1001) docker     (127)    70852 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.6.xml
--rw-r--r--   0 runner    (1001) docker     (127)    44139 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszo_7.0.xml
--rw-r--r--   0 runner    (1001) docker     (127)    42894 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszo_9.0.xml
--rw-r--r--   0 runner    (1001) docker     (127)    36664 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszr_13.1.xml
--rw-r--r--   0 runner    (1001) docker     (127)    68252 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.4.xml
--rw-r--r--   0 runner    (1001) docker     (127)    68256 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.4m.xml
--rw-r--r--   0 runner    (1001) docker     (127)    71118 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.5.xml
--rw-r--r--   0 runner    (1001) docker     (127)    70852 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.6.xml
--rw-r--r--   0 runner    (1001) docker     (127)    44137 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszr_7.0.xml
--rw-r--r--   0 runner    (1001) docker     (127)    42843 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszr_9.0.xml
--rw-r--r--   0 runner    (1001) docker     (127)    25967 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl2smo_0.1.xml
--rw-r--r--   0 runner    (1001) docker     (127)    32143 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl2smo_3b.xml
--rw-r--r--   0 runner    (1001) docker     (127)    31812 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl2smo_4.xml
--rw-r--r--   0 runner    (1001) docker     (127)    25966 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl2smr_0.1.xml
--rw-r--r--   0 runner    (1001) docker     (127)    31948 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl2smr_3b.xml
--rw-r--r--   0 runner    (1001) docker     (127)    31615 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl2smr_4.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9631 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)    18014 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/nc.py
--rw-r--r--   0 runner    (1001) docker     (127)    89975 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/ragged_array_ts.py
--rw-r--r--   0 runner    (1001) docker     (127)    57936 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/read_native/xarray_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.918756 ascat-2.4.1/src/ascat/regrid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/regrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/regrid/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/regrid/regrid.py
--rw-r--r--   0 runner    (1001) docker     (127)    11244 2024-05-28 09:09:19.000000 ascat-2.4.1/src/ascat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.922756 ascat-2.4.1/src/ascat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-05-28 09:09:29.000000 ascat-2.4.1/src/ascat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-28 09:09:29.000000 ascat-2.4.1/src/ascat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:09:29.000000 ascat-2.4.1/src/ascat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-28 09:09:29.000000 ascat-2.4.1/src/ascat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:09:29.000000 ascat-2.4.1/src/ascat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-28 09:09:29.000000 ascat-2.4.1/src/ascat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-28 09:09:29.000000 ascat-2.4.1/src/ascat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:09:29.922756 ascat-2.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-28 09:09:19.000000 ascat-2.4.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-28 09:09:19.000000 ascat-2.4.1/tests/get_path.py
--rw-r--r--   0 runner    (1001) docker     (127)    17871 2024-05-28 09:09:19.000000 ascat-2.4.1/tests/skip_test_ragged_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-05-28 09:09:19.000000 ascat-2.4.1/tests/test_cgls.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-28 09:09:19.000000 ascat-2.4.1/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (127)    19541 2024-05-28 09:09:19.000000 ascat-2.4.1/tests/test_file_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)    17247 2024-05-28 09:09:19.000000 ascat-2.4.1/tests/test_h_saf.py
--rw-r--r--   0 runner    (1001) docker     (127)    19189 2024-05-28 09:09:19.000000 ascat-2.4.1/tests/test_level1.py
--rw-r--r--   0 runner    (1001) docker     (127)    16684 2024-05-28 09:09:19.000000 ascat-2.4.1/tests/test_level2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-28 09:09:19.000000 ascat-2.4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:08:48.548509 ascat-2.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-31 13:08:42.000000 ascat-2.4.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:08:48.516508 ascat-2.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:08:48.520508 ascat-2.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-31 13:08:42.000000 ascat-2.4.2/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-31 13:08:42.000000 ascat-2.4.2/.github/workflows/upload_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-31 13:08:42.000000 ascat-2.4.2/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-31 13:08:42.000000 ascat-2.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-31 13:08:42.000000 ascat-2.4.2/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-31 13:08:42.000000 ascat-2.4.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-31 13:08:42.000000 ascat-2.4.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-05-31 13:08:42.000000 ascat-2.4.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-31 13:08:42.000000 ascat-2.4.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-05-31 13:08:48.548509 ascat-2.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-05-31 13:08:42.000000 ascat-2.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:08:48.528508 ascat-2.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:08:48.528508 ascat-2.4.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/ascat_bufr_format.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9929 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/docs_env.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:08:48.528508 ascat-2.4.2/docs/org/
+-rw-r--r--   0 runner    (1001) docker     (127)    33620 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/org/xarray_readers_tutorial.org
+-rw-r--r--   0 runner    (1001) docker     (127)    92416 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/read_cgls_swi_ts.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/read_cgls_swi_ts.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:08:48.528508 ascat-2.4.2/docs/read_cgls_swi_ts_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    65951 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/read_cgls_swi_ts_files/read_cgls_swi_ts_7_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)   578048 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/read_eumetsat.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    35677 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/read_eumetsat.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:08:48.528508 ascat-2.4.2/docs/read_eumetsat_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    99279 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/read_eumetsat_files/read_eumetsat_19_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)   151416 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/read_eumetsat_files/read_eumetsat_5_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)   151239 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/read_eumetsat_files/read_eumetsat_8_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)   719257 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/read_hsaf_cdr.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/read_hsaf_cdr.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:08:48.532508 ascat-2.4.2/docs/read_hsaf_cdr_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    68510 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/read_hsaf_cdr_files/read_hsaf_cdr_10_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    77447 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/read_hsaf_cdr_files/read_hsaf_cdr_12_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    78359 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/read_hsaf_cdr_files/read_hsaf_cdr_15_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   162796 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/read_hsaf_cdr_files/read_hsaf_cdr_18_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    78897 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/read_hsaf_cdr_files/read_hsaf_cdr_21_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    65970 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/read_hsaf_cdr_files/read_hsaf_cdr_8_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1256504 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/read_hsaf_nrt.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11409 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/read_hsaf_nrt.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:08:48.532508 ascat-2.4.2/docs/read_hsaf_nrt_files/
+-rw-r--r--   0 runner    (1001) docker     (127)   173484 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)   168175 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   165841 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)   171571 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33102 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/read_hsaf_nrt_files/read_hsaf_nrt_16_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31452 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/read_hsaf_nrt_files/read_hsaf_nrt_18_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)   186561 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/read_hsaf_nrt_files/read_hsaf_nrt_7_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1289682 2024-05-31 13:08:42.000000 ascat-2.4.2/docs/xarray_readers_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-31 13:08:42.000000 ascat-2.4.2/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-31 13:08:42.000000 ascat-2.4.2/environment_win.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-31 13:08:42.000000 ascat-2.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-31 13:08:48.548509 ascat-2.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-31 13:08:42.000000 ascat-2.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:08:48.516508 ascat-2.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:08:48.536508 ascat-2.4.2/src/ascat/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:08:48.536508 ascat-2.4.2/src/ascat/aggregate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/aggregate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/aggregate/aggregators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/aggregate/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7019 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/cgls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:08:48.536508 ascat-2.4.2/src/ascat/download/
+-rw-r--r--   0 runner    (1001) docker     (127)    20661 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/download/connectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/download/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:08:48.536508 ascat-2.4.2/src/ascat/eumetsat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/eumetsat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16171 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/eumetsat/level1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11671 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/eumetsat/level2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29708 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/file_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9481 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/h_saf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:08:48.536508 ascat-2.4.2/src/ascat/read_native/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21703 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/bufr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13374 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/cdr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73256 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/eps_native.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:08:48.544509 ascat-2.4.2/src/ascat/read_native/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/formats/ccsds.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/formats/eps.dtd
+-rw-r--r--   0 runner    (1001) docker     (127)    67604 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/formats/eps.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    34467 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszf_13.1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    63559 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszf_6.4.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    63563 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszf_6.4m.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    66425 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszf_6.5.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    66555 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszf_6.6.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    39840 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszf_7.0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    37290 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszf_9.0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    36662 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszo_13.1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    68252 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszo_6.4.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    68256 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszo_6.4m.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    71118 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszo_6.5.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    70852 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszo_6.6.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    44139 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszo_7.0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    42894 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszo_9.0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    36664 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszr_13.1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    68252 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszr_6.4.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    68256 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszr_6.4m.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    71118 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszr_6.5.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    70852 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszr_6.6.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    44137 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszr_7.0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    42843 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszr_9.0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    25967 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl2smo_0.1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    32143 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl2smo_3b.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    31812 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl2smo_4.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    25966 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl2smr_0.1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    31948 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl2smr_3b.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    31615 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl2smr_4.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9631 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18014 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/nc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89975 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/ragged_array_ts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57936 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/read_native/xarray_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:08:48.544509 ascat-2.4.2/src/ascat/regrid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/regrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/regrid/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/regrid/regrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11244 2024-05-31 13:08:42.000000 ascat-2.4.2/src/ascat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:08:48.548509 ascat-2.4.2/src/ascat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-05-31 13:08:48.000000 ascat-2.4.2/src/ascat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-31 13:08:48.000000 ascat-2.4.2/src/ascat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:08:48.000000 ascat-2.4.2/src/ascat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-31 13:08:48.000000 ascat-2.4.2/src/ascat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:08:48.000000 ascat-2.4.2/src/ascat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-31 13:08:48.000000 ascat-2.4.2/src/ascat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-31 13:08:48.000000 ascat-2.4.2/src/ascat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:08:48.548509 ascat-2.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-31 13:08:42.000000 ascat-2.4.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-31 13:08:42.000000 ascat-2.4.2/tests/get_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17871 2024-05-31 13:08:42.000000 ascat-2.4.2/tests/skip_test_ragged_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-05-31 13:08:42.000000 ascat-2.4.2/tests/test_cgls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-31 13:08:42.000000 ascat-2.4.2/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19541 2024-05-31 13:08:42.000000 ascat-2.4.2/tests/test_file_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17247 2024-05-31 13:08:42.000000 ascat-2.4.2/tests/test_h_saf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19189 2024-05-31 13:08:42.000000 ascat-2.4.2/tests/test_level1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16684 2024-05-31 13:08:42.000000 ascat-2.4.2/tests/test_level2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-31 13:08:42.000000 ascat-2.4.2/tox.ini
```

### Comparing `ascat-2.4.1/.coveragerc` & `ascat-2.4.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/.github/workflows/ubuntu.yml` & `ascat-2.4.2/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/.github/workflows/upload_pypi.yml` & `ascat-2.4.2/.github/workflows/upload_pypi.yml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/.github/workflows/windows.yml` & `ascat-2.4.2/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/.gitignore` & `ascat-2.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/CHANGELOG.rst` & `ascat-2.4.2/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+Version 2.4.2
+=============
+
+- Fix typo in flagfield name
+
 Version 2.4.1
 =============
 
 - Add keyword to ignore ASCAT Level 1b flag noise out of limits
 
 Version 2.4.0
 =============
```

### Comparing `ascat-2.4.1/LICENSE.txt` & `ascat-2.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/PKG-INFO` & `ascat-2.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascat
-Version: 2.4.1
+Version: 2.4.2
 Summary: Read and visualize for data from the Advanced Scatterometer (ASCAT)
 Home-page: https://tuwien.at/mg/geo/rs
 Author: TU Wien
 Author-email: remote.sensing@geo.tuwien.ac.at
 License: MIT
 Project-URL: Documentation, https://ascat.readthedocs.org/
 Platform: any
```

### Comparing `ascat-2.4.1/README.md` & `ascat-2.4.2/README.md`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/Makefile` & `ascat-2.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/ascat_bufr_format.rst` & `ascat-2.4.2/docs/ascat_bufr_format.rst`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/conf.py` & `ascat-2.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/examples.rst` & `ascat-2.4.2/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/index.rst` & `ascat-2.4.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/org/xarray_readers_tutorial.org` & `ascat-2.4.2/docs/org/xarray_readers_tutorial.org`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/read_cgls_swi_ts.ipynb` & `ascat-2.4.2/docs/read_cgls_swi_ts.ipynb`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/read_cgls_swi_ts.rst` & `ascat-2.4.2/docs/read_cgls_swi_ts.rst`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/read_cgls_swi_ts_files/read_cgls_swi_ts_7_0.png` & `ascat-2.4.2/docs/read_cgls_swi_ts_files/read_cgls_swi_ts_7_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/read_eumetsat.ipynb` & `ascat-2.4.2/docs/read_eumetsat.ipynb`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/read_eumetsat.rst` & `ascat-2.4.2/docs/read_eumetsat.rst`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/read_eumetsat_files/read_eumetsat_19_0.png` & `ascat-2.4.2/docs/read_eumetsat_files/read_eumetsat_19_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/read_eumetsat_files/read_eumetsat_5_0.png` & `ascat-2.4.2/docs/read_eumetsat_files/read_eumetsat_5_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/read_eumetsat_files/read_eumetsat_8_0.png` & `ascat-2.4.2/docs/read_eumetsat_files/read_eumetsat_8_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/read_hsaf_cdr.ipynb` & `ascat-2.4.2/docs/read_hsaf_cdr.ipynb`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/read_hsaf_cdr.rst` & `ascat-2.4.2/docs/read_hsaf_cdr.rst`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_10_1.png` & `ascat-2.4.2/docs/read_hsaf_cdr_files/read_hsaf_cdr_10_1.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_12_1.png` & `ascat-2.4.2/docs/read_hsaf_cdr_files/read_hsaf_cdr_12_1.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_15_1.png` & `ascat-2.4.2/docs/read_hsaf_cdr_files/read_hsaf_cdr_15_1.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_18_1.png` & `ascat-2.4.2/docs/read_hsaf_cdr_files/read_hsaf_cdr_18_1.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_21_1.png` & `ascat-2.4.2/docs/read_hsaf_cdr_files/read_hsaf_cdr_21_1.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/read_hsaf_cdr_files/read_hsaf_cdr_8_1.png` & `ascat-2.4.2/docs/read_hsaf_cdr_files/read_hsaf_cdr_8_1.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/read_hsaf_nrt.ipynb` & `ascat-2.4.2/docs/read_hsaf_nrt.ipynb`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/read_hsaf_nrt.rst` & `ascat-2.4.2/docs/read_hsaf_nrt.rst`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_0.png` & `ascat-2.4.2/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_1.png` & `ascat-2.4.2/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_1.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_2.png` & `ascat-2.4.2/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_2.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_3.png` & `ascat-2.4.2/docs/read_hsaf_nrt_files/read_hsaf_nrt_12_3.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_16_0.png` & `ascat-2.4.2/docs/read_hsaf_nrt_files/read_hsaf_nrt_16_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_18_0.png` & `ascat-2.4.2/docs/read_hsaf_nrt_files/read_hsaf_nrt_18_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/read_hsaf_nrt_files/read_hsaf_nrt_7_0.png` & `ascat-2.4.2/docs/read_hsaf_nrt_files/read_hsaf_nrt_7_0.png`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/docs/xarray_readers_tutorial.ipynb` & `ascat-2.4.2/docs/xarray_readers_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/setup.cfg` & `ascat-2.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/setup.py` & `ascat-2.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/__init__.py` & `ascat-2.4.2/src/ascat/__init__.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/aggregate/aggregators.py` & `ascat-2.4.2/src/ascat/aggregate/aggregators.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/aggregate/interface.py` & `ascat-2.4.2/src/ascat/aggregate/interface.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/cgls.py` & `ascat-2.4.2/src/ascat/cgls.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/download/connectors.py` & `ascat-2.4.2/src/ascat/download/connectors.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/download/interface.py` & `ascat-2.4.2/src/ascat/download/interface.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/eumetsat/level1.py` & `ascat-2.4.2/src/ascat/eumetsat/level1.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/eumetsat/level2.py` & `ascat-2.4.2/src/ascat/eumetsat/level2.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/file_handling.py` & `ascat-2.4.2/src/ascat/file_handling.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/h_saf.py` & `ascat-2.4.2/src/ascat/h_saf.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/bufr.py` & `ascat-2.4.2/src/ascat/read_native/bufr.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/cdr.py` & `ascat-2.4.2/src/ascat/read_native/cdr.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/eps_native.py` & `ascat-2.4.2/src/ascat/read_native/eps_native.py`

 * *Files 0% similar despite different names*

```diff
@@ -1983,15 +1983,15 @@
         "flagfield_pl": np.array([2, 2, 2, 2, 0, 0, 0, 0]),
         "flagfield_gen1": np.array([0, 2, 0, 0, 0, 0, 0, 0]),
         "flagfield_gen2": np.array([1, 0, 2, 0, 0, 0, 0, 0])
     }
 
     if ignore_noise_ool:
         # remove "noise out of limits" as red flag
-        flag_status_bit["flagfield_rf"] = np.array([2, 0, 0, 0, 0, 0, 0, 0])
+        flag_status_bit["flagfield_rf2"] = np.array([2, 0, 0, 0, 0, 0, 0, 0])
 
     f_usable = np.zeros(data["flagfield_rf1"].size, dtype=np.uint8)
 
     for flagfield, bitmask in flag_status_bit.items():
         subset = np.nonzero(data[flagfield])[0]
 
         if subset.size > 0:
```

### Comparing `ascat-2.4.1/src/ascat/read_native/formats/ccsds.xml` & `ascat-2.4.2/src/ascat/read_native/formats/ccsds.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/formats/eps.dtd` & `ascat-2.4.2/src/ascat/read_native/formats/eps.dtd`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/formats/eps.xsl` & `ascat-2.4.2/src/ascat/read_native/formats/eps.xsl`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszf_13.1.xml` & `ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszf_13.1.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.4.xml` & `ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszf_6.4.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.4m.xml` & `ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszf_6.4m.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.5.xml` & `ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszf_6.5.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszf_6.6.xml` & `ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszf_6.6.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszf_7.0.xml` & `ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszf_7.0.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszf_9.0.xml` & `ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszf_9.0.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszo_13.1.xml` & `ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszo_13.1.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.4.xml` & `ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszo_6.4.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.4m.xml` & `ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszo_6.4m.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.5.xml` & `ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszo_6.5.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszo_6.6.xml` & `ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszo_6.6.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszo_7.0.xml` & `ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszo_7.0.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszo_9.0.xml` & `ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszo_9.0.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszr_13.1.xml` & `ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszr_13.1.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.4.xml` & `ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszr_6.4.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.4m.xml` & `ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszr_6.4m.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.5.xml` & `ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszr_6.5.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszr_6.6.xml` & `ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszr_6.6.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszr_7.0.xml` & `ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszr_7.0.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl1bszr_9.0.xml` & `ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl1bszr_9.0.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl2smo_0.1.xml` & `ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl2smo_0.1.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl2smo_3b.xml` & `ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl2smo_3b.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl2smo_4.xml` & `ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl2smo_4.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl2smr_0.1.xml` & `ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl2smr_0.1.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl2smr_3b.xml` & `ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl2smr_3b.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/formats/eps_ascatl2smr_4.xml` & `ascat-2.4.2/src/ascat/read_native/formats/eps_ascatl2smr_4.xml`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/hdf5.py` & `ascat-2.4.2/src/ascat/read_native/hdf5.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/nc.py` & `ascat-2.4.2/src/ascat/read_native/nc.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/ragged_array_ts.py` & `ascat-2.4.2/src/ascat/read_native/ragged_array_ts.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/read_native/xarray_io.py` & `ascat-2.4.2/src/ascat/read_native/xarray_io.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/regrid/interface.py` & `ascat-2.4.2/src/ascat/regrid/interface.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/regrid/regrid.py` & `ascat-2.4.2/src/ascat/regrid/regrid.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat/utils.py` & `ascat-2.4.2/src/ascat/utils.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/src/ascat.egg-info/PKG-INFO` & `ascat-2.4.2/src/ascat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascat
-Version: 2.4.1
+Version: 2.4.2
 Summary: Read and visualize for data from the Advanced Scatterometer (ASCAT)
 Home-page: https://tuwien.at/mg/geo/rs
 Author: TU Wien
 Author-email: remote.sensing@geo.tuwien.ac.at
 License: MIT
 Project-URL: Documentation, https://ascat.readthedocs.org/
 Platform: any
```

### Comparing `ascat-2.4.1/src/ascat.egg-info/SOURCES.txt` & `ascat-2.4.2/src/ascat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/tests/get_path.py` & `ascat-2.4.2/tests/get_path.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/tests/skip_test_ragged_array.py` & `ascat-2.4.2/tests/skip_test_ragged_array.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/tests/test_cgls.py` & `ascat-2.4.2/tests/test_cgls.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/tests/test_download.py` & `ascat-2.4.2/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/tests/test_file_handling.py` & `ascat-2.4.2/tests/test_file_handling.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/tests/test_h_saf.py` & `ascat-2.4.2/tests/test_h_saf.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/tests/test_level1.py` & `ascat-2.4.2/tests/test_level1.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/tests/test_level2.py` & `ascat-2.4.2/tests/test_level2.py`

 * *Files identical despite different names*

### Comparing `ascat-2.4.1/tox.ini` & `ascat-2.4.2/tox.ini`

 * *Files identical despite different names*

