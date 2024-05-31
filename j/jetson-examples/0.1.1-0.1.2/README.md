# Comparing `tmp/jetson_examples-0.1.1.tar.gz` & `tmp/jetson_examples-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jetson_examples-0.1.1.tar", last modified: Wed May 29 08:43:40 2024, max compression
+gzip compressed data, was "jetson_examples-0.1.2.tar", last modified: Fri May 31 06:54:32 2024, max compression
```

## Comparing `jetson_examples-0.1.1.tar` & `jetson_examples-0.1.2.tar`

### file list

```diff
@@ -1,73 +1,81 @@
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-29 08:43:40.231138 jetson_examples-0.1.1/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1066 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/LICENSE
--rw-r--r--   0 youjiang  (1000) youjiang  (1000)     4846 2024-05-29 08:43:40.231138 jetson_examples-0.1.1/PKG-INFO
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     4196 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/README.md
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-29 08:43:40.231138 jetson_examples-0.1.1/jetson_examples.egg-info/
--rw-r--r--   0 youjiang  (1000) youjiang  (1000)     4846 2024-05-29 08:43:40.000000 jetson_examples-0.1.1/jetson_examples.egg-info/PKG-INFO
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1890 2024-05-29 08:43:40.000000 jetson_examples-0.1.1/jetson_examples.egg-info/SOURCES.txt
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)        1 2024-05-29 08:43:40.000000 jetson_examples-0.1.1/jetson_examples.egg-info/dependency_links.txt
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       58 2024-05-29 08:43:40.000000 jetson_examples-0.1.1/jetson_examples.egg-info/entry_points.txt
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       27 2024-05-29 08:43:40.000000 jetson_examples-0.1.1/jetson_examples.egg-info/top_level.txt
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1081 2024-05-29 08:42:27.000000 jetson_examples-0.1.1/pyproject.toml
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-29 08:43:40.227138 jetson_examples-0.1.1/reComputer/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       22 2024-05-29 08:42:39.000000 jetson_examples-0.1.1/reComputer/__init__.py
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     2088 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/main.py
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-29 08:43:40.227138 jetson_examples-0.1.1/reComputer/scripts/
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-29 08:43:40.231138 jetson_examples-0.1.1/reComputer/scripts/Sheared-LLaMA-2.7B-ShareGPT/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/Sheared-LLaMA-2.7B-ShareGPT/init.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      237 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/Sheared-LLaMA-2.7B-ShareGPT/run.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-29 08:43:40.231138 jetson_examples-0.1.1/reComputer/scripts/audiocraft/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      951 2024-05-29 08:42:13.000000 jetson_examples-0.1.1/reComputer/scripts/audiocraft/README.md
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       77 2024-05-29 07:36:41.000000 jetson_examples-0.1.1/reComputer/scripts/audiocraft/clean.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:41.000000 jetson_examples-0.1.1/reComputer/scripts/audiocraft/init.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      160 2024-05-29 07:36:41.000000 jetson_examples-0.1.1/reComputer/scripts/audiocraft/run.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      127 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/check.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      898 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/clean.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-29 08:43:40.231138 jetson_examples-0.1.1/reComputer/scripts/live-llava/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/live-llava/init.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)    10137 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/live-llava/run.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-29 08:43:40.231138 jetson_examples-0.1.1/reComputer/scripts/llama3/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/llama3/init.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      328 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/llama3/run.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-29 08:43:40.231138 jetson_examples-0.1.1/reComputer/scripts/llava/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       70 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/llava/clean.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/llava/init.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      251 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/llava/run.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-29 08:43:40.231138 jetson_examples-0.1.1/reComputer/scripts/llava-v1.5-7b/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/llava-v1.5-7b/init.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      251 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/llava-v1.5-7b/run.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-29 08:43:40.231138 jetson_examples-0.1.1/reComputer/scripts/llava-v1.6-vicuna-7b/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/llava-v1.6-vicuna-7b/init.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      269 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/llava-v1.6-vicuna-7b/run.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-29 08:43:40.231138 jetson_examples-0.1.1/reComputer/scripts/nanodb/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/nanodb/init.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      247 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/nanodb/readme.md
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     2571 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/nanodb/run.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-29 08:43:40.231138 jetson_examples-0.1.1/reComputer/scripts/nanoowl/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/nanoowl/init.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      264 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/nanoowl/run.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-29 08:43:40.231138 jetson_examples-0.1.1/reComputer/scripts/ollama/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/ollama/init.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      246 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/ollama/run.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1032 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/run.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-29 08:43:40.231138 jetson_examples-0.1.1/reComputer/scripts/stable-diffusion-webui/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/stable-diffusion-webui/init.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      160 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/stable-diffusion-webui/run.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-29 08:43:40.231138 jetson_examples-0.1.1/reComputer/scripts/text-generation-webui/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/text-generation-webui/init.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      407 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/text-generation-webui/run.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      900 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/update.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-29 08:43:40.231138 jetson_examples-0.1.1/reComputer/scripts/whisper/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/whisper/init.sh
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      146 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/whisper/run.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-29 08:43:40.231138 jetson_examples-0.1.1/reComputer/scripts/yolov8-rail-inspection/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     2008 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/yolov8-rail-inspection/readme.md
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      809 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/yolov8-rail-inspection/run.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-29 08:43:40.231138 jetson_examples-0.1.1/reComputer/scripts/yolov8:detect/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      167 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/yolov8:detect/Dockerfile
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1122 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/yolov8:detect/README.txt
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1307 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/yolov8:detect/app.py
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      130 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/yolov8:detect/run.sh
-drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-29 08:43:40.231138 jetson_examples-0.1.1/reComputer/scripts/yolov8:detect/templates/
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      524 2024-05-29 07:36:02.000000 jetson_examples-0.1.1/reComputer/scripts/yolov8:detect/templates/index.html
--rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       38 2024-05-29 08:43:40.231138 jetson_examples-0.1.1/setup.cfg
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.629692 jetson_examples-0.1.2/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1066 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/LICENSE
+-rw-r--r--   0 youjiang  (1000) youjiang  (1000)     5007 2024-05-31 06:54:32.629692 jetson_examples-0.1.2/PKG-INFO
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     4357 2024-05-31 06:53:02.000000 jetson_examples-0.1.2/README.md
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.629692 jetson_examples-0.1.2/jetson_examples.egg-info/
+-rw-r--r--   0 youjiang  (1000) youjiang  (1000)     5007 2024-05-31 06:54:32.000000 jetson_examples-0.1.2/jetson_examples.egg-info/PKG-INFO
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     2114 2024-05-31 06:54:32.000000 jetson_examples-0.1.2/jetson_examples.egg-info/SOURCES.txt
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)        1 2024-05-31 06:54:32.000000 jetson_examples-0.1.2/jetson_examples.egg-info/dependency_links.txt
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       58 2024-05-31 06:54:32.000000 jetson_examples-0.1.2/jetson_examples.egg-info/entry_points.txt
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       27 2024-05-31 06:54:32.000000 jetson_examples-0.1.2/jetson_examples.egg-info/top_level.txt
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1081 2024-05-30 07:28:59.000000 jetson_examples-0.1.2/pyproject.toml
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       22 2024-05-30 07:29:30.000000 jetson_examples-0.1.2/reComputer/__init__.py
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     2088 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/main.py
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/Sheared-LLaMA-2.7B-ShareGPT/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/Sheared-LLaMA-2.7B-ShareGPT/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      237 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/Sheared-LLaMA-2.7B-ShareGPT/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/audiocraft/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      951 2024-05-29 08:42:13.000000 jetson_examples-0.1.2/reComputer/scripts/audiocraft/README.md
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       77 2024-05-29 07:36:41.000000 jetson_examples-0.1.2/reComputer/scripts/audiocraft/clean.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:41.000000 jetson_examples-0.1.2/reComputer/scripts/audiocraft/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      160 2024-05-29 07:36:41.000000 jetson_examples-0.1.2/reComputer/scripts/audiocraft/run.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      127 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/check.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      898 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/clean.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/live-llava/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/live-llava/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)    10137 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/live-llava/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/llama3/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/llama3/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      328 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/llama3/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/llava/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       70 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/llava/clean.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/llava/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      251 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/llava/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/llava-v1.5-7b/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/llava-v1.5-7b/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      251 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/llava-v1.5-7b/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/llava-v1.6-vicuna-7b/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/llava-v1.6-vicuna-7b/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      269 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/llava-v1.6-vicuna-7b/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/nanodb/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/nanodb/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      247 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/nanodb/readme.md
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     2571 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/nanodb/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/nanoowl/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/nanoowl/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      264 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/nanoowl/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/ollama/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/ollama/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      246 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/ollama/run.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1032 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/stable-diffusion-webui/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/stable-diffusion-webui/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      160 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/stable-diffusion-webui/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/text-generation-webui/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/text-generation-webui/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      407 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/text-generation-webui/run.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      900 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/update.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/whisper/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      428 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/whisper/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      146 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/whisper/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/yolov10/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      466 2024-05-31 06:47:18.000000 jetson_examples-0.1.2/reComputer/scripts/yolov10/Dockerfile
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     3123 2024-05-31 06:47:18.000000 jetson_examples-0.1.2/reComputer/scripts/yolov10/README.md
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.625692 jetson_examples-0.1.2/reComputer/scripts/yolov10/assets/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)  2600779 2024-05-31 06:47:18.000000 jetson_examples-0.1.2/reComputer/scripts/yolov10/assets/webui.png
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      106 2024-05-31 06:49:00.000000 jetson_examples-0.1.2/reComputer/scripts/yolov10/clean.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1679 2024-05-31 06:47:18.000000 jetson_examples-0.1.2/reComputer/scripts/yolov10/init.sh
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      289 2024-05-31 06:47:18.000000 jetson_examples-0.1.2/reComputer/scripts/yolov10/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.629692 jetson_examples-0.1.2/reComputer/scripts/yolov8-rail-inspection/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     2008 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/yolov8-rail-inspection/readme.md
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      809 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/yolov8-rail-inspection/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.629692 jetson_examples-0.1.2/reComputer/scripts/yolov8:detect/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      167 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/yolov8:detect/Dockerfile
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1122 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/yolov8:detect/README.txt
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)     1307 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/yolov8:detect/app.py
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      130 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/yolov8:detect/run.sh
+drwxrwxr-x   0 youjiang  (1000) youjiang  (1000)        0 2024-05-31 06:54:32.629692 jetson_examples-0.1.2/reComputer/scripts/yolov8:detect/templates/
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)      524 2024-05-29 07:36:02.000000 jetson_examples-0.1.2/reComputer/scripts/yolov8:detect/templates/index.html
+-rw-rw-r--   0 youjiang  (1000) youjiang  (1000)       38 2024-05-31 06:54:32.629692 jetson_examples-0.1.2/setup.cfg
```

### Comparing `jetson_examples-0.1.1/LICENSE` & `jetson_examples-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.1.1/PKG-INFO` & `jetson_examples-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jetson-examples
-Version: 0.1.1
+Version: 0.1.2
 Summary: Running Gen AI models and applications on NVIDIA Jetson devices with one-line command
 Author-email: luozhixin <zhixin.luo@seeed.cc>
 Project-URL: Homepage, https://github.com/Seeed-Projects/jetson-examples
 Project-URL: Issues, https://github.com/Seeed-Projects/jetson-examples/issues
 Keywords: llama,llava,gpt,llm,nvidia,jetson,multimodal,jetson orin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -56,23 +56,24 @@
 
 ## Example list
 
 Here are some examples that can be run:
 
 | Example                                          | Type                     | Model/Data Size | Docker Image Size | Command                                 |
 | ------------------------------------------------ | ------------------------ | --------------- | ---------- | --------------------------------------- |
