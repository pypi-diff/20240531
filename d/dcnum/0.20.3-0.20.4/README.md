# Comparing `tmp/dcnum-0.20.3.tar.gz` & `tmp/dcnum-0.20.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcnum-0.20.3.tar", last modified: Wed May 29 18:23:26 2024, max compression
+gzip compressed data, was "dcnum-0.20.4.tar", last modified: Fri May 31 08:57:40 2024, max compression
```

## Comparing `dcnum-0.20.3.tar` & `dcnum-0.20.4.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:23:26.924884 dcnum-0.20.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:23:26.900884 dcnum-0.20.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:23:26.904884 dcnum-0.20.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-29 18:23:20.000000 dcnum-0.20.3/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-29 18:23:20.000000 dcnum-0.20.3/.github/workflows/deploy_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-29 18:23:20.000000 dcnum-0.20.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-29 18:23:20.000000 dcnum-0.20.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    12597 2024-05-29 18:23:20.000000 dcnum-0.20.3/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-29 18:23:20.000000 dcnum-0.20.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-29 18:23:26.924884 dcnum-0.20.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-29 18:23:20.000000 dcnum-0.20.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:23:26.904884 dcnum-0.20.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-29 18:23:20.000000 dcnum-0.20.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:23:26.904884 dcnum-0.20.3/docs/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-29 18:23:20.000000 dcnum-0.20.3/docs/extensions/github_changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-29 18:23:20.000000 dcnum-0.20.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-29 18:23:20.000000 dcnum-0.20.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-29 18:23:20.000000 dcnum-0.20.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 18:23:26.924884 dcnum-0.20.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:23:26.900884 dcnum-0.20.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:23:26.904884 dcnum-0.20.3/src/dcnum/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-29 18:23:26.000000 dcnum-0.20.3/src/dcnum/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:23:26.908884 dcnum-0.20.3/src/dcnum/feat/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/feat/event_extractor_manager_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:23:26.908884 dcnum-0.20.3/src/dcnum/feat/feat_background/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/feat/feat_background/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/feat/feat_background/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/feat/feat_background/bg_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13175 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/feat/feat_background/bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (127)    20709 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/feat/feat_background/bg_sparse_median.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:23:26.908884 dcnum-0.20.3/src/dcnum/feat/feat_brightness/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/feat/feat_brightness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/feat/feat_brightness/bright_all.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/feat/feat_brightness/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:23:26.908884 dcnum-0.20.3/src/dcnum/feat/feat_contour/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/feat/feat_contour/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/feat/feat_contour/contour.py
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/feat/feat_contour/moments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/feat/feat_contour/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:23:26.908884 dcnum-0.20.3/src/dcnum/feat/feat_texture/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/feat/feat_texture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/feat/feat_texture/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/feat/feat_texture/tex_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/feat/gate.py
--rw-r--r--   0 runner    (1001) docker     (127)    15644 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/feat/queue_event_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:23:26.912884 dcnum-0.20.3/src/dcnum/logic/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34411 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/logic/ctrl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/logic/job.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/logic/json_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:23:26.912884 dcnum-0.20.3/src/dcnum/meta/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/meta/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/meta/ppid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:23:26.912884 dcnum-0.20.3/src/dcnum/read/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/read/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/read/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    23489 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/read/hdf5_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/read/mapped.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:23:26.912884 dcnum-0.20.3/src/dcnum/segm/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/segm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/segm/segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (127)    12220 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/segm/segmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10690 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/segm/segmenter_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/segm/segmenter_gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/segm/segmenter_manager_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:23:26.912884 dcnum-0.20.3/src/dcnum/write/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/write/deque_writer_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/write/queue_collector_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)    15601 2024-05-29 18:23:20.000000 dcnum-0.20.3/src/dcnum/write/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:23:26.924884 dcnum-0.20.3/src/dcnum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-29 18:23:26.000000 dcnum-0.20.3/src/dcnum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-29 18:23:26.000000 dcnum-0.20.3/src/dcnum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:23:26.000000 dcnum-0.20.3/src/dcnum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-29 18:23:26.000000 dcnum-0.20.3/src/dcnum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 18:23:26.000000 dcnum-0.20.3/src/dcnum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:23:26.920884 dcnum-0.20.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:23:26.924884 dcnum-0.20.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/data/fmt-hdf5_cytoshot_extended-moments-features.zip
--rw-r--r--   0 runner    (1001) docker     (127)   650653 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
--rw-r--r--   0 runner    (1001) docker     (127)   284743 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/data/fmt-hdf5_cytoshot_full-features_2024.zip
--rw-r--r--   0 runner    (1001) docker     (127)   154010 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/data/fmt-hdf5_shapein_empty.zip
--rw-r--r--   0 runner    (1001) docker     (127)   275920 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/data/fmt-hdf5_shapein_raw-with-variable-length-logs.zip
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/helper_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_feat_background_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_feat_background_bg_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_feat_background_bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_feat_background_bg_sparsemed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_feat_brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_feat_event_extractor_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_feat_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_feat_haralick.py
--rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_feat_moments_based.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_feat_moments_based_extended.py
--rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_feat_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_logic_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_logic_join.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_logic_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    37009 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_logic_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_meta_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_meta_ppid_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_meta_ppid_bg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_meta_ppid_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_meta_ppid_feat.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_meta_ppid_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_meta_ppid_segm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_read_basin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_read_concat_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)    11771 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_read_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)    11056 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_read_hdf5_basins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_read_hdf5_index_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    14336 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_segm_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_segm_no_mask_proc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_write_deque_writer_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_write_queue_collector_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-05-29 18:23:20.000000 dcnum-0.20.3/tests/test_write_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.760693 dcnum-0.20.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.740693 dcnum-0.20.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.744693 dcnum-0.20.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-31 08:57:35.000000 dcnum-0.20.4/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-31 08:57:35.000000 dcnum-0.20.4/.github/workflows/deploy_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-31 08:57:35.000000 dcnum-0.20.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-31 08:57:35.000000 dcnum-0.20.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    12928 2024-05-31 08:57:35.000000 dcnum-0.20.4/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-31 08:57:35.000000 dcnum-0.20.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-31 08:57:40.760693 dcnum-0.20.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-31 08:57:35.000000 dcnum-0.20.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.744693 dcnum-0.20.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-31 08:57:35.000000 dcnum-0.20.4/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.744693 dcnum-0.20.4/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-31 08:57:35.000000 dcnum-0.20.4/docs/extensions/github_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-31 08:57:35.000000 dcnum-0.20.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-31 08:57:35.000000 dcnum-0.20.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-31 08:57:35.000000 dcnum-0.20.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 08:57:40.760693 dcnum-0.20.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.740693 dcnum-0.20.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.744693 dcnum-0.20.4/src/dcnum/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-31 08:57:40.000000 dcnum-0.20.4/src/dcnum/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.744693 dcnum-0.20.4/src/dcnum/feat/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/event_extractor_manager_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.748693 dcnum-0.20.4/src/dcnum/feat/feat_background/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/feat_background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/feat_background/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/feat_background/bg_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13175 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/feat_background/bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20709 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/feat_background/bg_sparse_median.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.748693 dcnum-0.20.4/src/dcnum/feat/feat_brightness/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/feat_brightness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/feat_brightness/bright_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/feat_brightness/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.748693 dcnum-0.20.4/src/dcnum/feat/feat_contour/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/feat_contour/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/feat_contour/contour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/feat_contour/moments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/feat_contour/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.748693 dcnum-0.20.4/src/dcnum/feat/feat_texture/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/feat_texture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/feat_texture/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/feat_texture/tex_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15700 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/feat/queue_event_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.748693 dcnum-0.20.4/src/dcnum/logic/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34792 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/logic/ctrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/logic/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/logic/json_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.748693 dcnum-0.20.4/src/dcnum/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/meta/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/meta/ppid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.748693 dcnum-0.20.4/src/dcnum/read/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/read/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/read/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23489 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/read/hdf5_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/read/mapped.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.752693 dcnum-0.20.4/src/dcnum/segm/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/segm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/segm/segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/segm/segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/segm/segmenter_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/segm/segmenter_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/segm/segmenter_manager_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.752693 dcnum-0.20.4/src/dcnum/write/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/write/deque_writer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/write/queue_collector_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15601 2024-05-31 08:57:35.000000 dcnum-0.20.4/src/dcnum/write/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.760693 dcnum-0.20.4/src/dcnum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-31 08:57:40.000000 dcnum-0.20.4/src/dcnum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-31 08:57:40.000000 dcnum-0.20.4/src/dcnum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 08:57:40.000000 dcnum-0.20.4/src/dcnum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-31 08:57:40.000000 dcnum-0.20.4/src/dcnum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-31 08:57:40.000000 dcnum-0.20.4/src/dcnum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.756693 dcnum-0.20.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:57:40.760693 dcnum-0.20.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/data/fmt-hdf5_cytoshot_extended-moments-features.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   650653 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   284743 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/data/fmt-hdf5_cytoshot_full-features_2024.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   154010 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/data/fmt-hdf5_shapein_empty.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   275920 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/data/fmt-hdf5_shapein_raw-with-variable-length-logs.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_feat_background_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_feat_background_bg_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_feat_background_bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_feat_background_bg_sparsemed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_feat_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_feat_event_extractor_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_feat_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_feat_haralick.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_feat_moments_based.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_feat_moments_based_extended.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_feat_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_logic_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_logic_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_logic_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37009 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_logic_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_meta_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_meta_ppid_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_meta_ppid_bg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_meta_ppid_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_meta_ppid_feat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_meta_ppid_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_meta_ppid_segm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_read_basin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_read_concat_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11771 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_read_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11056 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_read_hdf5_basins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_read_hdf5_index_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14336 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_segm_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_segm_no_mask_proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_write_deque_writer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_write_queue_collector_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-05-31 08:57:35.000000 dcnum-0.20.4/tests/test_write_writer.py
```

### Comparing `dcnum-0.20.3/.github/workflows/check.yml` & `dcnum-0.20.4/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/.github/workflows/deploy_pypi.yml` & `dcnum-0.20.4/.github/workflows/deploy_pypi.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/.gitignore` & `dcnum-0.20.4/.gitignore`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/CHANGELOG` & `dcnum-0.20.4/CHANGELOG`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+0.20.4
+ - fix: slot_chunks were not performed in increasing order, making it
+   impossible for writer to continue writing and consequent OOM
+ - enh: reserve one CPU for writer thread and control logic
+ - enh: disentangle logging and debugging keyword arguments
+ - enh: do not initialize slot_chunks and slot_states with lock
 0.20.3
  - enh: improve strategy for stalling for slow writer
 0.20.2
  - ref: remove __init__ from SegmentThresh
 0.20.1
  - fix: relative basin locations not written correctly
  - enh: increase deque size threshold for waiting for writer
