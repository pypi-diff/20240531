# Comparing `tmp/meditability-0.2.2.tar.gz` & `tmp/meditability-0.2.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meditability-0.2.2.tar", last modified: Mon Apr  1 18:06:59 2024, max compression
+gzip compressed data, was "meditability-0.2.3a0.tar", last modified: Tue May 21 19:38:21 2024, max compression
```

## Comparing `meditability-0.2.2.tar` & `meditability-0.2.3a0.tar`

### file list

```diff
@@ -1,75 +1,81 @@
-drwxr-xr-x   0 bellieny   (501) staff       (20)        0 2024-04-01 18:06:59.772370 meditability-0.2.2/
--rw-r--r--   0 bellieny   (501) staff       (20)    32337 2024-01-30 21:30:29.000000 meditability-0.2.2/LICENSE
--rw-r--r--   0 bellieny   (501) staff       (20)      558 2024-04-01 18:06:59.768252 meditability-0.2.2/PKG-INFO
--rw-r--r--   0 bellieny   (501) staff       (20)     3621 2024-02-16 18:08:11.000000 meditability-0.2.2/README.md
--rw-r--r--   0 bellieny   (501) staff       (20)       38 2024-04-01 18:06:59.772450 meditability-0.2.2/setup.cfg
--rw-r--r--   0 bellieny   (501) staff       (20)     1018 2024-03-13 00:31:40.000000 meditability-0.2.2/setup.py
-drwxr-xr-x   0 bellieny   (501) staff       (20)        0 2024-04-01 18:06:59.369024 meditability-0.2.2/src/
-drwxr-xr-x   0 bellieny   (501) staff       (20)        0 2024-04-01 18:06:59.766007 meditability-0.2.2/src/meditability.egg-info/
--rw-r--r--   0 bellieny   (501) staff       (20)      558 2024-04-01 18:06:58.000000 meditability-0.2.2/src/meditability.egg-info/PKG-INFO
--rw-r--r--   0 bellieny   (501) staff       (20)     2121 2024-04-01 18:06:59.000000 meditability-0.2.2/src/meditability.egg-info/SOURCES.txt
--rw-r--r--   0 bellieny   (501) staff       (20)        1 2024-04-01 18:06:58.000000 meditability-0.2.2/src/meditability.egg-info/dependency_links.txt
--rw-r--r--   0 bellieny   (501) staff       (20)       36 2024-04-01 18:06:58.000000 meditability-0.2.2/src/meditability.egg-info/entry_points.txt
--rw-r--r--   0 bellieny   (501) staff       (20)      148 2024-04-01 18:06:58.000000 meditability-0.2.2/src/meditability.egg-info/requires.txt
--rw-r--r--   0 bellieny   (501) staff       (20)        9 2024-04-01 18:06:58.000000 meditability-0.2.2/src/meditability.egg-info/top_level.txt
-drwxr-xr-x   0 bellieny   (501) staff       (20)        0 2024-04-01 18:06:59.506374 meditability-0.2.2/src/prog/
--rw-r--r--   0 bellieny   (501) staff       (20)       24 2024-01-12 17:32:35.000000 meditability-0.2.2/src/prog/__init__.py
--rw-r--r--   0 bellieny   (501) staff       (20)    11022 2024-04-01 18:00:41.000000 meditability-0.2.2/src/prog/arguments.py
--rw-r--r--   0 bellieny   (501) staff       (20)     5602 2024-02-16 18:08:11.000000 meditability-0.2.2/src/prog/db_set.py
--rw-r--r--   0 bellieny   (501) staff       (20)     6932 2024-04-01 18:00:41.000000 meditability-0.2.2/src/prog/guide_prediction.py
--rw-r--r--   0 bellieny   (501) staff       (20)     1144 2024-04-01 18:00:41.000000 meditability-0.2.2/src/prog/list_editors.py
--rw-r--r--   0 bellieny   (501) staff       (20)     1037 2024-02-16 23:52:11.000000 meditability-0.2.2/src/prog/mEdit.py
--rw-r--r--   0 bellieny   (501) staff       (20)     7693 2024-04-01 18:00:41.000000 meditability-0.2.2/src/prog/medit_lib.py
--rw-r--r--   0 bellieny   (501) staff       (20)     4968 2024-04-01 18:00:41.000000 meditability-0.2.2/src/prog/offtarget_prediction.py
-drwxr-xr-x   0 bellieny   (501) staff       (20)        0 2024-04-01 18:06:59.508356 meditability-0.2.2/src/smk/
--rw-r--r--   0 bellieny   (501) staff       (20)        0 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/__init__.py
-drwxr-xr-x   0 bellieny   (501) staff       (20)        0 2024-04-01 18:06:59.568907 meditability-0.2.2/src/smk/config/
--rw-r--r--   0 bellieny   (501) staff       (20)        0 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/config/__init__.py
--rw-r--r--   0 bellieny   (501) staff       (20)     2209 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/config/aws_download.yaml
--rw-r--r--   0 bellieny   (501) staff       (20)      469 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/config/caspedia_ingest.yaml
--rw-r--r--   0 bellieny   (501) staff       (20)      201 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/config/cluster.yaml
--rw-r--r--   0 bellieny   (501) staff       (20)     2473 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/config/guide_prediction_default_template.yaml
--rw-r--r--   0 bellieny   (501) staff       (20)     2227 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/config/guide_prediction_private_template.yaml
--rw-r--r--   0 bellieny   (501) staff       (20)      461 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/config/hgvs_input.yaml
--rw-r--r--   0 bellieny   (501) staff       (20)      281 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/config/id_convert.yaml
--rw-r--r--   0 bellieny   (501) staff       (20)       99 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/config/medit_cluster.yaml
--rw-r--r--   0 bellieny   (501) staff       (20)     1226 2024-02-16 18:08:11.000000 meditability-0.2.2/src/smk/config/medit_database.yaml
--rw-r--r--   0 bellieny   (501) staff       (20)     1841 2024-04-01 18:00:41.000000 meditability-0.2.2/src/smk/config/medit_guide_pred.yaml
--rw-r--r--   0 bellieny   (501) staff       (20)      613 2024-04-01 18:00:41.000000 meditability-0.2.2/src/smk/config/medit_offtarget.yaml
--rw-r--r--   0 bellieny   (501) staff       (20)     1639 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/config/preprocessing_configuration.yaml
-drwxr-xr-x   0 bellieny   (501) staff       (20)        0 2024-04-01 18:06:59.628584 meditability-0.2.2/src/smk/envs/
--rw-r--r--   0 bellieny   (501) staff       (20)        0 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/envs/__init__.py
--rw-r--r--   0 bellieny   (501) staff       (20)      692 2024-01-12 18:02:39.000000 meditability-0.2.2/src/smk/envs/b_medit.yaml
--rw-r--r--   0 bellieny   (501) staff       (20)     1582 2024-04-01 18:00:41.000000 meditability-0.2.2/src/smk/envs/casoff.yaml
--rw-r--r--   0 bellieny   (501) staff       (20)      221 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/envs/clinvar_pull.yaml
--rw-r--r--   0 bellieny   (501) staff       (20)     1363 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/envs/gdown.yaml
--rw-r--r--   0 bellieny   (501) staff       (20)     2289 2024-01-24 21:43:26.000000 meditability-0.2.2/src/smk/envs/medit.yaml
--rw-r--r--   0 bellieny   (501) staff       (20)      564 2024-01-17 02:04:41.000000 meditability-0.2.2/src/smk/envs/samtools.yaml
--rw-r--r--   0 bellieny   (501) staff       (20)     2533 2024-02-16 18:08:11.000000 meditability-0.2.2/src/smk/envs/vcf.yaml
-drwxr-xr-x   0 bellieny   (501) staff       (20)        0 2024-04-01 18:06:59.660987 meditability-0.2.2/src/smk/pipelines/
--rw-r--r--   0 bellieny   (501) staff       (20)      123 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/pipelines/__init__.py
--rw-r--r--   0 bellieny   (501) staff       (20)     3053 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/pipelines/compression_routine.smk
--rw-r--r--   0 bellieny   (501) staff       (20)     1242 2024-01-12 17:32:35.000000 meditability-0.2.2/src/smk/pipelines/filename_standardization.smk
--rw-r--r--   0 bellieny   (501) staff       (20)     7280 2024-04-01 18:00:41.000000 meditability-0.2.2/src/smk/pipelines/guide_prediction.smk
--rw-r--r--   0 bellieny   (501) staff       (20)     5660 2024-04-01 18:00:41.000000 meditability-0.2.2/src/smk/pipelines/offtarget_prediction.smk
-drwxr-xr-x   0 bellieny   (501) staff       (20)        0 2024-04-01 18:06:59.759505 meditability-0.2.2/src/smk/pipelines/py/
--rw-r--r--   0 bellieny   (501) staff       (20)        0 2024-01-12 00:46:24.000000 meditability-0.2.2/src/smk/pipelines/py/__init__.py
--rw-r--r--   0 bellieny   (501) staff       (20)    12717 2024-01-23 20:04:30.000000 meditability-0.2.2/src/smk/pipelines/py/annotate.py
--rw-r--r--   0 bellieny   (501) staff       (20)     2342 2023-10-03 00:05:02.000000 meditability-0.2.2/src/smk/pipelines/py/aws_pull.py
--rw-r--r--   0 bellieny   (501) staff       (20)     5963 2024-04-01 18:00:41.000000 meditability-0.2.2/src/smk/pipelines/py/build_casoff_input.py
--rw-r--r--   0 bellieny   (501) staff       (20)     4266 2024-04-01 18:00:41.000000 meditability-0.2.2/src/smk/pipelines/py/build_casoff_output.py
--rw-r--r--   0 bellieny   (501) staff       (20)     7717 2023-11-02 16:12:49.000000 meditability-0.2.2/src/smk/pipelines/py/clinVar_pull.py
--rw-r--r--   0 bellieny   (501) staff       (20)    17522 2024-04-01 18:00:42.000000 meditability-0.2.2/src/smk/pipelines/py/dataH.py
--rw-r--r--   0 bellieny   (501) staff       (20)     4373 2024-02-27 07:13:06.000000 meditability-0.2.2/src/smk/pipelines/py/deepcas_models.py
--rw-r--r--   0 bellieny   (501) staff       (20)      581 2024-02-01 17:56:08.000000 meditability-0.2.2/src/smk/pipelines/py/fasta_chromosome_rename.py
--rw-r--r--   0 bellieny   (501) staff       (20)    14046 2024-01-11 00:35:10.000000 meditability-0.2.2/src/smk/pipelines/py/featurization.py
--rw-r--r--   0 bellieny   (501) staff       (20)    19981 2024-04-01 18:00:42.000000 meditability-0.2.2/src/smk/pipelines/py/fetchGuides.py
--rw-r--r--   0 bellieny   (501) staff       (20)    19745 2024-02-16 23:52:11.000000 meditability-0.2.2/src/smk/pipelines/py/find_offtargets.py
--rw-r--r--   0 bellieny   (501) staff       (20)     4278 2023-09-27 16:24:56.000000 meditability-0.2.2/src/smk/pipelines/py/gdrive_import.py
--rw-r--r--   0 bellieny   (501) staff       (20)     3658 2023-10-16 17:01:06.000000 meditability-0.2.2/src/smk/pipelines/py/genome_seq_search.py
--rw-r--r--   0 bellieny   (501) staff       (20)    16732 2024-03-12 23:53:04.000000 meditability-0.2.2/src/smk/pipelines/py/make_tables.py
--rw-r--r--   0 bellieny   (501) staff       (20)     5481 2024-02-16 18:08:11.000000 meditability-0.2.2/src/smk/pipelines/py/ncbi_cross_database.py
--rw-r--r--   0 bellieny   (501) staff       (20)    12063 2024-02-27 07:13:06.000000 meditability-0.2.2/src/smk/pipelines/py/process_genome.py
--rw-r--r--   0 bellieny   (501) staff       (20)    14218 2024-02-22 04:49:22.000000 meditability-0.2.2/src/smk/pipelines/py/scoring.py
--rw-r--r--   0 bellieny   (501) staff       (20)    17166 2023-10-23 21:12:40.000000 meditability-0.2.2/src/smk/pipelines/py/validate.py
--rw-r--r--   0 bellieny   (501) staff       (20)     3701 2024-01-31 16:49:32.000000 meditability-0.2.2/src/smk/pipelines/vcf_processing.smk
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

