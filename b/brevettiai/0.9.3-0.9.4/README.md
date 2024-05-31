# Comparing `tmp/brevettiai-0.9.3.tar.gz` & `tmp/brevettiai-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brevettiai-0.9.3.tar", max compression
+gzip compressed data, was "brevettiai-0.9.4.tar", max compression
```

## Comparing `brevettiai-0.9.3.tar` & `brevettiai-0.9.4.tar`

### file list

```diff
@@ -1,140 +1,140 @@
--rw-r--r--   0        0        0    11358 2024-01-23 10:01:00.277232 brevettiai-0.9.3/LICENSE
--rw-r--r--   0        0        0      678 2024-01-23 10:01:00.277232 brevettiai-0.9.3/README.md
--rw-r--r--   0        0        0      306 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/__init__.py
--rw-r--r--   0        0        0      156 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/data/__init__.py
--rw-r--r--   0        0        0    21606 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/data/data_generator.py
--rw-r--r--   0        0        0      374 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/data/image/__init__.py
--rw-r--r--   0        0        0       86 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/data/image/annotation.py
--rw-r--r--   0        0        0     4805 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/data/image/annotation_loader.py
--rw-r--r--   0        0        0    10337 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/data/image/annotation_parser.py
--rw-r--r--   0        0        0     1683 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/data/image/annotation_pooling.py
--rw-r--r--   0        0        0      872 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/data/image/bayer_demosaic.py
--rw-r--r--   0        0        0    14515 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/data/image/bcimg_dataset.py
--rw-r--r--   0        0        0    26860 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/data/image/image_augmenter.py
--rw-r--r--   0        0        0    12005 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/data/image/image_loader.py
--rw-r--r--   0        0        0    10337 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/data/image/image_pipeline.py
--rw-r--r--   0        0        0      877 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/data/image/image_processor.py
--rw-r--r--   0        0        0     1271 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/data/image/image_region.py
--rw-r--r--   0        0        0      223 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/data/image/modules.py
--rw-r--r--   0        0        0     4612 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/data/image/multi_frame_imager.py
--rw-r--r--   0        0        0     4254 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/data/image/segmentation_loader.py
--rw-r--r--   0        0        0     5511 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/data/image/sequence_loader.py
--rw-r--r--   0        0        0    15180 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/data/image/utils.py
--rw-r--r--   0        0        0     1481 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/data/inspection_info.py
--rw-r--r--   0        0        0    10164 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/data/sample_integrity.py
--rw-r--r--   0        0        0     9711 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/data/sample_tools.py
--rw-r--r--   0        0        0     1075 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/data/serialization.py
--rw-r--r--   0        0        0     1292 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/data/tf_serialization.py
--rw-r--r--   0        0        0     4617 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/data/tf_types.py
--rw-r--r--   0        0        0     6422 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/data/tf_utils.py
--rw-r--r--   0        0        0      423 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/datamodel/__init__.py
--rw-r--r--   0        0        0      348 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/datamodel/camelmodel.py
--rw-r--r--   0        0        0      987 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/datamodel/color.py
--rw-r--r--   0        0        0     4092 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/datamodel/dataset.py
--rw-r--r--   0        0        0     4884 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/datamodel/image.py
--rw-r--r--   0        0        0     5656 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/datamodel/image_annotation.py
--rw-r--r--   0        0        0     1140 2024-01-23 10:01:00.277232 brevettiai-0.9.3/brevettiai/datamodel/tag.py
--rw-r--r--   0        0        0     7570 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/datamodel/web_api_types.py
--rw-r--r--   0        0        0     3819 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/examples/explore_application.py
--rw-r--r--   0        0        0      465 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/examples/plot_annotation.py
--rw-r--r--   0        0        0     1439 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/examples/run_experiment.py
--rw-r--r--   0        0        0       71 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/interfaces/__init__.py
--rw-r--r--   0        0        0     3101 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/interfaces/aws.py
--rw-r--r--   0        0        0     4862 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/interfaces/facets_atlas.py
--rw-r--r--   0        0        0     2357 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/interfaces/git_state.py
--rw-r--r--   0        0        0     2558 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/interfaces/package_validation.py
--rw-r--r--   0        0        0     3559 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/interfaces/pivot.py
--rw-r--r--   0        0        0     2268 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/interfaces/raygun.py
--rw-r--r--   0        0        0     2311 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/interfaces/remote_monitor.py
--rw-r--r--   0        0        0     1783 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/interfaces/sagemaker.py
--rw-r--r--   0        0        0    21985 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/interfaces/vue_schema_utils.py
--rw-r--r--   0        0        0      451 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/io/__init__.py
--rw-r--r--   0        0        0    15551 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/io/cloudpath.py
--rw-r--r--   0        0        0     1344 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/io/credentials.py
--rw-r--r--   0        0        0     4160 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/io/file_cache.py
--rw-r--r--   0        0        0     2071 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/io/files.py
--rw-r--r--   0        0        0      743 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/io/h5_metadata.py
--rw-r--r--   0        0        0     4677 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/io/local_io.py
--rw-r--r--   0        0        0     8813 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/io/minio_io.py
--rw-r--r--   0        0        0     4923 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/io/onnx.py
--rw-r--r--   0        0        0     2325 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/io/path.py
--rw-r--r--   0        0        0     1184 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/io/serialization.py
--rw-r--r--   0        0        0     2790 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/io/smart_open_patch.py
--rw-r--r--   0        0        0     3577 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/io/tf_recorder.py
--rw-r--r--   0        0        0     1365 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/io/url_io.py
--rw-r--r--   0        0        0     6825 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/io/utils.py
--rw-r--r--   0        0        0        0 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/ml/__init__.py
--rw-r--r--   0        0        0       47 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/ml/tensorflow/__init__.py
--rw-r--r--   0        0        0     5996 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/ml/tensorflow/annotation_loader.py
--rw-r--r--   0        0        0      111 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/model/__init__.py
--rw-r--r--   0        0        0     2692 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/model/catalogue.py
--rw-r--r--   0        0        0      534 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/model/factory/__init__.py
--rw-r--r--   0        0        0     2191 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/model/factory/lenet_backbone.py
--rw-r--r--   0        0        0     8746 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/model/factory/lraspp.py
--rw-r--r--   0        0        0     3690 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/model/factory/mobilenetv2_backbone.py
--rw-r--r--   0        0        0     2652 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/model/factory/segmentation.py
--rw-r--r--   0        0        0     2510 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/model/factory/unet.py
--rw-r--r--   0        0        0     2972 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/model/losses.py
--rw-r--r--   0        0        0      137 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/model/metadata/__init__.py
--rw-r--r--   0        0        0     1465 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/model/metadata/history.py
--rw-r--r--   0        0        0     2805 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/model/metadata/image_segmentation.py
--rw-r--r--   0        0        0      538 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/model/metadata/inference.py
--rw-r--r--   0        0        0     2903 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/model/metadata/metadata.py
--rw-r--r--   0        0        0      346 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/platform/__init__.py
--rw-r--r--   0        0        0     8568 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/platform/aipackage.py
--rw-r--r--   0        0        0     2758 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/platform/annotations.py
--rw-r--r--   0        0        0     1274 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/platform/dataset.py
--rw-r--r--   0        0        0     3231 2024-01-23 10:01:00.281232 brevettiai-0.9.3/brevettiai/platform/dataset_items.py
--rw-r--r--   0        0        0     8145 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/platform/model_archive.py
--rw-r--r--   0        0        0      368 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/platform/models/__init__.py
--rw-r--r--   0        0        0    21202 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/platform/models/annotation.py
--rw-r--r--   0        0        0    12476 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/platform/models/dataset.py
--rw-r--r--   0        0        0      370 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/platform/models/iomodel.py
--rw-r--r--   0        0        0    21112 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/platform/models/job.py
--rw-r--r--   0        0        0     5142 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/platform/models/platform_backend.py
--rw-r--r--   0        0        0     3720 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/platform/platform_credentials.py
--rw-r--r--   0        0        0    28260 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/platform/web_api.py
--rw-r--r--   0        0        0   150582 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/tests/bin/0_1543413266626.bmp
--rw-r--r--   0        0        0     6796 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/tests/bin/1651574629796.json
--rw-r--r--   0        0        0      249 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/tests/get_resources.py
--rw-r--r--   0        0        0     1767 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/tests/test_aipackage.py
--rw-r--r--   0        0        0     5092 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/tests/test_annotation_loader.py
--rw-r--r--   0        0        0     5858 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/tests/test_annotation_tooling.py
--rw-r--r--   0        0        0    15003 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/tests/test_data.py
--rw-r--r--   0        0        0     5048 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/tests/test_data_image.py
--rw-r--r--   0        0        0      882 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/tests/test_data_manipulation.py
--rw-r--r--   0        0        0      468 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/tests/test_generate_model_name.py
--rw-r--r--   0        0        0     3923 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/tests/test_image_loader.py
--rw-r--r--   0        0        0     1329 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/tests/test_model_archive.py
--rw-r--r--   0        0        0      577 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/tests/test_model_catalogue.py
--rw-r--r--   0        0        0     1139 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/tests/test_model_loss.py
--rw-r--r--   0        0        0     3500 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/tests/test_model_metadata.py
--rw-r--r--   0        0        0     1574 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/tests/test_pivot.py
--rw-r--r--   0        0        0     1249 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/tests/test_platform_annotation.py
--rw-r--r--   0        0        0     1263 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/tests/test_platform_job.py
--rw-r--r--   0        0        0     3732 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/tests/test_polygon_extraction.py
--rw-r--r--   0        0        0     1795 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/tests/test_schema.py
--rw-r--r--   0        0        0     1200 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/tests/test_tags.py
--rw-r--r--   0        0        0      667 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/tests/test_web_api.py
--rw-r--r--   0        0        0        0 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/tooling/__init__.py
--rw-r--r--   0        0        0     5288 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/tooling/annotation_tools.py
--rw-r--r--   0        0        0     7335 2024-01-23 10:01:00.285232 brevettiai-0.9.3/brevettiai/tooling/experiments.py
--rw-r--r--   0        0        0     1633 2024-01-23 10:01:00.289232 brevettiai-0.9.3/brevettiai/tooling/plot.py
--rw-r--r--   0        0        0       67 2024-01-23 10:01:00.289232 brevettiai-0.9.3/brevettiai/utils/__init__.py
--rw-r--r--   0        0        0     1117 2024-01-23 10:01:00.289232 brevettiai-0.9.3/brevettiai/utils/argparse_utils.py
--rw-r--r--   0        0        0      614 2024-01-23 10:01:00.289232 brevettiai-0.9.3/brevettiai/utils/dict_utils.py
--rw-r--r--   0        0        0      536 2024-01-23 10:01:00.289232 brevettiai-0.9.3/brevettiai/utils/env_variables.py
--rw-r--r--   0        0        0     2651 2024-01-23 10:01:00.289232 brevettiai-0.9.3/brevettiai/utils/model_version.py
--rw-r--r--   0        0        0     2589 2024-01-23 10:01:00.289232 brevettiai-0.9.3/brevettiai/utils/module.py
--rw-r--r--   0        0        0      292 2024-01-23 10:01:00.289232 brevettiai-0.9.3/brevettiai/utils/numpy_json_encoder.py
--rw-r--r--   0        0        0     5823 2024-01-23 10:01:00.289232 brevettiai-0.9.3/brevettiai/utils/onnx_benchmark.py
--rw-r--r--   0        0        0     1491 2024-01-23 10:01:00.289232 brevettiai-0.9.3/brevettiai/utils/pandas_utils.py
--rw-r--r--   0        0        0      850 2024-01-23 10:01:00.289232 brevettiai-0.9.3/brevettiai/utils/polygon_utils.py
--rw-r--r--   0        0        0     1707 2024-01-23 10:01:00.289232 brevettiai-0.9.3/brevettiai/utils/profiling.py
--rw-r--r--   0        0        0      433 2024-01-23 10:01:00.289232 brevettiai-0.9.3/brevettiai/utils/singleton.py
--rw-r--r--   0        0        0     5961 2024-01-23 10:01:00.289232 brevettiai-0.9.3/brevettiai/utils/tensorboard_collector.py
--rw-r--r--   0        0        0     3914 2024-01-23 10:01:00.289232 brevettiai-0.9.3/brevettiai/utils/tf_serving_request.py
--rw-r--r--   0        0        0     4171 2024-01-23 10:01:00.289232 brevettiai-0.9.3/brevettiai/utils/upload_data.py
--rw-r--r--   0        0        0      843 2024-01-23 10:01:00.289232 brevettiai-0.9.3/brevettiai/utils/validate_args.py
--rw-r--r--   0        0        0     2400 2024-01-23 10:01:00.289232 brevettiai-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     3005 1970-01-01 00:00:00.000000 brevettiai-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-05-31 13:30:27.274028 brevettiai-0.9.4/LICENSE
+-rw-r--r--   0        0        0      678 2024-05-31 13:30:27.274028 brevettiai-0.9.4/README.md
+-rw-r--r--   0        0        0      306 2024-05-31 13:30:27.274028 brevettiai-0.9.4/brevettiai/__init__.py
+-rw-r--r--   0        0        0      156 2024-05-31 13:30:27.274028 brevettiai-0.9.4/brevettiai/data/__init__.py
+-rw-r--r--   0        0        0    21606 2024-05-31 13:30:27.274028 brevettiai-0.9.4/brevettiai/data/data_generator.py
+-rw-r--r--   0        0        0      374 2024-05-31 13:30:27.274028 brevettiai-0.9.4/brevettiai/data/image/__init__.py
+-rw-r--r--   0        0        0       86 2024-05-31 13:30:27.274028 brevettiai-0.9.4/brevettiai/data/image/annotation.py
+-rw-r--r--   0        0        0     4805 2024-05-31 13:30:27.274028 brevettiai-0.9.4/brevettiai/data/image/annotation_loader.py
+-rw-r--r--   0        0        0    10337 2024-05-31 13:30:27.274028 brevettiai-0.9.4/brevettiai/data/image/annotation_parser.py
+-rw-r--r--   0        0        0     1683 2024-05-31 13:30:27.274028 brevettiai-0.9.4/brevettiai/data/image/annotation_pooling.py
+-rw-r--r--   0        0        0      872 2024-05-31 13:30:27.274028 brevettiai-0.9.4/brevettiai/data/image/bayer_demosaic.py
+-rw-r--r--   0        0        0    14515 2024-05-31 13:30:27.274028 brevettiai-0.9.4/brevettiai/data/image/bcimg_dataset.py
+-rw-r--r--   0        0        0    26860 2024-05-31 13:30:27.274028 brevettiai-0.9.4/brevettiai/data/image/image_augmenter.py
+-rw-r--r--   0        0        0    12005 2024-05-31 13:30:27.274028 brevettiai-0.9.4/brevettiai/data/image/image_loader.py
+-rw-r--r--   0        0        0    10337 2024-05-31 13:30:27.274028 brevettiai-0.9.4/brevettiai/data/image/image_pipeline.py
+-rw-r--r--   0        0        0      877 2024-05-31 13:30:27.274028 brevettiai-0.9.4/brevettiai/data/image/image_processor.py
+-rw-r--r--   0        0        0     1271 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/data/image/image_region.py
+-rw-r--r--   0        0        0      223 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/data/image/modules.py
+-rw-r--r--   0        0        0     4612 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/data/image/multi_frame_imager.py
+-rw-r--r--   0        0        0     4254 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/data/image/segmentation_loader.py
+-rw-r--r--   0        0        0     5511 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/data/image/sequence_loader.py
+-rw-r--r--   0        0        0    15180 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/data/image/utils.py
+-rw-r--r--   0        0        0     1481 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/data/inspection_info.py
+-rw-r--r--   0        0        0    10447 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/data/sample_integrity.py
+-rw-r--r--   0        0        0     9711 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/data/sample_tools.py
+-rw-r--r--   0        0        0     1075 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/data/serialization.py
+-rw-r--r--   0        0        0     1292 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/data/tf_serialization.py
+-rw-r--r--   0        0        0     4617 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/data/tf_types.py
+-rw-r--r--   0        0        0     6422 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/data/tf_utils.py
+-rw-r--r--   0        0        0      423 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/datamodel/__init__.py
+-rw-r--r--   0        0        0      348 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/datamodel/camelmodel.py
+-rw-r--r--   0        0        0      987 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/datamodel/color.py
+-rw-r--r--   0        0        0     4092 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/datamodel/dataset.py
+-rw-r--r--   0        0        0     4884 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/datamodel/image.py
+-rw-r--r--   0        0        0     5656 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/datamodel/image_annotation.py
+-rw-r--r--   0        0        0     1140 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/datamodel/tag.py
+-rw-r--r--   0        0        0     7570 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/datamodel/web_api_types.py
+-rw-r--r--   0        0        0     3819 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/examples/explore_application.py
+-rw-r--r--   0        0        0      465 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/examples/plot_annotation.py
+-rw-r--r--   0        0        0     1439 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/examples/run_experiment.py
+-rw-r--r--   0        0        0       71 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/interfaces/__init__.py
+-rw-r--r--   0        0        0     3101 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/interfaces/aws.py
+-rw-r--r--   0        0        0     4862 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/interfaces/facets_atlas.py
+-rw-r--r--   0        0        0     2357 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/interfaces/git_state.py
+-rw-r--r--   0        0        0     2817 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/interfaces/package_validation.py
+-rw-r--r--   0        0        0     3559 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/interfaces/pivot.py
+-rw-r--r--   0        0        0     2268 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/interfaces/raygun.py
+-rw-r--r--   0        0        0     2311 2024-05-31 13:30:27.278028 brevettiai-0.9.4/brevettiai/interfaces/remote_monitor.py
+-rw-r--r--   0        0        0     1783 2024-05-31 13:30:27.290028 brevettiai-0.9.4/brevettiai/interfaces/sagemaker.py
+-rw-r--r--   0        0        0    21985 2024-05-31 13:30:27.290028 brevettiai-0.9.4/brevettiai/interfaces/vue_schema_utils.py
+-rw-r--r--   0        0        0      451 2024-05-31 13:30:27.290028 brevettiai-0.9.4/brevettiai/io/__init__.py
+-rw-r--r--   0        0        0    15551 2024-05-31 13:30:27.290028 brevettiai-0.9.4/brevettiai/io/cloudpath.py
+-rw-r--r--   0        0        0     1344 2024-05-31 13:30:27.290028 brevettiai-0.9.4/brevettiai/io/credentials.py
+-rw-r--r--   0        0        0     4160 2024-05-31 13:30:27.290028 brevettiai-0.9.4/brevettiai/io/file_cache.py
+-rw-r--r--   0        0        0     2071 2024-05-31 13:30:27.290028 brevettiai-0.9.4/brevettiai/io/files.py
+-rw-r--r--   0        0        0      743 2024-05-31 13:30:27.290028 brevettiai-0.9.4/brevettiai/io/h5_metadata.py
+-rw-r--r--   0        0        0     4677 2024-05-31 13:30:27.290028 brevettiai-0.9.4/brevettiai/io/local_io.py
+-rw-r--r--   0        0        0     8813 2024-05-31 13:30:27.290028 brevettiai-0.9.4/brevettiai/io/minio_io.py
+-rw-r--r--   0        0        0     4923 2024-05-31 13:30:27.290028 brevettiai-0.9.4/brevettiai/io/onnx.py
+-rw-r--r--   0        0        0     2325 2024-05-31 13:30:27.290028 brevettiai-0.9.4/brevettiai/io/path.py
+-rw-r--r--   0        0        0     1184 2024-05-31 13:30:27.290028 brevettiai-0.9.4/brevettiai/io/serialization.py
+-rw-r--r--   0        0        0     2790 2024-05-31 13:30:27.290028 brevettiai-0.9.4/brevettiai/io/smart_open_patch.py
+-rw-r--r--   0        0        0     3577 2024-05-31 13:30:27.290028 brevettiai-0.9.4/brevettiai/io/tf_recorder.py
+-rw-r--r--   0        0        0     1365 2024-05-31 13:30:27.290028 brevettiai-0.9.4/brevettiai/io/url_io.py
+-rw-r--r--   0        0        0     6825 2024-05-31 13:30:27.290028 brevettiai-0.9.4/brevettiai/io/utils.py
+-rw-r--r--   0        0        0        0 2024-05-31 13:30:27.290028 brevettiai-0.9.4/brevettiai/ml/__init__.py
+-rw-r--r--   0        0        0       47 2024-05-31 13:30:27.290028 brevettiai-0.9.4/brevettiai/ml/tensorflow/__init__.py
+-rw-r--r--   0        0        0     5996 2024-05-31 13:30:27.290028 brevettiai-0.9.4/brevettiai/ml/tensorflow/annotation_loader.py
+-rw-r--r--   0        0        0      111 2024-05-31 13:30:27.290028 brevettiai-0.9.4/brevettiai/model/__init__.py
+-rw-r--r--   0        0        0     2692 2024-05-31 13:30:27.290028 brevettiai-0.9.4/brevettiai/model/catalogue.py
+-rw-r--r--   0        0        0      534 2024-05-31 13:30:27.290028 brevettiai-0.9.4/brevettiai/model/factory/__init__.py
+-rw-r--r--   0        0        0     2191 2024-05-31 13:30:27.290028 brevettiai-0.9.4/brevettiai/model/factory/lenet_backbone.py
+-rw-r--r--   0        0        0     8746 2024-05-31 13:30:27.294029 brevettiai-0.9.4/brevettiai/model/factory/lraspp.py
+-rw-r--r--   0        0        0     3690 2024-05-31 13:30:27.294029 brevettiai-0.9.4/brevettiai/model/factory/mobilenetv2_backbone.py
+-rw-r--r--   0        0        0     2652 2024-05-31 13:30:27.294029 brevettiai-0.9.4/brevettiai/model/factory/segmentation.py
+-rw-r--r--   0        0        0     2510 2024-05-31 13:30:27.294029 brevettiai-0.9.4/brevettiai/model/factory/unet.py
+-rw-r--r--   0        0        0     2972 2024-05-31 13:30:27.294029 brevettiai-0.9.4/brevettiai/model/losses.py
+-rw-r--r--   0        0        0      137 2024-05-31 13:30:27.294029 brevettiai-0.9.4/brevettiai/model/metadata/__init__.py
+-rw-r--r--   0        0        0     1586 2024-05-31 13:30:27.294029 brevettiai-0.9.4/brevettiai/model/metadata/history.py
+-rw-r--r--   0        0        0     2805 2024-05-31 13:30:27.294029 brevettiai-0.9.4/brevettiai/model/metadata/image_segmentation.py
+-rw-r--r--   0        0        0      538 2024-05-31 13:30:27.294029 brevettiai-0.9.4/brevettiai/model/metadata/inference.py
+-rw-r--r--   0        0        0     2903 2024-05-31 13:30:27.294029 brevettiai-0.9.4/brevettiai/model/metadata/metadata.py
+-rw-r--r--   0        0        0      346 2024-05-31 13:30:27.294029 brevettiai-0.9.4/brevettiai/platform/__init__.py
+-rw-r--r--   0        0        0     8568 2024-05-31 13:30:27.294029 brevettiai-0.9.4/brevettiai/platform/aipackage.py
+-rw-r--r--   0        0        0     2758 2024-05-31 13:30:27.294029 brevettiai-0.9.4/brevettiai/platform/annotations.py
+-rw-r--r--   0        0        0     1274 2024-05-31 13:30:27.294029 brevettiai-0.9.4/brevettiai/platform/dataset.py
+-rw-r--r--   0        0        0     3231 2024-05-31 13:30:27.294029 brevettiai-0.9.4/brevettiai/platform/dataset_items.py
+-rw-r--r--   0        0        0     8145 2024-05-31 13:30:27.294029 brevettiai-0.9.4/brevettiai/platform/model_archive.py
+-rw-r--r--   0        0        0      368 2024-05-31 13:30:27.294029 brevettiai-0.9.4/brevettiai/platform/models/__init__.py
+-rw-r--r--   0        0        0    21202 2024-05-31 13:30:27.294029 brevettiai-0.9.4/brevettiai/platform/models/annotation.py
+-rw-r--r--   0        0        0    12476 2024-05-31 13:30:27.294029 brevettiai-0.9.4/brevettiai/platform/models/dataset.py
+-rw-r--r--   0        0        0      370 2024-05-31 13:30:27.294029 brevettiai-0.9.4/brevettiai/platform/models/iomodel.py
+-rw-r--r--   0        0        0    21112 2024-05-31 13:30:27.294029 brevettiai-0.9.4/brevettiai/platform/models/job.py
+-rw-r--r--   0        0        0     5142 2024-05-31 13:30:27.294029 brevettiai-0.9.4/brevettiai/platform/models/platform_backend.py
+-rw-r--r--   0        0        0     3720 2024-05-31 13:30:27.294029 brevettiai-0.9.4/brevettiai/platform/platform_credentials.py
+-rw-r--r--   0        0        0    28260 2024-05-31 13:30:27.294029 brevettiai-0.9.4/brevettiai/platform/web_api.py
+-rw-r--r--   0        0        0   150582 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/tests/bin/0_1543413266626.bmp
+-rw-r--r--   0        0        0     6796 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/tests/bin/1651574629796.json
+-rw-r--r--   0        0        0      249 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/tests/get_resources.py
+-rw-r--r--   0        0        0     1767 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/tests/test_aipackage.py
+-rw-r--r--   0        0        0     5092 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/tests/test_annotation_loader.py
+-rw-r--r--   0        0        0     5858 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/tests/test_annotation_tooling.py
+-rw-r--r--   0        0        0    15003 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/tests/test_data.py
+-rw-r--r--   0        0        0     5048 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/tests/test_data_image.py
+-rw-r--r--   0        0        0      882 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/tests/test_data_manipulation.py
+-rw-r--r--   0        0        0      468 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/tests/test_generate_model_name.py
+-rw-r--r--   0        0        0     3923 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/tests/test_image_loader.py
+-rw-r--r--   0        0        0     1329 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/tests/test_model_archive.py
+-rw-r--r--   0        0        0      577 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/tests/test_model_catalogue.py
+-rw-r--r--   0        0        0     1139 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/tests/test_model_loss.py
+-rw-r--r--   0        0        0     3500 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/tests/test_model_metadata.py
+-rw-r--r--   0        0        0     1574 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/tests/test_pivot.py
+-rw-r--r--   0        0        0     1249 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/tests/test_platform_annotation.py
+-rw-r--r--   0        0        0     1263 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/tests/test_platform_job.py
+-rw-r--r--   0        0        0     3732 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/tests/test_polygon_extraction.py
+-rw-r--r--   0        0        0     1795 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/tests/test_schema.py
+-rw-r--r--   0        0        0     1200 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/tests/test_tags.py
+-rw-r--r--   0        0        0      667 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/tests/test_web_api.py
+-rw-r--r--   0        0        0        0 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/tooling/__init__.py
+-rw-r--r--   0        0        0     5288 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/tooling/annotation_tools.py
+-rw-r--r--   0        0        0     7335 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/tooling/experiments.py
+-rw-r--r--   0        0        0     1633 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/tooling/plot.py
+-rw-r--r--   0        0        0       67 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/utils/__init__.py
+-rw-r--r--   0        0        0     1117 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/utils/argparse_utils.py
+-rw-r--r--   0        0        0      614 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/utils/dict_utils.py
+-rw-r--r--   0        0        0      536 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/utils/env_variables.py
+-rw-r--r--   0        0        0     2651 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/utils/model_version.py
+-rw-r--r--   0        0        0     2589 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/utils/module.py
+-rw-r--r--   0        0        0      292 2024-05-31 13:30:27.298029 brevettiai-0.9.4/brevettiai/utils/numpy_json_encoder.py
+-rw-r--r--   0        0        0     5823 2024-05-31 13:30:27.302029 brevettiai-0.9.4/brevettiai/utils/onnx_benchmark.py
+-rw-r--r--   0        0        0     1491 2024-05-31 13:30:27.302029 brevettiai-0.9.4/brevettiai/utils/pandas_utils.py
+-rw-r--r--   0        0        0      850 2024-05-31 13:30:27.302029 brevettiai-0.9.4/brevettiai/utils/polygon_utils.py
+-rw-r--r--   0        0        0     1707 2024-05-31 13:30:27.302029 brevettiai-0.9.4/brevettiai/utils/profiling.py
+-rw-r--r--   0        0        0      433 2024-05-31 13:30:27.302029 brevettiai-0.9.4/brevettiai/utils/singleton.py
+-rw-r--r--   0        0        0     5961 2024-05-31 13:30:27.302029 brevettiai-0.9.4/brevettiai/utils/tensorboard_collector.py
+-rw-r--r--   0        0        0     3914 2024-05-31 13:30:27.302029 brevettiai-0.9.4/brevettiai/utils/tf_serving_request.py
+-rw-r--r--   0        0        0     4171 2024-05-31 13:30:27.302029 brevettiai-0.9.4/brevettiai/utils/upload_data.py
+-rw-r--r--   0        0        0      843 2024-05-31 13:30:27.302029 brevettiai-0.9.4/brevettiai/utils/validate_args.py
+-rw-r--r--   0        0        0     2428 2024-05-31 13:30:27.302029 brevettiai-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     3011 1970-01-01 00:00:00.000000 brevettiai-0.9.4/PKG-INFO
```

### Comparing `brevettiai-0.9.3/LICENSE` & `brevettiai-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/README.md` & `brevettiai-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/data/data_generator.py` & `brevettiai-0.9.4/brevettiai/data/data_generator.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/data/image/annotation_loader.py` & `brevettiai-0.9.4/brevettiai/data/image/annotation_loader.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/data/image/annotation_parser.py` & `brevettiai-0.9.4/brevettiai/data/image/annotation_parser.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/data/image/annotation_pooling.py` & `brevettiai-0.9.4/brevettiai/data/image/annotation_pooling.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/data/image/bayer_demosaic.py` & `brevettiai-0.9.4/brevettiai/data/image/bayer_demosaic.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/data/image/bcimg_dataset.py` & `brevettiai-0.9.4/brevettiai/data/image/bcimg_dataset.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/data/image/image_augmenter.py` & `brevettiai-0.9.4/brevettiai/data/image/image_augmenter.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/data/image/image_loader.py` & `brevettiai-0.9.4/brevettiai/data/image/image_loader.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/data/image/image_pipeline.py` & `brevettiai-0.9.4/brevettiai/data/image/image_pipeline.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/data/image/image_processor.py` & `brevettiai-0.9.4/brevettiai/data/image/image_processor.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/data/image/image_region.py` & `brevettiai-0.9.4/brevettiai/data/image/image_region.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/data/image/multi_frame_imager.py` & `brevettiai-0.9.4/brevettiai/data/image/multi_frame_imager.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/data/image/segmentation_loader.py` & `brevettiai-0.9.4/brevettiai/data/image/segmentation_loader.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/data/image/sequence_loader.py` & `brevettiai-0.9.4/brevettiai/data/image/sequence_loader.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/data/image/utils.py` & `brevettiai-0.9.4/brevettiai/data/image/utils.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/data/inspection_info.py` & `brevettiai-0.9.4/brevettiai/data/inspection_info.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/data/sample_integrity.py` & `brevettiai-0.9.4/brevettiai/data/sample_integrity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import logging
 import json
