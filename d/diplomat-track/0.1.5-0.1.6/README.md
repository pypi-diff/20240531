# Comparing `tmp/diplomat_track-0.1.5.tar.gz` & `tmp/diplomat_track-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diplomat_track-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "diplomat_track-0.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `diplomat_track-0.1.5.tar` & `diplomat_track-0.1.6.tar`

### file list

```diff
@@ -1,111 +1,112 @@
--rw-r--r--   0        0        0     6853 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/README.md
--rw-r--r--   0        0        0     2548 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/__init__.py
--rw-r--r--   0        0        0       45 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/__main__.py
--rw-r--r--   0        0        0     2456 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/_cli_runner.py
--rw-r--r--   0        0        0    23434 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/core_ops.py
--rw-r--r--   0        0        0     1432 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/frontend_ops.py
--rw-r--r--   0        0        0     7089 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/frontends/__init__.py
--rw-r--r--   0        0        0      901 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/frontends/csv/__init__.py
--rw-r--r--   0        0        0      475 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/frontends/csv/_verify_func.py
--rw-r--r--   0        0        0      938 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/frontends/csv/csv_utils.py
--rw-r--r--   0        0        0     5436 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/frontends/csv/label_videos.py
--rw-r--r--   0        0        0     3049 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/frontends/csv/tweak_results.py
--rw-r--r--   0        0        0     1464 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/frontends/deeplabcut/__init__.py
--rw-r--r--   0        0        0      980 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/frontends/deeplabcut/_verify_func.py
--rw-r--r--   0        0        0     2879 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/frontends/deeplabcut/convert_results_dlc.py
--rw-r--r--   0        0        0      679 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/frontends/deeplabcut/dlc_importer.py
--rw-r--r--   0        0        0    10254 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/frontends/deeplabcut/label_videos_dlc.py
--rw-r--r--   0        0        0    13430 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/frontends/deeplabcut/predict_frames_dlc.py
--rw-r--r--   0        0        0    19583 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/frontends/deeplabcut/predict_videos_dlc.py
--rw-r--r--   0        0        0     1806 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/frontends/deeplabcut/save_from_restore.py
--rw-r--r--   0        0        0     4185 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/frontends/deeplabcut/tweak_results.py
--rw-r--r--   0        0        0     1391 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/frontends/sleap/__init__.py
--rw-r--r--   0        0        0      458 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/frontends/sleap/_verify_func.py
--rw-r--r--   0        0        0     1704 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/frontends/sleap/convert_results_sleap.py
--rw-r--r--   0        0        0     5323 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/frontends/sleap/label_videos_sleap.py
--rw-r--r--   0        0        0     8744 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/frontends/sleap/predict_frames_sleap.py
--rw-r--r--   0        0        0     6418 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/frontends/sleap/predict_videos_sleap.py
--rw-r--r--   0        0        0     9260 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/frontends/sleap/run_utils.py
--rw-r--r--   0        0        0     1355 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/frontends/sleap/save_from_restore.py
--rw-r--r--   0        0        0      590 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/frontends/sleap/sleap_importer.py
--rw-r--r--   0        0        0    12331 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/frontends/sleap/sleap_providers.py
--rw-r--r--   0        0        0     2539 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/frontends/sleap/tweak_results_sleap.py
--rw-r--r--   0        0        0     2277 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/frontends/sleap/visual_settings.py
--rw-r--r--   0        0        0     5416 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/predictor_ops.py
--rw-r--r--   0        0        0        0 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/predictors/__init__.py
--rw-r--r--   0        0        0      699 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/predictors/argmax.py
--rw-r--r--   0        0        0    14516 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/predictors/fastplotter.py
--rw-r--r--   0        0        0        0 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/predictors/fpe/__init__.py
--rw-r--r--   0        0        0     4917 2024-04-23 15:05:56.405674 diplomat_track-0.1.5/diplomat/predictors/fpe/arr_utils.py
--rw-r--r--   0        0        0     1319 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/predictors/fpe/fpe_help.py
--rw-r--r--   0        0        0     7374 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/predictors/fpe/fpe_math.py
--rw-r--r--   0        0        0    24838 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/predictors/fpe/fpe_test_data.py
--rw-r--r--   0        0        0     4284 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/predictors/fpe/frame_pass.py
--rw-r--r--   0        0        0    23216 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/predictors/fpe/frame_pass_engine.py
--rw-r--r--   0        0        0     1530 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/predictors/fpe/frame_pass_loader.py
--rw-r--r--   0        0        0        0 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/predictors/fpe/frame_passes/__init__.py
--rw-r--r--   0        0        0    11011 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/predictors/fpe/frame_passes/cluster_frames.py
--rw-r--r--   0        0        0     9363 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/predictors/fpe/frame_passes/create_skeleton.py
--rw-r--r--   0        0        0    26266 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/predictors/fpe/frame_passes/fix_frame.py
--rw-r--r--   0        0        0    48985 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/predictors/fpe/frame_passes/mit_viterbi.py
--rw-r--r--   0        0        0     5120 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/predictors/fpe/frame_passes/optimize_std.py
--rw-r--r--   0        0        0    13500 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/predictors/fpe/skeleton_structures.py
--rw-r--r--   0        0        0    30391 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/predictors/fpe/sparse_storage.py
--rw-r--r--   0        0        0     5863 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/predictors/frame_exporter.py
--rw-r--r--   0        0        0    11920 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/predictors/plotter.py
--rw-r--r--   0        0        0        0 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/predictors/sfpe/__init__.py
--rw-r--r--   0        0        0      767 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/predictors/sfpe/assignment.py
--rw-r--r--   0        0        0    14995 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/predictors/sfpe/avl_tree.py
--rw-r--r--   0        0        0     9344 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/predictors/sfpe/disk_sparse_storage.py
--rw-r--r--   0        0        0    18778 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/predictors/sfpe/file_io.py
--rw-r--r--   0        0        0     1361 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/predictors/sfpe/growable_numpy_array.py
--rw-r--r--   0        0        0     4263 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/predictors/sfpe/segmentation.py
--rw-r--r--   0        0        0    70627 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/predictors/sfpe/segmented_frame_pass_engine.py
--rw-r--r--   0        0        0        0 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/predictors/supervised_fpe/__init__.py
--rw-r--r--   0        0        0    26301 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/predictors/supervised_fpe/labelers.py
--rw-r--r--   0        0        0     6622 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/predictors/supervised_fpe/scorers.py
--rw-r--r--   0        0        0    18822 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/predictors/supervised_fpe/supervised_frame_pass_engine.py
--rw-r--r--   0        0        0        0 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/predictors/supervised_sfpe/__init__.py
--rw-r--r--   0        0        0    28291 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/predictors/supervised_sfpe/supervised_segmented_frame_pass_engine.py
--rw-r--r--   0        0        0     2168 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/processing/__init__.py
--rw-r--r--   0        0        0     3523 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/processing/containers.py
--rw-r--r--   0        0        0    11144 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/processing/pose.py
--rw-r--r--   0        0        0    13781 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/processing/predictor.py
--rw-r--r--   0        0        0     3749 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/processing/progress_bar.py
--rw-r--r--   0        0        0    18651 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/processing/track_data.py
--rw-r--r--   0        0        0    21853 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/processing/type_casters.py
--rw-r--r--   0        0        0       96 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/utils/__init__.py
--rw-r--r--   0        0        0      360 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/utils/_bit_or.py
--rw-r--r--   0        0        0      874 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/utils/_function_tools.py
--rw-r--r--   0        0        0    11484 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/utils/cli_tools.py
--rw-r--r--   0        0        0     3153 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/utils/colormaps.py
--rw-r--r--   0        0        0    11695 2024-04-23 15:05:56.409674 diplomat_track-0.1.5/diplomat/utils/extract_frames.py
--rw-r--r--   0        0        0    10794 2024-04-23 15:05:56.413674 diplomat_track-0.1.5/diplomat/utils/frame_store_api.py
--rw-r--r--   0        0        0    28484 2024-04-23 15:05:56.413674 diplomat_track-0.1.5/diplomat/utils/frame_store_fmt.py
--rw-r--r--   0        0        0     8442 2024-04-23 15:05:56.413674 diplomat_track-0.1.5/diplomat/utils/graph_ops.py
--rw-r--r--   0        0        0     3980 2024-04-23 15:05:56.413674 diplomat_track-0.1.5/diplomat/utils/lazy_import.py
--rw-r--r--   0        0        0     4284 2024-04-23 15:05:56.413674 diplomat_track-0.1.5/diplomat/utils/pluginloader.py
--rw-r--r--   0        0        0     1690 2024-04-23 15:05:56.413674 diplomat_track-0.1.5/diplomat/utils/pretty_printer.py
--rw-r--r--   0        0        0     6965 2024-04-23 15:05:56.413674 diplomat_track-0.1.5/diplomat/utils/shapes.py
--rw-r--r--   0        0        0     2816 2024-04-23 15:05:56.413674 diplomat_track-0.1.5/diplomat/utils/track_formats.py
--rw-r--r--   0        0        0    11520 2024-04-23 15:05:56.413674 diplomat_track-0.1.5/diplomat/utils/tweak_ui.py
--rw-r--r--   0        0        0      925 2024-04-23 15:05:56.413674 diplomat_track-0.1.5/diplomat/utils/video_info.py
--rw-r--r--   0        0        0     1596 2024-04-23 15:05:56.413674 diplomat_track-0.1.5/diplomat/utils/video_io.py
--rw-r--r--   0        0        0     6823 2024-04-23 15:05:56.413674 diplomat_track-0.1.5/diplomat/utils/video_splitter.py
--rw-r--r--   0        0        0      403 2024-04-23 15:05:56.413674 diplomat_track-0.1.5/diplomat/wx_gui/__init__.py
--rw-r--r--   0        0        0    37702 2024-04-23 15:05:56.413674 diplomat_track-0.1.5/diplomat/wx_gui/fpe_editor.py
--rw-r--r--   0        0        0     4670 2024-04-23 15:05:56.413674 diplomat_track-0.1.5/diplomat/wx_gui/helpdialog.py
--rw-r--r--   0        0        0    14468 2024-04-23 15:05:56.413674 diplomat_track-0.1.5/diplomat/wx_gui/icons.py
--rw-r--r--   0        0        0    14402 2024-04-23 15:05:56.413674 diplomat_track-0.1.5/diplomat/wx_gui/id_swap_dialog.py
--rw-r--r--   0        0        0     2026 2024-04-23 15:05:56.413674 diplomat_track-0.1.5/diplomat/wx_gui/identity_swapper.py
--rw-r--r--   0        0        0    15199 2024-04-23 15:05:56.413674 diplomat_track-0.1.5/diplomat/wx_gui/labeler_lib.py
--rw-r--r--   0        0        0    46523 2024-04-23 15:05:56.413674 diplomat_track-0.1.5/diplomat/wx_gui/point_edit.py
--rw-r--r--   0        0        0    25981 2024-04-23 15:05:56.413674 diplomat_track-0.1.5/diplomat/wx_gui/probability_displayer.py
--rw-r--r--   0        0        0     7308 2024-04-23 15:05:56.413674 diplomat_track-0.1.5/diplomat/wx_gui/progress_bar.py
--rw-r--r--   0        0        0     2382 2024-04-23 15:05:56.413674 diplomat_track-0.1.5/diplomat/wx_gui/progress_dialog.py
--rw-r--r--   0        0        0     6002 2024-04-23 15:05:56.413674 diplomat_track-0.1.5/diplomat/wx_gui/score_lib.py
--rw-r--r--   0        0        0     8477 2024-04-23 15:05:56.413674 diplomat_track-0.1.5/diplomat/wx_gui/scroll_image_list.py
--rw-r--r--   0        0        0     4380 2024-04-23 15:05:56.413674 diplomat_track-0.1.5/diplomat/wx_gui/settings_dialog.py
--rw-r--r--   0        0        0    35348 2024-04-23 15:05:56.413674 diplomat_track-0.1.5/diplomat/wx_gui/video_player.py
--rw-r--r--   0        0        0     1119 2024-04-23 15:05:56.457674 diplomat_track-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     8081 1970-01-01 00:00:00.000000 diplomat_track-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     6853 2024-05-30 23:33:11.319871 diplomat_track-0.1.6/README.md
+-rw-r--r--   0        0        0     2548 2024-05-30 23:33:11.319871 diplomat_track-0.1.6/diplomat/__init__.py
+-rw-r--r--   0        0        0       45 2024-05-30 23:33:11.319871 diplomat_track-0.1.6/diplomat/__main__.py
+-rw-r--r--   0        0        0     2456 2024-05-30 23:33:11.319871 diplomat_track-0.1.6/diplomat/_cli_runner.py
+-rw-r--r--   0        0        0    23434 2024-05-30 23:33:11.319871 diplomat_track-0.1.6/diplomat/core_ops.py
+-rw-r--r--   0        0        0     1432 2024-05-30 23:33:11.319871 diplomat_track-0.1.6/diplomat/frontend_ops.py
+-rw-r--r--   0        0        0     7089 2024-05-30 23:33:11.319871 diplomat_track-0.1.6/diplomat/frontends/__init__.py
+-rw-r--r--   0        0        0      901 2024-05-30 23:33:11.319871 diplomat_track-0.1.6/diplomat/frontends/csv/__init__.py
+-rw-r--r--   0        0        0      475 2024-05-30 23:33:11.319871 diplomat_track-0.1.6/diplomat/frontends/csv/_verify_func.py
+-rw-r--r--   0        0        0      938 2024-05-30 23:33:11.319871 diplomat_track-0.1.6/diplomat/frontends/csv/csv_utils.py
+-rw-r--r--   0        0        0     5436 2024-05-30 23:33:11.319871 diplomat_track-0.1.6/diplomat/frontends/csv/label_videos.py
+-rw-r--r--   0        0        0     3049 2024-05-30 23:33:11.319871 diplomat_track-0.1.6/diplomat/frontends/csv/tweak_results.py
+-rw-r--r--   0        0        0     1464 2024-05-30 23:33:11.319871 diplomat_track-0.1.6/diplomat/frontends/deeplabcut/__init__.py
+-rw-r--r--   0        0        0      980 2024-05-30 23:33:11.319871 diplomat_track-0.1.6/diplomat/frontends/deeplabcut/_verify_func.py
+-rw-r--r--   0        0        0     2879 2024-05-30 23:33:11.319871 diplomat_track-0.1.6/diplomat/frontends/deeplabcut/convert_results_dlc.py
+-rw-r--r--   0        0        0      679 2024-05-30 23:33:11.319871 diplomat_track-0.1.6/diplomat/frontends/deeplabcut/dlc_importer.py
+-rw-r--r--   0        0        0    10254 2024-05-30 23:33:11.319871 diplomat_track-0.1.6/diplomat/frontends/deeplabcut/label_videos_dlc.py
+-rw-r--r--   0        0        0    13430 2024-05-30 23:33:11.319871 diplomat_track-0.1.6/diplomat/frontends/deeplabcut/predict_frames_dlc.py
+-rw-r--r--   0        0        0    19583 2024-05-30 23:33:11.319871 diplomat_track-0.1.6/diplomat/frontends/deeplabcut/predict_videos_dlc.py
+-rw-r--r--   0        0        0     1806 2024-05-30 23:33:11.319871 diplomat_track-0.1.6/diplomat/frontends/deeplabcut/save_from_restore.py
+-rw-r--r--   0        0        0     4185 2024-05-30 23:33:11.319871 diplomat_track-0.1.6/diplomat/frontends/deeplabcut/tweak_results.py
+-rw-r--r--   0        0        0     1391 2024-05-30 23:33:11.319871 diplomat_track-0.1.6/diplomat/frontends/sleap/__init__.py
+-rw-r--r--   0        0        0      458 2024-05-30 23:33:11.319871 diplomat_track-0.1.6/diplomat/frontends/sleap/_verify_func.py
+-rw-r--r--   0        0        0     1704 2024-05-30 23:33:11.319871 diplomat_track-0.1.6/diplomat/frontends/sleap/convert_results_sleap.py
+-rw-r--r--   0        0        0     5323 2024-05-30 23:33:11.319871 diplomat_track-0.1.6/diplomat/frontends/sleap/label_videos_sleap.py
+-rw-r--r--   0        0        0     8744 2024-05-30 23:33:11.319871 diplomat_track-0.1.6/diplomat/frontends/sleap/predict_frames_sleap.py
+-rw-r--r--   0        0        0     6418 2024-05-30 23:33:11.319871 diplomat_track-0.1.6/diplomat/frontends/sleap/predict_videos_sleap.py
+-rw-r--r--   0        0        0     9260 2024-05-30 23:33:11.319871 diplomat_track-0.1.6/diplomat/frontends/sleap/run_utils.py
+-rw-r--r--   0        0        0     1355 2024-05-30 23:33:11.319871 diplomat_track-0.1.6/diplomat/frontends/sleap/save_from_restore.py
+-rw-r--r--   0        0        0      590 2024-05-30 23:33:11.319871 diplomat_track-0.1.6/diplomat/frontends/sleap/sleap_importer.py
+-rw-r--r--   0        0        0    12331 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/frontends/sleap/sleap_providers.py
+-rw-r--r--   0        0        0     2539 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/frontends/sleap/tweak_results_sleap.py
+-rw-r--r--   0        0        0     2277 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/frontends/sleap/visual_settings.py
+-rw-r--r--   0        0        0     5416 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictor_ops.py
+-rw-r--r--   0        0        0        0 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/__init__.py
+-rw-r--r--   0        0        0      699 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/argmax.py
+-rw-r--r--   0        0        0    14516 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/fastplotter.py
+-rw-r--r--   0        0        0        0 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/fpe/__init__.py
+-rw-r--r--   0        0        0     4917 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/fpe/arr_utils.py
+-rw-r--r--   0        0        0     1319 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/fpe/fpe_help.py
+-rw-r--r--   0        0        0     7374 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/fpe/fpe_math.py
+-rw-r--r--   0        0        0    24838 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/fpe/fpe_test_data.py
+-rw-r--r--   0        0        0     4284 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/fpe/frame_pass.py
+-rw-r--r--   0        0        0    23216 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/fpe/frame_pass_engine.py
+-rw-r--r--   0        0        0     1530 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/fpe/frame_pass_loader.py
+-rw-r--r--   0        0        0        0 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/fpe/frame_passes/__init__.py
+-rw-r--r--   0        0        0    11011 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/fpe/frame_passes/cluster_frames.py
+-rw-r--r--   0        0        0     9363 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/fpe/frame_passes/create_skeleton.py
+-rw-r--r--   0        0        0    26334 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/fpe/frame_passes/fix_frame.py
+-rw-r--r--   0        0        0    48985 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/fpe/frame_passes/mit_viterbi.py
+-rw-r--r--   0        0        0     5120 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/fpe/frame_passes/optimize_std.py
+-rw-r--r--   0        0        0    13500 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/fpe/skeleton_structures.py
+-rw-r--r--   0        0        0    30391 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/fpe/sparse_storage.py
+-rw-r--r--   0        0        0     5863 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/frame_exporter.py
+-rw-r--r--   0        0        0    11920 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/plotter.py
+-rw-r--r--   0        0        0        0 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/sfpe/__init__.py
+-rw-r--r--   0        0        0      767 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/sfpe/assignment.py
+-rw-r--r--   0        0        0    14995 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/sfpe/avl_tree.py
+-rw-r--r--   0        0        0     9344 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/sfpe/disk_sparse_storage.py
+-rw-r--r--   0        0        0    18778 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/sfpe/file_io.py
+-rw-r--r--   0        0        0     1361 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/sfpe/growable_numpy_array.py
+-rw-r--r--   0        0        0     4263 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/sfpe/segmentation.py
+-rw-r--r--   0        0        0    70627 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/sfpe/segmented_frame_pass_engine.py
+-rw-r--r--   0        0        0        0 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/supervised_fpe/__init__.py
+-rw-r--r--   0        0        0    26301 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/supervised_fpe/labelers.py
+-rw-r--r--   0        0        0     6622 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/supervised_fpe/scorers.py
+-rw-r--r--   0        0        0    18822 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/supervised_fpe/supervised_frame_pass_engine.py
+-rw-r--r--   0        0        0        0 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/supervised_sfpe/__init__.py
+-rw-r--r--   0        0        0    28291 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/predictors/supervised_sfpe/supervised_segmented_frame_pass_engine.py
+-rw-r--r--   0        0        0     2168 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/processing/__init__.py
+-rw-r--r--   0        0        0     3523 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/processing/containers.py
+-rw-r--r--   0        0        0    11144 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/processing/pose.py
+-rw-r--r--   0        0        0    13781 2024-05-30 23:33:11.323871 diplomat_track-0.1.6/diplomat/processing/predictor.py
+-rw-r--r--   0        0        0     3749 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/processing/progress_bar.py
+-rw-r--r--   0        0        0    18651 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/processing/track_data.py
+-rw-r--r--   0        0        0    21853 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/processing/type_casters.py
+-rw-r--r--   0        0        0       96 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/utils/__init__.py
+-rw-r--r--   0        0        0      360 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/utils/_bit_or.py
+-rw-r--r--   0        0        0      874 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/utils/_function_tools.py
+-rw-r--r--   0        0        0    11484 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/utils/cli_tools.py
+-rw-r--r--   0        0        0     3153 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/utils/colormaps.py
+-rw-r--r--   0        0        0    11695 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/utils/extract_frames.py
+-rw-r--r--   0        0        0    10794 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/utils/frame_store_api.py
+-rw-r--r--   0        0        0    28484 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/utils/frame_store_fmt.py
+-rw-r--r--   0        0        0     8721 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/utils/graph_ops.py
+-rw-r--r--   0        0        0     3980 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/utils/lazy_import.py
+-rw-r--r--   0        0        0     4284 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/utils/pluginloader.py
+-rw-r--r--   0        0        0     1690 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/utils/pretty_printer.py
+-rw-r--r--   0        0        0     9598 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/utils/scipy_hungarian.py
+-rw-r--r--   0        0        0     6965 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/utils/shapes.py
+-rw-r--r--   0        0        0     2816 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/utils/track_formats.py
+-rw-r--r--   0        0        0    11520 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/utils/tweak_ui.py
+-rw-r--r--   0        0        0      925 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/utils/video_info.py
+-rw-r--r--   0        0        0     1596 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/utils/video_io.py
+-rw-r--r--   0        0        0     6823 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/utils/video_splitter.py
+-rw-r--r--   0        0        0      403 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/wx_gui/__init__.py
+-rw-r--r--   0        0        0    37702 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/wx_gui/fpe_editor.py
+-rw-r--r--   0        0        0     4670 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/wx_gui/helpdialog.py
+-rw-r--r--   0        0        0    14468 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/wx_gui/icons.py
+-rw-r--r--   0        0        0    14402 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/wx_gui/id_swap_dialog.py
+-rw-r--r--   0        0        0     2026 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/wx_gui/identity_swapper.py
+-rw-r--r--   0        0        0    15199 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/wx_gui/labeler_lib.py
+-rw-r--r--   0        0        0    46523 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/wx_gui/point_edit.py
+-rw-r--r--   0        0        0    25981 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/wx_gui/probability_displayer.py
+-rw-r--r--   0        0        0     7308 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/wx_gui/progress_bar.py
+-rw-r--r--   0        0        0     2382 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/wx_gui/progress_dialog.py
+-rw-r--r--   0        0        0     6002 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/wx_gui/score_lib.py
+-rw-r--r--   0        0        0     8477 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/wx_gui/scroll_image_list.py
+-rw-r--r--   0        0        0     4380 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/wx_gui/settings_dialog.py
+-rw-r--r--   0        0        0    35348 2024-05-30 23:33:11.327870 diplomat_track-0.1.6/diplomat/wx_gui/video_player.py
+-rw-r--r--   0        0        0     1119 2024-05-30 23:33:11.371868 diplomat_track-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     8081 1970-01-01 00:00:00.000000 diplomat_track-0.1.6/PKG-INFO
```

