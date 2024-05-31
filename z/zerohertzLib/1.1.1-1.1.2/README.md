# Comparing `tmp/zerohertzLib-1.1.1.tar.gz` & `tmp/zerohertzlib-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerohertzLib-1.1.1.tar", last modified: Tue May 28 16:45:02 2024, max compression
+gzip compressed data, was "zerohertzlib-1.1.2.tar", last modified: Fri May 31 17:14:17 2024, max compression
```

## Comparing `zerohertzLib-1.1.1.tar` & `zerohertzlib-1.1.2.tar`

### file list

```diff
@@ -1,84 +1,92 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:45:02.296166 zerohertzLib-1.1.1/
--rw-r--r--   0 root         (0) root         (0)     1067 2024-05-28 16:44:56.000000 zerohertzLib-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-28 16:44:56.000000 zerohertzLib-1.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3318 2024-05-28 16:45:02.296166 zerohertzLib-1.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2316 2024-05-28 16:44:56.000000 zerohertzLib-1.1.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 16:45:02.296166 zerohertzLib-1.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2704 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:45:02.288166 zerohertzLib-1.1.1/test/
--rw-r--r--   0 root         (0) root         (0)     4501 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/test/test_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     1822 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/test/test_api.py
--rw-r--r--   0 root         (0) root         (0)     1230 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/test/test_logging.py
--rw-r--r--   0 root         (0) root         (0)      220 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/test/test_monitoring.py
--rw-r--r--   0 root         (0) root         (0)     8641 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/test/test_plot.py
--rw-r--r--   0 root         (0) root         (0)     2150 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/test/test_quant.py
--rw-r--r--   0 root         (0) root         (0)     1961 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/test/test_util.py
--rw-r--r--   0 root         (0) root         (0)    14679 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/test/test_vision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:45:02.288166 zerohertzLib-1.1.1/zerohertzLib/
--rw-r--r--   0 root         (0) root         (0)     1794 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:45:02.288166 zerohertzLib-1.1.1/zerohertzLib/algorithm/
--rw-r--r--   0 root         (0) root         (0)     1040 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/algorithm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2626 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/algorithm/bisect.py
--rw-r--r--   0 root         (0) root         (0)     6708 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/algorithm/collections.py
--rw-r--r--   0 root         (0) root         (0)     2420 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/algorithm/fft.py
--rw-r--r--   0 root         (0) root         (0)     7065 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/algorithm/graph.py
--rw-r--r--   0 root         (0) root         (0)     1676 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/algorithm/prime.py
--rw-r--r--   0 root         (0) root         (0)     8048 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/algorithm/sort.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:45:02.288166 zerohertzLib-1.1.1/zerohertzLib/api/
--rw-r--r--   0 root         (0) root         (0)      446 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3865 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/api/discord.py
--rw-r--r--   0 root         (0) root         (0)    10958 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/api/github.py
--rw-r--r--   0 root         (0) root         (0)    30846 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/api/koreainvestment.py
--rw-r--r--   0 root         (0) root         (0)     5011 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/api/open_ai.py
--rw-r--r--   0 root         (0) root         (0)     7698 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/api/slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:45:02.288166 zerohertzLib-1.1.1/zerohertzLib/logging/
--rw-r--r--   0 root         (0) root         (0)      359 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/logging/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4738 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/logging/handler.py
--rw-r--r--   0 root         (0) root         (0)     5264 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/logging/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:45:02.288166 zerohertzLib-1.1.1/zerohertzLib/mlops/
--rw-r--r--   0 root         (0) root         (0)      273 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/mlops/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18002 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/mlops/triton.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:45:02.288166 zerohertzLib-1.1.1/zerohertzLib/monitoring/
--rw-r--r--   0 root         (0) root         (0)      333 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2829 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/monitoring/cpu.py
--rw-r--r--   0 root         (0) root         (0)     5184 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/monitoring/gpu.py
--rw-r--r--   0 root         (0) root         (0)     2678 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/monitoring/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:45:02.288166 zerohertzLib-1.1.1/zerohertzLib/plot/
--rw-r--r--   0 root         (0) root         (0)     1552 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/plot/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15381 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/plot/bar_chart.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:45:02.292166 zerohertzLib-1.1.1/zerohertzLib/plot/fonts/
--rw-r--r--   0 root         (0) root         (0)  7549348 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf
--rw-r--r--   0 root         (0) root         (0)   347988 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/plot/fonts/times.ttf
--rw-r--r--   0 root         (0) root         (0)     3435 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/plot/pie.py
--rw-r--r--   0 root         (0) root         (0)    11476 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/plot/plot.py
--rw-r--r--   0 root         (0) root         (0)     4046 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/plot/scatter.py
--rw-r--r--   0 root         (0) root         (0)     3292 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/plot/table.py
--rw-r--r--   0 root         (0) root         (0)     4838 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/plot/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:45:02.296166 zerohertzLib-1.1.1/zerohertzLib/quant/
--rw-r--r--   0 root         (0) root         (0)      885 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/quant/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14935 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/quant/backtest.py
--rw-r--r--   0 root         (0) root         (0)    13182 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/quant/methods.py
--rw-r--r--   0 root         (0) root         (0)    44465 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/quant/quant.py
--rw-r--r--   0 root         (0) root         (0)     3755 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/quant/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:45:02.296166 zerohertzLib-1.1.1/zerohertzLib/util/
--rw-r--r--   0 root         (0) root         (0)      458 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4527 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/util/csv.py
--rw-r--r--   0 root         (0) root         (0)    11173 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/util/data.py
--rw-r--r--   0 root         (0) root         (0)    11652 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/util/json.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:45:02.296166 zerohertzLib-1.1.1/zerohertzLib/vision/
--rw-r--r--   0 root         (0) root         (0)     1623 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/vision/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6967 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/vision/compare.py
--rw-r--r--   0 root         (0) root         (0)    12885 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/vision/convert.py
--rw-r--r--   0 root         (0) root         (0)    22463 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/vision/data.py
--rw-r--r--   0 root         (0) root         (0)    14878 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/vision/eval.py
--rw-r--r--   0 root         (0) root         (0)     4188 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/vision/gif.py
--rw-r--r--   0 root         (0) root         (0)    22281 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/vision/loader.py
--rw-r--r--   0 root         (0) root         (0)     7826 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/vision/transform.py
--rw-r--r--   0 root         (0) root         (0)     4219 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/vision/util.py
--rw-r--r--   0 root         (0) root         (0)    17516 2024-05-28 16:44:57.000000 zerohertzLib-1.1.1/zerohertzLib/vision/visual.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:45:02.288166 zerohertzLib-1.1.1/zerohertzLib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3318 2024-05-28 16:45:02.000000 zerohertzLib-1.1.1/zerohertzLib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1923 2024-05-28 16:45:02.000000 zerohertzLib-1.1.1/zerohertzLib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 16:45:02.000000 zerohertzLib-1.1.1/zerohertzLib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      457 2024-05-28 16:45:02.000000 zerohertzLib-1.1.1/zerohertzLib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-28 16:45:02.000000 zerohertzLib-1.1.1/zerohertzLib.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 17:14:17.790649 zerohertzlib-1.1.2/
+-rw-r--r--   0 root         (0) root         (0)     1067 2024-05-31 17:14:10.000000 zerohertzlib-1.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-31 17:14:10.000000 zerohertzlib-1.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6433 2024-05-31 17:14:17.790649 zerohertzlib-1.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2316 2024-05-31 17:14:10.000000 zerohertzlib-1.1.2/README.md
+-rw-r--r--   0 root         (0) root         (0)     2892 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 17:14:17.790649 zerohertzlib-1.1.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 17:14:17.778648 zerohertzlib-1.1.2/sphinx/
+-rw-r--r--   0 root         (0) root         (0)    12665 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/sphinx/example_images.py
+-rw-r--r--   0 root         (0) root         (0)      407 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/sphinx/release_note.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 17:14:17.778648 zerohertzlib-1.1.2/sphinx/source/
+-rw-r--r--   0 root         (0) root         (0)     5832 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/sphinx/source/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 17:14:17.778648 zerohertzlib-1.1.2/test/
+-rw-r--r--   0 root         (0) root         (0)     4501 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/test/test_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/test/test_api.py
+-rw-r--r--   0 root         (0) root         (0)     1230 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/test/test_logging.py
+-rw-r--r--   0 root         (0) root         (0)      220 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/test/test_monitoring.py
+-rw-r--r--   0 root         (0) root         (0)     8641 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/test/test_plot.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/test/test_quant.py
+-rw-r--r--   0 root         (0) root         (0)     1961 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/test/test_util.py
+-rw-r--r--   0 root         (0) root         (0)    14679 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/test/test_vision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 17:14:17.778648 zerohertzlib-1.1.2/zerohertzLib/
+-rw-r--r--   0 root         (0) root         (0)     1794 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 17:14:17.778648 zerohertzlib-1.1.2/zerohertzLib/algorithm/
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/algorithm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2626 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/algorithm/bisect.py
+-rw-r--r--   0 root         (0) root         (0)     6708 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/algorithm/collections.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/algorithm/fft.py
+-rw-r--r--   0 root         (0) root         (0)     7065 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/algorithm/graph.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/algorithm/prime.py
+-rw-r--r--   0 root         (0) root         (0)     8048 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/algorithm/sort.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 17:14:17.778648 zerohertzlib-1.1.2/zerohertzLib/api/
+-rw-r--r--   0 root         (0) root         (0)      446 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3865 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/api/discord.py
+-rw-r--r--   0 root         (0) root         (0)    10958 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/api/github.py
+-rw-r--r--   0 root         (0) root         (0)    30846 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/api/koreainvestment.py
+-rw-r--r--   0 root         (0) root         (0)     5011 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/api/open_ai.py
+-rw-r--r--   0 root         (0) root         (0)     7698 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/api/slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 17:14:17.778648 zerohertzlib-1.1.2/zerohertzLib/logging/
+-rw-r--r--   0 root         (0) root         (0)      359 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/logging/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4738 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/logging/handler.py
+-rw-r--r--   0 root         (0) root         (0)     5264 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/logging/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 17:14:17.778648 zerohertzlib-1.1.2/zerohertzLib/mlops/
+-rw-r--r--   0 root         (0) root         (0)      273 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/mlops/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2580 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/mlops/cli.py
+-rw-r--r--   0 root         (0) root         (0)    18197 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/mlops/triton.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 17:14:17.778648 zerohertzlib-1.1.2/zerohertzLib/monitoring/
+-rw-r--r--   0 root         (0) root         (0)      333 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2829 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/monitoring/cpu.py
+-rw-r--r--   0 root         (0) root         (0)     5184 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/monitoring/gpu.py
+-rw-r--r--   0 root         (0) root         (0)     2678 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/monitoring/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 17:14:17.782648 zerohertzlib-1.1.2/zerohertzLib/plot/
+-rw-r--r--   0 root         (0) root         (0)     1552 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/plot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15381 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/plot/bar_chart.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 17:14:17.786648 zerohertzlib-1.1.2/zerohertzLib/plot/fonts/
+-rw-r--r--   0 root         (0) root         (0)  7549348 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf
+-rw-r--r--   0 root         (0) root         (0)   347988 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/plot/fonts/times.ttf
+-rw-r--r--   0 root         (0) root         (0)     3435 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/plot/pie.py
+-rw-r--r--   0 root         (0) root         (0)    11476 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/plot/plot.py
+-rw-r--r--   0 root         (0) root         (0)     4046 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/plot/scatter.py
+-rw-r--r--   0 root         (0) root         (0)     3292 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/plot/table.py
+-rw-r--r--   0 root         (0) root         (0)     4838 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/plot/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 17:14:17.786648 zerohertzlib-1.1.2/zerohertzLib/quant/
+-rw-r--r--   0 root         (0) root         (0)      885 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/quant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14935 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/quant/backtest.py
+-rw-r--r--   0 root         (0) root         (0)    13182 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/quant/methods.py
+-rw-r--r--   0 root         (0) root         (0)    44465 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/quant/quant.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/quant/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 17:14:17.786648 zerohertzlib-1.1.2/zerohertzLib/util/
+-rw-r--r--   0 root         (0) root         (0)      458 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4527 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/util/csv.py
+-rw-r--r--   0 root         (0) root         (0)    11173 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/util/data.py
+-rw-r--r--   0 root         (0) root         (0)    11652 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/util/json.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 17:14:17.786648 zerohertzlib-1.1.2/zerohertzLib/vision/
+-rw-r--r--   0 root         (0) root         (0)     1623 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/vision/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1992 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/vision/cli.py
+-rw-r--r--   0 root         (0) root         (0)     6967 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/vision/compare.py
+-rw-r--r--   0 root         (0) root         (0)    12885 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/vision/convert.py
+-rw-r--r--   0 root         (0) root         (0)    22463 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/vision/data.py
+-rw-r--r--   0 root         (0) root         (0)    14878 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/vision/eval.py
+-rw-r--r--   0 root         (0) root         (0)     4188 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/vision/gif.py
+-rw-r--r--   0 root         (0) root         (0)    22281 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/vision/loader.py
+-rw-r--r--   0 root         (0) root         (0)     7826 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/vision/transform.py
+-rw-r--r--   0 root         (0) root         (0)     4219 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/vision/util.py
+-rw-r--r--   0 root         (0) root         (0)    17516 2024-05-31 17:14:11.000000 zerohertzlib-1.1.2/zerohertzLib/vision/visual.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 17:14:17.786648 zerohertzlib-1.1.2/zerohertzLib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6433 2024-05-31 17:14:17.000000 zerohertzlib-1.1.2/zerohertzLib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2091 2024-05-31 17:14:17.000000 zerohertzlib-1.1.2/zerohertzLib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 17:14:17.000000 zerohertzlib-1.1.2/zerohertzLib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      132 2024-05-31 17:14:17.000000 zerohertzlib-1.1.2/zerohertzLib.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      457 2024-05-31 17:14:17.000000 zerohertzlib-1.1.2/zerohertzLib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2024-05-31 17:14:17.000000 zerohertzlib-1.1.2/zerohertzLib.egg-info/top_level.txt
```

### Comparing `zerohertzLib-1.1.1/LICENSE` & `zerohertzlib-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/PKG-INFO` & `zerohertzlib-1.1.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: zerohertzLib
-Version: 1.1.1
-Summary: Zerohertz's Library
-Home-page: https://github.com/Zerohertz/zerohertzLib
-Author: Zerohertz
-Author-email: ohg3417@gmail.com
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-Provides-Extra: api
-Provides-Extra: mlops
-Provides-Extra: quant
-Provides-Extra: all
-License-File: LICENSE
-
-
 <p align="center">
     <img src="https://github.com/Zerohertz/Zerohertz/assets/42334717/90adcc0f-c6ec-4aca-af41-856931956093">
 </p>
 
 <h2 align = "center">
     ⚡ Zerohertz's Library ⚡
 </h2>
