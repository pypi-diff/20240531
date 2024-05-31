# Comparing `tmp/nanomotif-0.4.5.tar.gz` & `tmp/nanomotif-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanomotif-0.4.5.tar", last modified: Wed May 29 08:37:28 2024, max compression
+gzip compressed data, was "nanomotif-0.4.6.tar", last modified: Fri May 31 08:48:35 2024, max compression
```

## Comparing `nanomotif-0.4.5.tar` & `nanomotif-0.4.6.tar`

### file list

```diff
@@ -1,70 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:37:28.235812 nanomotif-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-29 08:37:23.000000 nanomotif-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7777 2024-05-29 08:37:28.235812 nanomotif-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-05-29 08:37:23.000000 nanomotif-0.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:37:28.191812 nanomotif-0.4.5/nanomotif/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11200 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/argparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/bin_consensus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:37:28.195812 nanomotif-0.4.5/nanomotif/binnary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/binnary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13167 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/binnary/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    15629 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/binnary/data_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/binnary/detect_contamination.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/binnary/include_contigs.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/binnary/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/binnary/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/binnary/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14370 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/candidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/dataload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:37:28.195812 nanomotif-0.4.5/nanomotif/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/datasets/geobacillus-contig-bin.tsv
--rw-r--r--   0 runner    (1001) docker     (127)   176247 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/datasets/geobacillus-plasmids.assembly.fasta
--rw-r--r--   0 runner    (1001) docker     (127) 26479844 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/datasets/geobacillus-plasmids.pileup.bed
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    28633 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    20007 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:37:28.231812 nanomotif-0.4.5/nanomotif/mtase_linker/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/mtase_linker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/mtase_linker/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/mtase_linker/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/old_search_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/scoremotifs.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/seed.py
--rw-r--r--   0 runner    (1001) docker     (127)    20090 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/seq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-29 08:37:23.000000 nanomotif-0.4.5/nanomotif/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:37:28.235812 nanomotif-0.4.5/nanomotif.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7777 2024-05-29 08:37:28.000000 nanomotif-0.4.5/nanomotif.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-29 08:37:28.000000 nanomotif-0.4.5/nanomotif.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 08:37:28.000000 nanomotif-0.4.5/nanomotif.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-29 08:37:28.000000 nanomotif-0.4.5/nanomotif.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 08:37:28.000000 nanomotif-0.4.5/nanomotif.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-29 08:37:28.000000 nanomotif-0.4.5/nanomotif.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 08:37:28.000000 nanomotif-0.4.5/nanomotif.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 08:37:28.235812 nanomotif-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-29 08:37:23.000000 nanomotif-0.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:37:28.231812 nanomotif-0.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:37:28.235812 nanomotif-0.4.5/tests/binnary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/binnary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/binnary/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/binnary/test_arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    11132 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/binnary/test_cli_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/binnary/test_data_processing_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/binnary/test_detect_contamination.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/binnary/test_generate_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/binnary/test_include_contigs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/binnary/test_scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/binnary/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/binnary/test_write_bins.py
--rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/test_candidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/test_dataload.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/test_motif_find.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:37:23.000000 nanomotif-0.4.5/tests/test_motif_score.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:48:35.994937 nanomotif-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-31 08:48:31.000000 nanomotif-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7777 2024-05-31 08:48:35.994937 nanomotif-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-05-31 08:48:31.000000 nanomotif-0.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:48:35.954937 nanomotif-0.4.6/nanomotif/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11711 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/argparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/bin_consensus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:48:35.954937 nanomotif-0.4.6/nanomotif/binnary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/binnary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13167 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/binnary/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15629 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/binnary/data_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/binnary/detect_contamination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/binnary/include_contigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/binnary/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/binnary/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/binnary/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14376 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/dataload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:48:35.958937 nanomotif-0.4.6/nanomotif/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/datasets/geobacillus-contig-bin.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)   176247 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/datasets/geobacillus-plasmids.assembly.fasta
+-rw-r--r--   0 runner    (1001) docker     (127) 26479844 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/datasets/geobacillus-plasmids.pileup.bed
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28633 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20408 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:48:35.990937 nanomotif-0.4.6/nanomotif/mtase_linker/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/mtase_linker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/mtase_linker/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/mtase_linker/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:48:35.990937 nanomotif-0.4.6/nanomotif/mtase_linker/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/mtase_linker/envs/blast-2.14.1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/mtase_linker/envs/defensefinder-1.2.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/mtase_linker/envs/prodigal-2.6.3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/mtase_linker/envs/python_env-3.12.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:48:35.990937 nanomotif-0.4.6/nanomotif/mtase_linker/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/mtase_linker/src/blastp_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/mtase_linker/src/extract_MTase_genes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/mtase_linker/src/mod_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/mtase_linker/src/motif_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/mtase_linker/src/utillities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/old_search_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/scoremotifs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20090 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/seq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-31 08:48:31.000000 nanomotif-0.4.6/nanomotif/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:48:35.994937 nanomotif-0.4.6/nanomotif.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7777 2024-05-31 08:48:35.000000 nanomotif-0.4.6/nanomotif.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-31 08:48:35.000000 nanomotif-0.4.6/nanomotif.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 08:48:35.000000 nanomotif-0.4.6/nanomotif.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-31 08:48:35.000000 nanomotif-0.4.6/nanomotif.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 08:48:35.000000 nanomotif-0.4.6/nanomotif.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-31 08:48:35.000000 nanomotif-0.4.6/nanomotif.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-31 08:48:35.000000 nanomotif-0.4.6/nanomotif.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 08:48:35.994937 nanomotif-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-31 08:48:31.000000 nanomotif-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:48:35.990937 nanomotif-0.4.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 08:48:31.000000 nanomotif-0.4.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:48:35.994937 nanomotif-0.4.6/tests/binnary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 08:48:31.000000 nanomotif-0.4.6/tests/binnary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-31 08:48:31.000000 nanomotif-0.4.6/tests/binnary/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-31 08:48:31.000000 nanomotif-0.4.6/tests/binnary/test_arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11132 2024-05-31 08:48:31.000000 nanomotif-0.4.6/tests/binnary/test_cli_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-05-31 08:48:31.000000 nanomotif-0.4.6/tests/binnary/test_data_processing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-31 08:48:31.000000 nanomotif-0.4.6/tests/binnary/test_detect_contamination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-31 08:48:31.000000 nanomotif-0.4.6/tests/binnary/test_generate_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-31 08:48:31.000000 nanomotif-0.4.6/tests/binnary/test_include_contigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-31 08:48:31.000000 nanomotif-0.4.6/tests/binnary/test_scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-31 08:48:31.000000 nanomotif-0.4.6/tests/binnary/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-31 08:48:31.000000 nanomotif-0.4.6/tests/binnary/test_write_bins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-05-31 08:48:31.000000 nanomotif-0.4.6/tests/test_candidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-31 08:48:31.000000 nanomotif-0.4.6/tests/test_dataload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-31 08:48:31.000000 nanomotif-0.4.6/tests/test_motif_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 08:48:31.000000 nanomotif-0.4.6/tests/test_motif_score.py
```

### Comparing `nanomotif-0.4.5/LICENSE` & `nanomotif-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/PKG-INFO` & `nanomotif-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanomotif
-Version: 0.4.5
+Version: 0.4.6
 Summary: Identifying methlyation motifs in nanopore data
 Author: AAU_DarkScience
 Author-email: shei@bio.aau.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wheel