+import logging
+
+import numpy as np
+import pandas as pd
 
 from brevettiai.interfaces import vue_schema_utils as vue
 from brevettiai.io import AnyPath
 
-import pandas as pd
-import numpy as np
-
 log = logging.getLogger(__name__)
 
 
 def merge_sample_identification(df, dfid, on="etag"):
     """
     Merge sample identification traits onto dataframe, such that values (excluding NA) are transfered to the dataframe
     :param df: Dataframe
@@ -171,18 +171,23 @@
                         marked_count = unique_items.samples[unique_items.purpose == purpose].sum()
                         assign_count = items_count * split - marked_count
                         unmarked = rng.permutation(unmarked.index)
 
                         cdf = unique_items.samples[unmarked].cumsum()
                         ix = np.searchsorted(cdf.values, assign_count, side="right")
                         if len(cdf.values) > ix:
-                            ix = ix - (rng.rand() > ((assign_count - cdf.values[ix - 1]) / (cdf.values[ix] - cdf.values[ix - 1])))
+                            if ix > 0:
+                                ix = ix - (rng.rand() > (
+                                        (assign_count - cdf.values[ix - 1]) / (cdf.values[ix] - cdf.values[ix - 1])))
+                            else:
+                                # If there is only one sample in the set assign according to split
+                                ix = -1 * (rng.rand() > split)
 
                         # Assign
-                        unique_items.loc[cdf.iloc[:ix+1].index, column] = purpose
+                        unique_items.loc[cdf.iloc[:ix + 1].index, column] = purpose
 
                 if uniqueness:
                     g.loc[:, column] = unique_items.set_index(uniqueness) \
                         .loc[g[uniqueness].set_index(uniqueness).index].purpose.values
                 else:
                     g.loc[:, column] = unique_items.purpose.values
                 return g
@@ -192,15 +197,15 @@
             else:
                 df = _split(df)
 
         if remainder:
             df.loc[df.purpose.isna(), column] = remainder
 
         # Ensure etag is unique across all stratified groups
-        #df.loc[:, column] = df.groupby("etag").first()[column].reindex(df.etag).values
+        # df.loc[:, column] = df.groupby("etag").first()[column].reindex(df.etag).values
         return df[columns]
 
     def update_unassigned(self, df, id_path,
                           purpose="train", remainder="devel", column="purpose"):
         """
         Updates sample purpose in id_path that may hold previous dataset splits and sample ids
         Unassigned samples are also assigned and id_path is updated
