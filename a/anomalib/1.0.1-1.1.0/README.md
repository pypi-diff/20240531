# Comparing `tmp/anomalib-1.0.1.tar.gz` & `tmp/anomalib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anomalib-1.0.1.tar", last modified: Wed Mar 27 16:33:11 2024, max compression
+gzip compressed data, was "anomalib-1.1.0.tar", last modified: Fri May 31 15:52:34 2024, max compression
```

## Comparing `anomalib-1.0.1.tar` & `anomalib-1.1.0.tar`

### file list

```diff
@@ -1,311 +1,334 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.062467 anomalib-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-27 16:32:58.000000 anomalib-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-27 16:32:58.000000 anomalib-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    24636 2024-03-27 16:33:11.062467 anomalib-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11258 2024-03-27 16:32:58.000000 anomalib-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7561 2024-03-27 16:32:58.000000 anomalib-1.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.034468 anomalib-1.0.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-27 16:32:58.000000 anomalib-1.0.1/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-27 16:32:58.000000 anomalib-1.0.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-27 16:32:58.000000 anomalib-1.0.1/requirements/installer.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-27 16:32:58.000000 anomalib-1.0.1/requirements/loggers.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-27 16:32:58.000000 anomalib-1.0.1/requirements/notebooks.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-27 16:32:58.000000 anomalib-1.0.1/requirements/openvino.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 16:33:11.062467 anomalib-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-03-27 16:32:58.000000 anomalib-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.030468 anomalib-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.034468 anomalib-1.0.1/src/anomalib/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.038468 anomalib-1.0.1/src/anomalib/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/callbacks/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/callbacks/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/callbacks/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/callbacks/model_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.038468 anomalib-1.0.1/src/anomalib/callbacks/nncf/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/callbacks/nncf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/callbacks/nncf/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     8560 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/callbacks/nncf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.038468 anomalib-1.0.1/src/anomalib/callbacks/normalization/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/callbacks/normalization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/callbacks/normalization/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/callbacks/normalization/min_max_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/callbacks/normalization/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/callbacks/post_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7400 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/callbacks/thresholding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/callbacks/tiler_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/callbacks/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7279 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/callbacks/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.038468 anomalib-1.0.1/src/anomalib/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20604 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/cli/install.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.038468 anomalib-1.0.1/src/anomalib/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/cli/utils/help_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    16173 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/cli/utils/installation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/cli/utils/openvino.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.038468 anomalib-1.0.1/src/anomalib/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.038468 anomalib-1.0.1/src/anomalib/data/base/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12039 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/base/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/base/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/base/depth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/base/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.038468 anomalib-1.0.1/src/anomalib/data/depth/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/depth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19072 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/depth/folder_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    12456 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/depth/mvtec_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.042468 anomalib-1.0.1/src/anomalib/data/image/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13103 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/image/btech.py
--rw-r--r--   0 runner    (1001) docker     (127)    19472 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/image/folder.py
--rw-r--r--   0 runner    (1001) docker     (127)    13495 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/image/kolektor.py
--rw-r--r--   0 runner    (1001) docker     (127)    16266 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/image/mvtec.py
--rw-r--r--   0 runner    (1001) docker     (127)    13188 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/image/visa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.042468 anomalib-1.0.1/src/anomalib/data/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/transforms/center_crop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.042468 anomalib-1.0.1/src/anomalib/data/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/utils/augmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/utils/boxes.py
--rw-r--r--   0 runner    (1001) docker     (127)    16864 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/utils/download.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.042468 anomalib-1.0.1/src/anomalib/data/utils/generators/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/utils/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/utils/generators/perlin.py
--rw-r--r--   0 runner    (1001) docker     (127)    15469 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/utils/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     7804 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/utils/split.py
--rw-r--r--   0 runner    (1001) docker     (127)     6786 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/utils/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (127)    15488 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/utils/tiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.042468 anomalib-1.0.1/src/anomalib/data/video/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19461 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/video/avenue.py
--rw-r--r--   0 runner    (1001) docker     (127)    14559 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/video/shanghaitech.py
--rw-r--r--   0 runner    (1001) docker     (127)    11606 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/data/video/ucsd_ped.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.042468 anomalib-1.0.1/src/anomalib/deploy/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13538 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/deploy/export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.042468 anomalib-1.0.1/src/anomalib/deploy/inferencers/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/deploy/inferencers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/deploy/inferencers/base_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12280 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/deploy/inferencers/openvino_inferencer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/deploy/inferencers/torch_inferencer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.042468 anomalib-1.0.1/src/anomalib/engine/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41022 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/engine/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.046468 anomalib-1.0.1/src/anomalib/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/loggers/comet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/loggers/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/loggers/wandb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.046468 anomalib-1.0.1/src/anomalib/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/metrics/anomaly_score_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/metrics/aupr.py
--rw-r--r--   0 runner    (1001) docker     (127)    12185 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/metrics/aupro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/metrics/auroc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/metrics/binning.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/metrics/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/metrics/f1_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/metrics/min_max.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/metrics/optimal_f1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/metrics/plotting_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/metrics/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/metrics/pro.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.046468 anomalib-1.0.1/src/anomalib/metrics/threshold/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/metrics/threshold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/metrics/threshold/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/metrics/threshold/f1_adaptive_threshold.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/metrics/threshold/manual_threshold.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.046468 anomalib-1.0.1/src/anomalib/models/
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.046468 anomalib-1.0.1/src/anomalib/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.046468 anomalib-1.0.1/src/anomalib/models/components/base/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/components/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11116 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/components/base/anomaly_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/components/base/buffer_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/components/base/dynamic_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/components/base/memory_bank_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.046468 anomalib-1.0.1/src/anomalib/models/components/classification/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/components/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/components/classification/kde_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.050468 anomalib-1.0.1/src/anomalib/models/components/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/components/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/components/cluster/gmm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/components/cluster/kmeans.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.050468 anomalib-1.0.1/src/anomalib/models/components/dimensionality_reduction/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/components/dimensionality_reduction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/components/dimensionality_reduction/pca.py
--rw-r--r--   0 runner    (1001) docker     (127)     6108 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/components/dimensionality_reduction/random_projection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.050468 anomalib-1.0.1/src/anomalib/models/components/feature_extractors/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/components/feature_extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/components/feature_extractors/timm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10021 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/components/feature_extractors/torchfx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/components/feature_extractors/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.050468 anomalib-1.0.1/src/anomalib/models/components/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/components/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/components/filters/blur.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.050468 anomalib-1.0.1/src/anomalib/models/components/flow/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/components/flow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13689 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/components/flow/all_in_one_block.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.050468 anomalib-1.0.1/src/anomalib/models/components/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/components/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/components/layers/sspcab.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.050468 anomalib-1.0.1/src/anomalib/models/components/sampling/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/components/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/components/sampling/k_center_greedy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.050468 anomalib-1.0.1/src/anomalib/models/components/stats/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/components/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/components/stats/kde.py
--rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/components/stats/multi_variate_gaussian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.050468 anomalib-1.0.1/src/anomalib/models/image/
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.050468 anomalib-1.0.1/src/anomalib/models/image/cfa/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/cfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/cfa/anomaly_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/cfa/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/cfa/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/cfa/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.050468 anomalib-1.0.1/src/anomalib/models/image/cflow/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/cflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/cflow/anomaly_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/cflow/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/cflow/torch_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/cflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.054468 anomalib-1.0.1/src/anomalib/models/image/csflow/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/csflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/csflow/anomaly_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/csflow/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/csflow/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    22137 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/csflow/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.054468 anomalib-1.0.1/src/anomalib/models/image/dfkde/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/dfkde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/dfkde/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/dfkde/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.054468 anomalib-1.0.1/src/anomalib/models/image/dfm/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/dfm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/dfm/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/dfm/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.054468 anomalib-1.0.1/src/anomalib/models/image/draem/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/draem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/draem/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/draem/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    19825 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/draem/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.054468 anomalib-1.0.1/src/anomalib/models/image/dsr/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/dsr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/dsr/anomaly_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/dsr/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/dsr/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    49228 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/dsr/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.054468 anomalib-1.0.1/src/anomalib/models/image/efficient_ad/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/efficient_ad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/efficient_ad/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16694 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/efficient_ad/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.054468 anomalib-1.0.1/src/anomalib/models/image/fastflow/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/fastflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/fastflow/anomaly_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/fastflow/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/fastflow/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/fastflow/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.054468 anomalib-1.0.1/src/anomalib/models/image/ganomaly/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/ganomaly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/ganomaly/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/ganomaly/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    13459 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/ganomaly/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.054468 anomalib-1.0.1/src/anomalib/models/image/padim/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/padim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/padim/anomaly_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/padim/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/padim/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.058467 anomalib-1.0.1/src/anomalib/models/image/patchcore/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/patchcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/patchcore/anomaly_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/patchcore/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9352 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/patchcore/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.058467 anomalib-1.0.1/src/anomalib/models/image/reverse_distillation/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/reverse_distillation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/reverse_distillation/anomaly_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.058467 anomalib-1.0.1/src/anomalib/models/image/reverse_distillation/components/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/reverse_distillation/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/reverse_distillation/components/bottleneck.py
--rw-r--r--   0 runner    (1001) docker     (127)    12033 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/reverse_distillation/components/de_resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/reverse_distillation/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/reverse_distillation/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/reverse_distillation/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.058467 anomalib-1.0.1/src/anomalib/models/image/rkde/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/rkde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/rkde/feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/rkde/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/rkde/region_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/rkde/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.058467 anomalib-1.0.1/src/anomalib/models/image/stfpm/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/stfpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/stfpm/anomaly_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/stfpm/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/stfpm/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/stfpm/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.058467 anomalib-1.0.1/src/anomalib/models/image/uflow/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/uflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7689 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/uflow/anomaly_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     6480 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/uflow/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/uflow/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/uflow/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     6857 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/uflow/torch_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.058467 anomalib-1.0.1/src/anomalib/models/image/winclip/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/winclip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/winclip/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/winclip/prompting.py
--rw-r--r--   0 runner    (1001) docker     (127)    18709 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/winclip/torch_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9356 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/image/winclip/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.062467 anomalib-1.0.1/src/anomalib/models/video/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/video/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.062467 anomalib-1.0.1/src/anomalib/models/video/ai_vad/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/video/ai_vad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.062467 anomalib-1.0.1/src/anomalib/models/video/ai_vad/clip/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/video/ai_vad/clip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8274 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/video/ai_vad/clip/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)    18045 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/video/ai_vad/clip/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13718 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/video/ai_vad/density.py
--rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/video/ai_vad/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/video/ai_vad/flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/video/ai_vad/lightning_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11816 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/video/ai_vad/regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/models/video/ai_vad/torch_model.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.062467 anomalib-1.0.1/src/anomalib/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/utils/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.062467 anomalib-1.0.1/src/anomalib/utils/cv/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/utils/cv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/utils/cv/connected_components.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.062467 anomalib-1.0.1/src/anomalib/utils/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/utils/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/utils/exceptions/imports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.062467 anomalib-1.0.1/src/anomalib/utils/normalization/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/utils/normalization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/utils/normalization/min_max.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/utils/post_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.062467 anomalib-1.0.1/src/anomalib/utils/types/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/utils/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.062467 anomalib-1.0.1/src/anomalib/utils/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/utils/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/utils/visualization/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15062 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/utils/visualization/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-03-27 16:32:58.000000 anomalib-1.0.1/src/anomalib/utils/visualization/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:33:11.034468 anomalib-1.0.1/src/anomalib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    24636 2024-03-27 16:33:10.000000 anomalib-1.0.1/src/anomalib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-03-27 16:33:11.000000 anomalib-1.0.1/src/anomalib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 16:33:10.000000 anomalib-1.0.1/src/anomalib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-27 16:33:10.000000 anomalib-1.0.1/src/anomalib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-27 16:33:10.000000 anomalib-1.0.1/src/anomalib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-27 16:33:10.000000 anomalib-1.0.1/src/anomalib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.844653 anomalib-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-31 15:52:26.000000 anomalib-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-31 15:52:26.000000 anomalib-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    27544 2024-05-31 15:52:34.844653 anomalib-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11415 2024-05-31 15:52:26.000000 anomalib-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-05-31 15:52:26.000000 anomalib-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:52:34.844653 anomalib-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.796652 anomalib-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.804653 anomalib-1.1.0/src/anomalib/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.808653 anomalib-1.1.0/src/anomalib/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/callbacks/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/callbacks/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/callbacks/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/callbacks/model_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.808653 anomalib-1.1.0/src/anomalib/callbacks/nncf/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/callbacks/nncf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/callbacks/nncf/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8560 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/callbacks/nncf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.808653 anomalib-1.1.0/src/anomalib/callbacks/normalization/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/callbacks/normalization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/callbacks/normalization/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/callbacks/normalization/min_max_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/callbacks/normalization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/callbacks/post_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7400 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/callbacks/thresholding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/callbacks/tiler_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/callbacks/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7279 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/callbacks/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.808653 anomalib-1.1.0/src/anomalib/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20335 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/cli/pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.808653 anomalib-1.1.0/src/anomalib/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9356 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/cli/utils/help_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16173 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/cli/utils/installation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/cli/utils/openvino.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.808653 anomalib-1.1.0/src/anomalib/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.808653 anomalib-1.1.0/src/anomalib/data/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14293 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/base/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/base/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/base/depth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/base/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.808653 anomalib-1.1.0/src/anomalib/data/depth/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/depth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19072 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/depth/folder_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12456 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/depth/mvtec_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.812653 anomalib-1.1.0/src/anomalib/data/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13103 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/image/btech.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19472 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/image/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13495 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/image/kolektor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16266 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/image/mvtec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13188 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/image/visa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.812653 anomalib-1.1.0/src/anomalib/data/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/transforms/center_crop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.812653 anomalib-1.1.0/src/anomalib/data/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/utils/augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/utils/boxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16975 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/utils/download.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.812653 anomalib-1.1.0/src/anomalib/data/utils/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/utils/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/utils/generators/perlin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15469 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/utils/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7804 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/utils/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6786 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/utils/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15486 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/utils/tiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.812653 anomalib-1.1.0/src/anomalib/data/video/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19461 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/video/avenue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14559 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/video/shanghaitech.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11606 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/data/video/ucsd_ped.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.812653 anomalib-1.1.0/src/anomalib/deploy/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/deploy/export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.816653 anomalib-1.1.0/src/anomalib/deploy/inferencers/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/deploy/inferencers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/deploy/inferencers/base_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12509 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/deploy/inferencers/openvino_inferencer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/deploy/inferencers/torch_inferencer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.816653 anomalib-1.1.0/src/anomalib/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44701 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/engine/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.816653 anomalib-1.1.0/src/anomalib/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/loggers/comet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/loggers/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/loggers/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/loggers/wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.816653 anomalib-1.1.0/src/anomalib/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/metrics/anomaly_score_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/metrics/aupr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12185 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/metrics/aupro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/metrics/auroc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/metrics/binning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/metrics/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/metrics/f1_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/metrics/f1_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/metrics/min_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/metrics/plotting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/metrics/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/metrics/pro.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.816653 anomalib-1.1.0/src/anomalib/metrics/threshold/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/metrics/threshold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/metrics/threshold/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/metrics/threshold/f1_adaptive_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/metrics/threshold/manual_threshold.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.816653 anomalib-1.1.0/src/anomalib/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.820653 anomalib-1.1.0/src/anomalib/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.820653 anomalib-1.1.0/src/anomalib/models/components/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/components/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13915 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/components/base/anomaly_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/components/base/buffer_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/components/base/dynamic_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12133 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/components/base/export_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/components/base/memory_bank_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.820653 anomalib-1.1.0/src/anomalib/models/components/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/components/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/components/classification/kde_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.820653 anomalib-1.1.0/src/anomalib/models/components/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/components/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/components/cluster/gmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/components/cluster/kmeans.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.820653 anomalib-1.1.0/src/anomalib/models/components/dimensionality_reduction/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/components/dimensionality_reduction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/components/dimensionality_reduction/pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6108 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/components/dimensionality_reduction/random_projection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.820653 anomalib-1.1.0/src/anomalib/models/components/feature_extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/components/feature_extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/components/feature_extractors/timm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10021 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/components/feature_extractors/torchfx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/components/feature_extractors/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.820653 anomalib-1.1.0/src/anomalib/models/components/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/components/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/components/filters/blur.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.820653 anomalib-1.1.0/src/anomalib/models/components/flow/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/components/flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13689 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/components/flow/all_in_one_block.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.820653 anomalib-1.1.0/src/anomalib/models/components/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/components/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/components/layers/sspcab.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.820653 anomalib-1.1.0/src/anomalib/models/components/sampling/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/components/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/components/sampling/k_center_greedy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.824653 anomalib-1.1.0/src/anomalib/models/components/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/components/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/components/stats/kde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/components/stats/multi_variate_gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.824653 anomalib-1.1.0/src/anomalib/models/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.824653 anomalib-1.1.0/src/anomalib/models/image/cfa/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/cfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/cfa/anomaly_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/cfa/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/cfa/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/cfa/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.824653 anomalib-1.1.0/src/anomalib/models/image/cflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/cflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/cflow/anomaly_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/cflow/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/cflow/torch_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/cflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.824653 anomalib-1.1.0/src/anomalib/models/image/csflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/csflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/csflow/anomaly_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/csflow/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/csflow/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22143 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/csflow/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.824653 anomalib-1.1.0/src/anomalib/models/image/dfkde/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/dfkde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/dfkde/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/dfkde/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.824653 anomalib-1.1.0/src/anomalib/models/image/dfm/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/dfm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/dfm/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/dfm/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.824653 anomalib-1.1.0/src/anomalib/models/image/draem/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/draem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/draem/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/draem/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19825 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/draem/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.828653 anomalib-1.1.0/src/anomalib/models/image/dsr/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/dsr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/dsr/anomaly_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7579 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/dsr/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/dsr/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49291 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/dsr/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.828653 anomalib-1.1.0/src/anomalib/models/image/efficient_ad/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/efficient_ad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14130 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/efficient_ad/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16694 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/efficient_ad/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.828653 anomalib-1.1.0/src/anomalib/models/image/fastflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/fastflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/fastflow/anomaly_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/fastflow/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/fastflow/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/fastflow/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.828653 anomalib-1.1.0/src/anomalib/models/image/fre/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      174 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/fre/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3941 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/fre/lightning_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4318 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/fre/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.828653 anomalib-1.1.0/src/anomalib/models/image/ganomaly/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/ganomaly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/ganomaly/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/ganomaly/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13459 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/ganomaly/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.828653 anomalib-1.1.0/src/anomalib/models/image/padim/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/padim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/padim/anomaly_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/padim/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/padim/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.828653 anomalib-1.1.0/src/anomalib/models/image/patchcore/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/patchcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/patchcore/anomaly_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/patchcore/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9393 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/patchcore/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.832653 anomalib-1.1.0/src/anomalib/models/image/reverse_distillation/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/reverse_distillation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/reverse_distillation/anomaly_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.832653 anomalib-1.1.0/src/anomalib/models/image/reverse_distillation/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/reverse_distillation/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/reverse_distillation/components/bottleneck.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12033 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/reverse_distillation/components/de_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/reverse_distillation/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/reverse_distillation/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/reverse_distillation/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.832653 anomalib-1.1.0/src/anomalib/models/image/rkde/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/rkde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/rkde/feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/rkde/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/rkde/region_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/rkde/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.832653 anomalib-1.1.0/src/anomalib/models/image/stfpm/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/stfpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/stfpm/anomaly_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/stfpm/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/stfpm/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/stfpm/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.832653 anomalib-1.1.0/src/anomalib/models/image/uflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/uflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7689 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/uflow/anomaly_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/uflow/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/uflow/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/uflow/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/uflow/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.832653 anomalib-1.1.0/src/anomalib/models/image/winclip/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/winclip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/winclip/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/winclip/prompting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18873 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/winclip/torch_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9356 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/image/winclip/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.832653 anomalib-1.1.0/src/anomalib/models/video/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/video/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.836653 anomalib-1.1.0/src/anomalib/models/video/ai_vad/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/video/ai_vad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.836653 anomalib-1.1.0/src/anomalib/models/video/ai_vad/clip/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/video/ai_vad/clip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8274 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/video/ai_vad/clip/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18045 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/video/ai_vad/clip/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13718 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/video/ai_vad/density.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/video/ai_vad/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/video/ai_vad/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/video/ai_vad/lightning_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11816 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/video/ai_vad/regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/models/video/ai_vad/torch_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.836653 anomalib-1.1.0/src/anomalib/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.836653 anomalib-1.1.0/src/anomalib/pipelines/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/pipelines/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/pipelines/benchmark/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/pipelines/benchmark/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/pipelines/benchmark/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.836653 anomalib-1.1.0/src/anomalib/pipelines/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/pipelines/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.836653 anomalib-1.1.0/src/anomalib/pipelines/components/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/pipelines/components/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/pipelines/components/base/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/pipelines/components/base/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/pipelines/components/base/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.836653 anomalib-1.1.0/src/anomalib/pipelines/components/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/pipelines/components/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/pipelines/components/runners/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/pipelines/components/runners/serial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.836653 anomalib-1.1.0/src/anomalib/pipelines/components/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/pipelines/components/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/pipelines/components/utils/grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/pipelines/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.840653 anomalib-1.1.0/src/anomalib/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/utils/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.840653 anomalib-1.1.0/src/anomalib/utils/cv/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/utils/cv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/utils/cv/connected_components.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.840653 anomalib-1.1.0/src/anomalib/utils/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/utils/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/utils/exceptions/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.840653 anomalib-1.1.0/src/anomalib/utils/normalization/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/utils/normalization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/utils/normalization/min_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/utils/post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/utils/rich.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.840653 anomalib-1.1.0/src/anomalib/utils/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/utils/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.840653 anomalib-1.1.0/src/anomalib/utils/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/utils/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/utils/visualization/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15062 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/utils/visualization/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-31 15:52:26.000000 anomalib-1.1.0/src/anomalib/utils/visualization/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:52:34.840653 anomalib-1.1.0/src/anomalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27544 2024-05-31 15:52:34.000000 anomalib-1.1.0/src/anomalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11301 2024-05-31 15:52:34.000000 anomalib-1.1.0/src/anomalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:52:34.000000 anomalib-1.1.0/src/anomalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-31 15:52:34.000000 anomalib-1.1.0/src/anomalib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-31 15:52:34.000000 anomalib-1.1.0/src/anomalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 15:52:34.000000 anomalib-1.1.0/src/anomalib.egg-info/top_level.txt
```

### Comparing `anomalib-1.0.1/LICENSE` & `anomalib-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/PKG-INFO` & `anomalib-1.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 Metadata-Version: 2.1
 Name: anomalib
