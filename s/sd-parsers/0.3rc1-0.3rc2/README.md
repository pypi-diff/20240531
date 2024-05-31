# Comparing `tmp/sd-parsers-0.3rc1.tar.gz` & `tmp/sd-parsers-0.3rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sd-parsers-0.3rc1.tar", last modified: Thu Dec  7 21:30:52 2023, max compression
+gzip compressed data, was "sd-parsers-0.3rc2.tar", last modified: Sun Dec 10 01:08:14 2023, max compression
```

## Comparing `sd-parsers-0.3rc1.tar` & `sd-parsers-0.3rc2.tar`

### file list

```diff
@@ -1,71 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:30:52.449008 sd-parsers-0.3rc1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:30:52.437008 sd-parsers-0.3rc1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:30:52.441008 sd-parsers-0.3rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/.github/workflows/publish-to.pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      628 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2023-12-07 21:30:52.449008 sd-parsers-0.3rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:30:52.441008 sd-parsers-0.3rc1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/examples/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/examples/deep_dive.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/examples/fast_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    14710 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/pdm.lock
--rw-r--r--   0 runner    (1001) docker     (127)      805 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-07 21:30:52.449008 sd-parsers-0.3rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:30:52.437008 sd-parsers-0.3rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:30:52.441008 sd-parsers-0.3rc1/src/sd_parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/src/sd_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/src/sd_parsers/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/src/sd_parsers/_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4640 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/src/sd_parsers/_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/src/sd_parsers/_parser_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/src/sd_parsers/_prompt_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:30:52.445008 sd-parsers-0.3rc1/src/sd_parsers/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/src/sd_parsers/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/src/sd_parsers/parsers/_automatic1111.py
--rw-r--r--   0 runner    (1001) docker     (127)     8569 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/src/sd_parsers/parsers/_comfyui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/src/sd_parsers/parsers/_dummy_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/src/sd_parsers/parsers/_invokeai.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/src/sd_parsers/parsers/_managed_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/src/sd_parsers/parsers/_novelai.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/src/sd_parsers/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:30:52.449008 sd-parsers-0.3rc1/src/sd_parsers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2023-12-07 21:30:52.000000 sd-parsers-0.3rc1/src/sd_parsers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2023-12-07 21:30:52.000000 sd-parsers-0.3rc1/src/sd_parsers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-07 21:30:52.000000 sd-parsers-0.3rc1/src/sd_parsers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-12-07 21:30:52.000000 sd-parsers-0.3rc1/src/sd_parsers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-07 21:30:52.000000 sd-parsers-0.3rc1/src/sd_parsers.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:30:52.445008 sd-parsers-0.3rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:30:52.437008 sd-parsers-0.3rc1/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:30:52.445008 sd-parsers-0.3rc1/tests/resources/bad_images/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/tests/resources/bad_images/empty_file.png
--rw-r--r--   0 runner    (1001) docker     (127)      585 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/tests/resources/bad_images/text_after_idat.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:30:52.437008 sd-parsers-0.3rc1/tests/resources/parsers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:30:52.445008 sd-parsers-0.3rc1/tests/resources/parsers/AUTOMATIC1111/
--rw-r--r--   0 runner    (1001) docker     (127)      705 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/tests/resources/parsers/AUTOMATIC1111/automatic1111_cropped.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      272 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/tests/resources/parsers/AUTOMATIC1111/automatic1111_cropped.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:30:52.449008 sd-parsers-0.3rc1/tests/resources/parsers/ComfyUI/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/tests/resources/parsers/ComfyUI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/tests/resources/parsers/ComfyUI/img2img_cropped.png
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/tests/resources/parsers/ComfyUI/img2img_cropped.py
--rw-r--r--   0 runner    (1001) docker     (127)    17446 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/tests/resources/parsers/ComfyUI/night_evening_day_morning_cropped.png
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/tests/resources/parsers/ComfyUI/night_evening_day_morning_cropped.py
--rw-r--r--   0 runner    (1001) docker     (127)    21184 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/tests/resources/parsers/ComfyUI/noisy_latents_3_subjects_cropped.png
--rw-r--r--   0 runner    (1001) docker     (127)    13981 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/tests/resources/parsers/ComfyUI/unclip_2pass_cropped.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:30:52.449008 sd-parsers-0.3rc1/tests/resources/parsers/InvokeAI/
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/tests/resources/parsers/InvokeAI/invokeai1_cropped.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:30:52.449008 sd-parsers-0.3rc1/tests/resources/parsers/NovelAI/
--rw-r--r--   0 runner    (1001) docker     (127)      780 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/tests/resources/parsers/NovelAI/novelai1_cropped.png
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/tests/test_automatic1111.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/tests/test_comfyui.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/tests/test_invokeai.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/tests/test_novelai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/tests/test_parser_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 21:30:52.449008 sd-parsers-0.3rc1/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/tests/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/tests/tools/crop_image.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      264 2023-12-07 21:30:42.000000 sd-parsers-0.3rc1/tests/tools/crop_image.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 01:08:14.650519 sd-parsers-0.3rc2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 01:08:14.642519 sd-parsers-0.3rc2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 01:08:14.642519 sd-parsers-0.3rc2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/.github/workflows/publish-to.pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2023-12-10 01:08:14.650519 sd-parsers-0.3rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 01:08:14.642519 sd-parsers-0.3rc2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/examples/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/examples/deep_dive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/examples/fast_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14710 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/pdm.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-10 01:08:14.650519 sd-parsers-0.3rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 01:08:14.642519 sd-parsers-0.3rc2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 01:08:14.646519 sd-parsers-0.3rc2/src/sd_parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/src/sd_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/src/sd_parsers/_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/src/sd_parsers/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/src/sd_parsers/_parser_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/src/sd_parsers/_prompt_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/src/sd_parsers/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 01:08:14.646519 sd-parsers-0.3rc2/src/sd_parsers/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/src/sd_parsers/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/src/sd_parsers/parsers/_automatic1111.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8600 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/src/sd_parsers/parsers/_comfyui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/src/sd_parsers/parsers/_dummy_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6521 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/src/sd_parsers/parsers/_invokeai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/src/sd_parsers/parsers/_managed_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/src/sd_parsers/parsers/_novelai.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/src/sd_parsers/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 01:08:14.650519 sd-parsers-0.3rc2/src/sd_parsers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2023-12-10 01:08:14.000000 sd-parsers-0.3rc2/src/sd_parsers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2023-12-10 01:08:14.000000 sd-parsers-0.3rc2/src/sd_parsers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-10 01:08:14.000000 sd-parsers-0.3rc2/src/sd_parsers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2023-12-10 01:08:14.000000 sd-parsers-0.3rc2/src/sd_parsers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-10 01:08:14.000000 sd-parsers-0.3rc2/src/sd_parsers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 01:08:14.646519 sd-parsers-0.3rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 01:08:14.642519 sd-parsers-0.3rc2/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 01:08:14.650519 sd-parsers-0.3rc2/tests/resources/bad_images/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/tests/resources/bad_images/empty_file.png
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/tests/resources/bad_images/text_after_idat.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 01:08:14.642519 sd-parsers-0.3rc2/tests/resources/parsers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 01:08:14.650519 sd-parsers-0.3rc2/tests/resources/parsers/AUTOMATIC1111/
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/tests/resources/parsers/AUTOMATIC1111/automatic1111_cropped.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/tests/resources/parsers/AUTOMATIC1111/automatic1111_cropped.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 01:08:14.650519 sd-parsers-0.3rc2/tests/resources/parsers/ComfyUI/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/tests/resources/parsers/ComfyUI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/tests/resources/parsers/ComfyUI/img2img_cropped.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/tests/resources/parsers/ComfyUI/img2img_cropped.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17446 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/tests/resources/parsers/ComfyUI/night_evening_day_morning_cropped.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4861 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/tests/resources/parsers/ComfyUI/night_evening_day_morning_cropped.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21184 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/tests/resources/parsers/ComfyUI/noisy_latents_3_subjects_cropped.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13981 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/tests/resources/parsers/ComfyUI/unclip_2pass_cropped.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 01:08:14.650519 sd-parsers-0.3rc2/tests/resources/parsers/InvokeAI/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/tests/resources/parsers/InvokeAI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/tests/resources/parsers/InvokeAI/invokeai_dream1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/tests/resources/parsers/InvokeAI/invokeai_dream1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/tests/resources/parsers/InvokeAI/invokeai_imeta1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/tests/resources/parsers/InvokeAI/invokeai_imeta1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/tests/resources/parsers/InvokeAI/invokeai_sdmeta1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/tests/resources/parsers/InvokeAI/invokeai_sdmeta1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 01:08:14.650519 sd-parsers-0.3rc2/tests/resources/parsers/NovelAI/
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/tests/resources/parsers/NovelAI/novelai1_cropped.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/tests/test_automatic1111.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/tests/test_comfyui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/tests/test_invokeai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/tests/test_novelai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/tests/test_parser_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 01:08:14.650519 sd-parsers-0.3rc2/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/tests/tools/crop_image.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      264 2023-12-10 01:08:06.000000 sd-parsers-0.3rc2/tests/tools/crop_image.sh
```

### Comparing `sd-parsers-0.3rc1/.github/workflows/publish-to.pypi.yml` & `sd-parsers-0.3rc2/.github/workflows/publish-to.pypi.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 name: Publish to PyPI
 on:
   push:
-    branches:
-      - master
     tags:
       - "v*"
 
 jobs:
   publish:
     name: Build and Publish to PyPI
     runs-on: ubuntu-latest
```

### Comparing `sd-parsers-0.3rc1/.github/workflows/test.yml` & `sd-parsers-0.3rc2/.github/workflows/test.yml`

 * *Files 3% similar despite different names*

```diff
@@ -21,11 +21,11 @@
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         pdm install -d
     - name: Lint with ruff
       run: |
-        pdm run ruff check --extend-select=D403 .
+        pdm run ruff check src
     - name: Test with pytest
       run: |
         pdm run pytest -v
```

### Comparing `sd-parsers-0.3rc1/LICENSE.txt` & `sd-parsers-0.3rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.3rc1/PKG-INFO` & `sd-parsers-0.3rc2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd-parsers
-Version: 0.3rc1
+Version: 0.3rc2
 Summary: a library to read metadata from images created by Stable Diffusion
 Author: d3x-at
 License: MIT License
         
         Copyright (c) 2023 d3x-at
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,14 +26,20 @@
         SOFTWARE.
 Project-URL: repository, https://github.com/d3x-at/sd-parsers
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: Pillow>=8.3.1
 
+> [!IMPORTANT]  
+> A release candidate featuring a revisited API and extended ComfyUI & InvokeAI parsing logic is available.
+> 
+> See [release notes](https://github.com/d3x-at/sd-parsers/releases/tag/v0.3rc2) for changes.
+>
+> Install with: ```pip install --upgrade --pre sd-parsers```
 
 ## Features
 
 Supports reading metadata from images generated with:
 * Automatic1111's Stable Diffusion web UI
 * ComfyUI *
 * InvokeAI
@@ -75,15 +81,15 @@
     prompt_info = parser_manager.parse(image)
 ```
 
 Each parser module can also be used directly, omitting the use of ```ParserManager```:
 
 ```python
 from PIL import Image
-from sd_parsers import ParserError
+from sd_parsers.exceptions import ParserError
 from sd_parsers.parsers import AUTOMATIC1111Parser
 
 parser = AUTOMATIC1111Parser()
 with Image.open("image.png") as image:
     prompt_info, error = parser.read_parameters(image)
     
     if prompt_info:
```

### Comparing `sd-parsers-0.3rc1/README.md` & `sd-parsers-0.3rc2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+> [!IMPORTANT]  
+> A release candidate featuring a revisited API and extended ComfyUI & InvokeAI parsing logic is available.
+> 
+> See [release notes](https://github.com/d3x-at/sd-parsers/releases/tag/v0.3rc2) for changes.
+>
+> Install with: ```pip install --upgrade --pre sd-parsers```
 
 ## Features
 
 Supports reading metadata from images generated with:
 * Automatic1111's Stable Diffusion web UI
 * ComfyUI *
 * InvokeAI
@@ -43,15 +49,15 @@
     prompt_info = parser_manager.parse(image)
 ```
 
 Each parser module can also be used directly, omitting the use of ```ParserManager```:
 
 ```python
 from PIL import Image
-from sd_parsers import ParserError
+from sd_parsers.exceptions import ParserError
 from sd_parsers.parsers import AUTOMATIC1111Parser
 
 parser = AUTOMATIC1111Parser()
 with Image.open("image.png") as image:
     prompt_info, error = parser.read_parameters(image)
     
     if prompt_info:
@@ -83,8 +89,8 @@
 
 
 ## Credits
 Idea and motivation using AUTOMATIC1111's stable diffusion webui
 - https://github.com/AUTOMATIC1111/stable-diffusion-webui
 
 Example workflows for testing the ComfyUI parser
-- https://github.com/comfyanonymous/ComfyUI_examples
+- https://github.com/comfyanonymous/ComfyUI_examples
```

### Comparing `sd-parsers-0.3rc1/examples/cmdline.py` & `sd-parsers-0.3rc2/examples/cmdline.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.3rc1/examples/deep_dive.py` & `sd-parsers-0.3rc2/examples/deep_dive.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.3rc1/examples/fast_api.py` & `sd-parsers-0.3rc2/examples/fast_api.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.3rc1/pdm.lock` & `sd-parsers-0.3rc2/pdm.lock`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.3rc1/pyproject.toml` & `sd-parsers-0.3rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.3rc1/src/sd_parsers/__init__.py` & `sd-parsers-0.3rc2/src/sd_parsers/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,23 +12,21 @@
 prompt_info = parser_manager.parse("image.png")
 
 if prompt_info is not None:
     for prompt in prompt_info.prompts:
         print(prompt.value)
 
 """
-from ._exceptions import ParserError
 from ._models import Model, Prompt, Sampler
 from ._parser import Generators, Parser
 from ._parser_manager import ParserManager
 from ._prompt_info import PromptInfo
 
 __all__ = [
     "Parser",
     "Generators",
     "ParserManager",
-    "ParserError",
     "PromptInfo",
     "Model",
     "Prompt",
     "Sampler",
 ]
```

### Comparing `sd-parsers-0.3rc1/src/sd_parsers/_models.py` & `sd-parsers-0.3rc2/src/sd_parsers/_models.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,32 +5,36 @@
 
 @dataclass(frozen=True)
 class Prompt:
     """Represents an image generation prompt."""
 
     value: str
     """The value of the prompt."""
+
     prompt_id: Optional[int] = None
-    """prompt id"""
-    weight: Optional[float] = None
-    """Prompt weight. (Specific to InvokeAI for now)"""
+    """Prompt id"""
+
+    parameters: Dict[str, Any] = field(default_factory=dict)
+    """Additional prompt parameters"""
 
     def __hash__(self) -> int:
         return hash((self.prompt_id, self.value))
 
 
 @dataclass(frozen=True)
 class Model:
     """Represents a model used during image generation."""
 
     model_id: Optional[int] = None
     name: Optional[str] = None
-    config: Optional[str] = None
     model_hash: Optional[str] = None
 
+    parameters: Dict[str, Any] = field(default_factory=dict)
+    """Additional model parameters"""
+
     def __hash__(self) -> int:
         return hash((self.model_id, self.name))
 
 
 @dataclass
 class Sampler:
     """Represents a model used during image generation."""
```

### Comparing `sd-parsers-0.3rc1/src/sd_parsers/_parser.py` & `sd-parsers-0.3rc2/src/sd_parsers/_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,31 +63,37 @@
     def parse(self, parameters: Dict[str, Any]) -> ParseResult:
         """Extract image generation information from the image metadata."""
 
     def normalize_parameters(
         self,
         parameters: Union[Dict[str, Any], Iterable[Tuple[str, Any]]],
         replacement_rules: Optional[ReplacementRules] = None,
+        to_lowercase=True,
+        replace_whitespace=True,
     ) -> Dict[str, Any]:
         """
         Apply replacement rules and basic formatting to the keys of select image metadata entries.
 
         Returns a dictionary with normalized parameter values.
 
         Override to alter the applied standardization logic.
         """
         if self.do_normalization_pass:
-            return _normalize_parameters(parameters, replacement_rules)
+            return _normalize_parameters(
+                parameters, replacement_rules, to_lowercase, replace_whitespace
+            )
 
         return parameters if isinstance(parameters, dict) else dict(parameters)  # type: ignore
 
 
 def _normalize_parameters(
     parameters: Union[Dict[str, Any], Iterable[Tuple[str, Any]]],
     replacement_rules: Optional[ReplacementRules] = None,
+    to_lowercase=True,
+    replace_whitespace=True,
 ) -> Dict[str, Any]:
     """
     Apply replacement rules and basic formatting to the keys of select image metadata entries.
 
     Returns a dictionary with normalized parameter values.
     """
 
@@ -105,17 +111,22 @@
             else:
                 format_values, format_string = instruction
                 with suppress(KeyError):
                     processed[property_key] = format_string.format(
                         **{key: raw_props[key] for key in format_values}
                     )
 
-    # remaining (unchanged) items
-    for property_key, value in raw_props.items():
-        processed[property_key.lower().replace(" ", "_")] = value
+    for key, value in raw_props.items():
+        if to_lowercase:
+            key = key.lower()
+
+        if replace_whitespace:
+            key = key.replace(" ", "_")
+
+        processed[key] = value
 
     return processed
 
 
 def get_exif_value(
     image: Image,
     key: str,
```

### Comparing `sd-parsers-0.3rc1/src/sd_parsers/_parser_manager.py` & `sd-parsers-0.3rc2/src/sd_parsers/_parser_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Provides the ParserManager class."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, List, Optional, Union
 
 from PIL import Image
 
-from ._exceptions import ParserError
 from ._parser import Parser
 from ._prompt_info import PromptInfo
+from .exceptions import ParserError
 from .parsers._managed_parsers import MANAGED_PARSERS
 
 if TYPE_CHECKING:
     from pathlib import Path
 
     from _typeshed import SupportsRead
```

### Comparing `sd-parsers-0.3rc1/src/sd_parsers/_prompt_info.py` & `sd-parsers-0.3rc2/src/sd_parsers/_prompt_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Provides the PromptInfo class."""
 from __future__ import annotations
 
 import itertools
 import logging
 from typing import TYPE_CHECKING, Any, Dict, List, Set
 
-from ._exceptions import ParserError
+from .exceptions import ParserError
 
 if TYPE_CHECKING:
     from ._models import Model, Prompt, Sampler
     from ._parser import Generators, Parser
 
 logger = logging.getLogger(__name__)
```

### Comparing `sd-parsers-0.3rc1/src/sd_parsers/parsers/_automatic1111.py` & `sd-parsers-0.3rc2/src/sd_parsers/parsers/_automatic1111.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import re
 from contextlib import suppress
 from typing import Any, Dict
 
 from PIL.Image import Image
 from PIL.PngImagePlugin import PngImageFile
 
-from .._exceptions import ParserError
 from .._models import Model, Prompt, Sampler
 from .._parser import Generators, Parser, ParseResult, get_exif_value, pop_keys
 from .._prompt_info import PromptInfo
+from ..exceptions import ParserError
 from ._managed_parsers import MANAGED_PARSERS
 
 SAMPLER_PARAMS = ["Sampler", "CFG scale", "Seed", "Steps", "ENSD"]
 
 
 class AUTOMATIC1111Parser(Parser):
     """parse images created in AUTOMATIC1111's webui"""
```

### Comparing `sd-parsers-0.3rc1/src/sd_parsers/parsers/_comfyui.py` & `sd-parsers-0.3rc2/src/sd_parsers/parsers/_comfyui.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from collections import defaultdict
 from contextlib import suppress
 from typing import Any, Dict, Generator, List, Optional, Set, Tuple
 
 from PIL.Image import Image
 from PIL.PngImagePlugin import PngImageFile
 
-from .._exceptions import ParserError
 from .._models import Model, Prompt, Sampler
 from .._parser import Generators, Parser, ParseResult
 from .._prompt_info import PromptInfo
+from ..exceptions import ParserError
 from ._managed_parsers import MANAGED_PARSERS
 
 logger = logging.getLogger(__name__)
 
 SAMPLER_PARAMS = {"sampler_name", "steps", "cfg"}
 POSITIVE_PROMPT_KEYS = ["text", "positive"]
 NEGATIVE_PROMPT_KEYS = ["text", "negative"]
@@ -42,15 +42,15 @@
         return PromptInfo(self, {"prompt": prompt, "workflow": workflow}), None
 
     def parse(self, parameters: Dict[str, Any]) -> ParseResult:
         try:
             prompt = parameters["prompt"]
             workflow = parameters["workflow"]
         except KeyError as error:
-            raise ParserError("error reading prameters") from error
+            raise ParserError("error reading parameters") from error
 
         samplers, metadata = ImageContext.extract(self, prompt, workflow)
         return samplers, metadata
 
 
 class ImageContext:
     parser: ComfyUIParser
@@ -183,19 +183,21 @@
                 inputs = node["inputs"]
                 ckpt_name = inputs["ckpt_name"]
             except KeyError:
                 pass
             else:
                 self.processed_nodes.add(node_id)
                 logger.debug("found model #%d: %s", node_id, ckpt_name)
-                return Model(
-                    name=ckpt_name,
-                    model_id=node_id,
-                    config=inputs.get("config_name", None),
-                )
+
+                model = Model(model_id=node_id, name=ckpt_name)
+
+                with suppress(KeyError):
+                    model.parameters["config_name"] = inputs["config_name"]
+
+                return model
 
         return None
 
     def _try_get_sampler(self, node_id: int, node):
         """Test if this node could contain sampler data"""
         try:
             if not SAMPLER_PARAMS.issubset(node["inputs"]):
```

### Comparing `sd-parsers-0.3rc1/src/sd_parsers/parsers/_dummy_parser.py` & `sd-parsers-0.3rc2/src/sd_parsers/parsers/_dummy_parser.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.3rc1/src/sd_parsers/parsers/_novelai.py` & `sd-parsers-0.3rc2/src/sd_parsers/parsers/_novelai.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import re
 from contextlib import suppress
 from typing import Any, Dict
 
 from PIL.Image import Image
 from PIL.PngImagePlugin import PngImageFile
 
-from .._exceptions import ParserError
 from .._models import Model, Prompt, Sampler
 from .._parser import Generators, Parser, ParseResult, pop_keys
 from .._prompt_info import PromptInfo
+from ..exceptions import ParserError
 from ._managed_parsers import MANAGED_PARSERS
 
 SAMPLER_PARAMS = ["seed", "strength", "noise", "scale"]
 
 
 class NovelAIParser(Parser):
     """parser for images generated by NovelAI"""
```

### Comparing `sd-parsers-0.3rc1/src/sd_parsers.egg-info/PKG-INFO` & `sd-parsers-0.3rc2/src/sd_parsers.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd-parsers
-Version: 0.3rc1
+Version: 0.3rc2
 Summary: a library to read metadata from images created by Stable Diffusion
 Author: d3x-at
 License: MIT License
         
         Copyright (c) 2023 d3x-at
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,14 +26,20 @@
         SOFTWARE.
 Project-URL: repository, https://github.com/d3x-at/sd-parsers
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: Pillow>=8.3.1
 
+> [!IMPORTANT]  
+> A release candidate featuring a revisited API and extended ComfyUI & InvokeAI parsing logic is available.
+> 
+> See [release notes](https://github.com/d3x-at/sd-parsers/releases/tag/v0.3rc2) for changes.
+>
+> Install with: ```pip install --upgrade --pre sd-parsers```
 
 ## Features
 
 Supports reading metadata from images generated with:
 * Automatic1111's Stable Diffusion web UI
 * ComfyUI *
 * InvokeAI
@@ -75,15 +81,15 @@
     prompt_info = parser_manager.parse(image)
 ```
 
 Each parser module can also be used directly, omitting the use of ```ParserManager```:
 
 ```python
 from PIL import Image
-from sd_parsers import ParserError
+from sd_parsers.exceptions import ParserError
 from sd_parsers.parsers import AUTOMATIC1111Parser
 
 parser = AUTOMATIC1111Parser()
 with Image.open("image.png") as image:
     prompt_info, error = parser.read_parameters(image)
     
     if prompt_info:
```

### Comparing `sd-parsers-0.3rc1/src/sd_parsers.egg-info/SOURCES.txt` & `sd-parsers-0.3rc2/src/sd_parsers.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 .github/workflows/publish-to.pypi.yml
 .github/workflows/test.yml
 examples/README.md
 examples/cmdline.py
 examples/deep_dive.py
 examples/fast_api.py
 src/sd_parsers/__init__.py
-src/sd_parsers/_exceptions.py
 src/sd_parsers/_models.py
 src/sd_parsers/_parser.py
 src/sd_parsers/_parser_manager.py
 src/sd_parsers/_prompt_info.py
+src/sd_parsers/exceptions.py
 src/sd_parsers/py.typed
 src/sd_parsers.egg-info/PKG-INFO
 src/sd_parsers.egg-info/SOURCES.txt
 src/sd_parsers.egg-info/dependency_links.txt
 src/sd_parsers.egg-info/requires.txt
 src/sd_parsers.egg-info/top_level.txt
 src/sd_parsers/parsers/__init__.py
@@ -41,12 +41,18 @@
 tests/resources/parsers/ComfyUI/__init__.py
 tests/resources/parsers/ComfyUI/img2img_cropped.png
 tests/resources/parsers/ComfyUI/img2img_cropped.py
 tests/resources/parsers/ComfyUI/night_evening_day_morning_cropped.png
 tests/resources/parsers/ComfyUI/night_evening_day_morning_cropped.py
 tests/resources/parsers/ComfyUI/noisy_latents_3_subjects_cropped.png
 tests/resources/parsers/ComfyUI/unclip_2pass_cropped.png
-tests/resources/parsers/InvokeAI/invokeai1_cropped.png
+tests/resources/parsers/InvokeAI/__init__.py
+tests/resources/parsers/InvokeAI/invokeai_dream1.png
+tests/resources/parsers/InvokeAI/invokeai_dream1.py
+tests/resources/parsers/InvokeAI/invokeai_imeta1.png
+tests/resources/parsers/InvokeAI/invokeai_imeta1.py
+tests/resources/parsers/InvokeAI/invokeai_sdmeta1.png
+tests/resources/parsers/InvokeAI/invokeai_sdmeta1.py
 tests/resources/parsers/NovelAI/novelai1_cropped.png
 tests/tools/__init__.py
 tests/tools/crop_image.py
 tests/tools/crop_image.sh
```

### Comparing `sd-parsers-0.3rc1/tests/resources/bad_images/text_after_idat.png` & `sd-parsers-0.3rc2/tests/resources/bad_images/text_after_idat.png`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.3rc1/tests/resources/parsers/AUTOMATIC1111/automatic1111_cropped.jpg` & `sd-parsers-0.3rc2/tests/resources/parsers/AUTOMATIC1111/automatic1111_cropped.jpg`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.3rc1/tests/resources/parsers/ComfyUI/img2img_cropped.png` & `sd-parsers-0.3rc2/tests/resources/parsers/ComfyUI/img2img_cropped.png`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.3rc1/tests/resources/parsers/ComfyUI/img2img_cropped.py` & `sd-parsers-0.3rc2/tests/resources/parsers/ComfyUI/img2img_cropped.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import pytest
 from sd_parsers import Model, Prompt, Sampler
 
-MODEL = Model(name="v1-5-pruned-emaonly.ckpt", config="v1-inference.yaml", model_id=4)
+MODEL = Model(
+    name="v1-5-pruned-emaonly.ckpt", parameters={"config_name": "v1-inference.yaml"}, model_id=4
+)
+
 PROMPTS = [
     Prompt(
         value="photograph of victorian woman with wings, sky clouds, " "meadow grass",
         prompt_id=6,
     )
 ]
+
 NEGATIVE_PROMPTS = [Prompt(value="watermark, text", prompt_id=7)]
 
 PARAM = pytest.param(
     "img2img_cropped.png",
     (
         [
             Sampler(
```

### Comparing `sd-parsers-0.3rc1/tests/resources/parsers/ComfyUI/night_evening_day_morning_cropped.png` & `sd-parsers-0.3rc2/tests/resources/parsers/ComfyUI/night_evening_day_morning_cropped.png`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.3rc1/tests/resources/parsers/ComfyUI/night_evening_day_morning_cropped.py` & `sd-parsers-0.3rc2/tests/resources/parsers/ComfyUI/night_evening_day_morning_cropped.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,41 @@
 import pytest
 from sd_parsers import Model, Prompt, Sampler
 
-MODEL1 = Model(model_id=45, name="Anything-V3.0.ckpt", config=None, model_hash=None)
+MODEL1 = Model(model_id=45, name="Anything-V3.0.ckpt", model_hash=None)
 MODEL2 = Model(
     model_id=46,
     name="AbyssOrangeMix2_hard.safetensors",
-    config=None,
     model_hash=None,
 )
 
 PROMPTS1 = [
     Prompt(
         value="(best quality) (daytime:1.2) sky (blue)",
         prompt_id=17,
-        weight=None,
     ),
     Prompt(
         value="(best quality) (night:1.3) (darkness) sky (black) (stars:1.2) "
         "(galaxy:1.2) (space) (universe)",
         prompt_id=14,
-        weight=None,
     ),
     Prompt(
         value="(best quality) (evening:1.2) (sky:1.2) (clouds) (colorful) "
         "(HDR:1.2) (sunset:1.3)",
         prompt_id=13,
-        weight=None,
     ),
     Prompt(
         value="(masterpiece) (best quality) morning sky",
         prompt_id=33,
-        weight=None,
     ),
     Prompt(
         value="(masterpiece) (best quality) beautiful landscape breathtaking "
         "amazing view nature photograph forest mountains ocean (sky) "
         "national park scenery",
         prompt_id=6,
-        weight=None,
     ),
 ]
 
 NEGATIVE_PROMPTS1 = [
     Prompt(
         value="(hands), text, error, cropped, (worst "
         "quality:1.2), (low quality:1.2), "
@@ -49,27 +43,25 @@
         "signature, watermark, username, "
         "blurry, artist name, monochrome, "
         "sketch, censorship, censor, "
         "(copyright:1.2), extra legs, "
         "(forehead mark) (depth of field) "
         "(emotionless) (penis) (pumpkin)",
         prompt_id=7,
-        weight=None,
     )
 ]
 
 PROMPTS2 = [
     Prompt(
         value="(best quality) beautiful (HDR:1.2) "
         "(realistic:1.2) landscape breathtaking amazing "
         "view nature scenery photograph forest "
         "mountains ocean daytime night evening morning, "
         "(sky:1.2)",
         prompt_id=26,
-        weight=None,
     )
 ]
 
 NEGATIVE_PROMPTS2 = [
     Prompt(
         value="(hands), text, error, cropped, (worst "
         "quality:1.2), (low quality:1.2), "
@@ -77,15 +69,14 @@
         "signature, watermark, username, "
         "blurry, artist name, monochrome, "
         "sketch, censorship, censor, "
         "(copyright:1.2), extra legs, "
         "(forehead mark) (depth of field) "
         "(emotionless) (penis) (pumpkin)",
         prompt_id=27,
-        weight=None,
     )
 ]
 
 PARAM = pytest.param(
     "night_evening_day_morning_cropped.png",
     (
         [
```

### Comparing `sd-parsers-0.3rc1/tests/resources/parsers/ComfyUI/noisy_latents_3_subjects_cropped.png` & `sd-parsers-0.3rc2/tests/resources/parsers/ComfyUI/noisy_latents_3_subjects_cropped.png`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.3rc1/tests/resources/parsers/ComfyUI/unclip_2pass_cropped.png` & `sd-parsers-0.3rc2/tests/resources/parsers/ComfyUI/unclip_2pass_cropped.png`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.3rc1/tests/resources/parsers/InvokeAI/invokeai1_cropped.png` & `sd-parsers-0.3rc2/tests/resources/parsers/InvokeAI/invokeai_sdmeta1.png`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.3rc1/tests/resources/parsers/NovelAI/novelai1_cropped.png` & `sd-parsers-0.3rc2/tests/resources/parsers/NovelAI/novelai1_cropped.png`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.3rc1/tests/test_automatic1111.py` & `sd-parsers-0.3rc2/tests/test_automatic1111.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.3rc1/tests/test_comfyui.py` & `sd-parsers-0.3rc2/tests/test_comfyui.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.3rc1/tests/test_invokeai.py` & `sd-parsers-0.3rc2/tests/resources/parsers/InvokeAI/invokeai_sdmeta1.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,96 +1,70 @@
 import pytest
-from PIL import Image
 from sd_parsers import Model, Prompt, Sampler
-from sd_parsers.parsers import InvokeAIParser
 
-from tests.tools import RESOURCE_PATH
+MODELS = [
+    Model(
+        name="deliberateForInvoke_v08",
+        model_hash="56d1442a0feefd64836a19ac8e3527ec71c884fc962e246ddf67b03e42921272",
+    )
+]
 
-MODEL = Model(
-    name="deliberateForInvoke_v08",
-    model_hash="56d1442a0feefd64836a19ac8e3527ec71c884fc962e246ddf67b03e42921272",
-)
 PROMPTS = [
     Prompt(
         value=(
             "professional full body photo of young woman, "
             "hyper long brunette hair, elegant hair, "
             "wearing a bikini top and asymmetric short skirt, "
             "curvy body, long legs, (imperfect skin), detailed skin, "
             "intense freckles, super long eye lashes, at night, outside, "
             "city background, 8k ultra detailed, realistic, high quality, "
             "film grain, low contrast"
         ),
-        weight=1.0,
+        parameters={"weight": 1.0},
     )
 ]
 
 NEGATIVE_PROMPTS = [
     Prompt(
         value="rendering, glowing eyes, skinny",
-        weight=1.0,
+        parameters={"weight": 1.0},
     )
 ]
 
-testdata = [
-    pytest.param(
-        "invokeai1_cropped.png",
-        (
-            Sampler(
-                name="k_lms",
-                parameters={
-                    "steps": 50,
-                    "cfg_scale": 5,
-                    "threshold": 0,
-                    "perlin": 0,
-                    "seed": 2980747362,
-                },
-                model=MODEL,
-                prompts=PROMPTS,
-                negative_prompts=NEGATIVE_PROMPTS,
-            ),
-            set([MODEL]),
-            set(PROMPTS),
-            set(NEGATIVE_PROMPTS),
-            {
-                "model": "stable diffusion",
-                "app_id": "invoke-ai/InvokeAI",
-                "app_version": "2.3.0",
-                "height": 768,
-                "width": 512,
-                "size": "512x768",
-                "seamless": False,
-                "hires_fix": False,
-                "type": "txt2img",
-                "postprocessing": [
-                    {"type": "codeformer", "strength": 0.9, "fidelity": 0.75},
-                    {"type": "esrgan", "scale": 4, "strength": 0.95},
-                ],
-                "variations": [],
+PARAM = pytest.param(
+    "invokeai_sdmeta1.png",
+    (
+        Sampler(
+            name="k_lms",
+            parameters={
+                "steps": 50,
+                "cfg_scale": 5,
+                "threshold": 0,
+                "perlin": 0,
+                "seed": 2980747362,
             },
+            model=MODELS[0],
+            prompts=PROMPTS,
+            negative_prompts=NEGATIVE_PROMPTS,
         ),
-        id="invokeai1_cropped.png",
+        set(MODELS),
+        set(PROMPTS),
+        set(NEGATIVE_PROMPTS),
+        {
+            "model": "stable diffusion",
+            "app_id": "invoke-ai/InvokeAI",
+            "app_version": "2.3.0",
+            "height": 768,
+            "width": 512,
+            "size": "512x768",
+            "seamless": False,
+            "hires_fix": False,
+            "type": "txt2img",
+            "postprocessing": [
+                {"type": "codeformer", "strength": 0.9, "fidelity": 0.75},
+                {"type": "esrgan", "scale": 4, "strength": 0.95},
+            ],
+            "variations": [],
+        },
     ),
-]
-
-
-@pytest.mark.parametrize("filename, expected", testdata)
-def test_parse(filename: str, expected):
-    (
-        expected_sampler,
-        expected_models,
-        expected_prompts,
-        expected_negative_prompts,
-        expected_metadata,
-    ) = expected
-
-    parser = InvokeAIParser()
-    with Image.open(RESOURCE_PATH / "parsers/InvokeAI" / filename) as image:
-        image_data, error = parser.read_parameters(image)
-
-    assert image_data is not None
-    assert error is None
-    assert image_data.samplers == [expected_sampler]
-    assert image_data.prompts == expected_prompts
-    assert image_data.negative_prompts == expected_negative_prompts
-    assert image_data.models == expected_models
-    assert image_data.metadata == expected_metadata
+    id="invokeai_sdmeta1.png",
+)
```

### Comparing `sd-parsers-0.3rc1/tests/test_novelai.py` & `sd-parsers-0.3rc2/tests/test_novelai.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,31 +2,25 @@
 from PIL import Image
 from sd_parsers import Model, Prompt, Sampler
 from sd_parsers.parsers import NovelAIParser
 
 from tests.tools import RESOURCE_PATH
 
 MODEL = Model(name="Stable Diffusion", model_hash="1D44365E")
-PROMPTS = [
-    Prompt(
-        value="masterpiece, best quality,  cat, space, icon",
-        weight=None,
-    )
-]
+PROMPTS = [Prompt(value="masterpiece, best quality,  cat, space, icon")]
 NEGATIVE_PROMPTS = [
     Prompt(
         value=(
             "lowres, bad anatomy, bad hands, text, error, missing fingers, "
             "extra digit, fewer digits, cropped, worst quality, low quality, "
             "normal quality, jpeg artifacts, signature, watermark, username, "
             "blurry, lowres, bad anatomy, bad hands, text, error, missing fingers, "
             "extra digit, fewer digits, cropped, worst quality, low quality, "
             "normal quality, jpeg artifacts, signature, watermark, username, blurry"
-        ),
-        weight=None,
+        )
     )
 ]
 
 testdata = [
     pytest.param(
         "novelai1_cropped.png",
         (
```

### Comparing `sd-parsers-0.3rc1/tests/test_parser_manager.py` & `sd-parsers-0.3rc2/tests/test_parser_manager.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.3rc1/tests/tools/crop_image.py` & `sd-parsers-0.3rc2/tests/tools/crop_image.py`

 * *Files identical despite different names*