```

### Comparing `nanomotif-0.4.5/README.md` & `nanomotif-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/nanomotif/argparser.py` & `nanomotif-0.4.6/nanomotif/argparser.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     ###########################################################################
     # Find Motifs
     parser_shared_find_motifs = argparse.ArgumentParser(add_help=False)
     parser_shared_find_motifs.add_argument("--search_frame_size", type=int, default=40, help="length of the sequnces sampled around confident methylatyion sites. Default: %(default)s")
     parser_shared_find_motifs.add_argument("--threshold_methylation_confident", type=float, default=0.80, help="minimum fraction of reads that must be methylated at a position for the position to be considered confiently methylated. These position are used to search for candidate motifs. Default: %(default)s")
     parser_shared_find_motifs.add_argument("--threshold_valid_coverage", type=int, default=5, help="minimum valid base coverage for a position to be considered. Default: %(default)s")
     parser_shared_find_motifs.add_argument("--minimum_kl_divergence", type=float, default=0.05, help="minimum KL-divergence for a position to considered for expansion in  motif search. Higher value means less exhaustive, but faster search. Default: %(default)s")
+    parser_shared_find_motifs.add_argument("--min_motifs_contig", type=int, default=20, help="minimum number of times a motif has to have been oberserved in a contig. Default: %(default)s")
     parser_find_motifs = subparsers.add_parser(
         'find_motifs', 
         parents=[parser_positional, parser_optional, parser_shared_find_motifs], 
         help="Finds motifs directly on contig level in provided assembly"
     )
 
     ###########################################################################
