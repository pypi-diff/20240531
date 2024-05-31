# Comparing `tmp/pyebsdindex-0.3.1.tar.gz` & `tmp/pyebsdindex-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyebsdindex-0.3.1.tar", last modified: Fri May 24 18:49:05 2024, max compression
+gzip compressed data, was "pyebsdindex-0.3.2.tar", last modified: Fri May 31 20:16:07 2024, max compression
```

## Comparing `pyebsdindex-0.3.1.tar` & `pyebsdindex-0.3.2.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:49:05.687178 pyebsdindex-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)   368506 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/IPFCubic.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   147377 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/IPFCubic.png
--rw-r--r--   0 runner    (1001) docker     (127)   197654 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/IPFHex.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    82053 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/IPFHex.png
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/License
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-24 18:49:05.687178 pyebsdindex-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/RELEASE.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:49:05.667178 pyebsdindex-0.3.1/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:49:05.667178 pyebsdindex-0.3.1/doc/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:49:05.667178 pyebsdindex-0.3.1/doc/_static/colormap_banners/
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/doc/_static/colormap_banners/banner0.png
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/doc/_static/colormap_banners/banner1.png
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/doc/_static/colormap_banners/create_colormap_banners.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/doc/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:49:05.671178 pyebsdindex-0.3.1/doc/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:49:05.671178 pyebsdindex-0.3.1/doc/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/doc/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/doc/_templates/custom-attribute-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/doc/_templates/custom-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/doc/_templates/custom-function-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/doc/_templates/custom-method-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/doc/_templates/custom-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/doc/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:49:05.671178 pyebsdindex-0.3.1/doc/dev/
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/doc/dev/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:49:05.671178 pyebsdindex-0.3.1/doc/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/doc/reference/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:49:05.671178 pyebsdindex-0.3.1/doc/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/doc/tutorials/NLPAR_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  1570100 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/doc/tutorials/ebsd_index_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/doc/tutorials/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:49:05.671178 pyebsdindex-0.3.1/doc/user/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/doc/user/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/doc/user/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:49:05.675178 pyebsdindex-0.3.1/pyebsdindex/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:49:05.679178 pyebsdindex-0.3.1/pyebsdindex/EBSDImage/
--rw-r--r--   0 runner    (1001) docker     (127)    12490 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/EBSDImage/IPFcolor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/EBSDImage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34888 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/_ebsd_index_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)    33740 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/_ebsd_index_single.py
--rw-r--r--   0 runner    (1001) docker     (127)    28606 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/band_detect.py
--rw-r--r--   0 runner    (1001) docker     (127)    17076 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/crystal_sym.py
--rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/crystallometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/ebsd_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    50809 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/ebsd_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)    12787 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/ebsdfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/misorientation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/nlpar.py
--rw-r--r--   0 runner    (1001) docker     (127)    29024 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/nlpar_cpu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:49:05.679178 pyebsdindex-0.3.1/pyebsdindex/opencl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/opencl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29511 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/opencl/band_detect_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)    28523 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/opencl/clkernels.cl
--rw-r--r--   0 runner    (1001) docker     (127)    13481 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/opencl/clnlpar.cl
--rw-r--r--   0 runner    (1001) docker     (127)    20626 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/opencl/nlpar_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)    28570 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/opencl/nlpar_clray.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/opencl/openclparam.py
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/opencl/radon_fast_cl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/opencl/test.cl
--rw-r--r--   0 runner    (1001) docker     (127)     9704 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/pairlib.py
--rw-r--r--   0 runner    (1001) docker     (127)    20611 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/pcopt.py
--rw-r--r--   0 runner    (1001) docker     (127)    14993 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/radon_fast.py
--rw-r--r--   0 runner    (1001) docker     (127)    22234 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/rotations.py
--rw-r--r--   0 runner    (1001) docker     (127)    51834 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/rotlib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:49:05.679178 pyebsdindex-0.3.1/pyebsdindex/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:49:05.663178 pyebsdindex-0.3.1/pyebsdindex/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:49:05.679178 pyebsdindex-0.3.1/pyebsdindex/tests/data/al_sim_20kv/
--rw-r--r--   0 runner    (1001) docker     (127)    10569 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/tests/data/al_sim_20kv/al_sim_20kv.png
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/tests/data/al_sim_20kv/generate_al_sim_20kv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/tests/numbatest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/tests/raytest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/tests/rotlibunittest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/tests/test_ebsd_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/tests/test_pcopt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/tests/test_tripletvote.py
--rw-r--r--   0 runner    (1001) docker     (127)    67523 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/pyebsdindex/tripletvote.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:49:05.683178 pyebsdindex-0.3.1/pyebsdindex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-24 18:49:05.000000 pyebsdindex-0.3.1/pyebsdindex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-24 18:49:05.000000 pyebsdindex-0.3.1/pyebsdindex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 18:49:05.000000 pyebsdindex-0.3.1/pyebsdindex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-24 18:49:05.000000 pyebsdindex-0.3.1/pyebsdindex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-24 18:49:05.000000 pyebsdindex-0.3.1/pyebsdindex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 18:49:05.000000 pyebsdindex-0.3.1/pyebsdindex.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-24 18:49:05.687178 pyebsdindex-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-24 18:49:01.000000 pyebsdindex-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:16:07.128372 pyebsdindex-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   368506 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/IPFCubic.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   147377 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/IPFCubic.png
+-rw-r--r--   0 runner    (1001) docker     (127)   197654 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/IPFHex.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    82053 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/IPFHex.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/License
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-31 20:16:07.128372 pyebsdindex-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/RELEASE.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:16:07.112372 pyebsdindex-0.3.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:16:07.112372 pyebsdindex-0.3.2/doc/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:16:07.112372 pyebsdindex-0.3.2/doc/_static/colormap_banners/
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/doc/_static/colormap_banners/banner0.png
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/doc/_static/colormap_banners/banner1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/doc/_static/colormap_banners/create_colormap_banners.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/doc/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:16:07.112372 pyebsdindex-0.3.2/doc/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:16:07.112372 pyebsdindex-0.3.2/doc/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/doc/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/doc/_templates/custom-attribute-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/doc/_templates/custom-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/doc/_templates/custom-function-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/doc/_templates/custom-method-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/doc/_templates/custom-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/doc/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:16:07.112372 pyebsdindex-0.3.2/doc/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/doc/dev/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:16:07.112372 pyebsdindex-0.3.2/doc/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/doc/reference/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:16:07.116372 pyebsdindex-0.3.2/doc/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/doc/tutorials/NLPAR_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1570100 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/doc/tutorials/ebsd_index_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/doc/tutorials/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:16:07.116372 pyebsdindex-0.3.2/doc/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/doc/user/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/doc/user/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:16:07.120372 pyebsdindex-0.3.2/pyebsdindex/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:16:07.120372 pyebsdindex-0.3.2/pyebsdindex/EBSDImage/
+-rw-r--r--   0 runner    (1001) docker     (127)    12490 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/EBSDImage/IPFcolor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/EBSDImage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34888 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/_ebsd_index_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33740 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/_ebsd_index_single.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28606 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/band_detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17076 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/crystal_sym.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/crystallometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/ebsd_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50809 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/ebsd_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12787 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/ebsdfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/misorientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/nlpar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29024 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/nlpar_cpu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:16:07.120372 pyebsdindex-0.3.2/pyebsdindex/opencl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/opencl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29542 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/opencl/band_detect_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28523 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/opencl/clkernels.cl
+-rw-r--r--   0 runner    (1001) docker     (127)    13481 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/opencl/clnlpar.cl
+-rw-r--r--   0 runner    (1001) docker     (127)    20873 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/opencl/nlpar_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28751 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/opencl/nlpar_clray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/opencl/openclparam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/opencl/radon_fast_cl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/opencl/test.cl
+-rw-r--r--   0 runner    (1001) docker     (127)     9704 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/pairlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20611 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/pcopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15025 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/radon_fast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22234 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/rotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51834 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/rotlib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:16:07.124372 pyebsdindex-0.3.2/pyebsdindex/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:16:07.108372 pyebsdindex-0.3.2/pyebsdindex/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:16:07.124372 pyebsdindex-0.3.2/pyebsdindex/tests/data/al_sim_20kv/
+-rw-r--r--   0 runner    (1001) docker     (127)    10569 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/tests/data/al_sim_20kv/al_sim_20kv.png
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/tests/data/al_sim_20kv/generate_al_sim_20kv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/tests/numbatest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/tests/raytest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/tests/rotlibunittest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/tests/test_ebsd_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/tests/test_pcopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/tests/test_tripletvote.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67523 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/pyebsdindex/tripletvote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:16:07.124372 pyebsdindex-0.3.2/pyebsdindex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-31 20:16:07.000000 pyebsdindex-0.3.2/pyebsdindex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-31 20:16:07.000000 pyebsdindex-0.3.2/pyebsdindex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:16:07.000000 pyebsdindex-0.3.2/pyebsdindex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-31 20:16:07.000000 pyebsdindex-0.3.2/pyebsdindex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-31 20:16:07.000000 pyebsdindex-0.3.2/pyebsdindex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:16:06.000000 pyebsdindex-0.3.2/pyebsdindex.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-31 20:16:07.128372 pyebsdindex-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-31 20:15:59.000000 pyebsdindex-0.3.2/setup.py
```

### Comparing `pyebsdindex-0.3.1/.readthedocs.yaml` & `pyebsdindex-0.3.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/CHANGELOG.rst` & `pyebsdindex-0.3.2/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 =========
 Changelog
 =========
 
 All notable changes to PyEBSDIndex will be documented in this file. The format is based
 on `Keep a Changelog <https://keepachangelog.com/en/1.1.0>`_.
 