@@ -22,15 +28,15 @@
 0.18.0
  - BREAKING CHANGE: mask postprocessing did a morphological opening instead
    of a morphological closing, failing to remove spurious noise
  - BREAKING CHANGE: perform first fill_holes and then closing_disk in mask
    postprocessing
  - feat: allow to specify ranges when creating an HDF5Data instance to
    enable e.g. processing only a portion of an input file
- - feat: volume computation via contour revolve algorithm
+ - feat: volume computation via contour revolve algorithm (#23)
  - feat: background offset (flickering) correction via the
    "offset_correction" keyword for the "sparsemed" background computer
    and "bg_off" everywhere else
  - enh: allow creating HDF5Writer from h5py.File
  - fix: mask postprocessing did a morphological opening instead
    of a morphological closing, failing to remove spurious noise
  - fix: remove mask ppid part for segmenters that do not use it
```

### Comparing `dcnum-0.20.3/LICENSE` & `dcnum-0.20.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/PKG-INFO` & `dcnum-0.20.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.20.3
+Version: 0.20.4
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Maximilian Schlögel, Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.20.3/README.rst` & `dcnum-0.20.4/README.rst`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/docs/conf.py` & `dcnum-0.20.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/docs/extensions/github_changelog.py` & `dcnum-0.20.4/docs/extensions/github_changelog.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/pyproject.toml` & `dcnum-0.20.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/src/dcnum/feat/event_extractor_manager_thread.py` & `dcnum-0.20.4/src/dcnum/feat/event_extractor_manager_thread.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,16 +42,16 @@
             :func:`.EventExtractor.get_init_kwargs` for more information.
         num_workers:
             Number of child threads or worker processes to use.
         writer_dq:
             The queue the writer uses. We monitor this queue. If it
             fills up, we take a break.
         debug:
-            Whether to run in debugging mode which means more log
-            messages and only one thread (`num_workers` has no effect).
+            Whether to run in debugging mode which means only one
+            event extraction thread (`num_workers` has no effect).
         """
         super(EventExtractorManagerThread, self).__init__(
               name="EventExtractorManager", *args, **kwargs)
         self.logger = logging.getLogger(
             "dcnum.feat.EventExtractorManagerThread")
         #: Keyword arguments for class:`.EventExtractor`
         self.fe_kwargs = fe_kwargs
@@ -100,33 +100,40 @@
                 ldq2 = len(self.writer_dq)
                 stall_time = (ldq2 - 200) / (ldq - ldq2) if ldq2 > 200 else 0
                 time.sleep(stall_time)
                 self.logger.warning(
                     f"Stalled {stall_time + 1:.1f}s for slow writer "
                     f"({ldq} chunks queued)")
 
-            cur_slot = 0
             unavailable_slots = 0
+            found_free_slot = False
             # Check all slots for segmented labels
-            while True:
-                # - "e" there is data from the segmenter (the extractor
-                #   can take it and process it)
-                # - "s" the extractor processed the data and is waiting
-                #   for the segmenter
-                if self.slot_states[cur_slot] == "e":
-                    # The segmenter has something for us in this slot.
-                    break
-                else:
-                    # Try another slot.
-                    unavailable_slots += 1
-                    cur_slot = (cur_slot + 1) % num_slots
-                if unavailable_slots >= num_slots:
-                    # There is nothing to do, try to avoid 100% CPU
-                    unavailable_slots = 0
-                    time.sleep(.1)
+            while not found_free_slot:
+                # We sort the slots according to the slot chunks so that we
+                # always process the slot with the smallest slot chunk number
+                # first. Initially, the slot_chunks array is filled with
+                # zeros, but the segmenter fills up the slots with the lowest
+                # number first.
+                for cur_slot in np.argsort(self.slot_chunks):
+                    # - "e" there is data from the segmenter (the extractor
+                    #   can take it and process it)
+                    # - "s" the extractor processed the data and is waiting
+                    #   for the segmenter
+                    if self.slot_states[cur_slot] == "e":
+                        # The segmenter has something for us in this slot.
+                        found_free_slot = True
+                        break
+                    else:
+                        # Try another slot.
+                        unavailable_slots += 1
+                        cur_slot = (cur_slot + 1) % num_slots
+                    if unavailable_slots >= num_slots:
+                        # There is nothing to do, try to avoid 100% CPU
+                        unavailable_slots = 0
+                        time.sleep(.1)
 
             t1 = time.monotonic()
 
             # We have a chunk, process it!
             chunk = self.slot_chunks[cur_slot]
             # Populate the labeling array for the workers
             new_labels = self.labels_list[cur_slot]
@@ -145,15 +152,15 @@
             # Make sure the entire chunk has been processed.
             while np.sum(worker_monitor) != frames_processed + chunk_size:
                 time.sleep(.1)
 
             # We are done here. The segmenter may continue its deed.
             self.slot_states[cur_slot] = "w"
 
-            self.logger.debug(f"Extracted one chunk: {chunk}")
+            self.logger.debug(f"Extracted chunk {chunk} in slot {cur_slot}")
             self.t_count += time.monotonic() - t1
 
             chunks_processed += 1
             frames_processed += chunk_size
 
             if chunks_processed == self.data.image.num_chunks:
                 break
```

### Comparing `dcnum-0.20.3/src/dcnum/feat/feat_background/base.py` & `dcnum-0.20.4/src/dcnum/feat/feat_background/base.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/src/dcnum/feat/feat_background/bg_copy.py` & `dcnum-0.20.4/src/dcnum/feat/feat_background/bg_copy.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/src/dcnum/feat/feat_background/bg_roll_median.py` & `dcnum-0.20.4/src/dcnum/feat/feat_background/bg_roll_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/src/dcnum/feat/feat_background/bg_sparse_median.py` & `dcnum-0.20.4/src/dcnum/feat/feat_background/bg_sparse_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/src/dcnum/feat/feat_brightness/bright_all.py` & `dcnum-0.20.4/src/dcnum/feat/feat_brightness/bright_all.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/src/dcnum/feat/feat_contour/moments.py` & `dcnum-0.20.4/src/dcnum/feat/feat_contour/moments.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/src/dcnum/feat/feat_contour/volume.py` & `dcnum-0.20.4/src/dcnum/feat/feat_contour/volume.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/src/dcnum/feat/feat_texture/tex_all.py` & `dcnum-0.20.4/src/dcnum/feat/feat_texture/tex_all.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/src/dcnum/feat/gate.py` & `dcnum-0.20.4/src/dcnum/feat/gate.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/src/dcnum/feat/queue_event_extractor.py` & `dcnum-0.20.4/src/dcnum/feat/queue_event_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                  event_queue: mp.Queue,
                  log_queue: mp.Queue,
                  feat_nevents: mp.Array,
                  label_array: mp.Array,
                  finalize_extraction: mp.Value,
                  invalid_mask_counter: mp.Value,
                  worker_monitor: mp.RawArray,
-                 log_level: int = logging.INFO,
+                 log_level: int = None,
                  extract_kwargs: dict = None,
                  worker_index: int = None,
                  *args, **kwargs):
         """Base class for event extraction from label images
 
         This class is meant to be subclassed to run either in a
         :class:`threading.Thread` or a :class:`multiprocessing.Process`.
@@ -99,15 +99,15 @@
         self.invalid_mask_counter = invalid_mask_counter
         #: worker busy counter
         self.worker_monitor = worker_monitor
         # Logging needs to be set up after `start` is called, otherwise
         # it looks like we have the same PID as the parent process. We
         # are setting up logging in `run`.
         self.logger = None
-        self.log_level = log_level
+        self.log_level = log_level or logging.getLogger("dcnum").level
         #: Shared array of length `len(data)` into which the number of
         #: events per frame is written.
         self.feat_nevents = feat_nevents
         #: Shared array containing the labels of one chunk from `data`.
         self.label_array = label_array
         #: Set to True to let worker join when `raw_queue` is empty.
         self.finalize_extraction = finalize_extraction
@@ -120,15 +120,15 @@
         self.extract_kwargs = extract_kwargs
 
     @staticmethod
     def get_init_kwargs(data: HDF5Data,
                         gate: Gate,
                         num_extractors: int,
                         log_queue: mp.Queue,
-                        log_level: int = logging.INFO,
+                        log_level: int = None,
                         ):
         """Get initialization arguments for :cass:`.QueueEventExtractor`
 
         This method was created for convenience reasons:
         - It makes sure that the order of arguments is correct, since it
           is implemented in the same class.
         - It simplifies testing.