@@ -43,27 +44,28 @@
         help="Find motifs indirectly in contigs by scoring with motifs found in other contigs"
     )
     parser_score_motifs.add_argument("motifs", type=str, help="path to the motifs file.")
     
     ###########################################################################
     # Bin consensus
     parser_shared_bin_consensus = argparse.ArgumentParser(add_help=False, conflict_handler="resolve")
-    parser_shared_bin_consensus.add_argument("bins", type=str, help="tsv file specifying which bin contigs belong.")
+    parser_shared_bin_consensus.add_argument("--min_motifs_bin", type=int, default=50, help="minimum number of times a motif has to have been oberserved in a bin. Default: %(default)s")
     parser_bin_consensus = subparsers.add_parser(
         'bin_consensus', 
         parents=[parser_positional, parser_optional, parser_shared_bin_consensus],
         help="Indentifies highly methylated motifs in bins"
     )
     parser_bin_consensus.add_argument("motifs", type=str, help="path to the motifs file.")
+    parser_bin_consensus.add_argument("bins", type=str, help="tsv file specifying which bin contigs belong.")
     parser_bin_consensus.add_argument("motifs_scored", metavar="motifs-scored", type=str, help="path to the motif-scored file.")
 
     ###########################################################################
     # Complete workflow
     parser_complete_workflow = subparsers.add_parser('motif_discovery', help='Runs find_motifs, score_motifs and bin_consensus', parents=[parser_positional, parser_optional, parser_shared_find_motifs, parser_shared_bin_consensus], conflict_handler="resolve")
-
+    parser_complete_workflow.add_argument("bins", type=str, help="tsv file specifying which bin contigs belong.")
 
     ###########################################################################
     # Bin contamination and inclusion
     parser_binnary_shared = argparse.ArgumentParser(description="Contamination DNA Methylation Pattern", add_help=False)
     """Function to add common arguments to a subparser."""
     parser_binnary_shared.add_argument(
         "--motifs_scored", type=str, help="Path to motifs-scored.tsv from nanomotif", required=True
@@ -187,12 +189,12 @@
     )
     parser_mtase_linker_install.add_argument("-d", "--dependency_dir", type=str, default=os.getcwd(), help="Path to installation location of dependencies. A folder named ML_dependencies will be generated. Default is cwd.")
     
 
 
     ###########################################################################
     # Check installation
-    parser_check_installation = subparsers.add_parser('check_installation', parents=[parser_optional, parser_shared_find_motifs], add_help=False, help="Performs small test run to verify that the installation is correct.")
+    parser_check_installation = subparsers.add_parser('check_installation', parents=[parser_optional, parser_shared_find_motifs, parser_shared_bin_consensus], add_help=False, help="Performs small test run to verify that the installation is correct.")
     
     
     return parser