```

### Comparing `brevettiai-0.9.3/brevettiai/data/sample_tools.py` & `brevettiai-0.9.4/brevettiai/data/sample_tools.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/data/serialization.py` & `brevettiai-0.9.4/brevettiai/data/serialization.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/data/tf_serialization.py` & `brevettiai-0.9.4/brevettiai/data/tf_serialization.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/data/tf_types.py` & `brevettiai-0.9.4/brevettiai/data/tf_types.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/data/tf_utils.py` & `brevettiai-0.9.4/brevettiai/data/tf_utils.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/datamodel/color.py` & `brevettiai-0.9.4/brevettiai/datamodel/color.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/datamodel/dataset.py` & `brevettiai-0.9.4/brevettiai/datamodel/dataset.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/datamodel/image.py` & `brevettiai-0.9.4/brevettiai/datamodel/image.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/datamodel/image_annotation.py` & `brevettiai-0.9.4/brevettiai/datamodel/image_annotation.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/datamodel/tag.py` & `brevettiai-0.9.4/brevettiai/datamodel/tag.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/datamodel/web_api_types.py` & `brevettiai-0.9.4/brevettiai/datamodel/web_api_types.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/examples/explore_application.py` & `brevettiai-0.9.4/brevettiai/examples/explore_application.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/examples/run_experiment.py` & `brevettiai-0.9.4/brevettiai/examples/run_experiment.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/interfaces/aws.py` & `brevettiai-0.9.4/brevettiai/interfaces/aws.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/interfaces/facets_atlas.py` & `brevettiai-0.9.4/brevettiai/interfaces/facets_atlas.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/interfaces/git_state.py` & `brevettiai-0.9.4/brevettiai/interfaces/git_state.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/interfaces/pivot.py` & `brevettiai-0.9.4/brevettiai/interfaces/pivot.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/interfaces/raygun.py` & `brevettiai-0.9.4/brevettiai/interfaces/raygun.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/interfaces/remote_monitor.py` & `brevettiai-0.9.4/brevettiai/interfaces/remote_monitor.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/interfaces/sagemaker.py` & `brevettiai-0.9.4/brevettiai/interfaces/sagemaker.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/interfaces/vue_schema_utils.py` & `brevettiai-0.9.4/brevettiai/interfaces/vue_schema_utils.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/io/cloudpath.py` & `brevettiai-0.9.4/brevettiai/io/cloudpath.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/io/credentials.py` & `brevettiai-0.9.4/brevettiai/io/credentials.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/io/file_cache.py` & `brevettiai-0.9.4/brevettiai/io/file_cache.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/io/files.py` & `brevettiai-0.9.4/brevettiai/io/files.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/io/h5_metadata.py` & `brevettiai-0.9.4/brevettiai/io/h5_metadata.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/io/local_io.py` & `brevettiai-0.9.4/brevettiai/io/local_io.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/io/minio_io.py` & `brevettiai-0.9.4/brevettiai/io/minio_io.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/io/onnx.py` & `brevettiai-0.9.4/brevettiai/io/onnx.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/io/path.py` & `brevettiai-0.9.4/brevettiai/io/path.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/io/serialization.py` & `brevettiai-0.9.4/brevettiai/io/serialization.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/io/smart_open_patch.py` & `brevettiai-0.9.4/brevettiai/io/smart_open_patch.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/io/tf_recorder.py` & `brevettiai-0.9.4/brevettiai/io/tf_recorder.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/io/url_io.py` & `brevettiai-0.9.4/brevettiai/io/url_io.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/io/utils.py` & `brevettiai-0.9.4/brevettiai/io/utils.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/ml/tensorflow/annotation_loader.py` & `brevettiai-0.9.4/brevettiai/ml/tensorflow/annotation_loader.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/model/catalogue.py` & `brevettiai-0.9.4/brevettiai/model/catalogue.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/model/factory/__init__.py` & `brevettiai-0.9.4/brevettiai/model/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/model/factory/lenet_backbone.py` & `brevettiai-0.9.4/brevettiai/model/factory/lenet_backbone.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/model/factory/lraspp.py` & `brevettiai-0.9.4/brevettiai/model/factory/lraspp.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/model/factory/mobilenetv2_backbone.py` & `brevettiai-0.9.4/brevettiai/model/factory/mobilenetv2_backbone.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/model/factory/segmentation.py` & `brevettiai-0.9.4/brevettiai/model/factory/segmentation.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/model/factory/unet.py` & `brevettiai-0.9.4/brevettiai/model/factory/unet.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/model/losses.py` & `brevettiai-0.9.4/brevettiai/model/losses.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/model/metadata/history.py` & `brevettiai-0.9.4/brevettiai/model/metadata/history.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from datetime import datetime
-from pydantic import BaseModel, root_validator, Field, Extra
-from typing import Optional, List, Union, Dict, Literal
+from typing import Optional, List, Union, Dict
 from uuid import uuid4
 