+0.3.2 (2024-05-31)
+==================
+
+Fixed
+-----
+- Fixed issues with smaller GPUs and NLPAR.
+- Improved the initial write of NLPAR file under Windows.
+- Fixed issue where user sends in non-numpy array of patterns to be indexed.
+
+
 0.3.1 (2024-05-24)
 ==================
 
 Fixed
 -----
 - Fixed issue when multiple OpenCL platforms are detected.  Will default to discrete GPUs, with whatever platform has the most discrete GPUs attached.  Otherwise, will fall back to integrated graphics.
```

### Comparing `pyebsdindex-0.3.1/IPFCubic.pdf` & `pyebsdindex-0.3.2/IPFCubic.pdf`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/IPFCubic.png` & `pyebsdindex-0.3.2/IPFCubic.png`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/IPFHex.pdf` & `pyebsdindex-0.3.2/IPFHex.pdf`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/IPFHex.png` & `pyebsdindex-0.3.2/IPFHex.png`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/License` & `pyebsdindex-0.3.2/License`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/PKG-INFO` & `pyebsdindex-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyebsdindex
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python based tool for Radon based EBSD indexing
 Home-page: https://pyebsdindex.readthedocs.io
 Download-URL: https://pypi.python.org/pypi/pyebsdindex
 Author: ['Dave Rowenhorst', 'Håkon Wiik Ånes']
 Maintainer: Dave Rowenhorst
 Maintainer-email: 
 License: Custom
```

