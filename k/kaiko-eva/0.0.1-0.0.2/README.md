# Comparing `tmp/kaiko_eva-0.0.1.tar.gz` & `tmp/kaiko_eva-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaiko_eva-0.0.1.tar", last modified: Fri Mar 22 13:51:45 2024, max compression
+gzip compressed data, was "kaiko_eva-0.0.2.tar", last modified: Fri May 31 08:47:39 2024, max compression
```

## Comparing `kaiko_eva-0.0.1.tar` & `kaiko_eva-0.0.2.tar`

### file list

```diff
@@ -1,300 +1,327 @@
--rw-r--r--   0        0        0    11338 2024-03-22 13:47:45.753068 kaiko_eva-0.0.1/LICENSE
--rw-r--r--   0        0        0     7626 2024-03-22 13:47:45.753068 kaiko_eva-0.0.1/README.md
--rw-r--r--   0        0        0     4123 2024-03-22 13:51:45.767768 kaiko_eva-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      518 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/__init__.py
--rw-r--r--   0        0        0      282 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/__main__.py
--rw-r--r--   0        0        0      611 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/__version__.py
--rw-r--r--   0        0        0      451 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/__init__.py
--rw-r--r--   0        0        0      110 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/callbacks/__init__.py
--rw-r--r--   0        0        0      121 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/callbacks/writers/__init__.py
--rw-r--r--   0        0        0     6752 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/callbacks/writers/embeddings.py
--rw-r--r--   0        0        0      616 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/callbacks/writers/typings.py
--rw-r--r--   0        0        0       68 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/cli/__init__.py
--rw-r--r--   0        0        0      422 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/cli/cli.py
--rw-r--r--   0        0        0      786 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/cli/logo.py
--rw-r--r--   0        0        0     2663 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/cli/setup.py
--rw-r--r--   0        0        0      340 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/data/__init__.py
--rw-r--r--   0        0        0      110 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/data/dataloaders/__init__.py
--rw-r--r--   0        0        0     2368 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/data/dataloaders/dataloader.py
--rw-r--r--   0        0        0      229 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/data/datamodules/__init__.py
--rw-r--r--   0        0        0      940 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/data/datamodules/call.py
--rw-r--r--   0        0        0     3878 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/data/datamodules/datamodule.py
--rw-r--r--   0        0        0     1869 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/data/datamodules/schemas.py
--rw-r--r--   0        0        0      281 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/data/datasets/__init__.py
--rw-r--r--   0        0        0     2005 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/data/datasets/base.py
--rw-r--r--   0        0        0      176 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/data/datasets/classification/__init__.py
--rw-r--r--   0        0        0     5215 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/data/datasets/classification/embeddings.py
--rw-r--r--   0        0        0      124 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/data/datasets/dataset.py
--rw-r--r--   0        0        0      100 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/data/samplers/__init__.py
--rw-r--r--   0        0        0      119 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/data/samplers/sampler.py
--rw-r--r--   0        0        0      157 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/data/transforms/__init__.py
--rw-r--r--   0        0        0      174 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/data/transforms/dtype/__init__.py
--rw-r--r--   0        0        0      725 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/data/transforms/dtype/array.py
--rw-r--r--   0        0        0       98 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/interface/__init__.py
--rw-r--r--   0        0        0     2741 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/interface/interface.py
--rw-r--r--   0        0        0      558 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/metrics/__init__.py
--rw-r--r--   0        0        0     1267 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/metrics/average_loss.py
--rw-r--r--   0        0        0      806 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/metrics/binary_balanced_accuracy.py
--rw-r--r--   0        0        0      301 2024-03-22 13:47:45.757068 kaiko_eva-0.0.1/src/eva/core/metrics/defaults/__init__.py
--rw-r--r--   0        0        0      316 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/metrics/defaults/classification/__init__.py
--rw-r--r--   0        0        0     2520 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/metrics/defaults/classification/binary.py
--rw-r--r--   0        0        0     2703 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/metrics/defaults/classification/multiclass.py
--rw-r--r--   0        0        0      422 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/metrics/structs/__init__.py
--rw-r--r--   0        0        0      149 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/metrics/structs/collection.py
--rw-r--r--   0        0        0      109 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/metrics/structs/metric.py
--rw-r--r--   0        0        0     3619 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/metrics/structs/module.py
--rw-r--r--   0        0        0     1480 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/metrics/structs/schemas.py
--rw-r--r--   0        0        0      388 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/metrics/structs/typings.py
--rw-r--r--   0        0        0      305 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/models/__init__.py
--rw-r--r--   0        0        0      255 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/models/modules/__init__.py
--rw-r--r--   0        0        0     4138 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/models/modules/head.py
--rw-r--r--   0        0        0      978 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/models/modules/inference.py
--rw-r--r--   0        0        0     5918 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/models/modules/module.py
--rw-r--r--   0        0        0      521 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/models/modules/typings.py
--rw-r--r--   0        0        0      227 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/models/modules/utils/__init__.py
--rw-r--r--   0        0        0     1915 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/models/modules/utils/batch_postprocess.py
--rw-r--r--   0        0        0      706 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/models/modules/utils/grad.py
--rw-r--r--   0        0        0      232 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/models/networks/__init__.py
--rw-r--r--   0        0        0      957 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/models/networks/_utils.py
--rw-r--r--   0        0        0     2411 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/models/networks/mlp.py
--rw-r--r--   0        0        0      159 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/models/networks/transforms/__init__.py
--rw-r--r--   0        0        0      822 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/models/networks/transforms/extract_cls_features.py
--rw-r--r--   0        0        0      381 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/models/networks/wrappers/__init__.py
--rw-r--r--   0        0        0     1320 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/models/networks/wrappers/base.py
--rw-r--r--   0        0        0     2035 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/models/networks/wrappers/from_function.py
--rw-r--r--   0        0        0     1289 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/models/networks/wrappers/huggingface.py
--rw-r--r--   0        0        0     1718 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/models/networks/wrappers/onnx.py
--rw-r--r--   0        0        0      208 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/trainers/__init__.py
--rw-r--r--   0        0        0     2571 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/trainers/_logging.py
--rw-r--r--   0        0        0     5652 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/trainers/_recorder.py
--rw-r--r--   0        0        0      321 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/trainers/_utils.py
--rw-r--r--   0        0        0     3775 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/trainers/functional.py
--rw-r--r--   0        0        0     3261 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/trainers/trainer.py
--rw-r--r--   0        0        0       58 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/utils/__init__.py
--rw-r--r--   0        0        0      112 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/utils/io/__init__.py
--rw-r--r--   0        0        0      509 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/utils/io/dataframe.py
--rw-r--r--   0        0        0     1383 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/utils/multiprocessing.py
--rw-r--r--   0        0        0      634 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/core/utils/workers.py
--rw-r--r--   0        0        0      438 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/__init__.py
--rw-r--r--   0        0        0      111 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/data/__init__.py
--rw-r--r--   0        0        0      497 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/data/datasets/__init__.py
--rw-r--r--   0        0        0     1414 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/data/datasets/_utils.py
--rw-r--r--   0        0        0     2099 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/data/datasets/_validators.py
--rw-r--r--   0        0        0      520 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/data/datasets/classification/__init__.py
--rw-r--r--   0        0        0     5637 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/data/datasets/classification/bach.py
--rw-r--r--   0        0        0     3060 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/data/datasets/classification/base.py
--rw-r--r--   0        0        0     5875 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/data/datasets/classification/crc.py
--rw-r--r--   0        0        0     3257 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/data/datasets/classification/mhist.py
--rw-r--r--   0        0        0     7253 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/data/datasets/classification/patch_camelyon.py
--rw-r--r--   0        0        0     8069 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/data/datasets/classification/total_segmentator.py
--rw-r--r--   0        0        0      249 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/data/datasets/segmentation/__init__.py
--rw-r--r--   0        0        0     3630 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/data/datasets/segmentation/base.py
--rw-r--r--   0        0        0     8075 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/data/datasets/segmentation/total_segmentator.py
--rw-r--r--   0        0        0      389 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/data/datasets/structs.py
--rw-r--r--   0        0        0     1100 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/data/datasets/vision.py
--rw-r--r--   0        0        0      120 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/data/transforms/__init__.py
--rw-r--r--   0        0        0      138 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/data/transforms/common/__init__.py
--rw-r--r--   0        0        0     1485 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/data/transforms/common/resize_and_crop.py
--rw-r--r--   0        0        0       89 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/models/__init__.py
--rw-r--r--   0        0        0      170 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/models/networks/__init__.py
--rw-r--r--   0        0        0     6796 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/models/networks/abmil.py
--rw-r--r--   0        0        0      148 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/models/networks/postprocesses/__init__.py
--rw-r--r--   0        0        0      822 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/models/networks/postprocesses/cls.py
--rw-r--r--   0        0        0       96 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/utils/__init__.py
--rw-r--r--   0        0        0      310 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/utils/io/__init__.py
--rw-r--r--   0        0        0      768 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/utils/io/_utils.py
--rw-r--r--   0        0        0     1489 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/utils/io/image.py
--rw-r--r--   0        0        0     1510 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/utils/io/nifti.py
--rw-r--r--   0        0        0      472 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/src/eva/vision/utils/io/text.py
--rw-r--r--   0        0        0       17 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0       22 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/tests/eva/__init__.py
--rw-r--r--   0        0        0      841 2024-03-22 13:47:45.761067 kaiko_eva-0.0.1/tests/eva/_cli.py
--rw-r--r--   0        0        0      129 2024-03-22 13:47:46.633063 kaiko_eva-0.0.1/tests/eva/assets/core/datasets/embeddings/embeddings/tensor_0_shape_8.pt
--rw-r--r--   0        0        0      129 2024-03-22 13:47:46.633063 kaiko_eva-0.0.1/tests/eva/assets/core/datasets/embeddings/embeddings/tensor_1_shape_8.pt
--rw-r--r--   0        0        0      129 2024-03-22 13:47:46.633063 kaiko_eva-0.0.1/tests/eva/assets/core/datasets/embeddings/embeddings/tensor_2_shape_8.pt
--rw-r--r--   0        0        0      129 2024-03-22 13:47:46.633063 kaiko_eva-0.0.1/tests/eva/assets/core/datasets/embeddings/embeddings/tensor_3_shape_8.pt
--rw-r--r--   0        0        0      129 2024-03-22 13:47:46.633063 kaiko_eva-0.0.1/tests/eva/assets/core/datasets/embeddings/embeddings/tensor_4_shape_1x8.pt
--rw-r--r--   0        0        0      129 2024-03-22 13:47:46.633063 kaiko_eva-0.0.1/tests/eva/assets/core/datasets/embeddings/embeddings/tensor_5_shape_1x8.pt
--rw-r--r--   0        0        0      129 2024-03-22 13:47:46.637063 kaiko_eva-0.0.1/tests/eva/assets/core/datasets/embeddings/embeddings/tensor_6_shape_1x8.pt
--rw-r--r--   0        0        0      129 2024-03-22 13:47:46.637063 kaiko_eva-0.0.1/tests/eva/assets/core/datasets/embeddings/embeddings/tensor_7_shape_1x8.pt
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.637063 kaiko_eva-0.0.1/tests/eva/assets/core/datasets/embeddings/manifest.csv
--rw-r--r--   0        0        0      129 2024-03-22 13:47:46.637063 kaiko_eva-0.0.1/tests/eva/assets/core/datasets/multi-embeddings/embeddings/tensor_0_shape_6x8.pt
--rw-r--r--   0        0        0      129 2024-03-22 13:47:46.637063 kaiko_eva-0.0.1/tests/eva/assets/core/datasets/multi-embeddings/embeddings/tensor_1_shape_3x8.pt
--rw-r--r--   0        0        0      129 2024-03-22 13:47:46.637063 kaiko_eva-0.0.1/tests/eva/assets/core/datasets/multi-embeddings/embeddings/tensor_2_shape_1x8.pt
--rw-r--r--   0        0        0      129 2024-03-22 13:47:46.637063 kaiko_eva-0.0.1/tests/eva/assets/core/datasets/multi-embeddings/embeddings/tensor_3_shape_2x8.pt
--rw-r--r--   0        0        0      129 2024-03-22 13:47:46.637063 kaiko_eva-0.0.1/tests/eva/assets/core/datasets/multi-embeddings/embeddings/tensor_4_shape_5x8.pt
--rw-r--r--   0        0        0      129 2024-03-22 13:47:46.637063 kaiko_eva-0.0.1/tests/eva/assets/core/datasets/multi-embeddings/embeddings/tensor_5_shape_3x8.pt
--rw-r--r--   0        0        0      129 2024-03-22 13:47:46.637063 kaiko_eva-0.0.1/tests/eva/assets/core/datasets/multi-embeddings/embeddings/tensor_6_shape_1x8.pt
--rw-r--r--   0        0        0      129 2024-03-22 13:47:46.637063 kaiko_eva-0.0.1/tests/eva/assets/core/datasets/multi-embeddings/embeddings/tensor_7_shape_6x8.pt
--rw-r--r--   0        0        0      129 2024-03-22 13:47:46.637063 kaiko_eva-0.0.1/tests/eva/assets/core/datasets/multi-embeddings/embeddings/tensor_8_shape_2x8.pt
--rw-r--r--   0        0        0      129 2024-03-22 13:47:46.637063 kaiko_eva-0.0.1/tests/eva/assets/core/datasets/multi-embeddings/embeddings/tensor_9_shape_5x8.pt
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.637063 kaiko_eva-0.0.1/tests/eva/assets/core/datasets/multi-embeddings/manifest.csv
--rw-r--r--   0        0        0      129 2024-03-22 13:47:46.637063 kaiko_eva-0.0.1/tests/eva/assets/images/random_bgr_32x32.png
--rw-r--r--   0        0        0      129 2024-03-22 13:47:46.637063 kaiko_eva-0.0.1/tests/eva/assets/images/random_grayscale_32x32.png
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.641063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Benign/b001.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.641063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Benign/b002.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.641063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Benign/b003.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.641063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Benign/b004.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.641063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Benign/b005.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.641063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Benign/b006.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.641063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/InSitu/is001.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.641063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/InSitu/is002.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.641063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/InSitu/is003.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.641063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/InSitu/is004.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.641063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/InSitu/is005.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.641063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/InSitu/is006.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.641063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Invasive/iv001.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.641063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Invasive/iv002.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.641063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Invasive/iv003.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.645063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Invasive/iv004.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.645063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Invasive/iv005.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.645063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Invasive/iv006.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.645063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Normal/n001.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.645063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Normal/n002.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.645063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Normal/n003.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.645063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Normal/n004.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.645063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Normal/n005.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.645063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Normal/n006.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.645063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/ADI/ADI-SIHVHHPH.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.645063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/ADI/ADI-SIHWWQMY.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.645063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/BACK/BACK-YYYHKNMK.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.645063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/BACK/BACK-YYYMDTNW.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.645063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/DEB/DEB-YYYRSHLP.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.645063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/DEB/DEB-YYYTCTDR.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.645063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/LYM/LYM-YYWRPGDD.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.649063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/LYM/LYM-YYYTKMWW.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.649063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/MUC/MUC-YYYNWSAM.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.649063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/MUC/MUC-YYYRQDLW.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.649063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/MUS/MUS-YYYNVQVQ.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.649063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/MUS/MUS-YYYRWWNH.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.649063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/NORM/NORM-YYTTIRVD.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.649063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/NORM/NORM-YYVAFTKA.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.649063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/STR/STR-YYYHNSSM.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.649063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/STR/STR-YYYWVWFG.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.649063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/TUM/TUM-YYYSGWYW.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.649063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/TUM/TUM-YYYYQFVN.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.649063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/ADI/ADI-SIHVHHPH.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.649063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/ADI/ADI-SIHWWQMY.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.649063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/BACK/BACK-YYYHKNMK.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.649063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/BACK/BACK-YYYMDTNW.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.649063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/DEB/DEB-YYYRSHLP.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.649063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/DEB/DEB-YYYTCTDR.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.649063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/LYM/LYM-YYWRPGDD.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.649063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/LYM/LYM-YYYTKMWW.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.649063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/MUC/MUC-YYYNWSAM.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.653063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/MUC/MUC-YYYRQDLW.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.653063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/MUS/MUS-YYYNVQVQ.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.653063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/MUS/MUS-YYYRWWNH.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.653063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/NORM/NORM-YYTTIRVD.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.653063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/NORM/NORM-YYVAFTKA.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.653063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/STR/STR-YYYHNSSM.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.653063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/STR/STR-YYYWVWFG.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.653063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/TUM/TUM-YYYSGWYW.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.653063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/TUM/TUM-YYYYQFVN.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.653063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/ADI/ADI-SIHVHHPH.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.653063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/ADI/ADI-SIHWWQMY.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.653063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/BACK/BACK-YYYHKNMK.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.653063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/BACK/BACK-YYYMDTNW.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.653063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/DEB/DEB-YYYRSHLP.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.653063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/DEB/DEB-YYYTCTDR.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.653063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/LYM/LYM-YYWRPGDD.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.653063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/LYM/LYM-YYYTKMWW.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.653063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/MUC/MUC-YYYNWSAM.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.653063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/MUC/MUC-YYYRQDLW.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.653063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/MUS/MUS-YYYNVQVQ.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.653063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/MUS/MUS-YYYRWWNH.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.653063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/NORM/NORM-YYTTIRVD.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.653063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/NORM/NORM-YYVAFTKA.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.653063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/STR/STR-YYYHNSSM.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.653063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/STR/STR-YYYWVWFG.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.657063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/TUM/TUM-YYYSGWYW.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.657063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/TUM/TUM-YYYYQFVN.tif
--rw-r--r--   0        0        0      128 2024-03-22 13:47:46.657063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/mhist/annotations.csv
--rw-r--r--   0        0        0      131 2024-03-22 13:47:46.657063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/mhist/images/MHIST_aaa.png
--rw-r--r--   0        0        0      131 2024-03-22 13:47:46.657063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/mhist/images/MHIST_aab.png
--rw-r--r--   0        0        0      130 2024-03-22 13:47:46.657063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/mhist/images/MHIST_aac.png
--rw-r--r--   0        0        0      131 2024-03-22 13:47:46.657063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/mhist/images/MHIST_aae.png
--rw-r--r--   0        0        0      131 2024-03-22 13:47:46.657063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/mhist/images/MHIST_aaf.png
--rw-r--r--   0        0        0      130 2024-03-22 13:47:46.657063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/mhist/images/MHIST_aag.png
--rw-r--r--   0        0        0      130 2024-03-22 13:47:46.657063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/mhist/images/MHIST_aah.png
--rw-r--r--   0        0        0      130 2024-03-22 13:47:46.657063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/patch_camelyon/camelyonpatch_level_2_split_test_x.h5
--rw-r--r--   0        0        0      129 2024-03-22 13:47:46.657063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/patch_camelyon/camelyonpatch_level_2_split_test_y.h5
--rw-r--r--   0        0        0      131 2024-03-22 13:47:46.657063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/patch_camelyon/camelyonpatch_level_2_split_train_x.h5
--rw-r--r--   0        0        0      129 2024-03-22 13:47:46.657063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/patch_camelyon/camelyonpatch_level_2_split_train_y.h5
--rw-r--r--   0        0        0      130 2024-03-22 13:47:46.657063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/patch_camelyon/camelyonpatch_level_2_split_valid_x.h5
--rw-r--r--   0        0        0      129 2024-03-22 13:47:46.657063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/patch_camelyon/camelyonpatch_level_2_split_valid_y.h5
--rw-r--r--   0        0        0     1790 2024-03-22 13:47:46.657063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0011/ct.nii.gz
--rw-r--r--   0        0        0      153 2024-03-22 13:47:46.657063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0011/segmentations/aorta_small.nii.gz
--rw-r--r--   0        0        0      152 2024-03-22 13:47:46.657063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0011/segmentations/brain_small.nii.gz
--rw-r--r--   0        0        0      152 2024-03-22 13:47:46.657063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0011/segmentations/colon_small.nii.gz
--rw-r--r--   0        0        0     1872 2024-03-22 13:47:46.657063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0461/ct.nii.gz
--rw-r--r--   0        0        0      159 2024-03-22 13:47:46.657063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0461/segmentations/aorta_small.nii.gz
--rw-r--r--   0        0        0      159 2024-03-22 13:47:46.657063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0461/segmentations/brain_small.nii.gz
--rw-r--r--   0        0        0      159 2024-03-22 13:47:46.657063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0461/segmentations/colon_small.nii.gz
--rw-r--r--   0        0        0     1401 2024-03-22 13:47:46.657063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0762/ct.nii.gz
--rw-r--r--   0        0        0      157 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0762/segmentations/aorta_small.nii.gz
--rw-r--r--   0        0        0      157 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0762/segmentations/brain_small.nii.gz
--rw-r--r--   0        0        0      157 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0762/segmentations/colon_small.nii.gz
--rw-r--r--   0        0        0      720 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/conftest.py
--rw-r--r--   0        0        0       41 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/callbacks/__init__.py
--rw-r--r--   0        0        0      991 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/callbacks/conftest.py
--rw-r--r--   0        0        0       34 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/callbacks/writers/__init__.py
--rw-r--r--   0        0        0     3938 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/callbacks/writers/test_embeddings.py
--rw-r--r--   0        0        0       36 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/data/__init__.py
--rw-r--r--   0        0        0       29 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/data/dataloaders/__init__.py
--rw-r--r--   0        0        0     1587 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/data/dataloaders/test_dataloader.py
--rw-r--r--   0        0        0       29 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/data/datamodules/__init__.py
--rw-r--r--   0        0        0      915 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/data/datamodules/_utils.py
--rw-r--r--   0        0        0     2776 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/data/datamodules/test_datamodule.py
--rw-r--r--   0        0        0     1052 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/data/datamodules/test_schemas.py
--rw-r--r--   0        0        0       31 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/data/datasets/__init__.py
--rw-r--r--   0        0        0       46 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/data/datasets/classification/__init__.py
--rw-r--r--   0        0        0     1369 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/data/datasets/classification/test_embedding_datasets.py
--rw-r--r--   0        0        0       39 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/metrics/__init__.py
--rw-r--r--   0        0        0       42 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/metrics/core/__init__.py
--rw-r--r--   0        0        0     1348 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/metrics/core/test_metric_module.py
--rw-r--r--   0        0        0     2000 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/metrics/core/test_schemas.py
--rw-r--r--   0        0        0       35 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/metrics/defaults/__init__.py
--rw-r--r--   0        0        0       60 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/metrics/defaults/classification/__init__.py
--rw-r--r--   0        0        0     1466 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/metrics/defaults/classification/test_binary.py
--rw-r--r--   0        0        0     1712 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/metrics/defaults/classification/test_multiclass.py
--rw-r--r--   0        0        0     1247 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/metrics/test_average_loss.py
--rw-r--r--   0        0        0     1521 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/metrics/test_binary_balanced_accuracy.py
--rw-r--r--   0        0        0       38 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/models/__init__.py
--rw-r--r--   0        0        0       35 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/models/modules/__init__.py
--rw-r--r--   0        0        0     2481 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/models/modules/conftest.py
--rw-r--r--   0        0        0     1383 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/models/modules/test_head.py
--rw-r--r--   0        0        0     1498 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/models/modules/test_inference.py
--rw-r--r--   0        0        0       62 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/models/modules/utils/__init__.py
--rw-r--r--   0        0        0     1985 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/models/modules/utils/test_batch_postproces.py
--rw-r--r--   0        0        0       36 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/models/networks/__init__.py
--rw-r--r--   0        0        0     1741 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/models/networks/test_mlp.py
--rw-r--r--   0        0        0       35 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/models/networks/wrappers/__init__.py
--rw-r--r--   0        0        0     1316 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/models/networks/wrappers/test_from_function.py
--rw-r--r--   0        0        0     1095 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/models/networks/wrappers/test_huggingface.py
--rw-r--r--   0        0        0     1263 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/models/networks/wrappers/test_onnx.py
--rw-r--r--   0        0        0      553 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/test_cli.py
--rw-r--r--   0        0        0       30 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/trainers/__init__.py
--rw-r--r--   0        0        0     4281 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/core/trainers/test_recorder.py
--rw-r--r--   0        0        0       24 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/vision/__init__.py
--rw-r--r--   0        0        0       25 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/vision/data/__init__.py
--rw-r--r--   0        0        0       29 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/vision/data/datasets/__init__.py
--rw-r--r--   0        0        0       51 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/vision/data/datasets/classification/__init__.py
--rw-r--r--   0        0        0     1388 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/vision/data/datasets/classification/test_bach.py
--rw-r--r--   0        0        0     1120 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/vision/data/datasets/classification/test_crc.py
--rw-r--r--   0        0        0     1384 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/vision/data/datasets/classification/test_mhist.py
--rw-r--r--   0        0        0     1371 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/vision/data/datasets/classification/test_patch_camelyon.py
--rw-r--r--   0        0        0     1669 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/vision/data/datasets/classification/test_total_segmentator.py
--rw-r--r--   0        0        0       49 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/vision/data/datasets/segmentation/__init__.py
--rw-r--r--   0        0        0     1624 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/vision/data/datasets/segmentation/test_total_segmentator.py
--rw-r--r--   0        0        0       31 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/vision/data/transforms/__init__.py
--rw-r--r--   0        0        0       42 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/vision/data/transforms/common/__init__.py
--rw-r--r--   0        0        0     1485 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/vision/data/transforms/common/test_resize_and_crop.py
--rw-r--r--   0        0        0       27 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/vision/models/__init__.py
--rw-r--r--   0        0        0       29 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/vision/models/networks/__init__.py
--rw-r--r--   0        0        0     1197 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/vision/models/networks/test_abmil.py
--rw-r--r--   0        0        0     2603 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/vision/test_vision_cli.py
--rw-r--r--   0        0        0       30 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/vision/utils/__init__.py
--rw-r--r--   0        0        0       31 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/vision/utils/io/__init__.py
--rw-r--r--   0        0        0      907 2024-03-22 13:47:46.661063 kaiko_eva-0.0.1/tests/eva/vision/utils/io/test_image.py
--rw-r--r--   0        0        0    22362 1970-01-01 00:00:00.000000 kaiko_eva-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11338 2024-03-21 10:37:52.551410 kaiko_eva-0.0.2/LICENSE
+-rw-r--r--   0        0        0     8740 2024-05-31 08:32:28.383715 kaiko_eva-0.0.2/README.md
+-rw-r--r--   0        0        0     4161 2024-05-31 08:47:39.582621 kaiko_eva-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-05-22 08:02:17.334178 kaiko_eva-0.0.2/src/eva/.DS_Store
+-rw-r--r--   0        0        0      518 2024-04-22 12:25:03.198196 kaiko_eva-0.0.2/src/eva/__init__.py
+-rw-r--r--   0        0        0      282 2024-05-22 13:18:40.826631 kaiko_eva-0.0.2/src/eva/__main__.py
+-rw-r--r--   0        0        0      611 2024-04-22 12:25:03.198612 kaiko_eva-0.0.2/src/eva/__version__.py
+-rw-r--r--   0        0        0      451 2024-05-17 13:54:04.193414 kaiko_eva-0.0.2/src/eva/core/__init__.py
+-rw-r--r--   0        0        0      191 2024-05-29 08:45:49.175163 kaiko_eva-0.0.2/src/eva/core/callbacks/__init__.py
+-rw-r--r--   0        0        0     4267 2024-05-29 08:45:49.175468 kaiko_eva-0.0.2/src/eva/core/callbacks/config.py
+-rw-r--r--   0        0        0      121 2024-05-29 08:45:49.175631 kaiko_eva-0.0.2/src/eva/core/callbacks/writers/__init__.py
+-rw-r--r--   0        0        0     6752 2024-05-29 08:45:49.175925 kaiko_eva-0.0.2/src/eva/core/callbacks/writers/embeddings.py
+-rw-r--r--   0        0        0      616 2024-05-29 08:45:49.176011 kaiko_eva-0.0.2/src/eva/core/callbacks/writers/typings.py
+-rw-r--r--   0        0        0       68 2024-04-22 12:25:03.199436 kaiko_eva-0.0.2/src/eva/core/cli/__init__.py
+-rw-r--r--   0        0        0      422 2024-05-22 13:19:09.082909 kaiko_eva-0.0.2/src/eva/core/cli/cli.py
+-rw-r--r--   0        0        0      786 2024-04-22 12:25:03.199788 kaiko_eva-0.0.2/src/eva/core/cli/logo.py
+-rw-r--r--   0        0        0     2663 2024-05-23 13:12:42.623629 kaiko_eva-0.0.2/src/eva/core/cli/setup.py
+-rw-r--r--   0        0        0      340 2024-04-22 12:25:03.199994 kaiko_eva-0.0.2/src/eva/core/data/__init__.py
+-rw-r--r--   0        0        0      110 2024-04-22 12:25:03.200104 kaiko_eva-0.0.2/src/eva/core/data/dataloaders/__init__.py
+-rw-r--r--   0        0        0     2368 2024-04-22 12:25:03.200193 kaiko_eva-0.0.2/src/eva/core/data/dataloaders/dataloader.py
+-rw-r--r--   0        0        0      229 2024-04-22 12:25:03.200290 kaiko_eva-0.0.2/src/eva/core/data/datamodules/__init__.py
+-rw-r--r--   0        0        0      940 2024-04-22 12:25:03.200554 kaiko_eva-0.0.2/src/eva/core/data/datamodules/call.py
+-rw-r--r--   0        0        0     3878 2024-04-22 12:25:03.200828 kaiko_eva-0.0.2/src/eva/core/data/datamodules/datamodule.py
+-rw-r--r--   0        0        0     1869 2024-04-22 12:25:03.200926 kaiko_eva-0.0.2/src/eva/core/data/datamodules/schemas.py
+-rw-r--r--   0        0        0      387 2024-04-24 08:29:34.869089 kaiko_eva-0.0.2/src/eva/core/data/datasets/__init__.py
+-rw-r--r--   0        0        0     2005 2024-04-22 12:25:03.201129 kaiko_eva-0.0.2/src/eva/core/data/datasets/base.py
+-rw-r--r--   0        0        0      124 2024-04-22 12:25:03.201222 kaiko_eva-0.0.2/src/eva/core/data/datasets/dataset.py
+-rw-r--r--   0        0        0      357 2024-04-24 08:29:34.869239 kaiko_eva-0.0.2/src/eva/core/data/datasets/embeddings/__init__.py
+-rw-r--r--   0        0        0     4979 2024-05-22 10:00:55.312140 kaiko_eva-0.0.2/src/eva/core/data/datasets/embeddings/base.py
+-rw-r--r--   0        0        0      371 2024-04-24 08:29:34.869570 kaiko_eva-0.0.2/src/eva/core/data/datasets/embeddings/classification/__init__.py
+-rw-r--r--   0        0        0     2467 2024-05-29 08:45:49.176180 kaiko_eva-0.0.2/src/eva/core/data/datasets/embeddings/classification/embeddings.py
+-rw-r--r--   0        0        0     4343 2024-05-29 08:45:49.176474 kaiko_eva-0.0.2/src/eva/core/data/datasets/embeddings/classification/multi_embeddings.py
+-rw-r--r--   0        0        0      100 2024-04-22 12:25:03.201861 kaiko_eva-0.0.2/src/eva/core/data/samplers/__init__.py
+-rw-r--r--   0        0        0      119 2024-04-22 12:25:03.201977 kaiko_eva-0.0.2/src/eva/core/data/samplers/sampler.py
+-rw-r--r--   0        0        0      308 2024-05-15 12:30:11.400819 kaiko_eva-0.0.2/src/eva/core/data/transforms/__init__.py
+-rw-r--r--   0        0        0      174 2024-04-22 12:25:03.202212 kaiko_eva-0.0.2/src/eva/core/data/transforms/dtype/__init__.py
+-rw-r--r--   0        0        0      725 2024-04-22 12:25:03.202309 kaiko_eva-0.0.2/src/eva/core/data/transforms/dtype/array.py
+-rw-r--r--   0        0        0      138 2024-04-24 08:29:34.870215 kaiko_eva-0.0.2/src/eva/core/data/transforms/padding/__init__.py
+-rw-r--r--   0        0        0     1185 2024-04-24 08:29:34.870346 kaiko_eva-0.0.2/src/eva/core/data/transforms/padding/pad_2d_tensor.py
+-rw-r--r--   0        0        0      149 2024-04-24 08:29:34.870484 kaiko_eva-0.0.2/src/eva/core/data/transforms/sampling/__init__.py
+-rw-r--r--   0        0        0     1229 2024-04-24 08:29:34.870639 kaiko_eva-0.0.2/src/eva/core/data/transforms/sampling/sample_from_axis.py
+-rw-r--r--   0        0        0       98 2024-04-22 12:25:03.202905 kaiko_eva-0.0.2/src/eva/core/interface/__init__.py
+-rw-r--r--   0        0        0     2741 2024-04-22 12:25:03.203012 kaiko_eva-0.0.2/src/eva/core/interface/interface.py
+-rw-r--r--   0        0        0      266 2024-05-29 08:45:49.176799 kaiko_eva-0.0.2/src/eva/core/loggers/__init__.py
+-rw-r--r--   0        0        0     1204 2024-05-23 12:07:25.681309 kaiko_eva-0.0.2/src/eva/core/loggers/dummy.py
+-rw-r--r--   0        0        0      204 2024-05-29 08:45:49.177266 kaiko_eva-0.0.2/src/eva/core/loggers/experimental_loggers.py
+-rw-r--r--   0        0        0      124 2024-05-29 08:45:49.177553 kaiko_eva-0.0.2/src/eva/core/loggers/log/__init__.py
+-rw-r--r--   0        0        0     1413 2024-05-29 08:45:49.177815 kaiko_eva-0.0.2/src/eva/core/loggers/log/parameters.py
+-rw-r--r--   0        0        0      415 2024-05-29 08:45:49.177971 kaiko_eva-0.0.2/src/eva/core/loggers/log/utils.py
+-rw-r--r--   0        0        0      558 2024-04-22 12:25:03.203549 kaiko_eva-0.0.2/src/eva/core/metrics/__init__.py
+-rw-r--r--   0        0        0     1267 2024-04-22 12:25:03.203663 kaiko_eva-0.0.2/src/eva/core/metrics/average_loss.py
+-rw-r--r--   0        0        0      806 2024-04-22 12:25:03.203780 kaiko_eva-0.0.2/src/eva/core/metrics/binary_balanced_accuracy.py
+-rw-r--r--   0        0        0      301 2024-05-29 07:48:25.823617 kaiko_eva-0.0.2/src/eva/core/metrics/defaults/__init__.py
+-rw-r--r--   0        0        0      316 2024-05-29 07:48:25.823744 kaiko_eva-0.0.2/src/eva/core/metrics/defaults/classification/__init__.py
+-rw-r--r--   0        0        0     2520 2024-05-29 07:48:25.823865 kaiko_eva-0.0.2/src/eva/core/metrics/defaults/classification/binary.py
+-rw-r--r--   0        0        0     2703 2024-05-29 07:48:25.823992 kaiko_eva-0.0.2/src/eva/core/metrics/defaults/classification/multiclass.py
+-rw-r--r--   0        0        0      422 2024-04-22 12:25:03.204328 kaiko_eva-0.0.2/src/eva/core/metrics/structs/__init__.py
+-rw-r--r--   0        0        0      149 2024-04-22 12:25:03.204429 kaiko_eva-0.0.2/src/eva/core/metrics/structs/collection.py
+-rw-r--r--   0        0        0      109 2024-04-22 12:25:03.204521 kaiko_eva-0.0.2/src/eva/core/metrics/structs/metric.py
+-rw-r--r--   0        0        0     3619 2024-04-22 12:25:03.204621 kaiko_eva-0.0.2/src/eva/core/metrics/structs/module.py
+-rw-r--r--   0        0        0     1480 2024-05-29 07:48:25.824123 kaiko_eva-0.0.2/src/eva/core/metrics/structs/schemas.py
+-rw-r--r--   0        0        0      388 2024-04-22 12:25:03.204810 kaiko_eva-0.0.2/src/eva/core/metrics/structs/typings.py
+-rw-r--r--   0        0        0      305 2024-04-22 12:25:03.204924 kaiko_eva-0.0.2/src/eva/core/models/__init__.py
+-rw-r--r--   0        0        0      255 2024-04-22 12:25:03.205039 kaiko_eva-0.0.2/src/eva/core/models/modules/__init__.py
+-rw-r--r--   0        0        0     3992 2024-05-28 07:59:19.140805 kaiko_eva-0.0.2/src/eva/core/models/modules/head.py
+-rw-r--r--   0        0        0      978 2024-04-22 12:25:03.205622 kaiko_eva-0.0.2/src/eva/core/models/modules/inference.py
+-rw-r--r--   0        0        0     6836 2024-05-17 13:54:37.866819 kaiko_eva-0.0.2/src/eva/core/models/modules/module.py
+-rw-r--r--   0        0        0      521 2024-05-29 08:45:49.178109 kaiko_eva-0.0.2/src/eva/core/models/modules/typings.py
+-rw-r--r--   0        0        0      227 2024-04-22 12:25:03.206295 kaiko_eva-0.0.2/src/eva/core/models/modules/utils/__init__.py
+-rw-r--r--   0        0        0     1915 2024-04-22 12:25:03.206572 kaiko_eva-0.0.2/src/eva/core/models/modules/utils/batch_postprocess.py
+-rw-r--r--   0        0        0      706 2024-04-22 12:25:03.206747 kaiko_eva-0.0.2/src/eva/core/models/modules/utils/grad.py
+-rw-r--r--   0        0        0      232 2024-05-29 07:48:25.824386 kaiko_eva-0.0.2/src/eva/core/models/networks/__init__.py
+-rw-r--r--   0        0        0      957 2024-04-22 12:25:03.206951 kaiko_eva-0.0.2/src/eva/core/models/networks/_utils.py
+-rw-r--r--   0        0        0     2411 2024-04-22 12:25:03.207048 kaiko_eva-0.0.2/src/eva/core/models/networks/mlp.py
+-rw-r--r--   0        0        0      159 2024-04-22 12:25:03.207142 kaiko_eva-0.0.2/src/eva/core/models/networks/transforms/__init__.py
+-rw-r--r--   0        0        0      822 2024-04-22 12:25:03.207233 kaiko_eva-0.0.2/src/eva/core/models/networks/transforms/extract_cls_features.py
+-rw-r--r--   0        0        0      381 2024-05-29 07:48:25.824512 kaiko_eva-0.0.2/src/eva/core/models/networks/wrappers/__init__.py
+-rw-r--r--   0        0        0     1320 2024-04-24 07:37:54.647925 kaiko_eva-0.0.2/src/eva/core/models/networks/wrappers/base.py
+-rw-r--r--   0        0        0     2035 2024-04-24 07:37:54.648148 kaiko_eva-0.0.2/src/eva/core/models/networks/wrappers/from_function.py
+-rw-r--r--   0        0        0     1289 2024-04-22 12:25:03.207911 kaiko_eva-0.0.2/src/eva/core/models/networks/wrappers/huggingface.py
+-rw-r--r--   0        0        0     1718 2024-04-22 12:25:03.208008 kaiko_eva-0.0.2/src/eva/core/models/networks/wrappers/onnx.py
+-rw-r--r--   0        0        0      208 2024-04-22 12:25:03.208124 kaiko_eva-0.0.2/src/eva/core/trainers/__init__.py
+-rw-r--r--   0        0        0     2571 2024-04-22 12:25:03.208378 kaiko_eva-0.0.2/src/eva/core/trainers/_logging.py
+-rw-r--r--   0        0        0     7702 2024-04-22 12:25:03.208729 kaiko_eva-0.0.2/src/eva/core/trainers/_recorder.py
+-rw-r--r--   0        0        0      321 2024-04-22 12:25:03.208868 kaiko_eva-0.0.2/src/eva/core/trainers/_utils.py
+-rw-r--r--   0        0        0     4360 2024-04-22 12:25:03.209188 kaiko_eva-0.0.2/src/eva/core/trainers/functional.py
+-rw-r--r--   0        0        0     3949 2024-04-24 08:29:34.871149 kaiko_eva-0.0.2/src/eva/core/trainers/trainer.py
+-rw-r--r--   0        0        0       58 2024-05-29 07:48:25.824651 kaiko_eva-0.0.2/src/eva/core/utils/__init__.py
+-rw-r--r--   0        0        0      112 2024-04-22 12:25:03.209465 kaiko_eva-0.0.2/src/eva/core/utils/io/__init__.py
+-rw-r--r--   0        0        0      509 2024-04-22 12:25:03.209556 kaiko_eva-0.0.2/src/eva/core/utils/io/dataframe.py
+-rw-r--r--   0        0        0     1383 2024-04-22 12:25:03.209678 kaiko_eva-0.0.2/src/eva/core/utils/multiprocessing.py
+-rw-r--r--   0        0        0      634 2024-04-22 12:25:03.209770 kaiko_eva-0.0.2/src/eva/core/utils/workers.py
+-rw-r--r--   0        0        0      438 2024-05-29 07:48:25.824863 kaiko_eva-0.0.2/src/eva/vision/__init__.py
+-rw-r--r--   0        0        0      111 2024-03-21 10:37:52.574125 kaiko_eva-0.0.2/src/eva/vision/data/__init__.py
+-rw-r--r--   0        0        0      402 2024-05-29 07:43:42.047059 kaiko_eva-0.0.2/src/eva/vision/data/datasets/__init__.py
+-rw-r--r--   0        0        0     1430 2024-05-07 09:27:26.760329 kaiko_eva-0.0.2/src/eva/vision/data/datasets/_utils.py
+-rw-r--r--   0        0        0     2099 2024-04-22 12:25:03.210923 kaiko_eva-0.0.2/src/eva/vision/data/datasets/_validators.py
+-rw-r--r--   0        0        0      362 2024-05-29 07:43:42.047398 kaiko_eva-0.0.2/src/eva/vision/data/datasets/classification/__init__.py
+-rw-r--r--   0        0        0     5637 2024-05-29 07:43:20.955020 kaiko_eva-0.0.2/src/eva/vision/data/datasets/classification/bach.py
+-rw-r--r--   0        0        0     3060 2024-05-29 07:43:20.955458 kaiko_eva-0.0.2/src/eva/vision/data/datasets/classification/base.py
+-rw-r--r--   0        0        0     5875 2024-05-29 07:43:20.955621 kaiko_eva-0.0.2/src/eva/vision/data/datasets/classification/crc.py
+-rw-r--r--   0        0        0     3257 2024-05-29 07:43:20.955774 kaiko_eva-0.0.2/src/eva/vision/data/datasets/classification/mhist.py
+-rw-r--r--   0        0        0     7253 2024-05-29 07:43:20.956233 kaiko_eva-0.0.2/src/eva/vision/data/datasets/classification/patch_camelyon.py
+-rw-r--r--   0        0        0      249 2024-05-27 11:19:15.559615 kaiko_eva-0.0.2/src/eva/vision/data/datasets/segmentation/__init__.py
+-rw-r--r--   0        0        0     2937 2024-05-07 09:23:51.252490 kaiko_eva-0.0.2/src/eva/vision/data/datasets/segmentation/base.py
+-rw-r--r--   0        0        0     8705 2024-05-29 07:48:25.825188 kaiko_eva-0.0.2/src/eva/vision/data/datasets/segmentation/total_segmentator.py
+-rw-r--r--   0        0        0      389 2024-04-22 12:25:03.213115 kaiko_eva-0.0.2/src/eva/vision/data/datasets/structs.py
+-rw-r--r--   0        0        0     1100 2024-04-22 12:25:03.213318 kaiko_eva-0.0.2/src/eva/vision/data/datasets/vision.py
+-rw-r--r--   0        0        0      120 2024-05-29 07:48:25.825338 kaiko_eva-0.0.2/src/eva/vision/data/transforms/__init__.py
+-rw-r--r--   0        0        0      138 2024-05-29 07:48:25.825477 kaiko_eva-0.0.2/src/eva/vision/data/transforms/common/__init__.py
+-rw-r--r--   0        0        0     1485 2024-05-29 07:43:20.956465 kaiko_eva-0.0.2/src/eva/vision/data/transforms/common/resize_and_crop.py
+-rw-r--r--   0        0        0     8196 2024-04-22 07:16:26.115886 kaiko_eva-0.0.2/src/eva/vision/models/.DS_Store
+-rw-r--r--   0        0        0       89 2024-04-22 12:25:03.214139 kaiko_eva-0.0.2/src/eva/vision/models/__init__.py
+-rw-r--r--   0        0        0     6148 2024-04-22 07:16:26.117285 kaiko_eva-0.0.2/src/eva/vision/models/networks/.DS_Store
+-rw-r--r--   0        0        0      170 2024-05-29 07:48:25.825608 kaiko_eva-0.0.2/src/eva/vision/models/networks/__init__.py
+-rw-r--r--   0        0        0     6796 2024-04-22 12:25:03.215132 kaiko_eva-0.0.2/src/eva/vision/models/networks/abmil.py
+-rw-r--r--   0        0        0      148 2024-04-22 12:25:03.216523 kaiko_eva-0.0.2/src/eva/vision/models/networks/postprocesses/__init__.py
+-rw-r--r--   0        0        0      822 2024-04-22 12:25:03.216641 kaiko_eva-0.0.2/src/eva/vision/models/networks/postprocesses/cls.py
+-rw-r--r--   0        0        0       96 2024-04-26 09:33:22.807317 kaiko_eva-0.0.2/src/eva/vision/utils/__init__.py
+-rw-r--r--   0        0        0      679 2024-05-29 07:48:25.825780 kaiko_eva-0.0.2/src/eva/vision/utils/convert.py
+-rw-r--r--   0        0        0      310 2024-05-29 07:48:25.825967 kaiko_eva-0.0.2/src/eva/vision/utils/io/__init__.py
+-rw-r--r--   0        0        0      768 2024-03-21 10:37:52.577330 kaiko_eva-0.0.2/src/eva/vision/utils/io/_utils.py
+-rw-r--r--   0        0        0     1489 2024-05-29 07:43:20.957612 kaiko_eva-0.0.2/src/eva/vision/utils/io/image.py
+-rw-r--r--   0        0        0     1659 2024-05-29 07:48:25.826140 kaiko_eva-0.0.2/src/eva/vision/utils/io/nifti.py
+-rw-r--r--   0        0        0      472 2024-03-21 10:37:52.577568 kaiko_eva-0.0.2/src/eva/vision/utils/io/text.py
+-rw-r--r--   0        0        0       17 2024-03-21 10:37:52.577636 kaiko_eva-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-22 12:25:03.217911 kaiko_eva-0.0.2/tests/eva/__init__.py
+-rw-r--r--   0        0        0      841 2024-03-21 10:37:52.577785 kaiko_eva-0.0.2/tests/eva/_cli.py
+-rw-r--r--   0        0        0     1225 2024-04-22 12:25:03.224180 kaiko_eva-0.0.2/tests/eva/assets/core/datasets/embeddings/embeddings/tensor_0_shape_8.pt
+-rw-r--r--   0        0        0     1225 2024-04-22 12:25:03.224522 kaiko_eva-0.0.2/tests/eva/assets/core/datasets/embeddings/embeddings/tensor_1_shape_8.pt
+-rw-r--r--   0        0        0     1225 2024-04-22 12:25:03.224832 kaiko_eva-0.0.2/tests/eva/assets/core/datasets/embeddings/embeddings/tensor_2_shape_8.pt
+-rw-r--r--   0        0        0     1225 2024-04-22 12:25:03.225151 kaiko_eva-0.0.2/tests/eva/assets/core/datasets/embeddings/embeddings/tensor_3_shape_8.pt
+-rw-r--r--   0        0        0     1235 2024-04-22 12:25:03.225803 kaiko_eva-0.0.2/tests/eva/assets/core/datasets/embeddings/embeddings/tensor_4_shape_1x8.pt
+-rw-r--r--   0        0        0     1235 2024-04-22 12:25:03.226119 kaiko_eva-0.0.2/tests/eva/assets/core/datasets/embeddings/embeddings/tensor_5_shape_1x8.pt
+-rw-r--r--   0        0        0     1235 2024-04-22 12:25:03.226422 kaiko_eva-0.0.2/tests/eva/assets/core/datasets/embeddings/embeddings/tensor_6_shape_1x8.pt
+-rw-r--r--   0        0        0     1235 2024-04-22 12:25:03.226716 kaiko_eva-0.0.2/tests/eva/assets/core/datasets/embeddings/embeddings/tensor_7_shape_1x8.pt
+-rw-r--r--   0        0        0      337 2024-04-22 12:25:03.227135 kaiko_eva-0.0.2/tests/eva/assets/core/datasets/embeddings/manifest.csv
+-rw-r--r--   0        0        0     1427 2024-04-22 12:25:03.227482 kaiko_eva-0.0.2/tests/eva/assets/core/datasets/multi-embeddings/embeddings/tensor_0_shape_6x8.pt
+-rw-r--r--   0        0        0     1299 2024-04-22 12:25:03.227697 kaiko_eva-0.0.2/tests/eva/assets/core/datasets/multi-embeddings/embeddings/tensor_1_shape_3x8.pt
+-rw-r--r--   0        0        0     1235 2024-04-22 12:25:03.227989 kaiko_eva-0.0.2/tests/eva/assets/core/datasets/multi-embeddings/embeddings/tensor_2_shape_1x8.pt
+-rw-r--r--   0        0        0     1299 2024-04-22 12:25:03.228354 kaiko_eva-0.0.2/tests/eva/assets/core/datasets/multi-embeddings/embeddings/tensor_3_shape_2x8.pt
+-rw-r--r--   0        0        0     1363 2024-04-22 12:25:03.228615 kaiko_eva-0.0.2/tests/eva/assets/core/datasets/multi-embeddings/embeddings/tensor_4_shape_5x8.pt
+-rw-r--r--   0        0        0     1299 2024-04-22 12:25:03.228917 kaiko_eva-0.0.2/tests/eva/assets/core/datasets/multi-embeddings/embeddings/tensor_5_shape_3x8.pt
+-rw-r--r--   0        0        0     1235 2024-04-22 12:25:03.229128 kaiko_eva-0.0.2/tests/eva/assets/core/datasets/multi-embeddings/embeddings/tensor_6_shape_1x8.pt
+-rw-r--r--   0        0        0     1427 2024-04-22 12:25:03.229414 kaiko_eva-0.0.2/tests/eva/assets/core/datasets/multi-embeddings/embeddings/tensor_7_shape_6x8.pt
+-rw-r--r--   0        0        0     1299 2024-04-22 12:25:03.232354 kaiko_eva-0.0.2/tests/eva/assets/core/datasets/multi-embeddings/embeddings/tensor_8_shape_2x8.pt
+-rw-r--r--   0        0        0     1363 2024-04-22 12:25:03.232710 kaiko_eva-0.0.2/tests/eva/assets/core/datasets/multi-embeddings/embeddings/tensor_9_shape_5x8.pt
+-rw-r--r--   0        0        0      514 2024-04-22 12:25:03.233049 kaiko_eva-0.0.2/tests/eva/assets/core/datasets/multi-embeddings/manifest.csv
+-rw-r--r--   0        0        0     3172 2024-03-21 10:37:52.788456 kaiko_eva-0.0.2/tests/eva/assets/images/random_bgr_32x32.png
+-rw-r--r--   0        0        0     1124 2024-03-21 10:37:52.788844 kaiko_eva-0.0.2/tests/eva/assets/images/random_grayscale_32x32.png
+-rw-r--r--   0        0        0      908 2024-03-21 10:37:52.789534 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Benign/b001.tif
+-rw-r--r--   0        0        0      908 2024-03-21 10:37:52.790074 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Benign/b002.tif
+-rw-r--r--   0        0        0      908 2024-03-21 10:37:52.790354 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Benign/b003.tif
+-rw-r--r--   0        0        0      908 2024-03-21 10:37:52.790738 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Benign/b004.tif
+-rw-r--r--   0        0        0      908 2024-03-21 10:37:52.791443 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Benign/b005.tif
+-rw-r--r--   0        0        0      908 2024-03-21 10:37:52.791569 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Benign/b006.tif
+-rw-r--r--   0        0        0      908 2024-03-21 10:37:52.791884 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/InSitu/is001.tif
+-rw-r--r--   0        0        0      908 2024-03-21 10:37:52.792162 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/InSitu/is002.tif
+-rw-r--r--   0        0        0      908 2024-03-21 10:37:52.792479 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/InSitu/is003.tif
+-rw-r--r--   0        0        0      908 2024-03-21 10:37:52.792668 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/InSitu/is004.tif
+-rw-r--r--   0        0        0      908 2024-03-21 10:37:52.792934 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/InSitu/is005.tif
+-rw-r--r--   0        0        0      908 2024-03-21 10:37:52.793056 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/InSitu/is006.tif
+-rw-r--r--   0        0        0      908 2024-03-21 10:37:52.793470 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Invasive/iv001.tif
+-rw-r--r--   0        0        0      908 2024-03-21 10:37:52.793726 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Invasive/iv002.tif
+-rw-r--r--   0        0        0      908 2024-03-21 10:37:52.794015 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Invasive/iv003.tif
+-rw-r--r--   0        0        0      908 2024-03-21 10:37:52.794287 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Invasive/iv004.tif
+-rw-r--r--   0        0        0      908 2024-03-21 10:37:52.794596 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Invasive/iv005.tif
+-rw-r--r--   0        0        0      908 2024-03-21 10:37:52.794739 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Invasive/iv006.tif
+-rw-r--r--   0        0        0      908 2024-03-21 10:37:52.795240 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Normal/n001.tif
+-rw-r--r--   0        0        0      908 2024-03-21 10:37:52.795521 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Normal/n002.tif
+-rw-r--r--   0        0        0      908 2024-03-21 10:37:52.795799 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Normal/n003.tif
+-rw-r--r--   0        0        0      908 2024-03-21 10:37:52.796073 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Normal/n004.tif
+-rw-r--r--   0        0        0      908 2024-03-21 10:37:52.796629 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Normal/n005.tif
+-rw-r--r--   0        0        0      908 2024-03-21 10:37:52.796810 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/bach/ICIAR2018_BACH_Challenge/Photos/Normal/n006.tif
+-rw-r--r--   0        0        0      652 2024-03-21 10:37:52.797282 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/ADI/ADI-SIHVHHPH.tif
+-rw-r--r--   0        0        0      654 2024-03-21 10:37:52.797698 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/ADI/ADI-SIHWWQMY.tif
+-rw-r--r--   0        0        0      922 2024-03-21 10:37:52.797998 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/BACK/BACK-YYYHKNMK.tif
+-rw-r--r--   0        0        0      182 2024-03-21 10:37:52.798391 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/BACK/BACK-YYYMDTNW.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.798697 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/DEB/DEB-YYYRSHLP.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.798953 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/DEB/DEB-YYYTCTDR.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.799492 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/LYM/LYM-YYWRPGDD.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.799721 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/LYM/LYM-YYYTKMWW.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.800053 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/MUC/MUC-YYYNWSAM.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.800327 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/MUC/MUC-YYYRQDLW.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.800645 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/MUS/MUS-YYYNVQVQ.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.800906 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/MUS/MUS-YYYRWWNH.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.801378 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/NORM/NORM-YYTTIRVD.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.801621 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/NORM/NORM-YYVAFTKA.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.801922 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/STR/STR-YYYHNSSM.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.802407 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/STR/STR-YYYWVWFG.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.802657 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/TUM/TUM-YYYSGWYW.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.802918 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/CRC-VAL-HE-7K/TUM/TUM-YYYYQFVN.tif
+-rw-r--r--   0        0        0      652 2024-03-21 10:37:52.803126 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/ADI/ADI-SIHVHHPH.tif
+-rw-r--r--   0        0        0      654 2024-03-21 10:37:52.803239 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/ADI/ADI-SIHWWQMY.tif
+-rw-r--r--   0        0        0      922 2024-03-21 10:37:52.803402 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/BACK/BACK-YYYHKNMK.tif
+-rw-r--r--   0        0        0      182 2024-03-21 10:37:52.803519 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/BACK/BACK-YYYMDTNW.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.803671 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/DEB/DEB-YYYRSHLP.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.803800 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/DEB/DEB-YYYTCTDR.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.803956 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/LYM/LYM-YYWRPGDD.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.804074 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/LYM/LYM-YYYTKMWW.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.804249 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/MUC/MUC-YYYNWSAM.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.804370 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/MUC/MUC-YYYRQDLW.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.804577 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/MUS/MUS-YYYNVQVQ.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.804728 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/MUS/MUS-YYYRWWNH.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.804976 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/NORM/NORM-YYTTIRVD.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.805159 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/NORM/NORM-YYVAFTKA.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.805381 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/STR/STR-YYYHNSSM.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.805757 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/STR/STR-YYYWVWFG.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.805974 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/TUM/TUM-YYYSGWYW.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.806132 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K-NONORM/TUM/TUM-YYYYQFVN.tif
+-rw-r--r--   0        0        0      652 2024-03-21 10:37:52.806345 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/ADI/ADI-SIHVHHPH.tif
+-rw-r--r--   0        0        0      654 2024-03-21 10:37:52.806536 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/ADI/ADI-SIHWWQMY.tif
+-rw-r--r--   0        0        0      922 2024-03-21 10:37:52.806703 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/BACK/BACK-YYYHKNMK.tif
+-rw-r--r--   0        0        0      182 2024-03-21 10:37:52.806823 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/BACK/BACK-YYYMDTNW.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.806990 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/DEB/DEB-YYYRSHLP.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.807135 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/DEB/DEB-YYYTCTDR.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.807349 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/LYM/LYM-YYWRPGDD.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.807488 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/LYM/LYM-YYYTKMWW.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.807650 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/MUC/MUC-YYYNWSAM.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.807777 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/MUC/MUC-YYYRQDLW.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.807943 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/MUS/MUS-YYYNVQVQ.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.808075 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/MUS/MUS-YYYRWWNH.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.808250 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/NORM/NORM-YYTTIRVD.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.808410 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/NORM/NORM-YYVAFTKA.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.808584 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/STR/STR-YYYHNSSM.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.808923 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/STR/STR-YYYWVWFG.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.809162 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/TUM/TUM-YYYSGWYW.tif
+-rw-r--r--   0        0        0      924 2024-03-21 10:37:52.809308 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/crc/NCT-CRC-HE-100K/TUM/TUM-YYYYQFVN.tif
+-rw-r--r--   0        0        0      266 2024-03-21 10:37:52.809575 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/mhist/annotations.csv
+-rw-r--r--   0        0        0   107906 2024-03-21 10:37:52.810489 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/mhist/images/MHIST_aaa.png
+-rw-r--r--   0        0        0   134779 2024-03-21 10:37:52.811112 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/mhist/images/MHIST_aab.png
+-rw-r--r--   0        0        0    82282 2024-03-21 10:37:52.811676 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/mhist/images/MHIST_aac.png
+-rw-r--r--   0        0        0   107100 2024-03-21 10:37:52.812297 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/mhist/images/MHIST_aae.png
+-rw-r--r--   0        0        0   133438 2024-03-21 10:37:52.812578 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/mhist/images/MHIST_aaf.png
+-rw-r--r--   0        0        0    80812 2024-03-21 10:37:52.813164 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/mhist/images/MHIST_aag.png
+-rw-r--r--   0        0        0    79468 2024-03-21 10:37:52.813740 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/mhist/images/MHIST_aah.png
+-rw-r--r--   0        0        0    29696 2024-03-21 10:37:52.814095 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/patch_camelyon/camelyonpatch_level_2_split_test_x.h5
+-rw-r--r--   0        0        0     2049 2024-03-21 10:37:52.814377 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/patch_camelyon/camelyonpatch_level_2_split_test_y.h5
+-rw-r--r--   0        0        0   112640 2024-03-21 10:37:52.815064 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/patch_camelyon/camelyonpatch_level_2_split_train_x.h5
+-rw-r--r--   0        0        0     2052 2024-03-21 10:37:52.815502 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/patch_camelyon/camelyonpatch_level_2_split_train_y.h5
+-rw-r--r--   0        0        0    57344 2024-03-21 10:37:52.815988 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/patch_camelyon/camelyonpatch_level_2_split_valid_x.h5
+-rw-r--r--   0        0        0     2050 2024-03-21 10:37:52.816272 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/patch_camelyon/camelyonpatch_level_2_split_valid_y.h5
+-rw-r--r--   0        0        0     1790 2024-03-21 10:37:52.816511 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0011/ct.nii.gz
+-rw-r--r--   0        0        0      153 2024-03-21 10:37:52.816641 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0011/segmentations/aorta_small.nii.gz
+-rw-r--r--   0        0        0      152 2024-03-21 10:37:52.816723 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0011/segmentations/brain_small.nii.gz
+-rw-r--r--   0        0        0      152 2024-03-21 10:37:52.816793 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0011/segmentations/colon_small.nii.gz
+-rw-r--r--   0        0        0       79 2024-05-29 07:43:42.048444 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0011/segmentations/semantic_labels/masks.nii.gz
+-rw-r--r--   0        0        0     1872 2024-03-21 10:37:52.816901 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0461/ct.nii.gz
+-rw-r--r--   0        0        0      159 2024-03-21 10:37:52.817018 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0461/segmentations/aorta_small.nii.gz
+-rw-r--r--   0        0        0      159 2024-03-21 10:37:52.817085 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0461/segmentations/brain_small.nii.gz
+-rw-r--r--   0        0        0      159 2024-03-21 10:37:52.817155 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0461/segmentations/colon_small.nii.gz
+-rw-r--r--   0        0        0       79 2024-05-29 07:43:42.048668 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0461/segmentations/semantic_labels/masks.nii.gz
+-rw-r--r--   0        0        0     1401 2024-03-21 10:37:52.817257 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0762/ct.nii.gz
+-rw-r--r--   0        0        0      157 2024-03-21 10:37:52.817365 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0762/segmentations/aorta_small.nii.gz
+-rw-r--r--   0        0        0      157 2024-03-21 10:37:52.817436 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0762/segmentations/brain_small.nii.gz
+-rw-r--r--   0        0        0      157 2024-03-21 10:37:52.817501 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0762/segmentations/colon_small.nii.gz
+-rw-r--r--   0        0        0       79 2024-05-29 07:43:42.048857 kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0762/segmentations/semantic_labels/masks.nii.gz
+-rw-r--r--   0        0        0      720 2024-03-21 10:37:52.817589 kaiko_eva-0.0.2/tests/eva/conftest.py
+-rw-r--r--   0        0        0       41 2024-04-22 12:25:03.233181 kaiko_eva-0.0.2/tests/eva/core/callbacks/__init__.py
+-rw-r--r--   0        0        0      991 2024-04-22 12:25:03.233471 kaiko_eva-0.0.2/tests/eva/core/callbacks/conftest.py
+-rw-r--r--   0        0        0       34 2024-04-22 12:25:03.233579 kaiko_eva-0.0.2/tests/eva/core/callbacks/writers/__init__.py
+-rw-r--r--   0        0        0     3938 2024-05-29 08:45:49.178383 kaiko_eva-0.0.2/tests/eva/core/callbacks/writers/test_embeddings.py
+-rw-r--r--   0        0        0       36 2024-04-22 12:25:03.233963 kaiko_eva-0.0.2/tests/eva/core/data/__init__.py
+-rw-r--r--   0        0        0       29 2024-04-22 12:25:03.234055 kaiko_eva-0.0.2/tests/eva/core/data/dataloaders/__init__.py
+-rw-r--r--   0        0        0     1587 2024-04-22 12:25:03.234145 kaiko_eva-0.0.2/tests/eva/core/data/dataloaders/test_dataloader.py
+-rw-r--r--   0        0        0       29 2024-04-22 12:25:03.234234 kaiko_eva-0.0.2/tests/eva/core/data/datamodules/__init__.py
+-rw-r--r--   0        0        0      915 2024-04-22 12:25:03.234322 kaiko_eva-0.0.2/tests/eva/core/data/datamodules/_utils.py
+-rw-r--r--   0        0        0     2776 2024-04-22 12:25:03.234408 kaiko_eva-0.0.2/tests/eva/core/data/datamodules/test_datamodule.py
+-rw-r--r--   0        0        0     1052 2024-04-22 12:25:03.234490 kaiko_eva-0.0.2/tests/eva/core/data/datamodules/test_schemas.py
+-rw-r--r--   0        0        0       31 2024-04-22 12:25:03.234575 kaiko_eva-0.0.2/tests/eva/core/data/datasets/__init__.py
+-rw-r--r--   0        0        0       37 2024-04-24 08:29:34.872907 kaiko_eva-0.0.2/tests/eva/core/data/datasets/embeddings/__init__.py
+-rw-r--r--   0        0        0       52 2024-04-24 08:29:34.873030 kaiko_eva-0.0.2/tests/eva/core/data/datasets/embeddings/classification/__init__.py
+-rw-r--r--   0        0        0     1436 2024-04-24 08:29:34.873160 kaiko_eva-0.0.2/tests/eva/core/data/datasets/embeddings/classification/test_embeddings.py
+-rw-r--r--   0        0        0     3403 2024-04-24 08:29:34.873276 kaiko_eva-0.0.2/tests/eva/core/data/datasets/embeddings/classification/test_multi_embeddings.py
+-rw-r--r--   0        0        0       33 2024-04-24 08:29:34.873403 kaiko_eva-0.0.2/tests/eva/core/data/transforms/__init__.py
+-rw-r--r--   0        0        0       36 2024-04-24 08:29:34.873516 kaiko_eva-0.0.2/tests/eva/core/data/transforms/padding/__init__.py
+-rw-r--r--   0        0        0     1619 2024-04-24 08:29:34.873634 kaiko_eva-0.0.2/tests/eva/core/data/transforms/padding/test_pad_2d_tensor.py
+-rw-r--r--   0        0        0       37 2024-04-24 08:29:34.873750 kaiko_eva-0.0.2/tests/eva/core/data/transforms/sampling/__init__.py
+-rw-r--r--   0        0        0     2648 2024-04-24 08:29:34.873870 kaiko_eva-0.0.2/tests/eva/core/data/transforms/sampling/test_sample_from_axis.py
+-rw-r--r--   0        0        0       39 2024-04-22 12:25:03.235765 kaiko_eva-0.0.2/tests/eva/core/metrics/__init__.py
+-rw-r--r--   0        0        0       42 2024-04-22 12:25:03.235849 kaiko_eva-0.0.2/tests/eva/core/metrics/core/__init__.py
+-rw-r--r--   0        0        0     1348 2024-04-22 12:25:03.235941 kaiko_eva-0.0.2/tests/eva/core/metrics/core/test_metric_module.py
+-rw-r--r--   0        0        0     2000 2024-04-22 12:25:03.236036 kaiko_eva-0.0.2/tests/eva/core/metrics/core/test_schemas.py
+-rw-r--r--   0        0        0       35 2024-04-22 12:25:03.236125 kaiko_eva-0.0.2/tests/eva/core/metrics/defaults/__init__.py
+-rw-r--r--   0        0        0       60 2024-04-22 12:25:03.236212 kaiko_eva-0.0.2/tests/eva/core/metrics/defaults/classification/__init__.py
+-rw-r--r--   0        0        0     1466 2024-04-22 12:25:03.236321 kaiko_eva-0.0.2/tests/eva/core/metrics/defaults/classification/test_binary.py
+-rw-r--r--   0        0        0     1712 2024-04-22 12:25:03.236488 kaiko_eva-0.0.2/tests/eva/core/metrics/defaults/classification/test_multiclass.py
+-rw-r--r--   0        0        0     1247 2024-04-22 12:25:03.236600 kaiko_eva-0.0.2/tests/eva/core/metrics/test_average_loss.py
+-rw-r--r--   0        0        0     1521 2024-04-22 12:25:03.236697 kaiko_eva-0.0.2/tests/eva/core/metrics/test_binary_balanced_accuracy.py
+-rw-r--r--   0        0        0       38 2024-04-22 12:25:03.236787 kaiko_eva-0.0.2/tests/eva/core/models/__init__.py
+-rw-r--r--   0        0        0       35 2024-04-22 12:25:03.236875 kaiko_eva-0.0.2/tests/eva/core/models/modules/__init__.py
+-rw-r--r--   0        0        0     2481 2024-04-22 12:25:03.237120 kaiko_eva-0.0.2/tests/eva/core/models/modules/conftest.py
+-rw-r--r--   0        0        0     1383 2024-05-29 07:48:25.826285 kaiko_eva-0.0.2/tests/eva/core/models/modules/test_head.py
+-rw-r--r--   0        0        0     1498 2024-05-29 07:48:25.826417 kaiko_eva-0.0.2/tests/eva/core/models/modules/test_inference.py
+-rw-r--r--   0        0        0       62 2024-04-22 12:25:03.237398 kaiko_eva-0.0.2/tests/eva/core/models/modules/utils/__init__.py
+-rw-r--r--   0        0        0     1985 2024-04-22 12:25:03.237490 kaiko_eva-0.0.2/tests/eva/core/models/modules/utils/test_batch_postproces.py
+-rw-r--r--   0        0        0       36 2024-04-22 12:25:03.237578 kaiko_eva-0.0.2/tests/eva/core/models/networks/__init__.py
+-rw-r--r--   0        0        0     1741 2024-04-22 12:25:03.237697 kaiko_eva-0.0.2/tests/eva/core/models/networks/test_mlp.py
+-rw-r--r--   0        0        0       35 2024-04-22 12:25:03.237793 kaiko_eva-0.0.2/tests/eva/core/models/networks/wrappers/__init__.py
+-rw-r--r--   0        0        0     1316 2024-04-22 12:25:03.237877 kaiko_eva-0.0.2/tests/eva/core/models/networks/wrappers/test_from_function.py
+-rw-r--r--   0        0        0     1095 2024-04-22 12:25:03.237976 kaiko_eva-0.0.2/tests/eva/core/models/networks/wrappers/test_huggingface.py
+-rw-r--r--   0        0        0     1263 2024-04-22 12:25:03.238155 kaiko_eva-0.0.2/tests/eva/core/models/networks/wrappers/test_onnx.py
+-rw-r--r--   0        0        0      553 2024-04-22 12:25:03.238434 kaiko_eva-0.0.2/tests/eva/core/test_cli.py
+-rw-r--r--   0        0        0       30 2024-04-22 12:25:03.238533 kaiko_eva-0.0.2/tests/eva/core/trainers/__init__.py
+-rw-r--r--   0        0        0     4281 2024-04-22 12:25:03.238914 kaiko_eva-0.0.2/tests/eva/core/trainers/test_recorder.py
+-rw-r--r--   0        0        0       24 2024-03-21 10:37:52.821807 kaiko_eva-0.0.2/tests/eva/vision/__init__.py
+-rw-r--r--   0        0        0       25 2024-03-21 10:37:52.821891 kaiko_eva-0.0.2/tests/eva/vision/data/__init__.py
+-rw-r--r--   0        0        0       29 2024-03-21 10:37:52.821970 kaiko_eva-0.0.2/tests/eva/vision/data/datasets/__init__.py
+-rw-r--r--   0        0        0       51 2024-03-21 10:37:52.822052 kaiko_eva-0.0.2/tests/eva/vision/data/datasets/classification/__init__.py
+-rw-r--r--   0        0        0     1388 2024-05-29 07:43:20.957943 kaiko_eva-0.0.2/tests/eva/vision/data/datasets/classification/test_bach.py
+-rw-r--r--   0        0        0     1120 2024-05-29 07:43:20.958469 kaiko_eva-0.0.2/tests/eva/vision/data/datasets/classification/test_crc.py
+-rw-r--r--   0        0        0     1384 2024-05-29 07:43:20.958629 kaiko_eva-0.0.2/tests/eva/vision/data/datasets/classification/test_mhist.py
+-rw-r--r--   0        0        0     1371 2024-05-29 07:43:20.958770 kaiko_eva-0.0.2/tests/eva/vision/data/datasets/classification/test_patch_camelyon.py
+-rw-r--r--   0        0        0       49 2024-03-21 10:37:52.822863 kaiko_eva-0.0.2/tests/eva/vision/data/datasets/segmentation/__init__.py
+-rw-r--r--   0        0        0     1689 2024-05-10 08:24:52.648259 kaiko_eva-0.0.2/tests/eva/vision/data/datasets/segmentation/test_total_segmentator.py
+-rw-r--r--   0        0        0       31 2024-03-21 10:37:52.823001 kaiko_eva-0.0.2/tests/eva/vision/data/transforms/__init__.py
+-rw-r--r--   0        0        0       42 2024-03-21 10:37:52.823078 kaiko_eva-0.0.2/tests/eva/vision/data/transforms/common/__init__.py
+-rw-r--r--   0        0        0     1485 2024-05-29 07:43:20.959125 kaiko_eva-0.0.2/tests/eva/vision/data/transforms/common/test_resize_and_crop.py
+-rw-r--r--   0        0        0       27 2024-03-21 10:37:52.823242 kaiko_eva-0.0.2/tests/eva/vision/models/__init__.py
+-rw-r--r--   0        0        0       29 2024-03-21 10:37:52.823318 kaiko_eva-0.0.2/tests/eva/vision/models/networks/__init__.py
+-rw-r--r--   0        0        0     1197 2024-03-21 10:37:52.823396 kaiko_eva-0.0.2/tests/eva/vision/models/networks/test_abmil.py
+-rw-r--r--   0        0        0     2603 2024-05-28 10:45:18.416575 kaiko_eva-0.0.2/tests/eva/vision/test_vision_cli.py
+-rw-r--r--   0        0        0       30 2024-03-21 10:37:52.823551 kaiko_eva-0.0.2/tests/eva/vision/utils/__init__.py
+-rw-r--r--   0        0        0       31 2024-03-21 10:37:52.823619 kaiko_eva-0.0.2/tests/eva/vision/utils/io/__init__.py
+-rw-r--r--   0        0        0      907 2024-03-21 10:37:52.823698 kaiko_eva-0.0.2/tests/eva/vision/utils/io/test_image.py
+-rw-r--r--   0        0        0     1051 2024-05-29 07:48:25.826582 kaiko_eva-0.0.2/tests/eva/vision/utils/test_convert.py
+-rw-r--r--   0        0        0    23562 1970-01-01 00:00:00.000000 kaiko_eva-0.0.2/PKG-INFO
```

### Comparing `kaiko_eva-0.0.1/LICENSE` & `kaiko_eva-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/README.md` & `kaiko_eva-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 <div align="center">
 