+from pydantic import BaseModel, root_validator, Field, Extra
+
 from brevettiai.platform.models.job import JobOutput, Job
 
 
 class ModelHistoryItem(BaseModel):
     """Base class for model history items"""
     type: Optional[str] = Field(default=None, description="Object specifier")
     history_item_version: str = Field(default="1.0", description="Metadata version number marker")
@@ -38,7 +39,13 @@
 
 class ModelHistory(BaseModel):
     __root__: List[KnownHistoryItems] = Field(default_factory=list)
 
     def append(self, item: ModelHistoryItem):
         self.__root__.append(item)
         return self
+
+    def __getitem__(self, index):
+        return self.__root__[index]
+
+    def __len__(self):
+        return len(self.__root__)
```

### Comparing `brevettiai-0.9.3/brevettiai/model/metadata/image_segmentation.py` & `brevettiai-0.9.4/brevettiai/model/metadata/image_segmentation.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/model/metadata/inference.py` & `brevettiai-0.9.4/brevettiai/model/metadata/inference.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/model/metadata/metadata.py` & `brevettiai-0.9.4/brevettiai/model/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/platform/aipackage.py` & `brevettiai-0.9.4/brevettiai/platform/aipackage.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/platform/annotations.py` & `brevettiai-0.9.4/brevettiai/platform/annotations.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/platform/dataset.py` & `brevettiai-0.9.4/brevettiai/platform/dataset.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/platform/dataset_items.py` & `brevettiai-0.9.4/brevettiai/platform/dataset_items.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/platform/model_archive.py` & `brevettiai-0.9.4/brevettiai/platform/model_archive.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/platform/models/annotation.py` & `brevettiai-0.9.4/brevettiai/platform/models/annotation.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/platform/models/dataset.py` & `brevettiai-0.9.4/brevettiai/platform/models/dataset.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/platform/models/job.py` & `brevettiai-0.9.4/brevettiai/platform/models/job.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/platform/models/platform_backend.py` & `brevettiai-0.9.4/brevettiai/platform/models/platform_backend.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/platform/platform_credentials.py` & `brevettiai-0.9.4/brevettiai/platform/platform_credentials.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/platform/web_api.py` & `brevettiai-0.9.4/brevettiai/platform/web_api.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/tests/bin/0_1543413266626.bmp` & `brevettiai-0.9.4/brevettiai/tests/bin/0_1543413266626.bmp`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/tests/bin/1651574629796.json` & `brevettiai-0.9.4/brevettiai/tests/bin/1651574629796.json`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/tests/test_aipackage.py` & `brevettiai-0.9.4/brevettiai/tests/test_aipackage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import os
-import unittest
-import string
 import random