+| 🆕 [yolov10](/reComputer/scripts/yolov10/README.md)     | Computer Vision         | 7.2M               | 5.74 GB     | `reComputer run yolov10`                 |
 | 🆕 llama3                                         | Text (LLM)               | 4.9GB           | 10.5GB     | `reComputer run llama3`                 |
 | 🆕 [ollama](https://github.com/ollama/ollama)     | Inference Server         | *               | 10.5GB     | `reComputer run ollama`                 |
 | LLaVA                                            | Text + Vision (VLM)      | 13GB            | 14.4GB     | `reComputer run llava`                  |
 | Live LLaVA                                       | Text + Vision (VLM)      | 13GB            | 20.3GB     | `reComputer run live-llava`             |
 | stable-diffusion-webui                           | Image Generation         | 3.97G           | 7.3GB      | `reComputer run stable-diffusion-webui` |
 | nanoowl                                          | Vision Transformers(ViT) | 613MB           | 15.1GB     | `reComputer run nanoowl`                |
 | [nanodb](../reComputer/scripts/nanodb/readme.md) | Vector Database          | 76GB            | 7.0GB      | `reComputer run nanodb`                 |
 | whisper                                          | Audio                    | 1.5GB           | 6.0GB      | `reComputer run whisper`                |
-| [🆕 yolov8-rail-inspection](/reComputer/scripts/yolov8-rail-inspection/readme.md) |Computer Vision | 6M | 13.8GB  | `reComputer run yolov8-rail-inspection`  |
+| [yolov8-rail-inspection](/reComputer/scripts/yolov8-rail-inspection/readme.md) |Computer Vision | 6M | 13.8GB  | `reComputer run yolov8-rail-inspection`  |
 
 > Note: You should have enough space to run example, like `LLaVA`, at least `27.4GB` totally
 
 More Examples can be found [examples.md](./docs/examples.md)
 
 ## Development
 Want to add your own example? Check out the [development guide](./docs/develop.md).
```

### Comparing `jetson_examples-0.1.1/README.md` & `jetson_examples-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -41,23 +41,24 @@
 
 ## Example list
 
 Here are some examples that can be run:
 
 | Example                                          | Type                     | Model/Data Size | Docker Image Size | Command                                 |
 | ------------------------------------------------ | ------------------------ | --------------- | ---------- | --------------------------------------- |
+| 🆕 [yolov10](/reComputer/scripts/yolov10/README.md)     | Computer Vision         | 7.2M               | 5.74 GB     | `reComputer run yolov10`                 |
 | 🆕 llama3                                         | Text (LLM)               | 4.9GB           | 10.5GB     | `reComputer run llama3`                 |
 | 🆕 [ollama](https://github.com/ollama/ollama)     | Inference Server         | *               | 10.5GB     | `reComputer run ollama`                 |
 | LLaVA                                            | Text + Vision (VLM)      | 13GB            | 14.4GB     | `reComputer run llava`                  |
 | Live LLaVA                                       | Text + Vision (VLM)      | 13GB            | 20.3GB     | `reComputer run live-llava`             |
 | stable-diffusion-webui                           | Image Generation         | 3.97G           | 7.3GB      | `reComputer run stable-diffusion-webui` |
 | nanoowl                                          | Vision Transformers(ViT) | 613MB           | 15.1GB     | `reComputer run nanoowl`                |
 | [nanodb](../reComputer/scripts/nanodb/readme.md) | Vector Database          | 76GB            | 7.0GB      | `reComputer run nanodb`                 |
 | whisper                                          | Audio                    | 1.5GB           | 6.0GB      | `reComputer run whisper`                |
-| [🆕 yolov8-rail-inspection](/reComputer/scripts/yolov8-rail-inspection/readme.md) |Computer Vision | 6M | 13.8GB  | `reComputer run yolov8-rail-inspection`  |
+| [yolov8-rail-inspection](/reComputer/scripts/yolov8-rail-inspection/readme.md) |Computer Vision | 6M | 13.8GB  | `reComputer run yolov8-rail-inspection`  |
 
 > Note: You should have enough space to run example, like `LLaVA`, at least `27.4GB` totally
 
 More Examples can be found [examples.md](./docs/examples.md)
 
 ## Development
 Want to add your own example? Check out the [development guide](./docs/develop.md).
```

### Comparing `jetson_examples-0.1.1/jetson_examples.egg-info/PKG-INFO` & `jetson_examples-0.1.2/jetson_examples.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jetson-examples
-Version: 0.1.1
+Version: 0.1.2
 Summary: Running Gen AI models and applications on NVIDIA Jetson devices with one-line command
 Author-email: luozhixin <zhixin.luo@seeed.cc>
 Project-URL: Homepage, https://github.com/Seeed-Projects/jetson-examples
 Project-URL: Issues, https://github.com/Seeed-Projects/jetson-examples/issues
 Keywords: llama,llava,gpt,llm,nvidia,jetson,multimodal,jetson orin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -56,23 +56,24 @@
 
 ## Example list
 
 Here are some examples that can be run:
 
 | Example                                          | Type                     | Model/Data Size | Docker Image Size | Command                                 |
 | ------------------------------------------------ | ------------------------ | --------------- | ---------- | --------------------------------------- |
+| 🆕 [yolov10](/reComputer/scripts/yolov10/README.md)     | Computer Vision         | 7.2M               | 5.74 GB     | `reComputer run yolov10`                 |
 | 🆕 llama3                                         | Text (LLM)               | 4.9GB           | 10.5GB     | `reComputer run llama3`                 |
 | 🆕 [ollama](https://github.com/ollama/ollama)     | Inference Server         | *               | 10.5GB     | `reComputer run ollama`                 |
 | LLaVA                                            | Text + Vision (VLM)      | 13GB            | 14.4GB     | `reComputer run llava`                  |
 | Live LLaVA                                       | Text + Vision (VLM)      | 13GB            | 20.3GB     | `reComputer run live-llava`             |
 | stable-diffusion-webui                           | Image Generation         | 3.97G           | 7.3GB      | `reComputer run stable-diffusion-webui` |
 | nanoowl                                          | Vision Transformers(ViT) | 613MB           | 15.1GB     | `reComputer run nanoowl`                |
 | [nanodb](../reComputer/scripts/nanodb/readme.md) | Vector Database          | 76GB            | 7.0GB      | `reComputer run nanodb`                 |
 | whisper                                          | Audio                    | 1.5GB           | 6.0GB      | `reComputer run whisper`                |
-| [🆕 yolov8-rail-inspection](/reComputer/scripts/yolov8-rail-inspection/readme.md) |Computer Vision | 6M | 13.8GB  | `reComputer run yolov8-rail-inspection`  |
+| [yolov8-rail-inspection](/reComputer/scripts/yolov8-rail-inspection/readme.md) |Computer Vision | 6M | 13.8GB  | `reComputer run yolov8-rail-inspection`  |
 
 > Note: You should have enough space to run example, like `LLaVA`, at least `27.4GB` totally
 
 More Examples can be found [examples.md](./docs/examples.md)
 
 ## Development
 Want to add your own example? Check out the [development guide](./docs/develop.md).
```

### Comparing `jetson_examples-0.1.1/jetson_examples.egg-info/SOURCES.txt` & `jetson_examples-0.1.2/jetson_examples.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,20 @@
 reComputer/scripts/ollama/run.sh
 reComputer/scripts/stable-diffusion-webui/init.sh
 reComputer/scripts/stable-diffusion-webui/run.sh
 reComputer/scripts/text-generation-webui/init.sh
 reComputer/scripts/text-generation-webui/run.sh
 reComputer/scripts/whisper/init.sh
 reComputer/scripts/whisper/run.sh
+reComputer/scripts/yolov10/Dockerfile
+reComputer/scripts/yolov10/README.md
+reComputer/scripts/yolov10/clean.sh
+reComputer/scripts/yolov10/init.sh
+reComputer/scripts/yolov10/run.sh
+reComputer/scripts/yolov10/assets/webui.png
 reComputer/scripts/yolov8-rail-inspection/readme.md
 reComputer/scripts/yolov8-rail-inspection/run.sh
 reComputer/scripts/yolov8:detect/Dockerfile
 reComputer/scripts/yolov8:detect/README.txt
 reComputer/scripts/yolov8:detect/app.py
 reComputer/scripts/yolov8:detect/run.sh
 reComputer/scripts/yolov8:detect/templates/index.html
```

### Comparing `jetson_examples-0.1.1/pyproject.toml` & `jetson_examples-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=57.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jetson-examples"
-version = "0.1.1"
+version = "0.1.2"
 authors = [{ name = "luozhixin", email = "zhixin.luo@seeed.cc" }]
 description = "Running Gen AI models and applications on NVIDIA Jetson devices with one-line command"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `jetson_examples-0.1.1/reComputer/main.py` & `jetson_examples-0.1.2/reComputer/main.py`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.1.1/reComputer/scripts/audiocraft/README.md` & `jetson_examples-0.1.2/reComputer/scripts/audiocraft/README.md`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.1.1/reComputer/scripts/clean.sh` & `jetson_examples-0.1.2/reComputer/scripts/clean.sh`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.1.1/reComputer/scripts/live-llava/run.sh` & `jetson_examples-0.1.2/reComputer/scripts/live-llava/run.sh`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.1.1/reComputer/scripts/nanodb/run.sh` & `jetson_examples-0.1.2/reComputer/scripts/nanodb/run.sh`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.1.1/reComputer/scripts/run.sh` & `jetson_examples-0.1.2/reComputer/scripts/run.sh`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.1.1/reComputer/scripts/update.sh` & `jetson_examples-0.1.2/reComputer/scripts/update.sh`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.1.1/reComputer/scripts/yolov8-rail-inspection/readme.md` & `jetson_examples-0.1.2/reComputer/scripts/yolov8-rail-inspection/readme.md`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.1.1/reComputer/scripts/yolov8-rail-inspection/run.sh` & `jetson_examples-0.1.2/reComputer/scripts/yolov8-rail-inspection/run.sh`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.1.1/reComputer/scripts/yolov8:detect/README.txt` & `jetson_examples-0.1.2/reComputer/scripts/yolov8:detect/README.txt`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.1.1/reComputer/scripts/yolov8:detect/app.py` & `jetson_examples-0.1.2/reComputer/scripts/yolov8:detect/app.py`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.1.1/reComputer/scripts/yolov8:detect/templates/index.html` & `jetson_examples-0.1.2/reComputer/scripts/yolov8:detect/templates/index.html`

 * *Files identical despite different names*

