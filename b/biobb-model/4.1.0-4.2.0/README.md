# Comparing `tmp/biobb_model-4.1.0.tar.gz` & `tmp/biobb_model-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobb_model-4.1.0.tar", last modified: Thu Sep 14 10:12:44 2023, max compression
+gzip compressed data, was "biobb_model-4.2.0.tar", last modified: Fri May 31 13:31:22 2024, max compression
```

## Comparing `biobb_model-4.1.0.tar` & `biobb_model-4.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-09-14 10:12:44.212674 biobb_model-4.1.0/
--rwxr-xr-x   0 pau        (501) staff       (20)    11358 2021-06-11 09:52:05.000000 biobb_model-4.1.0/LICENSE
--rw-r--r--   0 pau        (501) staff       (20)     6202 2023-09-14 10:12:44.212378 biobb_model-4.1.0/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)     5251 2023-09-14 10:10:11.000000 biobb_model-4.1.0/README.md
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-09-14 10:12:44.205312 biobb_model-4.1.0/biobb_model/
--rwxr-xr-x   0 pau        (501) staff       (20)       63 2023-09-14 10:09:21.000000 biobb_model-4.1.0/biobb_model/__init__.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-09-14 10:12:44.211732 biobb_model-4.1.0/biobb_model/model/
--rwxr-xr-x   0 pau        (501) staff       (20)      157 2022-11-02 12:01:31.000000 biobb_model-4.1.0/biobb_model/model/__init__.py
--rwxr-xr-x   0 pau        (501) staff       (20)     5196 2023-04-05 06:36:46.000000 biobb_model-4.1.0/biobb_model/model/checking_log.py
--rw-r--r--   0 pau        (501) staff       (20)      716 2023-04-05 06:37:11.000000 biobb_model-4.1.0/biobb_model/model/common.py
--rwxr-xr-x   0 pau        (501) staff       (20)     5605 2023-03-23 12:01:36.000000 biobb_model-4.1.0/biobb_model/model/fix_altlocs.py
--rwxr-xr-x   0 pau        (501) staff       (20)     5142 2023-03-27 10:29:40.000000 biobb_model-4.1.0/biobb_model/model/fix_amides.py
--rwxr-xr-x   0 pau        (501) staff       (20)     7211 2023-03-27 09:39:08.000000 biobb_model-4.1.0/biobb_model/model/fix_backbone.py
--rwxr-xr-x   0 pau        (501) staff       (20)     5263 2023-03-27 10:32:27.000000 biobb_model-4.1.0/biobb_model/model/fix_chirality.py
--rw-r--r--   0 pau        (501) staff       (20)     6145 2023-03-27 10:33:54.000000 biobb_model-4.1.0/biobb_model/model/fix_pdb.py
--rw-r--r--   0 pau        (501) staff       (20)    46058 2023-04-05 08:36:34.000000 biobb_model-4.1.0/biobb_model/model/fix_pdb_utils.py
--rwxr-xr-x   0 pau        (501) staff       (20)     6148 2023-03-27 10:33:01.000000 biobb_model-4.1.0/biobb_model/model/fix_side_chain.py
--rwxr-xr-x   0 pau        (501) staff       (20)     5117 2023-03-27 10:28:39.000000 biobb_model-4.1.0/biobb_model/model/fix_ssbonds.py
--rwxr-xr-x   0 pau        (501) staff       (20)     6529 2023-04-04 17:32:15.000000 biobb_model-4.1.0/biobb_model/model/mutate.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-09-14 10:12:44.212068 biobb_model-4.1.0/biobb_model/test/
--rwxr-xr-x   0 pau        (501) staff       (20)        0 2021-06-11 09:52:05.000000 biobb_model-4.1.0/biobb_model/test/__init__.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-09-14 10:12:44.207378 biobb_model-4.1.0/biobb_model.egg-info/
--rw-r--r--   0 pau        (501) staff       (20)     6202 2023-09-14 10:12:44.000000 biobb_model-4.1.0/biobb_model.egg-info/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)      678 2023-09-14 10:12:44.000000 biobb_model-4.1.0/biobb_model.egg-info/SOURCES.txt
--rw-r--r--   0 pau        (501) staff       (20)        1 2023-09-14 10:12:44.000000 biobb_model-4.1.0/biobb_model.egg-info/dependency_links.txt
--rw-r--r--   0 pau        (501) staff       (20)      453 2023-09-14 10:12:44.000000 biobb_model-4.1.0/biobb_model.egg-info/entry_points.txt
--rw-r--r--   0 pau        (501) staff       (20)       63 2023-09-14 10:12:44.000000 biobb_model-4.1.0/biobb_model.egg-info/requires.txt
--rw-r--r--   0 pau        (501) staff       (20)       12 2023-09-14 10:12:44.000000 biobb_model-4.1.0/biobb_model.egg-info/top_level.txt
--rw-r--r--   0 pau        (501) staff       (20)       38 2023-09-14 10:12:44.212774 biobb_model-4.1.0/setup.cfg
--rw-r--r--   0 pau        (501) staff       (20)     1976 2023-09-14 08:49:20.000000 biobb_model-4.1.0/setup.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-31 13:31:22.385570 biobb_model-4.2.0/
+-rwxr-xr-x   0 pau        (501) staff       (20)    11358 2021-06-11 09:52:05.000000 biobb_model-4.2.0/LICENSE
+-rw-r--r--   0 pau        (501) staff       (20)     6741 2024-05-31 13:31:22.385229 biobb_model-4.2.0/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)     5790 2024-05-31 13:27:58.000000 biobb_model-4.2.0/README.md
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-31 13:31:22.374365 biobb_model-4.2.0/biobb_model/
+-rwxr-xr-x   0 pau        (501) staff       (20)       84 2024-05-31 13:26:18.000000 biobb_model-4.2.0/biobb_model/__init__.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-31 13:31:22.384284 biobb_model-4.2.0/biobb_model/model/
+-rwxr-xr-x   0 pau        (501) staff       (20)      600 2024-05-30 08:58:28.000000 biobb_model-4.2.0/biobb_model/model/__init__.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     5254 2024-05-30 09:21:06.000000 biobb_model-4.2.0/biobb_model/model/checking_log.py
+-rw-r--r--   0 pau        (501) staff       (20)      782 2024-05-30 09:23:25.000000 biobb_model-4.2.0/biobb_model/model/common.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     5730 2024-05-30 09:23:59.000000 biobb_model-4.2.0/biobb_model/model/fix_altlocs.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     5200 2024-05-30 09:24:06.000000 biobb_model-4.2.0/biobb_model/model/fix_amides.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     7273 2024-05-30 09:24:35.000000 biobb_model-4.2.0/biobb_model/model/fix_backbone.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     5321 2024-05-30 09:24:20.000000 biobb_model-4.2.0/biobb_model/model/fix_chirality.py
+-rw-r--r--   0 pau        (501) staff       (20)     6349 2024-05-30 12:06:00.000000 biobb_model-4.2.0/biobb_model/model/fix_pdb.py
+-rw-r--r--   0 pau        (501) staff       (20)    46930 2024-05-30 12:04:02.000000 biobb_model-4.2.0/biobb_model/model/fix_pdb_utils.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     6206 2024-05-30 12:06:21.000000 biobb_model-4.2.0/biobb_model/model/fix_side_chain.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     5218 2024-05-30 12:06:32.000000 biobb_model-4.2.0/biobb_model/model/fix_ssbonds.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     6591 2024-05-30 12:06:47.000000 biobb_model-4.2.0/biobb_model/model/mutate.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-31 13:31:22.384885 biobb_model-4.2.0/biobb_model/test/
+-rwxr-xr-x   0 pau        (501) staff       (20)        0 2021-06-11 09:52:05.000000 biobb_model-4.2.0/biobb_model/test/__init__.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-31 13:31:22.376548 biobb_model-4.2.0/biobb_model.egg-info/
+-rw-r--r--   0 pau        (501) staff       (20)     6741 2024-05-31 13:31:22.000000 biobb_model-4.2.0/biobb_model.egg-info/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)      678 2024-05-31 13:31:22.000000 biobb_model-4.2.0/biobb_model.egg-info/SOURCES.txt
+-rw-r--r--   0 pau        (501) staff       (20)        1 2024-05-31 13:31:22.000000 biobb_model-4.2.0/biobb_model.egg-info/dependency_links.txt
+-rw-r--r--   0 pau        (501) staff       (20)      453 2024-05-31 13:31:22.000000 biobb_model-4.2.0/biobb_model.egg-info/entry_points.txt
+-rw-r--r--   0 pau        (501) staff       (20)       63 2024-05-31 13:31:22.000000 biobb_model-4.2.0/biobb_model.egg-info/requires.txt
+-rw-r--r--   0 pau        (501) staff       (20)       12 2024-05-31 13:31:22.000000 biobb_model-4.2.0/biobb_model.egg-info/top_level.txt
+-rw-r--r--   0 pau        (501) staff       (20)       38 2024-05-31 13:31:22.385666 biobb_model-4.2.0/setup.cfg
+-rw-r--r--   0 pau        (501) staff       (20)     1976 2024-05-31 13:25:04.000000 biobb_model-4.2.0/setup.py
```

### Comparing `biobb_model-4.1.0/LICENSE` & `biobb_model-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_model-4.1.0/PKG-INFO` & `biobb_model-4.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: biobb_model
-Version: 4.1.0
+Version: 4.2.0
 Summary: Biobb_model is the Biobb module collection to check and model 3d structures, create mutations or reconstruct missing atoms.
 Home-page: https://github.com/bioexcel/biobb_model
 Author: Biobb developers
 Author-email: pau.andrio@bsc.es