### Comparing `pyebsdindex-0.3.1/README.md` & `pyebsdindex-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/RELEASE.rst` & `pyebsdindex-0.3.2/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/doc/Makefile` & `pyebsdindex-0.3.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/doc/_static/colormap_banners/banner0.png` & `pyebsdindex-0.3.2/doc/_static/colormap_banners/banner0.png`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/doc/_static/colormap_banners/banner1.png` & `pyebsdindex-0.3.2/doc/_static/colormap_banners/banner1.png`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/doc/_static/colormap_banners/create_colormap_banners.py` & `pyebsdindex-0.3.2/doc/_static/colormap_banners/create_colormap_banners.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/doc/_static/custom.css` & `pyebsdindex-0.3.2/doc/_static/custom.css`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/doc/_templates/custom-class-template.rst` & `pyebsdindex-0.3.2/doc/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/doc/_templates/custom-module-template.rst` & `pyebsdindex-0.3.2/doc/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/doc/conf.py` & `pyebsdindex-0.3.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/doc/dev/index.rst` & `pyebsdindex-0.3.2/doc/dev/index.rst`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/doc/index.rst` & `pyebsdindex-0.3.2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/doc/make.bat` & `pyebsdindex-0.3.2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/doc/reference/index.rst` & `pyebsdindex-0.3.2/doc/reference/index.rst`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/doc/tutorials/NLPAR_demo.ipynb` & `pyebsdindex-0.3.2/doc/tutorials/NLPAR_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/doc/tutorials/ebsd_index_demo.ipynb` & `pyebsdindex-0.3.2/doc/tutorials/ebsd_index_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/doc/user/installation.rst` & `pyebsdindex-0.3.2/doc/user/installation.rst`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/EBSDImage/IPFcolor.py` & `pyebsdindex-0.3.2/pyebsdindex/EBSDImage/IPFcolor.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/__init__.py` & `pyebsdindex-0.3.2/pyebsdindex/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Initial committer first, then sorted by line contributions
 __credits__ = [
     "Dave Rowenhorst",
     "Håkon Wiik Ånes",
 ]
 __description__ = "Python based tool for Radon based EBSD indexing"
 __name__ = "pyebsdindex"
