# Comparing `tmp/todd_ai-0.4.0.tar.gz` & `tmp/todd_ai-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "todd_ai-0.4.0.tar", last modified: Wed Jul 26 04:28:57 2023, max compression
+gzip compressed data, was "todd_ai-0.5.0.tar", last modified: Fri May 31 15:40:50 2024, max compression
```

## Comparing `todd_ai-0.4.0.tar` & `todd_ai-0.5.0.tar`

### file list

```diff
@@ -1,112 +1,221 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.535079 todd_ai-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-26 04:28:48.000000 todd_ai-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15017 2023-07-26 04:28:57.535079 todd_ai-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-26 04:28:48.000000 todd_ai-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.523079 todd_ai-0.4.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      540 2023-07-26 04:28:48.000000 todd_ai-0.4.0/bin/git_rev_parse_head
--rwxr-xr-x   0 runner    (1001) docker     (123)      344 2023-07-26 04:28:48.000000 todd_ai-0.4.0/bin/git_status_porcelain
--rwxr-xr-x   0 runner    (1001) docker     (123)      627 2023-07-26 04:28:48.000000 todd_ai-0.4.0/bin/odpsrun
--rwxr-xr-x   0 runner    (1001) docker     (123)     1690 2023-07-26 04:28:48.000000 todd_ai-0.4.0/bin/odpsrun.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-07-26 04:28:48.000000 todd_ai-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 04:28:57.535079 todd_ai-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-26 04:28:48.000000 todd_ai-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.523079 todd_ai-0.4.0/todd/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.523079 todd_ai-0.4.0/todd/adapts/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/adapts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/adapts/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/adapts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/adapts/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/adapts/decouple.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/adapts/detach.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/adapts/dict_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/adapts/iou.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/adapts/label_enc.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/adapts/list_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/adapts/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/adapts/null.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/adapts/roi_align.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.527079 todd_ai-0.4.0/todd/base/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/base/bboxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/base/checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/base/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/base/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/base/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/base/registries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/base/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/base/stores.py
--rw-r--r--   0 runner    (1001) docker     (123)    10904 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/base/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.527079 todd_ai-0.4.0/todd/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/datasets/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/datasets/lmdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/datasets/pth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/datasets/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.527079 todd_ai-0.4.0/todd/distillers/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/distillers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/distillers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/distillers/single_student.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.527079 todd_ai-0.4.0/todd/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/hooks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/hooks/duplicated.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/hooks/multi_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/hooks/standard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.527079 todd_ai-0.4.0/todd/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/losses/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/losses/ckd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/losses/focal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/losses/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/losses/mimic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/losses/rcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/losses/schedulers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.527079 todd_ai-0.4.0/todd/reproduction/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/reproduction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13357 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/reproduction/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/reproduction/seed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.527079 todd_ai-0.4.0/todd/runners/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.531079 todd_ai-0.4.0/todd/runners/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/callbacks/autocast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/callbacks/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/callbacks/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/callbacks/composed.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/callbacks/interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/callbacks/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/callbacks/lr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/callbacks/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/callbacks/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/runners.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.531079 todd_ai-0.4.0/todd/runners/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/strategies/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/strategies/ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/runners/strategies/fsdp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.531079 todd_ai-0.4.0/todd/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/scripts/convert_ckpts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/scripts/convert_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/scripts/merge_lmdbs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.531079 todd_ai-0.4.0/todd/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/utils/generic_tensors.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/utils/metas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/utils/sgr.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/utils/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/utils/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.531079 todd_ai-0.4.0/todd/visuals/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/visuals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/visuals/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/visuals/cv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-07-26 04:28:48.000000 todd_ai-0.4.0/todd/visuals/pptx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:28:57.535079 todd_ai-0.4.0/todd_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15017 2023-07-26 04:28:57.000000 todd_ai-0.4.0/todd_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-26 04:28:57.000000 todd_ai-0.4.0/todd_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 04:28:57.000000 todd_ai-0.4.0/todd_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-26 04:28:57.000000 todd_ai-0.4.0/todd_ai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-26 04:28:57.000000 todd_ai-0.4.0/todd_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-26 04:28:57.000000 todd_ai-0.4.0/todd_ai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.581437 todd_ai-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-31 15:40:46.000000 todd_ai-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16859 2024-05-31 15:40:50.577437 todd_ai-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-31 15:40:46.000000 todd_ai-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.549437 todd_ai-0.5.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2173 2024-05-31 15:40:46.000000 todd_ai-0.5.0/bin/odpsrun
+-rw-r--r--   0 runner    (1001) docker     (127)     4920 2024-05-31 15:40:46.000000 todd_ai-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:40:50.581437 todd_ai-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-31 15:40:46.000000 todd_ai-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.549437 todd_ai-0.5.0/todd/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.553437 todd_ai-0.5.0/todd/colors/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/colors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/colors/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/colors/color_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/colors/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/colors/palette.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/colors/rgba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/colors/yiq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.553437 todd_ai-0.5.0/todd/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/configs/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/configs/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/configs/py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/configs/serializable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.553437 todd_ai-0.5.0/todd/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.553437 todd_ai-0.5.0/todd/datasets/access_layers/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/datasets/access_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/datasets/access_layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/datasets/access_layers/concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/datasets/access_layers/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/datasets/access_layers/pth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/datasets/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/datasets/lmdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/datasets/registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/datasets/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.553437 todd_ai-0.5.0/todd/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/loggers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.553437 todd_ai-0.5.0/todd/loggers/control_sequences/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/loggers/control_sequences/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/loggers/control_sequences/control_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/loggers/control_sequences/sgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/loggers/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/loggers/master.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.557437 todd_ai-0.5.0/todd/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.557437 todd_ai-0.5.0/todd/models/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/models/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/models/filters/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/models/filters/named_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/models/filters/named_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/models/filters/named_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13151 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/models/frozens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.557437 todd_ai-0.5.0/todd/models/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/models/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/models/losses/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/models/losses/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/models/losses/registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/models/losses/schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/models/mean_std.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/models/registries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.557437 todd_ai-0.5.0/todd/models/shadows/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/models/shadows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/models/shadows/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/models/shadows/ema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/models/shapes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.557437 todd_ai-0.5.0/todd/patches/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/patches/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.557437 todd_ai-0.5.0/todd/patches/cv2/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/patches/cv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/patches/cv2/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/patches/cv2/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.561437 todd_ai-0.5.0/todd/patches/py/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/patches/py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/patches/py/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/patches/py/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/patches/py/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/patches/py/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/patches/py/subprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.561437 todd_ai-0.5.0/todd/patches/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/patches/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/patches/torch/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/patches/torch/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/patches/torch/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/patches/torch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.561437 todd_ai-0.5.0/todd/registries/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/registries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/registries/build_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/registries/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/registries/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/registries/partial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/registries/patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13436 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/registries/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/registries/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/registries/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/registries/visual.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.561437 todd_ai-0.5.0/todd/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.565437 todd_ai-0.5.0/todd/runners/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/callbacks/autocast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/callbacks/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/callbacks/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/callbacks/composed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/callbacks/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/callbacks/interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/callbacks/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/callbacks/lr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/callbacks/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/callbacks/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/callbacks/shadow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/epoch_based_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/iter_based_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/memo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/registries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.565437 todd_ai-0.5.0/todd/runners/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/strategies/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/strategies/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/strategies/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/strategies/fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.565437 todd_ai-0.5.0/todd/runners/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/utils/etas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/utils/priority_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/utils/runner_holder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/runners/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.565437 todd_ai-0.5.0/todd/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      819 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/scripts/crop_border.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/scripts/merge_lmdbs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.565437 todd_ai-0.5.0/todd/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.565437 todd_ai-0.5.0/todd/tasks/image_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/tasks/image_generation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.569437 todd_ai-0.5.0/todd/tasks/knowledge_distillation/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/tasks/knowledge_distillation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.569437 todd_ai-0.5.0/todd/tasks/knowledge_distillation/distillers/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/tasks/knowledge_distillation/distillers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.569437 todd_ai-0.5.0/todd/tasks/knowledge_distillation/distillers/adapts/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/tasks/knowledge_distillation/distillers/adapts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/tasks/knowledge_distillation/distillers/adapts/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/tasks/knowledge_distillation/distillers/adapts/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/tasks/knowledge_distillation/distillers/adapts/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/tasks/knowledge_distillation/distillers/adapts/decouple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/tasks/knowledge_distillation/distillers/adapts/detach.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/tasks/knowledge_distillation/distillers/adapts/dict_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/tasks/knowledge_distillation/distillers/adapts/list_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/tasks/knowledge_distillation/distillers/adapts/null.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/tasks/knowledge_distillation/distillers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.569437 todd_ai-0.5.0/todd/tasks/knowledge_distillation/distillers/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/tasks/knowledge_distillation/distillers/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/tasks/knowledge_distillation/distillers/hooks/append.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/tasks/knowledge_distillation/distillers/hooks/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/tasks/knowledge_distillation/distillers/hooks/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/tasks/knowledge_distillation/distillers/hooks/vanilla.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/tasks/knowledge_distillation/distillers/registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/tasks/knowledge_distillation/distillers/single_student.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.569437 todd_ai-0.5.0/todd/tasks/knowledge_distillation/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/tasks/knowledge_distillation/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6679 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/tasks/knowledge_distillation/losses/mimic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/tasks/knowledge_distillation/registries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.569437 todd_ai-0.5.0/todd/tasks/knowledge_distillation/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/tasks/knowledge_distillation/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/tasks/knowledge_distillation/utils/pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.569437 todd_ai-0.5.0/todd/tasks/object_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/tasks/object_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14157 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/tasks/object_detection/bboxes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.573437 todd_ai-0.5.0/todd/tasks/object_detection/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-31 15:40:46.000000 todd_ai-0.5.0/todd/tasks/object_detection/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-31 15:40:47.000000 todd_ai-0.5.0/todd/tasks/object_detection/losses/focal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.573437 todd_ai-0.5.0/todd/tasks/object_detection_knowledge_distillation/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-31 15:40:47.000000 todd_ai-0.5.0/todd/tasks/object_detection_knowledge_distillation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.573437 todd_ai-0.5.0/todd/tasks/object_detection_knowledge_distillation/distillers/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-31 15:40:47.000000 todd_ai-0.5.0/todd/tasks/object_detection_knowledge_distillation/distillers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.573437 todd_ai-0.5.0/todd/tasks/object_detection_knowledge_distillation/distillers/adapts/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-31 15:40:47.000000 todd_ai-0.5.0/todd/tasks/object_detection_knowledge_distillation/distillers/adapts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-31 15:40:47.000000 todd_ai-0.5.0/todd/tasks/object_detection_knowledge_distillation/distillers/adapts/iou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-05-31 15:40:47.000000 todd_ai-0.5.0/todd/tasks/object_detection_knowledge_distillation/distillers/adapts/mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-31 15:40:47.000000 todd_ai-0.5.0/todd/tasks/object_detection_knowledge_distillation/distillers/adapts/roi_align.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.573437 todd_ai-0.5.0/todd/tasks/object_detection_knowledge_distillation/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-31 15:40:47.000000 todd_ai-0.5.0/todd/tasks/object_detection_knowledge_distillation/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-05-31 15:40:47.000000 todd_ai-0.5.0/todd/tasks/object_detection_knowledge_distillation/losses/ckd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-31 15:40:47.000000 todd_ai-0.5.0/todd/tasks/object_detection_knowledge_distillation/losses/rcnn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.573437 todd_ai-0.5.0/todd/tasks/optical_flow_estimation/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-31 15:40:47.000000 todd_ai-0.5.0/todd/tasks/optical_flow_estimation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-05-31 15:40:47.000000 todd_ai-0.5.0/todd/tasks/optical_flow_estimation/optical_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-31 15:40:47.000000 todd_ai-0.5.0/todd/tasks/registries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.573437 todd_ai-0.5.0/todd/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-31 15:40:47.000000 todd_ai-0.5.0/todd/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-31 15:40:47.000000 todd_ai-0.5.0/todd/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-31 15:40:47.000000 todd_ai-0.5.0/todd/utils/ema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-31 15:40:47.000000 todd_ai-0.5.0/todd/utils/holders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-31 15:40:47.000000 todd_ai-0.5.0/todd/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-31 15:40:47.000000 todd_ai-0.5.0/todd/utils/seeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-31 15:40:47.000000 todd_ai-0.5.0/todd/utils/state_dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-31 15:40:47.000000 todd_ai-0.5.0/todd/utils/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-31 15:40:47.000000 todd_ai-0.5.0/todd/utils/stores.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11731 2024-05-31 15:40:47.000000 todd_ai-0.5.0/todd/utils/trees.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.577437 todd_ai-0.5.0/todd/visuals/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-31 15:40:47.000000 todd_ai-0.5.0/todd/visuals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-31 15:40:47.000000 todd_ai-0.5.0/todd/visuals/anchors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-05-31 15:40:47.000000 todd_ai-0.5.0/todd/visuals/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-31 15:40:47.000000 todd_ai-0.5.0/todd/visuals/cv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7976 2024-05-31 15:40:47.000000 todd_ai-0.5.0/todd/visuals/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-31 15:40:47.000000 todd_ai-0.5.0/todd/visuals/raster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:40:50.577437 todd_ai-0.5.0/todd_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16859 2024-05-31 15:40:50.000000 todd_ai-0.5.0/todd_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-05-31 15:40:50.000000 todd_ai-0.5.0/todd_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:40:50.000000 todd_ai-0.5.0/todd_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-31 15:40:50.000000 todd_ai-0.5.0/todd_ai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-31 15:40:50.000000 todd_ai-0.5.0/todd_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-31 15:40:50.000000 todd_ai-0.5.0/todd_ai.egg-info/top_level.txt
```

### Comparing `todd_ai-0.4.0/LICENSE` & `todd_ai-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `todd_ai-0.4.0/PKG-INFO` & `todd_ai-0.5.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: todd_ai
-Version: 0.4.0
+Version: 0.5.0
 Summary: Toolkit for Object Detection Distillation
 Author-email: Luting Wang <wangluting@buaa.edu.cn>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -206,20 +206,63 @@
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/LutingWang/todd
 Project-URL: Documentation, https://toddai.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: einops
+Requires-Dist: ffmpeg-python
+Requires-Dist: lmdb
+Requires-Dist: opencv-python
+Requires-Dist: pandas
+Requires-Dist: python-pptx
+Requires-Dist: tensorboard
+Requires-Dist: timm
+Requires-Dist: toml
+Requires-Dist: typing_extensions
+Requires-Dist: yapf
 Provides-Extra: dev
+Requires-Dist: autoflake; extra == "dev"
+Requires-Dist: bandit[toml]; extra == "dev"
+Requires-Dist: codespell; extra == "dev"
+Requires-Dist: commitizen; extra == "dev"
+Requires-Dist: doc8; extra == "dev"
+Requires-Dist: docformatter[tomli]; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: flake8-bugbear; extra == "dev"
+Requires-Dist: flake8-docstrings; extra == "dev"
+Requires-Dist: ipdb; extra == "dev"
+Requires-Dist: ipykernel; extra == "dev"
+Requires-Dist: jupyter; extra == "dev"
+Requires-Dist: matplotlib; extra == "dev"
+Requires-Dist: mccabe; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pandas-stubs; extra == "dev"
+Requires-Dist: pep8-naming; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pydocstyle; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
+Requires-Dist: torch-tb-profiler; extra == "dev"
+Requires-Dist: tqdm; extra == "dev"
+Requires-Dist: types-Pillow; extra == "dev"
+Requires-Dist: types-toml; extra == "dev"
+Requires-Dist: types-tqdm; extra == "dev"
 Provides-Extra: doc
+Requires-Dist: mmcv<2.0; extra == "doc"
+Requires-Dist: python-docs-theme; extra == "doc"
+Requires-Dist: sphinx; extra == "doc"
+Requires-Dist: sphinx_rtd_theme; extra == "doc"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: coverage; extra == "test"
+Requires-Dist: mmcv<2.0; extra == "test"
+Requires-Dist: pytest; extra == "test"
 
 # Toolkit for Object Detection Distillation
 
 ```text
 _/_/_/_/_/                _/        _/
    _/      _/_/      _/_/_/    _/_/_/
   _/    _/    _/  _/    _/  _/    _/
@@ -228,15 +271,15 @@
 ```
 
 [![docs](https://readthedocs.org/projects/toddai/badge/?version=latest)](https://toddai.readthedocs.io/en/latest/?badge=latest)
 [![lint](https://github.com/LutingWang/todd/actions/workflows/lint.yaml/badge.svg)](https://github.com/LutingWang/todd/actions/workflows/lint.yaml)
 [![test](https://github.com/LutingWang/todd/actions/workflows/test.yaml/badge.svg)](https://github.com/LutingWang/todd/actions/workflows/test.yaml)
 [![publish](https://github.com/LutingWang/todd/actions/workflows/publish.yaml/badge.svg)](https://github.com/LutingWang/todd/actions/workflows/publish.yaml)
 
-[![codecov](https://codecov.io/gh/LutingWang/todd/branch/master/graph/badge.svg?token=BHDPCKVM1T)](https://codecov.io/gh/LutingWang/todd)
+[![codecov](https://codecov.io/gh/LutingWang/todd/branch/main/graph/badge.svg?token=BHDPCKVM1T)](https://codecov.io/gh/LutingWang/todd)
 [![PyPI](https://img.shields.io/pypi/v/todd_ai)](https://pypi.org/project/todd-ai/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/todd_ai)]((https://pypi.org/project/todd-ai/))
 [![wakatime](https://wakatime.com/badge/github/LutingWang/todd.svg)](https://wakatime.com/badge/github/LutingWang/todd)
 
 ## Installation
 
 Prerequisites:
@@ -253,8 +296,14 @@
 
 ```bash
 pip install .\[dev,doc,test\]
 ```
 
 TODO
 
-1. Complete repr
+1. Complete repr, especially for runners
+2. mypy supports recursive types
+3. add a script to prepare imagenet dataset
+4. add Any to all missing typing fields
+5. make loss registry a sub-registry of model registry
+6. refactor registries
+7. remove odpsrun
```

### Comparing `todd_ai-0.4.0/todd/adapts/attention.py` & `todd_ai-0.5.0/todd/tasks/knowledge_distillation/distillers/adapts/attention.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,42 @@
+__all__ = [
+    'SpatialAttention',
+    'ChannelAttention',
+]
+
 import einops
 import torch
 import torch.nn.functional as F
 
-from .base import AdaptRegistry, BaseAdapt
+from ..registries import AdaptRegistry
+from .base import BaseAdapt
 
 
-@AdaptRegistry.register()
-class AbsMeanSpatialAttention(BaseAdapt):
+@AdaptRegistry.register_()
+class SpatialAttention(BaseAdapt):
 