### Comparing `meditability-0.2.2/LICENSE` & `meditability-0.2.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `meditability-0.2.2/README.md` & `meditability-0.2.3a0/README.md`

 * *Files identical despite different names*

### Comparing `meditability-0.2.2/src/meditability.egg-info/SOURCES.txt` & `meditability-0.2.3a0/src/meditability.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 src/meditability.egg-info/dependency_links.txt
 src/meditability.egg-info/entry_points.txt
 src/meditability.egg-info/requires.txt
 src/meditability.egg-info/top_level.txt
 src/prog/__init__.py
 src/prog/arguments.py
 src/prog/db_set.py
+src/prog/debug_input_blocks.py
 src/prog/guide_prediction.py
 src/prog/list_editors.py
 src/prog/mEdit.py
 src/prog/medit_lib.py
+src/prog/ncbi_cross_database.py
 src/prog/offtarget_prediction.py
 src/smk/__init__.py
 src/smk/config/__init__.py
 src/smk/config/aws_download.yaml
 src/smk/config/caspedia_ingest.yaml
 src/smk/config/cluster.yaml
 src/smk/config/guide_prediction_default_template.yaml
@@ -27,19 +29,22 @@
 src/smk/config/medit_cluster.yaml
 src/smk/config/medit_database.yaml
 src/smk/config/medit_guide_pred.yaml
 src/smk/config/medit_offtarget.yaml
 src/smk/config/preprocessing_configuration.yaml
 src/smk/envs/__init__.py
 src/smk/envs/b_medit.yaml
+src/smk/envs/backup_medit.yaml
+src/smk/envs/bio.yaml
 src/smk/envs/casoff.yaml
 src/smk/envs/clinvar_pull.yaml
 src/smk/envs/gdown.yaml
 src/smk/envs/medit.yaml
 src/smk/envs/samtools.yaml
+src/smk/envs/test_medit.yaml
 src/smk/envs/vcf.yaml
 src/smk/pipelines/__init__.py
 src/smk/pipelines/compression_routine.smk
 src/smk/pipelines/filename_standardization.smk
 src/smk/pipelines/guide_prediction.smk
 src/smk/pipelines/offtarget_prediction.smk
 src/smk/pipelines/vcf_processing.smk
@@ -55,10 +60,11 @@
 src/smk/pipelines/py/featurization.py
 src/smk/pipelines/py/fetchGuides.py
 src/smk/pipelines/py/find_offtargets.py
 src/smk/pipelines/py/gdrive_import.py
 src/smk/pipelines/py/genome_seq_search.py
 src/smk/pipelines/py/make_tables.py
 src/smk/pipelines/py/ncbi_cross_database.py
+src/smk/pipelines/py/omim2hgvs.py
 src/smk/pipelines/py/process_genome.py
 src/smk/pipelines/py/scoring.py
 src/smk/pipelines/py/validate.py
```

### Comparing `meditability-0.2.2/src/prog/arguments.py` & `meditability-0.2.3a0/src/prog/arguments.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,22 +134,24 @@
 	                    mEdit will generate a random jobtag by default''')
 						)
 	run_params = fguides_parser.add_argument_group("== mEdit Core Parameters ==")
 	run_params.add_argument(
 		'-m',
 		dest='mode',
 		default='standard',
-		choices=['standard', 'private'],
+		choices=['fast', 'standard', 'private'],
 		help=textwrap.dedent('''
 			The MODE option determines how mEdit will run your job. 
 			[default = "standard"]
-			[1-] "standard": will find and process guides based on a 
+			[1-] "fast": will find and process guides based only on one 
+			reference human genome.
+			[2-] "standard": will find and process guides based on a 
 			reference human genome assembly along with a diverse set of 
 			pangenomes from HPRC.
-			[2-] "private": requires a private VCF file that will be 
+			[3-] "private": requires a private VCF file that will be 
 			 processed for guide prediction.''')
 	)
 	run_params.add_argument(
 		'-g',
 		dest='private_genome',
 		default=None,
 		help=textwrap.dedent('''
@@ -170,15 +172,14 @@
 			(ALT>REF). Alleles must be the plus strand.
 			Example: chr11:5226778C>T\n''')
 	)
 	run_params.add_argument(
 		'--editor',
 		dest='editor_request',
 		default='clinical',
-		choices=['clinical', 'custom', 'user defined list'],
 		help=textwrap.dedent('''
 			Delimits the set of editors to be used by mEdit. 
 			[default = "clinical"]
 			Use the "medit list" prompt to access the arrays of editors currently 
 			supported in each category.
 			[1-] "clinical": a short list of clinically relevant editors 
 			that are either in pre-clinical or clinical trials.
```

### Comparing `meditability-0.2.2/src/prog/db_set.py` & `meditability-0.2.3a0/src/prog/db_set.py`

 * *Files 13% similar despite different names*

```diff
@@ -45,31 +45,43 @@
 	processed_tables = f"{db_path_full}/{config_db_template['processed_tables']}"
 	config_db_template["processed_tables"] = f"{processed_tables}"
 	# config_db_template["simple_tables"] = f"{processed_tables}/{config_db_template['simple_tables']}"
 	# config_db_template["hgvs_lookup"] = f"{processed_tables}/{config_db_template['hgvs_lookup']}"
 	# config_db_template["clinvar_update"] = f"{processed_tables}/{config_db_template['clinvar_update']}"
 	config_db_template["refseq_table"] = f"{processed_tables}/{config_db_template['refseq_table']}"
 
+	# === Pull values from config variables
+	standard_ref_prefix = config_db_template["assembly_acc"]
+
 	#   == Parse the Raw Tables folder and its contents ==
 	# raw_tables = f"{db_path_full}/{config_db_template['raw_tables']}"
 	# config_db_template["raw_tables"] = f"{raw_tables}"
 	# config_db_template["clinvar_summary"] = f"{raw_tables}/{config_db_template['clinvar_summary']}"
 	# config_db_template["hpa"] = f"{raw_tables}/{config_db_template['hpa']}"
 	# config_db_template["gencode"] = f"{raw_tables}/{config_db_template['gencode']}"
 
 	# === Download Data ===
 	#   == SeqRecord Pickles
 	print("# ---*--- Database of Genomic References ---*---")
 	download_s3_objects("medit.db", "genome_pkl", fasta_root_path)
+	if not latest_genome_download:
+		standard_ref_path = f"{fasta_root_path}/hg38_{standard_ref_prefix}.fa"
+		launch_shell_cmd(f"bgzip -df -@ {threads} {standard_ref_path}.gz > {standard_ref_path}",
+						 message="Decompressing HPRC-compliant human reference genome")
+		pickle_chromosomes(standard_ref_path, fasta_root_path)
+		launch_shell_cmd(f"bgzip -cf -@ {threads} {standard_ref_path} > {standard_ref_path}.gz",
+						 message="Compressing human reference genome")
+		launch_shell_cmd(f"rm {standard_ref_path}",
+						 message="Cleaning up unused files")
 	# == Download the latest human reference genome by request
 	if latest_genome_download:
 		download_s3_objects("medit.db", "latest_genome_ref", fasta_root_path)
 		local_latest_ref_path = f"{fasta_root_path}/latest_hg38.fa"
 		pickle_chromosomes(local_latest_ref_path, fasta_root_path)