### Comparing `diplomat_track-0.1.5/README.md` & `diplomat_track-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/__init__.py` & `diplomat_track-0.1.6/diplomat/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 A tool providing multi-animal tracking capabilities on top of other Deep learning based tracking software.
 """
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 # Can be used by functions to determine if diplomat was invoked through it's CLI interface.
 CLI_RUN = False
 
 from diplomat.predictor_ops import list_predictor_plugins, get_predictor_settings, test_predictor_plugin
 from diplomat.frontend_ops import list_all_frontends, list_loaded_frontends
 from diplomat.utils.video_splitter import split_videos
 from diplomat.core_ops import track_with, track, track_and_interact, annotate, tweak, yaml, convert, interact
```

### Comparing `diplomat_track-0.1.5/diplomat/_cli_runner.py` & `diplomat_track-0.1.6/diplomat/_cli_runner.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/core_ops.py` & `diplomat_track-0.1.6/diplomat/core_ops.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/frontend_ops.py` & `diplomat_track-0.1.6/diplomat/frontend_ops.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/frontends/__init__.py` & `diplomat_track-0.1.6/diplomat/frontends/__init__.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/frontends/csv/__init__.py` & `diplomat_track-0.1.6/diplomat/frontends/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/frontends/csv/csv_utils.py` & `diplomat_track-0.1.6/diplomat/frontends/csv/csv_utils.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/frontends/csv/label_videos.py` & `diplomat_track-0.1.6/diplomat/frontends/csv/label_videos.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/frontends/csv/tweak_results.py` & `diplomat_track-0.1.6/diplomat/frontends/csv/tweak_results.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/frontends/deeplabcut/__init__.py` & `diplomat_track-0.1.6/diplomat/frontends/deeplabcut/__init__.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/frontends/deeplabcut/_verify_func.py` & `diplomat_track-0.1.6/diplomat/frontends/deeplabcut/_verify_func.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/frontends/deeplabcut/convert_results_dlc.py` & `diplomat_track-0.1.6/diplomat/frontends/deeplabcut/convert_results_dlc.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/frontends/deeplabcut/dlc_importer.py` & `diplomat_track-0.1.6/diplomat/frontends/deeplabcut/dlc_importer.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/frontends/deeplabcut/label_videos_dlc.py` & `diplomat_track-0.1.6/diplomat/frontends/deeplabcut/label_videos_dlc.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/frontends/deeplabcut/predict_frames_dlc.py` & `diplomat_track-0.1.6/diplomat/frontends/deeplabcut/predict_frames_dlc.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/frontends/deeplabcut/predict_videos_dlc.py` & `diplomat_track-0.1.6/diplomat/frontends/deeplabcut/predict_videos_dlc.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/frontends/deeplabcut/save_from_restore.py` & `diplomat_track-0.1.6/diplomat/frontends/deeplabcut/save_from_restore.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/frontends/deeplabcut/tweak_results.py` & `diplomat_track-0.1.6/diplomat/frontends/deeplabcut/tweak_results.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/frontends/sleap/__init__.py` & `diplomat_track-0.1.6/diplomat/frontends/sleap/__init__.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/frontends/sleap/convert_results_sleap.py` & `diplomat_track-0.1.6/diplomat/frontends/sleap/convert_results_sleap.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/frontends/sleap/label_videos_sleap.py` & `diplomat_track-0.1.6/diplomat/frontends/sleap/label_videos_sleap.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/frontends/sleap/predict_frames_sleap.py` & `diplomat_track-0.1.6/diplomat/frontends/sleap/predict_frames_sleap.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/frontends/sleap/predict_videos_sleap.py` & `diplomat_track-0.1.6/diplomat/frontends/sleap/predict_videos_sleap.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/frontends/sleap/run_utils.py` & `diplomat_track-0.1.6/diplomat/frontends/sleap/run_utils.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/frontends/sleap/save_from_restore.py` & `diplomat_track-0.1.6/diplomat/frontends/sleap/save_from_restore.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/frontends/sleap/sleap_importer.py` & `diplomat_track-0.1.6/diplomat/frontends/sleap/sleap_importer.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/frontends/sleap/sleap_providers.py` & `diplomat_track-0.1.6/diplomat/frontends/sleap/sleap_providers.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/frontends/sleap/tweak_results_sleap.py` & `diplomat_track-0.1.6/diplomat/frontends/sleap/tweak_results_sleap.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/frontends/sleap/visual_settings.py` & `diplomat_track-0.1.6/diplomat/frontends/sleap/visual_settings.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/predictor_ops.py` & `diplomat_track-0.1.6/diplomat/predictor_ops.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/predictors/argmax.py` & `diplomat_track-0.1.6/diplomat/predictors/argmax.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/predictors/fastplotter.py` & `diplomat_track-0.1.6/diplomat/predictors/fastplotter.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/predictors/fpe/arr_utils.py` & `diplomat_track-0.1.6/diplomat/predictors/fpe/arr_utils.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/predictors/fpe/fpe_help.py` & `diplomat_track-0.1.6/diplomat/predictors/fpe/fpe_help.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/predictors/fpe/fpe_math.py` & `diplomat_track-0.1.6/diplomat/predictors/fpe/fpe_math.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/predictors/fpe/fpe_test_data.py` & `diplomat_track-0.1.6/diplomat/predictors/fpe/fpe_test_data.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/predictors/fpe/frame_pass.py` & `diplomat_track-0.1.6/diplomat/predictors/fpe/frame_pass.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/predictors/fpe/frame_pass_engine.py` & `diplomat_track-0.1.6/diplomat/predictors/fpe/frame_pass_engine.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/predictors/fpe/frame_pass_loader.py` & `diplomat_track-0.1.6/diplomat/predictors/fpe/frame_pass_loader.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/predictors/fpe/frame_passes/cluster_frames.py` & `diplomat_track-0.1.6/diplomat/predictors/fpe/frame_passes/cluster_frames.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/predictors/fpe/frame_passes/create_skeleton.py` & `diplomat_track-0.1.6/diplomat/predictors/fpe/frame_passes/create_skeleton.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/predictors/fpe/frame_passes/fix_frame.py` & `diplomat_track-0.1.6/diplomat/predictors/fpe/frame_passes/fix_frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,14 +234,15 @@
     def create_fix_frame(
         cls,
         fb_data: ForwardBackwardData,
         frame_idx: int,
         skeleton: Optional[StorageGraph],
         algorithm: str = "greedy"
     ) -> List[ForwardBackwardFrame]:
+        #print(f"FixFrame.create_fix_frame.algorithm:={algorithm}")
         if(algorithm not in ("greedy", "hungarian")):
             raise ValueError("Algorithm passed not a support algorithm, use greedy or hungarian.")
 
         fixed_frame = [None] * fb_data.num_bodyparts
         num_outputs = fb_data.metadata.num_outputs
         down_scaling = fb_data.metadata.down_scaling
```

### Comparing `diplomat_track-0.1.5/diplomat/predictors/fpe/frame_passes/mit_viterbi.py` & `diplomat_track-0.1.6/diplomat/predictors/fpe/frame_passes/mit_viterbi.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/predictors/fpe/frame_passes/optimize_std.py` & `diplomat_track-0.1.6/diplomat/predictors/fpe/frame_passes/optimize_std.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/predictors/fpe/skeleton_structures.py` & `diplomat_track-0.1.6/diplomat/predictors/fpe/skeleton_structures.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/predictors/fpe/sparse_storage.py` & `diplomat_track-0.1.6/diplomat/predictors/fpe/sparse_storage.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/predictors/frame_exporter.py` & `diplomat_track-0.1.6/diplomat/predictors/frame_exporter.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/predictors/plotter.py` & `diplomat_track-0.1.6/diplomat/predictors/plotter.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/predictors/sfpe/assignment.py` & `diplomat_track-0.1.6/diplomat/predictors/sfpe/assignment.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/predictors/sfpe/avl_tree.py` & `diplomat_track-0.1.6/diplomat/predictors/sfpe/avl_tree.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/predictors/sfpe/disk_sparse_storage.py` & `diplomat_track-0.1.6/diplomat/predictors/sfpe/disk_sparse_storage.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/predictors/sfpe/file_io.py` & `diplomat_track-0.1.6/diplomat/predictors/sfpe/file_io.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/predictors/sfpe/growable_numpy_array.py` & `diplomat_track-0.1.6/diplomat/predictors/sfpe/growable_numpy_array.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/predictors/sfpe/segmentation.py` & `diplomat_track-0.1.6/diplomat/predictors/sfpe/segmentation.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/predictors/sfpe/segmented_frame_pass_engine.py` & `diplomat_track-0.1.6/diplomat/predictors/sfpe/segmented_frame_pass_engine.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/predictors/supervised_fpe/labelers.py` & `diplomat_track-0.1.6/diplomat/predictors/supervised_fpe/labelers.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/predictors/supervised_fpe/scorers.py` & `diplomat_track-0.1.6/diplomat/predictors/supervised_fpe/scorers.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/predictors/supervised_fpe/supervised_frame_pass_engine.py` & `diplomat_track-0.1.6/diplomat/predictors/supervised_fpe/supervised_frame_pass_engine.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/predictors/supervised_sfpe/supervised_segmented_frame_pass_engine.py` & `diplomat_track-0.1.6/diplomat/predictors/supervised_sfpe/supervised_segmented_frame_pass_engine.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/processing/__init__.py` & `diplomat_track-0.1.6/diplomat/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/processing/containers.py` & `diplomat_track-0.1.6/diplomat/processing/containers.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/processing/pose.py` & `diplomat_track-0.1.6/diplomat/processing/pose.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/processing/predictor.py` & `diplomat_track-0.1.6/diplomat/processing/predictor.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/processing/progress_bar.py` & `diplomat_track-0.1.6/diplomat/processing/progress_bar.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/processing/track_data.py` & `diplomat_track-0.1.6/diplomat/processing/track_data.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/processing/type_casters.py` & `diplomat_track-0.1.6/diplomat/processing/type_casters.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/utils/_function_tools.py` & `diplomat_track-0.1.6/diplomat/utils/_function_tools.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/utils/cli_tools.py` & `diplomat_track-0.1.6/diplomat/utils/cli_tools.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/utils/colormaps.py` & `diplomat_track-0.1.6/diplomat/utils/colormaps.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/utils/extract_frames.py` & `diplomat_track-0.1.6/diplomat/utils/extract_frames.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/utils/frame_store_api.py` & `diplomat_track-0.1.6/diplomat/utils/frame_store_api.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/utils/frame_store_fmt.py` & `diplomat_track-0.1.6/diplomat/utils/frame_store_fmt.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/utils/graph_ops.py` & `diplomat_track-0.1.6/diplomat/utils/graph_ops.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numba
 import numpy as np
 from typing import Tuple
 
+from .scipy_hungarian import linear_sum_assignment
 
 @numba.experimental.jitclass([
     ["_stack_ptr", numba.int64],
     ["_stack", numba.int64[:]]
 ])
 class Stack:
     def __init__(self, max_size: int):
@@ -122,26 +123,32 @@
             min_row_val = g[i, j] if(g[i, j] < min_row_val) else min_row_val
 
         for j in range(g.shape[1]):
             g[i, j] -= min_row_val
 
     return g
 
+def min_cost_matching(cost_matrix: np.ndarray, mode="scipy") -> Tuple[np.ndarray, np.ndarray]:
+    if mode == "scipy":
+        return linear_sum_assignment(cost_matrix)
+    else:
+        return _min_cost_matching(cost_matrix)
 
 @numba.njit
-def min_cost_matching(cost_matrix: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
+def _min_cost_matching(cost_matrix: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
     """
     Implementation of the hungarian algorithm for solving the minimum assignment problem. Given a cost matrix,
     find the optimal assignment of workers (rows) to jobs (columns). Algorithm is O(N^3).
 
     :param cost_matrix: The cost matrix to find an optimal matching for.
 
     :returns: A tuple of 2 numpy arrays, first representing row assignments (row -> column) and second column
               assignments (column -> row). Note, these are inversions of each other.
     """
+
     graph_copy = cost_matrix.copy()
 
     while(True):
         # Subtract current minimum row/column values to get current greedy solution...
         graph_copy = _min_row_subtract(graph_copy)
         graph_copy = _min_row_subtract(graph_copy.T).T
```

### Comparing `diplomat_track-0.1.5/diplomat/utils/lazy_import.py` & `diplomat_track-0.1.6/diplomat/utils/lazy_import.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/utils/pluginloader.py` & `diplomat_track-0.1.6/diplomat/utils/pluginloader.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/utils/pretty_printer.py` & `diplomat_track-0.1.6/diplomat/utils/pretty_printer.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/utils/shapes.py` & `diplomat_track-0.1.6/diplomat/utils/shapes.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/utils/track_formats.py` & `diplomat_track-0.1.6/diplomat/utils/track_formats.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/utils/tweak_ui.py` & `diplomat_track-0.1.6/diplomat/utils/tweak_ui.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/utils/video_info.py` & `diplomat_track-0.1.6/diplomat/utils/video_info.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/utils/video_io.py` & `diplomat_track-0.1.6/diplomat/utils/video_io.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/utils/video_splitter.py` & `diplomat_track-0.1.6/diplomat/utils/video_splitter.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/wx_gui/fpe_editor.py` & `diplomat_track-0.1.6/diplomat/wx_gui/fpe_editor.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/wx_gui/helpdialog.py` & `diplomat_track-0.1.6/diplomat/wx_gui/helpdialog.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/wx_gui/icons.py` & `diplomat_track-0.1.6/diplomat/wx_gui/icons.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/wx_gui/id_swap_dialog.py` & `diplomat_track-0.1.6/diplomat/wx_gui/id_swap_dialog.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/wx_gui/identity_swapper.py` & `diplomat_track-0.1.6/diplomat/wx_gui/identity_swapper.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/wx_gui/labeler_lib.py` & `diplomat_track-0.1.6/diplomat/wx_gui/labeler_lib.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/wx_gui/point_edit.py` & `diplomat_track-0.1.6/diplomat/wx_gui/point_edit.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/wx_gui/probability_displayer.py` & `diplomat_track-0.1.6/diplomat/wx_gui/probability_displayer.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/wx_gui/progress_bar.py` & `diplomat_track-0.1.6/diplomat/wx_gui/progress_bar.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/wx_gui/progress_dialog.py` & `diplomat_track-0.1.6/diplomat/wx_gui/progress_dialog.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/wx_gui/score_lib.py` & `diplomat_track-0.1.6/diplomat/wx_gui/score_lib.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/wx_gui/scroll_image_list.py` & `diplomat_track-0.1.6/diplomat/wx_gui/scroll_image_list.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/wx_gui/settings_dialog.py` & `diplomat_track-0.1.6/diplomat/wx_gui/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/diplomat/wx_gui/video_player.py` & `diplomat_track-0.1.6/diplomat/wx_gui/video_player.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/pyproject.toml` & `diplomat_track-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.5/PKG-INFO` & `diplomat_track-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diplomat-track
-Version: 0.1.5
+Version: 0.1.6
 Summary: A tool providing multi-animal tracking capabilities on top of other Deep learning based tracking software.
 Author-email: Isaac Robinson <isaac.k.robinson2000@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