-    def __init__(self, *args, temperature: float = 1, **kwargs):
+    def __init__(self, *args, temperature: float = 1, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self._temperature = temperature
 
     def forward(self, feat: torch.Tensor) -> torch.Tensor:
         _, _, h, w = feat.shape
         g = einops.reduce(
             torch.abs(feat),
             'n c h w -> n (h w)',
             reduction='mean',
         )
         a = h * w * F.softmax(g / self._temperature, dim=1)
         return einops.rearrange(a, 'n (h w) -> n 1 h w', h=h, w=w)
 
 
-@AdaptRegistry.register()
-class AbsMeanChannelAttention(BaseAdapt):
+@AdaptRegistry.register_()
+class ChannelAttention(BaseAdapt):
 
-    def __init__(self, *args, temperature: float = 1, **kwargs):
+    def __init__(self, *args, temperature: float = 1, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self._temperature = temperature
 
     def forward(self, feat: torch.Tensor) -> torch.Tensor:
         _, c, _, _ = feat.shape
         g = einops.reduce(torch.abs(feat), 'n c h w -> n c', reduction='mean')
         a = c * F.softmax(g / self._temperature, dim=1)
```

### Comparing `todd_ai-0.4.0/todd/adapts/base.py` & `todd_ai-0.5.0/todd/tasks/knowledge_distillation/distillers/registries.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 __all__ = [
-    'BaseAdapt',
     'AdaptRegistry',
+    'HookRegistry',
 ]
 
 import inspect
 import itertools
+from typing import cast
 
 import einops.layers.torch
-import torch.nn as nn
+from torch import nn
 
-from ..base import Registry
-from ..utils import Module
+from ....registries import Item
+from ..registries import DistillerRegistry
 
 
-class BaseAdapt(Module):
+class AdaptRegistry(DistillerRegistry):
     pass
 
 
-class AdaptRegistry(Registry):
+class HookRegistry(DistillerRegistry):
     pass
 
 
-for _, class_ in itertools.chain(
+for _, c in itertools.chain(
     inspect.getmembers(nn, inspect.isclass),
     inspect.getmembers(einops.layers.torch, inspect.isclass),
 ):
-    if issubclass(class_, nn.Module):
-        AdaptRegistry.register()(class_)
+    if issubclass(c, nn.Module):
+        AdaptRegistry.register_()(cast(Item, c))
 
-try:
+try:  # TODO: remove this
     import mmcv.cnn
 
     for k, v in itertools.chain(
         mmcv.cnn.CONV_LAYERS.module_dict.items(),
         mmcv.cnn.PLUGIN_LAYERS.module_dict.items(),
     ):
-        AdaptRegistry.register(keys=(f'mmcv_{k}', ))(v)
-except Exception:
+        AdaptRegistry.register_(f'mmcv_{k}')(v)
+except Exception:  # nosec B110 pylint: disable=broad-exception-caught
     pass
```

### Comparing `todd_ai-0.4.0/todd/adapts/custom.py` & `todd_ai-0.5.0/todd/tasks/knowledge_distillation/distillers/adapts/custom.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,18 @@
+__all__ = [
+    'Custom',
+]
+
 import string
 
-from .base import AdaptRegistry, BaseAdapt
+from ..registries import AdaptRegistry
+from .base import BaseAdapt
 
 
-@AdaptRegistry.register()
+@AdaptRegistry.register_()
 class Custom(BaseAdapt):
     """Custom adaptation described using patterns.
 
     Examples:
         >>> adapt = Custom(pattern='a + b * c')
         >>> adapt(1, 2, 3)
         7
@@ -17,17 +22,16 @@
         >>> adapt = Custom(pattern='a + b * c')
         >>> adapt(1, 2, 3, b=4)
         Traceback (most recent call last):
             ...
         RuntimeError: {'b'}
     """
 
-    def __init__(self, *args, pattern: str, **kwargs):
+    def __init__(self, *args, pattern: str, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self._pattern = pattern
 
     def forward(self, *args, **kwargs):
-        locals_ = dict(zip(string.ascii_letters, args))
-        if len(locals_.keys() & kwargs.keys()) != 0:
-            raise RuntimeError(locals_.keys() & kwargs.keys())
-        locals_.update(kwargs)
-        return eval(self._pattern, None, locals_)
+        if keys := set(string.ascii_letters) & kwargs.keys():
+            raise RuntimeError(keys)
+        kwargs |= zip(string.ascii_letters, args)
+        return eval(self._pattern, None, kwargs)  # nosec B307
```

### Comparing `todd_ai-0.4.0/todd/adapts/decouple.py` & `todd_ai-0.5.0/todd/tasks/knowledge_distillation/distillers/adapts/decouple.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,30 @@
+__all__ = [
+    'Decouple',
+]
+
 import einops
 import torch
-import torch.nn as nn
+from torch import nn
 
-from .base import AdaptRegistry, BaseAdapt
+from ..registries import AdaptRegistry
+from .base import BaseAdapt
 
 
-@AdaptRegistry.register()
+@AdaptRegistry.register_()
 class Decouple(BaseAdapt):
 
     def __init__(
         self,
         num: int,
         in_features: int,
         out_features: int,
         bias: bool = True,
         **kwargs,
-    ):
+    ) -> None:
         super().__init__(**kwargs)
         self._num = num
         self._layer = nn.Linear(in_features, out_features * num, bias)
 
     def forward(self, feat: torch.Tensor, id_: torch.Tensor) -> torch.Tensor:
         """Decouple features.
```

### Comparing `todd_ai-0.4.0/todd/adapts/dict_tensor.py` & `todd_ai-0.5.0/todd/tasks/knowledge_distillation/distillers/adapts/dict_tensor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+__all__ = [
+    'DictTensor',
+    'Union_',
+    'Intersect',
+]
+
 import itertools
 import operator
 from functools import reduce
 from typing import Iterable, Iterator, Mapping, Sequence, overload
 
 import einops
 import torch
 
-from .base import AdaptRegistry, BaseAdapt
-
-__all__ = [
-    'DictTensor',
-    'Union_',
-    'Intersect',
-]
+from ..registries import AdaptRegistry
+from .base import BaseAdapt
 
 KeyType = tuple[int, ...]
 
 
 class DictTensor(Mapping):
 
     def __init__(
@@ -94,35 +95,35 @@
         )
         dict_tensors = [
             DictTensor(keys, dict_tensor[keys]) for dict_tensor in dict_tensors
         ]
         return dict_tensors
 
 
-@AdaptRegistry.register(keys=('Union', ))
-class Union_(BaseAdapt):
+@AdaptRegistry.register_('Union')
+class Union_(BaseAdapt):  # pylint: disable=invalid-name
 
     def forward(
         self,
         feats: list[torch.Tensor],
         ids: list[torch.Tensor],
     ) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
-        """Match `feats` according to their `poses`.
+        """Match ``feats`` according to their ``poses``.
 
-        Align the `feats` coming from different sources to have same
-        `matched_pos` and stack them togethor. For positions where some
-        of `feats` do not show up, an all-zero tensor is added as
-        default. A 2D `mask` is returned to indicate the type of a
-        matched feature, where `1` corresponds to features coming from
-        `feats` and `0` for added default all-zero tensors.
+        Align the ``feats`` coming from different sources to have same
+        ``matched_pos`` and stack them togethor. For positions where some
+        of ``feats`` do not show up, an all-zero tensor is added as
+        default. A 2D ``mask`` is returned to indicate the type of a
+        matched feature, where ``1`` corresponds to features coming from
+        ``feats`` and ``0`` for added default all-zero tensors.
 
         Args:
             feats: [n_s x d_1 x d_2 x ... x d_m]
-                Features from `s` different sources, each source can
-                have different `n_s`.
+                Features from ``s`` different sources, each source can
+                have different ``n_s``.
             ids: [n_s x l]
                 Positions of each feature.
 
         Returns:
             union_feats: s x n x d_1 x d_2 x ... x d_m
             union_ids: n x l
             union_mask: s x n
@@ -135,29 +136,28 @@
             dict_tensor._values for dict_tensor in dict_tensors
         ])
         union_ids = union_feats.new_tensor(mask._keys)
         union_mask = einops.rearrange(mask._values, 'n s -> s n')
         return union_feats, union_ids, union_mask
 
 
-@AdaptRegistry.register()
+@AdaptRegistry.register_()
 class Intersect(BaseAdapt):
 
     def forward(
         self,
         feats: list[torch.Tensor],
         ids: list[torch.Tensor],
     ) -> list[torch.Tensor]:
-        """Match positions that show up both in `pred_poses` and
-        `target_poses`.
+        """Match positions.
 
         Args:
             feats: [n_s x d_1 x d_2 x ... x d_m]
-                Features from `s` different sources, each source can
-                have different `n_s`.
+                Features from ``s`` different sources, each source can
+                have different ``n_s``.
             ids: [n_s x l]
                 Positions of each feature.
 
         Returns:
             intersect_feats: [n x d_1 x d_2 x ... x d_m]
         """
         dict_tensors = [
```

### Comparing `todd_ai-0.4.0/todd/adapts/iou.py` & `todd_ai-0.5.0/todd/tasks/object_detection_knowledge_distillation/distillers/adapts/iou.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,39 @@
+__all__ = [
+    'IoU',
+]
+
 import torch
 
-from ..base import BBoxesXYXY
-from .base import AdaptRegistry, BaseAdapt
+from ....knowledge_distillation.distillers import AdaptRegistry
+from ....knowledge_distillation.distillers.adapts import BaseAdapt
+from ....object_detection import BBoxesXYXY
 
 
-@AdaptRegistry.register()
+@AdaptRegistry.register_()
 class IoU(BaseAdapt):
 
     def __init__(
         self,
         *args,
         aligned: bool = False,
         eps: float = 1e-6,
         **kwargs,
-    ):
+    ) -> None:
         super().__init__(*args, **kwargs)
         assert not aligned
         self._aligned = aligned
         self._eps = eps
 
     def _reshape(
         self,
         bboxes: torch.Tensor,
     ) -> tuple[torch.Tensor, torch.Size]:
-        """
+        """Reshape BBoxes.
+
         Args:
             bboxes: * x 4
 
         Returns:
             bboxes: prod(*) x 4
             shape: tuple(*)
         """
@@ -38,21 +44,22 @@
         return bboxes, shape
 
     def _iou(
         self,
         bboxes1: torch.Tensor,
         bboxes2: torch.Tensor,
     ) -> torch.Tensor:
-        """
+        r"""Compute IoU.
+
         Args:
-            bboxes1: \\*1 x 4
-            bboxes2: \\*2 x 4
+            bboxes1: \*1 x 4
+            bboxes2: \*2 x 4
 
         Returns:
-            ious: \\*1 x \\*2
+            ious: \*1 x \*2
         """
         bboxes1, shape1 = self._reshape(bboxes1)
         bboxes2, shape2 = self._reshape(bboxes2)
         ious = BBoxesXYXY.ious(
             BBoxesXYXY(bboxes1),
             BBoxesXYXY(bboxes2),
             self._eps,
@@ -60,15 +67,16 @@
         return ious.reshape(shape1 + shape2)
 
     def forward(
         self,
         bboxes1: list[torch.Tensor],
         bboxes2: list[torch.Tensor],
     ) -> list[list[torch.Tensor]]:
-        """
+        """Compute IoU.
+
         Args:
             bboxes1: n1 x m1 x 4
             bboxes2: n2 x m2 x 4
 
         Returns:
             ious: n1 x n2 x m1 x m2
         """
```

### Comparing `todd_ai-0.4.0/todd/adapts/mask.py` & `todd_ai-0.5.0/todd/tasks/object_detection_knowledge_distillation/distillers/adapts/mask.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,33 @@
+__all__ = [
+    'DeFeatMask',
+    'FGDMask',
+    'FGFIMask',
+    'FRSMask',
+]
+
 import math
-from abc import abstractmethod
+from abc import ABC, abstractmethod
 
 import einops
 import torch
 
-from .base import AdaptRegistry, BaseAdapt
+from ....knowledge_distillation.distillers import AdaptRegistry
+from ....knowledge_distillation.distillers.adapts import BaseAdapt
 
 
 class MultiLevelMask:
 
     def __init__(
         self,
         *args,
         strides: list[int],
         ceil_mode: bool = False,
         **kwargs,
-    ):
+    ) -> None:
         self._strides = strides
         self._ceil_mode = ceil_mode
         super().__init__(*args, **kwargs)
 
     @property
     def strides(self) -> list[int]:
         return self._strides
@@ -42,15 +50,16 @@
     def forward(
         self,
         shape: tuple[int, int],
         bboxes: list[torch.Tensor],
         *args,
         **kwargs,
     ) -> list[torch.Tensor]:
-        """
+        """Compute Multilevel Mask.
+
         Args:
             shape: (h, w)
             bboxes: n x m x 4
 
         Returns:
             masks: l x n x 1 x h x w
         """
@@ -60,17 +69,17 @@
             level_shape = (self._div(h, stride), self._div(w, stride))
             level_bboxes = [bbox / stride for bbox in bboxes]
             mask = self._forward(level_shape, level_bboxes, *args, **kwargs)
             masks.append(mask)
         return masks
 
 
-class SingleLevelMask(MultiLevelMask):
+class SingleLevelMask(MultiLevelMask, ABC):
 
-    def __init__(self, *args, stride: int, **kwargs):
+    def __init__(self, *args, stride: int, **kwargs) -> None:
         super().__init__(*args, strides=[stride], **kwargs)
 
     @property
     def stride(self) -> int:
         return self.strides[0]
 
     def forward(  # type: ignore[override]
@@ -78,104 +87,30 @@
         *args,
         **kwargs,
     ) -> torch.Tensor:
         masks = super().forward(*args, **kwargs)
         return masks[0]
 
 
-@AdaptRegistry.register()
-class LabelEncMask(BaseAdapt):
-
-    def __init__(
-        self,
-        *args,
-        num_classes: int = 80,
-        aug: bool = True,
-        **kwargs,
-    ):
-        super().__init__(*args, **kwargs)
-        self._num_classes = num_classes
-        self._aug = aug
-
-    def _mask(
-        self,
-        shape: tuple[int, int],
-        bboxes: torch.Tensor,
-        labels: torch.Tensor,
-    ) -> torch.Tensor:
-        """
-        Args:
-            shape: (h, w)
-            bboxes: m x 4
-            labels: m
-
-        Returns:
-            mask: k x h x w
-        """
-        masks = bboxes.new_zeros(self._num_classes, *shape)
-        bboxes = torch.cat(
-            [
-                bboxes[:, 2:] - bboxes[:, :2],
-                (bboxes[:, :2] + bboxes[:, 2:]) / 2
-            ],
-            dim=-1,
-        )
-        y, x = torch.meshgrid(
-            torch.arange(0, shape[0], dtype=torch.float, device=bboxes.device),
-            torch.arange(0, shape[1], dtype=torch.float, device=bboxes.device),
-        )
-        for (w, h, cx, cy), label in zip(bboxes.tolist(), labels.tolist()):
-            value = torch.max(
-                torch.abs(x - cx) / w,
-                torch.abs(y - cy) / h,
-            )
-            value = (1 - value) * (value < 0.5)
-            if self._aug:
-                weight = torch.rand((), device=value.device).clamp_max(0.5) * 2
-                value = value * weight
-            torch.maximum(masks[label], value, out=masks[label])
-        return masks
-
-    def forward(
-        self,
-        shape: tuple[int, int],
-        bboxes: list[torch.Tensor],
-        labels: list[torch.Tensor],
-    ) -> torch.Tensor:
-        """
-        Args:
-            shape: (h, w)
-            bboxes: n x m x 4
-            labels: n x m
-
-        Returns:
-            masks: n x k x h x w
-        """
-        masks = [  # yapf: disable
-            self._mask(shape, bbox, label)
-            for bbox, label in zip(bboxes, labels)
-        ]
-        return torch.stack(masks)
-
-
-@AdaptRegistry.register()
+@AdaptRegistry.register_()
 class DeFeatMask(MultiLevelMask, BaseAdapt):
 
     def __init__(
         self,
         *args,
         neg_gain: float = 4,
         **kwargs,
-    ):
+    ) -> None:
         super().__init__(*args, **kwargs)
         self._neg_gain = neg_gain
 
     @staticmethod
     def _normalize(masks: torch.Tensor) -> torch.Tensor:
-        """
+        """Normalize masks.
+
         Args:
             masks: n x 1 x h x w
 
         Returns:
             normalized_masks: n x 1 x h x w
         """
         values = einops.reduce(
@@ -193,15 +128,16 @@
         return self._normalize(masks)
 
     def _mask(
         self,
         shape: tuple[int, int],
         bboxes: torch.Tensor,
     ) -> torch.Tensor:
-        """
+        """Compute DeFeat Mask.
+
         Args:
             shape: (h, w)
             bboxes: m x 4
 
         Returns:
             mask: h x w
         """
@@ -213,15 +149,16 @@
     def _forward(
         self,
         shape: tuple[int, int],
         bboxes: list[torch.Tensor],
         *args,
         **kwargs,
     ) -> torch.Tensor:
-        """
+        """Compute DeFeat Mask.
+
         Args:
             shape: (h, w)
             bboxes: n x m x 4
 
         Returns:
             masks: n x 1 x h x w
         """
@@ -229,26 +166,27 @@
         masks = einops.rearrange(masks, 'n h w -> n 1 h w')
         masks = self._normalize_pos(masks)
         neg_masks = self._normalize_neg(masks <= 0)
         neg_masks = neg_masks * self._neg_gain
         return masks + neg_masks
 
 
-@AdaptRegistry.register()
+@AdaptRegistry.register_()
 class FGDMask(DeFeatMask):
 
     def _normalize_pos(self, masks: torch.Tensor) -> torch.Tensor:
         return masks
 
     def _mask(
         self,
         shape: tuple[int, int],
         bboxes: torch.Tensor,
     ) -> torch.Tensor:
-        """
+        """Compute FGD Mask.
+
         Args:
             shape: (h, w)
             bboxes: m x 4
 
         Returns:
             mask: h x w
         """
@@ -260,23 +198,24 @@
         )
         for i, (x0, y0, x1, y1) in enumerate(bboxes.tolist()):
             area = mask[y0:y1 + 2, x0:x1 + 2]
             torch.maximum(area, values[i], out=area)
         return mask
 
 
-@AdaptRegistry.register()
+@AdaptRegistry.register_()
 class FGFIMask(BaseAdapt):
 
-    def __init__(self, *args, thresh: float = 0.5, **kwargs):
+    def __init__(self, *args, thresh: float = 0.5, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self._thresh = thresh
 
     def _instance(self, ious: torch.Tensor) -> torch.Tensor:
-        """
+        """Compute FGFI Mask for an instance.
+
         Args:
             ious: h x w x k x m
 
         Returns:
             mask: h x w
         """
         thresh = einops.reduce(
@@ -284,27 +223,29 @@
             'h w k m -> 1 1 1 m',
             reduction='max',
         ) * self._thresh
         mask = einops.reduce(ious > thresh, 'h w k m -> h w', reduction='max')
         return mask
 
     def _batch(self, ious: list[torch.Tensor]) -> torch.Tensor:
-        """
+        """Compute FGFI Mask for a batch.
+
         Args:
             ious: n x h x w x k x m
 
         Returns:
             masks: n x 1 x h x w
         """
         masks = torch.stack([self._instance(iou) for iou in ious])
         masks = einops.rearrange(masks, 'n h w -> n 1 h w')
         return masks
 
     def forward(self, ious: list[list[torch.Tensor]]) -> list[torch.Tensor]:
-        """
+        """Compute FGFI Mask.
+
         Args:
             ious: l x n x h x w x k x m
 
         Returns:
             masks: l x n x 1 x h x w
         """
         masks = [self._batch(iou) for iou in ious]
@@ -327,23 +268,24 @@
 #             bboxes.int().tolist(),
 #             labels.tolist(),
 #         ):
 #             masks[label, y0:y1 + 1, x0:x1 + 1] = 1
 #         return masks
 
 
-@AdaptRegistry.register()
+@AdaptRegistry.register_()
 class FRSMask(BaseAdapt):
 
-    def __init__(self, *args, with_logits: bool = True, **kwargs):
+    def __init__(self, *args, with_logits: bool = True, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self._with_logits = with_logits
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
-        """
+        """Compute FRS Mask.
+
         Args:
             x: n x c x h x w
 
         Returns:
             masks: n x 1 x h x w
         """
         x = x.detach()
```

### Comparing `todd_ai-0.4.0/todd/adapts/roi_align.py` & `todd_ai-0.5.0/todd/tasks/object_detection_knowledge_distillation/distillers/adapts/roi_align.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,40 @@
+__all__ = [
+    'RoIAlign',
+]
+
 import torch
+from torch import nn
 
-from ..utils import ModuleList
-from .base import AdaptRegistry, BaseAdapt
+from ....knowledge_distillation.distillers import AdaptRegistry
+from ....knowledge_distillation.distillers.adapts import BaseAdapt
 
 
-@AdaptRegistry.register()
+@AdaptRegistry.register_()
 class RoIAlign(BaseAdapt):
 
-    def __init__(self, strides: list[int], *args, **kwargs):
+    def __init__(self, strides: list[int], *args, **kwargs) -> None:
         import mmcv.ops
 
         super().__init__(*args, **kwargs)
-        self._layers = ModuleList([
+        self._layers = nn.ModuleList([
             mmcv.ops.RoIAlign(
                 spatial_scale=1 / s,
                 output_size=7,
                 sampling_ratio=0,
             ) for s in strides
         ])
 
     def forward(
         self,
         feats: list[torch.Tensor],
         bboxes: list[torch.Tensor],
     ) -> list[torch.Tensor]:
-        """
+        """Perform RoI Align.
+
         Args:
             feats: l x n x c x h x w
             bboxes: n x r x 4
 
         Returns:
             roi_feats: l x r x c x 7 x 7
         """
```

### Comparing `todd_ai-0.4.0/todd/base/bboxes.py` & `todd_ai-0.5.0/todd/tasks/object_detection/bboxes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,176 +1,180 @@
+# pylint: disable=invalid-name,self-cls-assignment
+
 __all__ = [
-    'BBox',
     'BBoxes',
+    'BBoxesXY__',
+    'BBoxesCXCY__',
+    'BBoxes__XY',
+    'BBoxes__WH',
     'BBoxesXYXY',
     'BBoxesXYWH',
     'BBoxesCXCYWH',
 ]
 
-import numbers
+import functools
 from abc import ABC, abstractmethod
-from typing import Generator, TypeVar
+from typing import Any, Generator, TypeVar
 from typing_extensions import Self
 
 import einops
 import torch
 
-BBox = tuple[numbers.Real, numbers.Real, numbers.Real, numbers.Real]
+BBox = tuple[float, float, float, float]
 T = TypeVar('T', bound='BBoxes')
 
 
 class BBoxes(ABC):
 
-    def __init__(self, bboxes: torch.Tensor) -> None:
-        """Initialize.
+    def __init__(
+        self,
+        bboxes: torch.Tensor,
+        *,
+        normalized: bool = False,
+        image_wh: tuple[int, int] | None = None,
+    ) -> None:
+        r"""Initialize.
 
         Args:
-            bboxes: :math:`n \\times 4`.
+            bboxes: :math:`n \times 4`.
+            normalized: whether the bboxes are normalized.
+            image_wh: the size of the image.
 
         Bounding boxes must be 2 dimensional and the second dimension must be
-        of size 4:
-
-            >>> bboxes = torch.tensor([[10.0, 20.0, 40.0, 100.0]])
-            >>> BBoxesXYXY(bboxes[0])
-            Traceback (most recent call last):
-            ...
-            ValueError: bboxes must be at least 2-dim
-            >>> BBoxesXYXY(bboxes[:, :3])
-            Traceback (most recent call last):
-            ...
-            ValueError: bboxes must have 4 columns
+        of size 4.
         """
-        if bboxes.ndim < 2:
-            raise ValueError('bboxes must be at least 2-dim')
+        if bboxes.ndim != 2:
+            raise ValueError('bboxes must be 2-dim')
         if bboxes.shape[-1] != 4:
             raise ValueError('bboxes must have 4 columns')
         self._bboxes = bboxes
+        self._normalized = normalized
+        if image_wh is not None:
+            self.set_image_wh(image_wh)
 
     def __len__(self) -> int:
-        """Number of bboxes.
+        return self._bboxes.shape[0]
 
-        Examples:
+    def __iter__(self) -> Generator[BBox, None, None]:
+        """Iterate over bboxes.
 
-            >>> bboxes = torch.tensor([
-            ...     [5.0, 15.0, 8.0, 18.0],
-            ...     [5.0, 15.0, 8.0, 60.0],
-            ... ])
-            >>> len(BBoxesXYXY(bboxes))
-            2
+        Yields:
+            One bbox.
         """
-        return self._bboxes.shape[0]
+        yield from map(tuple, self._bboxes.tolist())
 
     def __repr__(self) -> str:
-        return f'{self.__class__.__name__}({self._bboxes})'
-
-    def __add__(self, other: Self) -> Self:
-        """Concatenate bboxes.
-
-        Args:
-            other: :math:`n' \\times 4`.
-
-        Returns:
-            :math:`(n + n') \\times 4`, where `n` is the length of `self`.
-
-        Examples:
-
-            >>> a = torch.tensor([[5.0, 15.0, 8.0, 18.0]])
-            >>> b = torch.tensor([[5.0, 15.0, 8.0, 60.0]])
-            >>> BBoxesXYXY(a) + BBoxesXYXY(b)
-            BBoxesXYXY(tensor([[ 5., 15.,  8., 18.],
-                    [ 5., 15.,  8., 60.]]))
-        """
-        bboxes = torch.cat([self._bboxes, other._bboxes])
-        return self.__class__(bboxes)
+        kwargs = ''
+        if self._normalized:
+            kwargs += ', normalized=True'
+        if self.has_image_wh:
+            kwargs += f', image_wh={self._image_wh}'
+        return f'{type(self).__name__}({self._bboxes}{kwargs})'
+
+    def _copy(self, bboxes: torch.Tensor, **kwargs) -> Self:
+        if self._normalized:
+            kwargs.setdefault('normalized', True)
+        if self.has_image_wh:
+            kwargs.setdefault('image_wh', self._image_wh)
+        return self.__class__(bboxes, **kwargs)
 
     def __getitem__(self, indices) -> Self:
         """Get specific bboxes.
 
         Args:
             indices: a index or multiple indices.
 
         Returns:
             If `indices` refers to a single box, return a ``tuple``.
             Otherwise, return ``BBoxes``.
-
-        Examples:
-
-            >>> bboxes = torch.tensor([
-            ...     [5.0, 15.0, 8.0, 18.0],
-            ...     [5.0, 15.0, 8.0, 60.0],
-            ...     [5.0, 15.0, 8.0, 105.0],
-            ... ])
-            >>> BBoxesXYXY(bboxes)[0]
-            BBoxesXYXY(tensor([[ 5., 15.,  8., 18.]]))
-            >>> BBoxesXYXY(bboxes)[:-1]
-            BBoxesXYXY(tensor([[ 5., 15.,  8., 18.],
-                    [ 5., 15.,  8., 60.]]))
         """
-        tensor = self._bboxes[indices]
-        if tensor.ndim == 1:
-            tensor = tensor.unsqueeze(0)
-        return self.__class__(tensor)
+        bboxes = self._bboxes[indices]
+        if bboxes.ndim == 1:
+            bboxes = bboxes.unsqueeze(0)
+        return self._copy(bboxes)
 
-    def __iter__(self) -> Generator[BBox, None, None]:
-        """Iterate over bboxes.
-
-        Yields:
-            One bbox.
+    def __add__(self, other: Self) -> Self:
+        r"""Concatenate bboxes.
 
-        Examples:
+        Args:
+            other: :math:`n' \times 4`.
 
-            >>> bboxes = torch.tensor([
-            ...     [5.0, 15.0, 8.0, 18.0],
-            ...     [5.0, 15.0, 8.0, 60.0],
-            ...     [5.0, 15.0, 8.0, 105.0],
-            ... ])
-            >>> for bbox in BBoxesXYXY(bboxes):
-            ...     print(bbox)
-            (5.0, 15.0, 8.0, 18.0)
-            (5.0, 15.0, 8.0, 60.0)
-            (5.0, 15.0, 8.0, 105.0)
+        Returns:
+            :math:`(n + n') \times 4`, where `n` is the length of `self`.
         """
-        yield from map(tuple, self._bboxes.tolist())
+        assert self._normalized == other._normalized
+        if self.has_image_wh:
+            assert self._image_wh == other._image_wh
+        else:
+            assert not other.has_image_wh
+        bboxes = torch.cat([self._bboxes, other._bboxes])
+        return self._copy(bboxes)
 
-    def __and__(self, other: 'BBoxes') -> torch.Tensor:
-        """Intersections.
+    @property
+    def normalized(self) -> bool:
+        return self._normalized
 
-        Args:
-            other: :math:`n' \\times 4`.
+    @property
+    def has_image_wh(self) -> bool:
+        return hasattr(self, '_image_wh')
 
-        Returns:
-            :math:`n \\times n'`.
-        """
-        lt = torch.maximum(  # [n, n', 2]
-            einops.rearrange(self.lt, 'n1 lt -> n1 1 lt'),
-            einops.rearrange(other.lt, 'n2 lt -> 1 n2 lt'),
-        )
-        rb = torch.minimum(  # [n, n', 2]
-            einops.rearrange(self.rb, 'n1 rb -> n1 1 rb'),
-            einops.rearrange(other.rb, 'n2 rb -> 1 n2 rb'),
-        )
-        wh = rb - lt
-        wh = wh.clamp_min_(0)
-        return wh[..., 0] * wh[..., 1]
+    @property
+    def image_wh(self) -> tuple[int, int]:
+        return self._image_wh
 
-    def __or__(self, other: 'BBoxes') -> torch.Tensor:
-        """Wraps `unions`.
+    def set_image_wh(
+        self,
+        image_wh: tuple[int, int],
+        override: bool = False,
+    ) -> None:
+        if not self.has_image_wh or override:
+            self._image_wh = image_wh
+            return
+        assert self._image_wh == image_wh, f"{self._image_wh} != {image_wh}"
 
-        Args:
-            other: :math:`n' \\times 4`.
+    def to_tensor(self) -> torch.Tensor:
+        return self._bboxes
 
-        Returns:
-            :math:`n \\times n'`.
-        """
-        return self.unions(other, self & other)
+    def _scale(self, ratio_xy: tuple[float, float]) -> torch.Tensor:
+        return self._bboxes.new_tensor(ratio_xy * 2)
 
-    @classmethod
-    @abstractmethod
-    def _from_bboxes(cls, bboxes: 'BBoxes') -> torch.Tensor:
-        pass
+    def scale(self, ratio_xy: tuple[float, float]) -> Self:
+        ratio = self._scale(ratio_xy)
+        bboxes = self._bboxes * ratio
+        return self._copy(bboxes)
+
+    def __mul__(self, ratio_xy: tuple[float, float]) -> Self:
+        return self.scale(ratio_xy)
+
+    def __truediv__(self, ratio_xy: tuple[float, float]) -> Self:
+        w, h = ratio_xy
+        ratio_xy = (1 / w, 1 / h)
+        return self.scale(ratio_xy)
+
+    def _translate(self, offset_xy: tuple[float, float]) -> torch.Tensor:
+        return self._bboxes.new_tensor(offset_xy * 2)
+
+    def translate(self, offset_xy: tuple[float, float]) -> Self:
+        offset = self._translate(offset_xy)
+        bboxes = self._bboxes + offset
+        return self._copy(bboxes)
+
+    def normalize(self) -> Self:
+        if self._normalized:
+            return self._copy(self._bboxes)
+        self = self / self.image_wh
+        self._normalized = True
+        return self
+
+    def denormalize(self) -> Self:
+        if not self._normalized:
+            return self._copy(self._bboxes)
+        self = self.scale(self.image_wh)
+        self._normalized = False
+        return self
 
     @property
     @abstractmethod
     def left(self) -> torch.Tensor:
         pass
 
     @property
@@ -224,168 +228,226 @@
         pass
 
     @property
     @abstractmethod
     def center(self) -> torch.Tensor:
         pass
 
-    @abstractmethod
-    def _round(self) -> torch.Tensor:
-        pass
+    @property
+    def area(self) -> torch.Tensor:
+        return self.width * self.height
 
+    @classmethod
     @abstractmethod
-    def _expand(self, ratio_wh: tuple[float, float]) -> torch.Tensor:
-        pass
+    def _from1(cls, bboxes: 'BBoxes') -> torch.Tensor:
+        """Convert to the first two coordinates of the bboxes.
 
-    @abstractmethod
-    def _clamp(self, image_wh: tuple[int, int]) -> torch.Tensor:
-        pass
+        Args:
+            bboxes: the bboxes to convert.
 
-    @abstractmethod
-    def _scale(self, ratio_wh: tuple[float, float]) -> torch.Tensor:
-        pass
+        Returns:
+            A tensor representing the first two coordinates of the bboxes.
+        """
 
+    @classmethod
     @abstractmethod
-    def _translate(self, offset: torch.Tensor) -> torch.Tensor:
-        """Translate bboxes.
+    def _from2(cls, bboxes: 'BBoxes') -> torch.Tensor:
+        """Convert to the last two coordinates of the bboxes.
 
         Args:
-            offset: :math:`n \\times 2` or 2.
+            bboxes: the bboxes to convert.
 
         Returns:
-            Translated bboxes.
+            A tensor representing the last two coordinates of the bboxes.
         """
-        pass
-
-    @property
-    def area(self) -> torch.Tensor:
-        return self.width * self.height
 
-    def to_tensor(self) -> torch.Tensor:
-        return self._bboxes
+    @classmethod
+    def from_(cls, bboxes: 'BBoxes') -> Self:
+        from1 = cls._from1(bboxes)
+        from2 = cls._from2(bboxes)
+        from_ = torch.cat([from1, from2], dim=-1)
+        kwargs: dict[str, Any] = dict()
+        if bboxes._normalized:
+            kwargs['normalized'] = True
+        if bboxes.has_image_wh:
+            kwargs['image_wh'] = bboxes._image_wh
+        return cls(from_, **kwargs)
 
     def to(self, cls: type[T]) -> T:
-        return cls.from_bboxes(self)
+        return cls.from_(self)
+
+    def intersections(self, other: 'BBoxes') -> torch.Tensor:
+        r"""Intersections.
+
+        Args:
+            other: :math:`n' \times 4`.
+
+        Returns:
+            :math:`n \times n'`.
+        """
+        lt = torch.maximum(  # [n, n', 2]
+            einops.rearrange(self.lt, 'n1 lt -> n1 1 lt'),
+            einops.rearrange(other.lt, 'n2 lt -> 1 n2 lt'),
+        )
+        rb = torch.minimum(  # [n, n', 2]
+            einops.rearrange(self.rb, 'n1 rb -> n1 1 rb'),
+            einops.rearrange(other.rb, 'n2 rb -> 1 n2 rb'),
+        )
+        wh = rb - lt
+        wh = wh.clamp_min_(0)
+        return wh[..., 0] * wh[..., 1]
+
+    def __and__(self, other: 'BBoxes') -> torch.Tensor:
+        return self.intersections(other)
 
     def unions(
         self,
         other: 'BBoxes',
         intersections: torch.Tensor,
     ) -> torch.Tensor:
-        """Unions.
+        r"""Unions.
 
         Args:
-            other: :math:`n' \\times 4`.
-            intersections: :math:`n \\times n'`
+            other: :math:`n' \times 4`.
+            intersections: :math:`n \times n'`
 
         Returns:
-            :math:`n \\times n'`.
+            :math:`n \times n'`.
         """
         return self.area[:, None] + other.area[None, :] - intersections
 
-    def ious(self, other: 'BBoxes', eps: float = 1e-6) -> torch.Tensor:
-        """Intersections over unions.
+    def __or__(self, other: 'BBoxes') -> torch.Tensor:
+        r"""Wrap `unions`.
 
         Args:
-            other: :math:`n' \\times 4`.
-            eps: avoid division by zero.
+            other: :math:`n' \times 4`.
 
         Returns:
-            :math:`n \\times n'`.
+            :math:`n \times n'`.
         """
-        intersections = self & other
-        unions = self.unions(other, intersections).clamp_min_(eps)
-        return intersections / unions
+        intersections = self.intersections(other)
+        return self.unions(other, intersections)
 
-    @classmethod
-    def from_bboxes(cls, *args, **kwargs) -> Self:
-        return cls(cls._from_bboxes(*args, **kwargs))
+    def ious(self, other: 'BBoxes', eps: float = 1e-6) -> torch.Tensor:
+        r"""Intersections over unions.
 
-    def round(self, *args, **kwargs) -> Self:
-        return self.__class__(self._round(*args, **kwargs))
+        Args:
+            other: :math:`n' \times 4`.
+            eps: avoid division by zero.
 
-    def expand(self, *args, **kwargs) -> Self:
-        return self.__class__(self._expand(*args, **kwargs))
+        Returns:
+            :math:`n \times n'`.
+        """
+        intersections = self.intersections(other)
+        unions = self.unions(other, intersections)
+        unions = unions.clamp_min_(eps)
+        return intersections / unions
 
-    def clamp(self, *args, **kwargs) -> Self:
-        return self.__class__(self._clamp(*args, **kwargs))
+    def round(self) -> Self:
+        return self.to(BBoxesXYXY).round().to(self.__class__)
 
-    def scale(self, *args, **kwargs) -> Self:
-        return self.__class__(self._scale(*args, **kwargs))
+    def expand(self, ratio_wh: tuple[float, float]) -> Self:
+        return self.to(BBoxesCXCYWH).expand(ratio_wh).to(self.__class__)
 
-    def translate(self, *args, **kwargs) -> Self:
-        return self.__class__(self._translate(*args, **kwargs))
+    def clamp(self) -> Self:
+        return self.to(BBoxesXYXY).clamp().to(self.__class__)
 
     def indices(
         self,
         *,
-        min_area: numbers.Real | None = None,
-        min_wh: tuple[int, int] | None = None,
+        min_area: float | None = None,
+        min_wh: tuple[float, float] | None = None,
     ) -> torch.Tensor:
         indices = self._bboxes.new_ones(len(self), dtype=torch.bool)
         if min_area is not None:
             indices &= self.area.ge(min_area)
         if min_wh is not None:
             indices &= self.wh.ge(torch.tensor(min_wh)).all(-1)
         return indices
 
 
-class BBoxesXY(BBoxes):
+class BBoxesXY__(BBoxes):
 
     @property
     def left(self) -> torch.Tensor:
         return self._bboxes[:, 0]
 
     @property
     def top(self) -> torch.Tensor:
         return self._bboxes[:, 1]
 
     @property
     def lt(self) -> torch.Tensor:
         return self._bboxes[:, :2]
 
-    def _scale(self, ratio_wh: tuple[float, float]) -> torch.Tensor:
-        scale = torch.tensor(ratio_wh * 2)
-        return self._bboxes * scale
+    @classmethod
+    def _from1(cls, bboxes: BBoxes) -> torch.Tensor:
+        return bboxes.lt
 
 
-class BBoxesWH(BBoxes):
+class BBoxesCXCY__(BBoxes):
 
     @property
-    def width(self) -> torch.Tensor:
+    def center_x(self) -> torch.Tensor:
+        return self._bboxes[:, 0]
+
+    @property
+    def center_y(self) -> torch.Tensor:
+        return self._bboxes[:, 1]
+
+    @property
+    def center(self) -> torch.Tensor:
+        return self._bboxes[:, :2]
+
+    @classmethod
+    def _from1(cls, bboxes: BBoxes) -> torch.Tensor:
+        return bboxes.center
+
+
+class BBoxes__XY(BBoxes):  # noqa: N801
+
+    @property
+    def right(self) -> torch.Tensor:
         return self._bboxes[:, 2]
 
     @property
-    def height(self) -> torch.Tensor:
+    def bottom(self) -> torch.Tensor:
         return self._bboxes[:, 3]
 
     @property
-    def wh(self) -> torch.Tensor:
+    def rb(self) -> torch.Tensor:
         return self._bboxes[:, 2:]
 
-    def _translate(self, offset: torch.Tensor) -> torch.Tensor:
-        offset = torch.cat([offset, torch.zeros_like(offset)], dim=-1)
-        return self._bboxes + offset
-
+    @classmethod
+    def _from2(cls, bboxes: BBoxes) -> torch.Tensor:
+        return bboxes.rb
 
-class BBoxesXYXY(BBoxesXY):
 
-    @classmethod
-    def _from_bboxes(cls, bboxes: BBoxes) -> torch.Tensor:
-        return torch.cat([bboxes.lt, bboxes.rb], dim=-1)
+class BBoxes__WH(BBoxes):  # noqa: N801
 
     @property
-    def right(self) -> torch.Tensor:
+    def width(self) -> torch.Tensor:
         return self._bboxes[:, 2]
 
     @property
-    def bottom(self) -> torch.Tensor:
+    def height(self) -> torch.Tensor:
         return self._bboxes[:, 3]
 
     @property
+    def wh(self) -> torch.Tensor:
+        return self._bboxes[:, 2:]
+
+    @classmethod
+    def _from2(cls, bboxes: BBoxes) -> torch.Tensor:
+        return bboxes.wh
+
+
+class BBoxesXYXY(BBoxesXY__, BBoxes__XY):
+
+    @property
     def width(self) -> torch.Tensor:
         return self.right - self.left
 
     @property
     def height(self) -> torch.Tensor:
         return self.bottom - self.top
 
@@ -394,50 +456,52 @@
         return (self.left + self.right) / 2
 
     @property
     def center_y(self) -> torch.Tensor:
         return (self.top + self.bottom) / 2
 
     @property
-    def rb(self) -> torch.Tensor:
-        return self._bboxes[:, 2:]
-
-    @property
     def wh(self) -> torch.Tensor:
         return self.rb - self.lt
 
     @property
     def center(self) -> torch.Tensor:
         return (self.lt + self.rb) / 2
 
-    def _round(self) -> torch.Tensor:
-        lt = self.lt.floor()
-        rb = self.rb.ceil()
-        return torch.cat([lt, rb], dim=-1)
+    @staticmethod
+    def _denormalized_decorator(func):
 
-    def _expand(self, ratio_wh: tuple[float, float]) -> torch.Tensor:
-        delta = self.wh * (torch.tensor(ratio_wh) - 1) / 2
-        delta = torch.cat([-delta, delta], dim=-1)
-        return self._bboxes + delta
+        @functools.wraps(func)
+        def wrapper(self: Self, *args, **kwargs) -> Self:
+            if normalized := self._normalized:
+                self = self.denormalize()
+            self = func(self, *args, **kwargs)
+            if normalized:
+                self = self.normalize()
+            return self
 
-    def _clamp(self, image_wh: tuple[int, int]) -> torch.Tensor:
-        lt = self.lt.clamp_min(0)
-        rb = self.rb.clamp_max(torch.tensor(image_wh))
-        return torch.cat([lt, rb], dim=-1)
-
-    def _translate(self, offset: torch.Tensor) -> torch.Tensor:
-        offset = torch.cat([offset, offset], dim=-1)
-        return self._bboxes + offset
+        return wrapper
 
+    @_denormalized_decorator
+    def round(self) -> Self:
+        lt = self.lt.floor()
+        rb = self.rb.ceil()
+        bboxes = torch.cat([lt, rb], dim=-1)
+        self = self._copy(bboxes)
+        return self
+
+    @_denormalized_decorator
+    def clamp(self) -> Self:
+        image_wh = self._bboxes.new_tensor(self.image_wh * 2)
+        bboxes = self._bboxes.clamp_min(0).clamp_max(image_wh)
+        self = self._copy(bboxes)
+        return self
 
-class BBoxesXYWH(BBoxesXY, BBoxesWH):
 
-    @classmethod
-    def _from_bboxes(cls, bboxes: BBoxes) -> torch.Tensor:
-        return torch.cat([bboxes.lt, bboxes.wh], dim=-1)
+class BBoxesXYWH(BBoxesXY__, BBoxes__WH):
 
     @property
     def right(self) -> torch.Tensor:
         return self.left + self.width
 
     @property
     def bottom(self) -> torch.Tensor:
@@ -455,47 +519,16 @@
     def rb(self) -> torch.Tensor:
         return self.lt + self.wh
 
     @property
     def center(self) -> torch.Tensor:
         return self.lt + self.wh / 2
 
-    def _round(self) -> torch.Tensor:
-        lt = self.lt.floor()
-        wh = self.rb.ceil() - lt
-        return torch.cat([lt, wh], dim=-1)
-
-    def _expand(self, ratio_wh: tuple[float, float]) -> torch.Tensor:
-        wh = self.wh * torch.tensor(ratio_wh)
-        lt = self.lt - (wh - self.wh) / 2
-        return torch.cat([lt, wh], dim=-1)
-
-    def _clamp(self, image_wh: tuple[int, int]) -> torch.Tensor:
-        lt = self.lt.clamp_min(0)
-        rb = self.rb.clamp_max(torch.tensor(image_wh))
-        return torch.cat([lt, rb - lt], dim=-1)
-
-
-class BBoxesCXCYWH(BBoxesWH):
-
-    @classmethod
-    def _from_bboxes(cls, bboxes: BBoxes) -> torch.Tensor:
-        return torch.cat([bboxes.center, bboxes.wh], dim=-1)
-
-    @property
-    def center_x(self) -> torch.Tensor:
-        return self._bboxes[:, 0]
-
-    @property
-    def center_y(self) -> torch.Tensor:
-        return self._bboxes[:, 1]
 
-    @property
-    def center(self) -> torch.Tensor:
-        return self._bboxes[:, :2]
+class BBoxesCXCYWH(BBoxesCXCY__, BBoxes__WH):
 
     @property
     def left(self) -> torch.Tensor:
         return self.center_x - self.width / 2
 
     @property
     def right(self) -> torch.Tensor:
@@ -513,30 +546,11 @@
     def lt(self) -> torch.Tensor:
         return self.center - self.wh / 2
 
     @property
     def rb(self) -> torch.Tensor:
         return self.center + self.wh / 2
 
-    def _round(self) -> torch.Tensor:
-        lt = self.lt.floor()
-        rb = self.rb.ceil()
-        center = (lt + rb) / 2
-        wh = (rb - lt) / 2
-        return torch.cat([center, wh], dim=-1)
-
-    def _expand(self, ratio_wh: tuple[float, float]) -> torch.Tensor:
-        wh = self.wh * torch.tensor(ratio_wh)
-        return torch.stack([self.center, wh], dim=-1)
-
-    def _clamp(self, image_wh: tuple[int, int]) -> torch.Tensor:
-        lt = self.lt.clamp_min(0)
-        rb = self.rb.clamp_max(torch.tensor(image_wh))
-        center = (lt + rb) / 2
-        wh = (rb - lt) / 2
-        return torch.stack([center, wh], dim=-1)
-
-    def _scale(self, ratio_wh: tuple[float, float]) -> torch.Tensor:
-        w, h = ratio_wh
-        ratio_center = w / 2, h / 2
-        scale = torch.tensor(ratio_center + ratio_wh)
-        return self._bboxes * scale
+    def expand(self, ratio_wh: tuple[float, float]) -> Self:
+        wh = self.wh * self._bboxes.new_tensor(ratio_wh)
+        bboxes = torch.cat([self.center, wh], dim=-1)
+        return self._copy(bboxes)
```

### Comparing `todd_ai-0.4.0/todd/base/registries.py` & `todd_ai-0.5.0/todd/registries/registry.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,423 +1,427 @@
+# pylint: disable=no-value-for-parameter
+
 __all__ = [
+    'Item',
     'RegistryMeta',
     'Registry',
-    'NormRegistry',
-    'LrSchedulerRegistry',
-    'OptimizerRegistry',
-    'RunnerRegistry',
-    'CallbackRegistry',
-    'LossRegistry',
-    'SchedulerRegistry',
-    'VisualRegistry',
-    'HookRegistry',
-    'AccessLayerRegistry',
-    'DatasetRegistry',
-    'StrategyRegistry',
-    'SamplerRegistry',
-    'ModelRegistry',
 ]
 
-import inspect
-import re
 from collections import UserDict
-from typing import Callable, Iterable, NoReturn, TypeVar
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    NoReturn,
+    Protocol,
+    TypeVar,
+    no_type_check,
+)
+
+from ..loggers import logger
+from ..patches.py import NonInstantiableMeta
+from .build_spec import BuildSpec
+
+if TYPE_CHECKING:
+    from ..configs import Config
+
+F = Callable[['Config'], Any]
+
 
-import torch
-import torch.nn as nn
-import torch.utils.data
-import torchvision.transforms as tf
+class Item(Protocol):
+    __name__: str
+    __qualname__: str
 
-from ..utils import NonInstantiableMeta
-from .configs import Config
-from .patches import logger
+    def __call__(self, *args, **kwargs) -> Any:
+        ...
 
-T = TypeVar('T', bound=Callable)
 
+T = TypeVar('T', bound=Item)
 
-class RegistryMeta(UserDict, NonInstantiableMeta):  # type: ignore[misc]
+
+class RegistryMeta(  # type: ignore[misc]
+    UserDict[str, Item],
+    NonInstantiableMeta,
+):
     """Meta class for registries.
 
-    Under the hood, registries are simply dictionaries:
+    Underneath, registries are simply dictionaries:
 
         >>> class Cat(metaclass=RegistryMeta): pass
         >>> class BritishShorthair: pass
         >>> Cat['british shorthair'] = BritishShorthair
         >>> Cat['british shorthair']
         <class '...BritishShorthair'>
 
-    Users can also access registries via higher level APIs, i.e. `register`
-    and `build`, for convenience.
+    In this example, ``Cat`` is a registry and the "british shorthair" is a
+    category in the registry.
+    ``BritishShorthair`` is an object or class that is associated to the
+    "british shorthair" category.
+
+    For convenience, users can also access registries via higher level APIs,
+    such as '`register_`' and '`build`'.
+    These provide easier interfaces to register and retrieve instances:
+
+        >>> class Persian: pass
+        >>> Cat.register_('persian')(Persian)
+        <class '...Persian'>
+        >>> from todd import Config
+        >>> Cat.build(Config(type='persian'))
+        <...Persian object at ...>
 
-    Registries can be subclassed.
-    Derived classes of a registry are child registries:
+    Registries can be subclassed as well to create specializations or child
+    registries:
 
         >>> class HairlessCat(Cat): pass
         >>> Cat.child('HairlessCat')
         <HairlessCat >
+
+    In the example above, ``HairlessCat`` can be seen as a subcategory or
+    specialization of ``Cat``.
+    This allows to organize instances into a hierarchically structured
+    registry.
     """
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(cls, *args, **kwargs) -> None:
         """Initialize."""
-        UserDict.__init__(self)
-        NonInstantiableMeta.__init__(self, *args, **kwargs)
+        UserDict.__init__(cls)
+        NonInstantiableMeta.__init__(cls, *args, **kwargs)
+
+    def __repr__(cls) -> str:
+        items = ' '.join(f'{k}={v}' for k, v in cls.items())
+        return f"<{cls.__name__} {items}>"
+
+    # Inheritance
+
+    @no_type_check
+    def __subclasses__(cls=...) -> Any:
+        """Fetch subclasses of the current class.
+
+        For more details, refer to `ABC subclassed by meta classes`_.
+
+        .. _ABC subclassed by meta classes:
+           https://blog.csdn.net/LutingWang/article/details/128320057
+        """
+        if cls is ...:
+            return NonInstantiableMeta.__subclasses__(RegistryMeta)
+        return super().__subclasses__()
 
-    def __call__(self, *args, **kwargs) -> NoReturn:
-        """Prevent `Registry` classes from being initialized.
+    def child(cls, key: str) -> 'RegistryMeta':
+        """Retrieve a direct or indirect derived child registry.
+
+        Given a dot-separated string of subclass names, this method searches
+        for the specified child registry within its inheritance tree and
+        returns the matching child class.
+
+        Args:
+            key: A string of dot-separated subclass names.
 
         Raises:
-            TypeError: always.
+            ValueError: If no subclass or more than one subclass with the
+                specified name exists.
+
+        Returns:
+            The specified child registry.
         """
-        raise TypeError("Registry cannot be initialized")
+        child = cls
+        for child_name in key.split('.'):
+            subclasses = tuple(child.__subclasses__())  # type: ignore[misc]
+            subclasses = tuple(
+                subclass for subclass in subclasses
+                if subclass.__name__ == child_name
+            )
+            if len(subclasses) == 0:
+                raise ValueError(f"{child_name} is not a child of {child}")
+            if len(subclasses) > 1:
+                raise ValueError(
+                    f"{child_name} matches multiple children of {child}"
+                )
+            child, = subclasses
+        return child
+
+    def _parse(cls, key: str) -> tuple['RegistryMeta', str]:
+        """Parse the ``key`` which may contain child classes separated by dots.
 
-    def __missing__(self, key: str) -> NoReturn:
+        Args:
+            key: the string to be parsed.
+
+        Returns:
+            A tuple containing the child registry object and the updated key
+            string.
+        """
+        if '.' not in key:
+            return cls, key
+        child_name, key = key.rsplit('.', 1)
+        child = cls.child(child_name)
+        return child, key
+
+    # Retrieval
+
+    def __missing__(cls, key: str) -> NoReturn:
         """Missing key.
 
         Args:
             key: the missing key.
 
         Raises:
             KeyError: always.
         """
-        logger.error(f"{key} does not exist in {self.__name__}")
+        logger.error("%s does not exist in %s", key, cls.__name__)
         raise KeyError(key)
 
-    def __repr__(self) -> str:
-        items = ' '.join(f'{k}={v}' for k, v in self.items())
-        return f"<{self.__name__} {items}>"
+    def parse(cls, key: str) -> tuple['RegistryMeta', Item]:
+        """Parse ``key``.
+
+        Returns:
+            The child registry and the corresponding type.
+        """
+        child, key = cls._parse(key)
+        item = super(RegistryMeta, child).__getitem__(key)
+        return child, item
+
+    def __contains__(cls, key) -> bool:
+        if not isinstance(key, str):
+            return False
+        child, key = cls._parse(key)
+        return super(RegistryMeta, child).__contains__(key)
+
+    def __getitem__(cls, key: str) -> Item:
+        _, item = cls.parse(key)
+        return item
+
+    # Registration
 
-    def __setitem__(self, key: str, item, forced: bool = False) -> None:
+    def __setitem__(cls, key: str, item: Item) -> None:
         """Register ``item`` with name ``key``.
 
         Args:
             key: name to be registered as.
             item: object to be registered.
-            forced: if set, ``item`` will always be registered.
-                By default, ``item`` will only be registered if ``key`` is
-                not registered yet.
 
         Raises:
-            KeyError: if ``key`` is already registered and ``forced`` is not
-                set.
+            KeyError: if ``key`` is already registered.
 
-        By default, registries refuse to alter the registered object, in order
-        to prevent unintended name clashes:
+        `RegistryMeta` refuses to alter the registered object, in order to
+        prevent unintended name clashes:
 
             >>> class Cat(metaclass=RegistryMeta): pass
             >>> Cat['british shorthair'] = 'british shorthair'
             >>> Cat['british shorthair'] = 'BritishShorthair'
             Traceback (most recent call last):
                 ...
             KeyError: 'british shorthair'
-
-        Specify the ``forced`` option to force registration:
-
-            >>> Cat.__setitem__(
-            ...     'british shorthair',
-            ...     'BritishShorthair',
-            ...     forced=True,
-            ... )
-            >>> Cat['british shorthair']
-            'BritishShorthair'
         """
-        if not forced and key in self:
-            logger.error(f"{key} already exist in {self.__name__}")
+        if key in cls:  # noqa: E501 pylint: disable=unsupported-membership-test
+            logger.error("%s already exist in %s", key, cls)
             raise KeyError(key)
-        return super().__setitem__(key, item)
-
-    def __subclasses__(
-        self=...,  # type: ignore[assignment]
-    ) -> list['RegistryMeta']:
-        """Refer to `ABC subclassed by meta classes`_.
-
-        Returns:
-            Children registries.
-
-        .. _ABC subclassed by meta classes:
-           https://blog.csdn.net/LutingWang/article/details/128320057
-        """
-        if self is ...:
-            return NonInstantiableMeta.__subclasses__(RegistryMeta)
-        return super().__subclasses__()
-
-    def child(self, key: str) -> 'RegistryMeta':
-        """Get a direct or indirect derived child registry.
-
-        Args:
-            key: dot separated subclass names.
-
-        Raises:
-            ValueError: if zero or multiple children are found.
-
-        Returns:
-            The derived registry.
-        """
-        for child_name in key.split('.'):
-            subclasses = tuple(
-                subclass
-                for subclass in self.__subclasses__()  # type: ignore[misc]
-                if subclass.__name__ == child_name
-            )
-            if len(subclasses) == 0:
-                raise ValueError(f"{key} is not a child of {self}")
-            if len(subclasses) > 1:
-                raise ValueError(f"{key} matches multiple children of {self}")
-            self, = subclasses
-        return self
-
-    def _parse(self, key: str) -> tuple['RegistryMeta', str]:
-        """Parse the child name from the ``key``.
+        child, key = cls._parse(key)
+        super(RegistryMeta, child).__setitem__(key, item)
 
-        Returns:
-            The child registry and the name to be registered.
-        """
-        if '.' not in key:
-            return self, key
-        child_name, key = key.rsplit('.', 1)
-        return self.child(child_name), key
-
-    def register(
-        self,
-        keys: Iterable[str] | None = None,
-        **kwargs,
+    def register_(
+        cls,
+        *args: str,
+        force: bool = False,
+        build_spec: BuildSpec | None = None,
     ) -> Callable[[T], T]:
-        """Register decorator.
+        """Register classes or functions to the registry.
 
         Args:
-            keys: names to be registered as.
-            kwargs: refer to `__setitem__`.
+            args: names to be registered as.
+            force: if set, registration will always happen.
 
         Returns:
             Wrapper function.
 
-        `register` is designed to be an decorator for classes and functions:
+        The decorator can be applied to both classes and functions:
 
             >>> class Cat(metaclass=RegistryMeta): pass
-            >>> @Cat.register()
+            >>> @Cat.register_()
             ... class Munchkin: pass
-            >>> @Cat.register()
+            >>> @Cat.register_()
             ... def munchkin() -> str:
             ...     return 'munchkin'
 
-        `register` has the following advantages:
+        If no arguments are given, the name of the object being registered is
+        used as the key:
 
-        - default name
+            >>> Cat['Munchkin']
+            <class '...Munchkin'>
+            >>> Cat['munchkin']
+            <function munchkin at ...>
+
+        It is possible to register an object with multiple names:
+
+            >>> @Cat.register_('British Longhair', 'british longhair')
+            ... class BritishLonghair: pass
+            >>> 'British Longhair' in Cat
+            True
+            >>> 'british longhair' in Cat
+            True
+
+        It also allows one to specify child registries as part of the key
+        during registration:
+
+            >>> class HairlessCat(Cat): pass
+            >>> @Cat.register_('HairlessCat.CanadianHairless')
+            ... def canadian_hairless() -> str:
+            ...     return 'canadian hairless'
+            >>> HairlessCat
+            <HairlessCat CanadianHairless=<function canadian_hairless at ...>>
 
-          By default, `register` uses the name of the registered object as
-          ``keys``:
+        If 'forced' is True and an item of the same name exists, the new item
+        will replace the old one in the registry:
 
-          >>> Cat['Munchkin']
-          <class '...Munchkin'>
-          >>> Cat['munchkin']
-          <function munchkin at ...>
-
-        - multiple names
-
-          >>> @Cat.register(('British Longhair', 'british longhair'))
-          ... class BritishLonghair: pass
-          >>> 'British Longhair' in Cat
-          True
-          >>> 'british longhair' in Cat
-          True
-
-        - compatibility with child registries
-
-          >>> class HairlessCat(Cat): pass
-          >>> @Cat.register(('HairlessCat.CanadianHairless',))
-          ... def canadian_hairless() -> str:
-          ...     return 'canadian hairless'
-          >>> HairlessCat
-          <HairlessCat CanadianHairless=<function canadian_hairless at ...>>
+            >>> class AnotherMunchkin: pass
+            >>> Cat.register_('Munchkin')(AnotherMunchkin)
+            Traceback (most recent call last):
+                ...
+            KeyError: 'Munchkin'
+            >>> Cat.register_('Munchkin', force=True)(AnotherMunchkin)
+            <class '...AnotherMunchkin'>
+            >>> Cat['Munchkin']
+            <class '...AnotherMunchkin'>
+
+        `BuildSpec` instances can be bind to objects during registration:
+
+            >>> build_spec = BuildSpec()
+            >>> @Cat.register_(build_spec=build_spec)
+            ... class Maine: pass
+            >>> Maine.build_spec is build_spec
+            True
         """
 
-        def wrapper_func(obj: T) -> T:
-            if keys is None:
-                self.__setitem__(obj.__name__, obj, **kwargs)
-            else:
-                for key in keys:
-                    registry, key = self._parse(key)
-                    registry.__setitem__(key, obj, **kwargs)
-            return obj
+        def wrapper_func(item: T) -> T:
+            keys = [item.__name__] if len(args) == 0 else args
+            for key in keys:
+                if force:
+                    cls.pop(key, None)
+                cls[key] = item  # noqa: E501 pylint: disable=unsupported-assignment-operation
+            if build_spec is not None:
+                item.build_spec = build_spec  # type: ignore[attr-defined]
+            return item
 
         return wrapper_func
 
-    def _build(self, config: Config):
+    # Deregistration
+
+    def __delitem__(cls, key: str) -> None:
+        child, key = cls._parse(key)
+        return super(RegistryMeta, child).__delitem__(key)
+
+    # Construction
+
+    def _build(cls, item: Item, config: 'Config') -> Any:
         """Build an instance according to the given config.
 
         Args:
+            item: instance type.
             config: instance specification.
 
         Returns:
             The built instance.
 
         To customize the build process of instances, registries must overload
         `_build` with a class method:
 
+            >>> from todd import Config
             >>> class Cat(metaclass=RegistryMeta):
             ...     @classmethod
-            ...     def _build(cls, config: Config) -> str:
-            ...         obj = RegistryMeta._build(cls, config)
-            ...         return obj.__class__.__name__.upper()
-            >>> @Cat.register()
-            ... class Munchkin: pass
-            >>> Cat.build(Config(type='Munchkin'))
-            'MUNCHKIN'
+            ...     def _build(cls, item: Item, config: Config):
+            ...         obj = RegistryMeta._build(cls, item, config)
+            ...         obj.name = obj.name.upper()
+            ...         return obj
+            >>> @Cat.register_()
+            ... class Munchkin:
+            ...     def __init__(self, name: str) -> None:
+            ...         self.name = name
+            >>> config = Config(type='Munchkin', name='Garfield')
+            >>> cat = Cat.build(config)
+            >>> cat.name
+            'GARFIELD'
         """
-        type_ = self[config.pop('type')]
-        return type_(**config)
+        return item(**config)
 
-    def build(self, config: Config, **kwargs):
+    def build(cls, config: 'Config', **kwargs) -> Any:
         """Call the registered object to construct a new instance.
 
         Args:
             config: build parameters.
             kwargs: default configuration.
 
         Returns:
             The built instance.
 
-        If the registered object is callable, the `build` method will
-        automatically call the objects:
+        The ``type`` entry of ``config`` specifies the name of the registered
+        object to be built.
+        The other entries of ``config`` will be passed to the object's call
+        method.
 
             >>> class Cat(metaclass=RegistryMeta): pass
-            >>> @Cat.register()
+            >>> @Cat.register_()
             ... def tabby(name: str) -> str:
             ...     return f'Tabby {name}'
+            >>> from todd import Config
             >>> Cat.build(Config(type='tabby', name='Garfield'))
             'Tabby Garfield'
 
-        Typically, ``config`` is a `Mapping` object.
-        The ``type`` entry of ``config`` specifies the name of the registered
-        object to be built.
-        The other entries of ``config`` will be passed to the object's call
-        method.
-
         Keyword arguments are the default configuration:
 
             >>> Cat.build(
             ...     Config(type='tabby'),
             ...     name='Garfield',
             ... )
             'Tabby Garfield'
 
-        Refer to `_build` for customizations.
+        Override :meth:`_build` for customization:
+
+            >>> class DomesticCat(Cat):
+            ...     @classmethod
+            ...     def _build(cls, item: Item, config: Config):
+            ...         return item, config
+            >>> @DomesticCat.register_()
+            ... class Maine: pass
+            >>> DomesticCat.build(Config(type='Maine', name='maine'), age=1.2)
+            (<class '...Maine'>, {'age': 1.2, 'name': 'maine'})
+
+        If the object has a property named ``build_spec``, the config is
+        converted before construction:
+
+            >>> from ..patches.py import classproperty
+            >>> @Cat.register_()
+            ... class Persian:
+            ...     def __init__(self, friend: str) -> None:
+            ...         self.friend = friend
+            ...     @classproperty
+            ...     def build_spec(self) -> BuildSpec:
+            ...         return BuildSpec(friend=lambda config: config.type)
+            >>> persian = Cat.build(
+            ...     Config(type='Persian'),
+            ...     friend=dict(type='Siamese'),
+            ... )
+            >>> persian.friend
+            'Siamese'
         """
-        default_config = Config(kwargs)
-        default_config.update(config)
+        from ..configs import Config, PyConfig
+        config = Config(kwargs) | config
+        py_config = PyConfig(config)
+
+        config_type = config.pop('type')
+        registry, item = cls.parse(config_type)
 
-        config = default_config.copy()
-        registry, config.type = self._parse(config.type)
+        if (build_spec := getattr(item, 'build_spec', None)) is not None:
+            config = build_spec(config)
 
         try:
-            return registry._build(config)
+            return registry._build(item, config)
         except Exception as e:
             # config may be altered
-            logger.error(f"Failed to build\n{default_config.dumps()}")
+            logger.error("Failed to build\n%s", py_config.dumps())
             raise e
 
 
 class Registry(metaclass=RegistryMeta):
     """Base registry.
 
     To create custom registry, inherit from the `Registry` class:
 
         >>> class CatRegistry(Registry): pass
     """
-
-
-class NormRegistry(Registry):
-    pass
-
-
-class OptimizerRegistry(Registry):
-
-    @staticmethod
-    def params(model: nn.Module, config: Config) -> Config:
-        config.params = [
-            p for n, p in model.named_parameters()
-            if re.match(config.params, n)
-        ]
-        return config
-
-    @classmethod
-    def _build(cls, config: Config) -> torch.optim.Optimizer:
-        model: nn.Module = config.pop('model')
-        params: Iterable[Config] | None = config.pop('params', None)
-        config.params = model.parameters() if params is None else [
-            cls.params(model, p) for p in params
-        ]
-        return RegistryMeta._build(cls, config)
-
-
-class LrSchedulerRegistry(Registry):
-    pass
-
-
-class RunnerRegistry(Registry):
-    pass
-
-
-class CallbackRegistry(Registry):
-    pass
-
-
-class LossRegistry(Registry):
-    pass
-
-
-class SchedulerRegistry(Registry):
-    pass
-
-
-class VisualRegistry(Registry):
-    pass
-
-
-class HookRegistry(Registry):
-    pass
-
-
-class DatasetRegistry(Registry):
-    pass
-
-
-class AccessLayerRegistry(Registry):
-    pass
-
-
-class StrategyRegistry(Registry):
-    pass
-
-
-class SamplerRegistry(Registry):
-    pass
-
-
-class ModelRegistry(Registry):
-    pass
-
-
-class TransformRegistry(Registry):
-    pass
-
-
-for c in torch.utils.data.Sampler.__subclasses__():
-    SamplerRegistry.register()(c)
-
-for c in torch.optim.Optimizer.__subclasses__():
-    OptimizerRegistry.register()(c)
-
-for c in torch.optim.lr_scheduler.LRScheduler.__subclasses__():
-    LrSchedulerRegistry.register()(c)
-
-NormRegistry['BN1d'] = nn.BatchNorm1d
-NormRegistry['BN2d'] = NormRegistry['BN'] = nn.BatchNorm2d
-NormRegistry['BN3d'] = nn.BatchNorm3d
-NormRegistry['SyncBN'] = nn.SyncBatchNorm
-NormRegistry['GN'] = nn.GroupNorm
-NormRegistry['LN'] = nn.LayerNorm
-NormRegistry['IN1d'] = nn.InstanceNorm1d
-NormRegistry['IN2d'] = NormRegistry['IN'] = nn.InstanceNorm2d
-NormRegistry['IN3d'] = nn.InstanceNorm3d
-
-for _, c in inspect.getmembers(tf, inspect.isclass):
-    TransformRegistry.register()(c)
```

### Comparing `todd_ai-0.4.0/todd/base/stores.py` & `todd_ai-0.5.0/todd/utils/stores.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,19 +2,18 @@
     'StoreMeta',
     'Store',
 ]
 
 import os
 
 import torch
-import torch.distributed
 from packaging.version import parse
 
-from ..utils import NonInstantiableMeta
-from .patches import logger
+from ..loggers import logger
+from ..patches.py import NonInstantiableMeta
 
 
 class StoreMeta(NonInstantiableMeta):
     """Stores for global variables.
 
     Stores provide an interface to access global variables:
 
@@ -64,61 +63,62 @@
     Assignments to those variables will not trigger exceptions, but will not
     take effect:
 
         >>> EnvStore.ENV_INT = 3
         >>> EnvStore.ENV_INT
         2
     """
+
     _read_only: dict[str, bool] = dict()
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(cls, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
-        if keys := self.__annotations__.keys() & self._read_only:
+        if keys := cls.__annotations__.keys() & cls._read_only:
             raise TypeError(f"Duplicated {keys=}")
 
-        for k, v in self.__annotations__.items():
+        for k, v in cls.__annotations__.items():
             variable = os.environ.get(k, '')
             if read_only := variable != '':
                 if v is not str:
-                    variable = eval(variable)
+                    variable = eval(variable)  # nosec B307
                     assert isinstance(variable, v)
                 super().__setattr__(k, variable)
-            self._read_only[k] = read_only
+            cls._read_only[k] = read_only
 
-    def __getattr__(self, name: str) -> None:
-        if name in self.__annotations__:
-            return self.__annotations__[name]()
+    def __getattr__(cls, name: str) -> None:
+        if name in cls.__annotations__:
+            return cls.__annotations__[name]()
         raise AttributeError(name)
 
-    def __setattr__(self, name: str, value) -> None:
-        if name in self.__annotations__ and self._read_only.get(name, False):
-            logger.debug(f"Cannot set {name} to {value}.")
+    def __setattr__(cls, name: str, value) -> None:
+        if name in cls.__annotations__ and cls._read_only.get(name, False):
+            logger.debug("Cannot set %s to %s.", name, value)
             return
         super().__setattr__(name, value)
 
-    def __repr__(self) -> str:
+    def __repr__(cls) -> str:
         variables = ' '.join(
-            f'{k}={getattr(self, k)}' for k in self.__annotations__
+            f'{k}={getattr(cls, k)}' for k in cls.__annotations__
         )
-        return f"<{self.__name__} {variables}>"
+        return f"<{cls.__name__} {variables}>"
 
 
 class Store(metaclass=StoreMeta):
     CPU: bool
 
     CUDA: bool = torch.cuda.is_available()
     MPS: bool
 
     DRY_RUN: bool
     TRAIN_WITH_VAL_DATASET: bool
 
 
 if parse(torch.__version__) >= parse('1.12'):
-    import torch.backends.mps as mps
+    from torch.backends import mps
     if mps.is_available():
         Store.MPS = True
 
 if not Store.CUDA and not Store.MPS:
     Store.CPU = True
 
 assert Store.CPU or Store.CUDA or Store.MPS
```

### Comparing `todd_ai-0.4.0/todd/datasets/folder.py` & `todd_ai-0.5.0/todd/colors/yiq.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 __all__ = [
-    'FolderAccessLayer',
+    'YIQ',
 ]
 
-import pathlib
-from typing import Iterator, TypeVar
+from colorsys import rgb_to_yiq, yiq_to_rgb
+from typing_extensions import Self
 
-from ..base import Config
-from .base import BaseAccessLayer
+from .color import Color
+from .rgba import RGBA
 
-KT = TypeVar('KT')
-VT = TypeVar('VT')
 
-
-class FolderAccessLayer(BaseAccessLayer[str, VT]):
+class YIQ(Color):
 
     def __init__(
         self,
-        *args,
-        folder_root: Config | None = None,
-        **kwargs,
+        luminance: float,
+        in_phase: float,
+        quadrature: float,
     ) -> None:
-        super().__init__(*args, **kwargs)
-        if folder_root is None:
-            folder_root = Config()
-        self._build_folder_root(folder_root)
-
-    def _build_folder_root(self, config: Config) -> None:
-        self._folder_root = pathlib.Path(self._data_root) / self._task_name
+        self._luminance = self._normalize(luminance)
+        self._in_phase = self._normalize(in_phase)
+        self._quadrature = self._normalize(quadrature)
+
+    def __repr__(self) -> str:
+        return (
+            f"{type(self).__name__}({self._luminance}, {self._in_phase}, "
+            f"{self._quadrature})"
+        )
 
     @property
-    def exists(self) -> bool:
-        return self._folder_root.exists()
-
-    def touch(self) -> None:
-        self._folder_root.mkdir(parents=True, exist_ok=True)
+    def luminance(self) -> float:
+        return self._luminance
 
-    def _files(self) -> Iterator[pathlib.Path]:
-        return (path for path in self._folder_root.iterdir() if path.is_file())
-
-    def _file(self, key: str) -> pathlib.Path:
-        return self._folder_root / key
+    @property
+    def in_phase(self) -> float:
+        return self._in_phase
 
-    def __iter__(self) -> Iterator[str]:
-        return (path.name for path in self._files())
+    @property
+    def quadrature(self) -> float:
+        return self._quadrature
 
-    def __len__(self) -> int:
-        return len(list(self._files()))
+    @classmethod
+    def _from(cls, rgba: RGBA) -> Self:
+        r, g, b, *_ = rgba.to_tuple()
+        y, i, q = rgb_to_yiq(r, g, b)
+        return cls(y, i, q)
+
+    def _to(self) -> RGBA:
+        r, g, b = yiq_to_rgb(*self._to_tuple())
+        return RGBA(r, g, b, alpha=1.)
 
-    def __delitem__(self, key: str) -> None:
-        self._file(key).unlink()
+    def _to_tuple(self) -> tuple[float, ...]:
+        return self._luminance, self._in_phase, self._quadrature
```

### Comparing `todd_ai-0.4.0/todd/datasets/lmdb.py` & `todd_ai-0.5.0/todd/datasets/lmdb.py`

 * *Files identical despite different names*

### Comparing `todd_ai-0.4.0/todd/datasets/zip.py` & `todd_ai-0.5.0/todd/datasets/zip.py`

 * *Files identical despite different names*

### Comparing `todd_ai-0.4.0/todd/losses/ckd.py` & `todd_ai-0.5.0/todd/tasks/object_detection_knowledge_distillation/losses/ckd.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,26 +3,27 @@
     'CKDLoss',
 ]
 
 import torch
 import torch.distributed as dist
 import torch.nn.functional as F
 
-from ..base import BBoxesXYXY, LossRegistry
-from ..utils import get_rank, get_world_size
-from .base import BaseLoss
+from ....models import LossRegistry
+from ....models.losses import BaseLoss
+from ....patches.torch import get_rank, get_world_size
+from ...object_detection import BBoxesXYXY
 
 
 def ckd_loss(
     pred: torch.Tensor,
     target: torch.Tensor,
     ignore: tuple[torch.Tensor, torch.Tensor] | None = None,
     gamma: float = 0.07,
 ) -> torch.Tensor:
-    """Wrapper of CKD loss.
+    """Compute the CKD loss.
 
     Refer to http://arxiv.org/abs/2108.07482.
 
     Args:
         pred: n x dim
             Normalized predictions.
 
@@ -75,26 +76,26 @@
             self._memory.pop(-1)
 
     @property
     def memory(self) -> torch.Tensor:
         return torch.cat(self._memory)
 
 
-@LossRegistry.register()
+@LossRegistry.register_()
 class CKDLoss(BaseLoss):
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self._memory_pool = MemoryPool()
 
-    def forward(
+    def forward(  # pylint: disable=arguments-differ
         self,
         preds: torch.Tensor,
         targets: torch.Tensor,
-        bboxes: list[torch.Tensor] | None = None,
+        bboxes: list[torch.Tensor] | None = None,  # TODO: change to BBoxes
     ) -> torch.Tensor:
         """Compute CKD loss.
 
         Refer to http://arxiv.org/abs/2108.07482.
 
         Args:
             preds: m x dim
```

### Comparing `todd_ai-0.4.0/todd/losses/functional.py` & `todd_ai-0.5.0/todd/runners/trainer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,103 +1,70 @@
 __all__ = [
-    'L1Loss',
-    'MSELoss',
-    'BCELoss',
-    'BCEWithLogitsLoss',
-    'CrossEntropyLoss',
+    'Trainer',
 ]
 
-from abc import abstractmethod
+from abc import ABC
+from typing import Any, Mapping, TypeVar
 
 import torch
-import torch.nn.functional as F
+from torch import nn
 
-from ..base import LossRegistry
-from .base import BaseLoss
+from ..configs import Config
+from ..registries import RunnerRegistry
+from .base import BaseRunner
+from .memo import Memo
 
+T = TypeVar('T', bound=nn.Module)
 
-class FunctionalLoss(BaseLoss):
 
-    @staticmethod
-    @abstractmethod
-    def func(*args, **kwargs) -> torch.Tensor:
-        pass
+@RunnerRegistry.register_()
+class Trainer(BaseRunner[T], ABC):
 
-    def forward(
+    @property
+    def iters_per_epoch(self) -> int:
+        return len(self._dataloader)
+
+    @property
+    def inner_iter(self) -> int:
+        return self._iter % self.iters_per_epoch
+
+    @property
+    def epoch(self) -> int:
+        return self._iter // self.iters_per_epoch
+
+    @property
+    def optimizer(self) -> torch.optim.Optimizer:
+        return self._optimizer
+
+    def _build_optimizer(
         self,
-        pred: torch.Tensor,
-        target: torch.Tensor,
-        mask: torch.Tensor | None = None,
         *args,
+        optimizer: Config,
         **kwargs,
-    ) -> torch.Tensor:
-        if mask is None:
-            loss = self.func(
-                pred,
-                target,
-                *args,
-                reduction=self.reduction,
-                **kwargs,
-            )
-        else:
-            loss = self.func(pred, target, *args, reduction='none', **kwargs)
-            loss = self.reduce(loss, mask)
-        return loss
-
-
-class NormMixin(FunctionalLoss):
-
-    def __init__(self, *args, norm: bool = False, **kwargs):
-        super().__init__(*args, **kwargs)
-        self._norm = norm
+    ) -> None:
+        self._optimizer = self._strategy.build_optimizer(optimizer)
+
+    def _build(self, *args, **kwargs) -> None:
+        super()._build(*args, **kwargs)
+        self._build_optimizer(*args, **kwargs)
+
+    def _setup(self) -> Memo:
+        self._model.train()
+        return super()._setup()
+
+    def state_dict(self, *args, **kwargs) -> dict[str, Any]:
+        state_dict = super().state_dict(*args, **kwargs)
+        state_dict['optim'] = self._strategy.optim_state_dict(*args, **kwargs)
+        return state_dict
 
-    def forward(
+    def load_state_dict(
         self,
-        pred: torch.Tensor,
-        target: torch.Tensor,
+        state_dict: Mapping[str, Any],
         *args,
         **kwargs,
-    ) -> torch.Tensor:
-        if self._norm:
-            pred = F.normalize(pred)
-            target = F.normalize(target)
-        return super().forward(pred, target, *args, **kwargs)
-
-
-@LossRegistry.register()
-class L1Loss(NormMixin, FunctionalLoss):
-
-    @staticmethod
-    def func(*args, **kwargs) -> torch.Tensor:
-        return F.l1_loss(*args, **kwargs)
-
-
-@LossRegistry.register()
-class MSELoss(NormMixin, FunctionalLoss):
-
-    @staticmethod
-    def func(*args, **kwargs) -> torch.Tensor:
-        return F.mse_loss(*args, **kwargs)
-
-
-@LossRegistry.register()
-class BCELoss(FunctionalLoss):
-
-    @staticmethod
-    def func(*args, **kwargs) -> torch.Tensor:
-        return F.binary_cross_entropy(*args, **kwargs)
-
-
-@LossRegistry.register()
-class BCEWithLogitsLoss(FunctionalLoss):
-
-    @staticmethod
-    def func(*args, **kwargs) -> torch.Tensor:
-        return F.binary_cross_entropy_with_logits(*args, **kwargs)
-
-
-@LossRegistry.register()
-class CrossEntropyLoss(FunctionalLoss):
-
-    @staticmethod
-    def func(*args, **kwargs) -> torch.Tensor:
-        return F.cross_entropy(*args, **kwargs)
+    ) -> None:
+        super().load_state_dict(state_dict, *args, **kwargs)
+        self._strategy.load_optim_state_dict(
+            state_dict['optim'],
+            *args,
+            **kwargs,
+        )
```

### Comparing `todd_ai-0.4.0/todd/losses/mimic.py` & `todd_ai-0.5.0/todd/tasks/knowledge_distillation/losses/mimic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,100 +1,107 @@
 __all__ = [
     'L12DLoss',
     'MSE2DLoss',
     'FGDLoss',
     'FGFILoss',
 ]
 
+from abc import ABC
+
 import einops
 import torch
 import torch.nn.functional as F
 
-from ..base import LossRegistry
-from .functional import FunctionalLoss, L1Loss, MSELoss
+from ....models import LossRegistry
+from ....models.losses import FunctionalLoss, L1Loss, MSELoss
 
 
-class _2DMixin(FunctionalLoss):
+class _2DMixin(FunctionalLoss, ABC):  # noqa: N801
 
     def forward(
         self,
         pred: torch.Tensor,
         target: torch.Tensor,
-        mask: torch.Tensor | None = None,
         *args,
+        mask: torch.Tensor | None = None,
         **kwargs,
     ) -> torch.Tensor:
         _, _, h, w = pred.shape
         if pred.shape != target.shape:
             target = F.adaptive_avg_pool2d(target, (h, w))
         if mask is not None and pred.shape != mask.shape:
             mask = F.adaptive_avg_pool2d(mask, (h, w))
-        return super().forward(pred, target, mask, *args, **kwargs)
+        return super().forward(pred, target, *args, mask=mask, **kwargs)
 
 
-@LossRegistry.register()
+@LossRegistry.register_()
 class L12DLoss(_2DMixin, L1Loss):
     pass
 
 
-@LossRegistry.register()
+@LossRegistry.register_()
 class MSE2DLoss(_2DMixin, MSELoss):
     pass
 
 
-@LossRegistry.register()
+@LossRegistry.register_()
 class FGFILoss(MSE2DLoss):
 
-    def forward(  # type: ignore[override]
+    def forward(
         self,
         pred: torch.Tensor,
         target: torch.Tensor,
-        mask: torch.Tensor,
         *args,
+        mask: torch.Tensor | None = None,
         **kwargs,
     ) -> torch.Tensor:
+        assert mask is not None
         n, _, h, w = pred.shape
         target = F.adaptive_avg_pool2d(target, (h, w))
         assert mask.shape == (n, 1, h, w) and mask.dtype == torch.bool
 
         pred = einops.rearrange(pred, 'n c h w -> n h w c')
         target = einops.rearrange(target, 'n c h w -> n h w c')
         mask = einops.rearrange(mask, 'n 1 h w -> n h w')
 
         return super().forward(  # type: ignore[misc]
             pred[mask],
             target[mask],
-            mask=None,
             *args,
+            mask=None,
             **kwargs,
         )
 
 
-@LossRegistry.register()
+@LossRegistry.register_()
 class FGDLoss(MSE2DLoss):
 
-    def forward(  # type: ignore[override]
+    def forward(
         self,
         pred: torch.Tensor,
         target: torch.Tensor,
-        attn_spatial: torch.Tensor,
-        attn_channel: torch.Tensor,
-        mask: torch.Tensor,
         *args,
+        mask: torch.Tensor | None = None,
+        attn_spatial: torch.Tensor | None = None,
+        attn_channel: torch.Tensor | None = None,
         **kwargs,
     ) -> torch.Tensor:
+        assert (
+            mask is not None and attn_spatial is not None
+            and attn_channel is not None
+        )
         _, _, h, w = pred.shape
         attn_spatial = F.adaptive_avg_pool2d(attn_spatial, (h, w))
         attn_channel = F.adaptive_avg_pool2d(attn_channel, (h, w))
         mask = attn_spatial * attn_channel * mask
         return super().forward(  # type: ignore[misc]
             pred,
             target,
-            mask=mask,
             *args,
+            mask=mask,
             **kwargs,
         )
 
 
 # @LOSSES.register()
 # class LabelEncLoss(MSE2DLoss):
```

### Comparing `todd_ai-0.4.0/todd/losses/rcnn.py` & `todd_ai-0.5.0/todd/tasks/object_detection_knowledge_distillation/losses/rcnn.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,46 +2,47 @@
     'SGFILoss',
 ]
 
 from typing import Callable
 
 import einops
 import torch
-import torch.nn as nn
 import torch.nn.functional as F
+from torch import nn
 
-from ..base import LossRegistry
-from .functional import MSELoss
+from ....models import LossRegistry
+from ....models.losses import MSELoss
 
 
-@LossRegistry.register()
+@LossRegistry.register_()
 class SGFILoss(MSELoss):
 
     def __init__(
         self,
         *args,
         in_channels: int = 256,
         hidden_channels: int = 128,
         out_channels: int = 64,
         **kwargs,
-    ):
+    ) -> None:
         from mmcv.cnn import ConvModule
 
         super().__init__(*args, **kwargs)
         self._embed: Callable[..., torch.Tensor] = nn.Sequential(
             ConvModule(in_channels, hidden_channels, 3, stride=2),
             ConvModule(hidden_channels, out_channels, 3, stride=2)
         )
         self._tau = nn.Parameter(torch.tensor([1.0], dtype=torch.float32))
 
-    def forward(  # type: ignore[override]
+    def forward(
         self,
-        preds: list[torch.Tensor],
-        targets: torch.Tensor,
+        pred: torch.Tensor,
+        target: torch.Tensor,
         *args,
+        mask: torch.Tensor | None = None,
         **kwargs,
     ):
         """Re-implementation of G-DetKD.
 
         Refer to http://arxiv.org/abs/2108.07482.
 
         Args:
@@ -50,41 +51,40 @@
                 Typical shape is 4 x 1024 x 256 x 7 x 7.
 
             target: r x c x h x w
 
         Returns:
             loss
         """
-        fused_preds = torch.stack(preds)
-        embed_pred = einops.rearrange(fused_preds, 'l r c h w -> (l r) c h w')
+        embed_pred = einops.rearrange(pred, 'l r c h w -> (l r) c h w')
         embed_pred = self._embed(embed_pred)
-        embed_target = self._embed(targets)
+        embed_target = self._embed(target)
 
         embed_pred = einops.rearrange(
             embed_pred,
             '(l r) out_channels 1 1 -> l r out_channels',
-            l=len(preds),
+            l=pred.shape[0],
         )
         embed_target = einops.rearrange(
             embed_target,
             'r out_channels 1 1 -> r out_channels',
         )
         similarity = torch.einsum(
             'l r c, r c -> l r',
             embed_pred,
             embed_target,
         )
         similarity = F.softmax(similarity / self._tau, dim=1)
 
         fused_pred = torch.einsum(
             'l r c h w, l r -> r c h w',
-            fused_preds,
+            pred,
             similarity,
         )
-        return super().forward(fused_pred, targets, *args, **kwargs)
+        return super().forward(fused_pred, target, *args, mask=mask, **kwargs)
 
 
 # @LOSSES.register()
 # class DevRCNNLoss(MSELoss):
 #     def __init__(
 #         self,
 #         *args,
```

### Comparing `todd_ai-0.4.0/todd/losses/schedulers.py` & `todd_ai-0.5.0/todd/models/losses/schedulers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,105 +1,99 @@
 __all__ = [
     'BaseScheduler',
-    'ConstantScheduler',
     'WarmupScheduler',
     'EarlyStopScheduler',
+    'DeferScheduler',
     'DecayScheduler',
     'StepScheduler',
     'CosineAnnealingScheduler',
+    'ComposedScheduler',
     'ChainedScheduler',
+    'SequentialScheduler',
 ]
 
 import bisect
 import math
-from abc import ABC, abstractmethod
-from typing import Iterable
+from typing import Iterable, cast
 
 import torch
+from torch import nn
 
-from ..base import SchedulerRegistry
+from ...patches.py import classproperty
+from ...registries import BuildSpec, BuildSpecMixin
+from .registries import SchedulerRegistry
 
 
-class BaseScheduler(torch.nn.Module, ABC):
+@SchedulerRegistry.register_()
+class BaseScheduler(nn.Module):
     """Base class for schedulers.
 
     Under most cases, schedulers are used as a variable loss weight.
     Schedulers are functions of `steps`, which could mean iterations or
     epochs.
     Users could increment `steps` by calling `step`, or directly set the
     `steps` property.
     Call the scheduler to get the value for the current step.
 
     .. note:: `steps` starts from 1, so `step` should be called after the
         first step.
+
+    The value of this scheduler is always the `gain`:
+
+        >>> base_scheduler = BaseScheduler(gain=5)
+        >>> base_scheduler()
+        5.0
+        >>> base_scheduler.step()
+        >>> base_scheduler()
+        5.0
     """
 
-    def __init__(self, gain: float = 1.0) -> None:
+    def __init__(self, *args, gain: float = 1.0, **kwargs) -> None:
         """Initialize.
 
         Args:
             gain: multiplier to the scheduler value.
         """
-        super().__init__()
+        super().__init__(*args, **kwargs)
         self._gain = gain
-        self.register_forward_hook(forward_hook)
+        self.register_forward_hook(lambda m, i, o: self._scale(o))
         self.register_buffer('_steps', torch.tensor(1))
 
     @property
     def gain(self) -> float:
         return self._gain
 
     @property
     def steps(self) -> int:
-        return self._steps.item()
+        return cast(int, self._steps.item())
 
     @steps.setter
     def steps(self, value: int) -> None:
         self._steps = torch.tensor(value)
 
     def step(self) -> None:
         self._steps += 1
 
-    @abstractmethod
+    def _scale(self, output: float) -> float:
+        return output * self.gain
+
     def forward(self) -> float:
-        """The scheduler's function.
+        """Compute the current schedule weight.
 
         Returns:
             The scheduler's value for the current step, before multiplying
             `gain`.
 
         Since `gain` is handled by this base class, it is usually adequate for
         `forward` to return a percentage value in :math:`[0, 1]`.
         """
-        pass
-
-
-def forward_hook(module: BaseScheduler, input_, output: float) -> float:
-    return output * module.gain
-
-
-@SchedulerRegistry.register()
-class ConstantScheduler(BaseScheduler):
-    """Unvarying scheduler.
-
-    The value of this scheduler is always the `gain`:
-
-        >>> constant = ConstantScheduler(5)
-        >>> constant()
-        5.0
-        >>> constant.step()
-        >>> constant()
-        5.0
-    """
-
-    def forward(self) -> float:
         return 1.0
 
 
-@SchedulerRegistry.register()
+@SchedulerRegistry.register_()
 class WarmupScheduler(BaseScheduler):
     """Warmup scheduler.
 
     The value will linearly increase from 0 to 1.
     At step ``end``, the value is 1.
 
         >>> warmup = WarmupScheduler(end=5)
@@ -119,15 +113,15 @@
         super().__init__(*args, **kwargs)
         self._end = end
 
     def forward(self) -> float:
         return min(self.steps / self._end, 1.0)
 
 
-@SchedulerRegistry.register()
+@SchedulerRegistry.register_()
 class EarlyStopScheduler(BaseScheduler):
     """Early stop.
 
     At some point, the value drops to 0 from 1.
 
         >>> early_stop = EarlyStopScheduler(at=3)
         >>> for _ in range(5):
@@ -144,15 +138,26 @@
         super().__init__(*args, **kwargs)
         self._at = at
 
     def forward(self) -> float:
         return float(self.steps < self._at)
 
 
-@SchedulerRegistry.register()
+@SchedulerRegistry.register_()
+class DeferScheduler(BaseScheduler):
+
+    def __init__(self, *args, to: int, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+        self._to = to
+
+    def forward(self) -> float:
+        return float(self.steps >= self._to)
+
+
+@SchedulerRegistry.register_()
 class DecayScheduler(BaseScheduler):
     """Decay scheduler.
 
     Before or at ``start``, the value is 1.
     After or at ``end``, the value is 0.
     In between, the value is interpolated.
 
@@ -179,15 +184,15 @@
         if self.steps <= self._start:
             return 1.0
         if self.steps >= self._end:
             return 0.0
         return (self._end - self.steps) / (self._end - self._start)
 
 
-@SchedulerRegistry.register()
+@SchedulerRegistry.register_()
 class StepScheduler(BaseScheduler):
     """Step scheduler.
 
     The value is multiplied by :math:`gamma` at every milestone:
 
         >>> step = StepScheduler(milestones=[3, 4], gamma=0.1)
         >>> for _ in range(5):
@@ -211,15 +216,15 @@
         self._milestones = sorted(milestones)
         self._gamma = gamma
 
     def forward(self) -> float:
         return self._gamma**bisect.bisect(self._milestones, self.steps)
 
 
-@SchedulerRegistry.register()
+@SchedulerRegistry.register_()
 class CosineAnnealingScheduler(BaseScheduler):
     """Cosine annealing scheduler.
 
     The value anneals as the cosine function is defined.
     The first step starts with 1.
     After ``duration`` steps, the value becomes 0.
     The best practice is to set ``duration`` to the total number of steps.
@@ -232,27 +237,54 @@
         0.904508
         0.654508
         0.345492
         0.095492
         0.0
     """
 
-    def __init__(self, *args, duration: int, **kwargs) -> None:
+    def __init__(
+        self,
+        *args,
+        duration: int,
+        min_: float = 0.,
+        **kwargs,
+    ) -> None:
         super().__init__(*args, **kwargs)
         self._duration = duration
+        self._min = min_
 
     def forward(self) -> float:
         steps = self.steps - 1
         if steps >= self._duration:
             return 0
-        return (1 + math.cos(math.pi * steps / self._duration)) / 2
+        return (
+            self._min + (1 - self._min) *
+            (1 + math.cos(math.pi * steps / self._duration)) / 2
+        )
+
 
+class ComposedScheduler(BuildSpecMixin, BaseScheduler):
 
-@SchedulerRegistry.register()
-class ChainedScheduler(BaseScheduler):
+    def __init__(
+        self,
+        *args,
+        schedulers: Iterable[BaseScheduler],
+        **kwargs,
+    ) -> None:
+        super().__init__(*args, **kwargs)
+        self._schedulers = tuple(schedulers)
+
+    @classproperty
+    def build_spec(self) -> BuildSpec:
+        build_spec = BuildSpec({'*schedulers': SchedulerRegistry.build})
+        return super().build_spec | build_spec
+
+
+@SchedulerRegistry.register_()
+class ChainedScheduler(ComposedScheduler):
     """Chained scheduler.
 
     Schedulers are chained in an multiplicative manner:
 
         >>> warmup = WarmupScheduler(end=5, gain=10)
         >>> step = StepScheduler(milestones=[3, 4], gamma=0.1)
         >>> chained = ChainedScheduler(schedulers=[warmup, step])
@@ -262,23 +294,39 @@
         2.0
         4.0
         0.6
         0.08
         0.1
     """
 
+    def forward(self) -> float:
+        return math.prod(scheduler() for scheduler in self._schedulers)
+
+    def step(self) -> None:
+        super().step()
+        for scheduler in self._schedulers:
+            scheduler.step()
+
+
+@SchedulerRegistry.register_()
+class SequentialScheduler(ComposedScheduler):
+
     def __init__(
         self,
         *args,
-        schedulers: Iterable[BaseScheduler],
+        milestones: Iterable[int],
         **kwargs,
     ) -> None:
         super().__init__(*args, **kwargs)
-        self._schedulers = tuple(schedulers)
+        self._milestones = sorted(milestones)
+
+    @property
+    def scheduler(self) -> BaseScheduler:
+        i = bisect.bisect(self._milestones, self.steps)
+        return self._schedulers[i]
 
     def forward(self) -> float:
-        return math.prod(scheduler() for scheduler in self._schedulers)
+        return self.scheduler()
 
     def step(self) -> None:
+        self.scheduler.step()
         super().step()
-        for scheduler in self._schedulers:
-            scheduler.step()
```

### Comparing `todd_ai-0.4.0/todd/reproduction/model.py` & `todd_ai-0.5.0/todd/models/frozens.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,423 +1,406 @@
 __all__ = [
-    'Finder',
-    'ParameterFinder',
-    'ModuleFinder',
+    'CheckMixin',
+    'NoGradMixin',
+    'EvalMixin',
+    'FreezeMixin',
     'FrozenMixin',
-    'state_dict_hook',
 ]
 
-import re
-import types
-from typing import Any, Generic, Iterable, MutableMapping, TypeVar
+from abc import ABC, abstractmethod
+from typing import Any, Iterable, MutableMapping
 from typing_extensions import Self
 
-import torch.nn as nn
+import torch
+from torch import nn
 
-from ..base import Config, get_
+from ..configs import Config
+from ..patches.py import classproperty
+from ..registries import BuildSpec, BuildSpecMixin, InitWeightsMixin
+from ..utils import Store
+from .filters import NamedModulesFilter, NamedParametersFilter
+from .registries import FilterRegistry
+
+
+class CheckMixin(nn.Module, ABC):
+    """Mixin to perform a check before the first forward pass of a module.
+
+    You should implement `check` in your subclass:
+
+        >>> class Model(CheckMixin):
+        ...     def check(
+        ...         self,
+        ...         module: nn.Module,
+        ...         args: tuple[Any],
+        ...         kwargs: dict[str, Any],
+        ...     ) -> None:
+        ...         print(
+        ...             f"Checking {repr(module.__class__.__name__)} with "
+        ...             f"{args=} and {kwargs=}"
+        ...         )
+        ...     def forward(self, *args, **kwargs) -> None:
+        ...         print(f"Forwarding with {args=} and {kwargs=}")
 
-T = TypeVar('T')
+    The `check` method executes prior to ``__call__``:
 
+        >>> model = Model()
+        >>> model(1, 2, a=3, b=4)
+        Checking 'Model' with args=(1, 2) and kwargs={'a': 3, 'b': 4}
+        Forwarding with args=(1, 2) and kwargs={'a': 3, 'b': 4}
+
+    If `Store.DRY_RUN` is False, the `check` method executes only once:
+
+        >>> Store.DRY_RUN
+        False
+        >>> model(1, a=2)
+        Forwarding with args=(1,) and kwargs={'a': 2}
+
+    If `Store.DRY_RUN` is True, the `check` method executes every time
+    ``__call__`` is invoked:
+
+        >>> Store.DRY_RUN = True
+        >>> model = Model()
+        >>> model(1, 2, a=3, b=4)
+        Checking 'Model' with args=(1, 2) and kwargs={'a': 3, 'b': 4}
+        Forwarding with args=(1, 2) and kwargs={'a': 3, 'b': 4}
+        >>> model(1, a=2)
+        Checking 'Model' with args=(1,) and kwargs={'a': 2}
+        Forwarding with args=(1,) and kwargs={'a': 2}
+    """
 
-class Finder(Generic[T]):
-    """Find objects in a model by names, regex, type, or types.
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
 
-    Consider the following model:
+        def forward_pre_hook(*args, **kwargs) -> None:
+            self.check(*args, **kwargs)
+            if not Store.DRY_RUN:
+                handle.remove()
+
+        handle = self.register_forward_pre_hook(
+            forward_pre_hook,
+            with_kwargs=True,
+        )
 
-        >>> class Model(nn.Module):
-        ...     def __init__(self, *args, **kwargs) -> None:
-        ...         super().__init__(*args, **kwargs)
-        ...         self._conv = nn.Conv2d(3, 8, 3)
-        ...         self._bn = nn.BatchNorm2d(8)
-        ...         self._conv1 = nn.Conv2d(8, 16, 3)
-        ...         self._bn1 = nn.BatchNorm2d(16)
-        ...         self._relu = nn.ReLU()
-        >>> model = Model().requires_grad_(False)
+    @abstractmethod
+    def check(
+        self,
+        module: nn.Module,
+        args: tuple[Any],
+        kwargs: dict[str, Any],
+    ) -> None:
+        pass
 
-    We can initialize a Finder as follows:
 
-        >>> finder = Finder(model)
+class NoGradMixin(CheckMixin, InitWeightsMixin, BuildSpecMixin):
+    """A mixin class that excludes specific parameters from gradient \
+    computation.
 
-    Suppose we want to find the first convolution and batch normalization
-    layers, this is how we can do it:
+    This mixin class is designed to be a base class for models that necessitate
+    certain parameters to be excluded from gradient computation.
+    It offers methods to scrutinize the model's weights and modify the state
+    dictionary for excluding frozen parameters.
 
-        >>> finder.find_by_names(['._conv', '._bn'])
-        [Conv2d(3, 8, ...), BatchNorm2d(8, ...)]
+    Args:
+        no_grad: A function specifying the parameters to be
+            excluded from gradient computation.
+        filter_state_dict: A flag controlling whether to filter the
+            state dictionary to exclude frozen parameters.
 
-    To find all convolution layers, we can do:
+    Given a model that inherits from this mixin class:
 
-        >>> finder.find_by_regex('_conv.*', 'modules')
-        [Conv2d(3, 8, ...), Conv2d(8, 16, ...)]
+        >>> class NoGrad(NoGradMixin):
+        ...     def __init__(self, *args, **kwargs):
+        ...         super().__init__(*args, **kwargs)
+        ...         self.conv = nn.Conv2d(1, 2, 3)
+        ...     def forward(self) -> None:
+        ...         pass
 
-    `find_by_type` provides another way to find convolution layers:
+    Users can specify parameters to be excluded from gradient computation via
+    a filter:
 
-        >>> finder.find_by_type(nn.Conv2d, 'modules')
-        [Conv2d(3, 8, ...), Conv2d(8, 16, ...)]
+        >>> npf = NamedParametersFilter(name='conv.weight')
+        >>> model = NoGrad(no_grad=npf)
 
-    Different from `find_by_type`, `find_by_types` can match multiple types:
+    The exclusion of parameters from gradient computation does not happen
+    immediately after the model is constructed:
 
-        >>> finder.find_by_types([nn.Conv2d, nn.BatchNorm2d], 'modules')
-        [Conv2d(3, 8, ...), BatchNorm2d(8, ...), Conv2d(8, 16, ...), BatchNorm\
-2d(16, ...)]
+        >>> {n: p.requires_grad for n, p in model.named_parameters()}
+        {'conv.weight': True, 'conv.bias': True}
 
-    `find_by_config` is a more flexible way to find objects.
-    For example, we can find the first convolution and batch normalization
-    layers by:
+    Instead, the exclusion is triggered by calling `init_weights`:
 
-        >>> finder.find_by_config(Config(names=['._conv', '._bn']))
-        [Conv2d(3, 8, ...), BatchNorm2d(8, ...)]
-    """
+        >>> _ = model.init_weights(Config())
+        >>> {n: p.requires_grad for n, p in model.named_parameters()}
+        {'conv.weight': False, 'conv.bias': True}
 
-    def __init__(self, model: nn.Module) -> None:
-        """Initialize a Finder.
+    or by calling `requires_grad_`:
 
-        Args:
-            model: a model to find objects in.
-        """
-        self._model = model
-
-    def _formulate(self, objects) -> list[T]:
-        """Formulate objects into desirable types.
-
-        Args:
-            objects: objects to formulate.
-
-        Returns:
-            A list of formulated objects.
-
-        This method is meant to be overridden by subclasses.
-        """
-        return objects
-
-    def find_by_names(self, names: Iterable[str]) -> list[T]:
-        """Find objects by exact name match.
-
-        Args:
-            names: names of objects to find.
-
-        Returns:
-            A list of objects.
-
-        Refer to `get_` for more details about how names are resolved.
-        """
-        objects = [get_(self._model, name) for name in names]
-        return self._formulate(objects)
-
-    def find_by_regex(self, regex: str, member: str) -> list[T]:
-        """Find objects by regex match.
-
-        Args:
-            regex: a regex to match names.
-            member: type of member to search in.
-
-        Returns:
-            A list of objects.
-
-        Compared with `find_by_names`, this method is more flexible, but it
-        requires traversing the model, which is slower.
-        """
-        objects = [
-            object_
-            for name, object_ in getattr(self._model, f'named_{member}')()
-            if re.search(regex, name)
-        ]
-        return self._formulate(objects)
+        >>> _ = model.requires_grad_()
+        >>> {n: p.requires_grad for n, p in model.named_parameters()}
+        {'conv.weight': False, 'conv.bias': True}
+        >>> _ = model.requires_grad_(False)
+        >>> {n: p.requires_grad for n, p in model.named_parameters()}
+        {'conv.weight': False, 'conv.bias': False}
 
-    def find_by_type(
-        self,
-        type_: type | tuple[type, ...],
-        member: str,
-    ) -> list[T]:
-        """Find objects by type.
-
-        Args:
-            type_: a type or a tuple of types to match.
-            member: type of member to search in.
-
-        Returns:
-            A list of objects.
-        """
-        objects = [
-            object_ for object_ in getattr(self._model, member)()
-            if isinstance(object_, type_)
-        ]
-        return self._formulate(objects)
+    Note that parameters that should be excluded from gradient computation can
+    sometimes be included.
+    A typical example is when the model is used as a component in another:
 
-    def find_by_types(
-        self,
-        types: Iterable[type],
-        *args,
-        **kwargs,
-    ) -> list[T]:
-        """Find objects by types.
+        >>> sequential = nn.Sequential(model)
+        >>> _ = sequential.requires_grad_()
+        >>> {n: p.requires_grad for n, p in sequential.named_parameters()}
+        {'0.conv.weight': True, '0.conv.bias': True}
 
-        Args:
-            types: types to match.
+    To prevent this, the `check` method can be used to verify if parameters
+    are correctly excluded from gradient computation:
 
-        Returns:
-            A list of objects.
-        """
-        return self.find_by_type(tuple(types), *args, **kwargs)
-
-    def find_by_config(self, config: Config) -> list[T]:
-        """Find objects by config.
-
-        Args:
-            config: the match config.
-
-        Returns:
-            A list of objects.
-
-        Raises:
-            ValueError: if ``config`` has no valid key.
-            ValueError: if ``config`` has multiple valid keys.
-
-        Valid keys include ``names``, ``regex``, ``type_``, and ``types``.
-        No valid key or multiple keys will raise an error:
-
-            >>> model = nn.Linear(1, 1)
-            >>> finder = Finder(model)
-            >>> finder.find_by_config(dict(name='.weight'))
-            Traceback (most recent call last):
-                ...
-            ValueError: no valid key in config={'name': '.weight'}
-            >>> finder.find_by_config(dict(names=['.weight'], regex='.*'))
-            Traceback (most recent call last):
-                ...
-            ValueError: multiple keys in config={'names': ['.weight'], 'regex'\
-: '.*'}
-        """
-        keys = config.keys() & ['names', 'regex', 'type_', 'types']
-        if len(keys) == 0:
-            raise ValueError(f"no valid key in {config=}")
-        if len(keys) > 1:
-            raise ValueError(f"multiple keys in {config=}")
-        key = keys.pop()
-        return getattr(self, f'find_by_{key}')(**config)
+        >>> model.check(model, tuple(), {})
+        Traceback (most recent call last):
+            ...
+        AssertionError
+        >>> _ = model.requires_grad_()
+        >>> model.check(model, tuple(), {})
 
-    def determine_modes(
-        self,
-        configs: Iterable[Config],
-    ) -> dict[T, bool | types.EllipsisType]:
-        """Determine modes of objects.
-
-        Args:
-            configs: configs specifying modes.
-
-        Returns:
-            A dict mapping objects to modes.
-
-        Example:
-            >>> class Model(nn.Module):
-            ...     def __init__(self, *args, **kwargs) -> None:
-            ...         super().__init__(*args, **kwargs)
-            ...         self.conv = nn.Conv1d(1, 2, 3)
-            ...         self.bn = nn.BatchNorm1d(3)
-            >>> model = Model().requires_grad_(False)
-            >>> finder = Finder(model)
-            >>> finder.determine_modes([
-            ...     Config(names=['.conv'], mode=False),
-            ...     Config(regex='bias', member='parameters', mode=True),
-            ...     Config(names=['.bn.bias'], mode=Ellipsis),
-            ... ])
-            {Conv1d(1, 2, kernel_size=(3,), stride=(1,)): False, Parameter con\
-taining:
-            tensor([..., ...]): True, Parameter containing:
-            tensor([0., 0., 0.]): Ellipsis}
-        """
-        modes: dict[T, bool | types.EllipsisType] = dict()
-        for config in configs:
-            config = config.copy()
-            mode = config.pop('mode')
-            for object_ in self.find_by_config(config):
-                modes[object_] = mode
-        return modes
-
-
-class ParameterFinder(Finder[nn.Parameter]):
-    """Find parameters."""
-
-    def _formulate(self, objects) -> list[nn.Parameter]:
-        """Formulate objects into parameters.
-
-        Args:
-            objects: objects to formulate.
-
-        Raises:
-            TypeError: if any element of ``objects`` is not supported.
-
-        Returns:
-            A list of parameters.
-
-        Supported elements include `nn.Parameter` and `nn.Module`:
-
-            >>> import torch
-            >>> model = nn.Linear(1, 2).requires_grad_(False)
-            >>> _ = model.weight.data.fill_(3.0)
-            >>> _ = model.bias.data.fill_(4.0)
-            >>> finder = ParameterFinder(model)
-            >>> finder._formulate([
-            ...     nn.Parameter(torch.tensor(5.0), requires_grad=False),
-            ...     model,
-            ... ])
-            [Parameter containing:
-            tensor(5.), Parameter containing:
-            tensor([[3.],
-                    [3.]]), Parameter containing:
-            tensor([4., 4.])]
-
-        Other types triggers exception:
-
-            >>> finder._formulate([torch.tensor(1.0)])
-            Traceback (most recent call last):
-               ...
-            TypeError: unsupported object_=tensor(1.)
-        """
-        parameters = []
-        for object_ in objects:
-            if isinstance(object_, nn.Parameter):
-                parameters.append(object_)
-            elif isinstance(object_, nn.Module):
-                parameters.extend(object_.parameters())
-            else:
-                raise TypeError(f"unsupported {object_=}")
-        return parameters
+    Refer to `CheckMixin` for more information on the `check` method.
 
+    By default, the state dictionary includes all parameters:
 
-class ModuleFinder(Finder[nn.Module]):
-    """Find modules."""
+        >>> list(model.state_dict())
+        ['conv.weight', 'conv.bias']
 
-    def _formulate(self, objects) -> list[nn.Module]:
-        """Formulate objects into modules.
+    However, in most cases, users may want to exclude frozen parameters from
+    the state dictionary.
+    This can be achieved by setting ``filter_state_dict`` to True:
 
-        Args:
-            objects: objects to formulate.
+        >>> model = NoGrad(no_grad=npf, filter_state_dict=True)
+        >>> list(model.state_dict())
+        ['conv.bias']
 
-        Returns:
-            A list of modules.
+    State dictionary filtering works even if the model is used as a component
+    in another model:
 
-        Raises:
-            TypeError: if any element of ``objects`` is not `nn.Module`.
+        >>> sequential = nn.Sequential(model)
+        >>> list(sequential.state_dict())
+        ['0.conv.bias']
+    """
 
-        In case users accidentally pass in `nn.Parameter`, a `TypeError` will
-        be raised:
+    def __init__(
+        self,
+        *args,
+        no_grad: NamedParametersFilter | None = None,
+        filter_state_dict: bool = False,
+        **kwargs,
+    ) -> None:
+        super().__init__(*args, **kwargs)
+        self._no_grad = no_grad
+        self._filter_state_dict = filter_state_dict
 
-            >>> model = nn.Linear(2, 1).requires_grad_(False)
-            >>> finder = ModuleFinder(model)
-            >>> finder._formulate([model.weight])
-            Traceback (most recent call last):
-                ...
-            TypeError: unsupported module=Parameter containing:
-            tensor([[..., ...]])
-        """
-        modules = list(objects)
-        for module in modules:
-            if not isinstance(module, nn.Module):
-                raise TypeError(f"unsupported {module=}")
-        return modules
+    @classproperty
+    def build_spec(self) -> BuildSpec:
+        build_spec = BuildSpec(no_grad=FilterRegistry.build)
+        return super().build_spec | build_spec
+
+    def check(self, *args, **kwargs) -> None:
+        super().check(*args, **kwargs)
+        for _, parameter in self._no_grad_named_parameters():
+            assert not parameter.requires_grad
+
+    def _no_grad_named_parameters(self) -> Iterable[tuple[str, nn.Parameter]]:
+        if self._no_grad is None:
+            return []
+        return self._no_grad(self)
+
+    def init_weights(self, config: Config) -> bool:
+        self.requires_grad_()
+        return super().init_weights(config)
 
+    def requires_grad_(self, requires_grad: bool = True) -> Self:
+        super().requires_grad_(requires_grad)
+        for _, parameter in self._no_grad_named_parameters():
+            parameter.requires_grad_(False)
+        return self
+
+    def state_dict(self, *args, prefix: str = '', **kwargs) -> Any:
+        state_dict: MutableMapping[str, torch.Tensor] = \
+            super().state_dict(*args, prefix=prefix, **kwargs)
+        if self._filter_state_dict:
+            for name, _ in self._no_grad_named_parameters():
+                state_dict.pop(prefix + name, None)
+        return state_dict
+
+
+class EvalMixin(CheckMixin, InitWeightsMixin, BuildSpecMixin):
+    """A mixin class that provides evaluation functionality for a model.
+
+    This mixin class is intended to be used as a base class for models that
+    require evaluation functionality.
+    It provides methods for checking the model's evaluation mode and toggling
+    between training and evaluation modes.
+
+    Args:
+        eval_: A function specifying the modules to be marked evaluation.
+
+    To use the mixin class, first define a model:
 
-class FrozenMixin(nn.Module):
-    """Freeze parameters."""
+        >>> class Eval(EvalMixin):
+        ...     def __init__(self, *args, **kwargs):
+        ...         super().__init__(*args, **kwargs)
+        ...         self.conv = nn.Conv2d(1, 2, 3)
+        ...         self.bn = nn.BatchNorm2d(2)
+        ...     def forward(self) -> None:
+        ...         pass
+
+    Set up a module filter:
+
+        >>> nmf = NamedModulesFilter(name='bn')
+
+    Construct the model:
+
+        >>> model = Eval(eval_=nmf)
+        >>> model.conv.training
+        True
+        >>> model.bn.training
+        True
+
+    Use `init_weights` to change the training property:
+
+        >>> model.init_weights(Config())
+        True
+        >>> model.conv.training
+        True
+        >>> model.bn.training
+        False
+
+    Use `check` method to verify if the properties meet the requirement:
+
+        >>> model.check(model, tuple(), {})
+        >>> model.bn.training = True
+        >>> model.check(model, tuple(), {})
+        Traceback (most recent call last):
+            ...
+        AssertionError
+
+    Use `train` to enforce the properties to meet the requirement:
+
+        >>> _ = model.train()
+        >>> model.conv.training
+        True
+        >>> model.bn.training
+        False
+        >>> _ = model.eval()
+        >>> model.conv.training
+        False
+        >>> model.bn.training
+        False
+
+    The model can be utilized as a component in other models:
+
+        >>> sequential = nn.Sequential(model)
+        >>> _ = sequential.train()
+        >>> sequential[0].conv.training
+        True
+        >>> sequential[0].bn.training
+        False
+    """
 
     def __init__(
         self,
-        requires_grad_configs: Iterable[Config] = tuple(),
-        train_configs: Iterable[Config] = tuple(),
-        with_state_dict_hook: bool = False,
         *args,
+        eval_: NamedModulesFilter | None = None,
         **kwargs,
     ) -> None:
         super().__init__(*args, **kwargs)
-        self._requires_grad_configs = tuple(requires_grad_configs)
-        self._train_configs = tuple(train_configs)
-        self._with_state_dict_hook = with_state_dict_hook
-        if with_state_dict_hook:
-            self._register_state_dict_hook(state_dict_hook)
-
-    @property
-    def requires_grad_configs(self) -> tuple[Config, ...]:
-        return self._requires_grad_configs
-
-    @property
-    def train_configs(self) -> tuple[Config, ...]:
-        return self._train_configs
+        self._eval = eval_
 
-    def requires_grad_(self, requires_grad: bool = True) -> Self:
-        self = super().requires_grad_(requires_grad)
-        finder = ParameterFinder(self)
-        configs = self._requires_grad_configs
-        modes = {
-            parameter: mode
-            for parameter, mode in finder.determine_modes(configs).items()
-            if mode is not ...
-        }
-        for parameter, mode in modes.items():
-            parameter.requires_grad_(mode)
-        return self
+    @classproperty
+    def build_spec(self) -> BuildSpec:
+        build_spec = BuildSpec(eval_=FilterRegistry.build)
+        return super().build_spec | build_spec
+
+    def check(self, *args, **kwargs) -> None:
+        super().check(*args, **kwargs)
+        for _, module in self._eval_modules():
+            assert not module.training
+
+    def _eval_modules(self) -> Iterable[tuple[str, nn.Module]]:
+        if self._eval is None:
+            return []
+        return self._eval(self)
+
+    def init_weights(self, config: Config) -> bool:
+        self.train()
+        return super().init_weights(config)
 
     def train(self, mode: bool = True) -> Self:
-        self = super().train(mode)
-        finder = ModuleFinder(self)
-        configs = self._train_configs
-        modes = {
-            module: module.training if mode is ... else mode
-            for module, mode in finder.determine_modes(configs).items()
-        }
-        for module in modes:
-            module.train(modes[module])
+        super().train(mode)
+        for _, module in self._eval_modules():
+            if module is self:
+                super().train(False)
+            else:
+                module.eval()
         return self
 
 
-def state_dict_hook(
-    model: FrozenMixin,
-    state_dict: MutableMapping[str, Any],
-    prefix: str,
-    *args,
-    **kwargs,
-) -> None:
-    """Hook for `torch.nn.Module.load_state_dict`.
-
-    Args:
-        model: the model to load state dict.
-        state_dict: the state dict to load.
-        prefix: the prefix of the model.
-        *args: other args.
-        **kwargs: other kwargs.
+class FreezeMixin(NoGradMixin, EvalMixin):
+    """A mixin class that provides freezing functionality to a model.
 
-    Example:
-
-        >>> class Model(FrozenMixin):
+    Examples:
+        >>> class Freeze(FreezeMixin):
         ...     def __init__(self, *args, **kwargs) -> None:
-        ...         super().__init__(
-        ...             *args,
-        ...             requires_grad_configs=[
-        ...                 Config(names=['.conv'], mode=False),
-        ...                 Config(names=['.bn'], mode=...),
-        ...             ],
-        ...             with_state_dict_hook=True,
-        ...             **kwargs,
-        ...         )
-        ...         self.conv = nn.Conv1d(1, 2, 1)
-        ...         self.bn = nn.BatchNorm1d(2)
-        >>> Model().state_dict()
-        OrderedDict([('bn.weight', tensor([1., 1.])), ('bn.bias', tensor([0., \
-0.])), ('bn.running_mean', tensor([0., 0.])), ('bn.running_var', tensor([1., 1\
-.])), ('bn.num_batches_tracked', tensor(0))])
-        >>> nn.Sequential(Model()).state_dict()
-        OrderedDict([('0.bn.weight', tensor([1., 1.])), ('0.bn.bias', tensor([\
-0., 0.])), ('0.bn.running_mean', tensor([0., 0.])), ('0.bn.running_var', tenso\
-r([1., 1.])), ('0.bn.num_batches_tracked', tensor(0))])
+        ...         super().__init__(*args, **kwargs)
+        ...         self.c = nn.Conv2d(1, 2, 3)
+        ...         self.b = nn.BatchNorm2d(2)
+        >>> nmf = NamedModulesFilter(name='b')
+        >>> freeze = Freeze(freeze=nmf)
+        >>> freeze.init_weights(Config())
+        True
+        >>> {n: p.requires_grad for n, p in freeze.named_parameters()}
+        {'c.weight': True, 'c.bias': True, 'b.weight': False, 'b.bias': False}
+        >>> {n: m.training for n, m in freeze.named_modules()}
+        {'': True, 'c': True, 'b': False}
     """
-    if len(state_dict) == 0:
-        return
-    finder = ParameterFinder(model)
-    modes = finder.determine_modes(model.requires_grad_configs)
-    parameter_names = {
-        parameter: name
-        for name, parameter in model.named_parameters()
-    }
-    for parameter, mode in modes.items():
-        if mode is False:
-            name = parameter_names[parameter]
-            name = name.replace('_fsdp_wrapped_module.', '')
-            state_dict.pop(prefix + name)
+
+    def __init__(
+        self,
+        *args,
+        freeze: NamedModulesFilter | None = None,
+        **kwargs,
+    ) -> None:
+        if freeze is None:
+            super().__init__(*args, **kwargs)
+            return
+        super().__init__(
+            *args,
+            eval_=freeze,
+            no_grad=NamedParametersFilter(modules=freeze),
+            **kwargs,
+        )
+
+    @classproperty
+    def build_spec(self) -> BuildSpec:
+        build_spec = BuildSpec(freeze=FilterRegistry.build)
+        return super().build_spec | build_spec
+
+
+class FrozenMixin(FreezeMixin):
+    """A mixin class that provides freezing functionality to a class.
+
+    This mixin class is used to create frozen modules, where the parameters
+    are excluded from gradient computation and the modules are marked as
+    evaluation.
+
+    Examples:
+        >>> class Frozen(FrozenMixin):
+        ...     def __init__(self) -> None:
+        ...         super().__init__()
+        ...         self.conv = nn.Conv2d(1, 2, 3)
+        >>> frozen = Frozen()
+        >>> frozen.init_weights(Config())
+        True
+        >>> {n: p.requires_grad for n, p in frozen.named_parameters()}
+        {'conv.weight': False, 'conv.bias': False}
+        >>> {n: m.training for n, m in frozen.named_modules()}
+        {'': False, 'conv': False}
+    """
+
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, freeze=NamedModulesFilter(name=''), **kwargs)
```

### Comparing `todd_ai-0.4.0/todd/runners/callbacks/autocast.py` & `todd_ai-0.5.0/todd/runners/callbacks/autocast.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 __all__ = [
     'AutocastCallback',
 ]
 
 import contextlib
-from typing import Any
 
 import torch
 
-from ...base import CallbackRegistry, Config
+from ...configs import Config
+from ..memo import Memo
+from ..registries import CallbackRegistry
 from .base import BaseCallback
 
-Memo = dict[str, Any]
 
-
-@CallbackRegistry.register()
+@CallbackRegistry.register_()
 class AutocastCallback(BaseCallback):
 
     def __init__(self, *args, autocast: Config, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self._autocast = autocast
 
     def run_iter_context(
```

### Comparing `todd_ai-0.4.0/todd/runners/callbacks/base.py` & `todd_ai-0.5.0/todd/runners/callbacks/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
+# pylint: disable=pointless-statement
+
 __all__ = [
     'BaseCallback',
 ]
 
 import contextlib
-from typing import Any
-
-from ...base import StateDictMixin
-from ..runners import RunnerHolderMixin
 
-Memo = dict[str, Any]
+from ...utils import StateDictMixin
+from ..memo import Memo
+from ..registries import CallbackRegistry
+from ..utils import RunnerHolderMixin
 
 
+@CallbackRegistry.register_()
 class BaseCallback(RunnerHolderMixin, StateDictMixin):
 
-    def connect(self) -> None:
+    def init(self, *args, **kwargs) -> None:
         pass
 
     def should_break(self, batch, memo: Memo) -> bool:
         """Determine whether to break the run loop.
 
         Args:
             batch: inputs.
```

### Comparing `todd_ai-0.4.0/todd/runners/callbacks/composed.py` & `todd_ai-0.5.0/todd/runners/callbacks/composed.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,47 @@
 __all__ = [
     'ComposedCallback',
 ]
 
-from collections import UserList
-from typing import Any, Iterable, Literal, Mapping, TypedDict
+from typing import Any, Iterable, Iterator, Literal, Mapping
 
-from ...base import CallbackRegistry, Config
+from ...configs import Config
+from ..registries import CallbackRegistry
+from ..utils import PriorityQueue
 from .base import BaseCallback
 
-Memo = dict[str, Any]
+KT = Literal['init', 'should_break', 'should_continue', 'before_run_iter',
+             'run_iter_context', 'after_run_iter', 'should_break_epoch',
+             'should_continue_epoch', 'before_run_epoch', 'run_epoch_context',
+             'after_run_epoch', 'before_run', 'after_run']
 
 
-class Priority(TypedDict, total=False):
-    connect: int
-    should_break: int
-    should_continue: int
-    before_run_iter: int
-    run_iter_context: int
-    after_run_iter: int
-    should_break_epoch: int
-    should_continue_epoch: int
-    before_run_epoch: int
-    run_epoch_context: int
-    after_run_epoch: int
-    before_run: int
-    after_run: int
-
-
-@CallbackRegistry.register()
-class ComposedCallback(BaseCallback, UserList[BaseCallback]):
+@CallbackRegistry.register_()
+class ComposedCallback(BaseCallback):
 
     def __init__(self, *args, callbacks: Iterable[Config], **kwargs) -> None:
-        self._priorities: list[Priority] = [
-            c.pop('priority', dict()) for c in callbacks
-        ]
         super().__init__(*args, **kwargs)
-        self.extend(
-            CallbackRegistry.build(c, runner=self._runner) for c in callbacks
-        )
+        priorities = [c.pop('priority', dict()) for c in callbacks]
+        queue = [
+            CallbackRegistry.build(c, runner=self.runner) for c in callbacks
+        ]
+        self._callbacks: PriorityQueue[KT, BaseCallback] = \
+            PriorityQueue(priorities, queue)
 
-    def _callbacks(
-        self,
-        name: Literal['connect', 'should_break', 'should_continue',
-                      'before_run_iter', 'run_iter_context', 'after_run_iter',
-                      'should_break_epoch', 'should_continue_epoch',
-                      'before_run_epoch', 'run_epoch_context',
-                      'after_run_epoch', 'before_run', 'after_run'],
-    ) -> list[BaseCallback]:
-        priorities = [p.get(name, 0) for p in self._priorities]
-        priority_index = [(p, i) for i, p in enumerate(priorities)]
-        priority_index = sorted(priority_index)
-        _, indices = zip(*priority_index)
-        return [self[i] for i in indices]
-
-    def connect(self) -> None:
-        super().connect()
-        for c in self._callbacks('connect'):
-            c.connect()
+    @property
+    def callbacks(self) -> PriorityQueue[KT, BaseCallback]:
+        return self._callbacks
+
+    def __iter__(self) -> Iterator[BaseCallback]:
+        return iter(self._callbacks.queue)
+
+    def init(self, *args, **kwargs) -> None:
+        super().init(*args, **kwargs)
+        for c in self._callbacks('init'):
+            c.init(*args, **kwargs)
 
     def should_break(self, *args, **kwargs) -> bool:
         super().should_break(*args, **kwargs)
         return any(
             c.should_break(*args, **kwargs)
             for c in self._callbacks('should_break')
         )
@@ -124,19 +105,25 @@
     def after_run(self, *args, **kwargs) -> None:
         super().after_run(*args, **kwargs)
         for c in self._callbacks('after_run'):
             c.after_run(*args, **kwargs)
 
     def state_dict(self, *args, **kwargs) -> dict[str, Any]:
         state_dict = super().state_dict(*args, **kwargs)
-        state_dict['callbacks'] = [c.state_dict(*args, **kwargs) for c in self]
+        state_dict['callbacks'] = [
+            c.state_dict(*args, **kwargs) for c in self._callbacks.queue
+        ]
         return state_dict
 
     def load_state_dict(
         self,
         state_dict: Mapping[str, Any],
         *args,
         **kwargs,
     ) -> None:
         super().load_state_dict(state_dict, *args, **kwargs)
-        for c, s in zip(self, state_dict['callbacks'], strict=True):
+        for c, s in zip(
+            self._callbacks.queue,
+            state_dict['callbacks'],
+            strict=True,
+        ):
             c.load_state_dict(s, *args, **kwargs)
```

### Comparing `todd_ai-0.4.0/todd/runners/callbacks/interval.py` & `todd_ai-0.5.0/todd/runners/callbacks/interval.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,14 @@
         self._interval = interval
         self._by_epoch = by_epoch
 
     def __should_run(self, step: int) -> bool:
         return self._interval > 0 and step % self._interval == 0
 
     def _should_run_iter(self) -> bool:
-        return not self._by_epoch and self.__should_run(self._runner.iter_)
+        return not self._by_epoch and self.__should_run(self.runner.iter_)
 
     def _should_run_epoch(self) -> bool:
         return (
             self._by_epoch
             and self.__should_run(self.epoch_based_trainer.epoch)
         )
```

### Comparing `todd_ai-0.4.0/todd/runners/callbacks/log.py` & `todd_ai-0.5.0/todd/runners/callbacks/log.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,97 @@
 __all__ = [
     'LogCallback',
 ]
 
+import datetime
 import logging
 from typing import Any
 
-from ...base import CallbackRegistry, Formatter
-from ...utils import get_rank, get_timestamp
+import torch
+
+from ...configs import Config
+from ...loggers import Formatter
+from ...patches.torch import get_rank
+from ...utils import Store, collect_env_, get_timestamp
+from ..memo import Memo
+from ..registries import CallbackRegistry, ETARegistry
+from ..utils import BaseETA
 from .base import BaseCallback
 from .interval import IntervalMixin
 
-Memo = dict[str, Any]
-
 
-@CallbackRegistry.register()
+@CallbackRegistry.register_()
 class LogCallback(IntervalMixin, BaseCallback):
 
     def __init__(
         self,
         *args,
+        collect_env: Config | None = None,
         with_file_handler: bool = False,
+        eta: Config | None = None,
         **kwargs,
     ) -> None:
         super().__init__(*args, **kwargs)
+        self._collect_env = collect_env
         self._with_file_handler = with_file_handler
+        self._eta_config = eta
 
-    def connect(self) -> None:
-        super().connect()
-        if get_rank() == 0 and self._with_file_handler:
-            file = self._runner.work_dir / f'{get_timestamp()}.log'
+    def init(self, *args, **kwargs) -> None:
+        super().init(*args, **kwargs)
+        if get_rank() > 0:
+            return
+        if self._with_file_handler:
+            file = self.runner.work_dir / f'{get_timestamp()}.log'
             handler = logging.FileHandler(file)
             handler.setFormatter(Formatter())
-            self._runner.logger.addHandler(handler)
+            self.runner.logger.addHandler(handler)
+        if self._collect_env is not None:
+            env = collect_env_(**self._collect_env)
+            self.runner.logger.info(env)
+
+    def before_run(self, memo: Memo) -> None:
+        super().before_run(memo)
+        self._eta: BaseETA | None = (
+            None if self._eta_config is None else ETARegistry.build(
+                self._eta_config,
+                start=self.runner.iter_ - 1,
+                end=self.runner.iters,
+            )
+        )
 
     def before_run_iter(self, batch, memo: Memo) -> None:
         super().before_run_iter(batch, memo)
         if get_rank() == 0 and self._should_run_iter():
             memo['log'] = dict()
 
     def after_run_iter(self, batch, memo: Memo) -> None:
         super().after_run_iter(batch, memo)
         if 'log' not in memo:
             return
+        prefix = f"Iter [{self.runner.iter_}/{self.runner.iters}] "
+
+        if self._eta is not None:
+            eta = self._eta(self.runner.iter_)
+            eta = round(eta)
+            prefix += f"ETA {str(datetime.timedelta(seconds=eta))} "
+
+        if Store.CUDA:
+            max_memory_allocated = max(
+                torch.cuda.max_memory_allocated(i)
+                for i in range(torch.cuda.device_count())
+            )
+            torch.cuda.reset_peak_memory_stats()
+            prefix += f"Memory {max_memory_allocated / 1024 ** 2:.2f}M "
+
         log: dict[str, Any] = memo.pop('log')
-        prefix = f"Iter [{self._runner.iter_}/{self._runner.iters}] "
-        message = ' '.join(f'{k}={v}' for k, v in log.items())
-        self._runner.logger.info(prefix + message)
+        message = ' '.join(f'{k}={v}' for k, v in log.items() if v is not None)
+        self.runner.logger.info(prefix + message)
 
     def before_run_epoch(self, epoch_memo: Memo, memo: Memo) -> None:
         super().before_run_epoch(epoch_memo, memo)
         runner = self.epoch_based_trainer
         if get_rank() == 0:
-            runner.logger.info(f"Epoch [{runner.epoch}/{runner.epochs}]")
+            runner.logger.info(
+                "Epoch [%d/%d]",
+                runner.epoch + 1,
+                runner.epochs,
+            )
```

### Comparing `todd_ai-0.4.0/todd/runners/callbacks/lr.py` & `todd_ai-0.5.0/todd/runners/callbacks/lr.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,57 +3,58 @@
     'LRScaleCallback',
 ]
 
 from typing import Any, Mapping, cast
 
 import torch
 
-from ...base import CallbackRegistry, Config, LrSchedulerRegistry
-from ...utils import get_world_size
-from ..runners import Trainer
+from ...configs import Config
+from ...patches.torch import get_rank, get_world_size
+from ...registries import LRSchedulerRegistry
+from ..memo import Memo
+from ..registries import CallbackRegistry
+from ..trainer import Trainer
 from .base import BaseCallback
 from .interval import IntervalMixin
 
-Memo = dict[str, Any]
 
-
-@CallbackRegistry.register()
+@CallbackRegistry.register_()
 class LRScheduleCallback(IntervalMixin, BaseCallback):
 
     def __init__(
         self,
         *args,
         lr_scheduler: Config,
         interval: int = 1,
         **kwargs,
     ) -> None:
         super().__init__(*args, interval=interval, **kwargs)
-        assert isinstance(self._runner, Trainer)
+        assert isinstance(self.runner, Trainer)
         self._lr_scheduler_config = lr_scheduler
 
-    def connect(self) -> None:
-        super().connect()
+    def init(self, *args, **kwargs) -> None:
+        super().init(*args, **kwargs)
         self._build_lr_scheduler()
 
     def _build_lr_scheduler(self) -> None:
-        runner = cast(Trainer, self._runner)
+        runner = cast(Trainer, self.runner)
         self._lr_scheduler: torch.optim.lr_scheduler.LRScheduler = \
-            LrSchedulerRegistry.build(
+            LRSchedulerRegistry.build(
                 self._lr_scheduler_config,
                 optimizer=runner.optimizer,
             )
 
     def after_run_iter(self, batch, memo: Memo) -> None:
         super().after_run_iter(batch, memo)
-        if self._should_run_iter():
-            self._lr_scheduler.step()
         if 'log' in memo:
             memo['log']['lr'] = [
                 f'{lr:.3e}' for lr in self._lr_scheduler.get_last_lr()
             ]
+        if self._should_run_iter():
+            self._lr_scheduler.step()
 
     def after_run_epoch(self, epoch_memo: Memo, memo: Memo) -> None:
         super().after_run_epoch(epoch_memo, memo)
         if self._should_run_epoch():
             self._lr_scheduler.step()
 
     def load_state_dict(
@@ -67,32 +68,34 @@
 
     def state_dict(self, *args, **kwargs) -> dict[str, Any]:
         state_dict = super().state_dict(*args, **kwargs)
         state_dict['lr_scheduler'] = self._lr_scheduler.state_dict()
         return state_dict
 
 
-@CallbackRegistry.register()
+@CallbackRegistry.register_()
 class LRScaleCallback(BaseCallback):
 
     def __init__(self, *args, lr_scaler: Config, **kwargs) -> None:
         super().__init__(*args, **kwargs)
-        assert isinstance(self._runner, Trainer)
+        assert isinstance(self.runner, Trainer)
         self._lr_scaler_config = lr_scaler
 
     def _scale_lr(self, config: Config) -> None:
-        runner = cast(Trainer, self._runner)
+        runner = cast(Trainer, self.runner)
+        assert runner.dataloader.batch_size is not None
         base_batch_size = config.base_batch_size
         batch_size = get_world_size() * runner.dataloader.batch_size
         lr_scaler = batch_size / base_batch_size
         if 'lr' in runner.optimizer.defaults:
             runner.optimizer.defaults['lr'] *= lr_scaler
         for param_group in runner.optimizer.param_groups:
             if 'lr' in param_group:
                 param_group['lr'] *= lr_scaler
-        runner.logger.info(
-            f"{base_batch_size=} {batch_size=} {lr_scaler=:.3f}"
-        )
+        if get_rank() == 0:
+            runner.logger.info(
+                f"{base_batch_size=} {batch_size=} {lr_scaler=:.3f}"
+            )
 
-    def connect(self) -> None:
-        super().connect()
+    def init(self, *args, **kwargs) -> None:
+        super().init(*args, **kwargs)
         self._scale_lr(self._lr_scaler_config)
```

### Comparing `todd_ai-0.4.0/todd/runners/callbacks/monitor.py` & `todd_ai-0.5.0/todd/runners/callbacks/monitor.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 __all__ = [
     'MonitorCallback',
 ]
 
 import contextlib
 import logging
-from typing import Any
 
-from ...base import CallbackRegistry
+from ..memo import Memo
+from ..registries import CallbackRegistry
 from .base import BaseCallback
 
-Memo = dict[str, Any]
-
 
 class Context:
 
     def __init__(self, logger: logging.Logger, **kwargs) -> None:
         self._logger = logger
         self._kwargs = kwargs
 
@@ -24,27 +22,27 @@
     def __exit__(self, *exc_info) -> None:
         if all(i is None for i in exc_info):
             return
         message = '\n'.join(f'{k}={v}' for k, v in self._kwargs.items())
         self._logger.exception("Unable to run " + message)
 
 
-@CallbackRegistry.register()
+@CallbackRegistry.register_()
 class MonitorCallback(BaseCallback):
 
     def run_iter_context(
         self,
         exit_stack: contextlib.ExitStack,
         batch,
         memo: Memo,
     ) -> None:
         super().run_iter_context(exit_stack, batch, memo)
         context = Context(
-            self._runner.logger,
-            iter_=self._runner.iter_,
+            self.runner.logger,
+            iter_=self.runner.iter_,
             batch=batch,
             memo=memo,
         )
         exit_stack.enter_context(context)
 
     def run_epoch_context(
         self,
```

### Comparing `todd_ai-0.4.0/todd/runners/strategies/base.py` & `todd_ai-0.5.0/todd/runners/strategies/fsdp.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,67 @@
 __all__ = [
-    'BaseStrategy',
+    'FSDPStrategy',
 ]
 
-import pathlib
-from typing import Any, Mapping
+from typing import Any, Mapping, TypeVar, cast
 
 import torch
-import torch.nn as nn
+from torch import nn
+from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
 
-from ...base import (
-    Config,
-    ModelRegistry,
-    OptimizerRegistry,
-    StateDictMixin,
-    StrategyRegistry,
-)
-from ..runners import RunnerHolderMixin
-
-
-@StrategyRegistry.register()
-class BaseStrategy(RunnerHolderMixin, StateDictMixin):
-    _model: nn.Module
+from ...configs import Config
+from ...registries import OptimizerRegistry
+from ..registries import StrategyRegistry
+from .cuda import CUDAStrategy
 
-    def __init__(
-        self,
-        *args,
-        model: Config,
-        **kwargs,
-    ) -> None:
-        super().__init__(*args, **kwargs)
-        self._build_model(model)
+# TODO: update when pytorch updates
 
-    def _build_model(self, config: Config) -> None:
-        self._model = ModelRegistry.build(config)
+T = TypeVar('T', bound=FSDP)
 
-    def build_optimizer(self, config: Config) -> torch.optim.Optimizer:
-        return OptimizerRegistry.build(config, model=self._model)
 
-    @property
-    def model(self) -> nn.Module:
-        return self._model
+@StrategyRegistry.register_()
+class FSDPStrategy(CUDAStrategy[T]):
+
+    def wrap_model(self, model: nn.Module, config: Config) -> T:
+        model = super().wrap_model(model, config)
+        model = FSDP(model, **config)
+        return cast(T, model)
 
     @property
     def module(self) -> nn.Module:
-        return self._model
+        return self.runner.model.module
+
+    def build_optimizer(self, config: Config) -> torch.optim.Optimizer:
+        return OptimizerRegistry.build(config, model=self.runner.model)
 
     def model_state_dict(self, *args, **kwargs) -> dict[str, Any]:
-        return self._model.state_dict(*args, **kwargs)
+        return self.runner.model.state_dict(*args, **kwargs)
 
     def load_model_state_dict(
         self,
         state_dict: Mapping[str, Any],
         *args,
         **kwargs,
     ) -> None:
-        self._model.load_state_dict(state_dict, *args, **kwargs)
-
-    def load_model_from(self, f: pathlib.Path, *args, **kwargs) -> None:
-        self._runner._logger.info(f"Loading model from {f}")
-        model_state_dict = torch.load(f, 'cpu')
-        self.load_model_state_dict(model_state_dict, *args, **kwargs)
+        self.runner.model.load_state_dict(state_dict, *args, **kwargs)
 
-    def optim_state_dict(self, *args, **kwargs) -> dict[str, Any]:
-        return self.trainer.optimizer.state_dict()
+    def optim_state_dict(
+        self,
+        *args,
+        **kwargs,
+    ) -> dict[str, Any]:
+        trainer = self.trainer
+        return FSDP.full_optim_state_dict(trainer.model, trainer.optimizer)
 
     def load_optim_state_dict(
         self,
         state_dict: Mapping[str, Any],
         *args,
         **kwargs,
     ) -> None:
-        self.trainer.optimizer.load_state_dict(state_dict)
+        state_dict = dict(state_dict)
+        trainer = self.trainer
+        sharded_state_dict = FSDP.scatter_full_optim_state_dict(
+            state_dict,
+            trainer.model,
+        )
+        trainer.optimizer.load_state_dict(sharded_state_dict)
```

### Comparing `todd_ai-0.4.0/todd/runners/strategies/ddp.py` & `todd_ai-0.5.0/todd/runners/strategies/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,97 @@
 __all__ = [
-    'DDPStrategy',
+    'BaseStrategy',
 ]
 
-from typing import TYPE_CHECKING, Any, Mapping
+from typing import Any, Mapping, TypeVar, cast
 
 import torch
-import torch.distributed
-import torch.nn as nn
-from torch.nn.parallel import DistributedDataParallel as DDP
-
-from ...base import Config, OptimizerRegistry, Store, StrategyRegistry
-from ...utils import get_local_rank
-from .base import BaseStrategy
+from torch import nn
 
+from ...configs import Config
+from ...patches.torch import get_rank
+from ...registries import ModelRegistry, OptimizerRegistry
+from ...utils import StateDictMixin
+from ..registries import StrategyRegistry
+from ..utils import RunnerHolderMixin
 
-@StrategyRegistry.register()
-class DDPStrategy(BaseStrategy):
-    _model: DDP
+T = TypeVar('T', bound=nn.Module)
+
+
+@StrategyRegistry.register_()
+class BaseStrategy(RunnerHolderMixin[T], StateDictMixin):
 
     def __init__(
         self,
         *args,
         setup: Config | None = None,
-        wrap_model: Config | None = None,
         **kwargs,
     ) -> None:
-        assert Store.CUDA
+        super().__init__(*args, **kwargs)
         if setup is None:
             setup = Config()
-        self._setup(setup)
-        super().__init__(*args, **kwargs)
-        if wrap_model is None:
-            wrap_model = Config()
-        self._wrap_model(wrap_model)
-
-    def _setup(self, config: Config) -> None:
-        init_process_group = config.get(
-            'init_process_group',
-            Config(backend='nccl'),
-        )
-        torch.distributed.init_process_group(**init_process_group)
-        torch.cuda.set_device(get_local_rank() % torch.cuda.device_count())
+        self.setup(setup)
+
+    def setup(self, config: Config) -> None:
+        pass
 
-    def _wrap_model(self, config: Config) -> None:
-        self._model = DDP(self._model.cuda(), **config)
+    def build_model(self, config: Config) -> nn.Module:
+        return ModelRegistry.build(config)
+
+    def map_model(self, model: nn.Module, config: Config) -> nn.Module:
+        return model
+
+    def wrap_model(self, model: nn.Module, config: Config) -> T:
+        return cast(T, model)
 
     def build_optimizer(self, config: Config) -> torch.optim.Optimizer:
-        return OptimizerRegistry.build(config, model=self._model.module)
+        return OptimizerRegistry.build(config, model=self.module)
+
+    @property
+    def module(self) -> nn.Module:
+        return self.runner.model
 
     def model_state_dict(self, *args, **kwargs) -> dict[str, Any]:
         return self.module.state_dict(*args, **kwargs)
 
     def load_model_state_dict(
         self,
         state_dict: Mapping[str, Any],
         *args,
         **kwargs,
     ) -> None:
-        self.module.load_state_dict(state_dict, *args, **kwargs)
+        incompatible_keys = self.module.load_state_dict(
+            state_dict,
+            *args,
+            **kwargs,
+        )
+        if get_rank() == 0:
+            self.runner.logger.info(incompatible_keys)
 
-    @property
-    def module(self) -> nn.Module:
-        return self._model.module
+    def load_model_from(
+        self,
+        f: (
+            torch.serialization.FILE_LIKE
+            | list[torch.serialization.FILE_LIKE]
+        ),
+        *args,
+        **kwargs,
+    ) -> None:
+        f_list = f if isinstance(f, list) else [f]
+        model_state_dict = dict()
+        for f_ in f_list:
+            if get_rank() == 0:
+                self.runner.logger.info("Loading model from %s", f_)
+            model_state_dict.update(torch.load(f_, 'cpu'))
+        self.load_model_state_dict(model_state_dict, *args, **kwargs)
 
-    if TYPE_CHECKING:
+    def optim_state_dict(self, *args, **kwargs) -> dict[str, Any]:
+        return self.trainer.optimizer.state_dict()
 
-        @property
-        def model(self) -> DDP:
-            ...
+    def load_optim_state_dict(
+        self,
+        state_dict: Mapping[str, Any],
+        *args,
+        **kwargs,
+    ) -> None:
+        state_dict = dict(state_dict)
+        self.trainer.optimizer.load_state_dict(state_dict)
```

### Comparing `todd_ai-0.4.0/todd/scripts/merge_lmdbs.py` & `todd_ai-0.5.0/todd/scripts/merge_lmdbs.py`

 * *Files identical despite different names*

### Comparing `todd_ai-0.4.0/todd/visuals/base.py` & `todd_ai-0.5.0/todd/visuals/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,26 @@
 __all__ = [
-    'XAnchor',
-    'YAnchor',
     'BaseVisual',
 ]
 
-import enum
 from abc import ABC, abstractmethod
-from typing import Any, NamedTuple
+from typing import Any
 
 import cv2
 import numpy as np
 import numpy.typing as npt
 import torch
 
-
-class Color(NamedTuple):
-    red: float
-    green: float
-    blue: float
-
-
-class XAnchor(enum.Enum):
-    LEFT = enum.auto()
-    RIGHT = enum.auto()
-
-
-class YAnchor(enum.Enum):
-    TOP = enum.auto()
-    BOTTOM = enum.auto()
+from ..colors import PALETTE, RGB, Color
+from ..configs import Config
+from ..patches.cv2 import ColorMap
+from .anchors import XAnchor, YAnchor
 
 
 class BaseVisual(ABC):
-    PALETTE = [
-        Color(106, 0, 228),
-        Color(119, 11, 32),
-        Color(165, 42, 42),
-        Color(0, 0, 192),
-        Color(197, 226, 255),
-        Color(0, 60, 100),
-        Color(0, 0, 142),
-        Color(255, 77, 255),
-        Color(153, 69, 1),
-        Color(120, 166, 157),
-        Color(0, 182, 199),
-        Color(0, 226, 252),
-        Color(182, 182, 255),
-        Color(0, 0, 230),
-        Color(220, 20, 60),
-        Color(163, 255, 0),
-        Color(0, 82, 0),
-        Color(3, 95, 161),
-        Color(0, 80, 100),
-        Color(183, 130, 88),
-    ]
 
     @abstractmethod
     def __init__(self, width: int, height: int) -> None:
         pass
 
     @property
     @abstractmethod
@@ -65,60 +29,59 @@
 
     @property
     @abstractmethod
     def height(self) -> int:
         pass
 
     def color(self, index: int) -> Color:
-        index %= len(self.PALETTE)
-        return self.PALETTE[index]
+        index %= len(PALETTE)
+        return PALETTE[index]
 
     @abstractmethod
-    def save(self, path) -> None:
+    def save(self, path: Any) -> None:
         pass
 
     @abstractmethod
     def image(
         self,
         image: npt.NDArray[np.uint8],
         left: int = 0,
         top: int = 0,
         width: int | None = None,
         height: int | None = None,
         opacity: float = 1.0,
-    ):
+    ) -> Any:
         pass
 
     def activation(
         self,
         activation: torch.Tensor,
         left: int = 0,
         top: int = 0,
         width: int | None = None,
         height: int | None = None,
-        inverse: bool = False,
         opacity: float = 0.5,
-    ):
+    ) -> Any:
         """Draw the activation map.
 
         Suppose our activation map is :math:`(256, 13, 20)`, where 256 is the
-        number of channels, 13 is the height, and 20 is the width::
+        number of channels, 13 is the height, and 20 is the width:
 
             >>> activation = torch.rand(256, 13, 20)
 
-        We first reduce the channel dimension, using whatever reduction::
+        We first reduce the channel dimension, using whatever reduction:
 
             >>> import einops
             >>> activation = einops.reduce(
             ...     activation,
             ...     'c h w -> h w',
             ...     reduction='mean',
             ... )
 
-        Then we draw the activation map::
+        Then we draw the activation map:
 
             >>> from .pptx import PPTXVisual
             >>> visual = PPTXVisual(640, 426)
             >>> visual.activation(
             ...     activation,
             ...     width=visual.width,
             ...     height=visual.height,
@@ -127,68 +90,65 @@
 
         Args:
             activation: :math:`(H, W)` or :math:`(H, W, 1)`
             left: x coordinate of the left side of the activation map
             top: y coordinate of the top size of the activation map
             width: width of the activation map
             height: height of the activation map
-            inverse: invert the activation map or not
             opacity: opacity of the activation map
         """
-        activation = activation.detach()
-        activation -= activation.min()
-        activation /= activation.max()
-        if inverse:
-            activation = 1 - activation
-        activation *= 255
-        array: npt.NDArray = activation.cpu().numpy()
-        image: npt.NDArray[np.uint8] = array.astype(np.uint8)
-        image = cv2.applyColorMap(image, cv2.COLORMAP_JET)
+        color_map = ColorMap(cv2.COLORMAP_JET)
+        image = color_map(activation.detach())
         return self.image(image, left, top, width, height, opacity)
 
     @abstractmethod
     def rectangle(
         self,
         left: int,
         top: int,
         width: int,
         height: int,
-        color: Color = Color(0, 0, 0),
-    ):
+        color: Color = RGB(0., 0., 0.),  # noqa: B008
+        thickness: int = 1,
+        fill: Color | None = None,
+    ) -> Any:
         pass
 
     @abstractmethod
     def text(
         self,
         text: str,
         x: int,
         y: int,
         x_anchor: XAnchor = XAnchor.LEFT,
-        y_anchor: YAnchor = YAnchor.BOTTOM,
-        color: Color = Color(0, 0, 0),
-    ):
+        y_anchor: YAnchor = YAnchor.TOP,
+        color: Color = RGB(0., 0., 0.),  # noqa: B008
+        font: Config | None = None,
+    ) -> Any:
         pass
 
     def annotation(
         self,
         text: str,
         left: int,
         top: int,
         width: int,
         height: int,
-        color: Color = Color(0, 0, 0),
+        color: Color = RGB(0., 0., 0.),  # noqa: B008
+        thickness: int = 1,
+        font: Config | None = None,
     ) -> tuple[Any, Any]:
         """Draw an annotation bbox.
 
         Each annotation comprises a bbox and a textual label.
         The bbox is given by (left, top, width, height).
         The text is labeled above the bbox, left-aligned.
 
         The method is useful to visualize dataset annotations or pseudo
-        labels, for example::
+        labels, for example:
 
             >>> from .pptx import PPTXVisual
             >>> visual = PPTXVisual(640, 426)
             >>>
             >>> annotations = [
             ...     dict(bbox=[236.98, 142.51, 24.7, 69.5], category_id=64),
             ...     dict(bbox=[7.03, 167.76, 149.32, 94.87], category_id=72),
@@ -215,15 +175,23 @@
             width: width of the bbox
             height: height of the bbox
             color: color of the bbox
 
         Returns:
             tuple of the bbox and the text object
         """
-        rectangle = self.rectangle(left, top, width, height, color)
+        rectangle = self.rectangle(
+            left,
+            top,
+            width,
+            height,
+            color,
+            thickness,
+        )
         text_ = self.text(
             text,
             left,
-            top,
+            top + height,
             color=color,
+            font=font,
         )
-        return (rectangle, text_)
+        return rectangle, text_
```

### Comparing `todd_ai-0.4.0/todd/visuals/cv2.py` & `todd_ai-0.5.0/todd/visuals/cv2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,94 +1,117 @@
 __all__ = [
     'CV2Visual',
 ]
 
-from typing import cast
+from typing import Any
 
 import cv2
 import numpy as np
 import numpy.typing as npt
 
-from ..base import VisualRegistry
-from .base import BaseVisual, Color, XAnchor, YAnchor
+from ..colors import BGR, RGB, Color
+from ..configs import Config
+from ..registries import VisualRegistry
+from .anchors import XAnchor, YAnchor
+from .raster import RasterVisual
 
+Image = npt.NDArray[np.uint8]
 
-@VisualRegistry.register()
-class CV2Visual(BaseVisual):
 
-    def __init__(self, width: int, height: int) -> None:
-        self._image = np.zeros((height, width, 3))
+@VisualRegistry.register_()
+class CV2Visual(RasterVisual):
+
+    def __init__(
+        self,
+        width: int,
+        height: int,
+        channels: int = 3,
+        **kwargs,
+    ) -> None:
+        self._image = np.zeros(
+            (height, width, channels),
+            dtype=np.uint8,
+            **kwargs,
+        )
 
     @property
     def width(self) -> int:
         return self._image.shape[1]
 
     @property
     def height(self) -> int:
         return self._image.shape[0]
 
-    def save(self, path) -> None:
+    def save(self, path: Any) -> None:
         cv2.imwrite(path, self._image)
 
     def image(
         self,
-        image: npt.NDArray[np.uint8],
+        image: Image,
         left: int = 0,
         top: int = 0,
         width: int | None = None,
         height: int | None = None,
         opacity: float = 1.0,
-    ) -> npt.NDArray[np.uint8]:
-        h, w, c = image.shape
-        assert c == 3
+    ) -> Image:
+        assert 0.0 <= opacity <= 1.0
 
+        h, w, _ = image.shape
         if width is not None or height is not None:
-            if width is None:
-                width = round(w / h * cast(int, height))
-            if height is None:
-                height = round(h / w * cast(int, width))
-            image = cv2.resize(image, (width, height))
-            h, w, _ = image.shape
+            w, h = self._scale_wh((w, h), width, height)
+            image = cv2.resize(image, (w, h))
 
-        assert 0.0 <= opacity <= 1.0
         self._image[top:top + h, left:left + w] *= 1 - opacity
         self._image[top:top + h, left:left + w] += image * opacity
 
-        return self._image.astype(np.uint8)
+        return self._image
 
     def rectangle(
         self,
         left: int,
         top: int,
         width: int,
         height: int,
-        color: Color = Color(0, 0, 0),
-    ) -> npt.NDArray[np.uint8]:
-        cv2.rectangle(
+        color: Color = RGB(0., 0., 0.),  # noqa: B008
+        thickness: int = 1,
+        fill: Color | None = None,
+    ) -> Image:
+        args = (
             self._image,
             (left, top),
             (left + width, top + height),
-            color,
-            thickness=1,
         )
-        return self._image.astype(np.uint8)
+        if fill is not None:
+            cv2.rectangle(*args, fill.to(BGR).to_tuple(), thickness=-1)
+        cv2.rectangle(*args, color.to(BGR).to_tuple(), thickness=thickness)
+        return self._image
 
     def text(
         self,
         text: str,
         x: int,
         y: int,
         x_anchor: XAnchor = XAnchor.LEFT,
-        y_anchor: YAnchor = YAnchor.BOTTOM,
-        color: Color = Color(0, 0, 0),
-    ) -> npt.NDArray[np.uint8]:
-        assert x_anchor is XAnchor.LEFT
-        assert y_anchor is YAnchor.BOTTOM
+        y_anchor: YAnchor = YAnchor.TOP,
+        color: Color = RGB(0., 0., 0.),  # noqa: B008
+        font: Config | None = None,
+        thickness: int = 1,
+    ) -> Image:
+        if font is None:
+            font = Config()
+
+        font_face = font.get('face', cv2.FONT_HERSHEY_COMPLEX_SMALL)
+        font_scale = font.get('scale', 1.0)
+
+        wh, _ = cv2.getTextSize(text, font_face, font_scale, thickness)
+        xy = self._translate_xy(wh, x, y, x_anchor, y_anchor)
+
         cv2.putText(
             self._image,
-            text=text,
-            org=(x, y),
-            fontFace=cv2.FONT_HERSHEY_COMPLEX_SMALL,
-            fontScale=1.0,
-            color=color,
+            text,
+            xy,
+            font_face,
+            font_scale,
+            color.to(BGR).to_tuple(),
+            thickness,
         )
-        return self._image.astype(np.uint8)
+        return self._image
```

### Comparing `todd_ai-0.4.0/todd/visuals/pptx.py` & `todd_ai-0.5.0/todd/visuals/pptx.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 __all__ = [
     'PPTXVisual',
 ]
 
 import io
+from typing import Any
 
 import cv2
 import numpy as np
 import numpy.typing as npt
 import pptx
 import pptx.dml.color
 import pptx.enum.shapes
@@ -15,110 +16,130 @@
 import pptx.presentation
 import pptx.shapes.autoshape
 import pptx.shapes.picture
 import pptx.shapes.shapetree
 import pptx.slide
 import pptx.util
 
-from ..base import VisualRegistry
-from .base import BaseVisual, Color, XAnchor, YAnchor
+from ..colors import RGB, Color
+from ..configs import Config
+from ..loggers import logger
+from ..registries import VisualRegistry
+from .anchors import XAnchor, YAnchor
+from .base import BaseVisual
 
 
-@VisualRegistry.register()
+@VisualRegistry.register_()
 class PPTXVisual(BaseVisual):
     """Visualize data in the format of PowerPoint.
 
     The PowerPoint contains only one slide.
     For more details, refer to python-pptx_.
 
     .. _python-pptx: https://github.com/scanny/python-pptx
     """
 
-    def __init__(self, width: int, height: int) -> None:
-        """Initializes the PowerPoint with a single slide.
+    def __init__(self, width: int, height: int, **kwargs) -> None:
+        """Initialize the PowerPoint with a single slide.
 
         To initialize a PowerPoint with width 640pt and height 426pt, use the
-        following code::
+        following code:
 
             >>> visual = PPTXVisual(640, 426)
 
         Once initialized, the width and height of the slide cannot be altered.
-        We can read the width and height of the PowerPoint by::
+        We can read the width and height of the PowerPoint by:
 
             >>> visual.width
             640
             >>> visual.height
             426
 
         Args:
             width: the width of the PowerPoint in point
             height: the height of the PowerPoint in point
         """
-        super().__init__(width, height)
+        self._presentation = pptx.Presentation(**kwargs)
 
-        pre: pptx.presentation.Presentation = pptx.Presentation()
-        pre.slide_width = pptx.util.Pt(width)
-        pre.slide_height = pptx.util.Pt(height)
-
-        layout: pptx.slide.SlideLayout = pre.slide_layouts[6]
-        slides: pptx.slide.Slides = pre.slides
-        slide: pptx.slide.Slide = slides.add_slide(layout)
-        shapes: pptx.shapes.shapetree.SlideShapes = slide.shapes
+        self.presentation.slide_width = pptx.util.Pt(width)
+        self.presentation.slide_height = pptx.util.Pt(height)
 
-        self._pre = pre
-        self._shapes = shapes
+        slides: pptx.slide.Slides = self.presentation.slides
+        slides.add_slide(self.presentation.slide_layouts[6])
 
     @property
     def width(self) -> int:
         """Width of the PowerPoint."""
-        width: pptx.util.Pt = self._pre.slide_width
+        width: pptx.util.Pt = self.presentation.slide_width
         return int(width.pt)
 
     @property
     def height(self) -> int:
         """Height of the PowerPoint."""
-        height: pptx.util.Pt = self._pre.slide_height
+        height: pptx.util.Pt = self.presentation.slide_height
         return int(height.pt)
 
-    def save(self, path) -> None:
+    @property
+    def presentation(self) -> pptx.presentation.Presentation:
+        return self._presentation
+
+    @property
+    def slide(self) -> pptx.slide.Slide:
+        return self.presentation.slides[0]
+
+    @property
+    def shapes(self) -> pptx.shapes.shapetree.SlideShapes:
+        return self.slide.shapes
+
+    @classmethod
+    def _set_color_format_rgb(
+        cls,
+        cf: pptx.dml.color.ColorFormat,
+        color: Color,
+    ) -> None:
+        cf.rgb = pptx.dml.color.RGBColor(
+            *color.to(RGB).to_tuple(),
+        )
+
+    def save(self, path: Any) -> None:
         """Save the PowerPoint.
 
-        The save target can either be a filepath, for example::
+        The save target can either be a filepath, for example:
 
             >>> import tempfile
             >>> with tempfile.NamedTemporaryFile() as f:
             ...     PPTXVisual(640, 426).save(f.name)
 
-        Or it can simply be a file-like object::
+        Or it can simply be a file-like object:
 
             >>> with tempfile.TemporaryFile() as f:
             ...     PPTXVisual(640, 426).save(f)
 
         Args:
             path: destination path
         """
-        self._pre.save(path)
+        self.presentation.save(path)
 
     def image(
         self,
         image: npt.NDArray[np.uint8],
         left: int = 0,
         top: int = 0,
         width: int | None = None,
         height: int | None = None,
         opacity: float = 1.0,
     ) -> pptx.shapes.picture.Picture:
         """Add an image to the PowerPoint.
 
-        Suppose the image is :math:`(426, 640)`::
+        Suppose the image is :math:`(426, 640)`:
 
             >>> image = np.random.randint(0, 256, (426, 640, 3))
 
         In most cases, the PowerPoint is of the same size as the image, so
-        that the image covers the whole background::
+        that the image covers the whole background:
 
             >>> h, w, _ = image.shape
             >>> visual = PPTXVisual(w, h)
             >>> visual.image(image)
             <pptx.shapes.picture.Picture object at ...>
 
         The returned `pptx.shapes.picture.Picture` object can be used to
@@ -136,116 +157,106 @@
             image: :math:`(H, W, 3)`
             left: x coordinate of the left side of the image
             top: y coordinate of the top side of the image
             width: width of the image
             height: height of the image
             opacity: opacity of the image
         """
+        assert 0.0 <= opacity <= 1.0
+
         h, w, c = image.shape
         assert c == 3
 
-        left_pixels = pptx.util.Pt(left)
-        top_pixels = pptx.util.Pt(top)
-        width_pixels = width if width is None else pptx.util.Pt(width)
-        height_pixels = height if height is None else pptx.util.Pt(height)
-
-        assert 0.0 <= opacity <= 1.0
-
         alpha = np.ones((h, w, 1)) * 255 * opacity
         image = np.concatenate([image, alpha], axis=-1)
         status, image = cv2.imencode('.png', image)
         assert status
-        bytes_io = io.BytesIO(image.tobytes())
-        picture = self._shapes.add_picture(
-            bytes_io,
-            left_pixels,
-            top_pixels,
-            width_pixels,
-            height_pixels,
+
+        picture = self.shapes.add_picture(
+            io.BytesIO(image.tobytes()),
+            pptx.util.Pt(left),
+            pptx.util.Pt(top),
+            width if width is None else pptx.util.Pt(width),
+            height if height is None else pptx.util.Pt(height),
         )
 
-        image_part: pptx.parts.image.Image = picture.image
-        assert image_part.dpi == (72, 72)
+        picture_image: pptx.parts.image.Image = picture.image
+        assert picture_image.dpi == (72, 72)
 
         return picture
 
     def rectangle(
         self,
         left: int,
         top: int,
         width: int,
         height: int,
-        color: Color = Color(0, 0, 0),
+        color: Color = RGB(0., 0., 0.),  # noqa: B008
+        thickness: int = 1,
+        fill: Color | None = None,
     ) -> pptx.shapes.autoshape.Shape:
-        rectangle: pptx.shapes.autoshape.Shape = self._shapes.add_shape(
-            pptx.enum.shapes.MSO_AUTO_SHAPE_TYPE.RECTANGLE,
+        rectangle: pptx.shapes.autoshape.Shape = self.shapes.add_shape(
+            pptx.enum.shapes.MSO_AUTO_SHAPE_TYPE.RECTANGLE,  # noqa: E501 pylint: disable=no-member
             pptx.util.Pt(left),
             pptx.util.Pt(top),
             pptx.util.Pt(width),
             pptx.util.Pt(height),
         )
 
-        fill: pptx.shapes.autoshape.FillFormat = rectangle.fill
-        fill.background()
-
         line: pptx.shapes.autoshape.LineFormat = rectangle.line
-        line.width = pptx.util.Pt(1)
+        line.width = pptx.util.Pt(thickness)
+        self._set_color_format_rgb(line.color, color)
 
-        line_color: pptx.dml.color.ColorFormat = line.color
-        line_color.rgb = pptx.dml.color.RGBColor(*color)
+        rectangle_fill: pptx.shapes.autoshape.FillFormat = rectangle.fill
+        if fill is None:
+            rectangle_fill.background()
+        else:
+            rectangle_fill.solid()
+            self._set_color_format_rgb(rectangle_fill.fore_color, fill)
 
         return rectangle
 
     def text(
         self,
         text: str,
         x: int,
         y: int,
         x_anchor: XAnchor = XAnchor.LEFT,
-        y_anchor: YAnchor = YAnchor.BOTTOM,
-        color: Color = Color(0, 0, 0),
+        y_anchor: YAnchor = YAnchor.TOP,
+        color: Color = RGB(0., 0., 0.),  # noqa: B008
+        font: Config | None = None,
     ) -> pptx.shapes.autoshape.Shape:
-        width = pptx.util.Pt(9 * len(text))
-        height = pptx.util.Pt(15)
-
-        if x_anchor is XAnchor.LEFT:
-            left = pptx.util.Pt(x)
-        elif x_anchor is XAnchor.RIGHT:
-            left = pptx.util.Pt(x) - width
-        else:
-            raise ValueError(f"Unsupported anchor {x_anchor}")
-
-        if y_anchor is YAnchor.TOP:
-            top = pptx.util.Pt(y)
-        elif y_anchor is YAnchor.BOTTOM:
-            top = pptx.util.Pt(y) - height
-        else:
-            raise ValueError(f"Unsupported anchor {y_anchor}")
-
-        textbox: pptx.shapes.autoshape.Shape = self._shapes.add_textbox(
-            left,
-            top,
-            width,
-            height,
+        if x_anchor is not XAnchor.LEFT:
+            logger.warning(
+                "%s does not support %s",
+                self.__class__.__name__,
+                f"{x_anchor=}",
+            )
+        if y_anchor is not YAnchor.TOP:
+            logger.warning(
+                "%s does not support %s",
+                self.__class__.__name__,
+                f"{y_anchor=}",
+            )
+        if font is None:
+            font = Config()
+
+        textbox: pptx.shapes.autoshape.Shape = self.shapes.add_textbox(
+            pptx.util.Pt(x),
+            pptx.util.Pt(y),
+            1,
+            1,
         )
 
         text_frame = textbox.text_frame
+        text_frame.text = text
         text_frame.margin_left = 0
         text_frame.margin_top = 0
         text_frame.margin_right = 0
         text_frame.margin_bottom = 0
-        text_frame.vertical_anchor = getattr(
-            pptx.enum.text.MSO_VERTICAL_ANCHOR,
-            y_anchor.name,
-        )
-
-        paragraph = text_frame.paragraphs[0]
-        paragraph.text = text
-
-        font = paragraph.font
-        font.name = 'Times New Roman'
-        font.size = pptx.util.Pt(12)
 
-        font_color: pptx.dml.color.ColorFormat = font.color
-        font_color.rgb = pptx.dml.color.RGBColor(*color)
+        paragraph_font = text_frame.paragraphs[0].font
+        paragraph_font.name = font.get('name', 'Times New Roman')
+        paragraph_font.size = pptx.util.Pt(font.get('size', 12))
+        self._set_color_format_rgb(paragraph_font.color, color)
 
         return textbox
```

### Comparing `todd_ai-0.4.0/todd_ai.egg-info/PKG-INFO` & `todd_ai-0.5.0/todd_ai.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: todd-ai
-Version: 0.4.0
+Name: todd_ai
+Version: 0.5.0
 Summary: Toolkit for Object Detection Distillation
 Author-email: Luting Wang <wangluting@buaa.edu.cn>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -206,20 +206,63 @@
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/LutingWang/todd
 Project-URL: Documentation, https://toddai.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: einops
+Requires-Dist: ffmpeg-python
+Requires-Dist: lmdb
+Requires-Dist: opencv-python
+Requires-Dist: pandas
+Requires-Dist: python-pptx
+Requires-Dist: tensorboard
+Requires-Dist: timm
+Requires-Dist: toml
+Requires-Dist: typing_extensions
+Requires-Dist: yapf
 Provides-Extra: dev
+Requires-Dist: autoflake; extra == "dev"
+Requires-Dist: bandit[toml]; extra == "dev"
+Requires-Dist: codespell; extra == "dev"
+Requires-Dist: commitizen; extra == "dev"
+Requires-Dist: doc8; extra == "dev"
+Requires-Dist: docformatter[tomli]; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: flake8-bugbear; extra == "dev"
+Requires-Dist: flake8-docstrings; extra == "dev"
+Requires-Dist: ipdb; extra == "dev"
+Requires-Dist: ipykernel; extra == "dev"
+Requires-Dist: jupyter; extra == "dev"
+Requires-Dist: matplotlib; extra == "dev"
+Requires-Dist: mccabe; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pandas-stubs; extra == "dev"
+Requires-Dist: pep8-naming; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pydocstyle; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
+Requires-Dist: torch-tb-profiler; extra == "dev"
+Requires-Dist: tqdm; extra == "dev"
+Requires-Dist: types-Pillow; extra == "dev"
+Requires-Dist: types-toml; extra == "dev"
+Requires-Dist: types-tqdm; extra == "dev"
 Provides-Extra: doc
+Requires-Dist: mmcv<2.0; extra == "doc"
+Requires-Dist: python-docs-theme; extra == "doc"
+Requires-Dist: sphinx; extra == "doc"
+Requires-Dist: sphinx_rtd_theme; extra == "doc"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: coverage; extra == "test"
+Requires-Dist: mmcv<2.0; extra == "test"
+Requires-Dist: pytest; extra == "test"
 
 # Toolkit for Object Detection Distillation
 
 ```text
 _/_/_/_/_/                _/        _/
    _/      _/_/      _/_/_/    _/_/_/
   _/    _/    _/  _/    _/  _/    _/
@@ -228,15 +271,15 @@
 ```
 
 [![docs](https://readthedocs.org/projects/toddai/badge/?version=latest)](https://toddai.readthedocs.io/en/latest/?badge=latest)
 [![lint](https://github.com/LutingWang/todd/actions/workflows/lint.yaml/badge.svg)](https://github.com/LutingWang/todd/actions/workflows/lint.yaml)
 [![test](https://github.com/LutingWang/todd/actions/workflows/test.yaml/badge.svg)](https://github.com/LutingWang/todd/actions/workflows/test.yaml)
 [![publish](https://github.com/LutingWang/todd/actions/workflows/publish.yaml/badge.svg)](https://github.com/LutingWang/todd/actions/workflows/publish.yaml)
 
-[![codecov](https://codecov.io/gh/LutingWang/todd/branch/master/graph/badge.svg?token=BHDPCKVM1T)](https://codecov.io/gh/LutingWang/todd)
+[![codecov](https://codecov.io/gh/LutingWang/todd/branch/main/graph/badge.svg?token=BHDPCKVM1T)](https://codecov.io/gh/LutingWang/todd)
 [![PyPI](https://img.shields.io/pypi/v/todd_ai)](https://pypi.org/project/todd-ai/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/todd_ai)]((https://pypi.org/project/todd-ai/))
 [![wakatime](https://wakatime.com/badge/github/LutingWang/todd.svg)](https://wakatime.com/badge/github/LutingWang/todd)
 
 ## Installation
 
 Prerequisites:
@@ -253,8 +296,14 @@
 
 ```bash
 pip install .\[dev,doc,test\]
 ```
 
 TODO
 
-1. Complete repr
+1. Complete repr, especially for runners
+2. mypy supports recursive types
+3. add a script to prepare imagenet dataset
+4. add Any to all missing typing fields
+5. make loss registry a sub-registry of model registry
+6. refactor registries
+7. remove odpsrun
```