@@ -168,15 +168,15 @@
         # "h" is signed short (np.int16)
         args["label_array"] = mp_spawn.RawArray(
             np.ctypeslib.ctypes.c_int16,
             int(np.prod(data.image.chunk_shape)))
         args["finalize_extraction"] = mp_spawn.Value("b", False)
         args["invalid_mask_counter"] = mp_spawn.Value("L", 0)
         args["worker_monitor"] = mp_spawn.RawArray("L", num_extractors)
-        args["log_level"] = log_level
+        args["log_level"] = log_level or logging.getLogger("dcnum").level
         return args
 
     def get_events_from_masks(self, masks, data_index, *,
                               brightness: bool = True,
                               haralick: bool = True,
                               volume: bool = True,
                               ):
```

### Comparing `dcnum-0.20.3/src/dcnum/logic/ctrl.py` & `dcnum-0.20.4/src/dcnum/logic/ctrl.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,16 +86,15 @@
         self._progress_bn = None  # creating basins
         # segmentation frame rate
         self._segm_rate = 0
 
         # Set up logging
         # General logger for this job
         self.main_logger = logging.getLogger("dcnum")
-        self.main_logger.setLevel(
-            logging.DEBUG if job["debug"] else logging.INFO)
+        self.main_logger.setLevel(job["log_level"])
         # Log file output in target directory
         self.path_log = job["path_out"].with_suffix(".log")
         self.path_log.parent.mkdir(exist_ok=True, parents=True)
         self.path_log.unlink(missing_ok=True)
         self._log_file_handler = logging.FileHandler(
             filename=self.path_log,
             encoding="utf-8",
@@ -655,42 +654,50 @@
             # to the total number of CPUs. However, we would need more RAM
             # (for caching the image data) and we also have more overhead.
             # Having two slots shared between all workers is more efficient.
             num_slots = 2
             # Split segmentation and feature extraction workers evenly.
             num_extractors = self.job["num_procs"] // 2
             num_segmenters = self.job["num_procs"] - num_extractors
+            # leave one CPU for the writer and the remaining Threads
+            num_segmenters -= 1
         else:  # GPU segmenter
             num_slots = 3
             num_extractors = self.job["num_procs"]
+            # leave one CPU for the writer and the remaining Threads
+            num_extractors -= 1
             num_segmenters = 1
         num_extractors = max(1, num_extractors)
         num_segmenters = max(1, num_segmenters)
         self.job.kwargs["segmenter_kwargs"]["num_workers"] = num_segmenters
-        slot_chunks = mp_spawn.Array("i", num_slots)
-        slot_states = mp_spawn.Array("u", num_slots)
+        self.job.kwargs["segmenter_kwargs"]["debug"] = self.job["debug"]
+        slot_chunks = mp_spawn.Array("i", num_slots, lock=False)
+        slot_states = mp_spawn.Array("u", num_slots, lock=False)
+
+        self.logger.debug(f"Number of slots: {num_slots}")
+        self.logger.debug(f"Number of segmenters: {num_segmenters}")
+        self.logger.debug(f"Number of extractors: {num_extractors}")
 
         # Initialize segmenter manager thread
         thr_segm = SegmenterManagerThread(
             segmenter=seg_cls(**self.job["segmenter_kwargs"]),
             image_data=imdat,
             bg_off=self.dtin["bg_off"] if "bg_off" in self.dtin else None,
             slot_states=slot_states,
             slot_chunks=slot_chunks,
-            debug=self.job["debug"],
         )
         thr_segm.start()
 
         # Start feature extractor thread
         fe_kwargs = QueueEventExtractor.get_init_kwargs(
             data=self.dtin,
             gate=gate.Gate(self.dtin, **self.job["gate_kwargs"]),
             num_extractors=num_extractors,
             log_queue=self.log_queue,
-            log_level=logging.DEBUG if self.job["debug"] else logging.INFO,
+            log_level=self.logger.level,
             )
         fe_kwargs["extract_kwargs"] = self.job["feature_kwargs"]
 
         thr_feat = EventExtractorManagerThread(
             slot_chunks=slot_chunks,
             slot_states=slot_states,
             fe_kwargs=fe_kwargs,
```

### Comparing `dcnum-0.20.3/src/dcnum/logic/job.py` & `dcnum-0.20.4/src/dcnum/logic/job.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import collections
 import copy
 import inspect
+import logging
 import multiprocessing as mp
 import pathlib
 from typing import Dict, Literal
 import warnings
 
 from ..feat import QueueEventExtractor
 from ..feat.feat_background.base import get_available_background_methods
@@ -27,14 +28,15 @@
                  feature_code: str = "legacy",
                  feature_kwargs: Dict = None,
                  gate_code: str = "norm",
                  gate_kwargs: Dict = None,
                  basin_strategy: Literal["drain", "tap"] = "drain",
                  no_basins_in_output: bool = None,
                  num_procs: int = None,
+                 log_level: int = logging.INFO,
                  debug: bool = False,
                  ):
         """Pipeline job recipe
 
         Parameters
         ----------
         path_in: pathlib.Path | str
@@ -69,16 +71,19 @@
               will contain all features, but will also be very big.
             - You can "tap" the basins, including the input file, which means
               that the output file will be comparatively small.
         no_basins_in_output: bool
             Deprecated
         num_procs: int
             Number of processes to use
+        log_level: int
+            Logging level to use.
         debug: bool
-            Whether to be verbose and use threads instead of processes
+            Whether to set logging level to "DEBUG" and
+            use threads instead of processes
         """
         if no_basins_in_output is not None:
             warnings.warn("The `no_basins_in_output` keyword argument is "
                           "deprecated. Please use `basin_strategy` instead.")
             if no_basins_in_output:
                 basin_strategy = "drain"
             else:
@@ -100,14 +105,17 @@
             # Extract from input file
             with HDF5Data(path_in) as hd:
                 self.kwargs["data_kwargs"]["pixel_size"] = hd.pixel_size
         # Set default output path
         if path_out is None:
             pin = pathlib.Path(path_in)
             path_out = pin.with_name(pin.stem + "_dcn.rtdc")
+        # Set logging level to DEBUG in debugging mode
+        if self.kwargs["debug"]:
+            self.kwargs["log_level"] = logging.DEBUG
         self.kwargs["path_out"] = pathlib.Path(path_out)
         # Set default mask kwargs for segmenter
         self.kwargs["segmenter_kwargs"].setdefault("kwargs_mask", {})
         # Set default number of processes
         if num_procs is None:
             self.kwargs["num_procs"] = mp.cpu_count()
```

### Comparing `dcnum-0.20.3/src/dcnum/logic/json_encoder.py` & `dcnum-0.20.4/src/dcnum/logic/json_encoder.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/src/dcnum/meta/paths.py` & `dcnum-0.20.4/src/dcnum/meta/paths.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/src/dcnum/meta/ppid.py` & `dcnum-0.20.4/src/dcnum/meta/ppid.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/src/dcnum/read/cache.py` & `dcnum-0.20.4/src/dcnum/read/cache.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/src/dcnum/read/hdf5_data.py` & `dcnum-0.20.4/src/dcnum/read/hdf5_data.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/src/dcnum/read/mapped.py` & `dcnum-0.20.4/src/dcnum/read/mapped.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/src/dcnum/segm/segm_thresh.py` & `dcnum-0.20.4/src/dcnum/segm/segm_thresh.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/src/dcnum/segm/segmenter.py` & `dcnum-0.20.4/src/dcnum/segm/segmenter.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         """Base segmenter
 
         Parameters
         ----------
         kwargs_mask: dict
             Keyword arguments for mask post-processing (see `process_mask`)
         debug: bool
-            Debugging parameters
+            Enable debugging mode (e.g. CPU segmenter runs in one thread)
         kwargs:
             Additional, optional keyword arguments for `segment_batch`.
         """
         self.debug = debug
         self.logger = logging.getLogger(__name__).getChild(
             self.__class__.__name__)
         spec = inspect.getfullargspec(self.segment_approach)
```

### Comparing `dcnum-0.20.3/src/dcnum/segm/segmenter_cpu.py` & `dcnum-0.20.4/src/dcnum/segm/segmenter_cpu.py`

 * *Files 7% similar despite different names*

```diff
@@ -185,17 +185,19 @@
         # populate image data
         self._mp_image_np[:] = image_data[start:stop]
 
         # Create the workers
         if self.debug:
             worker_cls = CPUSegmenterWorkerThread
             num_workers = 1
+            self.logger.debug("Running with one worker in main thread")
         else:
             worker_cls = CPUSegmenterWorkerProcess
             num_workers = min(self.num_workers, image_data.shape[0])
+            self.logger.debug(f"Running with {num_workers} workers")
 
         if not self._mp_workers:
             step_size = batch_size // num_workers
             rest = batch_size % num_workers
             wstart = 0
             for ii in range(num_workers):
                 # Give every worker the same-sized workload and add one
```

### Comparing `dcnum-0.20.3/src/dcnum/segm/segmenter_gpu.py` & `dcnum-0.20.4/src/dcnum/segm/segmenter_gpu.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/src/dcnum/segm/segmenter_manager_thread.py` & `dcnum-0.20.4/src/dcnum/segm/segmenter_manager_thread.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 class SegmenterManagerThread(threading.Thread):
     def __init__(self,
                  segmenter: Segmenter,
                  image_data: HDF5ImageCache | ImageCorrCache,
                  slot_states: mp.Array,
                  slot_chunks: mp.Array,
                  bg_off: np.ndarray = None,
-                 debug: bool = False,
                  *args, **kwargs):
         """Manage the segmentation of image data
 
         Parameters
         ----------
         segmenter:
             The segmenter instance to use.
@@ -39,18 +38,14 @@
         slot_chunks:
             For each slot in `slot_states`, this shared array defines
             on which chunk in `image_data` the segmentation took place.
         bg_off:
             1d array containing additional background image offset values
             that are added to each background image before subtraction
             from the input image
-        debug:
-            Whether to run in debugging mode (more verbose messages and
-            CPU-based segmentation is done in one single thread instead
-            of in multiple subprocesses).
 
         Notes
         -----
         This manager keeps a list `labels_list` which enumerates the
         slots just like `slot_states` and `slot_chunks` do. For each
         slot, this list contains the labeled image data (integer-valued)
         for the input `image_data` chunks.
@@ -76,41 +71,44 @@
         self.slot_states = slot_states
         #: Current slot chunk index for the slot states
         self.slot_chunks = slot_chunks
         #: List containing the segmented labels of each slot
         self.labels_list = [None] * len(self.slot_states)
         #: Time counter for segmentation
         self.t_count = 0
-        #: Whether running in debugging mode
-        self.debug = debug
 
     def run(self):
         num_slots = len(self.slot_states)
         # We iterate over all the chunks of the image data.
         for chunk in self.image_data.iter_chunks():
-            cur_slot = 0
-            empty_slots = 0
+            unavailable_slots = 0
+            found_free_slot = False
             # Wait for a free slot to perform segmentation (compute labels)
-            while True:
-                # - "e" there is data from the segmenter (the extractor
-                #   can take it and process it)
-                # - "s" the extractor processed the data and is waiting
-                #   for the segmenter
-                if self.slot_states[cur_slot] != "e":
-                    # It's the segmenter's turn. Note that we use '!= "e"',
-                    # because the initial value is "\x00".
-                    break
-                else:
-                    # Try another slot.
-                    empty_slots += 1
-                    cur_slot = (cur_slot + 1) % num_slots
-                if empty_slots >= num_slots:
-                    # There is nothing to do, try to avoid 100% CPU
-                    empty_slots = 0
-                    time.sleep(.01)
+            while not found_free_slot:
+                # We sort the slots according to the slot chunks so that we
+                # always process the slot with the smallest slot chunk number
+                # first. Initially, the slot_chunks array is filled with
+                # zeros, but we populate it here.
+                for cur_slot in np.argsort(self.slot_chunks):
+                    # - "e" there is data from the segmenter (the extractor
+                    #   can take it and process it)
+                    # - "s" the extractor processed the data and is waiting
+                    #   for the segmenter
+                    if self.slot_states[cur_slot] != "e":
+                        # It's the segmenter's turn. Note that we use '!= "e"',
+                        # because the initial value is "\x00".
+                        found_free_slot = True
+                        break
+                    else:
+                        # Try another slot.
+                        unavailable_slots += 1
+                    if unavailable_slots >= num_slots:
+                        # There is nothing to do, try to avoid 100% CPU
+                        unavailable_slots = 0
+                        time.sleep(.1)
 
             t1 = time.monotonic()
 
             # We have a free slot to compute the segmentation
             labels = self.segmenter.segment_chunk(
                 image_data=self.image_data,
                 chunk=chunk,
@@ -121,15 +119,15 @@
             # Store labels in a list accessible by the main thread
             self.labels_list[cur_slot] = np.copy(labels)
             # Remember the chunk index for this slot
             self.slot_chunks[cur_slot] = chunk
             # This must be done last: Let the extractor know that this
             # slot is ready for processing.
             self.slot_states[cur_slot] = "e"
-            self.logger.debug(f"Segmented one chunk: {chunk}")
+            self.logger.debug(f"Segmented chunk {chunk} in slot {cur_slot}")
 
             self.t_count += time.monotonic() - t1
 
         # Cleanup
         if isinstance(self.segmenter, CPUSegmenter):
             # Join the segmentation workers.
             self.segmenter.join_workers()
```

### Comparing `dcnum-0.20.3/src/dcnum/write/deque_writer_thread.py` & `dcnum-0.20.4/src/dcnum/write/deque_writer_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/src/dcnum/write/queue_collector_thread.py` & `dcnum-0.20.4/src/dcnum/write/queue_collector_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/src/dcnum/write/writer.py` & `dcnum-0.20.4/src/dcnum/write/writer.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/src/dcnum.egg-info/PKG-INFO` & `dcnum-0.20.4/src/dcnum.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.20.3
+Version: 0.20.4
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Maximilian Schlögel, Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.20.3/src/dcnum.egg-info/SOURCES.txt` & `dcnum-0.20.4/src/dcnum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/conftest.py` & `dcnum-0.20.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/data/fmt-hdf5_cytoshot_extended-moments-features.zip` & `dcnum-0.20.4/tests/data/fmt-hdf5_cytoshot_extended-moments-features.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip` & `dcnum-0.20.4/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/data/fmt-hdf5_cytoshot_full-features_2024.zip` & `dcnum-0.20.4/tests/data/fmt-hdf5_cytoshot_full-features_2024.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip` & `dcnum-0.20.4/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/data/fmt-hdf5_shapein_empty.zip` & `dcnum-0.20.4/tests/data/fmt-hdf5_shapein_empty.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/data/fmt-hdf5_shapein_raw-with-variable-length-logs.zip` & `dcnum-0.20.4/tests/data/fmt-hdf5_shapein_raw-with-variable-length-logs.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/helper_methods.py` & `dcnum-0.20.4/tests/helper_methods.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_feat_background_base.py` & `dcnum-0.20.4/tests/test_feat_background_base.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_feat_background_bg_copy.py` & `dcnum-0.20.4/tests/test_feat_background_bg_copy.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_feat_background_bg_roll_median.py` & `dcnum-0.20.4/tests/test_feat_background_bg_roll_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_feat_background_bg_sparsemed.py` & `dcnum-0.20.4/tests/test_feat_background_bg_sparsemed.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_feat_brightness.py` & `dcnum-0.20.4/tests/test_feat_brightness.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_feat_event_extractor_manager.py` & `dcnum-0.20.4/tests/test_feat_event_extractor_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     thr_segm = SegmenterManagerThread(
         segmenter=SegmentThresh(
             kwargs_mask={"closing_disk": 0},  # otherwise no event in 1st image
         ),
         image_data=hd.image_corr,
         slot_states=slot_states,
         slot_chunks=slot_chunks,
-        debug=True,
     )
     thr_segm.start()
 
     fe_kwargs = QueueEventExtractor.get_init_kwargs(
         data=hd,
         gate=Gate(hd),
         num_extractors=1,
```

### Comparing `dcnum-0.20.3/tests/test_feat_gate.py` & `dcnum-0.20.4/tests/test_feat_gate.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_feat_haralick.py` & `dcnum-0.20.4/tests/test_feat_haralick.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_feat_moments_based.py` & `dcnum-0.20.4/tests/test_feat_moments_based.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_feat_moments_based_extended.py` & `dcnum-0.20.4/tests/test_feat_moments_based_extended.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_feat_volume.py` & `dcnum-0.20.4/tests/test_feat_volume.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_logic_job.py` & `dcnum-0.20.4/tests/test_logic_job.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_logic_join.py` & `dcnum-0.20.4/tests/test_logic_join.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_logic_pipeline.py` & `dcnum-0.20.4/tests/test_logic_pipeline.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_meta_paths.py` & `dcnum-0.20.4/tests/test_meta_paths.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_meta_ppid_base.py` & `dcnum-0.20.4/tests/test_meta_ppid_base.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_meta_ppid_bg.py` & `dcnum-0.20.4/tests/test_meta_ppid_bg.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_meta_ppid_data.py` & `dcnum-0.20.4/tests/test_meta_ppid_data.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_meta_ppid_feat.py` & `dcnum-0.20.4/tests/test_meta_ppid_feat.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_meta_ppid_gate.py` & `dcnum-0.20.4/tests/test_meta_ppid_gate.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_meta_ppid_segm.py` & `dcnum-0.20.4/tests/test_meta_ppid_segm.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_read_basin.py` & `dcnum-0.20.4/tests/test_read_basin.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_read_concat_hdf5.py` & `dcnum-0.20.4/tests/test_read_concat_hdf5.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_read_hdf5.py` & `dcnum-0.20.4/tests/test_read_hdf5.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_read_hdf5_basins.py` & `dcnum-0.20.4/tests/test_read_hdf5_basins.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_read_hdf5_index_mapping.py` & `dcnum-0.20.4/tests/test_read_hdf5_index_mapping.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_segm_base.py` & `dcnum-0.20.4/tests/test_segm_base.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_segm_no_mask_proc.py` & `dcnum-0.20.4/tests/test_segm_no_mask_proc.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_segm_thresh.py` & `dcnum-0.20.4/tests/test_segm_thresh.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_write_deque_writer_thread.py` & `dcnum-0.20.4/tests/test_write_deque_writer_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_write_queue_collector_thread.py` & `dcnum-0.20.4/tests/test_write_queue_collector_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.3/tests/test_write_writer.py` & `dcnum-0.20.4/tests/test_write_writer.py`

 * *Files identical despite different names*