```

#### html2text {}

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1 Name: zerohertzLib Version: 1.1.1 Summary: Zerohertz's
-Library Home-page: https://github.com/Zerohertz/zerohertzLib Author: Zerohertz
-Author-email: ohg3417@gmail.com License: MIT Classifier: Development Status ::
-5 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
-Intended Audience :: Education Classifier: Intended Audience :: Science/
-Research Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
-Scientific/Engineering :: Mathematics Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Classifier: Topic :: Software
-Development Classifier: Topic :: Software Development :: Libraries Classifier:
-Topic :: Software Development :: Libraries :: Python Modules Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7.0 Description-Content-Type: text/markdown Provides-
-Extra: api Provides-Extra: mlops Provides-Extra: quant Provides-Extra: all
-License-File: LICENSE
   [https://github.com/Zerohertz/Zerohertz/assets/42334717/90adcc0f-c6ec-4aca-
                               af41-856931956093]
                     ********** ?â??¡ ZZeerroohheerrttzz''ss LLiibbrraarryy ?â??¡ **********
    _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_G_i_t_H_u_b_-_1_8_1_7_1_7_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
    _b_a_d_g_e_&_l_o_g_o_=_G_i_t_H_u_b_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_J_e_n_k_i_n_s_-
        _D_2_4_9_3_9_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_=_J_e_n_k_i_n_s_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_]_[_h_t_t_p_s_:_/_/
          _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_Z_e_r_o_h_e_r_t_z_'_s_%_2_0_B_l_o_g_-_8_0_0_a_0_a_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
```