-		launch_shell_cmd(f"bgzip -c -@ {threads} {local_latest_ref_path} > {local_latest_ref_path}.gz",
+		launch_shell_cmd(f"bgzip -cf -@ {threads} {local_latest_ref_path} > {local_latest_ref_path}.gz",
 						 message="Compressing human reference genome")
 		launch_shell_cmd(f"rm {local_latest_ref_path}",
 						 message="Cleaning up unused files")
 		config_db_template["latest_reference"] = "True"
 	if custom_reference:
 		local_custom_ref_path = f"{fasta_root_path}/custom_reference.fa"
 		launch_shell_cmd(f"cp {custom_reference} {local_custom_ref_path}",
```

### Comparing `meditability-0.2.2/src/prog/guide_prediction.py` & `meditability-0.2.3a0/src/prog/guide_prediction.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import sys
 # == Installed Modules ==
 import yaml
 # == Project Modules ==
 from prog.medit_lib import (compress_file,
                             file_exists,
                             launch_shell_cmd,
-                            parse_editor_request,
                             project_file_path,
                             prRed,
                             set_export,
                             write_yaml_to_file
                             )
 
 
@@ -21,16 +20,16 @@
 	query_input = args.query_input
 	user_jobtag = args.user_jobtag
 	root_dir = abspath(args.output)
 	db_path_full = f"{abspath(args.db_path)}/medit_database"
 	mode = args.mode
 	private_genomes = args.private_genome
 	qtype = args.qtype_request
-	editor_request = parse_editor_request(args.editor_request)
-	be_request = parse_editor_request(args.be_request)
+	editor_request = args.editor_request
+	be_request = args.be_request
 	cutdist = args.cutdist
 
 	# == Load SLURM-related values ==
 	ncores = args.ncores
 	maxtime = args.maxtime
 	parallel_processes = args.parallel_processes
 	dry_run = args.dry_run
@@ -86,31 +85,15 @@
 	try:
 		with open(config_db_path, 'r') as config_db_handle:
 			config_db = yaml.safe_load(config_db_handle)
 	except FileNotFoundError:
 		prRed(f"Couldn't fund the file {config_db_path}. "
 		      f"Please double-check the path to <medit_database> and provide the path via '-d' option")
 
-	# === Assign Variables to Configuration File ===
-	config_template['run_name'] = f"{mode}_{jobtag}"
-	config_template['support_tables'] = db_path_full
-	config_template['processing_mode'] = mode
-	config_template['output_directory'] = root_dir
-	config_template['variant_query_dir'] = query_input
-	# Assign run parameters to config
-	config_template['qtype'] = qtype
-	config_template['editor_request'] = editor_request
-	config_template['be_request'] = be_request
-	config_template['distance_from_cutsite'] = cutdist
-	# Assign cluster options
-	cluster_template['__default__']['cores'] = ncores
-	cluster_template['__default__']['time'] = maxtime
-
-	# ->=== PRIVATE GENOME RUN ===<-
-	# == Check run mode ==
+	# ->=== CHECK RUN MODE ===<-
 	if mode == 'private':
 		# == Enforce presence of private genome in this mode ==
 		if not private_genomes:
 			print("Please provide a VCF input file to run mEdit's private mode")
 			sys.exit(1)
 		# == Create a private VCF directory when a private run is issued
 		vcf_dir_path = f"{config_db['meditdb_path']}/{mode}/source_vcfs"
@@ -136,14 +119,34 @@
 					#   => Create a copy of the VCF in the internal mEdit directory
 					launch_shell_cmd(f"cp {private_genome} {vcf_dir_path}/{vcf_filename}", True)
 					#   => Check VCF file compression and compress if necessary
 					compress_file(f"{vcf_dir_path}/{vcf_filename}")
 			count_tag += 1
 		#   => Add any amount of private genomes to the config file
 		config_template["vcf_id"] = tagged_genomes
+	elif mode == 'fast':
+		allowed_rules = ['--until "predict_guides" --omit-from consensus_fasta']
+		# == 'fast' mode is a sub-mode of 'standard';
+		# downstram processes must acknowledge that this is a standard run
+		mode = 'standard'
+
+	# === Assign Variables to Configuration File ===
+	config_template['run_name'] = f"{mode}_{jobtag}"
+	config_template['support_tables'] = db_path_full
+	config_template['processing_mode'] = mode
+	config_template['output_directory'] = root_dir
+	config_template['variant_query_dir'] = query_input
+	# Assign run parameters to config
+	config_template['qtype'] = qtype
+	config_template['editor_request'] = editor_request
+	config_template['be_request'] = be_request
+	config_template['distance_from_cutsite'] = cutdist
+	# Assign cluster options
+	cluster_template['__default__']['cores'] = ncores
+	cluster_template['__default__']['time'] = maxtime
 
 	# === Write YAML configs to mEdit Root Directory ===
 	write_yaml_to_file(config_template, dynamic_config_path)
 	write_yaml_to_file(cluster_template, dynamic_cluster_path)
 
 	# === Invoke SMK Pipelines ===
 
@@ -157,14 +160,16 @@
 			                 f"-j {ncores} "
 			                 f"{smk_run_triggers} "
 			                 f"{allowed_rules[smk_setup_idx]} "
 			                 f"{cluster_smk_setup[smk_setup_idx]} "
 			                 f"--configfile {config_db_path} "
 			                 f"{dynamic_config_path} "
 			                 f"--use-conda "
+							 f"--keep-going "
+							 f"--rerun-incomplete "
 			                 f"{dryrun_setup}",
 			                 smk_verbosity[smk_setup_idx]
 			                 )
 		except subprocess.CalledProcessError as e:
 			print(f"Error: {e}")
 		except ValueError:
 			print(f"Process completed in a previous run. Moving to the next one...")
```

### Comparing `meditability-0.2.2/src/prog/list_editors.py` & `meditability-0.2.3a0/src/prog/list_editors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # == Native Modules
 import pickle
 from os.path import abspath, isdir
 # == Installed Modules
 import yaml
 # == Project Modules
+from prog.medit_lib import file_exists
 
 
 def ls_editors(args):
 	# == Load Run Parameters values ==
 	# print_editors = args.editors
 	# print_base_editors = args.base_editors
 
 	# === Load Database Path ===
 	db_path_full = f"{abspath(args.db_path)}/medit_database"
 	config_db_path = f"{db_path_full}/config_db/config_db.yaml"
 
-	if not isdir(db_path_full):
-		raise f"The database path {db_path_full} is not a directory."
+	if not file_exists(db_path_full):
+		print("The database path directory could not be found.")
+		exit(0)
 
 	# === Load configuration file ===
 	with open(config_db_path, 'r') as config_handle:
 		config_db_obj = yaml.safe_load(config_handle)
 
 	# === Load Editors Lists From Path Specified on config_db.yaml ===
 	# if print_editors:
```

### Comparing `meditability-0.2.2/src/prog/mEdit.py` & `meditability-0.2.3a0/src/prog/mEdit.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.2/src/prog/medit_lib.py` & `meditability-0.2.3a0/src/prog/medit_lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,24 +5,28 @@
 from datetime import datetime
 import secrets
 import string
 import pytz
 import os
 import os.path
 import re
+import requests
 import pathlib
 from pathlib import Path
 import pickle
 # == Installed Modules ==
 from alive_progress import alive_bar
 import yaml
 from importlib_resources import files
 from Bio import SeqIO
 import boto3
 from botocore.exceptions import NoCredentialsError
+from botocore import UNSIGNED
+from botocore.config import Config
+
 import pandas as pd
 # == Project Modules ==
 
 
 def compress_file(file_path: str):
 	if not is_gzipped(file_path):
 		# If not gzipped, compress the file
@@ -63,31 +67,32 @@
 	"""
 	Downloads a file or every file in a given AWS S3 bucket
 	:param s3_bucket_name:
 	:param s3_object_name:
 	:param destination_path:
 	:return:
 	"""
-	s3 = boto3.client('s3')
+	s3 = boto3.client('s3', config=Config(signature_version=UNSIGNED))
 	try:
 		response = s3.list_objects_v2(Bucket=s3_bucket_name, Prefix=s3_object_name)
 		content = response.get('Contents', [])
 		clean_content = consolidate_s3_download(content, s3_object_name)  # Skip the S3 object that denotes the parent folder
 	except NoCredentialsError:
-		prRed("AWS Credentials not available. Please sign in then try again!")
+		prRed("AWS issued credentials error. This is not an expected behavior. Please notify log this error on GitHub")
 		exit(0)
 	with alive_bar(len(clean_content), title=f'Downloading s3://{s3_bucket_name}/{s3_object_name}') as bar:
 		for content_idx in range(0, len(clean_content)):
 			key = clean_content[content_idx]['Key']
 			source_file = key.split("/")[-1]
 			destination_file = os.path.join(destination_path, source_file)
 			if file_exists(destination_file):
 				print(f"Skipping existing file: {destination_file}")
 				bar()
 				continue
+			# == This downloads the data from the S3 Bucket without requiring AWS credentials
 			pathlib.Path(destination_path).mkdir(parents=True, exist_ok=True)
 			s3.download_file(s3_bucket_name, key, destination_file)
 			bar()
 
 
 def export_guides_by_editor(guide_df_by_editor_dict: dict, output_dir: (str, Path)):
 	editors_list = []
@@ -106,15 +111,19 @@
 	return os.path.exists(file_path)
 
 
 def group_guide_table(guide_table_path: pathlib.Path, editor_filter: (list, str)):
 	guides_df = pd.read_csv(guide_table_path)
 	if editor_filter:
 		guides_df = guides_df[guides_df['Editor'].isin(editor_filter)]
-	grouped_guides_df = guides_df.groupby('Editor')
+	try:
+		grouped_guides_df = guides_df.groupby('Editor')
+	except KeyError:
+		print("Column name 'Editor' not found in <Guides_found.csv>. Please check the file path and try again.")
+		exit(0)
 	editor_expanded_dictionary = {}
 	for editor, stats in grouped_guides_df:
 		editor_expanded_dictionary.setdefault(editor, []).append(stats)
 	return editor_expanded_dictionary
 
 
 def handle_shell_exception(subprocess_result, shell_command, verbose: bool):
@@ -177,22 +186,14 @@
 	for root, dirs, files in os.walk(root_path, topdown=False):
 		for name in files:
 			if name.endswith(extension):
 				file_list.append(os.path.join(root, name))
 	return file_list
 
 
-def parse_editor_request(request):
-	processed_request = request
-	if type(processed_request) is list:
-		processed_request = request.split(',')
-
-	return processed_request
-
-
 def pickle_chromosomes(genome_fasta, output_dir):
 	records = SeqIO.parse(open(genome_fasta, 'rt'), "fasta")
 	with alive_bar(25, title=f'Serializing human chromosomes') as bar:
 		for record in records:
 			if re.search(r"chr\w{0,2}$", record.id, re.IGNORECASE):
 				outfile = f"{output_dir}/{record.id}.pkl"
 				with open(outfile, 'ab') as gfile:
```

### Comparing `meditability-0.2.2/src/prog/offtarget_prediction.py` & `meditability-0.2.3a0/src/prog/offtarget_prediction.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,15 @@
 						 f"--snakefile {project_file_path('smk.pipelines', 'offtarget_prediction.smk')} "
 						 f"{smk_run_triggers} "
 						 f"-j {ncores} "
 						 f"{cluster_smk_setup} "
 						 f"--configfile {config_db_path} "
 						 f"{dynamic_config_guidepred_path} {dynamic_config_off_path} "
 						 f"--use-conda "
+						 f"--rerun-incomplete "
 						 f"{dryrun_setup} ",
 						 smk_verbosity
 						 )
 	except subprocess.CalledProcessError as e:
 		print(f"Error: {e}")
 	except ValueError:
 		print(f"Process completed in a previous run. Moving to the next one...")
```

### Comparing `meditability-0.2.2/src/smk/config/aws_download.yaml` & `meditability-0.2.3a0/src/smk/config/aws_download.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.2/src/smk/config/guide_prediction_default_template.yaml` & `meditability-0.2.3a0/src/smk/config/guide_prediction_default_template.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.2/src/smk/config/guide_prediction_private_template.yaml` & `meditability-0.2.3a0/src/smk/config/guide_prediction_private_template.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.2/src/smk/config/medit_database.yaml` & `meditability-0.2.3a0/src/smk/config/medit_database.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 fasta_root_path: "genome_pkl"
 # == Informs mEdit whether the latest reference genome available was
 #   included in the database unpacking
 latest_reference: ""
 # == Informs mEdit whether the user has provided a custom reference or not
 custom_reference: ""
 # == Current hg38 assembly accession
-assembly_acc: "GCF_000001405.40"
+assembly_acc: "GCA_000001405.15"
 
 # == PROCESSED TABLES ==
 # Main path for processed tables
 processed_tables: "processed_tables"
 # Processed filepaths
 #simple_tables: "guide_acquisition_tables"####DANIEL No Longer needed
 hgvs_lookup: "HGVSlookup.csv"
```

### Comparing `meditability-0.2.2/src/smk/config/medit_guide_pred.yaml` & `meditability-0.2.3a0/src/smk/config/medit_guide_pred.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # === GENERAL RUN PARAMETERS ===
 # Email address required for Entrez queries
 entrez_login: ""
 # Default thread number for processing in this and associated SMK pipeline
-threads: "1"
+threads: 1
 # Run name | the run names must follow the naming standard:
 # <date>_<medit_version>
 # ::date+time:: -> YYMMDDHHMMSSf
 # ::random alphanumeric:: -> 9m7aQ0KRZx
 run_name: ""
 # Must be the same as specified for the run_name
 processing_mode: ""
```

### Comparing `meditability-0.2.2/src/smk/config/medit_offtarget.yaml` & `meditability-0.2.3a0/src/smk/config/medit_offtarget.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.2/src/smk/config/preprocessing_configuration.yaml` & `meditability-0.2.3a0/src/smk/config/preprocessing_configuration.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.2/src/smk/envs/b_medit.yaml` & `meditability-0.2.3a0/src/smk/envs/b_medit.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.2/src/smk/envs/casoff.yaml` & `meditability-0.2.3a0/src/smk/envs/casoff.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.2/src/smk/envs/gdown.yaml` & `meditability-0.2.3a0/src/smk/envs/gdown.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.2/src/smk/envs/medit.yaml` & `meditability-0.2.3a0/src/smk/envs/medit.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.2/src/smk/envs/samtools.yaml` & `meditability-0.2.3a0/src/smk/envs/samtools.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.2/src/smk/envs/vcf.yaml` & `meditability-0.2.3a0/src/smk/envs/vcf.yaml`

 * *Files identical despite different names*

### Comparing `meditability-0.2.2/src/smk/pipelines/compression_routine.smk` & `meditability-0.2.3a0/src/smk/pipelines/compression_routine.smk`

 * *Files identical despite different names*

### Comparing `meditability-0.2.2/src/smk/pipelines/filename_standardization.smk` & `meditability-0.2.3a0/src/smk/pipelines/filename_standardization.smk`

 * *Files identical despite different names*

### Comparing `meditability-0.2.2/src/smk/pipelines/guide_prediction.smk` & `meditability-0.2.3a0/src/smk/pipelines/guide_prediction.smk`

 * *Files 2% similar despite different names*

```diff
@@ -11,82 +11,29 @@
 # nohup snakemake --snakefile guide_prediction.smk -j 1 --cluster "sbatch -t {cluster.time} -n {cluster.cores}" --cluster-config config/cluster.yaml --use-conda &
 
 # Description:
 
 # noinspection SmkAvoidTabWhitespace
 rule all:
 	input:
+		# Predicted guides using the most recent human genome assembly
+		expand("{root_dir}/{mode}/jobs/{run_name}/guide_prediction-{sequence_id}/guides_report_ref/Guides_found.csv",
+			root_dir=config["output_directory"],mode=config["processing_mode"],
+			run_name=config["run_name"],sequence_id=config["sequence_id"]),
 		# With the relevant VCF downloaded, proceed with creating consensus FASTA
 		expand("{meditdb_path}/{mode}/consensus_refs/{sequence_id}/{vcf_id}.fa",
 			meditdb_path=config["meditdb_path"],mode=config["processing_mode"],
 			vcf_id=config["vcf_id"],sequence_id=config["sequence_id"]),