+import string
+import unittest
+from tempfile import TemporaryDirectory
 
-from brevettiai.tests.test_model_metadata import TestModelMetadata
 from brevettiai.platform import AIPackage
-from tempfile import TemporaryDirectory
+from brevettiai.tests.test_model_metadata import TestModelMetadata
 
 
 class TestAIPackage(unittest.TestCase):
     def test_write_archive(self):
         with TemporaryDirectory() as tmpdir:
             asset_name = "test"
             asset_content = b'test'
@@ -32,15 +32,15 @@
                 self.assertRaises(IOError, archive.open_read)
                 writer.add_asset(asset_name, "test.txt", testfile)
 
             # Check versioned name
             self.assertRegex(archive.versioned_name, r"test\.\d+\.aipkg")
 
             # Load package without password
-            self.assertRaises(IOError, AIPackage, path=testpackage)
+            self.assertRaises(OSError, AIPackage, path=testpackage)
 
             # Load package with password
             archive_out = AIPackage(path=testpackage, password=pw)
             with archive_out.open_read() as reader:
                 self.assertRaises(IOError, archive_out.open_write)
                 data = reader.get_asset(asset_name)
                 self.assertEqual(data.read(), asset_content)
```

### Comparing `brevettiai-0.9.3/brevettiai/tests/test_annotation_loader.py` & `brevettiai-0.9.4/brevettiai/tests/test_annotation_loader.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/tests/test_annotation_tooling.py` & `brevettiai-0.9.4/brevettiai/tests/test_annotation_tooling.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/tests/test_data.py` & `brevettiai-0.9.4/brevettiai/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/tests/test_data_image.py` & `brevettiai-0.9.4/brevettiai/tests/test_data_image.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/tests/test_data_manipulation.py` & `brevettiai-0.9.4/brevettiai/tests/test_data_manipulation.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/tests/test_image_loader.py` & `brevettiai-0.9.4/brevettiai/tests/test_image_loader.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/tests/test_model_archive.py` & `brevettiai-0.9.4/brevettiai/tests/test_model_archive.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/tests/test_model_catalogue.py` & `brevettiai-0.9.4/brevettiai/tests/test_model_catalogue.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/tests/test_model_loss.py` & `brevettiai-0.9.4/brevettiai/tests/test_model_loss.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/tests/test_model_metadata.py` & `brevettiai-0.9.4/brevettiai/tests/test_model_metadata.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/tests/test_pivot.py` & `brevettiai-0.9.4/brevettiai/tests/test_pivot.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/tests/test_platform_annotation.py` & `brevettiai-0.9.4/brevettiai/tests/test_platform_annotation.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/tests/test_platform_job.py` & `brevettiai-0.9.4/brevettiai/tests/test_platform_job.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/tests/test_polygon_extraction.py` & `brevettiai-0.9.4/brevettiai/tests/test_polygon_extraction.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/tests/test_schema.py` & `brevettiai-0.9.4/brevettiai/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/tests/test_tags.py` & `brevettiai-0.9.4/brevettiai/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/tests/test_web_api.py` & `brevettiai-0.9.4/brevettiai/tests/test_web_api.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/tooling/annotation_tools.py` & `brevettiai-0.9.4/brevettiai/tooling/annotation_tools.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/tooling/experiments.py` & `brevettiai-0.9.4/brevettiai/tooling/experiments.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/tooling/plot.py` & `brevettiai-0.9.4/brevettiai/tooling/plot.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/utils/argparse_utils.py` & `brevettiai-0.9.4/brevettiai/utils/argparse_utils.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/utils/dict_utils.py` & `brevettiai-0.9.4/brevettiai/utils/dict_utils.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/utils/env_variables.py` & `brevettiai-0.9.4/brevettiai/utils/env_variables.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/utils/model_version.py` & `brevettiai-0.9.4/brevettiai/utils/model_version.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/utils/module.py` & `brevettiai-0.9.4/brevettiai/utils/module.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/utils/onnx_benchmark.py` & `brevettiai-0.9.4/brevettiai/utils/onnx_benchmark.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/utils/pandas_utils.py` & `brevettiai-0.9.4/brevettiai/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/utils/polygon_utils.py` & `brevettiai-0.9.4/brevettiai/utils/polygon_utils.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/utils/profiling.py` & `brevettiai-0.9.4/brevettiai/utils/profiling.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/utils/tensorboard_collector.py` & `brevettiai-0.9.4/brevettiai/utils/tensorboard_collector.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/utils/tf_serving_request.py` & `brevettiai-0.9.4/brevettiai/utils/tf_serving_request.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/utils/upload_data.py` & `brevettiai-0.9.4/brevettiai/utils/upload_data.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/brevettiai/utils/validate_args.py` & `brevettiai-0.9.4/brevettiai/utils/validate_args.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.9.3/pyproject.toml` & `brevettiai-0.9.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brevettiai"
-version = "0.9.3"
+version = "0.9.4"
 readme = "README.md"
 homepage = "https://platform.brevetti.ai"
 documentation = "https://docs.brevetti.ai/"
 repository = "https://bitbucket.org/criterionai/core.git"
 description = "Brevetti AI library"
 license = "Apache-2.0"
 authors = ["Emil Tyge <emil@brevetti.ai>"]