### Comparing `zerohertzLib-1.1.1/test/test_algorithm.py` & `zerohertzlib-1.1.2/test/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/test/test_api.py` & `zerohertzlib-1.1.2/test/test_api.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/test/test_logging.py` & `zerohertzlib-1.1.2/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/test/test_plot.py` & `zerohertzlib-1.1.2/test/test_plot.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/test/test_quant.py` & `zerohertzlib-1.1.2/test/test_quant.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/test/test_util.py` & `zerohertzlib-1.1.2/test/test_util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/test/test_vision.py` & `zerohertzlib-1.1.2/test/test_vision.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/__init__.py` & `zerohertzlib-1.1.2/zerohertzLib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,8 +52,8 @@
     print("=" * 100)
     print(f"[Warning] {error}")
     print("Please Install OpenCV Dependency")
     print("--->\t$ sudo apt install python3-opencv -y\t<---")
     print("(but you can use other submodules except zerohertzLib.vision)")
     print("=" * 100)
 
-__version__ = "v1.1.1"
+__version__ = "v1.1.2"
```

### Comparing `zerohertzLib-1.1.1/zerohertzLib/algorithm/__init__.py` & `zerohertzlib-1.1.2/zerohertzLib/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/algorithm/bisect.py` & `zerohertzlib-1.1.2/zerohertzLib/algorithm/bisect.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/algorithm/collections.py` & `zerohertzlib-1.1.2/zerohertzLib/algorithm/collections.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/algorithm/fft.py` & `zerohertzlib-1.1.2/zerohertzLib/algorithm/fft.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/algorithm/graph.py` & `zerohertzlib-1.1.2/zerohertzLib/algorithm/graph.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/algorithm/prime.py` & `zerohertzlib-1.1.2/zerohertzLib/algorithm/prime.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/algorithm/sort.py` & `zerohertzlib-1.1.2/zerohertzLib/algorithm/sort.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/api/discord.py` & `zerohertzlib-1.1.2/zerohertzLib/api/discord.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/api/github.py` & `zerohertzlib-1.1.2/zerohertzLib/api/github.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/api/koreainvestment.py` & `zerohertzlib-1.1.2/zerohertzLib/api/koreainvestment.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/api/open_ai.py` & `zerohertzlib-1.1.2/zerohertzLib/api/open_ai.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/api/slack.py` & `zerohertzlib-1.1.2/zerohertzLib/api/slack.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/logging/handler.py` & `zerohertzlib-1.1.2/zerohertzLib/logging/handler.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/logging/logger.py` & `zerohertzlib-1.1.2/zerohertzLib/logging/logger.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/mlops/triton.py` & `zerohertzlib-1.1.2/zerohertzLib/mlops/triton.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 
 class TritonClientURL(grpcclient.InferenceServerClient):
     """외부에서 실행되는 triton inference server의 호출을 위한 class
 
     Args:
         url (``str``): 호출할 triton inference server의 URL
         port (``Optional[int]``): triton inference server의 gRPC 통신 port 번호
+        verbose (``Optional[bool]``): Verbose 출력 여부
 
     Methods:
         __call__:
             Model 호출 수행
 
             Args:
                 model (``Union[int, str]``): 호출할 model의 이름 및 ID
@@ -243,14 +244,15 @@
 class TritonClientK8s(TritonClientURL):
     """Kubernetes에서 실행되는 triton inference server의 호출을 위한 class
 
     Args:
         svc_name (``str``): 호출할 triton inference server의 Kubernetes service의 이름
         namespace (``str``): 호출할 triton inference server의 namespace
         port (``Optional[int]``): triton inference server의 gRPC 통신 port 번호