-__version__ = "0.3.1"
+__version__ = "0.3.2"
 
 
 # Try to import only once - also will perform check that at least one GPU is found.
 try:
     _pyopencl_installed = False
     import pyopencl
     from pyebsdindex.opencl import openclparam
```

### Comparing `pyebsdindex-0.3.1/pyebsdindex/_ebsd_index_parallel.py` & `pyebsdindex-0.3.2/pyebsdindex/_ebsd_index_parallel.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/_ebsd_index_single.py` & `pyebsdindex-0.3.2/pyebsdindex/_ebsd_index_single.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/band_detect.py` & `pyebsdindex-0.3.2/pyebsdindex/band_detect.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/crystal_sym.py` & `pyebsdindex-0.3.2/pyebsdindex/crystal_sym.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/crystallometry.py` & `pyebsdindex-0.3.2/pyebsdindex/crystallometry.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/ebsd_index.py` & `pyebsdindex-0.3.2/pyebsdindex/ebsd_index.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/ebsd_pattern.py` & `pyebsdindex-0.3.2/pyebsdindex/ebsd_pattern.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/ebsdfile.py` & `pyebsdindex-0.3.2/pyebsdindex/ebsdfile.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/misorientation.py` & `pyebsdindex-0.3.2/pyebsdindex/misorientation.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/nlpar.py` & `pyebsdindex-0.3.2/pyebsdindex/nlpar.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/nlpar_cpu.py` & `pyebsdindex-0.3.2/pyebsdindex/nlpar_cpu.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/opencl/band_detect_cl.py` & `pyebsdindex-0.3.2/pyebsdindex/opencl/band_detect_cl.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,14 +221,16 @@
 
     return bandData
 
 
   def radon_fasterCL(self,image,padding = np.array([0,0]), fixArtifacts = False, background = None, returnBuff = True, clparams=None ):
     # this function executes the radon sumations on the GPU
     tic = timer()
+    image = np.asarray(image)
+
     # make sure we have an OpenCL environment
     if clparams is not None:
       if clparams.queue is None:
         clparams.get_queue()
       gpu = clparams.gpu
       gpu_id = clparams.gpu_id
       ctx = clparams.ctx
```

### Comparing `pyebsdindex-0.3.1/pyebsdindex/opencl/clkernels.cl` & `pyebsdindex-0.3.2/pyebsdindex/opencl/clkernels.cl`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/opencl/clnlpar.cl` & `pyebsdindex-0.3.2/pyebsdindex/opencl/clnlpar.cl`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/opencl/nlpar_cl.py` & `pyebsdindex-0.3.2/pyebsdindex/opencl/nlpar_cl.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,14 +260,15 @@
         toc = timer()
         #print(toc - tic)
 
         sigmachunk = np.zeros((nrowchunk, ncolchunk ), dtype=np.float32)
 
 
         sigmachunk_gpu =  cl.Buffer(ctx, mf.WRITE_ONLY, size=sigmachunk.nbytes)