```

### Comparing `nanomotif-0.4.5/nanomotif/bin_consensus.py` & `nanomotif-0.4.6/nanomotif/bin_consensus.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/nanomotif/binnary/analysis.py` & `nanomotif-0.4.6/nanomotif/binnary/analysis.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/nanomotif/binnary/data_processing.py` & `nanomotif-0.4.6/nanomotif/binnary/data_processing.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/nanomotif/binnary/detect_contamination.py` & `nanomotif-0.4.6/nanomotif/binnary/detect_contamination.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/nanomotif/binnary/include_contigs.py` & `nanomotif-0.4.6/nanomotif/binnary/include_contigs.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/nanomotif/binnary/logging.py` & `nanomotif-0.4.6/nanomotif/binnary/logging.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/nanomotif/binnary/scoring.py` & `nanomotif-0.4.6/nanomotif/binnary/scoring.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/nanomotif/binnary/utils.py` & `nanomotif-0.4.6/nanomotif/binnary/utils.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/nanomotif/candidate.py` & `nanomotif-0.4.6/nanomotif/candidate.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         return str_equal and pos_equal
     def sub_motif_of(self, other_motif):
         """
         Check if a motif is in another motif.
         """
         assert isinstance(other_motif, Motif)
         # Strip for redundant posititons (flanking .)
-        if self.identical(other_motif):
+        if self.string == other_motif.string:
             return False
         self_stripped = self.new_stripped_motif()
         other_stripped = other_motif.new_stripped_motif()
 
         if self_stripped.length() < other_stripped.length():
             return False
```

### Comparing `nanomotif-0.4.5/nanomotif/constants.py` & `nanomotif-0.4.6/nanomotif/constants.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/nanomotif/dataload.py` & `nanomotif-0.4.6/nanomotif/dataload.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/nanomotif/datasets/geobacillus-plasmids.assembly.fasta` & `nanomotif-0.4.6/nanomotif/datasets/geobacillus-plasmids.assembly.fasta`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/nanomotif/datasets/geobacillus-plasmids.pileup.bed` & `nanomotif-0.4.6/nanomotif/datasets/geobacillus-plasmids.pileup.bed`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/nanomotif/datasets.py` & `nanomotif-0.4.6/nanomotif/datasets.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/nanomotif/evaluate.py` & `nanomotif-0.4.6/nanomotif/evaluate.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/nanomotif/feature.py` & `nanomotif-0.4.6/nanomotif/feature.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/nanomotif/main.py` & `nanomotif-0.4.6/nanomotif/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,20 @@
                 "contig", "motif", "mod_position", "mod_type", "n_mod", "n_nomod", "motif_type",
                 "motif_complement", "mod_position_complement", "n_mod_complement", "n_nomod_complement"
             ])
         except:
             df_out = df_out.select([
                 "contig", "motif", "mod_position", "mod_type", "n_mod", "n_nomod", "motif_type",
             ])
+        # Subtract prior alpha and beta from n_mod and n_nomod
+        if "model" in df.columns:
+            df_out = df_out.with_columns([
+                pl.col("n_mod") - nm.model.DEFAULT_PRIOR_BETA,
+                pl.col("n_nomod") - nm.model.DEFAULT_PRIOR_ALPHA
+            ])
         return df_out
     def save_motif_df(df, name):
         df = format_motif_df(df)
         df = df.sort(["contig", "mod_type", "motif"])
         df.write_csv(args.out + "/" + name + ".tsv", separator="\t")
     os.makedirs(args.out + "/precleanup-motifs/", exist_ok=True)
     save_motif_df(motifs, "precleanup-motifs/motifs-raw")
@@ -168,15 +174,15 @@
     if len(motifs) == 0:
         log.info("No motifs found")
         return
     motifs_file_name = motifs_file_name +   "-complement"
     save_motif_df(motifs, motifs_file_name)
 
     log.info(" - Removing motifs observed less than min count")