-		# Predicted guides using the most recent human genome assembly
-		expand("{root_dir}/{mode}/jobs/{run_name}/guide_prediction-{sequence_id}/guides_report_ref/Guides_found.csv",
-			root_dir=config["output_directory"], mode=config["processing_mode"],
-			run_name=config["run_name"], sequence_id=config["sequence_id"]),
 		# Predicted guides on alternative genomes based on the reference listed above
 		expand("{root_dir}/{mode}/jobs/{run_name}/guide_prediction-{sequence_id}/guides_report_{vcf_id}/Guide_differences.csv",
 			root_dir=config["output_directory"],mode=config["processing_mode"],
 			run_name=config["run_name"],sequence_id=config["sequence_id"],
 			vcf_id=config["vcf_id"])
 
 # noinspection SmkAvoidTabWhitespace
-rule consensus_fasta:
-	input:
-		assembly_path=lambda wildcards: glob.glob("{fasta_root_path}/{sequence_id}.fa.gz".format(
-			fasta_root_path=config["fasta_root_path"],sequence_id=wildcards.sequence_id)),
-		source_vcf = "{meditdb_path}/{mode}/source_vcfs/{vcf_id}.vcf.gz"
-	output:
-		consensus_fasta = "{meditdb_path}/{mode}/consensus_refs/{sequence_id}/{vcf_id}.fa",
-		filtered_vcf = "{meditdb_path}/{mode}/consensus_refs/{sequence_id}/{vcf_id}.filtered.vcf.gz"
-	params:
-		source_vcf_prefix="{meditdb_path}/{mode}/consensus_refs/{sequence_id}/{vcf_id}",
-		dump_dir="{meditdb_path}/consensus_refs/downloads",
-		fasta_root_path=config["fasta_root_path"]
-	conda:
-		"../envs/samtools.yaml"
-	# resources:
-	# 	mem_mb=100000
-	message:
-		"""
-# === CREATE CONSENSUS FASTA === #
-This rule creates a consensus sequence based on a VCF file.
-Inputs used:
---> Human genome assembly: {input.assembly_path}
---> Source VCF: {input.source_vcf}
-Outputs generated:
---> Filtered VCF: {output.filtered_vcf}
---> Consensus genome sequence: {output.consensus_fasta}
-Wildcards in this rule:
---> {wildcards}
-		"""
-	shell:
-		"""
-		# Prepare directories:
-        # 2) filter GAT1 or GAT2 samples (samples where one haplotype has a sequence depth = 0)
-        # & filter reference & variant alleles > 5nt
-        # Create index file
-        bcftools filter -O z -o {output.filtered_vcf} -e 'GT="." || ILEN <= -5 || ILEN >= 5' {input.source_vcf} 
-        bcftools index -f -t {output.filtered_vcf}
-
-        # 3) Making a consensus
-        #previously made a seperate hg38 Ref Fasta that only have standard chromsomes --> /groups/clinical/projects/editability/tables/raw_tables/VCFs/hg38_standard.fa.gz
-        samtools dict {input.assembly_path} -o {params.fasta_root_path}/{wildcards.sequence_id}.dict
-        samtools faidx {input.assembly_path} -o {input.assembly_path}.fai
-
-        # gzip -dv {output.filtered_vcf}
-        # bgzip {params.source_vcf_prefix}.filtered.vcf
-
-        bcftools consensus -f {input.assembly_path} {output.filtered_vcf} -o {output.consensus_fasta}
-        
-        # Cleanup
-        # rm {input.assembly_path}.fai {params.fasta_root_path}/{wildcards.sequence_id}.dict
-        """
-
-# noinspection SmkAvoidTabWhitespace
 rule predict_guides:
 	input:
 		query_manifest = lambda wildcards: glob.glob("{variant_query_dir}".format(
 			variant_query_dir=config["variant_query_dir"])),
 		assembly_dir_path = lambda wildcards: glob.glob("{fasta_root_path}".format(
 			fasta_root_path=config["fasta_root_path"]))
 	output:
@@ -132,14 +79,67 @@
 Wildcards in this rule:
 --> {wildcards}
         """
 	script:
 		"py/fetchGuides.py"
 
 # noinspection SmkAvoidTabWhitespace
+rule consensus_fasta:
+	input:
+		assembly_path=lambda wildcards: glob.glob("{fasta_root_path}/{sequence_id}.fa.gz".format(
+			fasta_root_path=config["fasta_root_path"],sequence_id=wildcards.sequence_id)),
+		source_vcf="{meditdb_path}/{mode}/source_vcfs/{vcf_id}.vcf.gz",
+	output:
+		consensus_fasta="{meditdb_path}/{mode}/consensus_refs/{sequence_id}/{vcf_id}.fa",
+		filtered_vcf="{meditdb_path}/{mode}/consensus_refs/{sequence_id}/{vcf_id}.filtered.vcf.gz"
+	params:
+		source_vcf_prefix="{meditdb_path}/{mode}/consensus_refs/{sequence_id}/{vcf_id}",
+		dump_dir="{meditdb_path}/consensus_refs/downloads",
+		fasta_root_path=config["fasta_root_path"]
+	conda:
+		"../envs/samtools.yaml"
+	# resources:
+	# 	mem_mb=100000
+	message:
+		"""
+# === CREATE CONSENSUS FASTA === #
+This rule creates a consensus sequence based on a VCF file.
+Inputs used:
+--> Human genome assembly: {input.assembly_path}
+--> Source VCF: {input.source_vcf}
+Outputs generated:
+--> Filtered VCF: {output.filtered_vcf}
+--> Consensus genome sequence: {output.consensus_fasta}
+Wildcards in this rule:
+--> {wildcards}
+		"""
+	shell:
+		"""
+		# Prepare directories:
+        # 2) filter GAT1 or GAT2 samples (samples where one haplotype has a sequence depth = 0)
+        # & filter reference & variant alleles > 5nt
+        # Create index file
+        bcftools filter -O z -o {output.filtered_vcf} -e 'GT="." || ILEN <= -5 || ILEN >= 5' {input.source_vcf} 
+        bcftools index -f -t {output.filtered_vcf}
+
+        # 3) Making a consensus
+        #previously made a seperate hg38 Ref Fasta that only have standard chromsomes --> /groups/clinical/projects/editability/tables/raw_tables/VCFs/hg38_standard.fa.gz
+        samtools dict {input.assembly_path} -o {params.fasta_root_path}/{wildcards.sequence_id}.dict
+        samtools faidx {input.assembly_path} -o {input.assembly_path}.fai
+
+        # gzip -dv {output.filtered_vcf}
+        # bgzip {params.source_vcf_prefix}.filtered.vcf
+
+        bcftools consensus -f {input.assembly_path} {output.filtered_vcf} -o {output.consensus_fasta}
+
+        # Cleanup
+        # rm {input.assembly_path}.fai {params.fasta_root_path}/{wildcards.sequence_id}.dict
+        """
+
+# noinspection SmkAvoidTabWhitespace
 rule process_altgenomes:
 	input:
 		filtered_vcf = lambda wildcards: glob.glob("{meditdb_path}/{mode}/consensus_refs/{sequence_id}/{vcf_id}.filtered.vcf.gz".format(
 			meditdb_path=config["meditdb_path"],mode=wildcards.mode,
 			vcf_id=wildcards.vcf_id,sequence_id=wildcards.sequence_id
 		)),
 		guides_report_out= "{root_dir}/{mode}/jobs/{run_name}/guide_prediction-{sequence_id}/guides_report_ref/Guides_found.csv",
```

### Comparing `meditability-0.2.2/src/smk/pipelines/offtarget_prediction.smk` & `meditability-0.2.3a0/src/smk/pipelines/offtarget_prediction.smk`

 * *Files 9% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 # nohup snakemake --snakefile *.smk -j 1 --cluster "sbatch -t {cluster.time} -n {cluster.cores}" --cluster-config config/cluster.yaml --use-conda &
 
 # Description:
 
 # noinspection SmkAvoidTabWhitespace
 rule all:
 	input:
-		expand("{fasta_root_path}/{sequence_id}.fa",
-			fasta_root_path=config["fasta_root_path"], sequence_id=config["sequence_id"]),
+		# expand("{fasta_root_path}/{sequence_id}.fa",
+		# 	fasta_root_path=config["fasta_root_path"], sequence_id=config["sequence_id"]),
 		# Prepare input files for casoffinder on a per-editor basis
 		expand("{root_dir}/{mode}/jobs/{run_name}/guide_prediction-{sequence_id}/offtarget_prediction/input_files/{editing_tool}_casoff_in.txt",
 			root_dir=config["output_directory"],mode=config["processing_mode"],
 			run_name=config["run_name"], sequence_id=config["sequence_id"],
 			editing_tool=config["editors_list"]),
 		# Run Cas-Offinder
 		expand("{root_dir}/{mode}/jobs/{run_name}/guide_prediction-{sequence_id}/offtarget_prediction/{editing_tool}_casoff.txt",
@@ -39,18 +39,26 @@
 	params:
 		decompressed_assembly_path = lambda wildcards: glob.glob("{fasta_root_path}/{sequence_id}.fa".format(
 			fasta_root_path=config["fasta_root_path"],sequence_id=wildcards.sequence_id)),
 		link_directory = "{root_dir}/{mode}/jobs/{run_name}/guide_prediction-{sequence_id}/offtarget_prediction/"
 	priority: 50
 	message:
 		"""
+		# === PREPARING REFERENCE GENOMES FOR CASOFFINDER === #
+		Inputs used:
+		Compressed genome reference: {input.assembly_path}
+		Outputs:
+		Target directoru: {params.link_directory}
+		Decompressed genome reference: {output.decompressed_assembly_symlink}
+		Wildcards in this rule:
+		{wildcards}
 		"""
 	shell:
 		"""
-		gzip -kdv {input.assembly_path}
+		gzip -kdvf {input.assembly_path}
 		ln --symbolic -t {params.link_directory} {params.decompressed_assembly_path}
 		"""
 
 # noinspection SmkAvoidTabWhitespace
 rule casoff_input_formatting:
 	input:
 		guides_per_editor_path = "{root_dir}/{mode}/jobs/{run_name}/guide_prediction-{sequence_id}/offtarget_prediction/{editing_tool}.pkl",
@@ -93,15 +101,15 @@
 		rna_bulge=config["RNAbb"],
 		dna_bulge=config["DNAbb"],
 		max_mismatch=config["max_mismatch"],
 		casoff_accelerator=config["PU"]
 	conda:
 		"../envs/casoff.yaml"
 	threads:
-		config["threads"]
+		int(config["threads"])
 	message:
 		"""
 # === PREDICT OFFTARGET EFFECT === #
 Inputs used:
 --> Analyze off-target effect for guides predicted for: {wildcards.editing_tool}
 --> Take formatted inputs from :\n {input.casoff_input}
```

### Comparing `meditability-0.2.2/src/smk/pipelines/py/annotate.py` & `meditability-0.2.3a0/src/smk/pipelines/py/annotate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 # Native Modules
 import gzip
 from subprocess import Popen, PIPE
 import os
+
 # Installed Modules
 from Bio.Seq import Seq
-# Project Modules
 
+########
+###      Transcript Class is used to compute/retrieve transcript information based on a list of coordinates
+###      1: Load list of genomic coordinates and ncbiRefSeq.bed file path
+###      2: Call upon any of these coordinates using the NCBI transcript ID or coordinates
+###         to retreive  gene names, features, reading frame, feature positions and transcript sequence
+########
 
 class Transcript:
