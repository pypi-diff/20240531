# Comparing `tmp/meditability-0.2.3.tar.gz` & `tmp/meditability-0.2.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meditability-0.2.3.tar", last modified: Thu May 30 23:41:45 2024, max compression
+gzip compressed data, was "meditability-0.2.3a0.tar", last modified: Tue May 21 19:38:21 2024, max compression
```

## Comparing `meditability-0.2.3.tar` & `meditability-0.2.3a0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-30 23:41:45.680060 meditability-0.2.3/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32337 2024-01-30 21:30:29.000000 meditability-0.2.3/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      275 2024-05-30 23:41:45.680060 meditability-0.2.3/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3621 2024-02-16 18:08:11.000000 meditability-0.2.3/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-30 23:41:45.684059 meditability-0.2.3/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1092 2024-05-30 23:41:00.000000 meditability-0.2.3/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-30 23:41:45.668059 meditability-0.2.3/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-30 23:41:45.672059 meditability-0.2.3/src/meditability.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      275 2024-05-30 23:41:45.000000 meditability-0.2.3/src/meditability.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2300 2024-05-30 23:41:45.000000 meditability-0.2.3/src/meditability.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-30 23:41:45.000000 meditability-0.2.3/src/meditability.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       66 2024-05-30 23:41:45.000000 meditability-0.2.3/src/meditability.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      166 2024-05-30 23:41:45.000000 meditability-0.2.3/src/meditability.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-05-30 23:41:45.000000 meditability-0.2.3/src/meditability.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-30 23:41:45.672059 meditability-0.2.3/src/prog/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       66 2024-04-10 18:12:18.000000 meditability-0.2.3/src/prog/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11066 2024-04-10 18:12:18.000000 meditability-0.2.3/src/prog/arguments.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6259 2024-05-20 22:54:21.000000 meditability-0.2.3/src/prog/db_set.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      244 2024-04-11 19:10:35.000000 meditability-0.2.3/src/prog/debug_input_blocks.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7100 2024-05-21 19:25:58.000000 meditability-0.2.3/src/prog/guide_prediction.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1194 2024-05-20 19:35:11.000000 meditability-0.2.3/src/prog/list_editors.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1037 2024-02-16 23:52:11.000000 meditability-0.2.3/src/prog/mEdit.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7915 2024-05-20 18:42:28.000000 meditability-0.2.3/src/prog/medit_lib.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7069 2024-04-12 17:41:44.000000 meditability-0.2.3/src/prog/ncbi_cross_database.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4998 2024-05-20 18:47:28.000000 meditability-0.2.3/src/prog/offtarget_prediction.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-30 23:41:45.672059 meditability-0.2.3/src/smk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-12 17:32:35.000000 meditability-0.2.3/src/smk/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-30 23:41:45.676060 meditability-0.2.3/src/smk/config/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-12 17:32:35.000000 meditability-0.2.3/src/smk/config/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2209 2024-01-12 17:32:35.000000 meditability-0.2.3/src/smk/config/aws_download.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      469 2024-01-12 17:32:35.000000 meditability-0.2.3/src/smk/config/caspedia_ingest.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      201 2024-01-12 17:32:35.000000 meditability-0.2.3/src/smk/config/cluster.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2473 2024-01-12 17:32:35.000000 meditability-0.2.3/src/smk/config/guide_prediction_default_template.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2227 2024-01-12 17:32:35.000000 meditability-0.2.3/src/smk/config/guide_prediction_private_template.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      461 2024-01-12 17:32:35.000000 meditability-0.2.3/src/smk/config/hgvs_input.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      281 2024-01-12 17:32:35.000000 meditability-0.2.3/src/smk/config/id_convert.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       99 2024-01-12 17:32:35.000000 meditability-0.2.3/src/smk/config/medit_cluster.yaml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1226 2024-05-20 20:59:19.000000 meditability-0.2.3/src/smk/config/medit_database.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1839 2024-05-17 18:44:49.000000 meditability-0.2.3/src/smk/config/medit_guide_pred.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      613 2024-04-01 18:00:41.000000 meditability-0.2.3/src/smk/config/medit_offtarget.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1639 2024-01-12 17:32:35.000000 meditability-0.2.3/src/smk/config/preprocessing_configuration.yaml
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-30 23:41:45.676060 meditability-0.2.3/src/smk/envs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-12 17:32:35.000000 meditability-0.2.3/src/smk/envs/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      692 2024-01-12 18:02:39.000000 meditability-0.2.3/src/smk/envs/b_medit.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2233 2024-01-22 22:57:06.000000 meditability-0.2.3/src/smk/envs/backup_medit.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6513 2023-11-27 19:17:03.000000 meditability-0.2.3/src/smk/envs/bio.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1582 2024-04-01 18:00:41.000000 meditability-0.2.3/src/smk/envs/casoff.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      221 2024-01-12 17:32:35.000000 meditability-0.2.3/src/smk/envs/clinvar_pull.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1363 2024-01-12 17:32:35.000000 meditability-0.2.3/src/smk/envs/gdown.yaml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2289 2024-01-24 21:43:26.000000 meditability-0.2.3/src/smk/envs/medit.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      564 2024-01-17 02:04:41.000000 meditability-0.2.3/src/smk/envs/samtools.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2266 2024-01-22 21:59:06.000000 meditability-0.2.3/src/smk/envs/test_medit.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2533 2024-02-16 18:08:11.000000 meditability-0.2.3/src/smk/envs/vcf.yaml
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-30 23:41:45.680060 meditability-0.2.3/src/smk/pipelines/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      123 2024-01-12 17:32:35.000000 meditability-0.2.3/src/smk/pipelines/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3053 2024-01-12 17:32:35.000000 meditability-0.2.3/src/smk/pipelines/compression_routine.smk
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1242 2024-01-12 17:32:35.000000 meditability-0.2.3/src/smk/pipelines/filename_standardization.smk
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7265 2024-04-10 18:12:18.000000 meditability-0.2.3/src/smk/pipelines/guide_prediction.smk
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5963 2024-05-18 00:06:25.000000 meditability-0.2.3/src/smk/pipelines/offtarget_prediction.smk
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-30 23:41:45.680060 meditability-0.2.3/src/smk/pipelines/py/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-12 00:46:24.000000 meditability-0.2.3/src/smk/pipelines/py/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11130 2024-05-16 19:20:00.000000 meditability-0.2.3/src/smk/pipelines/py/annotate.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2342 2023-10-03 00:05:02.000000 meditability-0.2.3/src/smk/pipelines/py/aws_pull.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5963 2024-04-01 18:00:41.000000 meditability-0.2.3/src/smk/pipelines/py/build_casoff_input.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4266 2024-04-01 18:00:41.000000 meditability-0.2.3/src/smk/pipelines/py/build_casoff_output.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7717 2023-11-02 16:12:49.000000 meditability-0.2.3/src/smk/pipelines/py/clinVar_pull.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19354 2024-05-16 19:20:00.000000 meditability-0.2.3/src/smk/pipelines/py/dataH.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4373 2024-02-27 07:13:06.000000 meditability-0.2.3/src/smk/pipelines/py/deepcas_models.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      884 2024-05-21 00:30:43.000000 meditability-0.2.3/src/smk/pipelines/py/fasta_chromosome_rename.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14046 2024-01-11 00:35:10.000000 meditability-0.2.3/src/smk/pipelines/py/featurization.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20926 2024-05-21 19:45:50.000000 meditability-0.2.3/src/smk/pipelines/py/fetchGuides.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20091 2024-05-16 19:20:00.000000 meditability-0.2.3/src/smk/pipelines/py/find_offtargets.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4278 2023-09-27 16:24:56.000000 meditability-0.2.3/src/smk/pipelines/py/gdrive_import.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3658 2023-10-16 17:01:06.000000 meditability-0.2.3/src/smk/pipelines/py/genome_seq_search.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16732 2024-03-12 23:53:04.000000 meditability-0.2.3/src/smk/pipelines/py/make_tables.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5481 2024-02-16 18:08:11.000000 meditability-0.2.3/src/smk/pipelines/py/ncbi_cross_database.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4988 2024-01-17 18:04:18.000000 meditability-0.2.3/src/smk/pipelines/py/omim2hgvs.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12085 2024-05-21 19:46:06.000000 meditability-0.2.3/src/smk/pipelines/py/process_genome.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14133 2024-05-16 19:20:00.000000 meditability-0.2.3/src/smk/pipelines/py/scoring.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17166 2023-10-23 21:12:40.000000 meditability-0.2.3/src/smk/pipelines/py/validate.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3701 2024-01-31 16:49:32.000000 meditability-0.2.3/src/smk/pipelines/vcf_processing.smk
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 19:38:21.163508 meditability-0.2.3a0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32337 2024-01-30 21:30:29.000000 meditability-0.2.3a0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      277 2024-05-21 19:38:21.163508 meditability-0.2.3a0/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3621 2024-02-16 18:08:11.000000 meditability-0.2.3a0/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-21 19:38:21.163508 meditability-0.2.3a0/setup.cfg
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1098 2024-05-17 18:06:03.000000 meditability-0.2.3a0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 19:38:21.151507 meditability-0.2.3a0/src/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 19:38:21.151507 meditability-0.2.3a0/src/meditability.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      277 2024-05-21 19:38:21.000000 meditability-0.2.3a0/src/meditability.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2300 2024-05-21 19:38:21.000000 meditability-0.2.3a0/src/meditability.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-21 19:38:21.000000 meditability-0.2.3a0/src/meditability.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       66 2024-05-21 19:38:21.000000 meditability-0.2.3a0/src/meditability.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      166 2024-05-21 19:38:21.000000 meditability-0.2.3a0/src/meditability.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-05-21 19:38:21.000000 meditability-0.2.3a0/src/meditability.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 19:38:21.155507 meditability-0.2.3a0/src/prog/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       66 2024-04-10 18:12:18.000000 meditability-0.2.3a0/src/prog/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11066 2024-04-10 18:12:18.000000 meditability-0.2.3a0/src/prog/arguments.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6259 2024-05-20 22:54:21.000000 meditability-0.2.3a0/src/prog/db_set.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      244 2024-04-11 19:10:35.000000 meditability-0.2.3a0/src/prog/debug_input_blocks.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7100 2024-05-21 19:25:58.000000 meditability-0.2.3a0/src/prog/guide_prediction.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1194 2024-05-20 19:35:11.000000 meditability-0.2.3a0/src/prog/list_editors.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1037 2024-02-16 23:52:11.000000 meditability-0.2.3a0/src/prog/mEdit.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7915 2024-05-20 18:42:28.000000 meditability-0.2.3a0/src/prog/medit_lib.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7069 2024-04-12 17:41:44.000000 meditability-0.2.3a0/src/prog/ncbi_cross_database.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4998 2024-05-20 18:47:28.000000 meditability-0.2.3a0/src/prog/offtarget_prediction.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 19:38:21.155507 meditability-0.2.3a0/src/smk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-12 17:32:35.000000 meditability-0.2.3a0/src/smk/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 19:38:21.155507 meditability-0.2.3a0/src/smk/config/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-12 17:32:35.000000 meditability-0.2.3a0/src/smk/config/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2209 2024-01-12 17:32:35.000000 meditability-0.2.3a0/src/smk/config/aws_download.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      469 2024-01-12 17:32:35.000000 meditability-0.2.3a0/src/smk/config/caspedia_ingest.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      201 2024-01-12 17:32:35.000000 meditability-0.2.3a0/src/smk/config/cluster.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2473 2024-01-12 17:32:35.000000 meditability-0.2.3a0/src/smk/config/guide_prediction_default_template.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2227 2024-01-12 17:32:35.000000 meditability-0.2.3a0/src/smk/config/guide_prediction_private_template.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      461 2024-01-12 17:32:35.000000 meditability-0.2.3a0/src/smk/config/hgvs_input.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      281 2024-01-12 17:32:35.000000 meditability-0.2.3a0/src/smk/config/id_convert.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       99 2024-01-12 17:32:35.000000 meditability-0.2.3a0/src/smk/config/medit_cluster.yaml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1226 2024-05-20 20:59:19.000000 meditability-0.2.3a0/src/smk/config/medit_database.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1839 2024-05-17 18:44:49.000000 meditability-0.2.3a0/src/smk/config/medit_guide_pred.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      613 2024-04-01 18:00:41.000000 meditability-0.2.3a0/src/smk/config/medit_offtarget.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1639 2024-01-12 17:32:35.000000 meditability-0.2.3a0/src/smk/config/preprocessing_configuration.yaml
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 19:38:21.159508 meditability-0.2.3a0/src/smk/envs/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-12 17:32:35.000000 meditability-0.2.3a0/src/smk/envs/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      692 2024-01-12 18:02:39.000000 meditability-0.2.3a0/src/smk/envs/b_medit.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2233 2024-01-22 22:57:06.000000 meditability-0.2.3a0/src/smk/envs/backup_medit.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6513 2023-11-27 19:17:03.000000 meditability-0.2.3a0/src/smk/envs/bio.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1582 2024-04-01 18:00:41.000000 meditability-0.2.3a0/src/smk/envs/casoff.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      221 2024-01-12 17:32:35.000000 meditability-0.2.3a0/src/smk/envs/clinvar_pull.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1363 2024-01-12 17:32:35.000000 meditability-0.2.3a0/src/smk/envs/gdown.yaml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2289 2024-01-24 21:43:26.000000 meditability-0.2.3a0/src/smk/envs/medit.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      564 2024-01-17 02:04:41.000000 meditability-0.2.3a0/src/smk/envs/samtools.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2266 2024-01-22 21:59:06.000000 meditability-0.2.3a0/src/smk/envs/test_medit.yaml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2533 2024-02-16 18:08:11.000000 meditability-0.2.3a0/src/smk/envs/vcf.yaml
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 19:38:21.159508 meditability-0.2.3a0/src/smk/pipelines/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      123 2024-01-12 17:32:35.000000 meditability-0.2.3a0/src/smk/pipelines/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3053 2024-01-12 17:32:35.000000 meditability-0.2.3a0/src/smk/pipelines/compression_routine.smk
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1242 2024-01-12 17:32:35.000000 meditability-0.2.3a0/src/smk/pipelines/filename_standardization.smk
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7265 2024-04-10 18:12:18.000000 meditability-0.2.3a0/src/smk/pipelines/guide_prediction.smk
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5963 2024-05-18 00:06:25.000000 meditability-0.2.3a0/src/smk/pipelines/offtarget_prediction.smk
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-21 19:38:21.163508 meditability-0.2.3a0/src/smk/pipelines/py/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-01-12 00:46:24.000000 meditability-0.2.3a0/src/smk/pipelines/py/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11130 2024-05-16 19:20:00.000000 meditability-0.2.3a0/src/smk/pipelines/py/annotate.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2342 2023-10-03 00:05:02.000000 meditability-0.2.3a0/src/smk/pipelines/py/aws_pull.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5963 2024-04-01 18:00:41.000000 meditability-0.2.3a0/src/smk/pipelines/py/build_casoff_input.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4266 2024-04-01 18:00:41.000000 meditability-0.2.3a0/src/smk/pipelines/py/build_casoff_output.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7717 2023-11-02 16:12:49.000000 meditability-0.2.3a0/src/smk/pipelines/py/clinVar_pull.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19354 2024-05-16 19:20:00.000000 meditability-0.2.3a0/src/smk/pipelines/py/dataH.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4373 2024-02-27 07:13:06.000000 meditability-0.2.3a0/src/smk/pipelines/py/deepcas_models.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      884 2024-05-21 00:30:43.000000 meditability-0.2.3a0/src/smk/pipelines/py/fasta_chromosome_rename.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14046 2024-01-11 00:35:10.000000 meditability-0.2.3a0/src/smk/pipelines/py/featurization.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20907 2024-05-21 19:05:45.000000 meditability-0.2.3a0/src/smk/pipelines/py/fetchGuides.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20091 2024-05-16 19:20:00.000000 meditability-0.2.3a0/src/smk/pipelines/py/find_offtargets.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4278 2023-09-27 16:24:56.000000 meditability-0.2.3a0/src/smk/pipelines/py/gdrive_import.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3658 2023-10-16 17:01:06.000000 meditability-0.2.3a0/src/smk/pipelines/py/genome_seq_search.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16732 2024-03-12 23:53:04.000000 meditability-0.2.3a0/src/smk/pipelines/py/make_tables.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5481 2024-02-16 18:08:11.000000 meditability-0.2.3a0/src/smk/pipelines/py/ncbi_cross_database.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4988 2024-01-17 18:04:18.000000 meditability-0.2.3a0/src/smk/pipelines/py/omim2hgvs.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12063 2024-02-27 07:13:06.000000 meditability-0.2.3a0/src/smk/pipelines/py/process_genome.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14133 2024-05-16 19:20:00.000000 meditability-0.2.3a0/src/smk/pipelines/py/scoring.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17166 2023-10-23 21:12:40.000000 meditability-0.2.3a0/src/smk/pipelines/py/validate.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3701 2024-01-31 16:49:32.000000 meditability-0.2.3a0/src/smk/pipelines/vcf_processing.smk
```

### Comparing `meditability-0.2.3/LICENSE` & `meditability-0.2.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/README.md` & `meditability-0.2.3a0/README.md`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/setup.py` & `meditability-0.2.3a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # == Installed Modules
 from setuptools import setup, find_packages
 # == Project Modules
 
 
 setup(
     name='meditability',
-    version='0.2.3',
+    version='0.2.3-alpha',
     description='',
     author='Interventional Genomics Unit',
     author_email='',
     entry_points={
         "console_scripts": [
             "medit = prog:main",
             "ncbi_cross_db = prog:cross_db"
```