-    motifs = motifs.filter(pl.col("n_mod") + pl.col("n_nomod") > 1)
+    motifs = motifs.filter((pl.col("n_mod") + pl.col("n_nomod")) > args.min_motifs_contig)
     if len(motifs) == 0:
         log.info("No motifs found")
         return
     motifs_file_name = motifs_file_name +   "-mincount"
     save_motif_df(motifs, motifs_file_name)
 
 
@@ -278,14 +284,16 @@
 
     output = output.rename({"bin":"contig", "n_mod_bin":"n_mod", "n_nomod_bin":"n_nomod"})
 
     output = nm.postprocess.join_motif_complements(output)
 
     output = output.rename({"contig":"bin", "n_mod":"n_mod_bin", "n_nomod":"n_nomod_bin"})
     output = output.sort(["bin", "mod_type", "motif"])
+
+    output = output.filter(pl.col("n_mod_bin") + pl.col("n_nomod_bin") > args.min_motifs_bin)
     output.write_csv(args.out + "/bin-motifs.tsv", separator="\t")
 
 def motif_discovery(args):
     # Check if output directory exists
     log.info("Loading required files")
     pileup = nm.load_pileup(args.pileup, threads = args.threads, min_fraction = args.threshold_methylation_general)
     assembly = nm.load_assembly(args.assembly)
```

### Comparing `nanomotif-0.4.5/nanomotif/model.py` & `nanomotif-0.4.6/nanomotif/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """
 Models
 """
 import numpy as np
 from scipy.stats import beta
 
+DEFAULT_PRIOR_BETA = 1
+DEFAULT_PRIOR_ALPHA = 0
+
 class BetaBernoulliModel():
-    def __init__(self, alpha = 0, beta = 1):
+    def __init__(self, alpha = DEFAULT_PRIOR_ALPHA, beta = DEFAULT_PRIOR_BETA):
         self.alpha = alpha
         self.beta = beta
         self._alpha = alpha
         self._beta = beta
 
     def update(self, n_positives, n_negatives):
         self._alpha += n_positives
```

### Comparing `nanomotif-0.4.5/nanomotif/mtase_linker/command.py` & `nanomotif-0.4.6/nanomotif/mtase_linker/command.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/nanomotif/mtase_linker/dependencies.py` & `nanomotif-0.4.6/nanomotif/mtase_linker/dependencies.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/nanomotif/old_search_method.py` & `nanomotif-0.4.6/nanomotif/old_search_method.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/nanomotif/parallel.py` & `nanomotif-0.4.6/nanomotif/parallel.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/nanomotif/postprocess.py` & `nanomotif-0.4.6/nanomotif/postprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     motif_df_clean = []
     for contig, df in motif_df.groupby("contig"):
         motif_strings = df.get_column("motif").to_list()
         positions = df.get_column("mod_position").to_list()
         motifs = [nm.candidate.Motif(motif_string, pos) for motif_string, pos in zip(motif_strings, positions)]
         clean_motifs = []
         for motif in motifs:
-            if not motif.have_isolated_bases():
+            if not motif.have_isolated_bases(isolation_size = 3):
                 clean_motifs.append(motif)
         df_clean = df.filter(col("motif").is_in(clean_motifs))
         motif_df_clean.append(df_clean)
     motif_df_clean = pl.concat(motif_df_clean)
     return motif_df_clean
 
 def remove_child_motifs(motifs):
```

### Comparing `nanomotif-0.4.5/nanomotif/scoremotifs.py` & `nanomotif-0.4.6/nanomotif/scoremotifs.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/nanomotif/seq.py` & `nanomotif-0.4.6/nanomotif/seq.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/nanomotif/utils.py` & `nanomotif-0.4.6/nanomotif/utils.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/nanomotif.egg-info/PKG-INFO` & `nanomotif-0.4.6/nanomotif.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanomotif
-Version: 0.4.5
+Version: 0.4.6
 Summary: Identifying methlyation motifs in nanopore data
 Author: AAU_DarkScience
 Author-email: shei@bio.aau.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wheel