+        verbose (``Optional[bool]``): Verbose 출력 여부
 
     Methods:
         __call__:
             Model 호출 수행
 
             Args:
                 model (``Union[int, str]``): 호출할 model의 이름 또는 ID
@@ -272,17 +274,21 @@
             >>> tc = zz.mlops.TritonClientK8s("triton-inference-server-svc", "yolo")
             >>> tc("YOLO", np.zeros((1, 3, 640, 640)))
             {'output0': array([[[3.90108061e+00, 3.51982164e+00, 7.49971962e+00, ...,
             2.21481919e-03, 1.17585063e-03, 1.36753917e-03]]], dtype=float32)}
     """
 
     def __init__(
-        self, svc_name: str, namespace: str, port: Optional[int] = 8001
+        self,
+        svc_name: str,
+        namespace: str,
+        port: Optional[int] = 8001,
+        verbose: Optional[bool] = False,
     ) -> None:
-        super().__init__(f"{svc_name}.{namespace}", port)
+        super().__init__(f"{svc_name}.{namespace}", port, verbose)
 
 
 class BaseTritonPythonModel(ABC):
     """Triton Inference Server에서 Python backend 사용을 위한 class
 
     Note:
         Abstract Base Class: Model의 추론을 수행하는 abstract method ``_inference`` 정의 후 사용