-Project-URL: Documentation, http://biobb_model.readthedocs.io/en/latest/
+Project-URL: Documentation, http://biobb-model.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,15 +21,15 @@
 License-File: LICENSE
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_model?label=Version)](https://GitHub.com/bioexcel/biobb_model/tags/)
 [![](https://img.shields.io/pypi/v/biobb-model.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-model/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_model?label=Conda)](https://anaconda.org/bioconda/biobb_model)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_model?label=Conda%20downloads)](https://anaconda.org/bioconda/biobb_model)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_model?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_model:4.1.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_model:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_model)
 [![](https://img.shields.io/pypi/pyversions/biobb-model.svg?label=Python%20Versions)](https://pypi.org/project/biobb-model/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_model)
 
 [![](https://readthedocs.org/projects/biobb-model/badge/?version=latest&label=Docs)](https://biobb-model.readthedocs.io/en/latest/?badge=latest)
@@ -40,63 +40,70 @@
 
 [![](https://docs.bioexcel.eu/biobb_model/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_model/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_model/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_model/coverage/)
 [![](https://docs.bioexcel.eu/biobb_model/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_model/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_model?label=Last%20Commit)](https://github.com/bioexcel/biobb_model/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_model.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_model/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 # biobb_model
 
 ### Introduction
 Biobb_model is the Biobb module collection to check and model 3d structures,
 create mutations or reconstruct missing atoms.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
-[latest API documentation](http://biobb_model.readthedocs.io/en/latest/).
+[latest API documentation](http://biobb-model.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2023.4
+v4.2.0 2024.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_model>=4.1.0"
+        pip install "biobb_model>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-model.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_model>=4.1.0"
+        conda install -c bioconda "biobb_model>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-model.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-model.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_model:4.1.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_model:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_model:4.1.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_model:4.2.0--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
@@ -113,14 +120,14 @@
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-model.readthedocs.io/en/latest/command_line.html).
 
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2024 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2024 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
```

### Comparing `biobb_model-4.1.0/README.md` & `biobb_model-4.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_model?label=Version)](https://GitHub.com/bioexcel/biobb_model/tags/)
 [![](https://img.shields.io/pypi/v/biobb-model.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-model/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_model?label=Conda)](https://anaconda.org/bioconda/biobb_model)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_model?label=Conda%20downloads)](https://anaconda.org/bioconda/biobb_model)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_model?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_model:4.1.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_model:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_model)
 [![](https://img.shields.io/pypi/pyversions/biobb-model.svg?label=Python%20Versions)](https://pypi.org/project/biobb-model/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_model)
 
 [![](https://readthedocs.org/projects/biobb-model/badge/?version=latest&label=Docs)](https://biobb-model.readthedocs.io/en/latest/?badge=latest)
@@ -18,63 +18,70 @@
 
 [![](https://docs.bioexcel.eu/biobb_model/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_model/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_model/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_model/coverage/)
 [![](https://docs.bioexcel.eu/biobb_model/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_model/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_model?label=Last%20Commit)](https://github.com/bioexcel/biobb_model/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_model.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_model/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 # biobb_model
 
 ### Introduction
 Biobb_model is the Biobb module collection to check and model 3d structures,
 create mutations or reconstruct missing atoms.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
-[latest API documentation](http://biobb_model.readthedocs.io/en/latest/).
+[latest API documentation](http://biobb-model.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2023.4
+v4.2.0 2024.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_model>=4.1.0"
+        pip install "biobb_model>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-model.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_model>=4.1.0"
+        conda install -c bioconda "biobb_model>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-model.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-model.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_model:4.1.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_model:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_model:4.1.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_model:4.2.0--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
@@ -91,14 +98,14 @@
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-model.readthedocs.io/en/latest/command_line.html).
 
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2024 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2024 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
```

### Comparing `biobb_model-4.1.0/biobb_model/model/checking_log.py` & `biobb_model-4.2.0/biobb_model/model/checking_log.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 
 """Module containing the CheckingLog class and the command line interface."""
 import argparse
+from typing import Dict, Optional
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
 
 
 class CheckingLog(BiobbObject):
     """
@@ -36,15 +37,15 @@
             * name: In house
             * license: Apache-2.0
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
     """
 
-    def __init__(self, input_pdb_path: str, output_log_path: str, properties: dict = None, **kwargs) -> None:
+    def __init__(self, input_pdb_path: str, output_log_path: str, properties: Optional[Dict] = None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
@@ -83,22 +84,22 @@
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
         # Remove temporal files
-        self.tmp_files.extend([self.stage_io_dict.get("unique_dir")])
+        self.tmp_files.extend([self.stage_io_dict.get("unique_dir", "")])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
         return self.return_code
 
 
-def checking_log(input_pdb_path: str, output_log_path: str, properties: dict = None, **kwargs) -> int:
+def checking_log(input_pdb_path: str, output_log_path: str, properties: Optional[Dict] = None, **kwargs) -> int:
     """Create :class:`CheckingLog <model.checking_log.CheckingLog>` class and
     execute the :meth:`launch() <model.checking_log.CheckingLog.launch>` method."""
     return CheckingLog(input_pdb_path=input_pdb_path,
                        output_log_path=output_log_path,
                        properties=properties, **kwargs).launch()
```

### Comparing `biobb_model-4.1.0/biobb_model/model/common.py` & `biobb_model-4.2.0/biobb_model/model/common.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """ Common functions for package biobb_model.model """
 from biobb_common.tools import file_utils as fu
+from typing import Optional
 import logging
 
 
-def modeller_installed(out_log: logging.Logger = None, global_log: logging.Logger = None) -> bool:
+def modeller_installed(out_log: Optional[logging.Logger] = None, global_log: Optional[logging.Logger] = None) -> bool:
     try:
-        import modeller
+        import modeller  # type: ignore
         from modeller import automodel
         fu.log(f"Modeller is installed in your environment. Modeller version: {modeller.__version__}", out_log, global_log)
-        fu.log(f"Modeller automodel class: {automodel.automodel}", out_log=out_log)
+        fu.log(f"Modeller automodel class: {automodel.automodel}", local_log=out_log)
     except ImportError:
         fu.log("Modeller is not installed in your environment.\nPlease install it by typing:\n\nconda install -c salilab modeller\n", out_log, global_log)
         return False
 
     return True
```

### Comparing `biobb_model-4.1.0/biobb_model/model/fix_altlocs.py` & `biobb_model-4.2.0/biobb_model/model/fix_altlocs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 #!/usr/bin/env python3
 
 """Module containing the FixAltLocs class and the command line interface."""
 import argparse
+from typing import Dict, Optional
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
 
 
 class FixAltLocs(BiobbObject):
     """
     | biobb_model FixAltLocs
     | Fix alternate locations from residues.
+    | Fix alternate locations using the altlocs list or occupancy.
 
     Args:
         input_pdb_path (str): Input PDB file path. File type: input. `Sample file <https://github.com/bioexcel/biobb_model/raw/master/biobb_model/test/data/model/3ebp.pdb>`_. Accepted formats: pdb (edam:format_1476).
         output_pdb_path (str): Output PDB file path. File type: output. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_model/master/biobb_model/test/reference/model/output_altloc.pdb>`_. Accepted formats: pdb (edam:format_1476).
         properties (dict - Python dictionary object containing the tool parameters, not input/output files):
             * **altlocs** (*list*) - (None) List of alternate locations to fix. Format: ["A339:A", "A171:B", "A768:A"]; where for each residue the format is as follows: "<chain><residue id>:<chosen alternate location>". If empty, no action will be executed.
             * **modeller_key** (*str*) - (None) Modeller license key.
@@ -36,15 +38,15 @@
             * name: In house
             * license: Apache-2.0
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
     """
 
-    def __init__(self, input_pdb_path: str, output_pdb_path: str, properties: dict = None, **kwargs) -> None:
+    def __init__(self, input_pdb_path: str, output_pdb_path: str, properties: Optional[Dict] = None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
@@ -90,22 +92,22 @@
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
         # Remove temporal files
-        self.tmp_files.extend([self.stage_io_dict.get("unique_dir")])
+        self.tmp_files.extend([self.stage_io_dict.get("unique_dir", "")])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
         return self.return_code
 
 
-def fix_altlocs(input_pdb_path: str, output_pdb_path: str, properties: dict = None, **kwargs) -> int:
+def fix_altlocs(input_pdb_path: str, output_pdb_path: str, properties: Optional[Dict] = None, **kwargs) -> int:
     """Create :class:`FixAltLocs <model.fix_altlocs.FixAltLocs>` class and
     execute the :meth:`launch() <model.fix_altlocs.FixAltLocs.launch>` method."""
     return FixAltLocs(input_pdb_path=input_pdb_path,
                       output_pdb_path=output_pdb_path,
                       properties=properties, **kwargs).launch()
```

### Comparing `biobb_model-4.1.0/biobb_model/model/fix_amides.py` & `biobb_model-4.2.0/biobb_model/model/fix_amides.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 
 """Module containing the FixAmides class and the command line interface."""
 import argparse
+from typing import Dict, Optional
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
 
 
 class FixAmides(BiobbObject):
     """
@@ -36,15 +37,15 @@
             * name: In house
             * license: Apache-2.0
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
     """
 
-    def __init__(self, input_pdb_path: str, output_pdb_path: str, properties: dict = None, **kwargs) -> None:
+    def __init__(self, input_pdb_path: str, output_pdb_path: str, properties: Optional[Dict] = None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
@@ -83,22 +84,22 @@
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
         # Remove temporal files
-        self.tmp_files.extend([self.stage_io_dict.get("unique_dir")])
+        self.tmp_files.extend([self.stage_io_dict.get("unique_dir", "")])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
         return self.return_code
 
 
-def fix_amides(input_pdb_path: str, output_pdb_path: str, properties: dict = None, **kwargs) -> int:
+def fix_amides(input_pdb_path: str, output_pdb_path: str, properties: Optional[Dict] = None, **kwargs) -> int:
     """Create :class:`FixAmides <model.fix_amides.FixAmides>` class and
     execute the :meth:`launch() <model.fix_amides.FixAmides.launch>` method."""
     return FixAmides(input_pdb_path=input_pdb_path,
                      output_pdb_path=output_pdb_path,
                      properties=properties, **kwargs).launch()
```

### Comparing `biobb_model-4.1.0/biobb_model/model/fix_backbone.py` & `biobb_model-4.2.0/biobb_model/model/fix_backbone.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 
 """Module containing the FixBackbone class and the command line interface."""
 import argparse
+from typing import Dict, Optional
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
 
 
 class FixBackbone(BiobbObject):
@@ -41,15 +42,15 @@
             * license: Apache-2.0
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
     """
 
     def __init__(self, input_pdb_path: str, input_fasta_canonical_sequence_path: str, output_pdb_path: str,
-                 properties: dict = None, **kwargs) -> None:
+                 properties: Optional[Dict] = None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
@@ -108,24 +109,24 @@
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
         # Remove temporal files
-        self.tmp_files.extend([self.io_dict['in'].get("stdin_file_path")])
-        self.tmp_files.extend([self.stage_io_dict.get("unique_dir")])
+        self.tmp_files.extend([self.io_dict['in'].get("stdin_file_path", "")])
+        self.tmp_files.extend([self.stage_io_dict.get("unique_dir", "")])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
         return self.return_code
 
 
 def fix_backbone(input_pdb_path: str, input_fasta_canonical_sequence_path: str, output_pdb_path: str,
-                 properties: dict = None, **kwargs) -> int:
+                 properties: Optional[Dict] = None, **kwargs) -> int:
     """Create :class:`FixBackbone <model.fix_backbone.FixBackbone>` class and
     execute the :meth:`launch() <model.fix_backbone.FixBackbone.launch>` method."""
     return FixBackbone(input_pdb_path=input_pdb_path,
                        input_fasta_canonical_sequence_path=input_fasta_canonical_sequence_path,
                        output_pdb_path=output_pdb_path,
                        properties=properties, **kwargs).launch()
```

### Comparing `biobb_model-4.1.0/biobb_model/model/fix_chirality.py` & `biobb_model-4.2.0/biobb_model/model/fix_chirality.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 
 """Module containing the FixChirality class and the command line interface."""
 import argparse
+from typing import Dict, Optional
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
 
 
 class FixChirality(BiobbObject):
     """
@@ -36,15 +37,15 @@
             * name: In house
             * license: Apache-2.0
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
     """
 
-    def __init__(self, input_pdb_path: str, output_pdb_path: str, properties: dict = None, **kwargs) -> None:
+    def __init__(self, input_pdb_path: str, output_pdb_path: str, properties: Optional[Dict] = None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
@@ -84,22 +85,22 @@
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
         # Remove temporal files
-        self.tmp_files.extend([self.stage_io_dict.get("unique_dir")])
+        self.tmp_files.extend([self.stage_io_dict.get("unique_dir", "")])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
         return self.return_code
 
 
-def fix_chirality(input_pdb_path: str, output_pdb_path: str, properties: dict = None, **kwargs) -> int:
+def fix_chirality(input_pdb_path: str, output_pdb_path: str, properties: Optional[Dict] = None, **kwargs) -> int:
     """Create :class:`FixChirality <model.fix_amides.FixChirality>` class and
     execute the :meth:`launch() <model.fix_amides.FixChirality.launch>` method."""
     return FixChirality(input_pdb_path=input_pdb_path,
                         output_pdb_path=output_pdb_path,
                         properties=properties, **kwargs).launch()
```

### Comparing `biobb_model-4.1.0/biobb_model/model/fix_pdb.py` & `biobb_model-4.2.0/biobb_model/model/fix_pdb.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 #!/usr/bin/env python3
 
 """Module containing the FixPdb class and the command line interface."""
 import argparse
+from typing import Dict, Optional
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
 
 from .fix_pdb_utils import Structure, generate_map_online
 
 
 class FixPdb(BiobbObject):
     """
     | biobb_model FixPdb
     | Class to renumerate residues in a PDB structure according to a reference sequence from UniProt.
+    | Fix the residue numbering in a PDB structure according to a reference sequence from UniProt.
+
     Args:
         input_pdb_path (str): Input PDB file path. File type: input. `Sample file <https://github.com/bioexcel/biobb_model/raw/master/biobb_model/test/data/model/2ki5.pdb>`_. Accepted formats: pdb (edam:format_1476).
         output_pdb_path (str): Output PDB file path. File type: output. `Sample file <https://github.com/bioexcel/biobb_model/raw/master/biobb_model/test/reference/model/output_pdb_path.pdb>`_. Accepted formats: pdb (edam:format_1476).
         properties (dict - Python dictionary object containing the tool parameters, not input/output files):
             * **forced_uniprot_references** (*str*) - (None) Set the UniProt accessions for sequences to be used as reference.
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
@@ -30,15 +33,15 @@
             * name: In house
             * license: Apache-2.0
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
     """
 
-    def __init__(self, input_pdb_path: str, output_pdb_path: str, properties: dict = None, **kwargs) -> None:
+    def __init__(self, input_pdb_path: str, output_pdb_path: str, properties: Optional[Dict] = None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
@@ -46,15 +49,15 @@
             "in": {"input_pdb_path": input_pdb_path},
             "out": {"output_pdb_path": output_pdb_path}
         }
 
         # Properties specific for BB
         self.forced_uniprot_references = properties.get('forced_uniprot_references')
         # If input forced uniprot references is a string and not a list then convert it
-        if type(self.forced_uniprot_references) == str:
+        if isinstance(self.forced_uniprot_references, str):
             self.forced_uniprot_references = self.forced_uniprot_references.split(' ')
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     @launchlogger
@@ -78,15 +81,16 @@
 
         # Add protein chains in case they are missing
         chains = structure.chains
         if len(chains) == 0 or (len(chains) == 1 and (chains[0].name == ' ' or chains[0].name == 'X')):
             structure.raw_protein_chainer()
 
         # Run all the mapping function
-        mapping = generate_map_online(structure, forced_uniprot_references)
+        if forced_uniprot_references:
+            mapping = generate_map_online(structure, forced_uniprot_references)
 
         # In case something went wrong with the mapping stop here
         if not mapping:
             self.return_code = -1
             return self.return_code
 
         # Change residue numbers in the structure according to the mapping results
@@ -99,22 +103,22 @@
 
         # Write the modified structure to a new pdb file
         structure.generate_pdb_file(output_pdb_path)
 
         print('Fixed :)')
 
         # Remove temporal files
-        self.tmp_files.extend([self.stage_io_dict.get("unique_dir")])
+        self.tmp_files.extend([self.stage_io_dict.get("unique_dir", "")])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
         return self.return_code
 
 
-def fix_pdb(input_pdb_path: str, output_pdb_path: str, properties: dict = None, **kwargs) -> int:
+def fix_pdb(input_pdb_path: str, output_pdb_path: str, properties: Optional[Dict] = None, **kwargs) -> int:
     """Create :class:`FixPdb <model.fix_pdb.FixPdb>` class and
     execute the :meth:`launch() <model.fix_pdb.FixPdb.launch>` method."""
     return FixPdb(input_pdb_path=input_pdb_path,
                   output_pdb_path=output_pdb_path,
                   properties=properties, **kwargs).launch()
```

### Comparing `biobb_model-4.1.0/biobb_model/model/fix_pdb_utils.py` & `biobb_model-4.2.0/biobb_model/model/fix_pdb_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 import os
 import urllib.request
 import json
 import math
 from bisect import bisect
-from Bio import pairwise2
-from Bio.pairwise2 import format_alignment
-from Bio.Blast import NCBIWWW
-import xmltodict
+from Bio import pairwise2  # type: ignore
+from Bio.pairwise2 import format_alignment  # type: ignore
+from Bio.Blast import NCBIWWW  # type: ignore
+import xmltodict  # type: ignore
 from typing import List, Tuple, Optional, Union
 Coords = Tuple[float, float, float]
 
 try:
-    from Bio.SubsMat import MatrixInfo
+    from Bio.SubsMat import MatrixInfo  # type: ignore
     blosum62 = MatrixInfo.blosum62
 except ImportError:
-    from Bio.Align import substitution_matrices
+    from Bio.Align import substitution_matrices  # type: ignore
     blosum62 = substitution_matrices.load("BLOSUM62")
 
 
 # An atom
 class Atom:
     def __init__(self, name: Optional[str] = None, element: Optional[str] = None, coords: Optional[Coords] = None):
         self.name = name
         self.element = element
         self.coords = coords
         # Set variables to store references to other related instances
         # These variables will be set further by the structure
-        self._structure = None
-        self._index = None
-        self._residue_index = None
+        self._structure: Optional[Structure] = None
+        self._index: Optional[int] = None
+        self._residue_index: Optional[int] = None
 
     def __repr__(self):
-        return '<Atom ' + self.name + '>'
+        return '<Atom ' + str(self.name) + '>'
 
     def __eq__(self, other):
         return self._residue_index == other._residue_index and self.name == other.name
 
     # The parent structure (read only)
     # This value is set by the structure itself
     def get_structure(self):
@@ -46,15 +46,15 @@
     # This value is set by the structure itself
     def get_index(self):
         return self._index
     index = property(get_index, None, None, "The residue index according to parent structure residues (read only)")
 
     # The atom residue index according to parent structure residues
     # If residue index is set then make changes in all the structure to make this change coherent
-    def get_residue_index(self) -> int:
+    def get_residue_index(self) -> Optional[int]:
         return self._residue_index
 
     def set_residue_index(self, new_residue_index: int):
         # If there is not strucutre yet it means the residue is beeing set before the structure
         # We just save the residue index and wait for the structure to be set
         if not self.structure:
             self._residue_index = new_residue_index
@@ -65,15 +65,15 @@
         current_residue.remove_atom(self)
         new_residue = self.structure.residues[new_residue_index]
         new_residue.add_atom(self)
     residue_index = property(get_residue_index, set_residue_index, None, "The atom residue index according to parent structure residues")
 
     # The atom residue
     # If residue is set then make changes in all the structure to make this change coherent
-    def get_residue(self) -> 'Residue':
+    def get_residue(self) -> Optional['Residue']:
         # If there is not strucutre yet it means the atom is beeing set before the structure
         # In this case it is not possible to get related residues in the structure
         if not self.structure:
             return None
         # Get the residue in the structure according to the residue index
         return self.structure.residues[self.residue_index]
 
@@ -104,24 +104,24 @@
 class Residue:
     def __init__(self, name: Optional[str] = None, number: Optional[int] = None, icode: Optional[str] = None):
         self.name = name
         self.number = number
         self.icode = icode
         # Set variables to store references to other related instaces
         # These variables will be set further by the structure
-        self._structure = None
-        self._index = None
-        self._atom_indices = []
-        self._chain_index = None
+        self._structure: Optional[Structure] = None
+        self._index: Optional[int] = None
+        self._atom_indices: List[int] = []
+        self._chain_index: Optional[int] = None
 
     def __repr__(self):
-        return '<Residue ' + self.name + str(self.number) + (self.icode if self.icode else '') + '>'
+        return '<Residue ' + str(self.name) + str(self.number) + (self.icode if self.icode else '') + '>'
 
     def __eq__(self, other):
-        if type(self) != type(other):
+        if not isinstance(self, type(other)):
             return False
         return (self._chain_index == other._chain_index and self.number == other.number and self.icode == other.icode)
 
     def __hash__(self):
         # WARNING: This is susceptible to duplicated residues
         return hash((self._chain_index, self.number, self.icode))
         # WARNING: This is not susceptible to duplicated residues
@@ -205,15 +205,15 @@
         # Remove the current atom index from the atom indices list
         self.atom_indices.remove(current_atom.index)  # This index MUST be in the list
         # Update the atom internal index
         current_atom._residue_index = None
 
     # The residue chain index according to parent structure chains
     # If chain index is set then make changes in all the structure to make this change coherent
-    def get_chain_index(self) -> int:
+    def get_chain_index(self) -> Optional[int]:
         return self._chain_index
 
     def set_chain_index(self, new_chain_index: int):
         # If there is not strucutre yet it means the chain is beeing set before the structure
         # We just save the chain index and wait for the structure to be set
         if not self.structure:
             self._chain_index = new_chain_index
@@ -227,25 +227,25 @@
         new_chain = self.structure.chains[new_chain_index]
         current_chain.remove_residue(self)
         new_chain.add_residue(self)
     chain_index = property(get_chain_index, set_chain_index, None, "The residue chain index according to parent structure chains")
 
     # The residue chain
     # If chain is set then make changes in all the structure to make this change coherent
-    def get_chain(self) -> 'Chain':
+    def get_chain(self) -> Union['Chain', List]:
         # If there is not strucutre yet it means the residue is beeing set before the structure
         # In this case it is not possible to get related chain in the structure
         if not self.structure:
             return []
         # Get the chain in the structure according to the chain index
         return self.structure.chains[self.chain_index]
 
     def set_chain(self, new_chain: Union['Chain', str]):
         # In case the chain is just a string we must find/create the corresponding chain
-        if type(new_chain) == str:
+        if isinstance(new_chain, str):
             letter = new_chain
             # Get the residue structure
             structure = self.structure
             if not structure:
                 raise ValueError('Cannot find the corresponding ' + new_chain + ' chain without the structure')
             # Find if the letter belongs to an already existing chain
             new_chain = structure.get_chain_by_name(letter)
@@ -254,30 +254,31 @@
                 new_chain = Chain(name=letter)
                 structure.set_new_chain(new_chain)
         # Find the new chain index and set it as the residue chain index
         # Note that the chain must be set in the structure already
         new_chain_index = new_chain.index
         if new_chain_index is None:
             raise ValueError('Chain ' + str(new_chain) + ' is not set in the structure')
-        self.set_chain_index(new_chain_index)
+        if isinstance(new_chain_index, int):
+            self.set_chain_index(new_chain_index)
     chain = property(get_chain, set_chain, None, "The residue chain")
 
 
 # A chain
 class Chain:
     def __init__(self, name: Optional[str] = None):
         self.name = name
         # Set variables to store references to other related instaces
         # These variables will be set further by the structure
-        self._structure = None
-        self._index = None
+        self._structure: Optional[Structure] = None
+        self._index: Optional[int] = None
         self.residue_indices = []
 
     def __repr__(self):
-        return '<Chain ' + self.name + '>'
+        return '<Chain ' + str(self.name) + '>'
 
     def __eq__(self, other):
         return self.name == other.name
 
     # The parent structure(read only)
     # This value is set by the structure itself
     def get_structure(self):
@@ -378,17 +379,17 @@
     def get_sequence(self) -> str:
         return ''.join([residue_name_2_letter(residue.name) for residue in self.residues])
 
 
 # A structure is a group of atoms organized in chains and residues
 class Structure:
     def __init__(self, atoms: List['Atom'] = [], residues: List['Residue'] = [], chains: List['Chain'] = []):
-        self.atoms = []
-        self.residues = []
-        self.chains = []
+        self.atoms: List[Atom] = []
+        self.residues: List[Residue] = []
+        self.chains: List[Chain] = []
         # Set references between instances
         for atom in atoms:
             self.set_new_atom(atom)
         for residue in residues:
             self.set_new_residue(residue)
         for chain in chains:
             self.set_new_chain(chain)
@@ -429,17 +430,17 @@
 
     # Purge chain from the structure
     # This can be done only when the chain has no residues left in the structure
     # Renumerate all chain indices which have been offsetted as a result of the purge
     def purge_chain(self, chain: 'Chain'):
         # Check the chain can be purged
         if chain not in self.chains:
-            raise ValueError('Chain ' + chain.name + ' is not in the structure already')
+            raise ValueError('Chain ' + str(chain.name) + ' is not in the structure already')
         if len(chain.residue_indices) > 0:
-            raise ValueError('Chain ' + chain.name + ' is still having residues and thus it cannot be purged')
+            raise ValueError('Chain ' + str(chain.name) + ' is still having residues and thus it cannot be purged')
         # Get the current index of the chain to be purged
         purged_index = chain.index
         # Chains and their residues below this index are not to be modified
         # Chains and their residues over this index must be renumerated
         for affected_chain in self.chains[purged_index+1:]:
             # Chaging the index automatically changes all chain residues '_chain_index' values.
             affected_chain.index -= 1
@@ -449,16 +450,16 @@
     # Set the structure from a pdb file
     @classmethod
     def from_pdb_file(cls, pdb_filename: str):
         if not os.path.exists(pdb_filename):
             raise SystemExit('File "' + pdb_filename + '" not found')
         # Read the pdb file line by line and set the parsed atoms, residues and chains
         parsed_atoms = []
-        parsed_residues = []
-        parsed_chains = []
+        parsed_residues: List[Residue] = []
+        parsed_chains: List[Chain] = []
         atom_index = -1
         residue_index = -1
         with open(pdb_filename, 'r') as file:
             for line in file:
                 # Parse atoms only
                 start = line[0:6]
                 is_atom = start == 'ATOM  ' or start == 'HETATM'
@@ -505,54 +506,57 @@
                 # Otherwise, include the new chain in the list
                 parsed_chains.append(parsed_chain)
                 parsed_chain.residue_indices.append(residue_index)
         return cls(atoms=parsed_atoms, residues=parsed_residues, chains=parsed_chains)
 
     # Fix atom elements by gueesing them when missing
     # Set all elements with the first letter upper and the second(if any) lower
-    def fix_atom_elements(self):
-        for atom in self.atoms:
-            # Make sure elements have the first letter cap and the second letter not cap
-            if atom.element:
-                atom.element = first_cap_only(atom.element)
-            # If elements are missing then guess them from atom names
-            else:
-                atom.element = guess_name_element(atom.name)
+    # def fix_atom_elements(self):
+    #     for atom in self.atoms:
+    #         # Make sure elements have the first letter cap and the second letter not cap
+    #         if atom.element:
+    #             atom.element = first_cap_only(atom.element)
+    #         # If elements are missing then guess them from atom names
+    #         else:
+    #             atom.element = guess_name_element(atom.name)
 
     # Generate a pdb file with current structure
     def generate_pdb_file(self, pdb_filename: str):
         with open(pdb_filename, "w") as file:
             file.write('REMARK mdtoolbelt generated pdb file\n')
             for a, atom in enumerate(self.atoms):
                 residue = atom.residue
                 index = str((a+1) % 100000).rjust(5)
-                name = ' ' + atom.name.ljust(3) if len(atom.name) < 4 else atom.name
+                name = ' ' + str(atom.name).ljust(3) if len(str(atom.name)) < 4 else atom.name
                 residue_name = residue.name.ljust(4)
                 chain = atom.chain.name.rjust(1)
                 residue_number = str(residue.number).rjust(4)
                 icode = residue.icode.rjust(1)
-                coords = atom.coords
-                x_coord, y_coord, z_coord = ["{:.3f}".format(coord).rjust(8) for coord in coords]
+                coords: Optional[Coords] = atom.coords
+                if not coords:
+                    raise ValueError('Atom ' + str(atom) + ' has no coordinates')
+                else:
+                    x_coord, y_coord, z_coord = ["{:.3f}".format(coord).rjust(8) for coord in coords]
                 occupancy = '1.00'  # Just a placeholder
                 temp_factor = '0.00'  # Just a placeholder
                 element = atom.element
-                atom_line = ('ATOM  ' + index + ' ' + name + ' ' + residue_name + chain + residue_number + icode + '   ' + x_coord + y_coord + z_coord + '  ' + occupancy + '  ' + temp_factor + '           ' + element).ljust(80) + '\n'
+                atom_line = ('ATOM  ' + str(index) + ' ' + str(name) + ' ' + residue_name + chain + residue_number + icode + '   ' + x_coord + y_coord + z_coord + '  ' + occupancy + '  ' + temp_factor + '           ' + element).ljust(80) + '\n'
                 file.write(atom_line)
 
     # Get a chain by its name
-    def get_chain_by_name(self, name: str) -> 'Chain':
+    def get_chain_by_name(self, name: str) -> Optional[Chain]:
         return next((c for c in self.chains if c.name == name), None)
 
     # Get a summary of the structure
     def display_summary(self):
         print('Atoms: ' + str(len(self.atoms)))
         print('Residues: ' + str(len(self.residues)))
         print('Chains: ' + str(len(self.chains)))
         for chain in self.chains:
-            print('Chain ' + chain.name + ' (' + str(len(chain.residue_indices)) + ' residues)')
+            print('Chain ' + str(chain.name) + ' (' + str(len(chain.residue_indices)) + ' residues)')
             print(' -> ' + chain.get_sequence())
 
     # This is an alternative system to find protein chains(anything else is chained as 'X')
     # This system does not depend on VMD
     # It totally overrides previous chains since it is expected to be used only when chains are missing
     def raw_protein_chainer(self):
         current_chain = self.get_next_available_chain_name()
@@ -562,30 +566,32 @@
             if not alpha_carbon:
                 residue.set_chain('X')
                 continue
             # Connected aminoacids have their alpha carbons at a distance of around 3.8 Ångstroms
             residues_are_connected = previous_alpha_carbon and calculate_distance(previous_alpha_carbon, alpha_carbon) < 4
             if not residues_are_connected:
                 current_chain = self.get_next_available_chain_name()
-            residue.set_chain(current_chain)
+            if current_chain:
+                residue.set_chain(current_chain)
             previous_alpha_carbon = alpha_carbon
 
     # Get the next available chain name
     # Find alphabetically the first letter which is not yet used as a chain name
     # If all letters in the alphabet are used already then return None
     def get_next_available_chain_name(self) -> Optional[str]:
         current_chain_names = [chain.name for chain in self.chains]
         return next((name for name in available_caps if name not in current_chain_names), None)
 
 
 # Calculate the distance between two atoms
 def calculate_distance(atom_1: Atom, atom_2: Atom) -> float:
-    squared_distances_sum = 0
-    for i in {'x': 0, 'y': 1, 'z': 2}.values():
-        squared_distances_sum += (atom_1.coords[i] - atom_2.coords[i])**2
+    squared_distances_sum = 0.0
+    if atom_1.coords is not None and atom_2.coords is not None:
+        for i in {'x': 0, 'y': 1, 'z': 2}.values():
+            squared_distances_sum += (atom_1.coords[i] - atom_2.coords[i])**2
     return math.sqrt(squared_distances_sum)
 
 
 # Set all available chains according to pdb standards
 available_caps = ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K',
                   'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
 
@@ -708,16 +714,16 @@
     elif residue_types == "aminoacids":
         target_residues = aminoacids
     elif residue_types == "nucleotides":
         target_residues = nucleotides
     else:
         raise ValueError('Unrecognized residue types ' + str(residue_types))
     # Now find the corresponding letter among the target residues
-    ref = target_residues.get(residue_name, False)
-    return ref if ref else "X"
+    ref = target_residues.get(residue_name, 'X')
+    return ref
 
 
 # Map the structure aminoacids sequences against the standard reference sequences
 # References are uniprot accession ids and they are optional
 # For each reference, align the reference sequence with the topology sequence
 # Chains which do not match any reference sequence will be blasted
 # Note that an internet connection is required both to retireve the uniprot reference sequence and to do the blast
@@ -735,15 +741,15 @@
         if next((letter for letter in sequence if letter != 'X'), None):
             structure_sequence['match'] = {'ref': None, 'map': None, 'score': 0}
             protein_sequences.append(structure_sequence)
     # For each input forced reference, get the reference sequence
     reference_sequences = {}
     if forced_references:
         # Check forced_references is not a string
-        if type(forced_references) == str:
+        if isinstance(forced_references, str):
             raise TypeError('Forced references should be a list and not a string a this point')
         for uniprot_id in forced_references:
             reference = get_uniprot_reference(uniprot_id)
             reference_sequences[reference['uniprot']] = reference['sequence']
             # Save the current whole reference object for later
             references[reference['uniprot']] = reference
 
@@ -790,15 +796,15 @@
     # To get them, we run a blast with each orphan chain sequence
     for structure_sequence in protein_sequences:
         # Skip already references chains
         if structure_sequence['match']['ref']:
             continue
         # Run the blast
         sequence = structure_sequence['sequence']
-        uniprot_id = blast(sequence)
+        uniprot_id = blast(sequence)[0]
         # Build a new reference from the resulting uniprot
         reference = get_uniprot_reference(uniprot_id)
         reference_sequences[reference['uniprot']] = reference['sequence']
         # Save the current whole reference object for later
         references[reference['uniprot']] = reference
         # If we have every protein chain matched with a reference already then we stop here
         if match_sequences():
@@ -806,43 +812,43 @@
     print('The BLAST failed to find a matching reference sequence for at least one protein sequence')
     return None
 
 
 # Try to match all protein sequences with the available reference sequences
 # In case of match, objects in the 'protein_sequences' list are modified by adding the result
 # Finally, return True if all protein sequences were matched with the available reference sequences or False if not
-def match_sequences(protein_sequences: list, reference_sequences: dict) -> bool:
-    # Track each chain-reference alignment match and keep the score of successful alignments
-    # Now for each structure sequence, align all reference sequences and keep the best alignment(if it meets the minimum)
-    for structure_sequence in protein_sequences:
-        for uniprot_id, reference_sequence in reference_sequences.items():
-            # Align the structure sequence with the reference sequence
-            align_results = align(reference_sequence, structure_sequence['sequence'])
-            if not align_results:
-                continue
-            # In case we have a valid alignment, check the alignment score is better than the current reference score(if any)
-            sequence_map, align_score = align_results
-            current_reference = structure_sequence['match']
-            if current_reference['score'] > align_score:
-                continue
-            reference = references[uniprot_id]
-
-            # If the alignment is better then we impose the new reference
-            structure_sequence['match'] = {'ref': reference, 'map': sequence_map, 'score': align_score}
-    # Finally, return True if all protein sequences were matched with the available reference sequences or False if not
-    return all([structure_sequence['match']['ref'] for structure_sequence in protein_sequences])
+# def match_sequences(protein_sequences: list, reference_sequences: dict) -> bool:
+#     # Track each chain-reference alignment match and keep the score of successful alignments
+#     # Now for each structure sequence, align all reference sequences and keep the best alignment(if it meets the minimum)
+#     for structure_sequence in protein_sequences:
+#         for uniprot_id, reference_sequence in reference_sequences.items():
+#             # Align the structure sequence with the reference sequence
+#             align_results = align(reference_sequence, structure_sequence['sequence'])
+#             if not align_results:
+#                 continue
+#             # In case we have a valid alignment, check the alignment score is better than the current reference score(if any)
+#             sequence_map, align_score = align_results
+#             current_reference = structure_sequence['match']
+#             if current_reference['score'] > align_score:
+#                 continue
+#             reference = references[uniprot_id]  # type: ignore
+
+#             # If the alignment is better then we impose the new reference
+#             structure_sequence['match'] = {'ref': reference, 'map': sequence_map, 'score': align_score}
+#     # Finally, return True if all protein sequences were matched with the available reference sequences or False if not
+#     return all([structure_sequence['match']['ref'] for structure_sequence in protein_sequences])
 
 
 # Reformat mapping data to the topology system(introduced later)
 def format_topology_data(structure: 'Structure', mapping_data: list) -> dict:
     # Get the count of residues from the structure
     residues_count = len(structure.residues)
     # Now format data
     reference_ids = []
-    residue_reference_indices = [None] * residues_count
+    residue_reference_indices: List = [None] * residues_count
     residue_reference_numbers = [None] * residues_count
     for data in mapping_data:
         match = data['match']
         # Get the reference index
         # Note that several matches may belong to the same reference and thus have the same index
         reference = match['ref']
         uniprot_id = reference['uniprot']
@@ -854,31 +860,32 @@
             if residue_number is None:
                 continue
             residue_index = residue_indices[r]
             residue_reference_indices[residue_index] = reference_index
             residue_reference_numbers[residue_index] = residue_number
     # If there are not references at the end then set all fields as None, in order to save space
     if len(reference_ids) == 0:
-        reference_ids = None
-        residue_reference_indices = None
-        residue_reference_numbers = None
+        reference_ids = []
+        residue_reference_indices = []
+        residue_reference_numbers = []
     # Return the 3 topology fields as they are in the database
     residues_map = {'references': reference_ids, 'residue_reference_indices': residue_reference_indices, 'residue_reference_numbers': residue_reference_numbers}
     return residues_map
 
 
 # Align a reference aminoacid sequence with each chain sequence in a topology
 # NEVER FORGET: This system relies on the fact that topology chains are not repeated
 def map_sequence(ref_sequence: str, structure: 'Structure') -> list:
     sequences = get_chain_sequences(structure)
-    mapping = []
+    mapping: List = []
     for s in sequences:
         sequence = sequences[s]
         sequence_map = align(ref_sequence, sequence)
-        mapping += sequence_map
+        if sequence_map:
+            mapping += sequence_map
     return mapping
 
 
 # Get each chain name and aminoacids sequence in a topology
 # Output format example: [{'sequence': 'VNLTT', 'indices': [1, 2, 3, 4, 5]}, ...]
 def get_chain_sequences(structure: 'Structure') -> list:
     sequences = []
@@ -908,15 +915,15 @@
 
     # If the new sequence is all 'X' stop here, since this would make the alignment infinite
     # Then an array filled with None is returned
     if all([letter == 'X' for letter in new_sequence]):
         return None
 
     # Return the new sequence as best aligned as possible with the reference sequence
-    alignments = pairwise2.align.localds(ref_sequence, new_sequence, blosum62, -10, -0.5)
+    alignments = pairwise2.align.localds(ref_sequence, new_sequence, blosum62, -10, -0.5)  # type: ignore
     # DANI: Habría que hacerlo de esta otra forma según el deprecation warning (arriba hay más código)
     # DANI: El problema es que el output lo tiene todo menos la sequencia en formato alienada
     # DANI: i.e. formato '----VNLTT', que es justo el que necesito
     # alignments = aligner.align(ref_sequence, new_sequence)
 
     # In case there are no alignments it means the current chain has nothing to do with this reference
     # Then an array filled with None is returned
@@ -939,15 +946,15 @@
     # Non maching sequence may return a 0.1-0.3 normalized score
     # Matching sequence may return >4 normalized score
     if normalized_score < 1:
         print('Not valid alignment')
         return None
 
     # Match each residue
-    aligned_mapping = []
+    aligned_mapping: List = []
     aligned_index = 0
     for l_index, letter in enumerate(aligned_sequence):
         # Guions are skipped
         if letter == '-':
             continue
         # Get the current residue of the new sequence
         equivalent_letter = new_sequence[aligned_index]
@@ -989,13 +996,13 @@
 def get_uniprot_reference(uniprot_accession: str) -> dict:
     # Request Uniprot
     request_url = 'https://www.ebi.ac.uk/proteins/api/proteins/' + uniprot_accession
     try:
         with urllib.request.urlopen(request_url) as response:
             parsed_response = json.loads(response.read().decode("utf-8"))
     # If the accession is not found in UniProt then the id is not valid
-    except urllib.error.HTTPError as error:
+    except urllib.error.HTTPError as error:  # type: ignore
         if error.code == 400:
             raise ValueError('Something went wrong with the Uniprot request: ' + request_url)
     # Get the aminoacids sequence
     sequence = parsed_response['sequence']['sequence']
     return {'uniprot': uniprot_accession, 'sequence': sequence}
```

### Comparing `biobb_model-4.1.0/biobb_model/model/fix_side_chain.py` & `biobb_model-4.2.0/biobb_model/model/fix_side_chain.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 
 """Module containing the FixSideChain class and the command line interface."""
 import argparse
+from typing import Dict, Optional
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
 from biobb_model.model.common import modeller_installed
 
 
@@ -39,15 +40,15 @@
             * name: In house
             * license: Apache-2.0
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
     """
 
-    def __init__(self, input_pdb_path: str, output_pdb_path: str, properties: dict = None, **kwargs) -> None:
+    def __init__(self, input_pdb_path: str, output_pdb_path: str, properties: Optional[Dict] = None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
@@ -94,22 +95,22 @@
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
         # Remove temporal files
-        self.tmp_files.extend([self.stage_io_dict.get("unique_dir")])
+        self.tmp_files.extend([self.stage_io_dict.get("unique_dir", "")])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
         return self.return_code
 
 
-def fix_side_chain(input_pdb_path: str, output_pdb_path: str, properties: dict = None, **kwargs) -> int:
+def fix_side_chain(input_pdb_path: str, output_pdb_path: str, properties: Optional[Dict] = None, **kwargs) -> int:
     """Create :class:`FixSideChain <model.fix_side_chain.FixSideChain>` class and
     execute the :meth:`launch() <model.fix_side_chain.FixSideChain.launch>` method."""
     return FixSideChain(input_pdb_path=input_pdb_path,
                         output_pdb_path=output_pdb_path,
                         properties=properties, **kwargs).launch()
```

### Comparing `biobb_model-4.1.0/biobb_model/model/fix_ssbonds.py` & `biobb_model-4.2.0/biobb_model/model/fix_ssbonds.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 #!/usr/bin/env python3
 
 """Module containing the FixSSBonds class and the command line interface."""
 import argparse
+from typing import Dict, Optional
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
 
 
 class FixSSBonds(BiobbObject):
     """
     | biobb_model FixSSBonds
     | Fix SS bonds from residues.
+    | Fix the SS bonds in a PDB structure.
 
     Args:
         input_pdb_path (str): Input PDB file path. File type: input. `Sample file <https://github.com/bioexcel/biobb_model/raw/master/biobb_model/test/data/model/1aki.pdb>`_. Accepted formats: pdb (edam:format_1476).
         output_pdb_path (str): Output PDB file path. File type: output. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_model/master/biobb_model/test/reference/model/output_ssbonds.pdb>`_. Accepted formats: pdb (edam:format_1476).
         properties (dict - Python dictionary object containing the tool parameters, not input/output files):
             * **modeller_key** (*str*) - (None) Modeller license key.
             * **binary_path** (*str*) - ("check_structure") Path to the check_structure executable binary.
@@ -35,15 +37,15 @@
             * name: In house
             * license: Apache-2.0
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
     """
 
-    def __init__(self, input_pdb_path: str, output_pdb_path: str, properties: dict = None, **kwargs) -> None:
+    def __init__(self, input_pdb_path: str, output_pdb_path: str, properties: Optional[Dict] = None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
@@ -83,22 +85,22 @@
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
         # Remove temporal files
-        self.tmp_files.extend([self.stage_io_dict.get("unique_dir")])
+        self.tmp_files.extend([self.stage_io_dict.get("unique_dir", "")])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
         return self.return_code
 
 
-def fix_ssbonds(input_pdb_path: str, output_pdb_path: str, properties: dict = None, **kwargs) -> int:
+def fix_ssbonds(input_pdb_path: str, output_pdb_path: str, properties: Optional[Dict] = None, **kwargs) -> int:
     """Create :class:`FixSSBonds <model.fix_ssbonds.FixSSBonds>` class and
     execute the :meth:`launch() <model.fix_ssbonds.FixSSBonds.launch>` method."""
     return FixSSBonds(input_pdb_path=input_pdb_path,
                       output_pdb_path=output_pdb_path,
                       properties=properties, **kwargs).launch()
```

### Comparing `biobb_model-4.1.0/biobb_model/model/mutate.py` & `biobb_model-4.2.0/biobb_model/model/mutate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 
 """Module containing the Mutate class and the command line interface."""
 import argparse
+from typing import Dict, Optional
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
 from biobb_model.model.common import modeller_installed
 
 
@@ -41,15 +42,15 @@
             * name: In house
             * license: Apache-2.0
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
     """
 
-    def __init__(self, input_pdb_path: str, output_pdb_path: str, properties: dict = None, **kwargs) -> None:
+    def __init__(self, input_pdb_path: str, output_pdb_path: str, properties: Optional[Dict] = None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
@@ -103,23 +104,23 @@
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
         # Remove temporal files
-        self.tmp_files.append(self.stage_io_dict.get("unique_dir"))
-        self.tmp_files.extend([self.stage_io_dict.get("unique_dir")])
+        self.tmp_files.append(self.stage_io_dict.get("unique_dir", ""))
+        self.tmp_files.extend([self.stage_io_dict.get("unique_dir", "")])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
         return self.return_code
 
 
-def mutate(input_pdb_path: str, output_pdb_path: str, properties: dict = None, **kwargs) -> int:
+def mutate(input_pdb_path: str, output_pdb_path: str, properties: Optional[Dict] = None, **kwargs) -> int:
     """Create :class:`Mutate <model.mutate.Mutate>` class and
     execute the :meth:`launch() <model.mutate.Mutate.launch>` method."""
     return Mutate(input_pdb_path=input_pdb_path,
                   output_pdb_path=output_pdb_path,
                   properties=properties, **kwargs).launch()
```

### Comparing `biobb_model-4.1.0/biobb_model.egg-info/PKG-INFO` & `biobb_model-4.2.0/biobb_model.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: biobb-model
-Version: 4.1.0
+Version: 4.2.0
 Summary: Biobb_model is the Biobb module collection to check and model 3d structures, create mutations or reconstruct missing atoms.
 Home-page: https://github.com/bioexcel/biobb_model
 Author: Biobb developers
 Author-email: pau.andrio@bsc.es
-Project-URL: Documentation, http://biobb_model.readthedocs.io/en/latest/
+Project-URL: Documentation, http://biobb-model.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,15 +21,15 @@
 License-File: LICENSE
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_model?label=Version)](https://GitHub.com/bioexcel/biobb_model/tags/)
 [![](https://img.shields.io/pypi/v/biobb-model.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-model/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_model?label=Conda)](https://anaconda.org/bioconda/biobb_model)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_model?label=Conda%20downloads)](https://anaconda.org/bioconda/biobb_model)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_model?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_model:4.1.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_model:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_model)
 [![](https://img.shields.io/pypi/pyversions/biobb-model.svg?label=Python%20Versions)](https://pypi.org/project/biobb-model/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_model)
 
 [![](https://readthedocs.org/projects/biobb-model/badge/?version=latest&label=Docs)](https://biobb-model.readthedocs.io/en/latest/?badge=latest)
@@ -40,63 +40,70 @@
 
 [![](https://docs.bioexcel.eu/biobb_model/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_model/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_model/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_model/coverage/)
 [![](https://docs.bioexcel.eu/biobb_model/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_model/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_model?label=Last%20Commit)](https://github.com/bioexcel/biobb_model/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_model.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_model/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 # biobb_model
 
 ### Introduction
 Biobb_model is the Biobb module collection to check and model 3d structures,
 create mutations or reconstruct missing atoms.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
-[latest API documentation](http://biobb_model.readthedocs.io/en/latest/).
+[latest API documentation](http://biobb-model.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2023.4
+v4.2.0 2024.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_model>=4.1.0"
+        pip install "biobb_model>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-model.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_model>=4.1.0"
+        conda install -c bioconda "biobb_model>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-model.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-model.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_model:4.1.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_model:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_model:4.1.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_model:4.2.0--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
@@ -113,14 +120,14 @@
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-model.readthedocs.io/en/latest/command_line.html).
 
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2024 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2024 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
```

### Comparing `biobb_model-4.1.0/biobb_model.egg-info/SOURCES.txt` & `biobb_model-4.2.0/biobb_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_model-4.1.0/setup.py` & `biobb_model-4.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_model",
-    version="4.1.0",
+    version="4.2.0",
     author="Biobb developers",
     author_email="pau.andrio@bsc.es",
     description="Biobb_model is the Biobb module collection to check and model 3d structures, create mutations or reconstruct missing atoms.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_model",
     project_urls={
-        "Documentation": "http://biobb_model.readthedocs.io/en/latest/",
+        "Documentation": "http://biobb-model.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['docs', 'test']),
     install_requires=[
-        'biobb_common==4.1.0',
+        'biobb_common==4.2.0',
         'biobb_structure_checking>=3.13.4',
         'xmltodict'
     ],
     python_requires='>=3.8',
     entry_points={
         "console_scripts": [
             "checking_log = biobb_model.model.checking_log:main",
```