+
         cl.enqueue_barrier(queue)
         prg.calcsigma(queue, (np.uint32(ncolchunk), np.uint32(nrowchunk)), None,
                                datapad_gpu, mask_gpu,sigmachunk_gpu,
                                dist_local, count_local,
                                np.int64(nn), np.int64(npatsteps), np.int64(npat_point),
                                np.float32(mxval) )
         if normalize_d is True:
@@ -400,15 +401,15 @@
     ctx = clparams.ctx
     prg = clparams.prg
     queue = clparams.queue
     mf = clparams.memflags
     clvectlen = 16
 
 
-
+    # print("target mem:", target_mem)
     chunks = self._calcchunks( [pwidth, pheight], ncols, nrows, target_bytes=target_mem,
                               col_overlap=sr, row_overlap=sr)
     #print(chunks[2], chunks[3])
     if verbose >=1:
       print("lambda:", lam, "search radius:", sr, "dthresh:", dthresh)
 
     # precalculate some needed arrays for the GPU
@@ -422,18 +423,22 @@
     npatsteps = int(maskpad.size/clvectlen) # how many clvector chunks to move through a pattern.
 
     chunksize = (chunks[2][:,1] - chunks[2][:,0]).reshape(1,-1) * \
                      (chunks[3][:, 1] - chunks[3][:, 0]).reshape(-1, 1)
     nchunks = chunksize.size
     #return chunks, chunksize
     mxchunk = int(chunksize.max())
+    # print("max chunk:" , mxchunk)
+
     npadmx = clvectlen * int(np.ceil(float(mxchunk)*npat_point/ clvectlen))
 
     datapad_gpu = cl.Buffer(ctx, mf.READ_WRITE, size=int(npadmx) * int(4))
     datapadout_gpu = cl.Buffer(ctx, mf.READ_WRITE, size=int(npadmx) * int(4))
+    # print("data pad", datapad_gpu.size)
+    # print("data out", datapadout_gpu.size)
 
     nnn = int((2 * sr + 1) ** 2)
 
 
     ndone = 0
     # if verbose >= 2:
     #   print('\n', end='')
@@ -465,22 +470,23 @@
           mxval *= 0.9961
 
         filldatain = cl.enqueue_fill_buffer(queue, datapad_gpu, np.float32(mxval+10), 0,int(4*npadmx))
         cl.enqueue_fill_buffer(queue, datapadout_gpu, np.float32(0.0), 0, int(4 * npadmx))
 
         sigmachunk = np.ascontiguousarray(sigma[rstart:rend, cstart:cend].astype(np.float32))
         sigmachunk_gpu = cl.Buffer(ctx, mf.READ_ONLY | mf.COPY_HOST_PTR, hostbuf=sigmachunk)
+        # print("sigma", sigmachunk_gpu.size)
         szdata = data.size
         npad = clvectlen * int(np.ceil(szdata / clvectlen))
 
         #datapad = np.zeros((npad), dtype=np.float32) + np.float32(mxval + 10)
         #datapad[0:szdata] = data.reshape(-1)
 
         data_gpu = cl.Buffer(ctx,mf.READ_ONLY | mf.COPY_HOST_PTR,hostbuf=data)
-
+        # print("data", data_gpu.size)
         if data.dtype.type is np.float32:
           prg.nlloadpat32flt(queue, (np.uint64(data.size),1), None, data_gpu, datapad_gpu, wait_for=[filldatain])
         if data.dtype.type is np.ubyte:
           prg.nlloadpat8bit(queue, (np.uint64(data.size),1), None, data_gpu, datapad_gpu, wait_for=[filldatain])
         if data.dtype.type is np.uint16:
           prg.nlloadpat16bit(queue, (np.uint64(data.size),1), None, data_gpu, datapad_gpu, wait_for=[filldatain])