@@ -36,28 +36,28 @@
 semidbm = "^0.5.1"
 
 mmh3 = ">=3.0"  # only sample integrity
 backoff = ">=1.10" # Only in io.minio
 
 tf2onnx = ">=1.9.0"  # onnx export
 onnxruntime = ">=1.6.0"  # Benchmarking
-onnxruntime-gpu = {version = ">=1.6.0", optional = true} # Benchmarking
+onnxruntime-gpu = { version = ">=1.6.0", optional = true } # Benchmarking
 h5py = "^3.6.0" # Metadata
-py7zr = ">=0.18.9" # AI package
+py7zr = ">=0.18.9,<0.21" # AI package
 
 
-tensorflow = {version = ">=2.7, !=2.9.2, <2.11", optional = true, markers="sys_platform != 'darwin'"}
-protobuf = {version = "<3.20",  optional = true}
-tensorflow-macos = {version = "^2.8", optional = true, markers="sys_platform == 'darwin'"}
-tensorflow-metal = { version = "^0.5", optional = true, markers="sys_platform == 'darwin'"}
-tensorflow_addons = {version = ">=0.16.1,<0.19", optional = true}
-tensorflow-io-gcs-filesystem = {version = "^0.31.0", optional = true}
+tensorflow = { version = ">=2.7, !=2.9.2, <2.11", optional = true, markers = "sys_platform != 'darwin'" }
+protobuf = { version = "<3.20", optional = true }
+tensorflow-macos = { version = "^2.8", optional = true, markers = "sys_platform == 'darwin'" }
+tensorflow-metal = { version = "^0.5", optional = true, markers = "sys_platform == 'darwin'" }
+tensorflow_addons = { version = ">=0.16.1,<0.19", optional = true }
+tensorflow-io-gcs-filesystem = { version = "^0.31.0", optional = true }
 