```

### Comparing `nanomotif-0.4.5/nanomotif.egg-info/SOURCES.txt` & `nanomotif-0.4.6/nanomotif.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -38,14 +38,23 @@
 nanomotif/binnary/utils.py
 nanomotif/datasets/geobacillus-contig-bin.tsv
 nanomotif/datasets/geobacillus-plasmids.assembly.fasta
 nanomotif/datasets/geobacillus-plasmids.pileup.bed
 nanomotif/mtase_linker/__init__.py
 nanomotif/mtase_linker/command.py
 nanomotif/mtase_linker/dependencies.py
+nanomotif/mtase_linker/envs/blast-2.14.1.yaml
+nanomotif/mtase_linker/envs/defensefinder-1.2.0.yaml
+nanomotif/mtase_linker/envs/prodigal-2.6.3.yaml
+nanomotif/mtase_linker/envs/python_env-3.12.0.yaml
+nanomotif/mtase_linker/src/blastp_processing.py
+nanomotif/mtase_linker/src/extract_MTase_genes.py
+nanomotif/mtase_linker/src/mod_typing.py
+nanomotif/mtase_linker/src/motif_assignment.py
+nanomotif/mtase_linker/src/utillities.py
 tests/__init__.py
 tests/test_candidate.py
 tests/test_dataload.py
 tests/test_motif_find.py
 tests/test_motif_score.py
 tests/binnary/__init__.py
 tests/binnary/conftest.py
```

### Comparing `nanomotif-0.4.5/setup.py` & `nanomotif-0.4.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,21 @@
     author='AAU_DarkScience',
     author_email='shei@bio.aau.com',
     license='MIT',
     packages=find_packages(),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     include_package_data=True,
-    package_data={'nanomotif': ['datasets/*'], '':['*.smk'], '':['*.yaml']},
+    package_data={'nanomotif': [
+        'datasets/*',
+        '*.smk',
+        '*.yaml',
+        "mtase_linker/envs/*",
+        "mtase_linker/src/*"
+    ]},
     zip_safe=False,
     install_requires=[
         "wheel",
         "requests",
         "numpy>=1.24.4",
         "pandas>=2.0.2",
         "polars>=0.19",
```

### Comparing `nanomotif-0.4.5/tests/binnary/conftest.py` & `nanomotif-0.4.6/tests/binnary/conftest.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/tests/binnary/test_arg_parser.py` & `nanomotif-0.4.6/tests/binnary/test_arg_parser.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/tests/binnary/test_cli_commands.py` & `nanomotif-0.4.6/tests/binnary/test_cli_commands.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/tests/binnary/test_data_processing_functions.py` & `nanomotif-0.4.6/tests/binnary/test_data_processing_functions.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/tests/binnary/test_detect_contamination.py` & `nanomotif-0.4.6/tests/binnary/test_detect_contamination.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/tests/binnary/test_generate_output.py` & `nanomotif-0.4.6/tests/binnary/test_generate_output.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/tests/binnary/test_include_contigs.py` & `nanomotif-0.4.6/tests/binnary/test_include_contigs.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/tests/binnary/test_scoring.py` & `nanomotif-0.4.6/tests/binnary/test_scoring.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/tests/binnary/test_utils.py` & `nanomotif-0.4.6/tests/binnary/test_utils.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/tests/binnary/test_write_bins.py` & `nanomotif-0.4.6/tests/binnary/test_write_bins.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/tests/test_candidate.py` & `nanomotif-0.4.6/tests/test_candidate.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/tests/test_dataload.py` & `nanomotif-0.4.6/tests/test_dataload.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.4.5/tests/test_motif_find.py` & `nanomotif-0.4.6/tests/test_motif_find.py`

 * *Files identical despite different names*