-Version: 1.0.1
+Version: 1.1.0
 Summary: anomalib - Anomaly Detection Library
-Home-page: 
 Author: Intel OpenVINO
-Author-email: help@openvino.intel.com
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -204,23 +202,83 @@
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Provides-Extra: loggers
+License-File: LICENSE
+Requires-Dist: omegaconf>=2.1.1
+Requires-Dist: rich>=13.5.2
+Requires-Dist: jsonargparse[signatures]>=4.27.7
+Requires-Dist: docstring_parser
+Requires-Dist: rich_argparse
 Provides-Extra: core
-Provides-Extra: notebooks
+Requires-Dist: av>=10.0.0; extra == "core"
+Requires-Dist: einops>=0.3.2; extra == "core"
+Requires-Dist: freia>=0.2; extra == "core"
+Requires-Dist: imgaug==0.4.0; extra == "core"
+Requires-Dist: kornia>=0.6.6; extra == "core"
+Requires-Dist: matplotlib>=3.4.3; extra == "core"
+Requires-Dist: opencv-python>=4.5.3.56; extra == "core"
+Requires-Dist: pandas>=1.1.0; extra == "core"
+Requires-Dist: timm<=1.0.3,>=0.5.4; extra == "core"
+Requires-Dist: lightning>=2.2; extra == "core"
+Requires-Dist: torch>=2; extra == "core"
+Requires-Dist: torchmetrics>=1.3.2; extra == "core"
+Requires-Dist: open-clip-torch>=2.23.0; extra == "core"
 Provides-Extra: openvino
+Requires-Dist: openvino>=2024.0; extra == "openvino"
+Requires-Dist: nncf>=2.10.0; extra == "openvino"
+Requires-Dist: onnx>=1.16.0; extra == "openvino"
+Provides-Extra: loggers
+Requires-Dist: comet-ml>=3.31.7; extra == "loggers"
+Requires-Dist: gradio>=4; extra == "loggers"
+Requires-Dist: tensorboard; extra == "loggers"
+Requires-Dist: wandb<=0.15.9,>=0.12.17; extra == "loggers"
+Requires-Dist: mlflow>=1.0.0; extra == "loggers"
+Provides-Extra: notebooks
+Requires-Dist: gitpython; extra == "notebooks"
+Requires-Dist: ipykernel; extra == "notebooks"
+Requires-Dist: ipywidgets; extra == "notebooks"
+Requires-Dist: notebook; extra == "notebooks"
+Provides-Extra: docs
+Requires-Dist: myst-parser; extra == "docs"
+Requires-Dist: nbsphinx; extra == "docs"
+Requires-Dist: pandoc; extra == "docs"
+Requires-Dist: sphinx<8.0; extra == "docs"
+Requires-Dist: sphinx_autodoc_typehints; extra == "docs"
+Requires-Dist: sphinx_book_theme; extra == "docs"
+Requires-Dist: sphinx-copybutton; extra == "docs"
+Requires-Dist: sphinx_design; extra == "docs"
+Provides-Extra: test
+Requires-Dist: pre-commit; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-xdist; extra == "test"
+Requires-Dist: pytest-mock; extra == "test"
+Requires-Dist: pytest-sugar; extra == "test"
+Requires-Dist: coverage[toml]; extra == "test"
+Requires-Dist: tox; extra == "test"
 Provides-Extra: full
+Requires-Dist: anomalib[core,loggers,notebooks,openvino]; extra == "full"
 Provides-Extra: dev
-License-File: LICENSE
+Requires-Dist: anomalib[docs,full,test]; extra == "dev"
 
 <div align="center">
 
 <img src="https://raw.githubusercontent.com/openvinotoolkit/anomalib/main/docs/source/_static/images/logos/anomalib-wide-blue.png" width="600px">
 
 **A library for benchmarking, developing and deploying deep learning anomaly detection algorithms**
 