-    tx_lib = {} #tid : []
+    tx_lib = {}
     coord2tid = {}
     labels = ['chrom', 'txStart', 'txEnd', 'strand', 'tid', 'eid', 'name',
               'cdsStart', 'cdsEnd', 'exonStarts', 'exonEnds', 'exonFrames']
 
     def __init__(self,entry):
         '''
         :param entry: NCBI Transcript Entry
@@ -33,37 +39,26 @@
 
         self.feature = None
         self.rf = None
         self.cdsseq = None
         self.txseq = None
 
     @classmethod
-    def transcript(cls, snvcoord):
-        if snvcoord in cls.coord2tid.keys():
-            tid = cls.coord2tid[snvcoord]
-            start, end = snvcoord.split(':')[1].split('-')
-            pos = int((int(start) + int(end)) /2)
-            obj = cls.tx_lib[tid]
-            obj.find_feature(pos)
-            return obj
-        else:
-            return 'intergenic'
-
-    @classmethod
-    def load_transcripts(cls, annote_path,snvcoords):
-        # print('DANIEL WE MIGHT NEED TO MAKE A TEMP FOLDER')
-        # print('SEE load_transcripts in annotate.py')
-        temp_bedfname = "temp_in.bed"
-        bed_entries = None
+    def load_transcripts(cls, annote_path, snvcoords):
+        '''
+        Must be initiated before annotating!
+        Loads coordinates into Transcript Class
+        '''
+        temp_bedfname = f"temp{snvcoords[0][-1]}_in.bed"
 
-        #reset dict
+        # reset dict
         cls.coord2tid = {}
         cls.tx_lib = {}
 
-        with open(temp_bedfname, 'w') as tempbed:
+        with open(temp_bedfname, 'w') as tempbed: # create bed with coordinates
             for coord in snvcoords:
                 coord_field = coord.split(':')
                 chrom = coord_field[0]
                 start = coord_field[1].split('-')[0]
                 end = coord_field[1].split('-')[1]
                 line = "\t".join([chrom, start, end])
                 tempbed.writelines(line + "\n")
@@ -76,46 +71,61 @@
             print("Bedtools process was interrupted!")
         if bedtools_out != '':
             bed_entries = bedtools_out.split('\n')[:-1]
 
             for bed_entry in bed_entries:
                 tokens = bed_entry.split('\t')
                 tokens = tokens[:-1] + tokens[-1].split('|')
-                snvcoord = f'{tokens[0]}:{tokens[1]}-{tokens[2]}'
+                coord = f'{tokens[0]}:{tokens[1]}-{tokens[2]}'
                 entry = dict(zip(cls.labels, tokens[-12:]))
 
                 if entry['chrom'] != '.':
-                    if snvcoord not in cls.coord2tid.keys():
-                        cls.coord2tid[snvcoord] = entry['tid']
+                    if coord not in cls.coord2tid.keys():
+                        cls.coord2tid[coord] = entry['tid']
                         cls.tx_lib[entry['tid']] = cls(entry)
                     # adjusting for overlaps to retrieve the most up to date transcript
                     else:
                         new_tid = entry['tid']
-                        oldtid = cls.coord2tid[snvcoord]
+                        oldtid = cls.coord2tid[coord]
 
                         if new_tid.startswith('NR') and oldtid.startswith('NM'):
                             pass
 
                         elif new_tid[0:2] == oldtid[0:2]:
                             if entry['eid'] != '-' or (float(oldtid.split('_')[-1]) < float(new_tid.split('_')[-1])):
-                                cls.coord2tid[snvcoord] = new_tid
+                                cls.coord2tid[coord] = new_tid
                                 obj = cls(entry)
                                 obj.overlapping_transcripts.append(oldtid)
                                 cls.tx_lib[entry['tid']] = obj
                         else:
-                            cls.coord2tid[snvcoord] = new_tid
+                            cls.coord2tid[coord] = new_tid
                             obj = cls(entry)
                             obj.overlapping_transcripts.append(oldtid)
                             cls.tx_lib[entry['tid']] = obj
 
                 else:
-                    cls.coord2tid[snvcoord] = 'intergenic'
+                    cls.coord2tid[coord] = 'intergenic'
         os.remove(temp_bedfname)
+
+
+    @classmethod
+    def transcript(cls, snvcoord):
+        if snvcoord in cls.coord2tid.keys():
+            tid = cls.coord2tid[snvcoord]
+            start, end = snvcoord.split(':')[1].split('-')
+            pos = int((int(start) + int(end)) /2)
+            obj = cls.tx_lib[tid]
+            obj.find_feature(pos)
+            return obj
+        else:
+            return 'intergenic'
+
     def __dict__(self):
         return self.entry
+
     def get_utrs(self):
         exon_starts = self.entry['exonStarts'][:-1].split(',')
         exon_ends = self.entry['exonEnds'][:-1].split(',')
         if self.exons:
             ogexons = [(int(exon_starts[i]) - self.entry['txStart'], int(exon_ends[i]) - self.entry['txStart']) for i in range(len(exon_ends))]
             utrs= [(ogexons[0][0],self.exons[0][0]-1),(self.exons[-1][1],ogexons[-1][1]-1)]
         else:
@@ -249,80 +259,31 @@
         self.feature, self.rf = feature, rf
 
 
 '''test
 annote_path = '/groups/clinical/projects/editability/tables/processed_tables/ncbiRefSeq.bed.gz'
 snvcoords = ['chr11:5225460-5225460','chr11:5226676-5226676',
              'chr3:136250375-136250375','chr16:57744390-57744390',
-             'chr16:136330169-136330169','chr18:58671560-58671560'
-             ]
+             'chr16:136330169-136330169','chr18:58671560-58671560']
+             
 Transcript.load_transcripts(annote_path,snvcoords)
 for snv in snvcoords:
     pos_in_transcript = Transcript.transcript(snv)
     if pos_in_transcript != 'intergenic':
         print(pos_in_transcript.tx_info())
         print(pos_in_transcript.feature)
     else:
         print('intergenic', snv)