```

### Comparing `pyebsdindex-0.3.1/pyebsdindex/opencl/nlpar_clray.py` & `pyebsdindex-0.3.2/pyebsdindex/opencl/nlpar_clray.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,17 +115,18 @@
     clparams.get_queue()
     if clparams.gpu[gpu_id].host_unified_memory:
       return nlpar_cl.NLPAR.calcsigma_cl(self, nn=nn, saturation_protect=saturation_protect,
                                          automask=automask,
                                          normalize_d=normalize_d,
                                          gpu_id=gpu_id, **kwargs)
 
-    target_mem = clparams.gpu[gpu_id].max_mem_alloc_size // 3
-    max_mem = clparams.gpu[gpu_id].global_mem_size * 0.75
+    target_mem = clparams.gpu[gpu_id].max_mem_alloc_size // 2
+    max_mem = clparams.gpu[gpu_id].global_mem_size * 0.5
     if target_mem * ngpuwrker > max_mem:
+      #print('revisemem:')
       target_mem = max_mem / ngpuwrker
 
     patternfile = self.getinfileobj()
 
     nrows = np.int64(self.nrows)  # np.uint64(patternfile.nRows)
     ncols = np.int64(self.ncols)  # np.uint64(patternfile.nCols)
 
@@ -475,15 +476,15 @@
                                          fileout=fileout,
                                          reset_sigma=reset_sigma,
                                          backsub = backsub,
                                          rescale = rescale,
                                          gpu_id= gpu_id)
 
     target_mem = clparams.gpu[gpu_id].max_mem_alloc_size//3
-    max_mem = clparams.gpu[gpu_id].global_mem_size*0.75
+    max_mem = clparams.gpu[gpu_id].global_mem_size*0.4
     if target_mem*ngpuwrker > max_mem:
       target_mem = max_mem/ngpuwrker
     #print(target_mem/1.0e9)
 
     chunks = self._calcchunks([pwidth, pheight], ncols, nrows, target_bytes=target_mem,
                               col_overlap=sr, row_overlap=sr)
 
@@ -541,15 +542,15 @@
 
     njobs = len(jobqueue)
     ndone = 0
     while ndone < njobs:
         if len(jobqueue) > 0:
             if len(idlewrker) > 0:
                 wrker = idlewrker.pop()
-                job = jobqueue.pop()
+                job = jobqueue.pop(0)
 
                 tasks.append(wrker.runnlpar_chunk.remote(job, nlparobj=nlpar_remote))
                 busywrker.append(wrker)
         if len(tasks) > 0:
             donetasks, stillbusy = ray.wait(tasks, num_returns=len(busywrker), timeout=0.1)
 
             for tsk in donetasks:
@@ -557,14 +558,18 @@
                 message, job, newdata = ray.get(tsk)
                 if message == 'Done':
                   idlewrker.append(busywrker.pop(indx))
                   tasks.remove(tsk)
                   ndone += 1
                   if verbose >= 2:
                     print("tiles complete: ", ndone, "/", njobs, sep='', end='\r')
+                else: #An error has occured ... hopefully just need a re-process.
+                  jobqueue.append(job)
+                  print(message)
+
     if verbose >= 2:
       print('\n', end='')
     return str(self.patternfileout.filepath)
 
   def _nlparchunkcalc_cl(self, data, calclim, clparams=None):
     data = np.ascontiguousarray(data)
     ctx = clparams.ctx