```

### Comparing `zerohertzLib-1.1.1/zerohertzLib/monitoring/cpu.py` & `zerohertzlib-1.1.2/zerohertzLib/monitoring/cpu.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/monitoring/gpu.py` & `zerohertzlib-1.1.2/zerohertzLib/monitoring/gpu.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/monitoring/storage.py` & `zerohertzlib-1.1.2/zerohertzLib/monitoring/storage.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/plot/__init__.py` & `zerohertzlib-1.1.2/zerohertzLib/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/plot/bar_chart.py` & `zerohertzlib-1.1.2/zerohertzLib/plot/bar_chart.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf` & `zerohertzlib-1.1.2/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/plot/fonts/times.ttf` & `zerohertzlib-1.1.2/zerohertzLib/plot/fonts/times.ttf`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/plot/pie.py` & `zerohertzlib-1.1.2/zerohertzLib/plot/pie.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/plot/plot.py` & `zerohertzlib-1.1.2/zerohertzLib/plot/plot.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/plot/scatter.py` & `zerohertzlib-1.1.2/zerohertzLib/plot/scatter.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/plot/table.py` & `zerohertzlib-1.1.2/zerohertzLib/plot/table.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/plot/util.py` & `zerohertzlib-1.1.2/zerohertzLib/plot/util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/quant/__init__.py` & `zerohertzlib-1.1.2/zerohertzLib/quant/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/quant/backtest.py` & `zerohertzlib-1.1.2/zerohertzLib/quant/backtest.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/quant/methods.py` & `zerohertzlib-1.1.2/zerohertzLib/quant/methods.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/quant/quant.py` & `zerohertzlib-1.1.2/zerohertzLib/quant/quant.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/quant/util.py` & `zerohertzlib-1.1.2/zerohertzLib/quant/util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/util/csv.py` & `zerohertzlib-1.1.2/zerohertzLib/util/csv.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/util/data.py` & `zerohertzlib-1.1.2/zerohertzLib/util/data.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/util/json.py` & `zerohertzlib-1.1.2/zerohertzLib/util/json.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/vision/__init__.py` & `zerohertzlib-1.1.2/zerohertzLib/vision/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/vision/compare.py` & `zerohertzlib-1.1.2/zerohertzLib/vision/compare.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/vision/convert.py` & `zerohertzlib-1.1.2/zerohertzLib/vision/convert.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/vision/data.py` & `zerohertzlib-1.1.2/zerohertzLib/vision/data.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/vision/eval.py` & `zerohertzlib-1.1.2/zerohertzLib/vision/eval.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/vision/gif.py` & `zerohertzlib-1.1.2/zerohertzLib/vision/gif.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/vision/loader.py` & `zerohertzlib-1.1.2/zerohertzLib/vision/loader.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/vision/transform.py` & `zerohertzlib-1.1.2/zerohertzLib/vision/transform.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/vision/util.py` & `zerohertzlib-1.1.2/zerohertzLib/vision/util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib/vision/visual.py` & `zerohertzlib-1.1.2/zerohertzLib/vision/visual.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.1.1/zerohertzLib.egg-info/SOURCES.txt` & `zerohertzlib-1.1.2/zerohertzLib.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 LICENSE
 MANIFEST.in
 README.md
-setup.py
+pyproject.toml
+sphinx/example_images.py
+sphinx/release_note.py
+sphinx/source/conf.py
 test/test_algorithm.py
 test/test_api.py
 test/test_logging.py
 test/test_monitoring.py
 test/test_plot.py
 test/test_quant.py
 test/test_util.py
 test/test_vision.py
 zerohertzLib/__init__.py
 zerohertzLib.egg-info/PKG-INFO
 zerohertzLib.egg-info/SOURCES.txt
 zerohertzLib.egg-info/dependency_links.txt
+zerohertzLib.egg-info/entry_points.txt
 zerohertzLib.egg-info/requires.txt
 zerohertzLib.egg-info/top_level.txt
 zerohertzLib/algorithm/__init__.py
 zerohertzLib/algorithm/bisect.py
 zerohertzLib/algorithm/collections.py
 zerohertzLib/algorithm/fft.py
 zerohertzLib/algorithm/graph.py
@@ -29,14 +33,15 @@
 zerohertzLib/api/koreainvestment.py
 zerohertzLib/api/open_ai.py
 zerohertzLib/api/slack.py
 zerohertzLib/logging/__init__.py
 zerohertzLib/logging/handler.py
 zerohertzLib/logging/logger.py
 zerohertzLib/mlops/__init__.py
+zerohertzLib/mlops/cli.py
 zerohertzLib/mlops/triton.py
 zerohertzLib/monitoring/__init__.py
 zerohertzLib/monitoring/cpu.py
 zerohertzLib/monitoring/gpu.py
 zerohertzLib/monitoring/storage.py
 zerohertzLib/plot/__init__.py
 zerohertzLib/plot/bar_chart.py
@@ -53,14 +58,15 @@
 zerohertzLib/quant/quant.py
 zerohertzLib/quant/util.py
 zerohertzLib/util/__init__.py
 zerohertzLib/util/csv.py
 zerohertzLib/util/data.py
 zerohertzLib/util/json.py
 zerohertzLib/vision/__init__.py
+zerohertzLib/vision/cli.py
 zerohertzLib/vision/compare.py
 zerohertzLib/vision/convert.py
 zerohertzLib/vision/data.py
 zerohertzLib/vision/eval.py
 zerohertzLib/vision/gif.py
 zerohertzLib/vision/loader.py
 zerohertzLib/vision/transform.py
```