+        
 #('ENST00000335295.4', 'NM_000518.5', 'HBB', '-', 5225463)
 #flanking-downstream
 #('ENST00000335295.4', 'NM_000518.5', 'HBB', '-', 5225463)
 #exon
 #('-', 'NM_001178014.2', 'PCCB', '+', 136250339)
 #start_codon
 #('ENST00000379661.8', 'NM_005886.3', 'KATNB1', '+', 57735769)
 #intron
 #('ENST00000649217.2', 'NM_006785.4', 'MALT1', '+', 58671464)
 #5utr
 
 
 '''
-
-#    def get_refseq_entry(term, field):
-#        '''
-#        Using ncbiRefSeq.bed.gz to find cds features by either interval, gene name or transcript ID
-#        example input:
-#        term, field = 'NM_000532.5', 'tid'
-#        term, field = 'PCCB','name'
-#        term,field =  'chr3:136250339-136330169','interval'
-#        annote_path = '/groups/clinical/projects/editability/tables/processed_tables/ncbiRefSeq.bed.gz'
-#        '''
-#
-#        labels = ['chrom', 'txStart', 'txEnd','strand','tid','eid,','name',
-#                  'cdsStart', 'cdsEnd','exonStart','exonEnd', 'exonFrames']
-#
-#        if field != 'interval':
-#            not_found = True
-#            for line in gzip.open(annote_path, 'rt'):
-#                tokens = line.split('\t')
-#                entry = dict(zip(labels, tokens))
-#                if term in entry[field]:
-#                    not_found = False
-#                    break
-
-#            if not_found:
-#                entry = None
-#                print(f"{term} not found in refseq data")
-
- #               if '.' in term:
- #                   new_term = term.split('.')[0]
- #                   print(f'searching for {new_term} instead')
- #                   entry = get_refseq_entry(new_term, field,annote_path)
-
- #       else:  # only used for intervals search
- #           not_found = True
- #           ch = term.split(":")[0]
- #           start, end = term.split(":")[1].split('-')
- #           pos = int((int(start) + int(end)) / 2)
-
- #           for line in gzip.open(annote_path, 'rt'):
- #               tokens = line.split('\t')
- #               entry = dict(zip(labels, tokens))
- #               if ch == entry['chrom']:
- #                   if pos in range(int(entry['txStart']), int(entry['txEnd'])):
- #                       not_found = False
- #                       break
- #           if not_found:
- #               entry = None
- #               print(f"{term} not found in refseq data")
- #       return entry
-
```

### Comparing `meditability-0.2.2/src/smk/pipelines/py/aws_pull.py` & `meditability-0.2.3a0/src/smk/pipelines/py/aws_pull.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.2/src/smk/pipelines/py/build_casoff_input.py` & `meditability-0.2.3a0/src/smk/pipelines/py/build_casoff_input.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.2/src/smk/pipelines/py/build_casoff_output.py` & `meditability-0.2.3a0/src/smk/pipelines/py/build_casoff_output.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.2/src/smk/pipelines/py/clinVar_pull.py` & `meditability-0.2.3a0/src/smk/pipelines/py/clinVar_pull.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.2/src/smk/pipelines/py/dataH.py` & `meditability-0.2.3a0/src/smk/pipelines/py/dataH.py`

 * *Files 17% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         self.pamISfirst = False  # Boolean
         self.win_size = list()  # Ex. list [4,8]
         self.gscoring = None  # Ex. True/False
         self.guidelen = 20
 
         # outputs
         self.guides_found = {'QueryTerm': [], 'GeneName':[],'Editor': [], 'Guide_ID': [], 'Coordinates': [],
-                             'Strand': [], 'gRNA': [], 'Pam': [], 'Variant Position': [], 'Extended Guide Site': [],
+                             'Strand': [], 'gRNA': [], 'Pam': [], 'Extended Guide Site': [],'Variant Position': [],
                              'Azimuth Score': [], 'DeepCas9 Score':[],'DeepCpf1 Score':[],
                              'OOF Score':[],'Ref>Alt': [], 'Annotation': []}
 
         self.BEguides_found = {'QueryTerm': [], 'GeneName':[],'Editor': [], 'Guide_ID': [], 'Coordinates': [],
                                'Strand': [],'gRNA': [], 'Pam': [], 'Variant Position': [],'Extended Guide Site': [],
                                'ABE score':[], 'CBE Score':[],
                                'Hg38 Reference (Codon>AA)': [], 'Alternate (Codon>AA)': [], 'BE Converted (Codon>AA)': [],
@@ -214,100 +214,131 @@
         self.BEguides_found['Hg38 Reference (Codon>AA)'].append(ref)
         self.BEguides_found['Alternate (Codon>AA)'].append(alt)
         self.BEguides_found['BE Converted (Codon>AA)'].append(convert)
         self.BEguides_found['Conversion Type'].append(ctype)
         self.BEguides_found['Bystander'].append(bystander)
         self.BEguides_found['Annotation'].append(self.annotation)
 
-    def get_guide_set(self, name, pam, pamISfirst, win_size, guidelen, BEmode):
+    def get_guide_set(self, name, pam, pamISfirst, win_size, guidelen,cut_site_position, BEmode):
         """
-        :param name:
+        :param name: editor name
         :param pam: pam seq ex:'NGG'
         :param pamISfirst: 5'or3'PAM ex:True/False
         :param win_size: list containing upper and lower limits of the targetable window. Ex:[4,8]
-        :param search window: intial search + or - SNV site
         :param guidelen: guide without pam length
         :return: Guide Dictionary
         """
-
         guides = []
-        pamlen = len(pam)
-        sitelen = guidelen + pamlen
-        snv_rel_pos = int(len(self.extracted_seq)/2)
-        extended_guide = '-'
         scores = {'azimuth':'-',
                   'deepcas9':'-',
                   'deepcpf1':'-',
                   'oof':'-'}
-        if BEmode:
-            win_size = [win_size[0] - guidelen -1,win_size[1] -guidelen-1]
 
-        pam_min, pam_max = int((snv_rel_pos - win_size[1]))- 1, int((snv_rel_pos - win_size[0])) - 1
+        pamlen = len(pam)
+        sitelen = guidelen + pamlen
+        var_relative_pos = int(len(self.extracted_seq)/2)
+
+        if BEmode:
+            # Adjust window to 5' spacer
+            # Example Base editing window = 4-8
+            #     4   8
+            #  XXXXXXXXXXXXXXXXXXXXNGGxxxxxx
+            win_size = [win_size[0] - guidelen,win_size[1] -guidelen]
+            pam_min, pam_max = int((var_relative_pos + abs(win_size[1]))), int((var_relative_pos + abs(win_size[0]))) + 1
 
-        if pamISfirst == True:
-            pam_min, pam_max = pam_min + pamlen, pam_max + pamlen
+        else:
+            # Adjust window to 3' PAM
+            # Example cas9 editing window  with cut site position -3 and dist 7= -10 and +4
+            #           -10        1   4
+            #  XXXXXXXXXXXXXXXXXXXXNGGxxxxxx
+
+            x = int((var_relative_pos - abs(win_size[1])))
+            pam_min, pam_max = x, (x + abs(win_size[1] - win_size[0]))
+            if pamISfirst == True:
+                # Adjust window to 5' PAM
+                # Example cas12 editing window  with cut site position 18 and dist 7 = 15 and +29
+                #  1             15             29
+                #  TTTVXXXXXXXXXXXXXXXXXXXXxxxxxx
+                pam_min, pam_max = pam_min - pamlen, pam_max - pamlen
 
         # Narrow based on guide params
-        for search_strand in ["-", "+"]:
+        for search_strand in ["+", "-"]:
             search_seq = Seq(self.extracted_seq) if search_strand == "+" else Seq(self.extracted_seq).reverse_complement()
-            pam_index = SeqUtils.nt_search(str(search_seq), pam)[1:]
+            snv_rel_pos = var_relative_pos
+            if search_strand == "-":
+                pam_start, pam_end = pam_min, pam_max - 1
+                if not BEmode:
+                    snv_rel_pos = var_relative_pos - 1
+            else:
+                pam_start, pam_end = pam_min + 1, pam_max
+            pam_index = SeqUtils.nt_search(str(search_seq).upper(), pam)[1:]
 
             for i in pam_index:
-                if i in range(pam_min, pam_max + 1):
-                    extended_guide = '-'
+                if i in range(pam_start, pam_end+1):
                     scores = {'azimuth': '-',
                               'deepcas9': '-',
                               'deepcpf1': '-',
                               'oof': '-'}
                     if not pamISfirst:  # 3' PAM
                         target_start = i - guidelen
                         guide = search_seq[i - guidelen:i]
                         extended_guide = str(search_seq[target_start - 3:target_start + sitelen + 4])
                         if not BEmode:
+                            snvpos = snv_rel_pos - (i + cut_site_position)
+                            if snvpos >= 0:
+                                snvpos += 1
                             if pam == 'NGG' and guidelen == 20:
                                 #Azmith only accurate for NGG pams
-                                scores['azimuth'] = scoring.azimuth([extended_guide],
+                                scores['azimuth'] = scoring.azimuth([extended_guide.upper()],
                                                            self.models_dir)[0]
-                                scores['deepcas9'] = round(scoring.deepspcas9([extended_guide],
+                                scores['deepcas9'] = round(scoring.deepspcas9([extended_guide.upper()],
                                                            self.models_dir)[0][0],2)
                             #oof_score use only for DSB
-                            mh_score, scores['oof'] = scoring.oofscore(str(search_seq[target_start - 20:target_start + sitelen + 20]))
+                            mh_score, scores['oof'] = scoring.oofscore(str(search_seq[target_start - 20:target_start + sitelen + 20]).upper())
+                        else:
+                            snvpos = int([guide.index(x) + 1 for x in guide if x.islower()][0])
 
                         pam_found = str(search_seq[i:i + pamlen])
 
                     else:
-                        target_start = i + pamlen
-                        guide = search_seq[target_start: i + sitelen]
-                        pam_found = search_seq[i:target_start]
+                        target_start = i
+                        guide_start = i + pamlen
+                        guide = search_seq[guide_start: guide_start + guidelen]
+                        pam_found = search_seq[i:guide_start]
                         extended_guide = str(search_seq[i - 5:i + sitelen + 4])
+                        snvpos = snv_rel_pos - (i + pamlen + cut_site_position)
+                        if snvpos >= 0:
+                            snvpos += 1
                         if 'Cas12a' in name:
-                            scores['deepcpf1'] = round(scoring.deepcpf1([extended_guide],
+                            scores['deepcpf1'] = round(scoring.deepcpf1([extended_guide.upper()],
                                                               self.models_dir)[0][0], 2)
+                    start_diff = target_start -snv_rel_pos
 
-                    snvpos = snv_rel_pos - target_start
-                    start = self.SNV_chr_pos - snvpos
+                    if search_strand == '-':
+                        start_diff = snv_rel_pos - (target_start + sitelen)
+                    start = self.SNV_chr_pos + start_diff
                     end = start + sitelen
-
-                    guides.append([name, guide, pam_found, search_strand, snvpos, scores,extended_guide, start, end])
-
+                    
+                    #print(pam_min,pam_max,name,i,snvpos, extended_guide)
+                    guides.append([name, guide, pam_found, search_strand, int(snvpos), scores,extended_guide, start, end])
                     if not BEmode:
-                        self.add_guides(name, guide, pam_found, search_strand, snvpos, scores ,extended_guide, start, end)
+                        self.add_guides(name, guide, pam_found, search_strand, int(snvpos), scores ,extended_guide, start, end)
         return guides
 
     def get_Guides(self, search_params, BEsearch_params=None):
         for name, params, in search_params.items():
-            pam, pamISfirst, guidelen, dsb_loc = params[0:4]
-            win_size = [int(dsb_loc)-self.dist_from_cutsite, int(dsb_loc)+self.dist_from_cutsite]
-            guides = self.get_guide_set(name, pam, pamISfirst,win_size, guidelen, BEmode=False)
+            pam, pamISfirst, guidelen, cut_site_position = params[0:4]
+            win_size = [int(cut_site_position) - self.dist_from_cutsite, int(cut_site_position) + self.dist_from_cutsite]
+            guides = self.get_guide_set(name, pam, pamISfirst, win_size, guidelen,cut_site_position, BEmode=False)
 
         # if BE mode is on
         if BEsearch_params is not None and len(self.NC_ref_allele + self.NC_alt_allele) ==2:
             for k, params, in BEsearch_params.items():
                 pam, pamISfirst, guidelen, win_size = params[0][0], params[0][1], params[0][2], params[0][3]
-                bguides = self.get_guide_set(k, pam, pamISfirst, win_size, guidelen, BEmode=True)
+                bguides = self.get_guide_set(k, pam, pamISfirst, win_size, guidelen,cut_site_position=100, BEmode=True)
 
                 # if guides are found sep neg and pos strand guides
                 if len(bguides) > 0:
                     pos_guides, neg_guides = [], []
                     for g in bguides:
                         if g[3] == '+':
                             pos_guides += [g]
```

### Comparing `meditability-0.2.2/src/smk/pipelines/py/deepcas_models.py` & `meditability-0.2.3a0/src/smk/pipelines/py/deepcas_models.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.2/src/smk/pipelines/py/fasta_chromosome_rename.py` & `meditability-0.2.3a0/src/smk/pipelines/py/fasta_chromosome_rename.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,25 +5,35 @@
 # == Installed Modules
 from Bio import SeqIO
 # == Project Modules
 
 
 def main():
 	INPUT_FASTA = sys.argv[1]
+	OUTPUT_FASTA = sys.argv[2]
+
+	# INPUT_CHROMOSOME = "/home/ubuntu/genomes/toy_genome.fna"
 
 	record = SeqIO.parse(open(INPUT_FASTA), "fasta")
 	changed_recs = []
 	for rec in record:
-		a = re.search(r"Homo sapiens chromosome (\d+), \S+ Primary Assembly", rec.description)
+		a = re.search(r"Homo sapiens chromosome (\w+), GRCh38 reference primary assembly", rec.description)
 		try:
 			rec.id = f"chr{a.group(1)}"
 			rec.name = f"chr{a.group(1)}"
 			rec.description = ""
 		except AttributeError:
-			pass
+			a = re.search(r"Homo sapiens (m)itochondrion", rec.description)
+			try:
+				mit_id = a.group(1)
+				rec.id = f"chrMT"
+				rec.name = f"chrMT"
+				rec.description = ""
+			except AttributeError:
+				continue
 		changed_recs.append(rec)
 
-		SeqIO.write(changed_recs, INPUT_FASTA, 'fasta')
+	SeqIO.write(changed_recs, OUTPUT_FASTA, 'fasta')
 
 
 if __name__ == "__main__":
 	main()
```

### Comparing `meditability-0.2.2/src/smk/pipelines/py/featurization.py` & `meditability-0.2.3a0/src/smk/pipelines/py/featurization.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.2/src/smk/pipelines/py/fetchGuides.py` & `meditability-0.2.3a0/src/smk/pipelines/py/fetchGuides.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 # Native Modules
 # import gzip
 # import zlib
 import pickle
 import os
 import re
+from copy import deepcopy
 # from zlib import error
 # Installed Modules
 import pandas as pd
-# from Bio import SeqIO, SeqUtils
 from Bio.Seq import Seq
 # Project Modules
 from dataH import DataHandler
 from annotate import Transcript
 
 
 ###############
 # Main Script with Fetch_Guides Class for running pipeline
 ###############
-
-
 def set_export(outdir):
 	# Create outdir if inexistent
 	if not os.path.exists(outdir):
 		os.makedirs(outdir)
 	return outdir
 
 
@@ -88,54 +86,61 @@
 		self.BE_choices = list(base_editors.keys())
 
 		## ------------Defaults and settings------------------##
 		##configure editor options
 		self.search_params = self.configure_search_params()
 
 		# configure BE options
+		self.BE_search_params = {}
 		if self.be_request != 'off':
 			self.BE_search_params = self.set_BE_params()
 
+
 		# ---------------Ouputs--------------------------#
 		self.all_variant = pd.DataFrame()
 		self.all_gene = pd.DataFrame()
 		self.all_guides = {}
 		self.all_BE = {}
 		self.not_found = {}
 
 	def configure_search_params(self):
 		"""
 		set paramteres for the selected editor or editors(not BE editors)
 		"""
+		search_params = {}
 		# search for all guides
 		if self.editor_request == 'clinical':
 			search_params = self.editor_lib['clinical']
 		# set custom editor params
 		elif self.editor_request == 'custom':
 			search_params = self.set_params(self.kwargs)
 
 		# search for selected subset
 		# TODO: The guide_prediction.py needs to ingest this correctly
-		elif type(self.editor_request) is list:
-			search_params = {}
+		elif len(self.editor_request.split(',')) >= 1:
+			user_request_editors = deepcopy(self.editor_lib['user_request'])
+			self.editor_request = list(self.editor_request.split(','))
 			for editor in self.editor_request:
 				try:
-					search_params[editor] = self.editor_lib['user_request'][editor]
-				except KeyError:
-					print(f"Please list one or more editors available at the current version's list:"
-						  f" \n{self.editor_lib['user_request'].keys()}")
-					raise Exception(f"The editor {editor} isn't available in the currently version of mEdit")
-
+					search_params.setdefault(editor, user_request_editors[editor])
+				except KeyError as e:
+					print(f"\n*********************************\n"
+						  f"The entry {editor} is not part of the built-in list of editing tools.\n"
+						  f"Please list one or more editors available at the current version's list.\n"
+						   f"For more information consult 'medit list --help'\n "
+						  f"*********************************\n")
+				else:
+					continue
 		# else use single set parameters
 		else:
-			if self.editor_request in self.editor_choices:
+			try:
 				search_params = {self.editor_request: self.editor_lib[self.editor_request]}
-
-			else:
-				print('Please choose a name(s) found in the editor name choices')
+			except KeyError:
+				raise Exception("Please choose a name(s) found in the editor name choices. "
+					   "For more information consult 'medit list --help")
 
 		print(f'Editor(s) set to: {[x for x in search_params.keys()]}')
 		return search_params
 
 	def set_params(self, kwargs):
 		name = 'custom'
 