### Comparing `meditability-0.2.3/src/meditability.egg-info/SOURCES.txt` & `meditability-0.2.3a0/src/meditability.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/prog/arguments.py` & `meditability-0.2.3a0/src/prog/arguments.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/prog/db_set.py` & `meditability-0.2.3a0/src/prog/db_set.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/prog/guide_prediction.py` & `meditability-0.2.3a0/src/prog/guide_prediction.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/prog/list_editors.py` & `meditability-0.2.3a0/src/prog/list_editors.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/prog/mEdit.py` & `meditability-0.2.3a0/src/prog/mEdit.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/prog/medit_lib.py` & `meditability-0.2.3a0/src/prog/medit_lib.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/prog/ncbi_cross_database.py` & `meditability-0.2.3a0/src/prog/ncbi_cross_database.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/prog/offtarget_prediction.py` & `meditability-0.2.3a0/src/prog/offtarget_prediction.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/config/aws_download.yaml` & `meditability-0.2.3a0/src/smk/config/aws_download.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/config/guide_prediction_default_template.yaml` & `meditability-0.2.3a0/src/smk/config/guide_prediction_default_template.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/config/guide_prediction_private_template.yaml` & `meditability-0.2.3a0/src/smk/config/guide_prediction_private_template.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/config/medit_database.yaml` & `meditability-0.2.3a0/src/smk/config/medit_database.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/config/medit_guide_pred.yaml` & `meditability-0.2.3a0/src/smk/config/medit_guide_pred.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/config/medit_offtarget.yaml` & `meditability-0.2.3a0/src/smk/config/medit_offtarget.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/config/preprocessing_configuration.yaml` & `meditability-0.2.3a0/src/smk/config/preprocessing_configuration.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/envs/b_medit.yaml` & `meditability-0.2.3a0/src/smk/envs/b_medit.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/envs/backup_medit.yaml` & `meditability-0.2.3a0/src/smk/envs/backup_medit.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/envs/bio.yaml` & `meditability-0.2.3a0/src/smk/envs/bio.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/envs/casoff.yaml` & `meditability-0.2.3a0/src/smk/envs/casoff.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/envs/gdown.yaml` & `meditability-0.2.3a0/src/smk/envs/gdown.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/envs/medit.yaml` & `meditability-0.2.3a0/src/smk/envs/medit.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/envs/samtools.yaml` & `meditability-0.2.3a0/src/smk/envs/samtools.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/envs/test_medit.yaml` & `meditability-0.2.3a0/src/smk/envs/test_medit.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/envs/vcf.yaml` & `meditability-0.2.3a0/src/smk/envs/vcf.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/pipelines/compression_routine.smk` & `meditability-0.2.3a0/src/smk/pipelines/compression_routine.smk`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/pipelines/filename_standardization.smk` & `meditability-0.2.3a0/src/smk/pipelines/filename_standardization.smk`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/pipelines/guide_prediction.smk` & `meditability-0.2.3a0/src/smk/pipelines/guide_prediction.smk`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/pipelines/offtarget_prediction.smk` & `meditability-0.2.3a0/src/smk/pipelines/offtarget_prediction.smk`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/pipelines/py/annotate.py` & `meditability-0.2.3a0/src/smk/pipelines/py/annotate.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/pipelines/py/aws_pull.py` & `meditability-0.2.3a0/src/smk/pipelines/py/aws_pull.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/pipelines/py/build_casoff_input.py` & `meditability-0.2.3a0/src/smk/pipelines/py/build_casoff_input.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/pipelines/py/build_casoff_output.py` & `meditability-0.2.3a0/src/smk/pipelines/py/build_casoff_output.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/pipelines/py/clinVar_pull.py` & `meditability-0.2.3a0/src/smk/pipelines/py/clinVar_pull.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/pipelines/py/dataH.py` & `meditability-0.2.3a0/src/smk/pipelines/py/dataH.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/pipelines/py/deepcas_models.py` & `meditability-0.2.3a0/src/smk/pipelines/py/deepcas_models.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/pipelines/py/fasta_chromosome_rename.py` & `meditability-0.2.3a0/src/smk/pipelines/py/fasta_chromosome_rename.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/pipelines/py/featurization.py` & `meditability-0.2.3a0/src/smk/pipelines/py/featurization.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/pipelines/py/fetchGuides.py` & `meditability-0.2.3a0/src/smk/pipelines/py/fetchGuides.py`

 * *Files 0% similar despite different names*