-opencv-python-headless = {version = ">=4.1", optional = true}
-opencv-python = {version = ">=4.1", optional = true}
+opencv-python-headless = { version = ">=4.1", optional = true }
+opencv-python = { version = ">=4.1", optional = true }
 oauthlib = "^3.2.2"
 requests-oauthlib = "^1.3.1"
 
 
 [tool.poetry.dev-dependencies]
 matplotlib = "*"
 coverage = "^6.2"
```

### Comparing `brevettiai-0.9.3/PKG-INFO` & `brevettiai-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brevettiai
-Version: 0.9.3
+Version: 0.9.4
 Summary: Brevetti AI library
 Home-page: https://platform.brevetti.ai
 License: Apache-2.0
 Author: Emil Tyge
 Author-email: emil@brevetti.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
@@ -31,15 +31,15 @@
 Requires-Dist: onnxruntime (>=1.6.0)
 Requires-Dist: onnxruntime-gpu (>=1.6.0) ; extra == "export-gpu"
 Requires-Dist: opencv-python (>=4.1) ; extra == "cv2"
 Requires-Dist: opencv-python-headless (>=4.1) ; extra == "cv2-headless"
 Requires-Dist: pandas (>=1.5.3)
 Requires-Dist: parse (>=1.19.0,<2.0.0)
 Requires-Dist: protobuf (<3.20) ; extra == "tf"
-Requires-Dist: py7zr (>=0.18.9)
+Requires-Dist: py7zr (>=0.18.9,<0.21)
 Requires-Dist: pydantic (>=1.9,<2.0,!=1.9.1)
 Requires-Dist: requests (>=2.23)
 Requires-Dist: requests-oauthlib (>=1.3.1,<2.0.0)
 Requires-Dist: semidbm (>=0.5.1,<0.6.0)
 Requires-Dist: shapely (>=2.0)
 Requires-Dist: smart-open (>=6.3.0,<7.0.0)
 Requires-Dist: tensorflow (>=2.7,!=2.9.2,<2.11) ; (sys_platform != "darwin") and (extra == "tf")
```