@@ -192,14 +197,20 @@
 
 	def write_gsearch_params(self, outfile):
 		# writes pickle of selected guide search params for later use in process_genome
 		# 'editor', 'pam', '5prime_pam','guide_length', 'DSB site', 'notes'
 		with open(outfile, 'ab') as gfile:
 			pickle.dump(self.search_params, gfile)
 
+	def write_gsearch_params(self, outfile):
+		# writes pickle of selected guide search params for later use in process_genome
+		# 'editor', 'pam', '5prime_pam','guide_length', 'DSB site', 'notes'
+		with open(outfile, 'ab') as gfile:
+			pickle.dump(self.BE_search_params, gfile)
+
 	def write_snv_site_info(self, outfile):
 		'''
 		#writes pickle of SNV site info for later use in process genome
 		#query, tid, eid, strand, ref, alt, feature_annotation, extracted_seq, codons, coord
 		'''
 		with open(outfile, 'ab') as sfile:
 			pickle.dump(self.snv_info, sfile)
@@ -258,39 +269,35 @@
 		for nf in nfqueries:
 			self.not_found[nf] = reason
 
 	@staticmethod
 	def extract_seqs(searchseq, pos, ref, alt, window):
 		# extracts the sequence +/windowbp surrounding a SNV then swaps ref for alt allele
 
+		alt = alt.lower()
+		searchseq = searchseq.upper()
+
 		if len(ref) == len(alt):  ##substitution
 			extracted_seq = str(searchseq[pos - window:pos + window])
-			variant_seq = (extracted_seq[0:window] + alt + extracted_seq[window + len(alt):]).upper()
+			variant_seq = (extracted_seq[0:window] + alt + extracted_seq[window + len(alt):])#.upper()
 
 
 		elif len(ref) > len(alt):  # deletion
-			diff= len(ref) - len(alt)
+			diff = len(ref) - len(alt)
 			extracted_seq = str(searchseq[pos - window:(pos + window + diff)])
-			variant_seq = (extracted_seq[0:window] + alt+ extracted_seq[window+len(ref):]).upper()
+			variant_seq = (extracted_seq[0:window] + alt + extracted_seq[window + len(ref):])#.upper()
 
 		elif len(ref) < len(alt):  # insertion
 			extracted_seq = str(searchseq[pos - window:pos + window - (len(alt))])
-			variant_seq = (extracted_seq[0:window] + alt + extracted_seq[window:]).upper()
+			variant_seq = (extracted_seq[0:window] + alt + extracted_seq[window:])#.upper()
 		# print(new_seq)
 
 		else:
 			print('VARIANT REF AND ALT DO NOT COMPLY')
-			print(ref,alt,pos)
-		#if len(variant_seq) != 2* self.window:
-		#	print('SEQUENCE LENGTH less than 100')
-		#	print('REF', ref)
-		#	print('ALT', alt)
-		#	print('t_pos', pos)
-
-
+			print(ref, alt, pos)
 		return variant_seq
 
 	def get_chroms(self, queries):
 		# finds unique chromosome for each hgvs
 		# needs to happen in order to select right fasta file
 		hgvs_tab = pd.read_csv(self.HGVSlookup_path)
 		q_prefixes = [x.split(':')[0] for x in queries]
@@ -306,15 +313,15 @@
 			chroms = self.get_chroms(self.queries)
 
 			for ch in chroms:
 				df = pd.read_csv(f"{self.processed_tables}/variant_tables/{ch}_variant.txt", low_memory=False)
 				gadf = df.loc[df['HGVS_Simple'].isin(self.queries)]
 				self.add_clinvar(gadf)
 				self.snv_info[ch] = \
-				gadf[['HGVS_Simple', 'PositionVCF', 'RefAlleleVCF', 'AltAlleleVCF']].to_dict('tight')['data']
+					gadf[['HGVS_Simple', 'PositionVCF', 'RefAlleleVCF', 'AltAlleleVCF']].to_dict('tight')['data']
 			found = []
 			for k in self.snv_info.keys():
 				for v in self.snv_info[k]:
 					found.append(v[0])
 			notfound = list(set(self.queries).difference(set(found)))
 			self.add_not_found(notfound, 'hgvs not found in medit variant database')
 
@@ -333,20 +340,27 @@
 	def find_transcript_info(self):
 
 		print("Gathering Variant Genomic Info from RefSeq file.......")
 
 		for ch, data in self.snv_info.items():  # find transcript info
 			new_data = []
 			snvcoords = [f'chr{ch}:{d[1]}-{d[1]}' for d in data]
-			Transcript.load_transcripts(self.annote_path, snvcoords)
+			try:
+				Transcript.load_transcripts(self.annote_path, snvcoords)
+			except IndexError:
+				# TODO: Something on commit f6f4b19 has changed the communication between fetchGuides and annotate.py
+				# TODO: @ACTG802 --> please advise on whether this needs fixing or just a bypass message would be enough
+				print(f"WARNING: function 'load_transcripts' from annotate.py got the wrong number of indices from snvcoords")
+				print(f"This is how it looks like: {snvcoords}")
+				continue
 
 			# === Transitioning SeqIO.read to direct import of Pickled SeqRecord Objects ===
 			chr_fasta_path = f"{self.fasta_path}/chr{str(ch)}.pkl"
 			try:
-				print(f"Finding transcripts information: Assessing {chr_fasta_path}")
+				print(f"Finding transcripts information on chromosome chr{str(ch)}")
 				with open(chr_fasta_path, 'rb') as pfile:
 					fasta = pickle.load(pfile)
 			except FileNotFoundError:
 				print(
 					f"The file {chr_fasta_path} was not found. Please regenerate background data and check the target directory")
 				continue
 			except pickle.UnpicklingError:
@@ -469,15 +483,15 @@
 					if len(self.all_guides.keys()) == 0:
 						for k, v in guides.items():
 							self.all_guides[k] = v
 					else:
 						for k, v in guides.items():
 							self.all_guides[k] += v
 
-						print(len((guides['gRNA'])), ' guides found for ', query)
+					print(len((guides['gRNA'])), ' guides found for ', query)
 				else:
 					print(f"No guides found for the query {query}")
 					self.add_not_found([query], 'no guides found')
 
 		guidedf, BEdf = None, None
 
 		if len(self.all_guides.keys()) != 0:
```

### Comparing `meditability-0.2.2/src/smk/pipelines/py/find_offtargets.py` & `meditability-0.2.3a0/src/smk/pipelines/py/find_offtargets.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     # INPUT LEG
     fnhead = input_filename.replace("_input.txt", "")
     id_dict = {}
     if bulge == True:
         with open(input_filename) as f:
             chrom_path = f.readline()
             pattern, bulge_dna, bulge_rna = f.readline().strip().split()
-            isreversed = False
+            isreversed = False ## PAM 5 or 3 prime
             for i in range(int(len(pattern) / 2)):
                 if pattern[i] == 'N' and pattern[len(pattern) - i - 1] != 'N':
                     isreversed = False
                     break
                 elif pattern[i] != 'N' and pattern[len(pattern) - i - 1] == 'N':
                     isreversed = True
                     break
@@ -102,32 +102,34 @@
                             bg_tgts[bg_tgt].add(mismatch)
                             id_dict[bg_tgt] = gid
 
                     for bulge_size in range(1, bulge_rna+1):
                         for i in range(1, len(target)-bulge_size):
                             bg_tgt = 'N' * (bulge_dna + bulge_size) + target[:i] + target[i+bulge_size:] + 'N' * len_pam
                             bg_tgts[bg_tgt].add(mismatch)
-                            rnabulge_dic[bg_tgt].append( (i, int(mismatch), target[i:i+bulge_size]) )
+                            rnabulge_dic[bg_tgt].append((i, int(mismatch), target[i:i+bulge_size]))
                             id_dict[bg_tgt] = gid
             if isreversed:
                 seq_pam = pattern[:len_pam]
             else:
                 seq_pam = pattern[-len_pam:]
+
         with open(fnhead + '_bulge.txt', 'w') as f:
             f.write(chrom_path)
             if isreversed:
                 f.write(pattern + bulge_dna*'N' + '\n')
             else:
                 f.write(bulge_dna*'N' + pattern + '\n')
             cnt = 0
             for tgt, mismatch in bg_tgts.items():
                 f.write(tgt + ' ' + str(max(mismatch)) + ' ' + '\n')
                 cnt+=1
         # THIS FILE PATH IS SUPPLIED TO CASOFF-FINDER
         casin = fnhead + '_bulge.txt'
+
     else:
         nobulge_dict = {}
         with open(input_filename) as inf:
             for line in inf:
                 entry = line.strip().split(' ')
                 if len(entry) > 2 and len(entry[-1]) > 3:
                     seq, mm, gid = entry
@@ -135,15 +137,14 @@
         casin = input_filename
 
     print("Created temporary file (%s)." % (casin))
     # THIS FILE PATH IS SUPPLIED TO CASOFF-FINDER
     outfn = fnhead + '_temp.txt'
     print("Running Cas-OFFinder (output file: %s)..." % outfn)
 
-
     p = Popen([cas_off_expath, casin, 'C', outfn])
     ret = p.wait()
     if ret != 0:
         print("Cas-OFFinder process was interrupted!")
         exit(ret)
     print("Processing output file...")
 
@@ -152,25 +153,25 @@
         fo.write('Coordinates\tDirection\tGuide_ID\tBulge type\tcrRNA\tDNA\tMismatches\tBulge Size\n')\
         #fo.write('Guide_ID\tBulge type\tcrRNA\tDNA\tChromosome\tPosition\tDirection\tMismatches\tBulge Size\n')
         ot_coords = []
         for line in fi:
             entries = line.strip().split('\t')
             ncnt = 0
 
-
             if bulge == False:
                 gid, mm = nobulge_dict[entries[0]]
                 coord = f'{entries[1]}:{entries[2]}-{int(entries[2]) + len(entries[0])}'
                 fo.write(f'{coord}\t{entries[4]}\t{gid}\tX\t{entries[0]}\t{entries[3]}\t{entries[5]}\t0\n')
                 ot_coords.append(coord)
             else:
                 if isreversed:
                     for c in entries[0][::-1]:
                         if c == 'N':
                             ncnt += 1
+                        else:
                             break
                     if ncnt == 0:
                         ncnt = -len(entries[0])
                 else:
                     for c in entries[0]:
                         if c == 'N':
                             ncnt += 1
@@ -214,46 +215,45 @@
                     ot_coords.append(coord)
                     fo.write(f'{entries[1]}:{start}-{start + len(tgt[1])}\t{entries[4]}\t{gid}\t{btype}\t{tgt[0]}\t{tgt[1]}\t{int(entries[5])}\t{nbulge}\n')
         remove(fnhead + '_temp.txt')
         remove(casin)
         editor = gid.split('_')[0]
         print(f'{len(ot_coords)} off targets found for {editor}')
 
-def score_ot(crrna,otseq,editor):
-    score = '.'
-    if 'spCas9' in editor:
-        # TODO: NEEDS
-        raise Exception("The function scoring.cfd_score requires a path to the model files")
-        score = scoring.cfd_score(crrna[:-3], otseq[:-4])
+def score_ot(crrna,otseq,models_dir):
+    score = 0
+    if '-' not in crrna[:-3]:
+        if '-' not in otseq[:-4]:
+            # TODO: NEEDS
+            #raise Exception("The function scoring.cfd_score requires a path to the model files")
+            score = scoring.cfd_score(crrna[:-3].upper(), otseq.upper(),models_dir)
     return score
 
 
-
-def annotate_ots(output_filename,annote_path):
+def annotate_ots(output_filename,annote_path,models_dir):
     '''
     Reads output, Scores each off-target seq and annotates each off_target
     '''