@@ -235,14 +293,15 @@
 [![pytorch](https://img.shields.io/badge/pytorch-1.8.1%2B-orange)]()
 [![openvino](https://img.shields.io/badge/openvino-2022.3.0-purple)]()
 
 [![Pre-Merge Checks](https://github.com/openvinotoolkit/anomalib/actions/workflows/pre_merge.yml/badge.svg)](https://github.com/openvinotoolkit/anomalib/actions/workflows/pre_merge.yml)
 [![Documentation Status](https://readthedocs.org/projects/anomalib/badge/?version=latest)](https://anomalib.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/openvinotoolkit/anomalib/branch/main/graph/badge.svg?token=Z6A07N1BZK)](https://codecov.io/gh/openvinotoolkit/anomalib)
 [![Downloads](https://static.pepy.tech/personalized-badge/anomalib?period=total&units=international_system&left_color=grey&right_color=green&left_text=PyPI%20Downloads)](https://pepy.tech/project/anomalib)
+[![Discord](https://img.shields.io/discord/1230798452577800237?style=plastic)](https://discord.com/channels/1230798452577800237)
 
 </div>
 
 ---
 
 # 👋 Introduction
 
@@ -253,30 +312,30 @@
 </p>
 
 ## Key features
 
 - Simple and modular API and CLI for training, inference, benchmarking, and hyperparameter optimization.
 - The largest public collection of ready-to-use deep learning anomaly detection algorithms and benchmark datasets.
 - [**Lightning**](https://www.lightning.ai/) based model implementations to reduce boilerplate code and limit the implementation efforts to the bare essentials.
-- All models can be exported to [**OpenVINO**](https://www.intel.com/content/www/us/en/developer/tools/openvino-toolkit/overview.html) Intermediate Representation (IR) for accelerated inference on intel hardware.
+- The majority of models can be exported to [**OpenVINO**](https://www.intel.com/content/www/us/en/developer/tools/openvino-toolkit/overview.html) Intermediate Representation (IR) for accelerated inference on Intel hardware.
 - A set of [inference tools](tools) for quick and easy deployment of the standard or custom anomaly detection models.
 
 # 📦 Installation
 
 Anomalib provides two ways to install the library. The first is through PyPI, and the second is through a local installation. PyPI installation is recommended if you want to use the library without making any changes to the source code. If you want to make changes to the library, then a local installation is recommended.
 
 <details>
 <summary>Install from PyPI</summary>
 Installing the library with pip is the easiest way to get started with anomalib.
 
 ```bash
 pip install anomalib
 ```
 
-This will install Anomalib CLI using the [installer](requirements/installer.txt) dependencies. Anomalib CLI is a command line interface for training, inference, benchmarking, and hyperparameter optimization. If you want to use the library as a Python package, you can install the library with the following command:
+This will install Anomalib CLI using the [dependencies](/pyproject.toml) in the `pyproject.toml` file. Anomalib CLI is a command line interface for training, inference, benchmarking, and hyperparameter optimization. If you want to use the library as a Python package, you can install the library with the following command:
 
 ```bash
 # Get help for the installation arguments
 anomalib install -h
 
 # Install the full package
 anomalib install
@@ -308,15 +367,15 @@
 
 # Clone the repository and install in editable mode
 git clone https://github.com/openvinotoolkit/anomalib.git
 cd anomalib
 pip install -e .
 ```
 
-This will install Anomalib CLI using the [installer](requirements/installer.txt) dependencies. Anomalib CLI is a command line interface for training, inference, benchmarking, and hyperparameter optimization. If you want to use the library as a Python package, you can install the library with the following command:
+This will install Anomalib CLI using the [dependencies](/pyproject.toml) in the `pyproject.toml` file. Anomalib CLI is a command line interface for training, inference, benchmarking, and hyperparameter optimization. If you want to use the library as a Python package, you can install the library with the following command:
 
 ```bash
 # Get help for the installation arguments
 anomalib install -h
 
 # Install the full package
 anomalib install
```

### Comparing `anomalib-1.0.1/README.md` & `anomalib-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 [![pytorch](https://img.shields.io/badge/pytorch-1.8.1%2B-orange)]()
 [![openvino](https://img.shields.io/badge/openvino-2022.3.0-purple)]()
 
 [![Pre-Merge Checks](https://github.com/openvinotoolkit/anomalib/actions/workflows/pre_merge.yml/badge.svg)](https://github.com/openvinotoolkit/anomalib/actions/workflows/pre_merge.yml)
 [![Documentation Status](https://readthedocs.org/projects/anomalib/badge/?version=latest)](https://anomalib.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/openvinotoolkit/anomalib/branch/main/graph/badge.svg?token=Z6A07N1BZK)](https://codecov.io/gh/openvinotoolkit/anomalib)
 [![Downloads](https://static.pepy.tech/personalized-badge/anomalib?period=total&units=international_system&left_color=grey&right_color=green&left_text=PyPI%20Downloads)](https://pepy.tech/project/anomalib)
+[![Discord](https://img.shields.io/discord/1230798452577800237?style=plastic)](https://discord.com/channels/1230798452577800237)
 
 </div>
 
 ---
 
 # 👋 Introduction
 
@@ -33,30 +34,30 @@
 </p>
 
 ## Key features
 
 - Simple and modular API and CLI for training, inference, benchmarking, and hyperparameter optimization.
 - The largest public collection of ready-to-use deep learning anomaly detection algorithms and benchmark datasets.
 - [**Lightning**](https://www.lightning.ai/) based model implementations to reduce boilerplate code and limit the implementation efforts to the bare essentials.
-- All models can be exported to [**OpenVINO**](https://www.intel.com/content/www/us/en/developer/tools/openvino-toolkit/overview.html) Intermediate Representation (IR) for accelerated inference on intel hardware.
+- The majority of models can be exported to [**OpenVINO**](https://www.intel.com/content/www/us/en/developer/tools/openvino-toolkit/overview.html) Intermediate Representation (IR) for accelerated inference on Intel hardware.
 - A set of [inference tools](tools) for quick and easy deployment of the standard or custom anomaly detection models.
 
 # 📦 Installation
 
 Anomalib provides two ways to install the library. The first is through PyPI, and the second is through a local installation. PyPI installation is recommended if you want to use the library without making any changes to the source code. If you want to make changes to the library, then a local installation is recommended.
 
 <details>
 <summary>Install from PyPI</summary>
 Installing the library with pip is the easiest way to get started with anomalib.
 
 ```bash
 pip install anomalib
 ```
 
-This will install Anomalib CLI using the [installer](requirements/installer.txt) dependencies. Anomalib CLI is a command line interface for training, inference, benchmarking, and hyperparameter optimization. If you want to use the library as a Python package, you can install the library with the following command:
+This will install Anomalib CLI using the [dependencies](/pyproject.toml) in the `pyproject.toml` file. Anomalib CLI is a command line interface for training, inference, benchmarking, and hyperparameter optimization. If you want to use the library as a Python package, you can install the library with the following command:
 
 ```bash
 # Get help for the installation arguments
 anomalib install -h
 
 # Install the full package
 anomalib install
@@ -88,15 +89,15 @@
 
 # Clone the repository and install in editable mode
 git clone https://github.com/openvinotoolkit/anomalib.git
 cd anomalib
 pip install -e .
 ```
 
-This will install Anomalib CLI using the [installer](requirements/installer.txt) dependencies. Anomalib CLI is a command line interface for training, inference, benchmarking, and hyperparameter optimization. If you want to use the library as a Python package, you can install the library with the following command:
+This will install Anomalib CLI using the [dependencies](/pyproject.toml) in the `pyproject.toml` file. Anomalib CLI is a command line interface for training, inference, benchmarking, and hyperparameter optimization. If you want to use the library as a Python package, you can install the library with the following command:
 
 ```bash
 # Get help for the installation arguments
 anomalib install -h
 
 # Install the full package
 anomalib install
```

### Comparing `anomalib-1.0.1/pyproject.toml` & `anomalib-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -9,59 +9,84 @@
 dynamic = ["version"]
 readme = "README.md"
 description = "anomalib - Anomaly Detection Library"
 requires-python = ">=3.10"
 license = { file = "LICENSE" }
 authors = [{ name = "Intel OpenVINO" }]
 
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: Apache Software License",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Topic :: Software Development :: Libraries",
+    "Topic :: Scientific/Engineering :: Artificial Intelligence",
+]
+
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 # REQUIREMENTS                                                                #
 dependencies = [
     "omegaconf>=2.1.1",
     "rich>=13.5.2",
-    "jsonargparse==4.27.1",
+    "jsonargparse[signatures]>=4.27.7",
     "docstring_parser",     # CLI help-formatter
     "rich_argparse",        # CLI help-formatter
 ]
 
 [project.optional-dependencies]
 core = [
     "av>=10.0.0",
     "einops>=0.3.2",
     "freia>=0.2",
     "imgaug==0.4.0",
-    "kornia>=0.6.6,<0.6.10",
+    "kornia>=0.6.6",
     "matplotlib>=3.4.3",
     "opencv-python>=4.5.3.56",
     "pandas>=1.1.0",
-    "timm>=0.5.4,<=0.6.13",
-    "lightning>2,<2.2.0",
-    "torch>=2,<2.2.0",
+    "timm>=0.5.4,<=1.0.3",
+    "lightning>=2.2",
+    "torch>=2",
     "torchmetrics>=1.3.2",
     "open-clip-torch>=2.23.0",
 ]
-openvino = ["openvino-dev>=2023.0", "nncf>=2.5.0", "onnx>=1.16.0"]
+openvino = ["openvino>=2024.0", "nncf>=2.10.0", "onnx>=1.16.0"]
 loggers = [
     "comet-ml>=3.31.7",
     "gradio>=4",
     "tensorboard",
-    "wandb==0.12.17",
+    "wandb>=0.12.17,<=0.15.9",
+    "mlflow >=1.0.0",
 ]
 notebooks = ["gitpython", "ipykernel", "ipywidgets", "notebook"]
-dev = [
+docs = [
+    "myst-parser",
+    "nbsphinx",
+    "pandoc",
+    "sphinx<8.0",  # 7.0 breaks readthedocs builds.
+    "sphinx_autodoc_typehints",
+    "sphinx_book_theme",
+    "sphinx-copybutton",
+    "sphinx_design",
+]
+test = [
     "pre-commit",
     "pytest",
     "pytest-cov",
     "pytest-xdist",
     "pytest-mock",
     "pytest-sugar",
     "coverage[toml]",
     "tox",
 ]
 full = ["anomalib[core,openvino,loggers,notebooks]"]
+dev = ["anomalib[full,docs,test]"]
 
 [project.scripts]
 anomalib = "anomalib.cli.cli:main"
 
 [tool.setuptools.dynamic]
 version = { attr = "anomalib.__version__" }
 
@@ -189,16 +214,14 @@
 # Allow imports relative to the "src" and "tests" directories.
 src = ["src", "tests"]
 
 [tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 15
 
-[tool.ruff.per-file-ignores]
-"tests/nightly/tools/benchmarking/test_benchmarking.py" = ["E402"]
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 # MYPY CONFIGURATION.                                                         #
```

### Comparing `anomalib-1.0.1/src/anomalib/__init__.py` & `anomalib-1.1.0/src/anomalib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Anomalib library for research and benchmarking."""
 
 # Copyright (C) 2022-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
 from enum import Enum
 
-__version__ = "1.0.1"
+__version__ = "1.1.0"
 
 
 class LearningType(str, Enum):
     """Learning type defining how the model learns from the dataset samples."""
 
     ONE_CLASS = "one_class"
     ZERO_SHOT = "zero_shot"
```

### Comparing `anomalib-1.0.1/src/anomalib/callbacks/__init__.py` & `anomalib-1.1.0/src/anomalib/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/callbacks/checkpoint.py` & `anomalib-1.1.0/src/anomalib/callbacks/checkpoint.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/callbacks/graph.py` & `anomalib-1.1.0/src/anomalib/callbacks/graph.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/callbacks/metrics.py` & `anomalib-1.1.0/src/anomalib/callbacks/metrics.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/callbacks/model_loader.py` & `anomalib-1.1.0/src/anomalib/callbacks/model_loader.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/callbacks/nncf/callback.py` & `anomalib-1.1.0/src/anomalib/callbacks/nncf/callback.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/callbacks/nncf/utils.py` & `anomalib-1.1.0/src/anomalib/callbacks/nncf/utils.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/callbacks/normalization/base.py` & `anomalib-1.1.0/src/anomalib/callbacks/normalization/base.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/callbacks/normalization/min_max_normalization.py` & `anomalib-1.1.0/src/anomalib/callbacks/normalization/min_max_normalization.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/callbacks/normalization/utils.py` & `anomalib-1.1.0/src/anomalib/callbacks/normalization/utils.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/callbacks/post_processor.py` & `anomalib-1.1.0/src/anomalib/callbacks/post_processor.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/callbacks/thresholding.py` & `anomalib-1.1.0/src/anomalib/callbacks/thresholding.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/callbacks/tiler_configuration.py` & `anomalib-1.1.0/src/anomalib/callbacks/tiler_configuration.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/callbacks/timer.py` & `anomalib-1.1.0/src/anomalib/callbacks/timer.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/callbacks/visualizer.py` & `anomalib-1.1.0/src/anomalib/callbacks/visualizer.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/cli/cli.py` & `anomalib-1.1.0/src/anomalib/cli/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,38 +2,37 @@
 
 # Copyright (C) 2023-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
 import logging
 from collections.abc import Callable, Sequence
 from functools import partial
-from inspect import signature
 from pathlib import Path
 from types import MethodType
 from typing import Any
 
 from jsonargparse import ActionConfigFile, ArgumentParser, Namespace
 from jsonargparse._actions import _ActionSubCommands
 from rich import traceback
 
 from anomalib import TaskType, __version__
+from anomalib.cli.pipelines import PIPELINE_REGISTRY, pipeline_subcommands, run_pipeline
 from anomalib.cli.utils.help_formatter import CustomHelpFormatter, get_short_docstring
 from anomalib.cli.utils.openvino import add_openvino_export_arguments
 from anomalib.loggers import configure_logger
 
 traceback.install()
 logger = logging.getLogger("anomalib.cli")
 
 _LIGHTNING_AVAILABLE = True
 try:
     from lightning.pytorch import Trainer
     from torch.utils.data import DataLoader, Dataset
 
     from anomalib.data import AnomalibDataModule
-    from anomalib.data.predict import PredictDataset
     from anomalib.engine import Engine
     from anomalib.metrics.threshold import BaseThreshold
     from anomalib.models import AnomalyModule
     from anomalib.utils.config import update_config
 
 except ImportError:
     _LIGHTNING_AVAILABLE = False
@@ -48,25 +47,26 @@
     For more details, the reader could refer to PyTorch Lightning CLI
     documentation.
 
     ``save_config_kwargs`` is set to ``overwrite=True`` so that the
     ``SaveConfigCallback`` overwrites the config if it already exists.
     """
 
-    def __init__(self, args: Sequence[str] | None = None) -> None:
+    def __init__(self, args: Sequence[str] | None = None, run: bool = True) -> None:
         self.parser = self.init_parser()
         self.subcommand_parsers: dict[str, ArgumentParser] = {}
         self.subcommand_method_arguments: dict[str, list[str]] = {}
         self.add_subcommands()
         self.config = self.parser.parse_args(args=args)
         self.subcommand = self.config["subcommand"]
         if _LIGHTNING_AVAILABLE:
             self.before_instantiate_classes()
             self.instantiate_classes()
-        self._run_subcommand()
+        if run:
+            self._run_subcommand()
 
     def init_parser(self, **kwargs) -> ArgumentParser:
         """Method that instantiates the argument parser."""
         kwargs.setdefault("dump_header", [f"anomalib=={__version__}"])
         parser = ArgumentParser(formatter_class=CustomHelpFormatter, **kwargs)
         parser.add_argument(
             "-c",
@@ -128,14 +128,21 @@
                 subcommand,
                 sub_parser,
                 help=self.anomalib_subcommands()[subcommand]["description"],
             )
             # add arguments to subcommand
             getattr(self, f"add_{subcommand}_arguments")(sub_parser)
 
+        # Add pipeline subcommands
+        if PIPELINE_REGISTRY is not None:
+            for subcommand, value in pipeline_subcommands().items():
+                sub_parser = PIPELINE_REGISTRY[subcommand].get_parser()
+                self.subcommand_parsers[subcommand] = sub_parser
+                parser_subcommands.add_subcommand(subcommand, sub_parser, help=value["description"])
+
     def add_arguments_to_parser(self, parser: ArgumentParser) -> None:
         """Extend trainer's arguments to add engine arguments.
 
         .. note::
             Since ``Engine`` parameters are manually added, any change to the
             ``Engine`` class should be reflected manually.
         """
@@ -212,33 +219,38 @@
             "--data",
             type=Dataset | AnomalibDataModule | DataLoader | str | Path,
             required=True,
         )
         added = parser.add_method_arguments(
             Engine,
             "predict",
-            skip={"model", "dataloaders", "datamodule", "dataset"},
+            skip={"model", "dataloaders", "datamodule", "dataset", "data_path"},
         )
         self.subcommand_method_arguments["predict"] = added
         self.add_arguments_to_parser(parser)
 
     def add_export_arguments(self, parser: ArgumentParser) -> None:
         """Add export arguments to the parser."""
         self._add_default_arguments_to_parser(parser)
         self._add_trainer_arguments_to_parser(parser)
         parser.add_subclass_arguments(
             AnomalyModule,
             "model",
             fail_untyped=False,
             required=True,
         )
+        parser.add_argument(
+            "--data",
+            type=AnomalibDataModule,
+            required=False,
+        )
         added = parser.add_method_arguments(
             Engine,
             "export",
-            skip={"mo_args", "model"},
+            skip={"ov_args", "model", "datamodule"},
         )
         self.subcommand_method_arguments["export"] = added
         add_openvino_export_arguments(parser)
         self.add_arguments_to_parser(parser)
 
     def _set_install_subcommand(self, action_subcommand: _ActionSubCommands) -> None:
         sub_parser = ArgumentParser(formatter_class=CustomHelpFormatter)
@@ -263,16 +275,14 @@
             help="Install the full-package for anomalib.",
         )
 
     def before_instantiate_classes(self) -> None:
         """Modify the configuration to properly instantiate classes and sets up tiler."""
         subcommand = self.config["subcommand"]
         if subcommand in (*self.subcommands(), "train", "predict"):
-            if self.config["subcommand"] == "predict" and isinstance(self.config["predict"]["data"], str | Path):
-                self.config["predict"]["data"] = self._set_predict_dataloader_namespace(self.config["predict"]["data"])
             self.config[subcommand] = update_config(self.config[subcommand])
 
     def instantiate_classes(self) -> None:
         """Instantiate classes depending on the subcommand.
 
         For trainer related commands it instantiates all the model, datamodule and trainer classes.
         But for subcommands we do not want to instantiate any trainer specific classes such as datamodule, model, etc
@@ -349,14 +359,16 @@
 
             install_kwargs = self.config.get("install", {})
             anomalib_install(**install_kwargs)
         elif self.config["subcommand"] in (*self.subcommands(), "train", "export", "predict"):
             fn = getattr(self.engine, self.subcommand)
             fn_kwargs = self._prepare_subcommand_kwargs(self.subcommand)
             fn(**fn_kwargs)
+        elif PIPELINE_REGISTRY is not None and self.subcommand in pipeline_subcommands():
+            run_pipeline(self.config)
         else:
             self.config_init = self.parser.instantiate_classes(self.config)
             getattr(self, f"{self.subcommand}")()
 
     @property
     def fit(self) -> Callable:
         """Fit the model using engine's fit method."""
@@ -411,35 +423,14 @@
             scheduler_kwargs = {"instantiate": False, "fail_untyped": False, "skip": {"optimizer"}}
             parser.add_subclass_arguments(
                 baseclass=LRSchedulerTypeTuple,
                 nested_key="lr_scheduler",
                 **scheduler_kwargs,
             )
 
-    def _set_predict_dataloader_namespace(self, data_path: str | Path | Namespace) -> Namespace:
-        """Set the predict dataloader namespace.
-
-        If the argument is of type str or Path, then it is assumed to be the path to the prediction data and is
-        assigned to PredictDataset.
-
-        Args:
-            data_path (str | Path | Namespace): Path to the data.
-
-        Returns:
-            Namespace: Namespace containing the predict dataloader.
-        """
-        if isinstance(data_path, str | Path):
-            init_args = {key: value.default for key, value in signature(PredictDataset).parameters.items()}
-            init_args["path"] = data_path
-            data_path = Namespace(
-                class_path="anomalib.data.predict.PredictDataset",
-                init_args=Namespace(init_args),
-            )
-        return data_path
-
     def _add_default_arguments_to_parser(self, parser: ArgumentParser) -> None:
         """Adds default arguments to the parser."""
         parser.add_argument(
             "--seed_everything",
             type=bool | int,
             default=True,
             help=(
@@ -459,14 +450,16 @@
         }
         fn_kwargs["model"] = self.model
         if self.datamodule is not None:
             if isinstance(self.datamodule, AnomalibDataModule):
                 fn_kwargs["datamodule"] = self.datamodule
             elif isinstance(self.datamodule, DataLoader):
                 fn_kwargs["dataloaders"] = self.datamodule
+            elif isinstance(self.datamodule, Path | str):
+                fn_kwargs["data_path"] = self.datamodule
         return fn_kwargs
 
     def _parser(self, subcommand: str | None) -> ArgumentParser:
         if subcommand is None:
             return self.parser
         # return the subcommand parser for the subcommand passed
         return self.subcommand_parsers[subcommand]
```

### Comparing `anomalib-1.0.1/src/anomalib/cli/install.py` & `anomalib-1.1.0/src/anomalib/cli/install.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/cli/utils/help_formatter.py` & `anomalib-1.1.0/src/anomalib/cli/utils/help_formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,49 +2,50 @@
 
 # Copyright (C) 2023 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
 import argparse
 import re
 import sys
-from typing import TypeVar
 
 import docstring_parser
 from jsonargparse import DefaultHelpFormatter
 from rich.markdown import Markdown
 from rich.panel import Panel
 from rich_argparse import RichHelpFormatter
 
 REQUIRED_ARGUMENTS = {
     "train": {"model", "model.help", "data", "data.help", "ckpt_path", "config"},
     "fit": {"model", "model.help", "data", "data.help", "ckpt_path", "config"},
     "validate": {"model", "model.help", "data", "data.help", "ckpt_path", "config"},
     "test": {"model", "model.help", "data", "data.help", "ckpt_path", "config"},
     "predict": {"model", "model.help", "data", "data.help", "ckpt_path", "config"},
+    "export": {"model", "model.help", "export_type", "ckpt_path", "config"},
 }
 
 try:
     from anomalib.engine import Engine
 
     DOCSTRING_USAGE = {
         "train": Engine.train,
         "fit": Engine.fit,
         "validate": Engine.validate,
         "test": Engine.test,
         "predict": Engine.predict,
+        "export": Engine.export,
     }
 except ImportError:
     print("To use other subcommand using `anomalib install`")
 
 
-def get_short_docstring(component: TypeVar) -> str:
+def get_short_docstring(component: type) -> str:
     """Get the short description from the docstring.
 
     Args:
-        component (TypeVar): The component to get the docstring from
+        component (type): The component to get the docstring from
 
     Returns:
         str: The short description
     """
     if component.__doc__ is None:
         return ""
     docstring = docstring_parser.parse(component.__doc__)
```

### Comparing `anomalib-1.0.1/src/anomalib/cli/utils/installation.py` & `anomalib-1.1.0/src/anomalib/cli/utils/installation.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/cli/utils/openvino.py` & `anomalib-1.1.0/src/anomalib/cli/utils/openvino.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     get_common_cli_parser = None
 
 
 def add_openvino_export_arguments(parser: ArgumentParser) -> None:
     """Add OpenVINO arguments to parser under --mo key."""
     if get_common_cli_parser is not None:
         group = parser.add_argument_group("OpenVINO Model Optimizer arguments (optional)")
-        mo_parser = get_common_cli_parser()
+        ov_parser = get_common_cli_parser()
         # remove redundant keys from mo keys
-        for arg in mo_parser._actions:  # noqa: SLF001
+        for arg in ov_parser._actions:  # noqa: SLF001
             if arg.dest in ("help", "input_model", "output_dir"):
                 continue
-            group.add_argument(f"--mo_args.{arg.dest}", type=arg.type, default=arg.default, help=arg.help)
+            group.add_argument(f"--ov_args.{arg.dest}", type=arg.type, default=arg.default, help=arg.help)
     else:
         logger.info("OpenVINO is possibly not installed in the environment. Skipping adding it to parser.")
```

### Comparing `anomalib-1.0.1/src/anomalib/data/__init__.py` & `anomalib-1.1.0/src/anomalib/data/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Anomalib Datasets."""
 
 # Copyright (C) 2022-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
-
 import importlib
 import logging
 from enum import Enum
 from itertools import chain
 
 from omegaconf import DictConfig, ListConfig
 
@@ -25,28 +24,43 @@
 
 DataFormat = Enum(  # type: ignore[misc]
     "DataFormat",
     {i.name: i.value for i in chain(DepthDataFormat, ImageDataFormat, VideoDataFormat)},
 )
 
 
-def get_datamodule(config: DictConfig | ListConfig) -> AnomalibDataModule:
+class UnknownDatamoduleError(ModuleNotFoundError):
+    ...
+
+
+def get_datamodule(config: DictConfig | ListConfig | dict) -> AnomalibDataModule:
     """Get Anomaly Datamodule.
 
     Args:
-        config (DictConfig | ListConfig): Configuration of the anomaly model.
+        config (DictConfig | ListConfig | dict): Configuration of the anomaly model.
 
     Returns:
         PyTorch Lightning DataModule
     """
     logger.info("Loading the datamodule")
 
-    module = importlib.import_module(".".join(config.data.class_path.split(".")[:-1]))
-    dataclass = getattr(module, config.data.class_path.split(".")[-1])
-    init_args = {**config.data.get("init_args", {})}  # get dict
+    if isinstance(config, dict):
+        config = DictConfig(config)
+
+    try:
+        _config = config.data if "data" in config else config
+        if len(_config.class_path.split(".")) > 1:
+            module = importlib.import_module(".".join(_config.class_path.split(".")[:-1]))
+        else:
+            module = importlib.import_module("anomalib.data")
+    except ModuleNotFoundError as exception:
+        logger.exception(f"ModuleNotFoundError: {_config.class_path}")
+        raise UnknownDatamoduleError from exception
+    dataclass = getattr(module, _config.class_path.split(".")[-1])
+    init_args = {**_config.get("init_args", {})}  # get dict
     if "image_size" in init_args:
         init_args["image_size"] = to_tuple(init_args["image_size"])
 
     return dataclass(**init_args)
 
 
 __all__ = [
```

### Comparing `anomalib-1.0.1/src/anomalib/data/base/datamodule.py` & `anomalib-1.1.0/src/anomalib/data/base/datamodule.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # Copyright (C) 2022-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
 
 import logging
 from abc import ABC, abstractmethod
+from pathlib import Path
 from typing import TYPE_CHECKING, Any
 
 from lightning.pytorch import LightningDataModule
 from lightning.pytorch.trainer.states import TrainerFn
 from lightning.pytorch.utilities.types import EVAL_DATALOADERS, TRAIN_DATALOADERS
 from torch.utils.data.dataloader import DataLoader, default_collate
 from torchvision.transforms.v2 import Resize, Transform
@@ -98,14 +99,19 @@
         self.test_split_ratio = test_split_ratio
         self.val_split_mode = ValSplitMode(val_split_mode)
         self.val_split_ratio = val_split_ratio
         self.image_size = image_size
         self.seed = seed
 
         # set transforms
+        if bool(train_transform) != bool(eval_transform):
+            msg = "Only one of train_transform and eval_transform was specified. This is not recommended because \
+                    it could lead to unexpected behaviour. Please ensure training and eval transforms have the same \
+                    reshape and normalization characteristics."
+            logger.warning(msg)
         self._train_transform = train_transform or transform
         self._eval_transform = eval_transform or transform
 
         self.train_data: AnomalibDataset
         self.val_data: AnomalibDataset
         self.test_data: AnomalibDataset
 
@@ -251,16 +257,14 @@
 
         This property is accessed by the engine to set the transform for the model. The eval_transform takes precedence
         over the train_transform, because the transform that we store in the model is the one that should be used during
         inference.
         """
         if self._eval_transform:
             return self._eval_transform
-        if self._train_transform:
-            return self._train_transform
         return None
 
     @property
     def train_transform(self) -> Transform:
         """Get the transforms that will be passed to the train dataset.
 
         If the train_transform is not set, the engine will request the transform from the model.
@@ -282,7 +286,55 @@
         if self._eval_transform:
             return self._eval_transform
         if getattr(self, "trainer", None) and self.trainer.model and self.trainer.model.transform:
             return self.trainer.model.transform
         if self.image_size:
             return Resize(self.image_size, antialias=True)
         return None
+
+    @classmethod
+    def from_config(
+        cls: type["AnomalibDataModule"],
+        config_path: str | Path,
+        **kwargs,
+    ) -> "AnomalibDataModule":
+        """Create a datamodule instance from the configuration.
+
+        Args:
+            config_path (str | Path): Path to the data configuration file.
+            **kwargs (dict): Additional keyword arguments.
+
+        Returns:
+            AnomalibDataModule: Datamodule instance.
+
+        Example:
+            The following example shows how to get datamodule from mvtec.yaml:
+
+            .. code-block:: python
+                >>> data_config = "configs/data/mvtec.yaml"
+                >>> datamodule = AnomalibDataModule.from_config(config_path=data_config)
+
+            The following example shows overriding the configuration file with additional keyword arguments:
+
+            .. code-block:: python
+                >>> override_kwargs = {"data.train_batch_size": 8}
+                >>> datamodule = AnomalibDataModule.from_config(config_path=data_config, **override_kwargs)
+        """
+        from jsonargparse import ArgumentParser
+
+        if not Path(config_path).exists():
+            msg = f"Configuration file not found: {config_path}"
+            raise FileNotFoundError(msg)
+
+        data_parser = ArgumentParser()
+        data_parser.add_subclass_arguments(AnomalibDataModule, "data", required=False, fail_untyped=False)
+        args = ["--data", str(config_path)]
+        for key, value in kwargs.items():
+            args.extend([f"--{key}", str(value)])
+        config = data_parser.parse_args(args=args)
+        instantiated_classes = data_parser.instantiate_classes(config)
+        datamodule = instantiated_classes.get("data")
+        if isinstance(datamodule, AnomalibDataModule):
+            return datamodule
+
+        msg = f"Datamodule is not an instance of AnomalibDataModule: {datamodule}"
+        raise ValueError(msg)
```

### Comparing `anomalib-1.0.1/src/anomalib/data/base/dataset.py` & `anomalib-1.1.0/src/anomalib/data/base/dataset.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/data/base/depth.py` & `anomalib-1.1.0/src/anomalib/data/base/depth.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/data/base/video.py` & `anomalib-1.1.0/src/anomalib/data/base/video.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/data/depth/folder_3d.py` & `anomalib-1.1.0/src/anomalib/data/depth/folder_3d.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/data/depth/mvtec_3d.py` & `anomalib-1.1.0/src/anomalib/data/depth/mvtec_3d.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/data/errors.py` & `anomalib-1.1.0/src/anomalib/data/errors.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/data/image/__init__.py` & `anomalib-1.1.0/src/anomalib/data/image/__init__.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/data/image/btech.py` & `anomalib-1.1.0/src/anomalib/data/image/btech.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/data/image/folder.py` & `anomalib-1.1.0/src/anomalib/data/image/folder.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/data/image/kolektor.py` & `anomalib-1.1.0/src/anomalib/data/image/kolektor.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/data/image/mvtec.py` & `anomalib-1.1.0/src/anomalib/data/image/mvtec.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/data/image/visa.py` & `anomalib-1.1.0/src/anomalib/data/image/visa.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/data/predict.py` & `anomalib-1.1.0/src/anomalib/data/predict.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/data/transforms/center_crop.py` & `anomalib-1.1.0/src/anomalib/data/transforms/center_crop.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/data/utils/__init__.py` & `anomalib-1.1.0/src/anomalib/data/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/data/utils/augmenter.py` & `anomalib-1.1.0/src/anomalib/data/utils/augmenter.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/data/utils/boxes.py` & `anomalib-1.1.0/src/anomalib/data/utils/boxes.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/data/utils/download.py` & `anomalib-1.1.0/src/anomalib/data/utils/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,15 +226,17 @@
     Args:
         tar_file (TarFile): TarFile object.
         root (Path): Root directory where the dataset will be stored.
         members (List[TarInfo]): List of safe members to be extracted.
 
     """
     for member in members:
-        tar_file.extract(member, root)
+        # check if the file already exists
+        if not (root / member.name).exists():
+            tar_file.extract(member, root, filter="data")
 
 
 def generate_hash(file_path: str | Path, algorithm: str = "sha256") -> str:
     """Generate a hash of a file using the specified algorithm.
 
     Args:
         file_path (str | Path): Path to the file to hash.
@@ -284,15 +286,15 @@
     """Extract a dataset.
 
     Args:
         file_name (Path): Path of the file to be extracted.
         root (Path): Root directory where the dataset will be stored.
 
     """
-    logger.info("Extracting dataset into root folder.")
+    logger.info(f"Extracting dataset into {root} folder.")
 
     # Safely extract zip files
     if file_name.suffix == ".zip":
         with ZipFile(file_name, "r") as zip_file:
             for file_info in zip_file.infolist():
                 if not is_file_potentially_dangerous(file_info.filename):
                     zip_file.extract(file_info, root)
```

### Comparing `anomalib-1.0.1/src/anomalib/data/utils/generators/perlin.py` & `anomalib-1.1.0/src/anomalib/data/utils/generators/perlin.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/data/utils/image.py` & `anomalib-1.1.0/src/anomalib/data/utils/image.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/data/utils/path.py` & `anomalib-1.1.0/src/anomalib/data/utils/path.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/data/utils/split.py` & `anomalib-1.1.0/src/anomalib/data/utils/split.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/data/utils/synthetic.py` & `anomalib-1.1.0/src/anomalib/data/utils/synthetic.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/data/utils/tiler.py` & `anomalib-1.1.0/src/anomalib/data/utils/tiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,15 +374,15 @@
             image = image.unsqueeze(0)
 
         self.batch_size, self.num_channels, self.input_h, self.input_w = image.shape
 
         if self.input_h < self.tile_size_h or self.input_w < self.tile_size_w:
             msg = (
                 f"One of the edges of the tile size {self.tile_size_h, self.tile_size_w} is larger than "
-                f"that of the image {{self.input_h, self.input_w}}."
+                f"that of the image {self.input_h, self.input_w}."
             )
             raise ValueError(
                 msg,
             )
 
         self.resized_h, self.resized_w = compute_new_image_size(
             image_size=(self.input_h, self.input_w),
```

### Comparing `anomalib-1.0.1/src/anomalib/data/utils/video.py` & `anomalib-1.1.0/src/anomalib/data/utils/video.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/data/video/avenue.py` & `anomalib-1.1.0/src/anomalib/data/video/avenue.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/data/video/shanghaitech.py` & `anomalib-1.1.0/src/anomalib/data/video/shanghaitech.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/data/video/ucsd_ped.py` & `anomalib-1.1.0/src/anomalib/data/video/ucsd_ped.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/deploy/export.py` & `anomalib-1.1.0/src/anomalib/models/components/base/export_mixin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,359 +1,311 @@
-"""Utilities for optimization and OpenVINO conversion."""
+"""Mixin for exporting models to disk."""
 
-# Copyright (C) 2022-2024 Intel Corporation
+# Copyright (C) 2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
 
 import json
 import logging
-from enum import Enum
+from collections.abc import Callable
 from pathlib import Path
+from tempfile import TemporaryDirectory
 from typing import TYPE_CHECKING, Any
 
 import numpy as np
 import torch
 from torch import nn
-from torchvision.transforms.v2 import CenterCrop, Compose, Resize, Transform
+from torchvision.transforms.v2 import Transform
 
 from anomalib import TaskType
-from anomalib.data.transforms import ExportableCenterCrop
-from anomalib.models.components import AnomalyModule
+from anomalib.data import AnomalibDataModule
+from anomalib.deploy.export import CompressionType, ExportType, InferenceModel
 from anomalib.utils.exceptions import try_import
 
 if TYPE_CHECKING:
     from torch.types import Number
 
-logger = logging.getLogger("anomalib")
+logger = logging.getLogger(__name__)
 
-if try_import("openvino"):
-    from openvino.runtime import serialize
-    from openvino.tools.ovc import convert_model
-
-
-class ExportType(str, Enum):
-    """Model export type.
-
-    Examples:
-        >>> from anomalib.deploy import ExportType
-        >>> ExportType.ONNX
-        'onnx'
-        >>> ExportType.OPENVINO
-        'openvino'
-        >>> ExportType.TORCH
-        'torch'
-    """
-
-    ONNX = "onnx"
-    OPENVINO = "openvino"
-    TORCH = "torch"
-
-
-class InferenceModel(nn.Module):
-    """Inference model for export.
-
-    The InferenceModel is used to wrap the model and transform for exporting to torch and ONNX/OpenVINO.
-
-    Args:
-        model (nn.Module): Model to export.
-        transform (Transform): Input transform for the model.
-        disable_antialias (bool, optional): Disable antialiasing in the Resize transforms of the given transform. This
-            is needed for ONNX/OpenVINO export, as antialiasing is not supported in the ONNX opset.
-    """
-
-    def __init__(self, model: nn.Module, transform: Transform, disable_antialias: bool = False) -> None:
-        super().__init__()
-        self.model = model
-        self.transform = transform
-        self.convert_center_crop()
-        if disable_antialias:
-            self.disable_antialias()
-
-    def forward(self, batch: torch.Tensor) -> torch.Tensor | tuple[torch.Tensor, torch.Tensor]:
-        """Transform the input batch and pass it through the model."""
-        batch = self.transform(batch)
-        return self.model(batch)
 
-    def disable_antialias(self) -> None:
-        """Disable antialiasing in the Resize transforms of the given transform.
+class ExportMixin:
+    """This mixin allows exporting models to torch and ONNX/OpenVINO."""
 
-        This is needed for ONNX/OpenVINO export, as antialiasing is not supported in the ONNX opset.
+    model: nn.Module
+    transform: Transform
+    configure_transforms: Callable
+    device: torch.device
+
+    def to_torch(
+        self,
+        export_root: Path | str,
+        transform: Transform | None = None,
+        task: TaskType | None = None,
+    ) -> Path:
+        """Export AnomalibModel to torch.
+
+        Args:
+            export_root (Path): Path to the output folder.
+            transform (Transform, optional): Input transforms used for the model. If not provided, the transform is
+                taken from the model.
+                Defaults to ``None``.
+            task (TaskType | None): Task type.
+                Defaults to ``None``.
+
+        Returns:
+            Path: Path to the exported pytorch model.
+
+        Examples:
+            Assume that we have a model to train and we want to export it to torch format.
+
+            >>> from anomalib.data import Visa
+            >>> from anomalib.models import Patchcore
+            >>> from anomalib.engine import Engine
+            ...
+            >>> datamodule = Visa()
+            >>> model = Patchcore()
+            >>> engine = Engine()
+            ...
+            >>> engine.fit(model, datamodule)
+
+            Now that we have a model trained, we can export it to torch format.
+
+            >>> model.to_torch(
+            ...     export_root="path/to/export",
+            ...     transform=datamodule.test_data.transform,
+            ...     task=datamodule.test_data.task,
+            ... )
         """
-        if isinstance(self.transform, Resize):
-            self.transform.antialias = False
-        if isinstance(self.transform, Compose):
-            for transform in self.transform.transforms:
-                if isinstance(transform, Resize):
-                    transform.antialias = False
-
-    def convert_center_crop(self) -> None:
-        """Convert CenterCrop to ExportableCenterCrop for ONNX export.
-
-        The original CenterCrop transform is not supported in ONNX export. This method replaces the CenterCrop to
-        ExportableCenterCrop, which is supported in ONNX export. For more details, see the implementation of
-        ExportableCenterCrop.
+        transform = transform or self.transform or self.configure_transforms()
+        inference_model = InferenceModel(model=self.model, transform=transform)
+        export_root = _create_export_root(export_root, ExportType.TORCH)
+        metadata = self._get_metadata(task=task)
+        pt_model_path = export_root / "model.pt"
+        torch.save(
+            obj={"model": inference_model, "metadata": metadata},
+            f=pt_model_path,
+        )
+        return pt_model_path
+
+    def to_onnx(
+        self,
+        export_root: Path | str,
+        input_size: tuple[int, int] | None = None,
+        transform: Transform | None = None,
+        task: TaskType | None = None,
+    ) -> Path:
+        """Export model to onnx.
+
+        Args:
+            export_root (Path): Path to the root folder of the exported model.
+            input_size (tuple[int, int] | None, optional): Image size used as the input for onnx converter.
+                Defaults to None.
+            transform (Transform, optional): Input transforms used for the model. If not provided, the transform is
+                taken from the model.
+                Defaults to ``None``.
+            task (TaskType | None): Task type.
+                Defaults to ``None``.
+
+        Returns:
+            Path: Path to the exported onnx model.
+
+        Examples:
+            Export the Lightning Model to ONNX:
+
+            >>> from anomalib.models import Patchcore
+            >>> from anomalib.data import Visa
+            ...
+            >>> datamodule = Visa()
+            >>> model = Patchcore()
+            ...
+            >>> model.to_onnx(
+            ...     export_root="path/to/export",
+            ...     transform=datamodule.test_data.transform,
+            ...     task=datamodule.test_data.task
+            ... )
+
+            Using Custom Transforms:
+            This example shows how to use a custom ``Compose`` object for the ``transform`` argument.
+
+            >>> model.to_onnx(
+            ...     export_root="path/to/export",
+            ...     task="segmentation",
+            ... )
         """
-        if isinstance(self.transform, CenterCrop):
-            self.transform = ExportableCenterCrop(size=self.transform.size)
-        elif isinstance(self.transform, Compose):
-            transforms = self.transform.transforms
-            for index in range(len(transforms)):
-                if isinstance(transforms[index], CenterCrop):
-                    transforms[index] = ExportableCenterCrop(size=transforms[index].size)
-
-
-def export_to_torch(
-    model: AnomalyModule,
-    export_root: Path | str,
-    transform: Transform | None = None,
-    task: TaskType | None = None,
-) -> Path:
-    """Export AnomalibModel to torch.
-
-    Args:
-        model (AnomalyModule): Model to export.
-        export_root (Path): Path to the output folder.
-        transform (Transform, optional): Input transforms used for the model. If not provided, the transform is taken
-            from the model.
-            Defaults to ``None``.
-        task (TaskType | None): Task type.
-            Defaults to ``None``.
-
-    Returns:
-        Path: Path to the exported pytorch model.
-
-    Examples:
-        Assume that we have a model to train and we want to export it to torch format.
-
-        >>> from anomalib.data import Visa
-        >>> from anomalib.models import Patchcore
-        >>> from anomalib.engine import Engine
-        ...
-        >>> datamodule = Visa()
-        >>> model = Patchcore()
-        >>> engine = Engine()
-        ...
-        >>> engine.fit(model, datamodule)
-
-        Now that we have a model trained, we can export it to torch format.
-
-        >>> from anomalib.deploy import export_to_torch
-        ...
-        >>> export_to_torch(
-        ...     model=model,
-        ...     export_root="path/to/export",
-        ...     transform=datamodule.test_data.transform,
-        ...     task=datamodule.test_data.task,
-        ... )
-    """
-    transform = transform or model.transform or model.configure_transforms()
-    inference_model = InferenceModel(model=model.model, transform=transform)
-    export_root = _create_export_root(export_root, ExportType.TORCH)
-    metadata = get_metadata(task=task, model=model)
-    pt_model_path = export_root / "model.pt"
-    torch.save(
-        obj={"model": inference_model, "metadata": metadata},
-        f=pt_model_path,
-    )
-    return pt_model_path
-
-
-def export_to_onnx(
-    model: AnomalyModule,
-    export_root: Path | str,
-    transform: Transform | None = None,
-    task: TaskType | None = None,
-    export_type: ExportType = ExportType.ONNX,
-) -> Path:
-    """Export model to onnx.
-
-    Args:
-        model (AnomalyModule): Model to export.
-        export_root (Path): Path to the root folder of the exported model.
-        transform (Transform, optional): Input transforms used for the model. If not provided, the transform is taken
-            from the model.
-            Defaults to ``None``.
-        task (TaskType | None): Task type.
-            Defaults to ``None``.
-        export_type (ExportType): Mode to export the model. Since this method is used by OpenVINO export as well, we
-            need to pass the export type so that the right export path is created.
-            Defaults to ``ExportType.ONNX``.
-
-    Returns:
-        Path: Path to the exported onnx model.
-
-    Examples:
-        Export the Lightning Model to ONNX:
-
-        >>> from anomalib.models import Patchcore
-        >>> from anomalib.data import Visa
-        >>> from anomalib.deploy import export_to_onnx
-        ...
-        >>> datamodule = Visa()
-        >>> model = Patchcore()
-        ...
-        >>> export_to_onnx(
-        ...     model=model,
-        ...     export_root="path/to/export",
-        ...     transform=datamodule.test_data.transform,
-        ...     task=datamodule.test_data.task
-        ... )
-
-        Using Custom Transforms:
-        This example shows how to use a custom ``Compose`` object for the ``transform`` argument.
-
-        >>> export_to_onnx(
-        ...     model=model,
-        ...     export_root="path/to/export",
-        ...     task="segmentation",
-        ... )
-    """
-    # TODO(djdameln): Move export functionality to anomaly module
-    # https://github.com/openvinotoolkit/anomalib/issues/1752
-    transform = transform or model.transform or model.configure_transforms()
-    inference_model = InferenceModel(model=model.model, transform=transform, disable_antialias=True)
-    export_root = _create_export_root(export_root, export_type)
-    _write_metadata_to_json(export_root, model, task)
-    onnx_path = export_root / "model.onnx"
-    torch.onnx.export(
-        inference_model,
-        torch.zeros((1, 3, 1, 1)).to(model.device),
-        str(onnx_path),
-        opset_version=14,
-        dynamic_axes={"input": {0: "batch_size", 2: "height", 3: "weight"}, "output": {0: "batch_size"}},
-        input_names=["input"],
-        output_names=["output"],
-    )
-
-    return onnx_path
-
-
-def export_to_openvino(
-    export_root: Path | str,
-    model: AnomalyModule,
-    transform: Transform | None = None,
-    ov_args: dict[str, Any] | None = None,
-    task: TaskType | None = None,
-) -> Path:
-    """Convert onnx model to OpenVINO IR.
-
-    Args:
-        export_root (Path): Path to the export folder.
-        model (AnomalyModule): AnomalyModule to export.
-        transform (Transform, optional): Input transforms used for the model. If not provided, the transform is taken
-            from the model.
-            Defaults to ``None``.
-        ov_args: Model optimizer arguments for OpenVINO model conversion.
-            Defaults to ``None``.
-        task (TaskType | None): Task type.
-            Defaults to ``None``.
-
-    Returns:
-        Path: Path to the exported onnx model.
-
-    Raises:
-        ModuleNotFoundError: If OpenVINO is not installed.
-
-    Returns:
-        Path: Path to the exported OpenVINO IR.
-
-    Examples:
-        Export the Lightning Model to OpenVINO IR:
-        This example demonstrates how to export the Lightning Model to OpenVINO IR.
-
-        >>> from anomalib.models import Patchcore
-        >>> from anomalib.data import Visa
-        >>> from anomalib.deploy import export_to_openvino
-        ...
-        >>> datamodule = Visa()
-        >>> model = Patchcore()
-        ...
-        >>> export_to_openvino(
-        ...     export_root="path/to/export",
-        ...     model=model,
-        ...     input_size=(224, 224),
-        ...     transform=datamodule.test_data.transform,
-        ...     task=datamodule.test_data.task
-        ... )
-
-        Using Custom Transforms:
-        This example shows how to use a custom ``Transform`` object for the ``transform`` argument.
-
-        >>> from torchvision.transforms.v2 import Resize
-        >>> transform = Resize(224, 224)
-        ...
-        >>> export_to_openvino(
-        ...     export_root="path/to/export",
-        ...     model=model,
-        ...     transform=transform,
-        ...     task="segmentation",
-        ... )
-
-    """
-    model_path = export_to_onnx(model, export_root, transform, task, ExportType.OPENVINO)
-    ov_model_path = model_path.with_suffix(".xml")
-    ov_args = {} if ov_args is None else ov_args
-    if convert_model is not None and serialize is not None:
-        model = convert_model(model_path, **ov_args)
-        serialize(model, ov_model_path)
-    else:
-        logger.exception("Could not find OpenVINO methods. Please check OpenVINO installation.")
-        raise ModuleNotFoundError
-    return ov_model_path
-
-
-def get_metadata(
-    model: AnomalyModule,
-    task: TaskType | None = None,
-) -> dict[str, Any]:
-    """Get metadata for the exported model.
-
-    Args:
-        model (AnomalyModule): Anomaly model which contains metadata related to normalization.
-        task (TaskType | None): Task type.
-            Defaults to None.
-
-    Returns:
-        dict[str, Any]: Metadata for the exported model.
-    """
-    data_metadata = {"task": task}
-    model_metadata = _get_model_metadata(model)
-    metadata = {**data_metadata, **model_metadata}
+        transform = transform or self.transform or self.configure_transforms()
+        inference_model = InferenceModel(model=self.model, transform=transform, disable_antialias=True)
+        export_root = _create_export_root(export_root, ExportType.ONNX)
+        input_shape = torch.zeros((1, 3, *input_size)) if input_size else torch.zeros((1, 3, 1, 1))
+        dynamic_axes = (
+            None if input_size else {"input": {0: "batch_size", 2: "height", 3: "weight"}, "output": {0: "batch_size"}}
+        )
+        _write_metadata_to_json(self._get_metadata(task), export_root)
+        onnx_path = export_root / "model.onnx"
+        torch.onnx.export(
+            inference_model,
+            input_shape.to(self.device),
+            str(onnx_path),
+            opset_version=14,
+            dynamic_axes=dynamic_axes,
+            input_names=["input"],
+            output_names=["output"],
+        )
+
+        return onnx_path
+
+    def to_openvino(
+        self,
+        export_root: Path | str,
+        input_size: tuple[int, int] | None = None,
+        transform: Transform | None = None,
+        compression_type: CompressionType | None = None,
+        datamodule: AnomalibDataModule | None = None,
+        ov_args: dict[str, Any] | None = None,
+        task: TaskType | None = None,
+    ) -> Path:
+        """Convert onnx model to OpenVINO IR.
+
+        Args:
+            export_root (Path): Path to the export folder.
+            input_size (tuple[int, int] | None, optional): Input size of the model. Used for adding metadata to the IR.
+                Defaults to None.
+            transform (Transform, optional): Input transforms used for the model. If not provided, the transform is
+                taken from the model.
+                Defaults to ``None``.
+            compression_type (CompressionType, optional): Compression type for better inference performance.
+                Defaults to ``None``.
+            datamodule (AnomalibDataModule | None, optional): Lightning datamodule.
+                Must be provided if CompressionType.INT8_PTQ is selected.
+                Defaults to ``None``.
+            ov_args (dict | None): Model optimizer arguments for OpenVINO model conversion.
+                Defaults to ``None``.
+            task (TaskType | None): Task type.
+                Defaults to ``None``.
+
+        Returns:
+            Path: Path to the exported onnx model.
+
+        Raises:
+            ModuleNotFoundError: If OpenVINO is not installed.
+
+        Returns:
+            Path: Path to the exported OpenVINO IR.
+
+        Examples:
+            Export the Lightning Model to OpenVINO IR:
+            This example demonstrates how to export the Lightning Model to OpenVINO IR.
+
+            >>> from anomalib.models import Patchcore
+            >>> from anomalib.data import Visa
+            ...
+            >>> datamodule = Visa()
+            >>> model = Patchcore()
+            ...
+            >>> model.to_openvino(
+            ...     export_root="path/to/export",
+            ...     transform=datamodule.test_data.transform,
+            ...     task=datamodule.test_data.task
+            ... )
+
+            Using Custom Transforms:
+            This example shows how to use a custom ``Transform`` object for the ``transform`` argument.
+
+            >>> from torchvision.transforms.v2 import Resize
+            >>> transform = Resize(224, 224)
+            ...
+            >>> model.to_openvino(
+            ...     export_root="path/to/export",
+            ...     transform=transform,
+            ...     task="segmentation",
+            ... )
+        """
+        if not try_import("openvino"):
+            logger.exception("Could not find OpenVINO. Please check OpenVINO installation.")
+            raise ModuleNotFoundError
+        if not try_import("nncf"):
+            logger.exception("Could not find NNCF. Please check NNCF installation.")
+            raise ModuleNotFoundError
+
+        import nncf
+        import openvino as ov
+
+        with TemporaryDirectory() as onnx_directory:
+            model_path = self.to_onnx(onnx_directory, input_size, transform, task)
+            export_root = _create_export_root(export_root, ExportType.OPENVINO)
+            ov_model_path = export_root / "model.xml"
+            ov_args = {} if ov_args is None else ov_args
+
+            model = ov.convert_model(model_path, **ov_args)
+            if compression_type == CompressionType.INT8:
+                model = nncf.compress_weights(model)
+            elif compression_type == CompressionType.INT8_PTQ:
+                if datamodule is None:
+                    msg = "Datamodule must be provided for OpenVINO INT8_PTQ compression"
+                    raise ValueError(msg)
+
+                dataloader = datamodule.val_dataloader()
+                if len(dataloader.dataset) < 300:
+                    logger.warning(
+                        f">300 images recommended for INT8 quantization, found only {len(dataloader.dataset)} images",
+                    )
+                calibration_dataset = nncf.Dataset(dataloader, lambda x: x["image"])
+                model = nncf.quantize(model, calibration_dataset)
+
+            # fp16 compression is enabled by default
+            compress_to_fp16 = compression_type == CompressionType.FP16
+            ov.save_model(model, ov_model_path, compress_to_fp16=compress_to_fp16)
+            _write_metadata_to_json(self._get_metadata(task), export_root)
+
+        return ov_model_path
+
+    def _get_metadata(
+        self,
+        task: TaskType | None = None,
+    ) -> dict[str, Any]:
+        """Get metadata for the exported model.
+
+        Args:
+            task (TaskType | None): Task type.
+                Defaults to None.
 
-    # Convert torch tensors to python lists or values for json serialization.
-    for key, value in metadata.items():
-        if isinstance(value, torch.Tensor):
-            metadata[key] = value.numpy().tolist()
+        Returns:
+            dict[str, Any]: Metadata for the exported model.
+        """
+        model_metadata = {}
+        cached_metadata: dict[str, Number | torch.Tensor] = {}
+        for threshold_name in ("image_threshold", "pixel_threshold"):
+            if hasattr(self, threshold_name):
+                cached_metadata[threshold_name] = getattr(self, threshold_name).cpu().value.item()
+        if hasattr(self, "normalization_metrics") and self.normalization_metrics.state_dict() is not None:
+            for key, value in self.normalization_metrics.state_dict().items():
+                cached_metadata[key] = value.cpu()
+        # Remove undefined values by copying in a new dict
+        for key, val in cached_metadata.items():
+            if not np.isinf(val).all():
+                model_metadata[key] = val
+        del cached_metadata
+        metadata = {"task": task, **model_metadata}
+
+        # Convert torch tensors to python lists or values for json serialization.
+        for key, value in metadata.items():
+            if isinstance(value, torch.Tensor):
+                metadata[key] = value.numpy().tolist()
 
-    return metadata
+        return metadata
 
 
-def _get_model_metadata(model: AnomalyModule) -> dict[str, torch.Tensor]:
-    """Get meta data related to normalization from model.
+def _write_metadata_to_json(metadata: dict[str, Any], export_root: Path) -> None:
+    """Write metadata to json file.
 
     Args:
-        model (AnomalyModule): Anomaly model which contains metadata related to normalization.
-
-    Returns:
-        dict[str, torch.Tensor]: Model metadata
+        metadata (dict[str, Any]): Metadata to export.
+        export_root (Path): Path to the exported model.
     """
-    metadata = {}
-    cached_metadata: dict[str, Number | torch.Tensor] = {}
-    for threshold_name in ("image_threshold", "pixel_threshold"):
-        if hasattr(model, threshold_name):
-            cached_metadata[threshold_name] = getattr(model, threshold_name).cpu().value.item()
-    if hasattr(model, "normalization_metrics") and model.normalization_metrics.state_dict() is not None:
-        for key, value in model.normalization_metrics.state_dict().items():
-            cached_metadata[key] = value.cpu()
-    # Remove undefined values by copying in a new dict
-    for key, val in cached_metadata.items():
-        if not np.isinf(val).all():
-            metadata[key] = val
-    del cached_metadata
-    return metadata
+    with (export_root / "metadata.json").open("w", encoding="utf-8") as metadata_file:
+        json.dump(metadata, metadata_file, ensure_ascii=False, indent=4)
 
 
 def _create_export_root(export_root: str | Path, export_type: ExportType) -> Path:
     """Create export directory.
 
     Args:
         export_root (str | Path): Path to the root folder of the exported model.
@@ -361,27 +313,7 @@
 
     Returns:
         Path: Path to the export directory.
     """
     export_root = Path(export_root) / "weights" / export_type.value
     export_root.mkdir(parents=True, exist_ok=True)
     return export_root
-
-
-def _write_metadata_to_json(
-    export_root: Path,
-    model: AnomalyModule,
-    task: TaskType | None = None,
-) -> None:
-    """Write metadata to json file.
-
-    Args:
-        export_root (Path): Path to the exported model.
-        transform (dict[str, Any] | AnomalibDataset | AnomalibDataModule | A.Compose): Data transforms (augmentations)
-            used for the model.
-        model (AnomalyModule): AnomalyModule to export.
-        task (TaskType | None): Task type.
-            Defaults to None.
-    """
-    metadata = get_metadata(task=task, model=model)
-    with (export_root / "metadata.json").open("w", encoding="utf-8") as metadata_file:
-        json.dump(metadata, metadata_file, ensure_ascii=False, indent=4)
```

### Comparing `anomalib-1.0.1/src/anomalib/deploy/inferencers/base_inferencer.py` & `anomalib-1.1.0/src/anomalib/deploy/inferencers/base_inferencer.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/deploy/inferencers/openvino_inferencer.py` & `anomalib-1.1.0/src/anomalib/deploy/inferencers/openvino_inferencer.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 from anomalib.utils.visualization import ImageResult
 
 from .base_inferencer import Inferencer
 
 logger = logging.getLogger("anomalib")
 
 if find_spec("openvino") is not None:
-    import openvino.runtime as ov
+    import openvino as ov
 
     if TYPE_CHECKING:
-        from openvino.runtime import CompiledModel
+        from openvino import CompiledModel
 else:
     logger.warning("OpenVINO is not installed. Please install OpenVINO to use OpenVINOInferencer.")
 
 
 class OpenVINOInferencer(Inferencer):
     """OpenVINO implementation for the inference.
 
@@ -195,14 +195,18 @@
         # Convert PIL image to numpy array
         if isinstance(image, Image.Image):
             image = np.array(image, dtype=np.float32)
         if not isinstance(image, np.ndarray):
             msg = f"Input image must be a numpy array or a path to an image. Got {type(image)}"
             raise TypeError(msg)
 
+        # Resize image to model input size if not dynamic
+        if self.input_blob.partial_shape[2].is_static and self.input_blob.partial_shape[3].is_static:
+            image = cv2.resize(image, tuple(list(self.input_blob.shape)[2:][::-1]))
+
         # Normalize numpy array to range [0, 1]
         if image.dtype != np.float32:
             image = image.astype(np.float32)
         if image.max() > 1.0:
             image /= 255.0
 
         # Check if metadata is provided, if not use the default metadata.
```

### Comparing `anomalib-1.0.1/src/anomalib/deploy/inferencers/torch_inferencer.py` & `anomalib-1.1.0/src/anomalib/deploy/inferencers/torch_inferencer.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,19 +263,19 @@
                 pred_score = predictions["pred_score"].detach().cpu().numpy()
             else:
                 pred_score = anomaly_map.reshape(-1).max()
 
         # Case III: Predictions could be a list of tensors.
         elif isinstance(predictions, Sequence):
             if isinstance(predictions[1], (torch.Tensor)):
-                anomaly_map, pred_score = predictions
+                pred_score, anomaly_map = predictions
                 anomaly_map = anomaly_map.detach().cpu().numpy()
                 pred_score = pred_score.detach().cpu().numpy()
             else:
-                anomaly_map, pred_score = predictions
+                pred_score, anomaly_map = predictions
                 pred_score = pred_score.detach()
         else:
             msg = (
                 f"Unknown prediction type {type(predictions)}. "
                 "Expected torch.Tensor, list[torch.Tensor] or dict[str, torch.Tensor]."
             )
             raise TypeError(msg)
```

### Comparing `anomalib-1.0.1/src/anomalib/engine/engine.py` & `anomalib-1.1.0/src/anomalib/engine/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import logging
 from collections.abc import Iterable
 from pathlib import Path
 from typing import Any
 
 import torch
-from lightning.pytorch.callbacks import Callback
+from lightning.pytorch.callbacks import Callback, RichModelSummary, RichProgressBar
 from lightning.pytorch.loggers import Logger
 from lightning.pytorch.trainer import Trainer
 from lightning.pytorch.utilities.types import _EVALUATE_OUTPUT, _PREDICT_OUTPUT, EVAL_DATALOADERS, TRAIN_DATALOADERS
 from torch.utils.data import DataLoader, Dataset
 from torchvision.transforms.v2 import Transform
 
 from anomalib import LearningType, TaskType
@@ -22,15 +22,15 @@
 from anomalib.callbacks.normalization import get_normalization_callback
 from anomalib.callbacks.normalization.base import NormalizationCallback
 from anomalib.callbacks.post_processor import _PostProcessorCallback
 from anomalib.callbacks.thresholding import _ThresholdCallback
 from anomalib.callbacks.timer import TimerCallback
 from anomalib.callbacks.visualizer import _VisualizationCallback
 from anomalib.data import AnomalibDataModule, AnomalibDataset, PredictDataset
-from anomalib.deploy.export import ExportType, export_to_onnx, export_to_openvino, export_to_torch
+from anomalib.deploy import CompressionType, ExportType
 from anomalib.models import AnomalyModule
 from anomalib.utils.normalization import NormalizationMethod
 from anomalib.utils.path import create_versioned_dir
 from anomalib.utils.types import NORMALIZATION, THRESHOLD
 from anomalib.utils.visualization import ImageVisualizer
 
 logger = logging.getLogger(__name__)
@@ -221,14 +221,36 @@
             msg = (
                 f"Trainer can only have one thresholding callback but multiple found: {callbacks}. "
                 "Please check your configuration. Exiting to avoid unexpected behavior."
             )
             raise ValueError(msg)
         return callbacks[0] if len(callbacks) > 0 else None
 
+    @property
+    def checkpoint_callback(self) -> ModelCheckpoint | None:
+        """The ``ModelCheckpoint`` callback in the trainer.callbacks list, or ``None`` if it doesn't exist.
+
+        Returns:
+            ModelCheckpoint | None: ModelCheckpoint callback, if available.
+        """
+        if self._trainer is None:
+            return None
+        return self.trainer.checkpoint_callback
+
+    @property
+    def best_model_path(self) -> str | None:
+        """The path to the best model checkpoint.
+
+        Returns:
+            str: Path to the best model checkpoint.
+        """
+        if self.checkpoint_callback is None:
+            return None
+        return self.checkpoint_callback.best_model_path
+
     def _setup_workspace(
         self,
         model: AnomalyModule,
         train_dataloaders: TRAIN_DATALOADERS | None = None,
         val_dataloaders: EVAL_DATALOADERS | None = None,
         test_dataloaders: EVAL_DATALOADERS | None = None,
         datamodule: AnomalibDataModule | None = None,
@@ -380,15 +402,15 @@
         if dataloaders:
             for dataloader in dataloaders:
                 if not getattr(dataloader.dataset, "transform", None):
                     dataloader.dataset.transform = transform
 
     def _setup_anomalib_callbacks(self) -> None:
         """Set up callbacks for the trainer."""
-        _callbacks: list[Callback] = []
+        _callbacks: list[Callback] = [RichProgressBar(), RichModelSummary()]
 
         # Add ModelCheckpoint if it is not in the callbacks list.
         has_checkpoint_callback = any(isinstance(c, ModelCheckpoint) for c in self._cache.args["callbacks"])
         if has_checkpoint_callback is False:
             _callbacks.append(
                 ModelCheckpoint(
                     dirpath=self._cache.args["default_root_dir"] / "weights" / "lightning",
@@ -668,14 +690,15 @@
         self,
         model: AnomalyModule | None = None,
         dataloaders: EVAL_DATALOADERS | None = None,
         datamodule: AnomalibDataModule | None = None,
         dataset: Dataset | PredictDataset | None = None,
         return_predictions: bool | None = None,
         ckpt_path: str | Path | None = None,
+        data_path: str | Path | None = None,
     ) -> _PREDICT_OUTPUT | None:
         """Predict using the model using the trainer.
 
         Sets up the trainer and the dataset task if not already set up. Then validates the model if needed and a
         validation dataloader is available. Finally, predicts using the model.
 
         Args:
@@ -699,14 +722,17 @@
                 Defaults to None.
             ckpt_path (str | None, optional):
                 Either ``"best"``, ``"last"``, ``"hpc"`` or path to the checkpoint you wish to predict.
                 If ``None`` and the model instance was passed, use the current weights.
                 Otherwise, the best model checkpoint from the previous ``trainer.fit`` call will be loaded
                 if a checkpoint callback is configured.
                 Defaults to None.
+            data_path (str | Path | None):
+                Path to the image or folder containing images to generate predictions for.
+                Defaults to None.
 
         Returns:
             _PREDICT_OUTPUT | None: Predictions.
 
         CLI Usage:
             1. you can pick a model.
                 ```python
@@ -739,26 +765,27 @@
 
         if model:
             self._setup_trainer(model)
 
         if not ckpt_path:
             logger.warning("ckpt_path is not provided. Model weights will not be loaded.")
 
-        # Handle the instance when a dataset is passed to the predict method
+        # Collect dataloaders
+        if dataloaders is None:
+            dataloaders = []
+        elif isinstance(dataloaders, DataLoader):
+            dataloaders = [dataloaders]
+        elif not isinstance(dataloaders, list):
+            msg = f"Unknown type for dataloaders {type(dataloaders)}"
+            raise TypeError(msg)
         if dataset is not None:
-            dataloader = DataLoader(dataset)
-            if dataloaders is None:
-                dataloaders = dataloader
-            elif isinstance(dataloaders, DataLoader):
-                dataloaders = [dataloaders, dataloader]
-            elif isinstance(dataloaders, list):  # dataloader is a list
-                dataloaders.append(dataloader)
-            else:
-                msg = f"Unknown type for dataloaders {type(dataloaders)}"
-                raise TypeError(msg)
+            dataloaders.append(DataLoader(dataset))
+        if data_path is not None:
+            dataloaders.append(DataLoader(PredictDataset(data_path)))
+        dataloaders = dataloaders or None
 
         self._setup_dataset_task(dataloaders, datamodule)
         self._setup_transform(model or self.model, datamodule=datamodule, dataloaders=dataloaders, ckpt_path=ckpt_path)
 
         if self._should_run_validation(model or self.model, None, datamodule, ckpt_path):
             logger.info("Running validation before predicting to collect normalization metrics and/or thresholds.")
             self.trainer.validate(
@@ -834,89 +861,153 @@
         else:
             self.trainer.fit(model, train_dataloaders, val_dataloaders, datamodule, ckpt_path)
         self.trainer.test(model, test_dataloaders, ckpt_path=ckpt_path, datamodule=datamodule)
 
     def export(
         self,
         model: AnomalyModule,
-        export_type: ExportType,
+        export_type: ExportType | str,
         export_root: str | Path | None = None,
+        input_size: tuple[int, int] | None = None,
         transform: Transform | None = None,
+        compression_type: CompressionType | None = None,
+        datamodule: AnomalibDataModule | None = None,
         ov_args: dict[str, Any] | None = None,
         ckpt_path: str | Path | None = None,
     ) -> Path | None:
-        """Export the model in PyTorch, ONNX or OpenVINO format.
+        r"""Export the model in PyTorch, ONNX or OpenVINO format.
 
         Args:
             model (AnomalyModule): Trained model.
             export_type (ExportType): Export type.
             export_root (str | Path | None, optional): Path to the output directory. If it is not set, the model is
                 exported to trainer.default_root_dir. Defaults to None.
+            input_size (tuple[int, int] | None, optional): A statis input shape for the model, which is exported to ONNX
+                and OpenVINO format. Defaults to None.
             transform (Transform | None, optional): Input transform to include in the exported model. If not provided,
-                the engine will try to use the transform from the datamodule or dataset. Defaults to None.
+                the engine will try to use the default transform from the model.
+                Defaults to ``None``.
+            compression_type (CompressionType | None, optional): Compression type for OpenVINO exporting only.
+                Defaults to ``None``.
+            datamodule (AnomalibDataModule | None, optional): Lightning datamodule.
+                Must be provided if CompressionType.INT8_PTQ is selected.
+                Defaults to ``None``.
             ov_args (dict[str, Any] | None, optional): This is optional and used only for OpenVINO's model optimizer.
                 Defaults to None.
             ckpt_path (str | Path | None): Checkpoint path. If provided, the model will be loaded from this path.
 
         Returns:
             Path: Path to the exported model.
 
         Raises:
             ValueError: If Dataset, Datamodule, and transform are not provided.
             TypeError: If path to the transform file is not a string or Path.
 
         CLI Usage:
             1. To export as a torch ``.pt`` file you can run the following command.
                 ```python
-                anomalib export --model Padim --export_mode TORCH --data MVTec
+                anomalib export --model Padim --export_mode torch --ckpt_path <PATH_TO_CHECKPOINT>
                 ```
             2. To export as an ONNX ``.onnx`` file you can run the following command.
                 ```python
-                anomalib export --model Padim --export_mode ONNX --data Visa --input_size "[256,256]"
+                anomalib export --model Padim --export_mode onnx --ckpt_path <PATH_TO_CHECKPOINT> \
+                --input_size "[256,256]"
                 ```
             3. To export as an OpenVINO ``.xml`` and ``.bin`` file you can run the following command.
                 ```python
-                anomalib export --model Padim --export_mode OPENVINO --data Visa --input_size "[256,256]"
+                anomalib export --model Padim --export_mode openvino --ckpt_path <PATH_TO_CHECKPOINT> \
+                --input_size "[256,256]"
                 ```
-            4. You can also overrride OpenVINO model optimizer by adding the ``--mo_args.<key>`` arguments.
+            4. You can also override OpenVINO model optimizer by adding the ``--ov_args.<key>`` arguments.
                 ```python
-                anomalib export --model Padim --export_mode OPENVINO --data Visa --input_size "[256,256]" \
-                    --mo_args.compress_to_fp16 False
+                anomalib export --model Padim --export_mode openvino --ckpt_path <PATH_TO_CHECKPOINT> \
+                --input_size "[256,256]" --ov_args.compress_to_fp16 False
                 ```
         """
+        export_type = ExportType(export_type)
         self._setup_trainer(model)
         if ckpt_path:
             ckpt_path = Path(ckpt_path).resolve()
             model = model.__class__.load_from_checkpoint(ckpt_path)
 
         if export_root is None:
             export_root = Path(self.trainer.default_root_dir)
 
         exported_model_path: Path | None = None
         if export_type == ExportType.TORCH:
-            exported_model_path = export_to_torch(
-                model=model,
+            exported_model_path = model.to_torch(
                 export_root=export_root,
                 transform=transform,
                 task=self.task,
             )
         elif export_type == ExportType.ONNX:
-            exported_model_path = export_to_onnx(
-                model=model,
+            exported_model_path = model.to_onnx(
                 export_root=export_root,
+                input_size=input_size,
                 transform=transform,
                 task=self.task,
             )
         elif export_type == ExportType.OPENVINO:
-            exported_model_path = export_to_openvino(
-                model=model,
+            exported_model_path = model.to_openvino(
                 export_root=export_root,
+                input_size=input_size,
                 transform=transform,
                 task=self.task,
+                compression_type=compression_type,
+                datamodule=datamodule,
                 ov_args=ov_args,
             )
         else:
             logging.error(f"Export type {export_type} is not supported yet.")
 
         if exported_model_path:
             logging.info(f"Exported model to {exported_model_path}")
         return exported_model_path
+
+    @classmethod
+    def from_config(
+        cls: type["Engine"],
+        config_path: str | Path,
+        **kwargs,
+    ) -> tuple["Engine", AnomalyModule, AnomalibDataModule]:
+        """Create an Engine instance from a configuration file.
+
+        Args:
+            config_path (str | Path): Path to the full configuration file.
+            **kwargs (dict): Additional keyword arguments.
+
+        Returns:
+            tuple[Engine, AnomalyModule, AnomalibDataModule]: Engine instance.
+
+        Example:
+            The following example shows training with full configuration file:
+
+            .. code-block:: python
+                >>> config_path = "anomalib_full_config.yaml"
+                >>> engine, model, datamodule = Engine.from_config(config_path=config_path)
+                >>> engine.fit(datamodule=datamodule, model=model)
+
+            The following example shows overriding the configuration file with additional keyword arguments:
+
+            .. code-block:: python
+                >>> override_kwargs = {"data.train_batch_size": 8}
+                >>> engine, model, datamodule = Engine.from_config(config_path=config_path, **override_kwargs)
+                >>> engine.fit(datamodule=datamodule, model=model)
+        """
+        from anomalib.cli.cli import AnomalibCLI
+
+        if not Path(config_path).exists():
+            msg = f"Configuration file not found: {config_path}"
+            raise FileNotFoundError(msg)
+
+        args = [
+            "fit",
+            "--config",
+            str(config_path),
+        ]
+        for key, value in kwargs.items():
+            args.extend([f"--{key}", str(value)])
+        anomalib_cli = AnomalibCLI(
+            args=args,
+            run=False,
+        )
+        return anomalib_cli.engine, anomalib_cli.model, anomalib_cli.datamodule
```

### Comparing `anomalib-1.0.1/src/anomalib/loggers/__init__.py` & `anomalib-1.1.0/src/anomalib/loggers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,22 +11,24 @@
 __all__ = [
     "configure_logger",
     "get_experiment_logger",
 ]
 
 try:
     from .comet import AnomalibCometLogger  # noqa: F401
+    from .mlflow import AnomalibMLFlowLogger  # noqa: F401
     from .tensorboard import AnomalibTensorBoardLogger  # noqa: F401
     from .wandb import AnomalibWandbLogger  # noqa: F401
 
     __all__.extend(
         [
             "AnomalibCometLogger",
             "AnomalibTensorBoardLogger",
             "AnomalibWandbLogger",
+            "AnomalibMLFlowLogger",
         ],
     )
 except ImportError:
     print("To use any logger install it using `anomalib install -v`")
 
 
 def configure_logger(level: int | str = logging.INFO) -> None:
```

### Comparing `anomalib-1.0.1/src/anomalib/loggers/base.py` & `anomalib-1.1.0/src/anomalib/loggers/base.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/loggers/comet.py` & `anomalib-1.1.0/src/anomalib/loggers/comet.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/loggers/tensorboard.py` & `anomalib-1.1.0/src/anomalib/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/loggers/wandb.py` & `anomalib-1.1.0/src/anomalib/loggers/wandb.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """wandb logger with add image interface."""
 
 # Copyright (C) 2022-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
+from typing import TYPE_CHECKING, Literal
 
 import numpy as np
+from lightning.fabric.utilities.types import _PATH
 from lightning.pytorch.loggers.wandb import WandbLogger
 from lightning.pytorch.utilities import rank_zero_only
 from matplotlib.figure import Figure
 
 from anomalib.utils.exceptions import try_import
 
+from .base import ImageLoggerBase
+
 if try_import("wandb"):
     import wandb
 
-from typing import TYPE_CHECKING
-
-from .base import ImageLoggerBase
-
 if TYPE_CHECKING:
     from wandb.sdk.lib import RunDisabled
-    from wandb.wandb_run import Run
+    from wandb.sdk.wandb_run import Run
 
 
 class AnomalibWandbLogger(ImageLoggerBase, WandbLogger):
     """Logger for wandb.
 
     Adds interface for `add_image` in the logger rather than calling the experiment object.
 
@@ -40,16 +40,18 @@
         $ pip install wandb
 
     Args:
         name: Display name for the run.
             Defaults to ``None``.
         save_dir: Path where data is saved (wandb dir by default).
             Defaults to ``None``.
+        version: Sets the version, mainly used to resume a previous run.
         offline: Run offline (data can be streamed later to wandb servers).
             Defaults to ``False``.
+        dir: Alias for save_dir.
         id: Sets the version, mainly used to resume a previous run.
             Defaults to ``None``.
         anonymous: Enables or explicitly disables anonymous logging.
             Defaults to ``None``.
         version: Same as id.
             Defaults to ``None``.
         project: The name of the project to which this run will belong.
@@ -85,36 +87,40 @@
         - `W&B Documentation <https://docs.wandb.ai/integrations/lightning>`__
 
     """
 
     def __init__(
         self,
         name: str | None = None,
-        save_dir: str | None = None,
-        offline: bool | None = False,
+        save_dir: _PATH = ".",
+        version: str | None = None,
+        offline: bool = False,
+        dir: _PATH | None = None,  # kept to match wandb init # noqa: A002
         id: str | None = None,  # kept to match wandb init # noqa: A002
         anonymous: bool | None = None,
-        version: str | None = None,
         project: str | None = None,
-        log_model: str | bool = False,
-        experiment: type["Run"] | type["RunDisabled"] | None = None,
-        prefix: str | None = "",
+        log_model: Literal["all"] | bool = False,
+        experiment: "Run | RunDisabled | None" = None,
+        prefix: str = "",
+        checkpoint_name: str | None = None,
         **kwargs,
     ) -> None:
         super().__init__(
             name=name,
             save_dir=save_dir,
+            version=version,
             offline=offline,
+            dir=dir,
             id=id,
             anonymous=anonymous,
-            version=version,
             project=project,
             log_model=log_model,
             experiment=experiment,
             prefix=prefix,
+            checkpoint_name=checkpoint_name,
             **kwargs,
         )
         self.image_list: list[wandb.Image] = []  # Cache images
 
     @rank_zero_only
     def add_image(self, image: np.ndarray | Figure, name: str | None = None, **kwargs) -> None:
         """Interface to add image to wandb logger.
```

### Comparing `anomalib-1.0.1/src/anomalib/metrics/__init__.py` & `anomalib-1.1.0/src/anomalib/metrics/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 """Custom anomaly evaluation metrics."""
 
 # Copyright (C) 2022-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
-
 import importlib
 import logging
 from collections.abc import Callable
 from typing import Any
 
 import torchmetrics
 from omegaconf import DictConfig, ListConfig
 
 from .anomaly_score_distribution import AnomalyScoreDistribution
 from .aupr import AUPR
 from .aupro import AUPRO
 from .auroc import AUROC
 from .collection import AnomalibMetricCollection
+from .f1_max import F1Max
 from .f1_score import F1Score
 from .min_max import MinMax
 from .precision_recall_curve import BinaryPrecisionRecallCurve
 from .pro import PRO
 from .threshold import F1AdaptiveThreshold, ManualThreshold
 
 __all__ = [
     "AUROC",
     "AUPR",
     "AUPRO",
     "AnomalyScoreDistribution",
     "BinaryPrecisionRecallCurve",
     "F1AdaptiveThreshold",
+    "F1Max",
     "F1Score",
     "ManualThreshold",
     "MinMax",
     "PRO",
 ]
 
 logger = logging.getLogger(__name__)
```

### Comparing `anomalib-1.0.1/src/anomalib/metrics/anomaly_score_distribution.py` & `anomalib-1.1.0/src/anomalib/metrics/anomaly_score_distribution.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/metrics/aupr.py` & `anomalib-1.1.0/src/anomalib/metrics/aupr.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 # Copyright (C) 2022-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
 
 import torch
 from matplotlib.figure import Figure
-from torchmetrics import PrecisionRecallCurve
+from torchmetrics.classification import BinaryPrecisionRecallCurve
 from torchmetrics.utilities.compute import auc
 from torchmetrics.utilities.data import dim_zero_cat
 
 from .plotting_utils import plot_figure
 
 
-class AUPR(PrecisionRecallCurve):
+class AUPR(BinaryPrecisionRecallCurve):
     """Area under the PR curve.
 
     This metric computes the area under the precision-recall curve.
 
     Args:
         kwargs: Additional arguments to the TorchMetrics base class.
```

### Comparing `anomalib-1.0.1/src/anomalib/metrics/aupro.py` & `anomalib-1.1.0/src/anomalib/metrics/aupro.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/metrics/auroc.py` & `anomalib-1.1.0/src/anomalib/metrics/auroc.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/metrics/binning.py` & `anomalib-1.1.0/src/anomalib/metrics/binning.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/metrics/collection.py` & `anomalib-1.1.0/src/anomalib/metrics/collection.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/metrics/f1_score.py` & `anomalib-1.1.0/src/anomalib/metrics/f1_score.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 This is added for convenience.
 """
 
 # Copyright (C) 2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
-
 import logging
 from typing import Any, Literal
 
 from torchmetrics.classification import BinaryF1Score
 
 logger = logging.getLogger(__name__)
```

### Comparing `anomalib-1.0.1/src/anomalib/metrics/min_max.py` & `anomalib-1.1.0/src/anomalib/metrics/min_max.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/metrics/optimal_f1.py` & `anomalib-1.1.0/src/anomalib/metrics/f1_max.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,77 @@
-"""Implementation of Optimal F1 score based on TorchMetrics."""
+"""Implementation of F1Max score based on TorchMetrics."""
 
 # Copyright (C) 2022-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
 import logging
 
 import torch
-from torchmetrics import Metric, PrecisionRecallCurve
+from torchmetrics import Metric
+
+from anomalib.metrics.precision_recall_curve import BinaryPrecisionRecallCurve
 
 logger = logging.getLogger(__name__)
 
 
-class OptimalF1(Metric):
-    """Optimal F1 Metric.
+class F1Max(Metric):
+    """F1Max Metric for Computing the Maximum F1 Score.
 
-    Compute the optimal F1 score at the adaptive threshold, based on the F1
-    metric of the true labels and the predicted anomaly scores.
+    This class is designed to calculate the maximum F1 score from the precision-
+    recall curve for binary classification tasks. The F1 score is a harmonic
+    mean of precision and recall, offering a balance between these two metrics.
+    The maximum F1 score (F1-Max) is particularly useful in scenarios where an
+    optimal balance between precision and recall is desired, such as in
+    imbalanced datasets or when both false positives and false negatives carry
+    significant costs.
+
+    After computing the F1Max score, the class also identifies and stores the
+    threshold that yields this maximum F1 score, which providing insight into
+    the optimal point for the classification decision.
 
     Args:
-        num_classes (int): Number of classes.
-        full_state_update (bool, optional): Whether to update the state with the
-            new values.
-            Defaults to ``False``.
-        kwargs: Any keyword arguments.
-
-    .. deprecated:: 1.0.0
-        OptimalF1 metric is deprecated and will be removed in a future release.
-        The optimal F1 score for Anomalib predictions can be obtained by
-        computing the adaptive threshold with the AnomalyScoreThreshold metric
-        and setting the computed threshold value in TorchMetrics F1Score metric.
+        **kwargs: Variable keyword arguments that can be passed to the parent class.
+
+    Attributes:
+        full_state_update (bool): Indicates whether the metric requires updating
+            the entire state. Set to False for this metric as it calculates the
+            F1 score based on the current state without needing historical data.
+        precision_recall_curve (BinaryPrecisionRecallCurve): Utility to compute
+            precision and recall values across different thresholds.
+        threshold (torch.Tensor): Stores the threshold value that results in the
+            maximum F1 score.
+
+    Examples:
+        >>> from anomalib.metrics import F1Max
+        >>> import torch
+
+        >>> preds = torch.tensor([0.1, 0.4, 0.35, 0.8])
+        >>> target = torch.tensor([0, 0, 1, 1])
+
+        >>> f1_max = F1Max()
+        >>> f1_max.update(preds, target)
+
+        >>> optimal_f1_score = f1_max.compute()
+        >>> print(f"Optimal F1 Score: {f1_max_score}")
+        >>> print(f"Optimal Threshold: {f1_max.threshold}")
+
+    Note:
+        - Use `update` method to input predictions and target labels.
+        - Use `compute` method to calculate the maximum F1 score after all
+          updates.
+        - Use `reset` method to clear the current state and prepare for a new
+          set of calculations.
     """
 
     full_state_update: bool = False
 
-    def __init__(self, num_classes: int, **kwargs) -> None:
-        msg = (
-            "OptimalF1 metric is deprecated and will be removed in a future release. The optimal F1 score for "
-            "Anomalib predictions can be obtained by computing the adaptive threshold with the "
-            "AnomalyScoreThreshold metric and setting the computed threshold value in TorchMetrics F1Score metric."
-        )
-        logger.warning(msg)
+    def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
 
-        self.precision_recall_curve = PrecisionRecallCurve(num_classes=num_classes)
+        self.precision_recall_curve = BinaryPrecisionRecallCurve()
 
         self.threshold: torch.Tensor
 
     def update(self, preds: torch.Tensor, target: torch.Tensor, *args, **kwargs) -> None:
         """Update the precision-recall curve metric."""
         del args, kwargs  # These variables are not used.
```

### Comparing `anomalib-1.0.1/src/anomalib/metrics/plotting_utils.py` & `anomalib-1.1.0/src/anomalib/metrics/plotting_utils.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/metrics/precision_recall_curve.py` & `anomalib-1.1.0/src/anomalib/metrics/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/metrics/pro.py` & `anomalib-1.1.0/src/anomalib/metrics/pro.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/metrics/threshold/base.py` & `anomalib-1.1.0/src/anomalib/metrics/threshold/base.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/metrics/threshold/f1_adaptive_threshold.py` & `anomalib-1.1.0/src/anomalib/metrics/threshold/f1_adaptive_threshold.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/metrics/threshold/manual_threshold.py` & `anomalib-1.1.0/src/anomalib/metrics/threshold/manual_threshold.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/__init__.py` & `anomalib-1.1.0/src/anomalib/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Load Anomaly Model."""
 
-# Copyright (C) 2022-2023 Intel Corporation
+# Copyright (C) 2022-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
-
 import logging
 from importlib import import_module
 
 from jsonargparse import Namespace
 from omegaconf import DictConfig, OmegaConf
 
 from anomalib.models.components import AnomalyModule
@@ -19,40 +18,42 @@
     Csflow,
     Dfkde,
     Dfm,
     Draem,
     Dsr,
     EfficientAd,
     Fastflow,
+    Fre,
     Ganomaly,
     Padim,
     Patchcore,
     ReverseDistillation,
     Rkde,
     Stfpm,
     Uflow,
     WinClip,
 )
 from .video import AiVad
 
 
 class UnknownModelError(ModuleNotFoundError):
-    ...
+    pass
 
 
 __all__ = [
     "Cfa",
     "Cflow",
     "Csflow",
     "Dfkde",
     "Dfm",
     "Draem",
     "Dsr",
     "EfficientAd",
     "Fastflow",
+    "Fre",
     "Ganomaly",
     "Padim",
     "Patchcore",
     "ReverseDistillation",
     "Rkde",
     "Stfpm",
     "Uflow",
```

### Comparing `anomalib-1.0.1/src/anomalib/models/components/__init__.py` & `anomalib-1.1.0/src/anomalib/models/components/__init__.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/components/base/anomaly_module.py` & `anomalib-1.1.0/src/anomalib/models/components/base/anomaly_module.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 """Base Anomaly Module for Training Task."""
 
 # Copyright (C) 2022-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
 import importlib
 import logging
-from abc import ABC, abstractproperty
+from abc import ABC, abstractmethod
 from collections import OrderedDict
+from pathlib import Path
 from typing import TYPE_CHECKING, Any
 
 import lightning.pytorch as pl
 import torch
 from lightning.pytorch.trainer.states import TrainerFn
 from lightning.pytorch.utilities.types import STEP_OUTPUT
 from torch import nn
 from torchvision.transforms.v2 import Compose, Normalize, Resize, Transform
 
 from anomalib import LearningType
 from anomalib.metrics import AnomalibMetricCollection
 from anomalib.metrics.threshold import BaseThreshold
 
+from .export_mixin import ExportMixin
+
 if TYPE_CHECKING:
     from lightning.pytorch.callbacks import Callback
     from torchmetrics import Metric
 
 
 logger = logging.getLogger(__name__)
 
 
-class AnomalyModule(pl.LightningModule, ABC):
+class AnomalyModule(ExportMixin, pl.LightningModule, ABC):
     """AnomalyModule to train, validate, predict and test images.
 
     Acts as a base class for all the Anomaly Modules in the library.
     """
 
     def __init__(self) -> None:
         super().__init__()
@@ -132,15 +135,16 @@
           Dictionary containing images, features, true labels and masks.
           These are required in `validation_epoch_end` for feature concatenation.
         """
         del args, kwargs  # These variables are not used.
 
         return self.predict_step(batch, batch_idx)
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def trainer_arguments(self) -> dict[str, Any]:
         """Arguments used to override the trainer parameters so as to train the model correctly."""
         raise NotImplementedError
 
     def _save_to_state_dict(self, destination: OrderedDict, prefix: str, keep_vars: bool) -> None:
         if hasattr(self, "image_threshold"):
             destination[
@@ -199,15 +203,16 @@
 
     def _get_instance(self, state_dict: OrderedDict[str, Any], dict_key: str) -> BaseThreshold:
         """Get the threshold class from the ``state_dict``."""
         class_path = state_dict.pop(dict_key)
         module = importlib.import_module(".".join(class_path.split(".")[:-1]))
         return getattr(module, class_path.split(".")[-1])()
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def learning_type(self) -> LearningType:
         """Learning type of the model."""
         raise NotImplementedError
 
     @property
     def transform(self) -> Transform:
         """Retrieve the model-specific transform.
@@ -267,7 +272,69 @@
         """Called when loading the model from a checkpoint.
 
         Loads the transform from the checkpoint and calls setup to ensure that the torch model is built before loading
         the state dict.
         """
         self._transform = checkpoint["transform"]
         self.setup("load_checkpoint")
+
+    @classmethod
+    def from_config(
+        cls: type["AnomalyModule"],
+        config_path: str | Path,
+        **kwargs,
+    ) -> "AnomalyModule":
+        """Create a model instance from the configuration.
+
+        Args:
+            config_path (str | Path): Path to the model configuration file.
+            **kwargs (dict): Additional keyword arguments.
+
+        Returns:
+            AnomalyModule: model instance.
+
+        Example:
+            The following example shows how to get model from patchcore.yaml:
+
+            .. code-block:: python
+                >>> model_config = "configs/model/patchcore.yaml"
+                >>> model = AnomalyModule.from_config(config_path=model_config)
+
+            The following example shows overriding the configuration file with additional keyword arguments:
+
+            .. code-block:: python
+                >>> override_kwargs = {"model.pre_trained": False}
+                >>> model = AnomalyModule.from_config(config_path=model_config, **override_kwargs)
+        """
+        from jsonargparse import ActionConfigFile, ArgumentParser
+        from lightning.pytorch import Trainer
+
+        from anomalib import TaskType
+
+        if not Path(config_path).exists():
+            msg = f"Configuration file not found: {config_path}"
+            raise FileNotFoundError(msg)
+
+        model_parser = ArgumentParser()
+        model_parser.add_argument(
+            "-c",
+            "--config",
+            action=ActionConfigFile,
+            help="Path to a configuration file in json or yaml format.",
+        )
+        model_parser.add_subclass_arguments(AnomalyModule, "model", required=False, fail_untyped=False)
+        model_parser.add_argument("--task", type=TaskType | str, default=TaskType.SEGMENTATION)
+        model_parser.add_argument("--metrics.image", type=list[str] | str | None, default=["F1Score", "AUROC"])
+        model_parser.add_argument("--metrics.pixel", type=list[str] | str | None, default=None, required=False)
+        model_parser.add_argument("--metrics.threshold", type=BaseThreshold | str, default="F1AdaptiveThreshold")
+        model_parser.add_class_arguments(Trainer, "trainer", fail_untyped=False, instantiate=False, sub_configs=True)
+        args = ["--config", str(config_path)]
+        for key, value in kwargs.items():
+            args.extend([f"--{key}", str(value)])
+        config = model_parser.parse_args(args=args)
+        instantiated_classes = model_parser.instantiate_classes(config)
+        model = instantiated_classes.get("model")
+        if isinstance(model, AnomalyModule):
+            return model
+
+        msg = f"Model is not an instance of AnomalyModule: {model}"
+        raise ValueError(msg)
```

### Comparing `anomalib-1.0.1/src/anomalib/models/components/base/buffer_list.py` & `anomalib-1.1.0/src/anomalib/models/components/base/buffer_list.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/components/base/dynamic_buffer.py` & `anomalib-1.1.0/src/anomalib/models/components/base/dynamic_buffer.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/components/base/memory_bank_module.py` & `anomalib-1.1.0/src/anomalib/models/components/base/memory_bank_module.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/components/classification/kde_classifier.py` & `anomalib-1.1.0/src/anomalib/models/components/classification/kde_classifier.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/components/cluster/gmm.py` & `anomalib-1.1.0/src/anomalib/models/components/cluster/gmm.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/components/cluster/kmeans.py` & `anomalib-1.1.0/src/anomalib/models/components/cluster/kmeans.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/components/dimensionality_reduction/pca.py` & `anomalib-1.1.0/src/anomalib/models/components/dimensionality_reduction/pca.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/components/dimensionality_reduction/random_projection.py` & `anomalib-1.1.0/src/anomalib/models/components/dimensionality_reduction/random_projection.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/components/feature_extractors/timm.py` & `anomalib-1.1.0/src/anomalib/models/components/feature_extractors/timm.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/components/feature_extractors/torchfx.py` & `anomalib-1.1.0/src/anomalib/models/components/feature_extractors/torchfx.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/components/feature_extractors/utils.py` & `anomalib-1.1.0/src/anomalib/models/components/feature_extractors/utils.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/components/filters/blur.py` & `anomalib-1.1.0/src/anomalib/models/components/filters/blur.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,15 +60,17 @@
         else:
             kernel_size = kernel_size if isinstance(kernel_size, tuple) else (kernel_size, kernel_size)
 
         self.kernel: torch.Tensor
         self.register_buffer("kernel", get_gaussian_kernel2d(kernel_size=kernel_size, sigma=sigma))
         if normalize:
             self.kernel = normalize_kernel2d(self.kernel)
-        self.kernel.unsqueeze_(0).unsqueeze_(0)
+
+        self.kernel = self.kernel.view(1, 1, *self.kernel.shape[-2:])
+
         self.kernel = self.kernel.expand(self.channels, -1, -1, -1)
         self.border_type = border_type
         self.padding = padding
         self.height, self.width = self.kernel.shape[-2:]
         self.padding_shape = _compute_padding([self.height, self.width])
 
     def forward(self, input_tensor: torch.Tensor) -> torch.Tensor:
```

### Comparing `anomalib-1.0.1/src/anomalib/models/components/flow/all_in_one_block.py` & `anomalib-1.1.0/src/anomalib/models/components/flow/all_in_one_block.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/components/layers/sspcab.py` & `anomalib-1.1.0/src/anomalib/models/components/layers/sspcab.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/components/sampling/k_center_greedy.py` & `anomalib-1.1.0/src/anomalib/models/components/sampling/k_center_greedy.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 - https://arxiv.org/abs/1708.00489
 """
 
 # Copyright (C) 2022-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
 import torch
-from rich.progress import track
 from torch.nn import functional as F  # noqa: N812
 
 from anomalib.models.components.dimensionality_reduction import SparseRandomProjection
+from anomalib.utils.rich import safe_track
 
 
 class KCenterGreedy:
     """Implements k-center-greedy method.
 
     Args:
         embedding (torch.Tensor): Embedding vector extracted from a CNN
@@ -94,15 +94,15 @@
             self.reset_distances()
         else:
             self.features = self.embedding.reshape(self.embedding.shape[0], -1)
             self.update_distances(cluster_centers=selected_idxs)
 
         selected_coreset_idxs: list[int] = []
         idx = int(torch.randint(high=self.n_observations, size=(1,)).item())
-        for _ in track(range(self.coreset_size), description="Selecting Coreset Indices."):
+        for _ in safe_track(sequence=range(self.coreset_size), description="Selecting Coreset Indices."):
             self.update_distances(cluster_centers=[idx])
             idx = self.get_new_idx()
             if idx in selected_idxs:
                 msg = "New indices should not be in selected indices."
                 raise ValueError(msg)
             self.min_distances[idx] = 0
             selected_coreset_idxs.append(idx)
```

### Comparing `anomalib-1.0.1/src/anomalib/models/components/stats/kde.py` & `anomalib-1.1.0/src/anomalib/models/components/stats/kde.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/components/stats/multi_variate_gaussian.py` & `anomalib-1.1.0/src/anomalib/models/components/stats/multi_variate_gaussian.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/__init__.py` & `anomalib-1.1.0/src/anomalib/models/image/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from .csflow import Csflow
 from .dfkde import Dfkde
 from .dfm import Dfm
 from .draem import Draem
 from .dsr import Dsr
 from .efficient_ad import EfficientAd
 from .fastflow import Fastflow
+from .fre import Fre
 from .ganomaly import Ganomaly
 from .padim import Padim
 from .patchcore import Patchcore
 from .reverse_distillation import ReverseDistillation
 from .rkde import Rkde
 from .stfpm import Stfpm
 from .uflow import Uflow
@@ -27,14 +28,15 @@
     "Csflow",
     "Dfkde",
     "Dfm",
     "Draem",
     "Dsr",
     "EfficientAd",
     "Fastflow",
+    "Fre",
     "Ganomaly",
     "Padim",
     "Patchcore",
     "ReverseDistillation",
     "Rkde",
     "Stfpm",
     "Uflow",
```

### Comparing `anomalib-1.0.1/src/anomalib/models/image/cfa/anomaly_map.py` & `anomalib-1.1.0/src/anomalib/models/image/cfa/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/cfa/lightning_model.py` & `anomalib-1.1.0/src/anomalib/models/image/cfa/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/cfa/loss.py` & `anomalib-1.1.0/src/anomalib/models/image/cfa/loss.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/cfa/torch_model.py` & `anomalib-1.1.0/src/anomalib/models/image/cfa/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/cflow/anomaly_map.py` & `anomalib-1.1.0/src/anomalib/models/image/cflow/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/cflow/lightning_model.py` & `anomalib-1.1.0/src/anomalib/models/image/cflow/lightning_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,14 @@
         Returns:
           Loss value for the batch
 
         """
         del args, kwargs  # These variables are not used.
 
         opt = self.optimizers()
-        self.model.encoder.eval()
 
         images: torch.Tensor = batch["image"]
         activation = self.model.encoder(images)
         avg_loss = torch.zeros([1], dtype=torch.float64).to(images.device)
 
         height = []
         width = []
```

### Comparing `anomalib-1.0.1/src/anomalib/models/image/cflow/torch_model.py` & `anomalib-1.1.0/src/anomalib/models/image/cflow/torch_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """PyTorch model for CFlow model implementation."""
 
 # Copyright (C) 2022-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
-
 from collections.abc import Sequence
 
 import einops
 import torch
 from torch import nn
 
 from anomalib.models.components import TimmFeatureExtractor
@@ -54,15 +53,19 @@
 
         self.backbone = backbone
         self.fiber_batch_size = fiber_batch_size
         self.condition_vector: int = condition_vector
         self.dec_arch = decoder
         self.pool_layers = layers
 
-        self.encoder = TimmFeatureExtractor(backbone=self.backbone, layers=self.pool_layers, pre_trained=pre_trained)
+        self.encoder = TimmFeatureExtractor(
+            backbone=self.backbone,
+            layers=self.pool_layers,
+            pre_trained=pre_trained,
+        ).eval()
         self.pool_dims = self.encoder.out_dims
         self.decoders = nn.ModuleList(
             [
                 cflow_head(
                     condition_vector=self.condition_vector,
                     coupling_blocks=coupling_blocks,
                     clamp_alpha=clamp_alpha,
```

### Comparing `anomalib-1.0.1/src/anomalib/models/image/cflow/utils.py` & `anomalib-1.1.0/src/anomalib/models/image/cflow/utils.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/csflow/anomaly_map.py` & `anomalib-1.1.0/src/anomalib/models/image/csflow/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/csflow/lightning_model.py` & `anomalib-1.1.0/src/anomalib/models/image/csflow/lightning_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 https://arxiv.org/pdf/2110.02855.pdf
 """
 
 # Copyright (C) 2022-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
-
 import logging
 from typing import Any
 
 import torch
 from lightning.pytorch.utilities.types import STEP_OUTPUT
 
 from anomalib import LearningType
@@ -64,29 +63,29 @@
         self.model = CsFlowModel(
             input_size=self.input_size,
             cross_conv_hidden_channels=self.cross_conv_hidden_channels,
             n_coupling_blocks=self.n_coupling_blocks,
             clamp=self.clamp,
             num_channels=self.num_channels,
         )
+        self.model.feature_extractor.eval()
 
     def training_step(self, batch: dict[str, str | torch.Tensor], *args, **kwargs) -> STEP_OUTPUT:
         """Perform the training step of CS-Flow.
 
         Args:
             batch (dict[str, str | torch.Tensor]): Input batch
             args: Arguments.
             kwargs: Keyword arguments.
 
         Returns:
             Loss value
         """
         del args, kwargs  # These variables are not used.
 
-        self.model.feature_extractor.eval()
         z_dist, jacobians = self.model(batch["image"])
         loss = self.loss(z_dist, jacobians)
         self.log("train_loss", loss.item(), on_epoch=True, prog_bar=True, logger=True)
         return {"loss": loss}
 
     def validation_step(self, batch: dict[str, str | torch.Tensor], *args, **kwargs) -> STEP_OUTPUT:
         """Perform the validation step for CS Flow.
```

### Comparing `anomalib-1.0.1/src/anomalib/models/image/csflow/loss.py` & `anomalib-1.1.0/src/anomalib/models/image/csflow/loss.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/csflow/torch_model.py` & `anomalib-1.1.0/src/anomalib/models/image/csflow/torch_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 # https://github.com/marco-rudolph/cs-flow
 # SPDX-License-Identifier: MIT
 #
 # Modified
 # Copyright (C) 2022-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
-
 from math import exp
 
 import numpy as np
 import torch
 from FrEIA.framework import GraphINN, InputNode, Node, OutputNode
 from FrEIA.modules import InvertibleModule
 from torch import nn
@@ -558,15 +557,15 @@
         clamp: int = 3,
         num_channels: int = 3,
     ) -> None:
         super().__init__()
         self.input_dims = (num_channels, *input_size)
         self.clamp = clamp
         self.cross_conv_hidden_channels = cross_conv_hidden_channels
-        self.feature_extractor = MultiScaleFeatureExtractor(n_scales=3, input_size=input_size)
+        self.feature_extractor = MultiScaleFeatureExtractor(n_scales=3, input_size=input_size).eval()
         self.graph = CrossScaleFlow(
             input_dims=self.input_dims,
             n_coupling_blocks=n_coupling_blocks,
             clamp=clamp,
             cross_conv_hidden_channels=cross_conv_hidden_channels,
         )
         self.anomaly_map_generator = AnomalyMapGenerator(input_dims=self.input_dims, mode=AnomalyMapMode.ALL)
```

### Comparing `anomalib-1.0.1/src/anomalib/models/image/dfkde/lightning_model.py` & `anomalib-1.1.0/src/anomalib/models/image/dfkde/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/dfkde/torch_model.py` & `anomalib-1.1.0/src/anomalib/models/image/dfkde/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/dfm/lightning_model.py` & `anomalib-1.1.0/src/anomalib/models/image/dfm/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/dfm/torch_model.py` & `anomalib-1.1.0/src/anomalib/models/image/dfm/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/draem/lightning_model.py` & `anomalib-1.1.0/src/anomalib/models/image/draem/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/draem/loss.py` & `anomalib-1.1.0/src/anomalib/models/image/draem/loss.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/draem/torch_model.py` & `anomalib-1.1.0/src/anomalib/models/image/draem/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/dsr/anomaly_generator.py` & `anomalib-1.1.0/src/anomalib/models/image/dsr/anomaly_generator.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/dsr/lightning_model.py` & `anomalib-1.1.0/src/anomalib/models/image/dsr/lightning_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         optimizer_u = torch.optim.Adam(params=self.model.upsampling_module.parameters(), lr=0.0002)
 
         return ({"optimizer": optimizer_d, "lr_scheduler": scheduler_d}, {"optimizer": optimizer_u})
 
     def on_train_start(self) -> None:
         """Load pretrained weights of the discrete model when starting training."""
         ckpt: Path = self.prepare_pretrained_model()
-        self.model.load_pretrained_discrete_model_weights(ckpt)
+        self.model.load_pretrained_discrete_model_weights(ckpt, self.device)
 
     def on_train_epoch_start(self) -> None:
         """Display a message when starting to train the upsampling module."""
         if self.current_epoch == self.second_phase:
             logger.info("Now training upsampling module.")
 
     def training_step(self, batch: dict[str, str | Tensor]) -> STEP_OUTPUT:
```

### Comparing `anomalib-1.0.1/src/anomalib/models/image/dsr/loss.py` & `anomalib-1.1.0/src/anomalib/models/image/dsr/loss.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/dsr/torch_model.py` & `anomalib-1.1.0/src/anomalib/models/image/dsr/torch_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,17 +77,17 @@
             out_channels=self.anomaly_map_dim,
             base_width=64,
         )
 
         for parameters in self.discrete_latent_model.parameters():
             parameters.requires_grad = False
 
-    def load_pretrained_discrete_model_weights(self, ckpt: Path) -> None:
+    def load_pretrained_discrete_model_weights(self, ckpt: Path, device: torch.device | str | None = None) -> None:
         """Load pre-trained model weights."""
-        self.discrete_latent_model.load_state_dict(torch.load(ckpt))
+        self.discrete_latent_model.load_state_dict(torch.load(ckpt, map_location=device))
 
     def forward(
         self,
         batch: torch.Tensor,
         anomaly_map_to_generate: torch.Tensor | None = None,
     ) -> dict[str, torch.Tensor]:
         """Compute the anomaly mask from an input image.
```

### Comparing `anomalib-1.0.1/src/anomalib/models/image/efficient_ad/lightning_model.py` & `anomalib-1.1.0/src/anomalib/models/image/efficient_ad/lightning_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,50 +54,47 @@
         weight_decay (float): optimizer weight decay
             Defaults to ``0.00001``.
         padding (bool): use padding in convoluional layers
             Defaults to ``False``.
         pad_maps (bool): relevant if padding is set to False. In this case, pad_maps = True pads the
             output anomaly maps so that their size matches the size in the padding = True case.
             Defaults to ``True``.
-        batch_size (int): batch size for imagenet dataloader
-            Defaults to ``1``.
     """
 
     def __init__(
         self,
         imagenet_dir: Path | str = "./datasets/imagenette",
         teacher_out_channels: int = 384,
         model_size: EfficientAdModelSize = EfficientAdModelSize.S,
         lr: float = 0.0001,
         weight_decay: float = 0.00001,
         padding: bool = False,
         pad_maps: bool = True,
-        batch_size: int = 1,
     ) -> None:
         super().__init__()
 
         self.imagenet_dir = Path(imagenet_dir)
         self.model_size = model_size
         self.model: EfficientAdModel = EfficientAdModel(
             teacher_out_channels=teacher_out_channels,
             model_size=model_size,
             padding=padding,
             pad_maps=pad_maps,
         )
-        self.batch_size = batch_size
+        self.batch_size = 1  # imagenet dataloader batch_size is 1 according to the paper
         self.lr = lr
         self.weight_decay = weight_decay
 
     def prepare_pretrained_model(self) -> None:
         """Prepare the pretrained teacher model."""
         pretrained_models_dir = Path("./pre_trained/")
         if not (pretrained_models_dir / "efficientad_pretrained_weights").is_dir():
             download_and_extract(pretrained_models_dir, WEIGHTS_DOWNLOAD_INFO)
         teacher_path = (
-            pretrained_models_dir / "efficientad_pretrained_weights" / f"pretrained_teacher_{self.model_size}.pth"
+            pretrained_models_dir / "efficientad_pretrained_weights" / f"pretrained_teacher_{self.model_size.value}.pth"
         )
         logger.info(f"Load pretrained teacher model from {teacher_path}")
         self.model.teacher.load_state_dict(torch.load(teacher_path, map_location=torch.device(self.device)))
 
     def prepare_imagenette_data(self, image_size: tuple[int, int] | torch.Size) -> None:
         """Prepare ImageNette dataset transformations.
 
@@ -233,17 +230,26 @@
 
         scheduler = torch.optim.lr_scheduler.StepLR(optimizer, step_size=int(0.95 * num_steps), gamma=0.1)
         return {"optimizer": optimizer, "lr_scheduler": scheduler}
 
     def on_train_start(self) -> None:
         """Called before the first training epoch.
 
-        First sets up the pretrained teacher model, then prepares the imagenette data, and finally calculates or
-        loads the channel-wise mean and std of the training dataset and push to the model.
+        First check if EfficientAd-specific parameters are set correctly (train_batch_size of 1
+        and no Imagenet normalization in transforms), then sets up the pretrained teacher model,
+        then prepares the imagenette data, and finally calculates or loads
+        the channel-wise mean and std of the training dataset and push to the model.
         """
+        if self.trainer.datamodule.train_batch_size != 1:
+            msg = "train_batch_size for EfficientAd should be 1."
+            raise ValueError(msg)
+        if self._transform and any(isinstance(transform, Normalize) for transform in self._transform.transforms):
+            msg = "Transforms for EfficientAd should not contain Normalize."
+            raise ValueError(msg)
+
         sample = next(iter(self.trainer.train_dataloader))
         image_size = sample["image"].shape[-2:]
         self.prepare_pretrained_model()
         self.prepare_imagenette_data(image_size)
         if not self.model.is_set(self.model.mean_std):
             channel_mean_std = self.teacher_channel_mean_std(self.trainer.datamodule.train_dataloader())
             self.model.mean_std.update(channel_mean_std)
@@ -310,15 +316,14 @@
 
         Returns:
             LearningType: Learning type of the model.
         """
         return LearningType.ONE_CLASS
 
     def configure_transforms(self, image_size: tuple[int, int] | None = None) -> Transform:
-        """Default transform for Padim."""
+        """Default transform for EfficientAd. Imagenet normalization applied in forward."""
         image_size = image_size or (256, 256)
         return Compose(
             [
                 Resize(image_size, antialias=True),
-                Normalize(mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225]),
             ],
         )
```

### Comparing `anomalib-1.0.1/src/anomalib/models/image/efficient_ad/torch_model.py` & `anomalib-1.1.0/src/anomalib/models/image/efficient_ad/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/fastflow/anomaly_map.py` & `anomalib-1.1.0/src/anomalib/models/image/fastflow/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/fastflow/lightning_model.py` & `anomalib-1.1.0/src/anomalib/models/image/fastflow/lightning_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 https://arxiv.org/abs/2111.07677
 """
 
 # Copyright (C) 2022-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
-
 from typing import Any
 
 import torch
 from lightning.pytorch.utilities.types import STEP_OUTPUT
 from torch import optim
 
 from anomalib import LearningType
@@ -48,17 +47,16 @@
 
         self.backbone = backbone
         self.pre_trained = pre_trained
         self.flow_steps = flow_steps
         self.conv3x3_only = conv3x3_only
         self.hidden_ratio = hidden_ratio
 
-        self.loss = FastflowLoss()
-
         self.model: FastflowModel
+        self.loss = FastflowLoss()
 
     def _setup(self) -> None:
         if self.input_size is None:
             msg = "Fastflow needs input size to build torch model."
             raise ValueError(msg)
 
         self.model = FastflowModel(
```

### Comparing `anomalib-1.0.1/src/anomalib/models/image/fastflow/loss.py` & `anomalib-1.1.0/src/anomalib/models/image/fastflow/loss.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/fastflow/torch_model.py` & `anomalib-1.1.0/src/anomalib/models/image/fastflow/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/ganomaly/lightning_model.py` & `anomalib-1.1.0/src/anomalib/models/image/ganomaly/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/ganomaly/loss.py` & `anomalib-1.1.0/src/anomalib/models/image/ganomaly/loss.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/ganomaly/torch_model.py` & `anomalib-1.1.0/src/anomalib/models/image/ganomaly/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/padim/anomaly_map.py` & `anomalib-1.1.0/src/anomalib/models/image/padim/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/padim/lightning_model.py` & `anomalib-1.1.0/src/anomalib/models/image/padim/lightning_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 Paper https://arxiv.org/abs/2011.08785
 """
 
 # Copyright (C) 2022-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
-
 import logging
 
 import torch
 from lightning.pytorch.utilities.types import STEP_OUTPUT
 from torchvision.transforms.v2 import Compose, Normalize, Resize, Transform
 
 from anomalib import LearningType
@@ -48,15 +47,15 @@
         super().__init__()
 
         self.model: PadimModel = PadimModel(
             backbone=backbone,
             pre_trained=pre_trained,
             layers=layers,
             n_features=n_features,
-        ).eval()
+        )
 
         self.stats: list[torch.Tensor] = []
         self.embeddings: list[torch.Tensor] = []
 
     @staticmethod
     def configure_optimizers() -> None:
         """PADIM doesn't require optimization, therefore returns no optimizers."""
@@ -71,17 +70,15 @@
             kwargs: Additional keyword arguments.
 
         Returns:
             Hierarchical feature map
         """
         del args, kwargs  # These variables are not used.
 
-        self.model.feature_extractor.eval()
         embedding = self.model(batch["image"])
-
         self.embeddings.append(embedding.cpu())
 
     def fit(self) -> None:
         """Fit a Gaussian to the embedding collected from the training set."""
         logger.info("Aggregating the embedding extracted from the training set.")
         embeddings = torch.vstack(self.embeddings)
```

### Comparing `anomalib-1.0.1/src/anomalib/models/image/padim/torch_model.py` & `anomalib-1.1.0/src/anomalib/models/image/padim/torch_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """PyTorch model for the PaDiM model implementation."""
 
 # Copyright (C) 2022-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
-
 from random import sample
 from typing import TYPE_CHECKING
 
 import torch
 from torch import nn
 from torch.nn import functional as F  # noqa: N812
 
@@ -63,25 +62,29 @@
         n_features (int, optional): Number of features to retain in the dimension reduction step.
             Default values from the paper are available for: resnet18 (100), wide_resnet50_2 (550).
             Defaults to ``None``.
     """
 
     def __init__(
         self,
-        layers: list[str],
         backbone: str = "resnet18",
+        layers: list[str] = ["layer1", "layer2", "layer3"],  # noqa: B006
         pre_trained: bool = True,
         n_features: int | None = None,
     ) -> None:
         super().__init__()
         self.tiler: Tiler | None = None
 
         self.backbone = backbone
         self.layers = layers
-        self.feature_extractor = TimmFeatureExtractor(backbone=self.backbone, layers=layers, pre_trained=pre_trained)
+        self.feature_extractor = TimmFeatureExtractor(
+            backbone=self.backbone,
+            layers=layers,
+            pre_trained=pre_trained,
+        ).eval()
         self.n_features_original = sum(self.feature_extractor.out_dims)
         self.n_features = n_features or _N_FEATURES_DEFAULTS.get(self.backbone)
         if self.n_features is None:
             msg = (
                 f"n_features must be specified for backbone {self.backbone}. "
                 f"Default values are available for: {sorted(_N_FEATURES_DEFAULTS.keys())}"
             )
@@ -119,14 +122,15 @@
             dict_keys(['layer1', 'layer2', 'layer3'])
 
             >>> [v.shape for v in features.values()]
             [torch.Size([32, 64, 56, 56]),
             torch.Size([32, 128, 28, 28]),
             torch.Size([32, 256, 14, 14])]
         """
+        output_size = input_tensor.shape[-2:]
         if self.tiler:
             input_tensor = self.tiler.tile(input_tensor)
 
         with torch.no_grad():
             features = self.feature_extractor(input_tensor)
             embeddings = self.generate_embedding(features)
 
@@ -136,15 +140,15 @@
         if self.training:
             output = embeddings
         else:
             output = self.anomaly_map_generator(
                 embedding=embeddings,
                 mean=self.gaussian.mean,
                 inv_covariance=self.gaussian.inv_covariance,
-                image_size=input_tensor.shape[-2:],
+                image_size=output_size,
             )
         return output
 
     def generate_embedding(self, features: dict[str, torch.Tensor]) -> torch.Tensor:
         """Generate embedding from hierarchical feature map.
 
         Args:
```

### Comparing `anomalib-1.0.1/src/anomalib/models/image/patchcore/anomaly_map.py` & `anomalib-1.1.0/src/anomalib/models/image/patchcore/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/patchcore/lightning_model.py` & `anomalib-1.1.0/src/anomalib/models/image/patchcore/lightning_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,17 +74,15 @@
             kwargs: Additional keyword arguments.
 
         Returns:
             dict[str, np.ndarray]: Embedding Vector
         """
         del args, kwargs  # These variables are not used.
 
-        self.model.feature_extractor.eval()
         embedding = self.model(batch["image"])
-
         self.embeddings.append(embedding)
 
     def fit(self) -> None:
         """Apply subsampling to the embedding collected from the training set."""
         logger.info("Aggregating the embedding extracted from the training set.")
         embeddings = torch.vstack(self.embeddings)
```

### Comparing `anomalib-1.0.1/src/anomalib/models/image/patchcore/torch_model.py` & `anomalib-1.1.0/src/anomalib/models/image/patchcore/torch_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         self.layers = layers
         self.num_neighbors = num_neighbors
 
         self.feature_extractor = TimmFeatureExtractor(
             backbone=self.backbone,
             pre_trained=pre_trained,
             layers=self.layers,
-        )
+        ).eval()
         self.feature_pooler = torch.nn.AvgPool2d(3, 1, 1)
         self.anomaly_map_generator = AnomalyMapGenerator()
 
         self.register_buffer("memory_bank", torch.Tensor())
         self.memory_bank: torch.Tensor
 
     def forward(self, input_tensor: torch.Tensor) -> torch.Tensor | dict[str, torch.Tensor]:
@@ -66,14 +66,15 @@
 
         Args:
             input_tensor (torch.Tensor): Input tensor
 
         Returns:
             Tensor | dict[str, torch.Tensor]: Embedding for training, anomaly map and anomaly score for testing.
         """
+        output_size = input_tensor.shape[-2:]
         if self.tiler:
             input_tensor = self.tiler.tile(input_tensor)
 
         with torch.no_grad():
             features = self.feature_extractor(input_tensor)
 
         features = {layer: self.feature_pooler(feature) for layer, feature in features.items()}
@@ -94,15 +95,15 @@
             patch_scores = patch_scores.reshape((batch_size, -1))
             locations = locations.reshape((batch_size, -1))
             # compute anomaly score
             pred_score = self.compute_anomaly_score(patch_scores, locations, embedding)
             # reshape to w, h
             patch_scores = patch_scores.reshape((batch_size, 1, width, height))
             # get anomaly map
-            anomaly_map = self.anomaly_map_generator(patch_scores, input_tensor.shape[-2:])
+            anomaly_map = self.anomaly_map_generator(patch_scores, output_size)
 
             output = {"anomaly_map": anomaly_map, "pred_score": pred_score}
 
         return output
 
     def generate_embedding(self, features: dict[str, torch.Tensor]) -> torch.Tensor:
         """Generate embedding from hierarchical feature map.
```

### Comparing `anomalib-1.0.1/src/anomalib/models/image/reverse_distillation/anomaly_map.py` & `anomalib-1.1.0/src/anomalib/models/image/reverse_distillation/anomaly_map.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 # Copyright (C) 2022-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
 
 from enum import Enum
 
 import torch
-from kornia.filters import gaussian_blur2d
 from omegaconf import ListConfig
 from torch import nn
 from torch.nn import functional as F  # noqa: N812
 
+from anomalib.models.components import GaussianBlur2d
+
 
 class AnomalyMapGenerationMode(str, Enum):
     """Type of mode when generating anomaly imape."""
 
     ADD = "add"
     MULTIPLY = "multiply"
 
@@ -83,12 +84,13 @@
             distance_map = torch.unsqueeze(distance_map, dim=1)
             distance_map = F.interpolate(distance_map, size=self.image_size, mode="bilinear", align_corners=True)
             if self.mode == AnomalyMapGenerationMode.MULTIPLY:
                 anomaly_map *= distance_map
             elif self.mode == AnomalyMapGenerationMode.ADD:
                 anomaly_map += distance_map
 
-        return gaussian_blur2d(
-            anomaly_map,
+        gaussian_blur = GaussianBlur2d(
             kernel_size=(self.kernel_size, self.kernel_size),
             sigma=(self.sigma, self.sigma),
-        )
+        ).to(student_features[0].device)
+
+        return gaussian_blur(anomaly_map)
```

### Comparing `anomalib-1.0.1/src/anomalib/models/image/reverse_distillation/components/__init__.py` & `anomalib-1.1.0/src/anomalib/models/image/reverse_distillation/components/__init__.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/reverse_distillation/components/bottleneck.py` & `anomalib-1.1.0/src/anomalib/models/image/reverse_distillation/components/bottleneck.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/reverse_distillation/components/de_resnet.py` & `anomalib-1.1.0/src/anomalib/models/image/reverse_distillation/components/de_resnet.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/reverse_distillation/lightning_model.py` & `anomalib-1.1.0/src/anomalib/models/image/reverse_distillation/lightning_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 https://arxiv.org/abs/2201.10703v2
 """
 
 # Copyright (C) 2022-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
-
 from collections.abc import Sequence
 from typing import Any
 
 import torch
 from lightning.pytorch.utilities.types import STEP_OUTPUT
 from torch import optim
 
@@ -46,17 +45,16 @@
         super().__init__()
 
         self.backbone = backbone
         self.pre_trained = pre_trained
         self.layers = layers
         self.anomaly_map_mode = anomaly_map_mode
 
-        self.loss = ReverseDistillationLoss()
-
         self.model: ReverseDistillationModel
+        self.loss = ReverseDistillationLoss()
 
     def _setup(self) -> None:
         if self.input_size is None:
             msg = "Input size is required for Reverse Distillation model."
             raise ValueError(msg)
 
         self.model = ReverseDistillationModel(
```

### Comparing `anomalib-1.0.1/src/anomalib/models/image/reverse_distillation/loss.py` & `anomalib-1.1.0/src/anomalib/models/image/reverse_distillation/loss.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/reverse_distillation/torch_model.py` & `anomalib-1.1.0/src/anomalib/models/image/reverse_distillation/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/rkde/feature_extractor.py` & `anomalib-1.1.0/src/anomalib/models/image/rkde/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/rkde/lightning_model.py` & `anomalib-1.1.0/src/anomalib/models/image/rkde/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/rkde/region_extractor.py` & `anomalib-1.1.0/src/anomalib/models/image/rkde/region_extractor.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/rkde/torch_model.py` & `anomalib-1.1.0/src/anomalib/models/image/rkde/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/stfpm/anomaly_map.py` & `anomalib-1.1.0/src/anomalib/models/image/stfpm/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/stfpm/lightning_model.py` & `anomalib-1.1.0/src/anomalib/models/image/stfpm/lightning_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 https://arxiv.org/abs/2103.04257
 """
 
 # Copyright (C) 2022-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
-
 from collections.abc import Sequence
 from typing import Any
 
 import torch
 from lightning.pytorch.utilities.types import STEP_OUTPUT
 from torch import optim
 
@@ -57,15 +56,14 @@
           kwargs: Additional keyword arguments.
 
         Returns:
           Loss value
         """
         del args, kwargs  # These variables are not used.
 
-        self.model.teacher_model.eval()
         teacher_features, student_features = self.model.forward(batch["image"])
         loss = self.loss(teacher_features, student_features)
         self.log("train_loss", loss.item(), on_epoch=True, prog_bar=True, logger=True)
         return {"loss": loss}
 
     def validation_step(self, batch: dict[str, str | torch.Tensor], *args, **kwargs) -> STEP_OUTPUT:
         """Perform a validation Step of STFPM.
```

### Comparing `anomalib-1.0.1/src/anomalib/models/image/stfpm/loss.py` & `anomalib-1.1.0/src/anomalib/models/image/stfpm/loss.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/stfpm/torch_model.py` & `anomalib-1.1.0/src/anomalib/models/image/stfpm/torch_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """PyTorch model for the STFPM model implementation."""
 
 # Copyright (C) 2022-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
-
 from collections.abc import Sequence
 from typing import TYPE_CHECKING
 
 import torch
 from torch import nn
 
 from anomalib.models.components import TimmFeatureExtractor
@@ -32,15 +31,15 @@
         layers: Sequence[str],
         backbone: str = "resnet18",
     ) -> None:
         super().__init__()
         self.tiler: Tiler | None = None
 
         self.backbone = backbone
-        self.teacher_model = TimmFeatureExtractor(backbone=self.backbone, pre_trained=True, layers=layers)
+        self.teacher_model = TimmFeatureExtractor(backbone=self.backbone, pre_trained=True, layers=layers).eval()
         self.student_model = TimmFeatureExtractor(
             backbone=self.backbone,
             pre_trained=False,
             layers=layers,
             requires_grad=True,
         )
 
@@ -58,14 +57,15 @@
 
         Args:
           images (torch.Tensor): Batch of images.
 
         Returns:
           Teacher and student features when in training mode, otherwise the predicted anomaly maps.
         """
+        output_size = images.shape[-2:]
         if self.tiler:
             images = self.tiler.tile(images)
         teacher_features: dict[str, torch.Tensor] = self.teacher_model(images)
         student_features: dict[str, torch.Tensor] = self.student_model(images)
 
         if self.tiler:
             for layer, data in teacher_features.items():
@@ -75,11 +75,11 @@
 
         if self.training:
             output = teacher_features, student_features
         else:
             output = self.anomaly_map_generator(
                 teacher_features=teacher_features,
                 student_features=student_features,
-                image_size=images.shape[-2:],
+                image_size=output_size,
             )
 
         return output
```

### Comparing `anomalib-1.0.1/src/anomalib/models/image/uflow/anomaly_map.py` & `anomalib-1.1.0/src/anomalib/models/image/uflow/anomaly_map.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/uflow/feature_extraction.py` & `anomalib-1.1.0/src/anomalib/models/image/uflow/feature_extraction.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,23 +28,21 @@
     Returns:
         FeatureExtractorInterface: Feature extractor.
     """
     if backbone not in AVAILABLE_EXTRACTORS:
         msg = f"Feature extractor must be one of {AVAILABLE_EXTRACTORS}."
         raise ValueError(msg)
 
+    feature_extractor: nn.Module
     if backbone in ["resnet18", "wide_resnet50_2"]:
-        return FeatureExtractor(backbone, input_size, layers=("layer1", "layer2", "layer3"))
+        feature_extractor = FeatureExtractor(backbone, input_size, layers=("layer1", "layer2", "layer3")).eval()
     if backbone == "mcait":
-        return MCaitFeatureExtractor()
-    msg = (
-        "`backbone` must be one of `[mcait, resnet18, wide_resnet50_2]`. These are the only feature extractors tested. "
-        "It does not mean that other feature extractors will not work."
-    )
-    raise ValueError(msg)
+        feature_extractor = MCaitFeatureExtractor().eval()
+
+    return feature_extractor
 
 
 class FeatureExtractor(TimmFeatureExtractor):
     """Feature extractor based on ResNet (or others) backbones.
 
     Args:
         backbone (str): Backbone of the feature extractor.
```

### Comparing `anomalib-1.0.1/src/anomalib/models/image/uflow/lightning_model.py` & `anomalib-1.1.0/src/anomalib/models/image/uflow/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/uflow/loss.py` & `anomalib-1.1.0/src/anomalib/models/image/uflow/loss.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/uflow/torch_model.py` & `anomalib-1.1.0/src/anomalib/models/image/uflow/torch_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """U-Flow torch model."""
 
 # Copyright (C) 2023-2024 Intel Corporation
 # SPDX-License-Identifier: Apache-2.0
 
-
 import torch
 from FrEIA import framework as ff
 from FrEIA import modules as fm
 from torch import nn
 
 from anomalib.models.components.flow import AllInOneBlock
```

### Comparing `anomalib-1.0.1/src/anomalib/models/image/winclip/lightning_model.py` & `anomalib-1.1.0/src/anomalib/models/image/winclip/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/winclip/prompting.py` & `anomalib-1.1.0/src/anomalib/models/image/winclip/prompting.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/image/winclip/torch_model.py` & `anomalib-1.1.0/src/anomalib/models/image/winclip/torch_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,14 +218,15 @@
         pooled, _ = self.clip.visual._global_pool(masked)  # noqa: SLF001
 
         if self.clip.visual.proj is not None:
             pooled = pooled @ self.clip.visual.proj
 
         return pooled.reshape((n_masks, batch_size, -1)).permute(1, 0, 2)
 
+    @torch.no_grad
     def forward(self, batch: torch.Tensor) -> tuple[torch.Tensor, torch.Tensor]:
         """Forward-pass through the model to obtain image and pixel scores.
 
         Args:
             batch (torch.Tensor): Batch of input images of shape ``(batch_size, C, H, W)``.
 
         Returns:
@@ -310,49 +311,51 @@
             strict=True,
         ):
             scores = visual_association_score(window_embedding, reference_embedding)
             multi_scale_scores.append(harmonic_aggregation(scores, self.grid_size, mask))
 
         return torch.stack(multi_scale_scores).mean(dim=0)
 
+    @torch.no_grad
     def _collect_text_embeddings(self, class_name: str) -> None:
         """Collect text embeddings for the object class using a compositional prompt ensemble.
 
         First, an ensemble of normal and anomalous prompts is created based on the name of the object class. The
         prompt ensembles are then tokenized and encoded to obtain prompt embeddings. The prompt embeddings are
         averaged to obtain a single text embedding for the object class. These final text embeddings are stored in
         the model to be used during inference.
 
         Args:
             class_name (str): The name of the object class used in the prompt ensemble.
         """
+        # get the device, this is to ensure that we move the text embeddings to the same device as the model
+        device = next(self.parameters()).device
         # collect prompt ensemble
         normal_prompts, anomalous_prompts = create_prompt_ensemble(class_name)
         # tokenize prompts
         normal_tokens = tokenize(normal_prompts)
         anomalous_tokens = tokenize(anomalous_prompts)
         # encode tokens to obtain prompt embeddings
-        with torch.no_grad():
-            normal_embeddings = self.clip.encode_text(normal_tokens)
-            anomalous_embeddings = self.clip.encode_text(anomalous_tokens)
+        normal_embeddings = self.clip.encode_text(normal_tokens.to(device))
+        anomalous_embeddings = self.clip.encode_text(anomalous_tokens.to(device))
         # average prompt embeddings
         normal_embeddings = torch.mean(normal_embeddings, dim=0, keepdim=True)
         anomalous_embeddings = torch.mean(anomalous_embeddings, dim=0, keepdim=True)
         # concatenate and store
         text_embeddings = torch.cat((normal_embeddings, anomalous_embeddings))
         self._text_embeddings = text_embeddings
 
+    @torch.no_grad
     def _collect_visual_embeddings(self, images: torch.Tensor) -> None:
         """Collect visual embeddings based on a set of normal reference images.
 
         Args:
             images (torch.Tensor): Tensor of shape ``(K, C, H, W)`` containing the reference images.
         """
-        with torch.no_grad():
-            _, self._visual_embeddings, self._patch_embeddings = self.encode_image(images)
+        _, self._visual_embeddings, self._patch_embeddings = self.encode_image(images)
 
     def _generate_masks(self) -> list[torch.Tensor]:
         """Prepare a set of masks that operate as multi-scale sliding windows.
 
         For each of the scales, a set of masks is created that select patches from the feature map. Each mask represents
         a sliding window location in the pixel domain. The masks are stored in the model to be used during inference.
```

### Comparing `anomalib-1.0.1/src/anomalib/models/image/winclip/utils.py` & `anomalib-1.1.0/src/anomalib/models/image/winclip/utils.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/video/ai_vad/clip/clip.py` & `anomalib-1.1.0/src/anomalib/models/video/ai_vad/clip/clip.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/video/ai_vad/clip/model.py` & `anomalib-1.1.0/src/anomalib/models/video/ai_vad/clip/model.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/video/ai_vad/density.py` & `anomalib-1.1.0/src/anomalib/models/video/ai_vad/density.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/video/ai_vad/features.py` & `anomalib-1.1.0/src/anomalib/models/video/ai_vad/features.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/video/ai_vad/flow.py` & `anomalib-1.1.0/src/anomalib/models/video/ai_vad/flow.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/video/ai_vad/lightning_model.py` & `anomalib-1.1.0/src/anomalib/models/video/ai_vad/lightning_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/video/ai_vad/regions.py` & `anomalib-1.1.0/src/anomalib/models/video/ai_vad/regions.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/models/video/ai_vad/torch_model.py` & `anomalib-1.1.0/src/anomalib/models/video/ai_vad/torch_model.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/utils/cv/connected_components.py` & `anomalib-1.1.0/src/anomalib/utils/cv/connected_components.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/utils/exceptions/imports.py` & `anomalib-1.1.0/src/anomalib/utils/exceptions/imports.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/utils/normalization/min_max.py` & `anomalib-1.1.0/src/anomalib/utils/normalization/min_max.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/utils/path.py` & `anomalib-1.1.0/src/anomalib/utils/path.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/utils/post_processing.py` & `anomalib-1.1.0/src/anomalib/utils/post_processing.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/utils/types/__init__.py` & `anomalib-1.1.0/src/anomalib/utils/types/__init__.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/utils/visualization/base.py` & `anomalib-1.1.0/src/anomalib/utils/visualization/base.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/utils/visualization/image.py` & `anomalib-1.1.0/src/anomalib/utils/visualization/image.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib/utils/visualization/metrics.py` & `anomalib-1.1.0/src/anomalib/utils/visualization/metrics.py`

 * *Files identical despite different names*

### Comparing `anomalib-1.0.1/src/anomalib.egg-info/PKG-INFO` & `anomalib-1.1.0/src/anomalib.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 Metadata-Version: 2.1
 Name: anomalib
-Version: 1.0.1
+Version: 1.1.0
 Summary: anomalib - Anomaly Detection Library
-Home-page: 
 Author: Intel OpenVINO
-Author-email: help@openvino.intel.com
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -204,23 +202,83 @@
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Provides-Extra: loggers
+License-File: LICENSE
+Requires-Dist: omegaconf>=2.1.1
+Requires-Dist: rich>=13.5.2
+Requires-Dist: jsonargparse[signatures]>=4.27.7
+Requires-Dist: docstring_parser
+Requires-Dist: rich_argparse
 Provides-Extra: core
-Provides-Extra: notebooks
+Requires-Dist: av>=10.0.0; extra == "core"
+Requires-Dist: einops>=0.3.2; extra == "core"
+Requires-Dist: freia>=0.2; extra == "core"
+Requires-Dist: imgaug==0.4.0; extra == "core"
+Requires-Dist: kornia>=0.6.6; extra == "core"
+Requires-Dist: matplotlib>=3.4.3; extra == "core"
+Requires-Dist: opencv-python>=4.5.3.56; extra == "core"
+Requires-Dist: pandas>=1.1.0; extra == "core"
+Requires-Dist: timm<=1.0.3,>=0.5.4; extra == "core"
+Requires-Dist: lightning>=2.2; extra == "core"
+Requires-Dist: torch>=2; extra == "core"
+Requires-Dist: torchmetrics>=1.3.2; extra == "core"
+Requires-Dist: open-clip-torch>=2.23.0; extra == "core"
 Provides-Extra: openvino
+Requires-Dist: openvino>=2024.0; extra == "openvino"
+Requires-Dist: nncf>=2.10.0; extra == "openvino"
+Requires-Dist: onnx>=1.16.0; extra == "openvino"
+Provides-Extra: loggers
+Requires-Dist: comet-ml>=3.31.7; extra == "loggers"
+Requires-Dist: gradio>=4; extra == "loggers"
+Requires-Dist: tensorboard; extra == "loggers"
+Requires-Dist: wandb<=0.15.9,>=0.12.17; extra == "loggers"
+Requires-Dist: mlflow>=1.0.0; extra == "loggers"
+Provides-Extra: notebooks
+Requires-Dist: gitpython; extra == "notebooks"
+Requires-Dist: ipykernel; extra == "notebooks"
+Requires-Dist: ipywidgets; extra == "notebooks"
+Requires-Dist: notebook; extra == "notebooks"
+Provides-Extra: docs
+Requires-Dist: myst-parser; extra == "docs"
+Requires-Dist: nbsphinx; extra == "docs"
+Requires-Dist: pandoc; extra == "docs"
+Requires-Dist: sphinx<8.0; extra == "docs"
+Requires-Dist: sphinx_autodoc_typehints; extra == "docs"
+Requires-Dist: sphinx_book_theme; extra == "docs"
+Requires-Dist: sphinx-copybutton; extra == "docs"
+Requires-Dist: sphinx_design; extra == "docs"
+Provides-Extra: test
+Requires-Dist: pre-commit; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-xdist; extra == "test"
+Requires-Dist: pytest-mock; extra == "test"
+Requires-Dist: pytest-sugar; extra == "test"
+Requires-Dist: coverage[toml]; extra == "test"
+Requires-Dist: tox; extra == "test"
 Provides-Extra: full
+Requires-Dist: anomalib[core,loggers,notebooks,openvino]; extra == "full"
 Provides-Extra: dev
-License-File: LICENSE
+Requires-Dist: anomalib[docs,full,test]; extra == "dev"
 
 <div align="center">
 
 <img src="https://raw.githubusercontent.com/openvinotoolkit/anomalib/main/docs/source/_static/images/logos/anomalib-wide-blue.png" width="600px">
 
 **A library for benchmarking, developing and deploying deep learning anomaly detection algorithms**
 
@@ -235,14 +293,15 @@
 [![pytorch](https://img.shields.io/badge/pytorch-1.8.1%2B-orange)]()
 [![openvino](https://img.shields.io/badge/openvino-2022.3.0-purple)]()
 
 [![Pre-Merge Checks](https://github.com/openvinotoolkit/anomalib/actions/workflows/pre_merge.yml/badge.svg)](https://github.com/openvinotoolkit/anomalib/actions/workflows/pre_merge.yml)
 [![Documentation Status](https://readthedocs.org/projects/anomalib/badge/?version=latest)](https://anomalib.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/openvinotoolkit/anomalib/branch/main/graph/badge.svg?token=Z6A07N1BZK)](https://codecov.io/gh/openvinotoolkit/anomalib)
 [![Downloads](https://static.pepy.tech/personalized-badge/anomalib?period=total&units=international_system&left_color=grey&right_color=green&left_text=PyPI%20Downloads)](https://pepy.tech/project/anomalib)
+[![Discord](https://img.shields.io/discord/1230798452577800237?style=plastic)](https://discord.com/channels/1230798452577800237)
 
 </div>
 
 ---
 
 # 👋 Introduction
 
@@ -253,30 +312,30 @@
 </p>
 
 ## Key features
 
 - Simple and modular API and CLI for training, inference, benchmarking, and hyperparameter optimization.
 - The largest public collection of ready-to-use deep learning anomaly detection algorithms and benchmark datasets.
 - [**Lightning**](https://www.lightning.ai/) based model implementations to reduce boilerplate code and limit the implementation efforts to the bare essentials.
-- All models can be exported to [**OpenVINO**](https://www.intel.com/content/www/us/en/developer/tools/openvino-toolkit/overview.html) Intermediate Representation (IR) for accelerated inference on intel hardware.
+- The majority of models can be exported to [**OpenVINO**](https://www.intel.com/content/www/us/en/developer/tools/openvino-toolkit/overview.html) Intermediate Representation (IR) for accelerated inference on Intel hardware.
 - A set of [inference tools](tools) for quick and easy deployment of the standard or custom anomaly detection models.
 
 # 📦 Installation
 
 Anomalib provides two ways to install the library. The first is through PyPI, and the second is through a local installation. PyPI installation is recommended if you want to use the library without making any changes to the source code. If you want to make changes to the library, then a local installation is recommended.
 
 <details>
 <summary>Install from PyPI</summary>
 Installing the library with pip is the easiest way to get started with anomalib.
 
 ```bash
 pip install anomalib
 ```
 
-This will install Anomalib CLI using the [installer](requirements/installer.txt) dependencies. Anomalib CLI is a command line interface for training, inference, benchmarking, and hyperparameter optimization. If you want to use the library as a Python package, you can install the library with the following command:
+This will install Anomalib CLI using the [dependencies](/pyproject.toml) in the `pyproject.toml` file. Anomalib CLI is a command line interface for training, inference, benchmarking, and hyperparameter optimization. If you want to use the library as a Python package, you can install the library with the following command:
 
 ```bash
 # Get help for the installation arguments
 anomalib install -h
 
 # Install the full package
 anomalib install
@@ -308,15 +367,15 @@
 
 # Clone the repository and install in editable mode
 git clone https://github.com/openvinotoolkit/anomalib.git
 cd anomalib
 pip install -e .
 ```
 
-This will install Anomalib CLI using the [installer](requirements/installer.txt) dependencies. Anomalib CLI is a command line interface for training, inference, benchmarking, and hyperparameter optimization. If you want to use the library as a Python package, you can install the library with the following command:
+This will install Anomalib CLI using the [dependencies](/pyproject.toml) in the `pyproject.toml` file. Anomalib CLI is a command line interface for training, inference, benchmarking, and hyperparameter optimization. If you want to use the library as a Python package, you can install the library with the following command:
 
 ```bash
 # Get help for the installation arguments
 anomalib install -h
 
 # Install the full package
 anomalib install
```

### Comparing `anomalib-1.0.1/src/anomalib.egg-info/SOURCES.txt` & `anomalib-1.1.0/src/anomalib.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-setup.py
-requirements/core.txt
-requirements/dev.txt
-requirements/installer.txt
-requirements/loggers.txt
-requirements/notebooks.txt
-requirements/openvino.txt
 src/anomalib/__init__.py
 src/anomalib/py.typed
 src/anomalib.egg-info/PKG-INFO
 src/anomalib.egg-info/SOURCES.txt
 src/anomalib.egg-info/dependency_links.txt
 src/anomalib.egg-info/entry_points.txt
 src/anomalib.egg-info/requires.txt
@@ -33,14 +26,15 @@
 src/anomalib/callbacks/normalization/__init__.py
 src/anomalib/callbacks/normalization/base.py
 src/anomalib/callbacks/normalization/min_max_normalization.py
 src/anomalib/callbacks/normalization/utils.py
 src/anomalib/cli/__init__.py
 src/anomalib/cli/cli.py
 src/anomalib/cli/install.py
+src/anomalib/cli/pipelines.py
 src/anomalib/cli/utils/__init__.py
 src/anomalib/cli/utils/help_formatter.py
 src/anomalib/cli/utils/installation.py
 src/anomalib/cli/utils/openvino.py
 src/anomalib/data/__init__.py
 src/anomalib/data/errors.py
 src/anomalib/data/predict.py
@@ -84,39 +78,41 @@
 src/anomalib/deploy/inferencers/openvino_inferencer.py
 src/anomalib/deploy/inferencers/torch_inferencer.py
 src/anomalib/engine/__init__.py
 src/anomalib/engine/engine.py
 src/anomalib/loggers/__init__.py
 src/anomalib/loggers/base.py
 src/anomalib/loggers/comet.py
+src/anomalib/loggers/mlflow.py
 src/anomalib/loggers/tensorboard.py
 src/anomalib/loggers/wandb.py
 src/anomalib/metrics/__init__.py
 src/anomalib/metrics/anomaly_score_distribution.py
 src/anomalib/metrics/aupr.py
 src/anomalib/metrics/aupro.py
 src/anomalib/metrics/auroc.py
 src/anomalib/metrics/binning.py
 src/anomalib/metrics/collection.py
+src/anomalib/metrics/f1_max.py
 src/anomalib/metrics/f1_score.py
 src/anomalib/metrics/min_max.py
-src/anomalib/metrics/optimal_f1.py
 src/anomalib/metrics/plotting_utils.py
 src/anomalib/metrics/precision_recall_curve.py
 src/anomalib/metrics/pro.py
 src/anomalib/metrics/threshold/__init__.py
 src/anomalib/metrics/threshold/base.py
 src/anomalib/metrics/threshold/f1_adaptive_threshold.py
 src/anomalib/metrics/threshold/manual_threshold.py
 src/anomalib/models/__init__.py
 src/anomalib/models/components/__init__.py
 src/anomalib/models/components/base/__init__.py
 src/anomalib/models/components/base/anomaly_module.py
 src/anomalib/models/components/base/buffer_list.py
 src/anomalib/models/components/base/dynamic_buffer.py
+src/anomalib/models/components/base/export_mixin.py
 src/anomalib/models/components/base/memory_bank_module.py
 src/anomalib/models/components/classification/__init__.py
 src/anomalib/models/components/classification/kde_classifier.py
 src/anomalib/models/components/cluster/__init__.py
 src/anomalib/models/components/cluster/gmm.py
 src/anomalib/models/components/cluster/kmeans.py
 src/anomalib/models/components/dimensionality_reduction/__init__.py
@@ -172,14 +168,17 @@
 src/anomalib/models/image/efficient_ad/lightning_model.py
 src/anomalib/models/image/efficient_ad/torch_model.py
 src/anomalib/models/image/fastflow/__init__.py
 src/anomalib/models/image/fastflow/anomaly_map.py
 src/anomalib/models/image/fastflow/lightning_model.py
 src/anomalib/models/image/fastflow/loss.py
 src/anomalib/models/image/fastflow/torch_model.py
+src/anomalib/models/image/fre/__init__.py
+src/anomalib/models/image/fre/lightning_model.py
+src/anomalib/models/image/fre/torch_model.py
 src/anomalib/models/image/ganomaly/__init__.py
 src/anomalib/models/image/ganomaly/lightning_model.py
 src/anomalib/models/image/ganomaly/loss.py
 src/anomalib/models/image/ganomaly/torch_model.py
 src/anomalib/models/image/padim/__init__.py
 src/anomalib/models/image/padim/anomaly_map.py
 src/anomalib/models/image/padim/lightning_model.py
@@ -224,18 +223,36 @@
 src/anomalib/models/video/ai_vad/flow.py
 src/anomalib/models/video/ai_vad/lightning_model.py
 src/anomalib/models/video/ai_vad/regions.py
 src/anomalib/models/video/ai_vad/torch_model.py
 src/anomalib/models/video/ai_vad/clip/__init__.py
 src/anomalib/models/video/ai_vad/clip/clip.py
 src/anomalib/models/video/ai_vad/clip/model.py
+src/anomalib/pipelines/__init__.py
+src/anomalib/pipelines/types.py
+src/anomalib/pipelines/benchmark/__init__.py
+src/anomalib/pipelines/benchmark/generator.py
+src/anomalib/pipelines/benchmark/job.py
+src/anomalib/pipelines/benchmark/pipeline.py
+src/anomalib/pipelines/components/__init__.py
+src/anomalib/pipelines/components/base/__init__.py
+src/anomalib/pipelines/components/base/job.py
+src/anomalib/pipelines/components/base/pipeline.py
+src/anomalib/pipelines/components/base/runner.py
+src/anomalib/pipelines/components/runners/__init__.py
+src/anomalib/pipelines/components/runners/parallel.py
+src/anomalib/pipelines/components/runners/serial.py
+src/anomalib/pipelines/components/utils/__init__.py
+src/anomalib/pipelines/components/utils/grid_search.py
 src/anomalib/utils/__init__.py
 src/anomalib/utils/config.py
+src/anomalib/utils/logging.py
 src/anomalib/utils/path.py
 src/anomalib/utils/post_processing.py
+src/anomalib/utils/rich.py
 src/anomalib/utils/cv/__init__.py
 src/anomalib/utils/cv/connected_components.py
 src/anomalib/utils/exceptions/__init__.py
 src/anomalib/utils/exceptions/imports.py
 src/anomalib/utils/normalization/__init__.py
 src/anomalib/utils/normalization/min_max.py
 src/anomalib/utils/types/__init__.py
```