```

### Comparing `pyebsdindex-0.3.1/pyebsdindex/opencl/openclparam.py` & `pyebsdindex-0.3.2/pyebsdindex/opencl/openclparam.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 The US Naval Research Laboratory Date: 21 Aug 2020'''
 
 
 import numpy as np
 from os import path
 import pyopencl as cl
 from os import environ
-environ['PYOPENCL_COMPILER_OUTPUT'] = '1'
+environ['PYOPENCL_COMPILER_OUTPUT'] = '0'
 
 RADDEG = 180.0/np.pi
 DEGRAD = np.pi/180.0
 
 
 
 class OpenClParam():
```

### Comparing `pyebsdindex-0.3.1/pyebsdindex/opencl/radon_fast_cl.py` & `pyebsdindex-0.3.2/pyebsdindex/opencl/radon_fast_cl.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/opencl/test.cl` & `pyebsdindex-0.3.2/pyebsdindex/opencl/test.cl`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/pairlib.py` & `pyebsdindex-0.3.2/pyebsdindex/pairlib.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/pcopt.py` & `pyebsdindex-0.3.2/pyebsdindex/pcopt.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/radon_fast.py` & `pyebsdindex-0.3.2/pyebsdindex/radon_fast.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,28 +231,31 @@
       image = image.reshape(shapeIm)
 
     #print(timer()-tic)
     return radon
 
   def radon_faster(self,imageIn,padding = np.array([0,0]), fixArtifacts = False, background = None, normalization=True):
     tic = timer()
+
     shapeIm = np.shape(imageIn)
     if imageIn.ndim == 2:
       nIm = 1
       #image = image[np.newaxis, : ,:]
       #reform = True
     else:
       nIm = shapeIm[0]
     #  reform = False
 
+
     if background is None:
       image = (imageIn.reshape(-1)).astype(np.float32)
     else:
       image = imageIn - background
       image = (image.reshape(-1)).astype(np.float32)
+    image = np.asarray(image)
 
     nPx = shapeIm[-1]*shapeIm[-2]
     indxDim = np.asarray(self.indexPlan.shape)
     #radon = np.zeros([nIm, self.nRho+2*padding[0], self.nTheta+2*padding[1]], dtype=np.float32)
     radon = np.full([self.nRho + 2 * padding[0],self.nTheta + 2 * padding[1], nIm],self.missingval,dtype=np.float32)
     shp = radon.shape
```

### Comparing `pyebsdindex-0.3.1/pyebsdindex/rotations.py` & `pyebsdindex-0.3.2/pyebsdindex/rotations.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/rotlib.py` & `pyebsdindex-0.3.2/pyebsdindex/rotlib.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/tests/conftest.py` & `pyebsdindex-0.3.2/pyebsdindex/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/tests/data/al_sim_20kv/al_sim_20kv.png` & `pyebsdindex-0.3.2/pyebsdindex/tests/data/al_sim_20kv/al_sim_20kv.png`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/tests/data/al_sim_20kv/generate_al_sim_20kv.py` & `pyebsdindex-0.3.2/pyebsdindex/tests/data/al_sim_20kv/generate_al_sim_20kv.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/tests/numbatest.py` & `pyebsdindex-0.3.2/pyebsdindex/tests/numbatest.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/tests/raytest.py` & `pyebsdindex-0.3.2/pyebsdindex/tests/raytest.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/tests/rotlibunittest.py` & `pyebsdindex-0.3.2/pyebsdindex/tests/rotlibunittest.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/tests/test_ebsd_index.py` & `pyebsdindex-0.3.2/pyebsdindex/tests/test_ebsd_index.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/tests/test_package.py` & `pyebsdindex-0.3.2/pyebsdindex/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/tests/test_pcopt.py` & `pyebsdindex-0.3.2/pyebsdindex/tests/test_pcopt.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/tests/test_tripletvote.py` & `pyebsdindex-0.3.2/pyebsdindex/tests/test_tripletvote.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex/tripletvote.py` & `pyebsdindex-0.3.2/pyebsdindex/tripletvote.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex.egg-info/PKG-INFO` & `pyebsdindex-0.3.2/pyebsdindex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyebsdindex
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python based tool for Radon based EBSD indexing
 Home-page: https://pyebsdindex.readthedocs.io
 Download-URL: https://pypi.python.org/pypi/pyebsdindex
 Author: ['Dave Rowenhorst', 'Håkon Wiik Ånes']
 Maintainer: Dave Rowenhorst
 Maintainer-email: 
 License: Custom
```

### Comparing `pyebsdindex-0.3.1/pyebsdindex.egg-info/SOURCES.txt` & `pyebsdindex-0.3.2/pyebsdindex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/pyebsdindex.egg-info/requires.txt` & `pyebsdindex-0.3.2/pyebsdindex.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.3.1/setup.py` & `pyebsdindex-0.3.2/setup.py`

 * *Files identical despite different names*