-    #annote_path = "/groups/clinical/projects/editability/tables/processed_tables/ncbiRefSeq.bed.gz"
-    #output_filename = '/groups/clinical/projects/editability/medit_queries/medit_test/test_out/hg38_hg38_spCas9_casoffinder_output.txt'
+
     editor = output_filename.split('_casoff')[0].split('_')[-1]
     coords = []
     scores = []
     spec_scores = {}
     res = open(output_filename, 'r').readlines()
     for line in res[1:]:
         line = line.strip().split('\t')
         coords.append(line[0])
         if line[2] not in spec_scores.keys():
-            spec_scores[line[2]] = 0
-        score = score_ot(line[4], line[5],editor)
-        if score != '.':
-            if score != 1:
+            spec_scores[line[2]] = 0 if editor == 'spCas9' else '.'
+        if editor == 'spCas9':
+            score = score_ot(line[4], line[5],models_dir)
+            if score > 0 and score != 1:
                 spec_scores[line[2]] = spec_scores[line[2]] + score
         else:
-            spec_scores[line[2]] = '.'
+            score = '.'
         scores.append(score)
 
     Transcript.load_transcripts(annote_path,coords)
 
     new_lines = []
     annotate_out = output_filename.replace('_output', '_annotated')
     with open(annotate_out, 'w') as anout:
@@ -275,15 +275,18 @@
                 new_line = line + [x, str(scores[cnt])]
                 new_lines.append(new_line)
             cnt += 1
             anout.write('\t'.join(new_line) + '\n')
 
     if editor == 'spCas9':
         for gid, sum_score in spec_scores.items():
-            spec_scores[gid] = scoring.cfd_spec_score(sum_score)
+            if sum_score!= 0:
+                spec_scores[gid] = scoring.cfd_spec_score(sum_score)
+        else:
+            spec_scores[gid] = "."
     #remove(output_filename)
     return new_lines, spec_scores
 
 
 def agg_results(lines,mmco):
     '''
     sums the number of off-targets for each guide
@@ -312,27 +315,26 @@
         gdf = gdf.drop(columns='Num Off Targets per MM')
     if 'Off Target Score' in gdf.columns:
         gdf = gdf.drop(columns='Off Target Score')
 
     # Update main guides table with specifity Scoress
     spec_scores = df.T.sort_index()['spec_score']
     df =df.drop(index = 'spec_score')
-
+    df = df.astype('int')
     #Add off_targets summary
     df.index = pd.MultiIndex.from_tuples(list(df.index), names=['BulgeType', 'Number of Mismatches'])
     df = df.reset_index()
     ot_per_mm = df.loc[df['BulgeType']=='X']
     ot_per_mm= ot_per_mm.iloc[:, 2:].T.sort_index()
     ot_per_mm=ot_per_mm.stack().astype('str').groupby(level=0).apply('|'.join)
     ot_per_mm=ot_per_mm.rename('Guide_ID')#('Num Off Targets per Mismatch')
     gdf = gdf.sort_values('Guide_ID')
     gdf['Off Target Score'] = list(spec_scores)
     gdf['Num Off Targets per MM'] = list(ot_per_mm)
 
-
     # create off_target summary of totals
     if casoff_params[1] == 0:
         df = df.loc[df.BulgeType != 'RNA']
     if casoff_params[2] == 0:
         df = df.loc[df.BulgeType != 'DNA']
     offtarget_summary_report = df.pivot_table(columns=['BulgeType', 'Number of Mismatches'], aggfunc="sum")
 
@@ -347,42 +349,55 @@
                     fasta_fname,
                     guide_tab_fname,
                     search_params,
                     cas_off_expath,
                     genome_name,
                     guide_src_name,
                     casoff_params,
-                    annote_path):
-    #guide_tab_fname = '/groups/clinical/projects/editability/medit_queries/medit_test/test_out/hg38_Guides_found.csv'
+                    annote_path,
+                    models_dir):
+    #guide_tab_fname = '/groups/clinical/projects/editability/medit_queries/medit_showcase/out/hg38_Guides_found.csv'
     gdf = pd.read_csv(guide_tab_fname)
+    #gdf = gdf.iloc[0,:]
     ots = {}
     gpr = gdf.groupby('Editor')
     if casoff_params[1:3] == (0, 0):
         bulge = False
     else:
         bulge = True
     # for each editor type find off_targets
     for editor, stats in gpr:
-        infile = f"{resultsfolder}{genome_name}_{guide_src_name}_{editor}_casoffinder_input.txt"
-        pam, pamISfirst, guidelen = search_params[editor][0:3]
+
+        try:
+            pam, pamISfirst, guidelen = search_params[editor][0:3]
+        except:
+            # BE search params
+            pam, pamISfirst, guidelen = search_params[editor][0][0:3]
+
         guides, gnames = list(stats.gRNA), list(stats.Guide_ID)
+        guides =[g.upper() for g in guides]
+
         # make input file
+        infile = f"{resultsfolder}{genome_name}_{editor}_casoffinder_input.txt"
+
+
         make_casoffinder_input(infile,
                                fasta_fname,
                                pam,
                                pamISfirst,
                                guidelen,
                                guides,
                                gnames,
                                casoff_params)
 
         output_filename = infile.replace('_input.txt', '_output.txt')
+
         cas_offinder_bulge(infile, output_filename, cas_off_expath, bulge)
 
-        new_lines, spec_scores = annotate_ots(output_filename,annote_path)
+        new_lines, spec_scores = annotate_ots(output_filename,annote_path,models_dir)
 
         ot_dict = agg_results(new_lines,casoff_params[0])#sum off-targets
         for k, v in ot_dict.items():
             v['spec_score'] = spec_scores[k]
             ots[k] = v
     write_out_res(ots, gdf, casoff_params, resultsfolder, guide_tab_fname)
 
@@ -426,47 +441,50 @@
 
     #resultsfolder = "/groups/clinical/projects/editability/medit_queries/medit_test/test_out/"
 
     paths = listdir(resultsfolder)
 
     # Guide search params
     search_params = pickle.load(open(guide_search_params, 'rb'))
-    # search_params = pickle.load(open(resultsfolder + "guide_search_params.pkl", 'rb'))
 
     # hg38 or consensus sequence
     fasta_fname = fasta_ref
     genome_name = fastaref_name
     # fasta_fname = '/groups/clinical/projects/clinical_shared_data/hg38/hg38.fa'
     # genome_name = 'hg38'
 
     # hg38 guides found (but could be {alt_genome}_differences.csv
     guide_tab_fname = guides_report
     guides_src_name = guideref_name
-    # guide_tab_fname = resultsfolder + 'Guides_found.csv'
     # guide_src_name = 'hg38'
 
     ### Daniel---> Pycharm is not find subprocess.Popen(casoffinder...) without an absolute path. so I'm adding this
     # but I don't think its needed in the final version
     cas_off_expath = '/home/thudson/miniconda3/envs/edit/bin/cas-offinder'
 
     # defaults - we may allow users to change these cas-offinder settings?
     # according to Gorodkin et al. and Lin et al.  DNA bulges are even more tolerated than mismatches alone
     # https://www.nature.com/articles/s41467-022-30515-0
-    # RNAbb = 0  # RNA bulge, a deletion in the off-target
+    # RNAbb = 1  # RNA bulge, a deletion in the off-target
     # DNAbb = 1  # DNA bulge, an insertion in the off-target
-    # mm = 3  # max allowable mismatch
+    # mm = 4  # max allowable mismatch
     # PU = 'C'  # G = GPU C = CPU A = Accelerators -- I don't really know which should be default?
-    #casoff_params = (3, 0, 0, "C")
-    casoff_params = (mm, RNAbb, DNAbb, PU)
+
+    # guide_tab_fname = gout
+    #search_params = pickle.load(open(resultsfolder + "guide_search_params.pkl", 'rb'))
+    # mm, RNAbb, DNAbb, PU = 6,2,2,"C"
+    # models_dir = '/home/thudson/projects/editability/src/pkl/models/'
 
     run_casoffinder(resultsfolder,
                     fasta_fname,
                     guide_tab_fname,
                     search_params,
                     cas_off_expath,
                     genome_name,
-                    guides_src_name,
-                    casoff_params)
+                    guide_src_name,
+                    casoff_params,
+                    annote_path,
+                    models_dir)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `meditability-0.2.2/src/smk/pipelines/py/gdrive_import.py` & `meditability-0.2.3a0/src/smk/pipelines/py/gdrive_import.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.2/src/smk/pipelines/py/genome_seq_search.py` & `meditability-0.2.3a0/src/smk/pipelines/py/genome_seq_search.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.2/src/smk/pipelines/py/make_tables.py` & `meditability-0.2.3a0/src/smk/pipelines/py/make_tables.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.2/src/smk/pipelines/py/ncbi_cross_database.py` & `meditability-0.2.3a0/src/smk/pipelines/py/ncbi_cross_database.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.2/src/smk/pipelines/py/process_genome.py` & `meditability-0.2.3a0/src/smk/pipelines/py/process_genome.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.2/src/smk/pipelines/py/scoring.py` & `meditability-0.2.3a0/src/smk/pipelines/py/scoring.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Native Modules
 from math import exp
 import pickle
 import re
+import os
+import os
+os.environ['TF_CPP_MIN_LOG_LEVEL'] = '1'
 # Installed Modules
 import pandas as pd
 import numpy as np
 import tensorflow.compat.v1 as tf1
 from tensorflow.keras.models import load_model
 # Project Modules
 from featurization import featurize_data
@@ -64,21 +67,14 @@
             elif data[l][i] in "Tt":
                 DATA_X[l, 0, i, 3] = 1
             else:
                 pass
     return DATA_X
 
 
-##########
-##
-##                   DANIEL MAKE TENSORFLOR STOP YELLING AT ME!!!!
-##   it's giving me some warning about keras conv. layers but still runs
-##
-##########
-
 def deepspcas9(cas9_sites, models_dir):
     '''
     Hui Kwon Kim et al. ,SpCas9 activity prediction by DeepSpCas9,
     a deep learning–based model with high generalization performance.Sci. Adv.5,eaax9249(2019).
     predicts the likelihood of getting a spCas9 indel at the desired target
     This script is copied and modified from https://github.com/MyungjaeSong/Paired-Library
     '''
@@ -364,22 +360,21 @@
 pam = 'AGG'
 spacer = 'GTGCGGCTGGCCCAGGACCT'
 target = spacer + pam
 target30mer = 'CTTGTGCGGCTGGCCCAGGACCTAGGCGAG'
 target60mer = 'ATCTCTTACAACGACTTCTTGTGCGGCTGGCCCAGGACCTAGGCGAGGCAGTAGGGGATGACA'
 off_target_seqs = ['GTGGGGCTGACCCAGGACCTGAG','GGGCCTCTGGCCCAGGACCTGGG']
 
-
 print('Microhomology Out-Of-Frame score: ',oofscore(seq = target60mer))
 # Ans: 3730.1, 64.2
 
 print('Azimuth on-target score: ',azimuth([target30mer])[0])
 #Ans: 0.38
 
-print('CFD score ',cfd_score(spacer, off_target_seqs[1]))
+print('CFD score ',cfd_score(spacer, off_target_seqs[1],models_dir = models_dir))
 print('CFD score ',cfd_score(spacer, off_target_seqs[0]))
 #0.44, 0.12
 
 print('CFD spec score ',cfd_spec_score(sum([0.44,0.12])))
 #99
 
 seq1, seq2 = 'GTGCGGCTGGCCCAGGACC-T', 'GTGCtGCTacCCCAGGACCCTCGG'
```

### Comparing `meditability-0.2.2/src/smk/pipelines/py/validate.py` & `meditability-0.2.3a0/src/smk/pipelines/py/validate.py`

 * *Files identical despite different names*

### Comparing `meditability-0.2.2/src/smk/pipelines/vcf_processing.smk` & `meditability-0.2.3a0/src/smk/pipelines/vcf_processing.smk`

 * *Files identical despite different names*