```diff
@@ -457,15 +457,15 @@
 		for ch, data in self.snv_info.items():
 
 			for d in data:
 				try:
 					query, tid, eid, gname, strand, ref, alt, feature_annotation, extracted_seq, codons, coord = d
 				except ValueError:
 					print(
-						f"WARNING: fetchGuides.py --> The query below has the wrong number of values to unpack. Needs further investigation:\n{d}")
+						f"WARNING: The query below has the wrong number of values to unpack. Needs further investigation:\n{d}")
 					continue
 				dh = DataHandler(query, strand, ref, alt, feature_annotation, models_dir, extracted_seq, codons, coord,
 								 gname, self.dist_from_cutsite)
 
 				if self.be_request != 'off':
 					guides, BEguides = dh.get_Guides(self.search_params, self.BE_search_params)
 				else:
```

### Comparing `meditability-0.2.3/src/smk/pipelines/py/find_offtargets.py` & `meditability-0.2.3a0/src/smk/pipelines/py/find_offtargets.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/pipelines/py/gdrive_import.py` & `meditability-0.2.3a0/src/smk/pipelines/py/gdrive_import.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/pipelines/py/genome_seq_search.py` & `meditability-0.2.3a0/src/smk/pipelines/py/genome_seq_search.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/pipelines/py/make_tables.py` & `meditability-0.2.3a0/src/smk/pipelines/py/make_tables.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/pipelines/py/ncbi_cross_database.py` & `meditability-0.2.3a0/src/smk/pipelines/py/ncbi_cross_database.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/pipelines/py/omim2hgvs.py` & `meditability-0.2.3a0/src/smk/pipelines/py/omim2hgvs.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/pipelines/py/process_genome.py` & `meditability-0.2.3a0/src/smk/pipelines/py/process_genome.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     new_guides = {}
     v_info = [[],[],[],[],[],[],[]]
     for ch, data in hg38_snvinfo.items():
         for d in data:
             try:
                 query, tid, eid, strand, hgref, hgalt, feature_annotation, hg38extracted_seq, codons, hg38coord = d
             except ValueError:
-                print(f"WARNING: process_genome.py --> The query below has the wrong number of values to unpack. "
+                print(f"WARNING: The query below has the wrong number of values to unpack. "
                       f"Needs further investigation:\n{d}")
                 continue
 
             # Check VCF if variant exsists in hg38 extracted_seq
             records_found = extract_vcf_record(snv_coord=hg38coord, vcf_fname = vcf_fname, window=30)
 
             if len(records_found) > 0:
```

### Comparing `meditability-0.2.3/src/smk/pipelines/py/scoring.py` & `meditability-0.2.3a0/src/smk/pipelines/py/scoring.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/pipelines/py/validate.py` & `meditability-0.2.3a0/src/smk/pipelines/py/validate.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.3/src/smk/pipelines/vcf_processing.smk` & `meditability-0.2.3a0/src/smk/pipelines/vcf_processing.smk`

 * *Files identical despite different names*