-<img src="https://github.com/kaiko-ai/eva/blob/main/docs/images/eva-logo.png?raw=true" width="400">
+<br />
+
+<img src="https://github.com/kaiko-ai/eva/blob/main/docs/images/eva-logo.png?raw=true" width="340">
 
 <br />
+<br />
 
 _Oncology FM Evaluation Framework by kaiko.ai_
 
 [![PyPI](https://img.shields.io/pypi/v/kaiko-eva.svg?logo=python)](https://pypi.python.org/pypi/kaiko-eva)
-[![CI](https://github.com/kaiko-ai/eva/workflows/CI/badge.svg)](https://github.com/kaiko-ai/eva/actions?query=workflow%3ACI)
-[![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg?labelColor=gray)](https://github.com/kaiko-ai/eva#license)
+[![docs](https://img.shields.io/badge/📚_docs-latest-green)](https://kaiko-ai.github.io/eva/latest)
+[![license](https://img.shields.io/badge/⚖️_License-Apache%202.0-blue.svg?labelColor=gray)](https://github.com/kaiko-ai/eva#license)<br>
+[![paper](http://img.shields.io/badge/OpenReview-MIDL_2024-B31B1B.svg)](https://openreview.net/forum?id=FNBQOPj18N&noteId=FNBQOPj18N)
 
 <p align="center">
   <a href="https://github.com/kaiko-ai/eva#installation">Installation</a> •
   <a href="https://github.com/kaiko-ai/eva#how-to-use">How To Use</a> •
   <a href="https://kaiko-ai.github.io/eva/">Documentation</a> •
   <a href="https://kaiko-ai.github.io/eva/dev/datasets/">Datasets</a> •
   <a href="https://github.com/kaiko-ai/eva#benchmarks">Benchmarks</a> <br>
@@ -55,26 +59,26 @@
 You can verify that the installation was successful by executing:
 ```sh
 eva --version
 ```
 
 ## How To Use
 
-_eva_ can be used directly from the terminal as a CLI tool as follows:
+_`eva`_ can be used directly from the terminal as a CLI tool as follows:
 ```sh
 eva {fit,predict,predict_fit} --config url/or/path/to/the/config.yaml 
 ```
 
-When used as a CLI tool, `_eva_` supports configuration files (`.yaml`) as an argument to define its functionality.
+When used as a CLI tool, _`eva`_ supports configuration files (`.yaml`) as an argument to define its functionality.
 Native supported configs can be found at the [configs](https://github.com/kaiko-ai/eva/tree/main/configs) directory
 of the repo. Apart from cloning the repo, you can download the latest config folder as `.zip` from your browser from
 [here](https://download-directory.github.io/?url=https://github.com/kaiko-ai/eva/tree/main/configs). Alternatively,
 from a specific release the configs can be downloaded from the terminal as follows:
 ```sh
-curl -LO https://github.com/kaiko-ai/eva/releases/download/0.0.1/configs.zip | unzip configs.zip
+curl -LO https://github.com/kaiko-ai/eva/releases/download/0.0.1/configs.zip | unzip configs
 ```
 
 For example, to perform a downstream evaluation of DINO ViT-S/16 on the BACH dataset with
 linear probing by first inferring the embeddings and performing 5 sequential fits, execute:
 ```sh
 # from a locally stored config file
 eva predict_fit --config ./configs/vision/dino_vit/offline/bach.yaml
@@ -94,51 +98,54 @@
 ```
 
 For more information, please refer to the [documentation](https://kaiko-ai.github.io/eva/dev/user-guide/tutorials/offline_vs_online/)
 and [tutorials](https://kaiko-ai.github.io/eva/dev/user-guide/advanced/replicate_evaluations/).
 
 ## Benchmarks
 
-In this section you will find model benchmarks which were generated with _eva_.
+In this section you will find model benchmarks which were generated with _`eva`_.
 
 ### Table I: WSI patch-level benchmark
 
 <br />
 
 <div align="center">
 
 | Model                                            | BACH  | CRC   | MHIST | PCam/val | PCam/test |
 |--------------------------------------------------|-------|-------|-------|----------|-----------|
 | ViT-S/16 _(random)_	<sup>[1]</sup>               | 0.410 | 0.617 | 0.501 | 0.753    | 0.728     |
 | ViT-S/16 _(ImageNet)_ <sup>[1]</sup>             | 0.695 | 0.935 | 0.831 | 0.864    | 0.849     |
 | ViT-B/8 _(ImageNet)_ <sup>[1]</sup>              | 0.710 | 0.939 | 0.814 | 0.870    | 0.856     |
+| ViT-L/14 _(ImageNet)_ <sup>[1]</sup>             | 0.707 | 0.916 | 0.832 | 0.873    | 0.888     |
 | DINO<sub>(p=16)</sub> <sup>[2]</sup>             | 0.801 | 0.934 | 0.768 | 0.889    | 0.895     |
 | Phikon <sup>[3]</sup>                            | 0.725 | 0.935 | 0.777 | 0.912    | 0.915     |
-| ViT-S/16 _(kaiko.ai)_ <sup>[4]</sup>             | 0.797 | 0.943 | 0.828 | 0.903    | 0.893     |
-| ViT-S/8 _(kaiko.ai)_ <sup>[4]</sup>              | 0.834 | 0.946 | 0.832 | 0.897    | 0.887     |
-| ViT-B/16 _(kaiko.ai)_	<sup>[4]</sup>             | 0.810 | 0.960 | 0.826 | 0.900    | 0.898     |
-| ViT-B/8 _(kaiko.ai)_ <sup>[4]</sup>              | 0.865 | 0.956 | 0.809 | 0.913    | 0.921     |
-| ViT-L/14 _(kaiko.ai)_ <sup>[4]</sup>             | 0.870 | 0.930 | 0.809 | 0.908    | 0.898     |
+| UNI <sup>[4]</sup>                               | 0.814 | 0.950 | 0.837 | 0.936    | 0.938     |
+| ViT-S/16 _(kaiko.ai)_ <sup>[5]</sup>             | 0.797 | 0.943 | 0.828 | 0.903    | 0.893     |
+| ViT-S/8 _(kaiko.ai)_ <sup>[5]</sup>              | 0.834 | 0.946 | 0.832 | 0.897    | 0.887     |
+| ViT-B/16 _(kaiko.ai)_	<sup>[5]</sup>             | 0.810 | 0.960 | 0.826 | 0.900    | 0.898     |
+| ViT-B/8 _(kaiko.ai)_ <sup>[5]</sup>              | 0.865 | 0.956 | 0.809 | 0.913    | 0.921     |
+| ViT-L/14 _(kaiko.ai)_ <sup>[5]</sup>             | 0.870 | 0.930 | 0.809 | 0.908    | 0.898     |
 
 _Table I: Linear probing evaluation of FMs on patch-level downstream datasets.<br> We report averaged balanced accuracy
 over 5 runs, with an average standard deviation of ±0.003._
 
 </div>
 
 <br />
 
 _References_:
-1. _"Emerging properties in self-supervised vision transformers”_
-2. _"Benchmarking self-supervised learning on diverse pathology datasets”_
-3. _"Scaling self-supervised learning for histopathology with masked image modeling”_
-4. _"Towards Training Large-Scale Pathology Foundation Models: from TCGA to Hospital Scale”_
+1. _"Emerging properties in self-supervised vision transformers”_, [arXiv](https://arxiv.org/abs/2104.14294)
+2. _"Benchmarking self-supervised learning on diverse pathology datasets”_, [arXiv](https://arxiv.org/abs/2212.04690)
+3. _"Scaling self-supervised learning for histopathology with masked image modeling”_, [medRxiv](https://www.medrxiv.org/content/10.1101/2023.07.21.23292757v1)
+4. _"A General-Purpose Self-Supervised Model for Computational Pathology”_, [arXiv](https://arxiv.org/abs/2308.15474)
+5. _"Towards Training Large-Scale Pathology Foundation Models: from TCGA to Hospital Scale”_, [arXiv](https://arxiv.org/pdf/2404.15217)
 
 ## Contributing
 
-_eva_ is an open source project and welcomes contributions of all kinds. Please checkout the [developer](./docs/DEVELOPER_GUIDE.md)
+_`eva`_ is an open source project and welcomes contributions of all kinds. Please checkout the [developer](./docs/DEVELOPER_GUIDE.md)
 and [contributing guide](./docs/CONTRIBUTING.md) for help on how to do so.
 
 All contributors must follow the [code of conduct](./docs/CODE_OF_CONDUCT.md).
 
 
 ## Acknowledgements
 
@@ -155,11 +162,28 @@
 [![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)<br>
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm-project.org)
 [![Nox](https://img.shields.io/badge/%F0%9F%A6%8A-Nox-D85E00.svg)](https://github.com/wntrblm/nox)
 [![Built with Material for MkDocs](https://img.shields.io/badge/Material_for_MkDocs-526CFE?logo=MaterialForMkDocs&logoColor=white)](https://squidfunk.github.io/mkdocs-material/)
 
 </div>
 
----
+
+## Citation
+
+If you find this repository useful, please consider giving a star ⭐ and adding the following citation:
+
+```
+@inproceedings{
+kaiko.ai2024eva,
+title={eva: Evaluation framework for pathology foundation models},
+author={kaiko.ai and Ioannis Gatopoulos and Nicolas K{\"a}nzig and Roman Moser and Sebastian Ot{\'a}lora},
+booktitle={Medical Imaging with Deep Learning},
+year={2024},
+url={https://openreview.net/forum?id=FNBQOPj18N}
+}
+```
+
+<br />
+
 <div align="center">
   <img src="https://github.com/kaiko-ai/eva/blob/main/docs/images/kaiko-logo.png?raw=true" width="200">
 </div>
```

#### html2text {}

```diff
@@ -1,14 +1,18 @@
+
  [https://github.com/kaiko-ai/eva/blob/main/docs/images/eva-logo.png?raw=true]
+
 _Oncology FM Evaluation Framework by kaiko.ai_ [![PyPI](https://img.shields.io/
  pypi/v/kaiko-eva.svg?logo=python)](https://pypi.python.org/pypi/kaiko-eva) [!
-    [CI](https://github.com/kaiko-ai/eva/workflows/CI/badge.svg)](https://
-   github.com/kaiko-ai/eva/actions?query=workflow%3ACI) [![license](https://
- img.shields.io/badge/License-Apache%202.0-blue.svg?labelColor=gray)](https://
-                       github.com/kaiko-ai/eva#license)
+  [docs](https://img.shields.io/badge/ð_docs-latest-green)](https://kaiko-
+      ai.github.io/eva/latest) [![license](https://img.shields.io/badge/
+  âï¸_License-Apache%202.0-blue.svg?labelColor=gray)](https://github.com/
+                             kaiko-ai/eva#license)
+[![paper](http://img.shields.io/badge/OpenReview-MIDL_2024-B31B1B.svg)](https:/
+            /openreview.net/forum?id=FNBQOPj18N&noteId=FNBQOPj18N)
   _I_n_s_t_a_l_l_a_t_i_o_n â¢ _H_o_w_ _T_o_ _U_s_e â¢ _D_o_c_u_m_e_n_t_a_t_i_o_n â¢ _D_a_t_a_s_e_t_s â¢ _B_e_n_c_h_m_a_r_k_s
                         _C_o_n_t_r_i_b_u_t_e â¢ _A_c_k_n_o_w_l_e_d_g_e_m_e_n_t_s
 
 _`eva`_ is an evaluation framework for oncology foundation models (FMs) by
 [kaiko.ai](https://kaiko.ai/). Check out the [documentation](https://kaiko-
 ai.github.io/eva/) for more information. ### Highlights: - Easy and reliable
 benchmark of Oncology FMs - Automatic embedding inference and evaluation of a
@@ -16,65 +20,72 @@
 ai.github.io/eva/dev/datasets/) and models - Produce statistics over multiple
 evaluation fits and multiple metrics ## Installation Simple installation from
 PyPI: ```sh # to install the core version only pip install kaiko-eva # to
 install the expanded `vision` version pip install 'kaiko-eva[vision]' # to
 install everything pip install 'kaiko-eva[all]' ``` To install the latest
 version of the `main` branch: ```sh pip install "kaiko-eva[all] @ git+https://
 github.com/kaiko-ai/eva.git" ``` You can verify that the installation was
-successful by executing: ```sh eva --version ``` ## How To Use _eva_ can be
+successful by executing: ```sh eva --version ``` ## How To Use _`eva`_ can be
 used directly from the terminal as a CLI tool as follows: ```sh eva
 {fit,predict,predict_fit} --config url/or/path/to/the/config.yaml ``` When used
-as a CLI tool, `_eva_` supports configuration files (`.yaml`) as an argument to
+as a CLI tool, _`eva`_ supports configuration files (`.yaml`) as an argument to
 define its functionality. Native supported configs can be found at the
 [configs](https://github.com/kaiko-ai/eva/tree/main/configs) directory of the
 repo. Apart from cloning the repo, you can download the latest config folder as
 `.zip` from your browser from [here](https://download-directory.github.io/
 ?url=https://github.com/kaiko-ai/eva/tree/main/configs). Alternatively, from a
 specific release the configs can be downloaded from the terminal as follows:
 ```sh curl -LO https://github.com/kaiko-ai/eva/releases/download/0.0.1/
-configs.zip | unzip configs.zip ``` For example, to perform a downstream
-evaluation of DINO ViT-S/16 on the BACH dataset with linear probing by first
-inferring the embeddings and performing 5 sequential fits, execute: ```sh #
-from a locally stored config file eva predict_fit --config ./configs/vision/
-dino_vit/offline/bach.yaml # from a remote stored config file eva predict_fit -
--config https://raw.githubusercontent.com/kaiko-ai/eva/main/configs/vision/
-dino_vit/offline/bach.yaml ``` > [!NOTE] > All the datasets that support
-automatic download in the repo have by default the option to automatically
-download set to false. > For automatic download you have to manually set
-download=true. To view all the possibles, execute: ```sh eva --help ``` For
-more information, please refer to the [documentation](https://kaiko-
-ai.github.io/eva/dev/user-guide/tutorials/offline_vs_online/) and [tutorials]
-(https://kaiko-ai.github.io/eva/dev/user-guide/advanced/replicate_evaluations/
-). ## Benchmarks In this section you will find model benchmarks which were
-generated with _eva_. ### Table I: WSI patch-level benchmark
+configs.zip | unzip configs ``` For example, to perform a downstream evaluation
+of DINO ViT-S/16 on the BACH dataset with linear probing by first inferring the
+embeddings and performing 5 sequential fits, execute: ```sh # from a locally
+stored config file eva predict_fit --config ./configs/vision/dino_vit/offline/
+bach.yaml # from a remote stored config file eva predict_fit --config https://
+raw.githubusercontent.com/kaiko-ai/eva/main/configs/vision/dino_vit/offline/
+bach.yaml ``` > [!NOTE] > All the datasets that support automatic download in
+the repo have by default the option to automatically download set to false. >
+For automatic download you have to manually set download=true. To view all the
+possibles, execute: ```sh eva --help ``` For more information, please refer to
+the [documentation](https://kaiko-ai.github.io/eva/dev/user-guide/tutorials/
+offline_vs_online/) and [tutorials](https://kaiko-ai.github.io/eva/dev/user-
+guide/advanced/replicate_evaluations/). ## Benchmarks In this section you will
+find model benchmarks which were generated with _`eva`_. ### Table I: WSI
+patch-level benchmark
 | Model | BACH | CRC | MHIST | PCam/val | PCam/test | |------------------------
  --------------------------|-------|-------|-------|----------|-----------| |
 ViT-S/16 _(random)_ [1] | 0.410 | 0.617 | 0.501 | 0.753 | 0.728 | | ViT-S/16 _
      (ImageNet)_ [1] | 0.695 | 0.935 | 0.831 | 0.864 | 0.849 | | ViT-B/8 _
- (ImageNet)_ [1] | 0.710 | 0.939 | 0.814 | 0.870 | 0.856 | | DINO(p=16) [2] |
+    (ImageNet)_ [1] | 0.710 | 0.939 | 0.814 | 0.870 | 0.856 | | ViT-L/14 _
+ (ImageNet)_ [1] | 0.707 | 0.916 | 0.832 | 0.873 | 0.888 | | DINO(p=16) [2] |
 0.801 | 0.934 | 0.768 | 0.889 | 0.895 | | Phikon [3] | 0.725 | 0.935 | 0.777 |
- 0.912 | 0.915 | | ViT-S/16 _(kaiko.ai)_ [4] | 0.797 | 0.943 | 0.828 | 0.903 |
-0.893 | | ViT-S/8 _(kaiko.ai)_ [4] | 0.834 | 0.946 | 0.832 | 0.897 | 0.887 | |
-ViT-B/16 _(kaiko.ai)_ [4] | 0.810 | 0.960 | 0.826 | 0.900 | 0.898 | | ViT-B/8 _
-    (kaiko.ai)_ [4] | 0.865 | 0.956 | 0.809 | 0.913 | 0.921 | | ViT-L/14 _
-  (kaiko.ai)_ [4] | 0.870 | 0.930 | 0.809 | 0.908 | 0.898 | _Table I: Linear
+0.912 | 0.915 | | UNI [4] | 0.814 | 0.950 | 0.837 | 0.936 | 0.938 | | ViT-S/16
+    _(kaiko.ai)_ [5] | 0.797 | 0.943 | 0.828 | 0.903 | 0.893 | | ViT-S/8 _
+    (kaiko.ai)_ [5] | 0.834 | 0.946 | 0.832 | 0.897 | 0.887 | | ViT-B/16 _
+     (kaiko.ai)_ [5] | 0.810 | 0.960 | 0.826 | 0.900 | 0.898 | | ViT-B/8 _
+    (kaiko.ai)_ [5] | 0.865 | 0.956 | 0.809 | 0.913 | 0.921 | | ViT-L/14 _
+  (kaiko.ai)_ [5] | 0.870 | 0.930 | 0.809 | 0.908 | 0.898 | _Table I: Linear
          probing evaluation of FMs on patch-level downstream datasets.
   We report averaged balanced accuracy over 5 runs, with an average standard
                             deviation of Â±0.003._
 
 _References_: 1. _"Emerging properties in self-supervised vision
-transformersâ_ 2. _"Benchmarking self-supervised learning on diverse
-pathology datasetsâ_ 3. _"Scaling self-supervised learning for histopathology
-with masked image modelingâ_ 4. _"Towards Training Large-Scale Pathology
-Foundation Models: from TCGA to Hospital Scaleâ_ ## Contributing _eva_ is an
-open source project and welcomes contributions of all kinds. Please checkout
-the [developer](./docs/DEVELOPER_GUIDE.md) and [contributing guide](./docs/
-CONTRIBUTING.md) for help on how to do so. All contributors must follow the
-[code of conduct](./docs/CODE_OF_CONDUCT.md). ## Acknowledgements Our codebase
-is built using multiple opensource contributions
+transformersâ_, [arXiv](https://arxiv.org/abs/2104.14294) 2. _"Benchmarking
+self-supervised learning on diverse pathology datasetsâ_, [arXiv](https://
+arxiv.org/abs/2212.04690) 3. _"Scaling self-supervised learning for
+histopathology with masked image modelingâ_, [medRxiv](https://
+www.medrxiv.org/content/10.1101/2023.07.21.23292757v1) 4. _"A General-Purpose
+Self-Supervised Model for Computational Pathologyâ_, [arXiv](https://
+arxiv.org/abs/2308.15474) 5. _"Towards Training Large-Scale Pathology
+Foundation Models: from TCGA to Hospital Scaleâ_, [arXiv](https://arxiv.org/
+pdf/2404.15217) ## Contributing _`eva`_ is an open source project and welcomes
+contributions of all kinds. Please checkout the [developer](./docs/
+DEVELOPER_GUIDE.md) and [contributing guide](./docs/CONTRIBUTING.md) for help
+on how to do so. All contributors must follow the [code of conduct](./docs/
+CODE_OF_CONDUCT.md). ## Acknowledgements Our codebase is built using multiple
+opensource contributions
                [![python](https://img.shields.io/badge/-Python-
 blue?logo=python&logoColor=white)](https://github.com/pre-commit/pre-commit) [!
                 [pytorch](https://img.shields.io/badge/PyTorch-
 ee4c2c?logo=pytorch&logoColor=white)](https://pytorch.org/get-started/locally/
         ) [![lightning](https://img.shields.io/badge/-â¡ï¸_Lightning-
  792ee5?logo=pytorchlightning&logoColor=white)](https://pytorchlightning.ai/)
           [![black](https://img.shields.io/badge/Code%20Style-Black-
@@ -87,9 +98,14 @@
            pyright_badge.svg)](https://microsoft.github.io/pyright/)
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://
     pdm-project.org) [![Nox](https://img.shields.io/badge/%F0%9F%A6%8A-Nox-
 D85E00.svg)](https://github.com/wntrblm/nox) [![Built with Material for MkDocs]
               (https://img.shields.io/badge/Material_for_MkDocs-
  526CFE?logo=MaterialForMkDocs&logoColor=white)](https://squidfunk.github.io/
                                mkdocs-material/)
----
+## Citation If you find this repository useful, please consider giving a star
+â­ and adding the following citation: ``` @inproceedings{ kaiko.ai2024eva,
+title={eva: Evaluation framework for pathology foundation models}, author=
+{kaiko.ai and Ioannis Gatopoulos and Nicolas K{\"a}nzig and Roman Moser and
+Sebastian Ot{\'a}lora}, booktitle={Medical Imaging with Deep Learning}, year=
+{2024}, url={https://openreview.net/forum?id=FNBQOPj18N} } ```
 [https://github.com/kaiko-ai/eva/blob/main/docs/images/kaiko-logo.png?raw=true]
```

### Comparing `kaiko_eva-0.0.1/pyproject.toml` & `kaiko_eva-0.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "kaiko-eva"
-version = "0.0.1"
+version = "0.0.2"
 description = "Evaluation Framework for oncology foundation models."
 keywords = [
     "machine-learning",
     "evaluation-framework",
     "oncology",
     "foundation-models",
 ]
@@ -30,23 +30,25 @@
 maintainers = [
     { name = "Ioannis Gatopoulos", email = "ioannis@kaiko.ai" },
     { name = "Nicolas Känzig", email = "nicolas@kaiko.ai" },
     { name = "Roman Moser", email = "roman@kaiko.ai" },
 ]
 requires-python = ">=3.10"
 dependencies = [
-    "lightning>=2.2.1",
-    "jsonargparse[omegaconf]>=4.27.4",
+    "torch==2.3.0",
+    "lightning>=2.2.2",
+    "jsonargparse[omegaconf]==4.28",
     "tensorboard>=2.16.2",
     "loguru>=0.7.2",
     "pandas>=2.2.0",
     "transformers>=4.38.2",
     "onnxruntime>=1.17.1",
-    "onnx>=1.15.0",
+    "onnx>=1.16.0",
     "toolz>=0.12.1",
+    "rich>=13.7.1",
 ]
 
 [project.urls]
 Homepage = "https://kaiko-ai.github.io/eva/dev/"
 Repository = "https://github.com/kaiko-ai/eva"
 Documentation = "https://kaiko-ai.github.io/eva/dev/"
```

### Comparing `kaiko_eva-0.0.1/src/eva/__init__.py` & `kaiko_eva-0.0.2/src/eva/__init__.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/__version__.py` & `kaiko_eva-0.0.2/src/eva/__version__.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/callbacks/writers/embeddings.py` & `kaiko_eva-0.0.2/src/eva/core/callbacks/writers/embeddings.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/callbacks/writers/typings.py` & `kaiko_eva-0.0.2/src/eva/core/callbacks/writers/typings.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/cli/logo.py` & `kaiko_eva-0.0.2/src/eva/core/cli/logo.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/cli/setup.py` & `kaiko_eva-0.0.2/src/eva/core/cli/setup.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/data/dataloaders/dataloader.py` & `kaiko_eva-0.0.2/src/eva/core/data/dataloaders/dataloader.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/data/datamodules/call.py` & `kaiko_eva-0.0.2/src/eva/core/data/datamodules/call.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/data/datamodules/datamodule.py` & `kaiko_eva-0.0.2/src/eva/core/data/datamodules/datamodule.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/data/datamodules/schemas.py` & `kaiko_eva-0.0.2/src/eva/core/data/datamodules/schemas.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/data/datasets/base.py` & `kaiko_eva-0.0.2/src/eva/core/data/datasets/base.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/data/datasets/classification/embeddings.py` & `kaiko_eva-0.0.2/src/eva/core/data/datasets/embeddings/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-"""Embeddings classification dataset."""
+"""Base dataset class for Embeddings."""
 
+import abc
 import os
-from typing import Callable, Dict, Tuple
+from typing import Callable, Dict, Literal, Tuple
 
 import numpy as np
 import pandas as pd
 import torch
 from typing_extensions import override
 
 from eva.core.data.datasets import base
 from eva.core.utils import io
 
+default_column_mapping: Dict[str, str] = {
+    "path": "embeddings",
+    "target": "target",
+    "split": "split",
+    "multi_id": "slide_id",
+}
+"""The default column mapping of the variables to the manifest columns."""
 
-class EmbeddingsClassificationDataset(base.Dataset):
-    """Embeddings classification dataset."""
 
-    default_column_mapping: Dict[str, str] = {
-        "data": "embeddings",
-        "target": "target",
-        "split": "split",
-    }
-    """The default column mapping of the variables to the manifest columns."""
+class EmbeddingsDataset(base.Dataset):
+    """Abstract base class for embedding datasets."""
 
     def __init__(
         self,
         root: str,
         manifest_file: str,
-        split: str | None = None,
+        split: Literal["train", "val", "test"] | None = None,
         column_mapping: Dict[str, str] = default_column_mapping,
         embeddings_transforms: Callable | None = None,
         target_transforms: Callable | None = None,
     ) -> None:
         """Initialize dataset.
 
         Expects a manifest file listing the paths of .pt files that contain
@@ -50,32 +52,58 @@
             target_transforms: A function/transform that transforms the target.
         """
         super().__init__()
 
         self._root = root
         self._manifest_file = manifest_file
         self._split = split
-        self._column_mapping = self.default_column_mapping | column_mapping
+        self._column_mapping = default_column_mapping | column_mapping
         self._embeddings_transforms = embeddings_transforms
         self._target_transforms = target_transforms
 
         self._data: pd.DataFrame
 
+    @abc.abstractmethod
+    def _load_embeddings(self, index: int) -> torch.Tensor:
+        """Returns the `index`'th embedding sample.
+
+        Args:
+            index: The index of the data sample to load.
+
+        Returns:
+            The embedding sample as a tensor.
+        """
+
+    @abc.abstractmethod
+    def _load_target(self, index: int) -> np.ndarray:
+        """Returns the `index`'th target sample.
+
+        Args:
+            index: The index of the data sample to load.
+
+        Returns:
+            The sample target as an array.
+        """
+
+    @abc.abstractmethod
+    def __len__(self) -> int:
+        """Returns the total length of the data."""
+
     def filename(self, index: int) -> str:
         """Returns the filename of the `index`'th data sample.
 
         Note that this is the relative file path to the root.
 
         Args:
             index: The index of the data-sample to select.
 
         Returns:
             The filename of the `index`'th data sample.
         """
-        return self._data.at[index, self._column_mapping["data"]]
+        return self._data.at[index, self._column_mapping["path"]]
 
     @override
     def setup(self):
         self._data = self._load_manifest()
 
     def __getitem__(self, index) -> Tuple[torch.Tensor, np.ndarray]:
         """Returns the `index`'th data sample.
@@ -86,44 +114,14 @@
         Returns:
             A data sample and its target.
         """
         embeddings = self._load_embeddings(index)
         target = self._load_target(index)
         return self._apply_transforms(embeddings, target)
 
-    def __len__(self) -> int:
-        """Returns the total length of the data."""
-        return len(self._data)
-
-    def _load_embeddings(self, index: int) -> torch.Tensor:
-        """Returns the `index`'th embedding sample.
-
-        Args:
-            index: The index of the data sample to load.
-
-        Returns:
-            The sample embedding as an array.
-        """
-        filename = self.filename(index)
-        embeddings_path = os.path.join(self._root, filename)
-        tensor = torch.load(embeddings_path, map_location="cpu")
-        return tensor.squeeze(0)
-
-    def _load_target(self, index: int) -> np.ndarray:
-        """Returns the `index`'th target sample.
-
-        Args:
-            index: The index of the data sample to load.
-
-        Returns:
-            The sample target as an array.
-        """
-        target = self._data.at[index, self._column_mapping["target"]]
-        return np.asarray(target, dtype=np.int64)
-
     def _load_manifest(self) -> pd.DataFrame:
         """Loads manifest file and filters the data based on the split column.
 
         Returns:
             The data as a pandas DataFrame.
         """
         manifest_path = os.path.join(self._root, self._manifest_file)
```

### Comparing `kaiko_eva-0.0.1/src/eva/core/data/transforms/dtype/array.py` & `kaiko_eva-0.0.2/src/eva/core/data/transforms/dtype/array.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/interface/interface.py` & `kaiko_eva-0.0.2/src/eva/core/interface/interface.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/metrics/__init__.py` & `kaiko_eva-0.0.2/src/eva/core/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/metrics/average_loss.py` & `kaiko_eva-0.0.2/src/eva/core/metrics/average_loss.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/metrics/binary_balanced_accuracy.py` & `kaiko_eva-0.0.2/src/eva/core/metrics/binary_balanced_accuracy.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/metrics/defaults/classification/binary.py` & `kaiko_eva-0.0.2/src/eva/core/metrics/defaults/classification/binary.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/metrics/defaults/classification/multiclass.py` & `kaiko_eva-0.0.2/src/eva/core/metrics/defaults/classification/multiclass.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/metrics/structs/module.py` & `kaiko_eva-0.0.2/src/eva/core/metrics/structs/module.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/metrics/structs/schemas.py` & `kaiko_eva-0.0.2/src/eva/core/metrics/structs/schemas.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/models/modules/head.py` & `kaiko_eva-0.0.2/src/eva/core/models/modules/head.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,31 +51,31 @@
         self.head = head
         self.criterion = criterion
         self.backbone = backbone
         self.optimizer = optimizer
         self.lr_scheduler = lr_scheduler
 
     @override
+    def configure_model(self) -> Any:
+        if self.backbone is not None:
+            grad.deactivate_requires_grad(self.backbone)
+
+    @override
     def configure_optimizers(self) -> Any:
-        parameters = list(self.head.parameters())
+        parameters = self.head.parameters()
         optimizer = self.optimizer(parameters)
         lr_scheduler = self.lr_scheduler(optimizer)
         return {"optimizer": optimizer, "lr_scheduler": lr_scheduler}
 
     @override
     def forward(self, tensor: torch.Tensor, *args: Any, **kwargs: Any) -> torch.Tensor:
         features = tensor if self.backbone is None else self.backbone(tensor)
         return self.head(features).squeeze(-1)
 
     @override
-    def on_fit_start(self) -> None:
-        if self.backbone is not None:
-            grad.deactivate_requires_grad(self.backbone)
-
-    @override
     def training_step(self, batch: INPUT_BATCH, *args: Any, **kwargs: Any) -> STEP_OUTPUT:
         return self._batch_step(batch)
 
     @override
     def validation_step(self, batch: INPUT_BATCH, *args: Any, **kwargs: Any) -> STEP_OUTPUT:
         return self._batch_step(batch)
 
@@ -84,19 +84,14 @@
         return self._batch_step(batch)
 
     @override
     def predict_step(self, batch: INPUT_BATCH, *args: Any, **kwargs: Any) -> torch.Tensor:
         tensor = INPUT_BATCH(*batch).data
         return tensor if self.backbone is None else self.backbone(tensor)
 
-    @override
-    def on_fit_end(self) -> None:
-        if self.backbone is not None:
-            grad.activate_requires_grad(self.backbone)
-
     def _batch_step(self, batch: INPUT_BATCH) -> STEP_OUTPUT:
         """Performs a model forward step and calculates the loss.
 
         Args:
             batch: The desired batch to process.
 
         Returns:
```

### Comparing `kaiko_eva-0.0.1/src/eva/core/models/modules/inference.py` & `kaiko_eva-0.0.2/src/eva/core/models/modules/inference.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/models/modules/module.py` & `kaiko_eva-0.0.2/src/eva/core/models/modules/module.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Base model module."""
 
 from typing import Any, Mapping
 
 import lightning.pytorch as pl
 import torch
+from lightning.pytorch.strategies.single_device import SingleDeviceStrategy
 from lightning.pytorch.utilities import memory
 from lightning.pytorch.utilities.types import STEP_OUTPUT
 from typing_extensions import override
 
 from eva.core.metrics import structs as metrics_lib
 from eva.core.models.modules.typings import INPUT_BATCH
 from eva.core.models.modules.utils import batch_postprocess
@@ -42,28 +43,47 @@
         return metrics_lib.MetricsSchema()
 
     @property
     def default_postprocess(self) -> batch_postprocess.BatchPostProcess:
         """The default post-processes."""
         return batch_postprocess.BatchPostProcess()
 
+    @property
+    def metrics_device(self) -> torch.device:
+        """Returns the device by which the metrics should be calculated.
+
+        We allocate the metrics to CPU when operating on single device, as
+        it is much faster, but to GPU when employing multiple ones, as DDP
+        strategy requires the metrics to be allocated to the module's GPU.
+        """
+        move_to_cpu = isinstance(self.trainer.strategy, SingleDeviceStrategy)
+        return torch.device("cpu") if move_to_cpu else self.device
+
+    @override
+    def on_fit_start(self) -> None:
+        self.metrics.to(device=self.metrics_device)
+
     @override
     def on_train_batch_end(
         self,
         outputs: STEP_OUTPUT,
         batch: INPUT_BATCH,
         batch_idx: int,
     ) -> None:
         outputs = self._common_batch_end(outputs)
         self._forward_and_log_metrics(
             self.metrics.training_metrics,
             batch_outputs=outputs,
         )
 
     @override
+    def on_validation_start(self) -> None:
+        self.metrics.to(device=self.metrics_device)
+
+    @override
     def on_validation_batch_end(
         self,
         outputs: STEP_OUTPUT,
         batch: INPUT_BATCH,
         batch_idx: int,
         dataloader_idx: int = 0,
     ) -> None:
@@ -75,14 +95,18 @@
         )
 
     @override
     def on_validation_epoch_end(self) -> None:
         self._compute_and_log_metrics(self.metrics.validation_metrics)
 
     @override
+    def on_test_start(self) -> None:
+        self.metrics.to(device=self.metrics_device)
+
+    @override
     def on_test_batch_end(
         self,
         outputs: STEP_OUTPUT,
         batch: INPUT_BATCH,
         batch_idx: int,
         dataloader_idx: int = 0,
     ) -> None:
@@ -106,15 +130,15 @@
         Args:
             outputs: The batch step outputs.
 
         Returns:
             The updated outputs.
         """
         self._postprocess(outputs)
-        return memory.recursive_detach(outputs, to_cpu=self.device.type == "cpu")
+        return memory.recursive_detach(outputs, to_cpu=self.metrics_device.type == "cpu")
 
     def _forward_and_log_metrics(
         self,
         metrics: metrics_lib.MetricCollection,
         batch_outputs: STEP_OUTPUT,
     ) -> None:
         """Performs a forward pass to the metrics and logs them.
```

### Comparing `kaiko_eva-0.0.1/src/eva/core/models/modules/typings.py` & `kaiko_eva-0.0.2/src/eva/core/models/modules/typings.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/models/modules/utils/batch_postprocess.py` & `kaiko_eva-0.0.2/src/eva/core/models/modules/utils/batch_postprocess.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/models/modules/utils/grad.py` & `kaiko_eva-0.0.2/src/eva/core/models/modules/utils/grad.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/models/networks/_utils.py` & `kaiko_eva-0.0.2/src/eva/core/models/networks/_utils.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/models/networks/mlp.py` & `kaiko_eva-0.0.2/src/eva/core/models/networks/mlp.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/models/networks/transforms/extract_cls_features.py` & `kaiko_eva-0.0.2/src/eva/core/models/networks/transforms/extract_cls_features.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/models/networks/wrappers/base.py` & `kaiko_eva-0.0.2/src/eva/core/models/networks/wrappers/base.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/models/networks/wrappers/from_function.py` & `kaiko_eva-0.0.2/src/eva/core/models/networks/wrappers/from_function.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/models/networks/wrappers/huggingface.py` & `kaiko_eva-0.0.2/src/eva/core/models/networks/wrappers/huggingface.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/models/networks/wrappers/onnx.py` & `kaiko_eva-0.0.2/src/eva/core/models/networks/wrappers/onnx.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/trainers/_logging.py` & `kaiko_eva-0.0.2/src/eva/core/trainers/_logging.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/trainers/_recorder.py` & `kaiko_eva-0.0.2/src/eva/core/trainers/_recorder.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,71 @@
 """Multi-run summary recorder."""
 
 import collections
 import json
 import os
 import statistics
 import sys
-from typing import Any, Dict, List, Mapping
+from typing import Dict, List, Mapping, TypedDict
 
 from lightning.pytorch.utilities.types import _EVALUATE_OUTPUT
 from lightning_fabric.utilities import cloud_io
 from loguru import logger
 from omegaconf import OmegaConf
+from rich import console as rich_console
+from rich import table as rich_table
 from toolz import dicttoolz
 
 SESSION_METRICS = Mapping[str, List[float]]
 """Session metrics type-hint."""
 
 
+class SESSION_STATISTICS(TypedDict):
+    """Type-hint for aggregated metrics of multiple runs with mean & stdev."""
+
+    mean: float
+    stdev: float
+    values: List[float]
+
+
+class STAGE_RESULTS(TypedDict):
+    """Type-hint for metrics statstics for val & test stages."""
+
+    val: List[Dict[str, SESSION_STATISTICS]]
+    test: List[Dict[str, SESSION_STATISTICS]]
+
+
+class RESULTS_DICT(TypedDict):
+    """Type-hint for the final results dictionary."""
+
+    metrics: STAGE_RESULTS
+
+
 class SessionRecorder:
     """Multi-run (session) summary logger."""
 
     def __init__(
         self,
         output_dir: str,
         results_file: str = "results.json",
         config_file: str = "config.yaml",
+        verbose: bool = True,
     ) -> None:
         """Initializes the recorder.
 
         Args:
             output_dir: The destination folder to save the results.
             results_file: The name of the results json file.
             config_file: The name of the yaml configuration file.
+            verbose: Whether to print the session metrics.
         """
         self._output_dir = output_dir
         self._results_file = results_file
         self._config_file = config_file
+        self._verbose = verbose
 
         self._validation_metrics: List[SESSION_METRICS] = []
         self._test_metrics: List[SESSION_METRICS] = []
 
     @property
     def filename(self) -> str:
         """Returns the output filename."""
@@ -63,30 +89,32 @@
         validation_scores: _EVALUATE_OUTPUT,
         test_scores: _EVALUATE_OUTPUT | None = None,
     ) -> None:
         """Updates the state of the tracked metrics in-place."""
         self._update_validation_metrics(validation_scores)
         self._update_test_metrics(test_scores)
 
-    def compute(self) -> Dict[str, List[Dict[str, Any]]]:
+    def compute(self) -> STAGE_RESULTS:
         """Computes and returns the session statistics."""
         validation_statistics = list(map(_calculate_statistics, self._validation_metrics))
         test_statistics = list(map(_calculate_statistics, self._test_metrics))
         return {"val": validation_statistics, "test": test_statistics}
 
-    def export(self) -> Dict[str, Any]:
+    def export(self) -> RESULTS_DICT:
         """Exports the results."""
         statistics = self.compute()
         return {"metrics": statistics}
 
     def save(self) -> None:
         """Saves the recorded results."""
         results = self.export()
         _save_json(results, self.filename)
         self._save_config()
+        if self._verbose:
+            _print_results(results)
 
     def reset(self) -> None:
         """Resets the state of the tracked metrics."""
         self._validation_metrics = []
         self._test_metrics = []
 
     def _update_validation_metrics(self, metrics: _EVALUATE_OUTPUT) -> None:
@@ -121,29 +149,63 @@
 
 
 def _init_session_metrics(n_datasets: int) -> List[SESSION_METRICS]:
     """Returns the init session metrics."""
     return [collections.defaultdict(list) for _ in range(n_datasets)]
 
 
-def _calculate_statistics(session_metrics: SESSION_METRICS) -> Dict[str, float | List[float]]:
+def _calculate_statistics(session_metrics: SESSION_METRICS) -> Dict[str, SESSION_STATISTICS]:
     """Calculate the metric statistics of a dataset session run."""
 
-    def _calculate_metric_statistics(values: List[float]) -> Dict[str, float | List[float]]:
+    def _calculate_metric_statistics(values: List[float]) -> SESSION_STATISTICS:
         """Calculates and returns the metric statistics."""
         mean = statistics.mean(values)
         stdev = statistics.stdev(values) if len(values) > 1 else 0
         return {"mean": mean, "stdev": stdev, "values": values}
 
     return dicttoolz.valmap(_calculate_metric_statistics, session_metrics)
 
 
-def _save_json(data: Dict[str, Any], save_as: str = "data.json"):
+def _save_json(data: RESULTS_DICT, save_as: str = "data.json"):
     """Saves data to a json file."""
     if not save_as.endswith(".json"):
         raise ValueError()
 
     output_dir = os.path.dirname(save_as)
     fs = cloud_io.get_filesystem(output_dir, anon=False)
     fs.makedirs(output_dir, exist_ok=True)
     with fs.open(save_as, "w") as file:
-        json.dump(data, file, indent=4, sort_keys=True)
+        json.dump(data, file, indent=2, sort_keys=True)
+
+
+def _print_results(results: RESULTS_DICT) -> None:
+    """Prints the results to the console."""
+    try:
+        for stage in ["val", "test"]:
+            for dataset_idx in range(len(results["metrics"][stage])):
+                _print_table(results["metrics"][stage][dataset_idx], stage, dataset_idx)
+    except Exception as e:
+        logger.error(f"Failed to print the results: {e}")
+
+
+def _print_table(metrics_dict: Dict[str, SESSION_STATISTICS], stage: str, dataset_idx: int):
+    """Prints the metrics of a single dataset as a table."""
+    metrics_table = rich_table.Table(
+        title=f"\n{stage.capitalize()} Dataset {dataset_idx}", title_style="bold"
+    )
+    metrics_table.add_column("Metric", style="cyan")
+    metrics_table.add_column("Mean", style="magenta")
+    metrics_table.add_column("Stdev", style="magenta")
+    metrics_table.add_column("All", style="magenta")
+
+    n_runs = len(metrics_dict[next(iter(metrics_dict))]["values"])
+    for metric_name, metric_dict in metrics_dict.items():
+        row = [
+            metric_name,
+            f'{metric_dict["mean"]:.3f}',
+            f'{metric_dict["stdev"]:.3f}',
+            ", ".join(f'{metric_dict["values"][i]:.3f}' for i in range(n_runs)),
+        ]
+        metrics_table.add_row(*row)
+
+    console = rich_console.Console()
+    console.print(metrics_table)
```

### Comparing `kaiko_eva-0.0.1/src/eva/core/trainers/functional.py` & `kaiko_eva-0.0.2/src/eva/core/trainers/functional.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,82 +12,99 @@
 
 def run_evaluation_session(
     base_trainer: eva_trainer.Trainer,
     base_model: modules.ModelModule,
     datamodule: datamodules.DataModule,
     *,
     n_runs: int = 1,
+    verbose: bool = True,
 ) -> None:
     """Runs a downstream evaluation session out-of-place.
 
     It performs an evaluation run (fit and evaluate) on the model
     multiple times. Note that as the input `base_trainer` and
     `base_model` would be cloned, the input object would not
     be modified.
 
     Args:
         base_trainer: The base trainer module to use.
         base_model: The base model module to use.
         datamodule: The data module.
         n_runs: The amount of runs (fit and evaluate) to perform.
+        verbose: Whether to verbose the session metrics instead of
+            these of each individual runs and vice-versa.
     """
-    recorder = _recorder.SessionRecorder(output_dir=base_trainer.default_log_dir)
+    recorder = _recorder.SessionRecorder(output_dir=base_trainer.default_log_dir, verbose=verbose)
     for run_index in range(n_runs):
         validation_scores, test_scores = run_evaluation(
-            base_trainer, base_model, datamodule, run_id=f"run_{run_index}"
+            base_trainer,
+            base_model,
+            datamodule,
+            run_id=f"run_{run_index}",
+            verbose=not verbose,
         )
         recorder.update(validation_scores, test_scores)
     recorder.save()
 
 
 def run_evaluation(
     base_trainer: eva_trainer.Trainer,
     base_model: modules.ModelModule,
     datamodule: datamodules.DataModule,
     *,
     run_id: str | None = None,
+    verbose: bool = True,
 ) -> Tuple[_EVALUATE_OUTPUT, _EVALUATE_OUTPUT | None]:
     """Fits and evaluates a model out-of-place.
 
     Args:
         base_trainer: The base trainer to use but not modify.
         base_model: The model module to use but not modify.
         datamodule: The data module.
         run_id: The run id to be appended to the output log directory.
             If `None`, it will use the log directory of the trainer as is.
+        verbose: Whether to print the validation and test metrics
+            in the end of the training.
 
     Returns:
         A tuple of with the validation and the test metrics (if exists).
     """
     trainer, model = _utils.clone(base_trainer, base_model)
     trainer.setup_log_dirs(run_id or "")
-    return fit_and_validate(trainer, model, datamodule)
+    return fit_and_validate(trainer, model, datamodule, verbose=verbose)
 
 
 def fit_and_validate(
     trainer: eva_trainer.Trainer,
     model: modules.ModelModule,
     datamodule: datamodules.DataModule,
+    verbose: bool = True,
 ) -> Tuple[_EVALUATE_OUTPUT, _EVALUATE_OUTPUT | None]:
     """Fits and evaluates a model in-place.
 
     If the test set is set in the datamodule, it will evaluate the model
     on the test set as well.
 
     Args:
         trainer: The trainer module to use and update in-place.
         model: The model module to use and update in-place.
         datamodule: The data module.
+        verbose: Whether to print the validation and test metrics
+            in the end of the training.
 
     Returns:
         A tuple of with the validation and the test metrics (if exists).
     """
     trainer.fit(model, datamodule=datamodule)
-    validation_scores = trainer.validate(datamodule=datamodule)
-    test_scores = None if datamodule.datasets.test is None else trainer.test(datamodule=datamodule)
+    validation_scores = trainer.validate(datamodule=datamodule, verbose=verbose)
+    test_scores = (
+        None
+        if datamodule.datasets.test is None
+        else trainer.test(datamodule=datamodule, verbose=verbose)
+    )
     return validation_scores, test_scores
 
 
 def infer_model(
     base_trainer: eva_trainer.Trainer,
     base_model: modules.ModelModule,
     datamodule: datamodules.DataModule,
```

### Comparing `kaiko_eva-0.0.1/src/eva/core/trainers/trainer.py` & `kaiko_eva-0.0.2/src/eva/core/trainers/trainer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """Core trainer module."""
 
 import os
 from typing import Any
 
+import loguru
 from lightning.pytorch import loggers as pl_loggers
 from lightning.pytorch import trainer as pl_trainer
 from lightning.pytorch.utilities import argparse
+from lightning_fabric.utilities import cloud_io
 from typing_extensions import override
 
+from eva.core import loggers as eva_loggers
 from eva.core.data import datamodules
 from eva.core.models import modules
 from eva.core.trainers import _logging, functional
 
 
 class Trainer(pl_trainer.Trainer):
     """Core trainer class.
@@ -61,21 +64,31 @@
     def setup_log_dirs(self, subdirectory: str = "") -> None:
         """Setups the logging directory of the trainer and experimental loggers in-place.
 
         Args:
             subdirectory: Whether to append a subdirectory to the output log.
         """
         self._log_dir = os.path.join(self.default_root_dir, self._session_id, subdirectory)
-        os.fspath(self._log_dir)
 
-        for logger in self.loggers:
-            if isinstance(logger, (pl_loggers.CSVLogger, pl_loggers.TensorBoardLogger)):
-                logger._root_dir = self.default_root_dir
-                logger._name = self._session_id
-                logger._version = subdirectory
+        enabled_loggers = []
+        if isinstance(self.loggers, list) and len(self.loggers) > 0:
+            for logger in self.loggers:
+                if isinstance(logger, (pl_loggers.CSVLogger, pl_loggers.TensorBoardLogger)):
+                    if not cloud_io._is_local_file_protocol(self.default_root_dir):
+                        loguru.logger.warning(
+                            f"Skipped {type(logger).__name__} as remote storage is not supported."
+                        )
+                        continue
+                    else:
+                        logger._root_dir = self.default_root_dir
+                        logger._name = self._session_id
+                        logger._version = subdirectory
+                enabled_loggers.append(logger)
+
+        self._loggers = enabled_loggers or [eva_loggers.DummyLogger(self._log_dir)]
 
     def run_evaluation_session(
         self,
         model: modules.ModelModule,
         datamodule: datamodules.DataModule,
     ) -> None:
         """Runs an evaluation session out-of-place.
@@ -90,8 +103,9 @@
             datamodule: The data module.
         """
         functional.run_evaluation_session(
             base_trainer=self,
             base_model=model,
             datamodule=datamodule,
             n_runs=self._n_runs,
+            verbose=self._n_runs > 1,
         )
```

### Comparing `kaiko_eva-0.0.1/src/eva/core/utils/multiprocessing.py` & `kaiko_eva-0.0.2/src/eva/core/utils/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/core/utils/workers.py` & `kaiko_eva-0.0.2/src/eva/core/utils/workers.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/vision/data/datasets/_utils.py` & `kaiko_eva-0.0.2/src/eva/vision/data/datasets/_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Dataset related function and helper functions."""
 
-from typing import List, Tuple
+from typing import List, Sequence, Tuple
 
 
 def indices_to_ranges(indices: List[int]) -> List[Tuple[int, int]]:
     """Turns a list of indices to a list of ranges.
 
     The produced range intervals are half-open inequalities: start <= x < end.
 
@@ -29,19 +29,19 @@
         end = start if start_index == i else current
         ranges.append((start, end + 1))
         start_index = i + 1
 
     return ranges
 
 
-def ranges_to_indices(ranges: List[Tuple[int, int]]) -> List[int]:
+def ranges_to_indices(ranges: Sequence[Tuple[int, int]]) -> List[int]:
     """Unpacks a list of ranges to individual indices.
 
     Args:
-        ranges: The list of ranges to produce the indices from.
+        ranges: A sequence of ranges to produce the indices from.
 
     Return:
         A list of the indices.
 
     Example:
         >>> ranges == [(0, 3), (4, 5), (6, 9)]
         >>> indices = ranges_to_indices(ranges)
```

### Comparing `kaiko_eva-0.0.1/src/eva/vision/data/datasets/_validators.py` & `kaiko_eva-0.0.2/src/eva/vision/data/datasets/_validators.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/vision/data/datasets/classification/bach.py` & `kaiko_eva-0.0.2/src/eva/vision/data/datasets/classification/bach.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/vision/data/datasets/classification/base.py` & `kaiko_eva-0.0.2/src/eva/vision/data/datasets/classification/base.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/vision/data/datasets/classification/crc.py` & `kaiko_eva-0.0.2/src/eva/vision/data/datasets/classification/crc.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/vision/data/datasets/classification/mhist.py` & `kaiko_eva-0.0.2/src/eva/vision/data/datasets/classification/mhist.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/vision/data/datasets/classification/patch_camelyon.py` & `kaiko_eva-0.0.2/src/eva/vision/data/datasets/classification/patch_camelyon.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/vision/data/datasets/classification/total_segmentator.py` & `kaiko_eva-0.0.2/src/eva/vision/data/datasets/segmentation/total_segmentator.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,33 +2,34 @@
 
 import functools
 import os
 from glob import glob
 from typing import Callable, Dict, List, Literal, Tuple
 
 import numpy as np
+from torchvision import tv_tensors
 from torchvision.datasets import utils
 from typing_extensions import override
 
 from eva.vision.data.datasets import _utils, _validators, structs
-from eva.vision.data.datasets.classification import base
-from eva.vision.utils import io
+from eva.vision.data.datasets.segmentation import base
+from eva.vision.utils import convert, io
 
 
-class TotalSegmentatorClassification(base.ImageClassification):
-    """TotalSegmentator multi-label classification dataset."""
+class TotalSegmentator2D(base.ImageSegmentation):
+    """TotalSegmentator 2D segmentation dataset."""
 
-    _train_index_ranges: List[Tuple[int, int]] = [(0, 83)]
-    """Train range indices."""
+    _expected_dataset_lengths: Dict[str, int] = {
+        "train_small": 29892,
+        "val_small": 6480,
+    }
+    """Dataset version and split to the expected size."""
 
-    _val_index_ranges: List[Tuple[int, int]] = [(83, 103)]
-    """Validation range indices."""
-
-    _n_slices_per_image: int = 20
-    """The amount of slices to sample per 3D CT scan image."""
+    _sample_every_n_slices: int | None = None
+    """The amount of slices to sub-sample per 3D CT scan image."""
 
     _resources_full: List[structs.DownloadResource] = [
         structs.DownloadResource(
             filename="Totalsegmentator_dataset_v201.zip",
             url="https://zenodo.org/records/10047292/files/Totalsegmentator_dataset_v201.zip",
             md5="fe250e5718e0a3b5df4c4ea9d58a62fe",
         ),
@@ -44,47 +45,45 @@
     ]
     """Resources for the small dataset version."""
 
     def __init__(
         self,
         root: str,
         split: Literal["train", "val"] | None,
-        version: Literal["small", "full"] = "small",
+        version: Literal["small", "full"] | None = "small",
         download: bool = False,
-        image_transforms: Callable | None = None,
-        target_transforms: Callable | None = None,
+        as_uint8: bool = True,
+        transforms: Callable | None = None,
     ) -> None:
         """Initialize dataset.
 
         Args:
             root: Path to the root directory of the dataset. The dataset will
                 be downloaded and extracted here, if it does not already exist.
-            split: Dataset split to use. If None, the entire dataset is used.
-            version: The version of the dataset to initialize.
+            split: Dataset split to use. If `None`, the entire dataset is used.
+            version: The version of the dataset to initialize. If `None`, it will
+                use the files located at root as is and wont perform any checks.
             download: Whether to download the data for the specified split.
                 Note that the download will be executed only by additionally
                 calling the :meth:`prepare_data` method and if the data does not
                 exist yet on disk.
-            image_transforms: A function/transform that takes in an image
-                and returns a transformed version.
-            target_transforms: A function/transform that takes in the target
-                and transforms it.
+            as_uint8: Whether to convert and return the images as a 8-bit.
+            transforms: A function/transforms that takes in an image and a target
+                mask and returns the transformed versions of both.
         """
-        super().__init__(
-            image_transforms=image_transforms,
-            target_transforms=target_transforms,
-        )
+        super().__init__(transforms=transforms)
 
         self._root = root
         self._split = split
         self._version = version
         self._download = download
+        self._as_uint8 = as_uint8
 
         self._samples_dirs: List[str] = []
-        self._indices: List[int] = []
+        self._indices: List[Tuple[int, int]] = []
 
     @functools.cached_property
     @override
     def classes(self) -> List[str]:
         def get_filename(path: str) -> str:
             """Returns the filename from the full path."""
             return os.path.basename(path).split(".")[0]
@@ -97,117 +96,136 @@
     @property
     @override
     def class_to_idx(self) -> Dict[str, int]:
         return {label: index for index, label in enumerate(self.classes)}
 
     @override
     def filename(self, index: int) -> str:
-        sample_dir = self._samples_dirs[self._indices[index]]
+        sample_idx, _ = self._indices[index]
+        sample_dir = self._samples_dirs[sample_idx]
         return os.path.join(sample_dir, "ct.nii.gz")
 
     @override
     def prepare_data(self) -> None:
         if self._download:
             self._download_dataset()
-        _validators.check_dataset_exists(self._root, True)
 
     @override
     def configure(self) -> None:
         self._samples_dirs = self._fetch_samples_dirs()
         self._indices = self._create_indices()
 
     @override
     def validate(self) -> None:
+        if self._version is None:
+            return
+
         _validators.check_dataset_integrity(
             self,
-            length=1660 if self._split == "train" else 400,
+            length=self._expected_dataset_lengths.get(f"{self._split}_{self._version}", 0),
             n_classes=117,
             first_and_last_labels=("adrenal_gland_left", "vertebrae_T9"),
         )
 
     @override
     def __len__(self) -> int:
-        return len(self._indices) * self._n_slices_per_image
+        return len(self._indices)
 
     @override
-    def load_image(self, index: int) -> np.ndarray:
-        image_path = self._get_image_path(index)
-        slice_index = self._get_sample_slice_index(index)
+    def load_image(self, index: int) -> tv_tensors.Image:
+        sample_index, slice_index = self._indices[index]
+        image_path = self._get_image_path(sample_index)
         image_array = io.read_nifti_slice(image_path, slice_index)
-        return image_array.repeat(3, axis=2)
+        if self._as_uint8:
+            image_array = convert.to_8bit(image_array)
+        image_rgb_array = image_array.repeat(3, axis=2)
+        return tv_tensors.Image(image_rgb_array.transpose(2, 0, 1))
 
     @override
-    def load_target(self, index: int) -> np.ndarray:
-        masks = self._load_masks(index)
-        targets = [1 in masks[..., mask_index] for mask_index in range(masks.shape[-1])]
-        return np.asarray(targets, dtype=np.int64)
-
-    def _load_masks(self, index: int) -> np.ndarray:
-        """Returns the `index`'th target mask sample."""
-        masks_dir = self._get_masks_dir(index)
-        slice_index = self._get_sample_slice_index(index)
+    def load_mask(self, index: int) -> tv_tensors.Mask:
+        sample_index, slice_index = self._indices[index]
+        masks_dir = self._get_masks_dir(sample_index)
         mask_paths = (os.path.join(masks_dir, label + ".nii.gz") for label in self.classes)
-        masks = [io.read_nifti_slice(path, slice_index) for path in mask_paths]
-        return np.concatenate(masks, axis=-1)
-
-    def _get_masks_dir(self, index: int) -> str:
-        """Returns the directory of the corresponding masks."""
-        sample_dir = self._get_sample_dir(index)
-        return os.path.join(self._root, sample_dir, "segmentations")
+        one_hot_encoded = np.concatenate(
+            [io.read_nifti_slice(path, slice_index) for path in mask_paths],
+            axis=2,
+        )
+        background_mask = one_hot_encoded.sum(axis=2, keepdims=True) == 0
+        one_hot_encoded_with_bg = np.concatenate([background_mask, one_hot_encoded], axis=2)
+        segmentation_label = np.argmax(one_hot_encoded_with_bg, axis=2)
+        return tv_tensors.Mask(segmentation_label)
 
-    def _get_image_path(self, index: int) -> str:
+    def _get_image_path(self, sample_index: int) -> str:
         """Returns the corresponding image path."""
-        sample_dir = self._get_sample_dir(index)
+        sample_dir = self._samples_dirs[sample_index]
         return os.path.join(self._root, sample_dir, "ct.nii.gz")
 
-    def _get_sample_dir(self, index: int) -> str:
-        """Returns the corresponding sample directory."""
-        sample_index = self._indices[index // self._n_slices_per_image]
-        return self._samples_dirs[sample_index]
-
-    def _get_sample_slice_index(self, index: int) -> int:
-        """Returns the corresponding slice index."""
-        image_path = self._get_image_path(index)
-        total_slices = io.fetch_total_nifti_slices(image_path)
-        slice_indices = np.linspace(0, total_slices - 1, num=self._n_slices_per_image, dtype=int)
-        return slice_indices[index % self._n_slices_per_image]
+    def _get_masks_dir(self, sample_index: int) -> str:
+        """Returns the directory of the corresponding masks."""
+        sample_dir = self._samples_dirs[sample_index]
+        return os.path.join(self._root, sample_dir, "segmentations")
+
+    def _get_number_of_slices_per_sample(self, sample_index: int) -> int:
+        """Returns the total amount of slices of a sample."""
+        image_path = self._get_image_path(sample_index)
+        return io.fetch_total_nifti_slices(image_path)
 
     def _fetch_samples_dirs(self) -> List[str]:
         """Returns the name of all the samples of all the splits of the dataset."""
         sample_filenames = [
             filename
             for filename in os.listdir(self._root)
             if os.path.isdir(os.path.join(self._root, filename))
         ]
         return sorted(sample_filenames)
 
-    def _create_indices(self) -> List[int]:
-        """Builds the dataset indices for the specified split."""
-        split_index_ranges = {
-            "train": self._train_index_ranges,
-            "val": self._val_index_ranges,
-            None: [(0, 103)],
-        }
-        index_ranges = split_index_ranges.get(self._split)
-        if index_ranges is None:
-            raise ValueError("Invalid data split. Use 'train', 'val' or `None`.")
+    def _get_split_indices(self) -> List[int]:
+        """Returns the samples indices that corresponding the dataset split and version."""
+        key = f"{self._split}_{self._version}"
+        match key:
+            case "train_small":
+                index_ranges = [(0, 83)]
+            case "val_small":
+                index_ranges = [(83, 102)]
+            case _:
+                index_ranges = [(0, len(self._samples_dirs))]
 
         return _utils.ranges_to_indices(index_ranges)
 
+    def _create_indices(self) -> List[Tuple[int, int]]:
+        """Builds the dataset indices for the specified split.
+
+        Returns:
+            A list of tuples, where the first value indicates the
+            sample index which the second its corresponding slice
+            index.
+        """
+        indices = [
+            (sample_idx, slide_idx)
+            for sample_idx in self._get_split_indices()
+            for slide_idx in range(self._get_number_of_slices_per_sample(sample_idx))
+            if slide_idx % (self._sample_every_n_slices or 1) == 0
+        ]
+        return indices
+
     def _download_dataset(self) -> None:
         """Downloads the dataset."""
         dataset_resources = {
             "small": self._resources_small,
             "full": self._resources_full,
-            None: (0, 103),
         }
-        resources = dataset_resources.get(self._version)
+        resources = dataset_resources.get(self._version or "")
         if resources is None:
-            raise ValueError("Invalid data version. Use 'small' or 'full'.")
+            raise ValueError(
+                f"Can't download data version '{self._version}'. Use 'small' or 'full'."
+            )
 
         for resource in resources:
+            if os.path.isdir(self._root):
+                continue
+
             utils.download_and_extract_archive(
                 resource.url,
                 download_root=self._root,
                 filename=resource.filename,
                 remove_finished=True,
             )
```

### Comparing `kaiko_eva-0.0.1/src/eva/vision/data/datasets/segmentation/base.py` & `kaiko_eva-0.0.2/src/eva/vision/data/datasets/segmentation/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,34 @@
 """Base for image segmentation datasets."""
 
 import abc
 from typing import Any, Callable, Dict, List, Tuple
 
-import numpy as np
+from torchvision import tv_tensors
 from typing_extensions import override
 
 from eva.vision.data.datasets import vision
 
 
-class ImageSegmentation(vision.VisionDataset[Tuple[np.ndarray, np.ndarray]], abc.ABC):
+class ImageSegmentation(vision.VisionDataset[Tuple[tv_tensors.Image, tv_tensors.Mask]], abc.ABC):
     """Image segmentation abstract dataset."""
 
     def __init__(
         self,
-        image_transforms: Callable | None = None,
-        target_transforms: Callable | None = None,
-        image_target_transforms: Callable | None = None,
+        transforms: Callable | None = None,
     ) -> None:
         """Initializes the image segmentation base class.
 
         Args:
-            image_transforms: A function/transform that takes in an image
-                and returns a transformed version.
-            target_transforms: A function/transform that takes in the target
-                and transforms it.
-            image_target_transforms: A function/transforms that takes in an
+            transforms: A function/transforms that takes in an
                 image and a label and returns the transformed versions of both.
-                This transform happens after the `image_transforms` and
-                `target_transforms`.
         """
         super().__init__()
 
-        self._image_transforms = image_transforms
-        self._target_transforms = target_transforms
-        self._image_target_transforms = image_target_transforms
+        self._transforms = transforms
 
     @property
     def classes(self) -> List[str] | None:
         """Returns the list with names of the dataset names."""
 
     @property
     def class_to_idx(self) -> Dict[str, int] | None:
@@ -52,61 +42,56 @@
                 If `None`, it will return the metadata of the current dataset.
 
         Returns:
             The sample metadata.
         """
 
     @abc.abstractmethod
-    def load_image(self, index: int) -> np.ndarray:
+    def load_image(self, index: int) -> tv_tensors.Image:
         """Loads and returns the `index`'th image sample.
 
         Args:
             index: The index of the data sample to load.
 
         Returns:
-            The image as a numpy array.
+            An image torchvision tensor (channels, height, width).
         """
 
     @abc.abstractmethod
-    def load_mask(self, index: int) -> np.ndarray:
-        """Returns the `index`'th target mask sample.
+    def load_mask(self, index: int) -> tv_tensors.Mask:
+        """Returns the `index`'th target masks sample.
 
         Args:
-            index: The index of the data sample target mask to load.
+            index: The index of the data sample target masks to load.
 
         Returns:
-            The sample mask as a stack of binary mask arrays (label, height, width).
+            The semantic mask as a (H x W) shaped tensor with integer
+            values which represent the pixel class id.
         """
 
     @abc.abstractmethod
     @override
     def __len__(self) -> int:
         raise NotImplementedError
 
     @override
-    def __getitem__(self, index: int) -> Tuple[np.ndarray, np.ndarray]:
+    def __getitem__(self, index: int) -> Tuple[tv_tensors.Image, tv_tensors.Mask]:
         image = self.load_image(index)
         mask = self.load_mask(index)
         return self._apply_transforms(image, mask)
 
     def _apply_transforms(
-        self, image: np.ndarray, target: np.ndarray
-    ) -> Tuple[np.ndarray, np.ndarray]:
+        self, image: tv_tensors.Image, mask: tv_tensors.Mask
+    ) -> Tuple[tv_tensors.Image, tv_tensors.Mask]:
         """Applies the transforms to the provided data and returns them.
 
         Args:
             image: The desired image.
-            target: The target of the image.
+            mask: The target segmentation mask.
 
         Returns:
-            A tuple with the image and the target transformed.
+            A tuple with the image and the masks transformed.
         """
-        if self._image_transforms is not None:
-            image = self._image_transforms(image)
+        if self._transforms is not None:
+            image, mask = self._transforms(image, mask)
 
-        if self._target_transforms is not None:
-            target = self._target_transforms(target)
-
-        if self._image_target_transforms is not None:
-            image, target = self._image_target_transforms(image, target)
-
-        return image, target
+        return image, mask
```

### Comparing `kaiko_eva-0.0.1/src/eva/vision/data/datasets/vision.py` & `kaiko_eva-0.0.2/src/eva/vision/data/datasets/vision.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/vision/data/transforms/common/resize_and_crop.py` & `kaiko_eva-0.0.2/src/eva/vision/data/transforms/common/resize_and_crop.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/vision/models/networks/abmil.py` & `kaiko_eva-0.0.2/src/eva/vision/models/networks/abmil.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/vision/models/networks/postprocesses/cls.py` & `kaiko_eva-0.0.2/src/eva/vision/models/networks/postprocesses/cls.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/vision/utils/io/_utils.py` & `kaiko_eva-0.0.2/src/eva/vision/utils/io/_utils.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/vision/utils/io/image.py` & `kaiko_eva-0.0.2/src/eva/vision/utils/io/image.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/src/eva/vision/utils/io/nifti.py` & `kaiko_eva-0.0.2/src/eva/vision/utils/io/nifti.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,35 +4,39 @@
 
 import nibabel as nib
 import numpy.typing as npt
 
 from eva.vision.utils.io import _utils
 
 
-def read_nifti_slice(path: str, slice_index: int) -> npt.NDArray[Any]:
+def read_nifti_slice(
+    path: str, slice_index: int, *, use_storage_dtype: bool = True
+) -> npt.NDArray[Any]:
     """Reads and loads a NIfTI image from a file path as `uint8`.
 
     Args:
         path: The path to the NIfTI file.
-        slice_index: The image slice index to return. If `None`, it will
-            return the full 3D image.
+        slice_index: The image slice index to return.
+        use_storage_dtype: Whether to cast the raw image
+            array to the inferred type.
 
     Returns:
-        The image as a numpy array.
+        The image as a numpy array (height, width, channels).
 
     Raises:
         FileExistsError: If the path does not exist or it is unreachable.
         ValueError: If the input channel is invalid for the image.
     """
     _utils.check_file(path)
     image_data = nib.load(path)  # type: ignore
-    dtype = image_data.get_data_dtype()  # type: ignore
     image_slice = image_data.slicer[:, :, slice_index : slice_index + 1]  # type: ignore
     image_array = image_slice.get_fdata()
-    return image_array.astype(dtype)
+    if use_storage_dtype:
+        image_array = image_array.astype(image_data.get_data_dtype())  # type: ignore
+    return image_array
 
 
 def fetch_total_nifti_slices(path: str) -> int:
     """Fetches the total slides of a NIfTI image file.
 
     Args:
         path: The path to the NIfTI file.
```

### Comparing `kaiko_eva-0.0.1/tests/eva/_cli.py` & `kaiko_eva-0.0.2/tests/eva/_cli.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0011/ct.nii.gz` & `kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0011/ct.nii.gz`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0461/ct.nii.gz` & `kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0461/ct.nii.gz`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0762/ct.nii.gz` & `kaiko_eva-0.0.2/tests/eva/assets/vision/datasets/total_segmentator/Totalsegmentator_dataset_v201/s0762/ct.nii.gz`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/conftest.py` & `kaiko_eva-0.0.2/tests/eva/conftest.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/core/callbacks/conftest.py` & `kaiko_eva-0.0.2/tests/eva/core/callbacks/conftest.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/core/callbacks/writers/test_embeddings.py` & `kaiko_eva-0.0.2/tests/eva/core/callbacks/writers/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/core/data/dataloaders/test_dataloader.py` & `kaiko_eva-0.0.2/tests/eva/core/data/dataloaders/test_dataloader.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/core/data/datamodules/_utils.py` & `kaiko_eva-0.0.2/tests/eva/core/data/datamodules/_utils.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/core/data/datamodules/test_datamodule.py` & `kaiko_eva-0.0.2/tests/eva/core/data/datamodules/test_datamodule.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/core/data/datamodules/test_schemas.py` & `kaiko_eva-0.0.2/tests/eva/core/data/datamodules/test_schemas.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/core/data/datasets/classification/test_embedding_datasets.py` & `kaiko_eva-0.0.2/tests/eva/core/data/datasets/embeddings/classification/test_embeddings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 """Tests for the embeddings datasets."""
 
 import os
-from typing import Tuple
+from typing import Literal
 
 import numpy as np
 import pytest
 import torch
 
-from eva.core.data.datasets import classification
+from eva.core.data.datasets.embeddings import classification
 
 
-@pytest.mark.parametrize(
-    "split, embeddings_shape",
-    [("train", (8,)), ("val", (8,))],
-)
-def test_patch_embedding_dataset(
-    patch_embeddings_dataset: classification.EmbeddingsClassificationDataset,
-    embeddings_shape: Tuple[int, ...],
-):
-    """Test that the EmbeddingsClassificationDataset level dataset."""
+@pytest.mark.parametrize("split", ["train", "val"])
+def test_embedding_dataset(embeddings_dataset: classification.EmbeddingsClassificationDataset):
+    """Tests that the dataset returns data in the expected format."""
     # assert data sample is a tuple
-    sample = patch_embeddings_dataset[0]
+    sample = embeddings_dataset[0]
     assert isinstance(sample, tuple)
     assert len(sample) == 2
     # assert the format of the `image` and `target`
     embeddings, target = sample
     assert isinstance(embeddings, torch.Tensor)
-    assert embeddings.shape == embeddings_shape
+    assert embeddings.shape == (8,)
     assert isinstance(target, np.ndarray)
     assert target in [0, 1]
 
 
 @pytest.fixture(scope="function")
-def patch_embeddings_dataset(
-    split: str, assets_path: str
+def embeddings_dataset(
+    split: Literal["train", "val", "test"], root_dir: str
 ) -> classification.EmbeddingsClassificationDataset:
     """EmbeddingsClassificationDataset dataset fixture."""
     dataset = classification.EmbeddingsClassificationDataset(
-        root=os.path.join(assets_path, "core", "datasets", "embeddings"),
+        root=root_dir,
         manifest_file="manifest.csv",
         split=split,
     )
     dataset.prepare_data()
     dataset.setup()
     return dataset
+
+
+@pytest.fixture(scope="function")
+def root_dir(assets_path: str):
+    """Returns the root directory of the test embeddings dataset."""
+    return os.path.join(assets_path, "core", "datasets", "embeddings")
```

### Comparing `kaiko_eva-0.0.1/tests/eva/core/metrics/core/test_metric_module.py` & `kaiko_eva-0.0.2/tests/eva/core/metrics/core/test_metric_module.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/core/metrics/core/test_schemas.py` & `kaiko_eva-0.0.2/tests/eva/core/metrics/core/test_schemas.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/core/metrics/defaults/classification/test_binary.py` & `kaiko_eva-0.0.2/tests/eva/core/metrics/defaults/classification/test_binary.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/core/metrics/defaults/classification/test_multiclass.py` & `kaiko_eva-0.0.2/tests/eva/core/metrics/defaults/classification/test_multiclass.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/core/metrics/test_average_loss.py` & `kaiko_eva-0.0.2/tests/eva/core/metrics/test_average_loss.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/core/metrics/test_binary_balanced_accuracy.py` & `kaiko_eva-0.0.2/tests/eva/core/metrics/test_binary_balanced_accuracy.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/core/models/modules/conftest.py` & `kaiko_eva-0.0.2/tests/eva/core/models/modules/conftest.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/core/models/modules/test_head.py` & `kaiko_eva-0.0.2/tests/eva/core/models/modules/test_head.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/core/models/modules/test_inference.py` & `kaiko_eva-0.0.2/tests/eva/core/models/modules/test_inference.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/core/models/modules/utils/test_batch_postproces.py` & `kaiko_eva-0.0.2/tests/eva/core/models/modules/utils/test_batch_postproces.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/core/models/networks/test_mlp.py` & `kaiko_eva-0.0.2/tests/eva/core/models/networks/test_mlp.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/core/models/networks/wrappers/test_from_function.py` & `kaiko_eva-0.0.2/tests/eva/core/models/networks/wrappers/test_from_function.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/core/models/networks/wrappers/test_huggingface.py` & `kaiko_eva-0.0.2/tests/eva/core/models/networks/wrappers/test_huggingface.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/core/models/networks/wrappers/test_onnx.py` & `kaiko_eva-0.0.2/tests/eva/core/models/networks/wrappers/test_onnx.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/core/test_cli.py` & `kaiko_eva-0.0.2/tests/eva/core/test_cli.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/core/trainers/test_recorder.py` & `kaiko_eva-0.0.2/tests/eva/core/trainers/test_recorder.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/vision/data/datasets/classification/test_bach.py` & `kaiko_eva-0.0.2/tests/eva/vision/data/datasets/classification/test_bach.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/vision/data/datasets/classification/test_crc.py` & `kaiko_eva-0.0.2/tests/eva/vision/data/datasets/classification/test_crc.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/vision/data/datasets/classification/test_mhist.py` & `kaiko_eva-0.0.2/tests/eva/vision/data/datasets/classification/test_mhist.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/vision/data/datasets/classification/test_patch_camelyon.py` & `kaiko_eva-0.0.2/tests/eva/vision/data/datasets/classification/test_patch_camelyon.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/vision/data/datasets/classification/test_total_segmentator.py` & `kaiko_eva-0.0.2/tests/eva/vision/data/datasets/segmentation/test_total_segmentator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-"""TotalSegmentator dataset tests."""
+"""TotalSegmentator2D dataset tests."""
 
 import os
 from typing import Literal
 
-import numpy as np
 import pytest
+from torchvision import tv_tensors
 
 from eva.vision.data import datasets
 
 
 @pytest.mark.parametrize(
     "split, expected_length",
-    [("train", 1660), ("val", 400), (None, 2060)],
+    [("train", 9), ("val", 9), (None, 9)],
 )
 def test_length(
-    total_segmentator_dataset: datasets.TotalSegmentatorClassification, expected_length: int
+    total_segmentator_dataset: datasets.TotalSegmentator2D, expected_length: int
 ) -> None:
     """Tests the length of the dataset."""
     assert len(total_segmentator_dataset) == expected_length
 
 
 @pytest.mark.parametrize(
-    "split",
+    "split, index",
     [
-        None,
-        "train",
+        (None, 0),
+        ("train", 0),
+        ("val", 0),
     ],
 )
-def test_sample(total_segmentator_dataset: datasets.TotalSegmentatorClassification) -> None:
+def test_sample(total_segmentator_dataset: datasets.TotalSegmentator2D, index: int) -> None:
     """Tests the format of a dataset sample."""
     # assert data sample is a tuple
-    sample = total_segmentator_dataset[0]
+    sample = total_segmentator_dataset[index]
     assert isinstance(sample, tuple)
     assert len(sample) == 2
-    # assert the format of the `image` and `target`
-    image, target = sample
-    assert isinstance(image, np.ndarray)
-    assert image.shape == (16, 16, 3)
-    assert isinstance(target, np.ndarray)
-    assert all(target == [0, 0, 0])
+    # assert the format of the `image` and `mask`
+    image, mask = sample
+    assert isinstance(image, tv_tensors.Image)
+    assert image.shape == (3, 16, 16)
+    assert isinstance(mask, tv_tensors.Mask)
+    assert mask.shape == (16, 16)
 
 
 @pytest.fixture(scope="function")
 def total_segmentator_dataset(
-    split: Literal["train", "val"],
-    assets_path: str,
-) -> datasets.TotalSegmentatorClassification:
-    """TotalSegmentator dataset fixture."""
-    dataset = datasets.TotalSegmentatorClassification(
+    split: Literal["train", "val"] | None, assets_path: str
+) -> datasets.TotalSegmentator2D:
+    """TotalSegmentator2D dataset fixture."""
+    dataset = datasets.TotalSegmentator2D(
         root=os.path.join(
             assets_path,
             "vision",
             "datasets",
             "total_segmentator",
             "Totalsegmentator_dataset_v201",
         ),
         split=split,
-        download=False,
+        version=None,
     )
     dataset.prepare_data()
     dataset.configure()
     return dataset
```

### Comparing `kaiko_eva-0.0.1/tests/eva/vision/data/transforms/common/test_resize_and_crop.py` & `kaiko_eva-0.0.2/tests/eva/vision/data/transforms/common/test_resize_and_crop.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/vision/models/networks/test_abmil.py` & `kaiko_eva-0.0.2/tests/eva/vision/models/networks/test_abmil.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/vision/test_vision_cli.py` & `kaiko_eva-0.0.2/tests/eva/vision/test_vision_cli.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/tests/eva/vision/utils/io/test_image.py` & `kaiko_eva-0.0.2/tests/eva/vision/utils/io/test_image.py`

 * *Files identical despite different names*

### Comparing `kaiko_eva-0.0.1/PKG-INFO` & `kaiko_eva-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: kaiko-eva
-Version: 0.0.1
+Version: 0.0.2
 Summary: Evaluation Framework for oncology foundation models.
-Keywords: machine-learning evaluation-framework oncology foundation-models
-Author-Email: Ioannis Gatopoulos <ioannis@kaiko.ai>, Nicolas Känzig <nicolas@kaiko.ai>, Roman Moser <roman@kaiko.ai>
-Maintainer-Email: Ioannis Gatopoulos <ioannis@kaiko.ai>, Nicolas Känzig <nicolas@kaiko.ai>, Roman Moser <roman@kaiko.ai>
+Keywords: machine-learning,evaluation-framework,oncology,foundation-models
+Author-Email: Ioannis Gatopoulos <ioannis@kaiko.ai>, =?utf-8?q?Nicolas_K=C3=A4nzig?= <nicolas@kaiko.ai>, Roman Moser <roman@kaiko.ai>
+Maintainer-Email: Ioannis Gatopoulos <ioannis@kaiko.ai>, =?utf-8?q?Nicolas_K=C3=A4nzig?= <nicolas@kaiko.ai>, Roman Moser <roman@kaiko.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
            1. Definitions.
@@ -211,23 +211,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Homepage, https://kaiko-ai.github.io/eva/dev/
 Project-URL: Repository, https://github.com/kaiko-ai/eva
 Project-URL: Documentation, https://kaiko-ai.github.io/eva/dev/
 Requires-Python: >=3.10
-Requires-Dist: lightning>=2.2.1
-Requires-Dist: jsonargparse[omegaconf]>=4.27.4
+Requires-Dist: torch==2.3.0
+Requires-Dist: lightning>=2.2.2
+Requires-Dist: jsonargparse[omegaconf]==4.28
 Requires-Dist: tensorboard>=2.16.2
 Requires-Dist: loguru>=0.7.2
 Requires-Dist: pandas>=2.2.0
 Requires-Dist: transformers>=4.38.2
 Requires-Dist: onnxruntime>=1.17.1
-Requires-Dist: onnx>=1.15.0
+Requires-Dist: onnx>=1.16.0
 Requires-Dist: toolz>=0.12.1
+Requires-Dist: rich>=13.7.1
 Requires-Dist: h5py>=3.10.0; extra == "vision"
 Requires-Dist: nibabel>=5.2.0; extra == "vision"
 Requires-Dist: opencv-python-headless>=4.9.0.80; extra == "vision"
 Requires-Dist: timm>=0.9.12; extra == "vision"
 Requires-Dist: torchvision>=0.17.0; extra == "vision"
 Requires-Dist: h5py>=3.10.0; extra == "all"
 Requires-Dist: nibabel>=5.2.0; extra == "all"
@@ -236,23 +238,27 @@
 Requires-Dist: torchvision>=0.17.0; extra == "all"
 Provides-Extra: vision
 Provides-Extra: all
 Description-Content-Type: text/markdown
 
 <div align="center">
 
-<img src="https://github.com/kaiko-ai/eva/blob/main/docs/images/eva-logo.png?raw=true" width="400">
+<br />
+
+<img src="https://github.com/kaiko-ai/eva/blob/main/docs/images/eva-logo.png?raw=true" width="340">
 
 <br />
+<br />
 
 _Oncology FM Evaluation Framework by kaiko.ai_
 
 [![PyPI](https://img.shields.io/pypi/v/kaiko-eva.svg?logo=python)](https://pypi.python.org/pypi/kaiko-eva)
-[![CI](https://github.com/kaiko-ai/eva/workflows/CI/badge.svg)](https://github.com/kaiko-ai/eva/actions?query=workflow%3ACI)
-[![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg?labelColor=gray)](https://github.com/kaiko-ai/eva#license)
+[![docs](https://img.shields.io/badge/📚_docs-latest-green)](https://kaiko-ai.github.io/eva/latest)
+[![license](https://img.shields.io/badge/⚖️_License-Apache%202.0-blue.svg?labelColor=gray)](https://github.com/kaiko-ai/eva#license)<br>
+[![paper](http://img.shields.io/badge/OpenReview-MIDL_2024-B31B1B.svg)](https://openreview.net/forum?id=FNBQOPj18N&noteId=FNBQOPj18N)
 
 <p align="center">
   <a href="https://github.com/kaiko-ai/eva#installation">Installation</a> •
   <a href="https://github.com/kaiko-ai/eva#how-to-use">How To Use</a> •
   <a href="https://kaiko-ai.github.io/eva/">Documentation</a> •
   <a href="https://kaiko-ai.github.io/eva/dev/datasets/">Datasets</a> •
   <a href="https://github.com/kaiko-ai/eva#benchmarks">Benchmarks</a> <br>
@@ -295,26 +301,26 @@
 You can verify that the installation was successful by executing:
 ```sh
 eva --version
 ```
 
 ## How To Use
 
-_eva_ can be used directly from the terminal as a CLI tool as follows:
+_`eva`_ can be used directly from the terminal as a CLI tool as follows:
 ```sh
 eva {fit,predict,predict_fit} --config url/or/path/to/the/config.yaml 
 ```
 
-When used as a CLI tool, `_eva_` supports configuration files (`.yaml`) as an argument to define its functionality.
+When used as a CLI tool, _`eva`_ supports configuration files (`.yaml`) as an argument to define its functionality.
 Native supported configs can be found at the [configs](https://github.com/kaiko-ai/eva/tree/main/configs) directory
 of the repo. Apart from cloning the repo, you can download the latest config folder as `.zip` from your browser from
 [here](https://download-directory.github.io/?url=https://github.com/kaiko-ai/eva/tree/main/configs). Alternatively,
 from a specific release the configs can be downloaded from the terminal as follows:
 ```sh
-curl -LO https://github.com/kaiko-ai/eva/releases/download/0.0.1/configs.zip | unzip configs.zip
+curl -LO https://github.com/kaiko-ai/eva/releases/download/0.0.1/configs.zip | unzip configs
 ```
 
 For example, to perform a downstream evaluation of DINO ViT-S/16 on the BACH dataset with
 linear probing by first inferring the embeddings and performing 5 sequential fits, execute:
 ```sh
 # from a locally stored config file
 eva predict_fit --config ./configs/vision/dino_vit/offline/bach.yaml
@@ -334,51 +340,54 @@
 ```
 
 For more information, please refer to the [documentation](https://kaiko-ai.github.io/eva/dev/user-guide/tutorials/offline_vs_online/)
 and [tutorials](https://kaiko-ai.github.io/eva/dev/user-guide/advanced/replicate_evaluations/).
 
 ## Benchmarks
 
-In this section you will find model benchmarks which were generated with _eva_.
+In this section you will find model benchmarks which were generated with _`eva`_.
 
 ### Table I: WSI patch-level benchmark
 
 <br />
 
 <div align="center">
 
 | Model                                            | BACH  | CRC   | MHIST | PCam/val | PCam/test |
 |--------------------------------------------------|-------|-------|-------|----------|-----------|
 | ViT-S/16 _(random)_	<sup>[1]</sup>               | 0.410 | 0.617 | 0.501 | 0.753    | 0.728     |
 | ViT-S/16 _(ImageNet)_ <sup>[1]</sup>             | 0.695 | 0.935 | 0.831 | 0.864    | 0.849     |
 | ViT-B/8 _(ImageNet)_ <sup>[1]</sup>              | 0.710 | 0.939 | 0.814 | 0.870    | 0.856     |
+| ViT-L/14 _(ImageNet)_ <sup>[1]</sup>             | 0.707 | 0.916 | 0.832 | 0.873    | 0.888     |
 | DINO<sub>(p=16)</sub> <sup>[2]</sup>             | 0.801 | 0.934 | 0.768 | 0.889    | 0.895     |
 | Phikon <sup>[3]</sup>                            | 0.725 | 0.935 | 0.777 | 0.912    | 0.915     |
-| ViT-S/16 _(kaiko.ai)_ <sup>[4]</sup>             | 0.797 | 0.943 | 0.828 | 0.903    | 0.893     |
-| ViT-S/8 _(kaiko.ai)_ <sup>[4]</sup>              | 0.834 | 0.946 | 0.832 | 0.897    | 0.887     |
-| ViT-B/16 _(kaiko.ai)_	<sup>[4]</sup>             | 0.810 | 0.960 | 0.826 | 0.900    | 0.898     |
-| ViT-B/8 _(kaiko.ai)_ <sup>[4]</sup>              | 0.865 | 0.956 | 0.809 | 0.913    | 0.921     |
-| ViT-L/14 _(kaiko.ai)_ <sup>[4]</sup>             | 0.870 | 0.930 | 0.809 | 0.908    | 0.898     |
+| UNI <sup>[4]</sup>                               | 0.814 | 0.950 | 0.837 | 0.936    | 0.938     |
+| ViT-S/16 _(kaiko.ai)_ <sup>[5]</sup>             | 0.797 | 0.943 | 0.828 | 0.903    | 0.893     |
+| ViT-S/8 _(kaiko.ai)_ <sup>[5]</sup>              | 0.834 | 0.946 | 0.832 | 0.897    | 0.887     |
+| ViT-B/16 _(kaiko.ai)_	<sup>[5]</sup>             | 0.810 | 0.960 | 0.826 | 0.900    | 0.898     |
+| ViT-B/8 _(kaiko.ai)_ <sup>[5]</sup>              | 0.865 | 0.956 | 0.809 | 0.913    | 0.921     |
+| ViT-L/14 _(kaiko.ai)_ <sup>[5]</sup>             | 0.870 | 0.930 | 0.809 | 0.908    | 0.898     |
 
 _Table I: Linear probing evaluation of FMs on patch-level downstream datasets.<br> We report averaged balanced accuracy
 over 5 runs, with an average standard deviation of ±0.003._
 
 </div>
 
 <br />
 
 _References_:
-1. _"Emerging properties in self-supervised vision transformers”_
-2. _"Benchmarking self-supervised learning on diverse pathology datasets”_
-3. _"Scaling self-supervised learning for histopathology with masked image modeling”_
-4. _"Towards Training Large-Scale Pathology Foundation Models: from TCGA to Hospital Scale”_
+1. _"Emerging properties in self-supervised vision transformers”_, [arXiv](https://arxiv.org/abs/2104.14294)
+2. _"Benchmarking self-supervised learning on diverse pathology datasets”_, [arXiv](https://arxiv.org/abs/2212.04690)
+3. _"Scaling self-supervised learning for histopathology with masked image modeling”_, [medRxiv](https://www.medrxiv.org/content/10.1101/2023.07.21.23292757v1)
+4. _"A General-Purpose Self-Supervised Model for Computational Pathology”_, [arXiv](https://arxiv.org/abs/2308.15474)
+5. _"Towards Training Large-Scale Pathology Foundation Models: from TCGA to Hospital Scale”_, [arXiv](https://arxiv.org/pdf/2404.15217)
 
 ## Contributing
 
-_eva_ is an open source project and welcomes contributions of all kinds. Please checkout the [developer](./docs/DEVELOPER_GUIDE.md)
+_`eva`_ is an open source project and welcomes contributions of all kinds. Please checkout the [developer](./docs/DEVELOPER_GUIDE.md)
 and [contributing guide](./docs/CONTRIBUTING.md) for help on how to do so.
 
 All contributors must follow the [code of conduct](./docs/CODE_OF_CONDUCT.md).
 
 
 ## Acknowledgements
 
@@ -395,11 +404,28 @@
 [![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)<br>
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm-project.org)
 [![Nox](https://img.shields.io/badge/%F0%9F%A6%8A-Nox-D85E00.svg)](https://github.com/wntrblm/nox)
 [![Built with Material for MkDocs](https://img.shields.io/badge/Material_for_MkDocs-526CFE?logo=MaterialForMkDocs&logoColor=white)](https://squidfunk.github.io/mkdocs-material/)
 
 </div>
 
----
+
+## Citation
+
+If you find this repository useful, please consider giving a star ⭐ and adding the following citation:
+
+```
+@inproceedings{
+kaiko.ai2024eva,
+title={eva: Evaluation framework for pathology foundation models},
+author={kaiko.ai and Ioannis Gatopoulos and Nicolas K{\"a}nzig and Roman Moser and Sebastian Ot{\'a}lora},
+booktitle={Medical Imaging with Deep Learning},
+year={2024},
+url={https://openreview.net/forum?id=FNBQOPj18N}
+}
+```
+
+<br />
+
 <div align="center">
   <img src="https://github.com/kaiko-ai/eva/blob/main/docs/images/kaiko-logo.png?raw=true" width="200">
 </div>
```

