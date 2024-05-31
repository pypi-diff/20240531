# Comparing `tmp/cellfinder-1.3.0rc0.tar.gz` & `tmp/cellfinder-1.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellfinder-1.3.0rc0.tar", last modified: Tue May 28 15:38:41 2024, max compression
+gzip compressed data, was "cellfinder-1.3.0rc1.tar", last modified: Fri May 31 13:59:40 2024, max compression
```

## Comparing `cellfinder-1.3.0rc0.tar` & `cellfinder-1.3.0rc1.tar`

### file list

```diff
@@ -1,254 +1,89 @@
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.218645 cellfinder-1.3.0rc0/.github/
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/.github/workflows/
--rw-rw-r--   0 adam      (1001) adam      (1001)     5102 2024-05-28 15:38:31.000000 cellfinder-1.3.0rc0/.github/workflows/test_and_deploy.yml
--rw-rw-r--   0 adam      (1001) adam      (1001)     1779 2024-05-28 15:38:31.000000 cellfinder-1.3.0rc0/.github/workflows/test_include_guard.yaml
--rw-rw-r--   0 adam      (1001) adam      (1001)     1493 2024-05-07 13:49:17.000000 cellfinder-1.3.0rc0/.gitignore
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/.napari/
--rw-rw-r--   0 adam      (1001) adam      (1001)      342 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/.napari/config.yml
--rw-rw-r--   0 adam      (1001) adam      (1001)     1806 2024-05-07 13:49:17.000000 cellfinder-1.3.0rc0/CITATION.cff
--rw-rw-r--   0 adam      (1001) adam      (1001)     1564 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/LICENSE
--rw-rw-r--   0 adam      (1001) adam      (1001)      320 2024-05-07 13:49:17.000000 cellfinder-1.3.0rc0/MANIFEST.in
--rw-r--r--   0 adam      (1001) adam      (1001)     6457 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1001)     4180 2024-05-28 14:59:11.000000 cellfinder-1.3.0rc0/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/cellfinder/
--rw-rw-r--   0 adam      (1001) adam      (1001)     1182 2024-05-28 14:59:11.000000 cellfinder-1.3.0rc0/cellfinder/__init__.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/cellfinder/__pycache__/
--rw-rw-r--   0 adam      (1001) adam      (1001)     1336 2024-05-28 13:04:31.000000 cellfinder-1.3.0rc0/cellfinder/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     2087 2024-05-23 15:52:38.000000 cellfinder-1.3.0rc0/cellfinder/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     1302 2024-05-28 14:59:17.000000 cellfinder-1.3.0rc0/cellfinder/__pycache__/__init__.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     1578 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/cli_migration_warning.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/cellfinder/core/
--rw-rw-r--   0 adam      (1001) adam      (1001)       62 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/__init__.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/cellfinder/core/__pycache__/
--rw-rw-r--   0 adam      (1001) adam      (1001)      229 2024-01-03 15:53:03.000000 cellfinder-1.3.0rc0/cellfinder/core/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)      287 2024-05-23 15:52:58.000000 cellfinder-1.3.0rc0/cellfinder/core/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)      279 2024-05-23 14:13:04.000000 cellfinder-1.3.0rc0/cellfinder/core/__pycache__/__init__.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     3097 2024-05-28 10:53:41.000000 cellfinder-1.3.0rc0/cellfinder/core/__pycache__/main.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     4249 2024-05-23 15:52:59.000000 cellfinder-1.3.0rc0/cellfinder/core/__pycache__/main.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     3866 2024-05-28 15:02:46.000000 cellfinder-1.3.0rc0/cellfinder/core/__pycache__/main.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)      287 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/core/__pycache__/types.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)      382 2024-05-23 15:52:59.000000 cellfinder-1.3.0rc0/cellfinder/core/__pycache__/types.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)      355 2024-05-23 14:13:05.000000 cellfinder-1.3.0rc0/cellfinder/core/__pycache__/types.cpython-312.pyc
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/cellfinder/core/classify/
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__init__.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/
--rw-rw-r--   0 adam      (1001) adam      (1001)      171 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)      187 2024-05-23 15:52:58.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)      175 2024-05-23 14:13:04.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/__init__.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     4335 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/augment.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     7771 2024-05-23 15:52:59.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/augment.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     7149 2024-05-23 14:13:05.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/augment.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     3016 2024-05-28 10:53:42.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/classify.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     4579 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/classify.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     4128 2024-05-28 15:02:54.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/classify.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)    14282 2024-05-28 10:53:42.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/cube_generator.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)    24420 2024-05-23 15:52:58.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/cube_generator.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)    22810 2024-05-28 14:59:19.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/cube_generator.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     7352 2024-05-28 10:53:41.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/resnet.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)    11288 2024-05-23 15:53:00.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/resnet.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     9766 2024-05-28 14:59:19.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/resnet.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     2364 2024-05-28 10:53:42.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/tools.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     3544 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/tools.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     3259 2024-05-28 15:02:54.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/__pycache__/tools.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     6321 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/augment.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     3061 2024-05-28 14:59:11.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/classify.py
--rw-rw-r--   0 adam      (1001) adam      (1001)    17125 2024-05-28 14:59:11.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/cube_generator.py
--rw-rw-r--   0 adam      (1001) adam      (1001)    10034 2024-05-28 14:59:11.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/resnet.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     2560 2024-05-28 14:59:11.000000 cellfinder-1.3.0rc0/cellfinder/core/classify/tools.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/cellfinder/core/config/
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/config/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1001)       56 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/config/cellfinder.conf
--rw-rw-r--   0 adam      (1001) adam      (1001)      107 2024-01-03 15:53:15.000000 cellfinder-1.3.0rc0/cellfinder/core/config/cellfinder.conf.custom
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/cellfinder/core/detect/
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/__init__.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/cellfinder/core/detect/__pycache__/
--rw-rw-r--   0 adam      (1001) adam      (1001)      169 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)      185 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)      173 2024-05-23 14:13:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/__pycache__/__init__.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     7846 2024-05-07 13:49:24.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/__pycache__/detect.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)    11736 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/__pycache__/detect.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)    10384 2024-05-23 14:13:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/__pycache__/detect.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     9592 2024-05-07 13:49:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/detect.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/__init__.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/__pycache__/
--rw-rw-r--   0 adam      (1001) adam      (1001)      177 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)      193 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)      181 2024-05-23 14:13:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/__pycache__/__init__.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     2038 2024-05-07 15:42:37.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/__pycache__/setup_filters.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     2707 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/__pycache__/setup_filters.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     2500 2024-05-23 14:13:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/__pycache__/setup_filters.cpython-312.pyc
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/
--rw-rw-r--   0 adam      (1001) adam      (1001)       40 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/__init__.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/__pycache__/
--rw-rw-r--   0 adam      (1001) adam      (1001)      233 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)      263 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)      240 2024-05-23 14:13:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/__pycache__/__init__.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     1449 2024-05-07 13:49:24.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/__pycache__/classical_filter.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     1942 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/__pycache__/classical_filter.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     1829 2024-05-23 14:13:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/__pycache__/classical_filter.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     2808 2024-05-07 15:42:37.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/__pycache__/plane_filter.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     3857 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/__pycache__/plane_filter.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     3665 2024-05-23 14:13:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/__pycache__/plane_filter.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     3082 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/__pycache__/tile_walker.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     4520 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/__pycache__/tile_walker.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     4496 2024-05-23 14:13:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/__pycache__/tile_walker.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     1331 2024-05-07 13:49:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/classical_filter.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     2746 2024-05-07 15:02:11.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/plane_filter.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     3001 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/tile_walker.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     2084 2024-05-07 15:02:11.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/setup_filters.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__init__.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.222645 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/
--rw-rw-r--   0 adam      (1001) adam      (1001)      184 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)      200 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)      188 2024-05-23 14:13:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/__init__.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)    31524 2024-01-16 13:15:35.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/ball_filter._cube_overlaps-199.py310.1.nbc
--rw-rw-r--   0 adam      (1001) adam      (1001)     1478 2024-01-16 13:15:35.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/ball_filter._cube_overlaps-199.py310.nbi
--rw-rw-r--   0 adam      (1001) adam      (1001)    33890 2024-05-09 11:20:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/ball_filter._cube_overlaps-263.py310.1.nbc
--rw-rw-r--   0 adam      (1001) adam      (1001)    34146 2024-05-09 11:20:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/ball_filter._cube_overlaps-263.py310.2.nbc
--rw-rw-r--   0 adam      (1001) adam      (1001)     2498 2024-05-09 11:20:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/ball_filter._cube_overlaps-263.py310.nbi
--rw-rw-r--   0 adam      (1001) adam      (1001)    33846 2024-05-23 15:53:33.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/ball_filter._cube_overlaps-263.py311.1.nbc
--rw-rw-r--   0 adam      (1001) adam      (1001)    34102 2024-05-23 15:53:34.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/ball_filter._cube_overlaps-263.py311.2.nbc
--rw-rw-r--   0 adam      (1001) adam      (1001)     2498 2024-05-23 15:53:34.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/ball_filter._cube_overlaps-263.py311.nbi
--rw-rw-r--   0 adam      (1001) adam      (1001)    33929 2024-05-23 14:13:33.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/ball_filter._cube_overlaps-263.py312.1.nbc
--rw-rw-r--   0 adam      (1001) adam      (1001)    34185 2024-05-23 14:13:33.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/ball_filter._cube_overlaps-263.py312.2.nbc
--rw-rw-r--   0 adam      (1001) adam      (1001)     2498 2024-05-23 14:13:33.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/ball_filter._cube_overlaps-263.py312.nbi
--rw-rw-r--   0 adam      (1001) adam      (1001)     9803 2024-05-07 13:49:24.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/ball_filter.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)    15888 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/ball_filter.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)    14649 2024-05-23 14:13:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/ball_filter.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     9893 2024-05-07 13:49:24.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/structure_detection.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)    15465 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/structure_detection.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)    14790 2024-05-23 14:13:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/structure_detection.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     6806 2024-05-07 13:49:24.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/structure_splitting.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)    11313 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/structure_splitting.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)    10217 2024-05-23 14:13:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/structure_splitting.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     5437 2024-05-07 13:49:24.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/volume_filter.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)    10104 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/volume_filter.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     9349 2024-05-23 14:13:29.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/__pycache__/volume_filter.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)    13894 2024-05-07 13:49:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/ball_filter.py
--rw-rw-r--   0 adam      (1001) adam      (1001)    11307 2024-05-07 13:49:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/structure_detection.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     7660 2024-05-07 13:49:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/structure_splitting.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     7035 2024-05-07 13:49:17.000000 cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/volume_filter.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/cellfinder/core/download/
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/download/__init__.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/cellfinder/core/download/__pycache__/
--rw-rw-r--   0 adam      (1001) adam      (1001)      171 2024-01-03 15:53:03.000000 cellfinder-1.3.0rc0/cellfinder/core/download/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)      187 2024-05-23 15:52:59.000000 cellfinder-1.3.0rc0/cellfinder/core/download/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)      175 2024-05-23 14:13:05.000000 cellfinder-1.3.0rc0/cellfinder/core/download/__pycache__/__init__.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     1857 2024-05-09 10:52:26.000000 cellfinder-1.3.0rc0/cellfinder/core/download/__pycache__/cli.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     2316 2024-05-23 15:17:23.000000 cellfinder-1.3.0rc0/cellfinder/core/download/__pycache__/cli.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     3264 2024-05-09 10:45:04.000000 cellfinder-1.3.0rc0/cellfinder/core/download/__pycache__/download.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     4608 2024-05-23 15:52:59.000000 cellfinder-1.3.0rc0/cellfinder/core/download/__pycache__/download.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     4057 2024-05-23 14:13:05.000000 cellfinder-1.3.0rc0/cellfinder/core/download/__pycache__/download.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     1764 2024-05-09 10:43:09.000000 cellfinder-1.3.0rc0/cellfinder/core/download/cli.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     3277 2024-05-09 10:43:09.000000 cellfinder-1.3.0rc0/cellfinder/core/download/download.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     3625 2024-05-28 14:59:11.000000 cellfinder-1.3.0rc0/cellfinder/core/main.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/cellfinder/core/tools/
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__init__.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/
--rw-rw-r--   0 adam      (1001) adam      (1001)     2743 2024-05-23 13:35:02.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/IO.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)      168 2024-01-03 15:53:03.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)      184 2024-05-23 15:52:59.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)      172 2024-05-23 14:13:05.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/__init__.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     3065 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/array_operations.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     4786 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/array_operations.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     4433 2024-05-23 14:13:29.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/array_operations.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     1325 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/geometry.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     1924 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/geometry.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     1694 2024-05-23 14:13:29.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/geometry.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     1869 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/image_processing.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     2434 2024-05-23 15:14:59.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/image_processing.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     1831 2024-05-28 10:53:42.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/prep.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     2982 2024-05-23 15:53:17.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/prep.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     2640 2024-05-28 15:02:54.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/prep.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     1153 2024-05-09 10:45:04.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/source_files.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     1338 2024-05-23 15:52:59.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/source_files.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     1282 2024-05-23 14:13:05.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/source_files.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     2738 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/system.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     3303 2024-05-23 15:14:59.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/system.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     1590 2024-01-03 15:53:03.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/tf.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     4167 2024-01-03 15:53:41.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/tiff.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     4889 2024-05-23 15:17:23.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/tiff.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     5418 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/tools.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     7524 2024-05-23 15:52:59.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/tools.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     6614 2024-05-23 14:13:05.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/tools.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     3371 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/array_operations.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     1124 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/geometry.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     2269 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/image_processing.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     2175 2024-05-28 14:59:11.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/prep.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      856 2024-05-09 10:43:09.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/source_files.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     2232 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/system.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     2899 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/tiff.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     4867 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/tools/tools.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/cellfinder/core/train/
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/train/__init__.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/cellfinder/core/train/__pycache__/
--rw-rw-r--   0 adam      (1001) adam      (1001)      168 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/core/train/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)      184 2024-05-23 15:52:59.000000 cellfinder-1.3.0rc0/cellfinder/core/train/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)      172 2024-05-23 14:13:05.000000 cellfinder-1.3.0rc0/cellfinder/core/train/__pycache__/__init__.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     9635 2024-05-28 10:53:41.000000 cellfinder-1.3.0rc0/cellfinder/core/train/__pycache__/train_yml.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)    15619 2024-05-23 15:52:59.000000 cellfinder-1.3.0rc0/cellfinder/core/train/__pycache__/train_yml.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)    13611 2024-05-28 14:59:19.000000 cellfinder-1.3.0rc0/cellfinder/core/train/__pycache__/train_yml.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)    13260 2024-05-28 14:59:11.000000 cellfinder-1.3.0rc0/cellfinder/core/train/train_yml.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      106 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/core/types.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/cellfinder/napari/
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2024-01-16 12:55:27.000000 cellfinder-1.3.0rc0/cellfinder/napari/__init__.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/cellfinder/napari/__pycache__/
--rw-rw-r--   0 adam      (1001) adam      (1001)      164 2024-01-16 12:55:32.000000 cellfinder-1.3.0rc0/cellfinder/napari/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)      180 2024-05-23 15:52:58.000000 cellfinder-1.3.0rc0/cellfinder/napari/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)      168 2024-05-23 14:13:04.000000 cellfinder-1.3.0rc0/cellfinder/napari/__pycache__/__init__.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)    16221 2024-05-07 13:49:25.000000 cellfinder-1.3.0rc0/cellfinder/napari/__pycache__/curation.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)    26918 2024-05-23 14:14:01.000000 cellfinder-1.3.0rc0/cellfinder/napari/__pycache__/curation.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     2378 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/napari/__pycache__/input_container.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     3071 2024-05-23 15:52:59.000000 cellfinder-1.3.0rc0/cellfinder/napari/__pycache__/input_container.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     2769 2024-05-23 14:13:05.000000 cellfinder-1.3.0rc0/cellfinder/napari/__pycache__/input_container.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)      960 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/napari/__pycache__/sample_data.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     1373 2024-05-23 14:13:10.000000 cellfinder-1.3.0rc0/cellfinder/napari/__pycache__/sample_data.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     3817 2024-05-07 13:49:25.000000 cellfinder-1.3.0rc0/cellfinder/napari/__pycache__/utils.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     5550 2024-05-23 15:52:59.000000 cellfinder-1.3.0rc0/cellfinder/napari/__pycache__/utils.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     4934 2024-05-23 14:13:05.000000 cellfinder-1.3.0rc0/cellfinder/napari/__pycache__/utils.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)    21447 2024-05-07 13:49:17.000000 cellfinder-1.3.0rc0/cellfinder/napari/curation.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/cellfinder/napari/detect/
--rw-rw-r--   0 adam      (1001) adam      (1001)       34 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/__init__.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/cellfinder/napari/detect/__pycache__/
--rw-rw-r--   0 adam      (1001) adam      (1001)      215 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)      245 2024-05-23 15:52:58.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)      222 2024-05-23 14:13:04.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/__pycache__/__init__.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)    10018 2024-05-07 13:49:25.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/__pycache__/detect.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)    14902 2024-05-23 15:52:58.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/__pycache__/detect.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)    13667 2024-05-23 14:13:04.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/__pycache__/detect.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     5225 2024-05-07 13:49:25.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/__pycache__/detect_containers.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     8717 2024-05-23 15:52:59.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/__pycache__/detect_containers.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     7387 2024-05-23 14:13:05.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/__pycache__/detect_containers.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     3305 2024-05-07 13:49:25.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/__pycache__/thread_worker.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     5136 2024-05-23 15:52:59.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/__pycache__/thread_worker.cpython-311.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     4576 2024-05-23 14:13:05.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/__pycache__/thread_worker.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)    13658 2024-05-07 13:49:17.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/detect.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     5377 2024-05-07 13:49:17.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/detect_containers.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     3078 2024-05-07 13:49:17.000000 cellfinder-1.3.0rc0/cellfinder/napari/detect/thread_worker.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     2150 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/napari/input_container.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      921 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/napari/napari.yaml
--rw-rw-r--   0 adam      (1001) adam      (1001)      732 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/napari/sample_data.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/cellfinder/napari/train/
--rw-rw-r--   0 adam      (1001) adam      (1001)       35 2024-01-03 15:51:03.000000 cellfinder-1.3.0rc0/cellfinder/napari/train/__init__.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/cellfinder/napari/train/__pycache__/
--rw-rw-r--   0 adam      (1001) adam      (1001)      215 2024-01-03 15:53:05.000000 cellfinder-1.3.0rc0/cellfinder/napari/train/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)      222 2024-05-23 14:14:04.000000 cellfinder-1.3.0rc0/cellfinder/napari/train/__pycache__/__init__.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     5073 2024-05-07 13:49:25.000000 cellfinder-1.3.0rc0/cellfinder/napari/train/__pycache__/train.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     7017 2024-05-23 14:14:04.000000 cellfinder-1.3.0rc0/cellfinder/napari/train/__pycache__/train.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     4609 2024-05-09 10:51:35.000000 cellfinder-1.3.0rc0/cellfinder/napari/train/__pycache__/train_containers.cpython-310.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     6891 2024-05-23 15:15:00.000000 cellfinder-1.3.0rc0/cellfinder/napari/train/__pycache__/train_containers.cpython-312.pyc
--rw-rw-r--   0 adam      (1001) adam      (1001)     5941 2024-05-07 13:49:17.000000 cellfinder-1.3.0rc0/cellfinder/napari/train/train.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     4386 2024-05-09 10:43:09.000000 cellfinder-1.3.0rc0/cellfinder/napari/train/train_containers.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     3824 2024-05-07 13:49:17.000000 cellfinder-1.3.0rc0/cellfinder/napari/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/cellfinder.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1001)     6457 2024-05-28 15:38:40.000000 cellfinder-1.3.0rc0/cellfinder.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1001)    12378 2024-05-28 15:38:41.000000 cellfinder-1.3.0rc0/cellfinder.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1001)        1 2024-05-28 15:38:40.000000 cellfinder-1.3.0rc0/cellfinder.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1001)      247 2024-05-28 15:38:40.000000 cellfinder-1.3.0rc0/cellfinder.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1001)      373 2024-05-28 15:38:40.000000 cellfinder-1.3.0rc0/cellfinder.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1001)       11 2024-05-28 15:38:40.000000 cellfinder-1.3.0rc0/cellfinder.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1001)     3499 2024-05-28 15:38:31.000000 cellfinder-1.3.0rc0/pyproject.toml
--rw-rw-r--   0 adam      (1001) adam      (1001)       38 2024-05-28 15:38:41.226645 cellfinder-1.3.0rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.967397 cellfinder-1.3.0rc1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.951397 cellfinder-1.3.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.955397 cellfinder-1.3.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/.github/workflows/test_include_guard.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.955397 cellfinder-1.3.0rc1/.napari/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/.napari/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-05-31 13:59:40.967397 cellfinder-1.3.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.955397 cellfinder-1.3.0rc1/cellfinder/
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/cli_migration_warning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.955397 cellfinder-1.3.0rc1/cellfinder/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.955397 cellfinder-1.3.0rc1/cellfinder/core/classify/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/classify/augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/classify/classify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17125 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/classify/cube_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10034 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/classify/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/classify/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.959397 cellfinder-1.3.0rc1/cellfinder/core/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/config/cellfinder.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.959397 cellfinder-1.3.0rc1/cellfinder/core/detect/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/detect/detect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.959397 cellfinder-1.3.0rc1/cellfinder/core/detect/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/detect/filters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.959397 cellfinder-1.3.0rc1/cellfinder/core/detect/filters/plane/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/detect/filters/plane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/detect/filters/plane/classical_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/detect/filters/plane/plane_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/detect/filters/plane/tile_walker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/detect/filters/setup_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.959397 cellfinder-1.3.0rc1/cellfinder/core/detect/filters/volume/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/detect/filters/volume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13894 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/detect/filters/volume/ball_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/detect/filters/volume/structure_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/detect/filters/volume/structure_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7035 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/detect/filters/volume/volume_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.959397 cellfinder-1.3.0rc1/cellfinder/core/download/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/download/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/download/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.959397 cellfinder-1.3.0rc1/cellfinder/core/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/tools/array_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/tools/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/tools/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/tools/prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/tools/source_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/tools/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/tools/tiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/tools/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.963397 cellfinder-1.3.0rc1/cellfinder/core/train/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13260 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/train/train_yml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/core/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.963397 cellfinder-1.3.0rc1/cellfinder/napari/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/napari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21447 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/napari/curation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.963397 cellfinder-1.3.0rc1/cellfinder/napari/detect/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/napari/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13658 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/napari/detect/detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/napari/detect/detect_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/napari/detect/thread_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/napari/input_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/napari/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/napari/sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.963397 cellfinder-1.3.0rc1/cellfinder/napari/train/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/napari/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/napari/train/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/napari/train/train_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/cellfinder/napari/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:40.963397 cellfinder-1.3.0rc1/cellfinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-05-31 13:59:40.000000 cellfinder-1.3.0rc1/cellfinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-31 13:59:40.000000 cellfinder-1.3.0rc1/cellfinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:59:40.000000 cellfinder-1.3.0rc1/cellfinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-31 13:59:40.000000 cellfinder-1.3.0rc1/cellfinder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-31 13:59:40.000000 cellfinder-1.3.0rc1/cellfinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 13:59:40.000000 cellfinder-1.3.0rc1/cellfinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-31 13:59:33.000000 cellfinder-1.3.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 13:59:40.967397 cellfinder-1.3.0rc1/setup.cfg
```

### Comparing `cellfinder-1.3.0rc0/.github/workflows/test_and_deploy.yml` & `cellfinder-1.3.0rc1/.github/workflows/test_and_deploy.yml`

 * *Files 2% similar despite different names*

```diff
@@ -44,19 +44,19 @@
       matrix:
         # Run all supported Python versions on linux
         os: [ubuntu-latest]
         python-version: ["3.9", "3.10", "3.11"]
         # Include one windows and two macOS (intel based and arm based) runs
         include:
           - os: macos-13
-            python-version: "3.10"
+            python-version: "3.11"
           - os: macos-latest
-            python-version: "3.10"
+            python-version: "3.11"
           - os: windows-latest
-            python-version: "3.10"
+            python-version: "3.11"
 
     steps:
       - name: Cache brainglobe directory
         uses: actions/cache@v3
         with:
           path: | # ensure we don't cache any interrupted atlas download and extraction, if e.g. we cancel the workflow manually
             ~/.brainglobe
@@ -94,15 +94,15 @@
       - name: Setup qtpy libraries
         uses: tlambert03/setup-qt-libs@v1
       # Setup VTK with headless display
       - uses: pyvista/setup-headless-display-action@v2
       # Run test suite with numba disabled
       - uses: neuroinformatics-unit/actions/test@v2
         with:
-          python-version: "3.10"
+          python-version: "3.11"
           secret-codecov-token: ${{ secrets.CODECOV_TOKEN }}
           codecov-flags: "numba"
 
   # Run brainglobe-workflows brainmapper-CLI tests to check for
   # breakages
   test_brainmapper_cli:
     needs: [linting, manifest]
@@ -121,18 +121,18 @@
             !~/.brainglobe/atlas.tar.gz
           key: brainglobe
       - name: Checkout brainglobe-workflows
         uses: actions/checkout@v3
         with:
           repository: 'brainglobe/brainglobe-workflows'
 
-      - name: Set up Python 3.10
+      - name: Set up Python 3.11
         uses: actions/setup-python@v3
         with:
-          python-version: "3.10"
+          python-version: "3.11"
 
       - name: Install test dependencies
         run: |
           python -m pip install --upgrade pip wheel
           # Install cellfinder from the latest SHA on this branch
           python -m pip install "cellfinder @ git+$GITHUB_SERVER_URL/$GITHUB_REPOSITORY@$GITHUB_SHA"
```

### Comparing `cellfinder-1.3.0rc0/.github/workflows/test_include_guard.yaml` & `cellfinder-1.3.0rc1/.github/workflows/test_include_guard.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     steps:
       - name: Check out repository
         uses: actions/checkout@v3
 
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
-          python-version: '3.10'
+          python-version: '3.11'
 
       - name: Install cellfinder via pip
         run: python -m pip install -e "."
 
       - name: Test (working) import
         uses: jannekem/run-python-script-action@v1
         env:
```

### Comparing `cellfinder-1.3.0rc0/.gitignore` & `cellfinder-1.3.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/CITATION.cff` & `cellfinder-1.3.0rc1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/LICENSE` & `cellfinder-1.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/PKG-INFO` & `cellfinder-1.3.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellfinder
-Version: 1.3.0rc0
+Version: 1.3.0rc1
 Summary: Automated 3D cell detection in large microscopy images
 Author-email: "Adam Tyson, Christian Niedworok, Charly Rousseau" <code@adamltyson.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://brainglobe.info/documentation/cellfinder/index.html
 Project-URL: Source Code, https://github.com/brainglobe/cellfinder
 Project-URL: Bug Tracker, https://github.com/brainglobe/cellfinder/issues
 Project-URL: Documentation, https://brainglobe.info/documentation/cellfinder/index.html
@@ -14,14 +14,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: brainglobe-utils>=0.5.0
 Requires-Dist: brainglobe-napari-io>=0.3.4
 Requires-Dist: dask[array]
```

### Comparing `cellfinder-1.3.0rc0/README.md` & `cellfinder-1.3.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/__init__.py` & `cellfinder-1.3.0rc1/cellfinder/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,11 +23,10 @@
         f"https://github.com/brainglobe/brainglobe-meta#readme."
     ) from e
 
 
 # Set the Keras backend to torch
 os.environ["KERAS_BACKEND"] = "torch"
 
-__author__ = "Adam Tyson, Christian Niedworok, Charly Rousseau"
 __license__ = "BSD-3-Clause"
 
 DEFAULT_CELLFINDER_DIRECTORY = Path.home() / ".brainglobe" / "cellfinder"
```

### Comparing `cellfinder-1.3.0rc0/cellfinder/cli_migration_warning.py` & `cellfinder-1.3.0rc1/cellfinder/cli_migration_warning.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/core/classify/augment.py` & `cellfinder-1.3.0rc1/cellfinder/core/classify/augment.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/core/classify/classify.py` & `cellfinder-1.3.0rc1/cellfinder/core/classify/classify.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/core/classify/cube_generator.py` & `cellfinder-1.3.0rc1/cellfinder/core/classify/cube_generator.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/core/classify/resnet.py` & `cellfinder-1.3.0rc1/cellfinder/core/classify/resnet.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/core/classify/tools.py` & `cellfinder-1.3.0rc1/cellfinder/core/classify/tools.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/core/detect/detect.py` & `cellfinder-1.3.0rc1/cellfinder/core/detect/detect.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/__pycache__/classical_filter.cpython-312.pyc` & `cellfinder-1.3.0rc1/cellfinder/core/detect/filters/plane/classical_filter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,115 +1,84 @@
-00000000: cb0d 0d0a 0000 0000 5d31 3a66 3305 0000  ........]1:f3...
-00000010: e300 0000 0000 0000 0000 0000 0009 0000  ................
-00000020: 0000 0000 00f3 6c00 0000 9700 6400 6401  ......l.....d.d.
-00000030: 6c00 5a01 6400 6402 6c02 6d03 5a03 6d04  l.Z.d.d.l.m.Z.m.
-00000040: 5a04 0100 6400 6403 6c05 6d06 5a06 0100  Z...d.d.l.m.Z...
-00000050: 0900 6409 6404 6501 6a0e 0000 0000 0000  ..d.d.e.j.......
-00000060: 0000 0000 0000 0000 0000 0000 6405 6508  ............d.e.
-00000070: 6406 6508 6407 6501 6a0e 0000 0000 0000  d.e.d.e.j.......
-00000080: 0000 0000 0000 0000 0000 0000 6608 6408  ............f.d.
-00000090: 8405 5a09 7901 290a e900 0000 004e 2902  ..Z.y.)......N).
-000000a0: da0f 6761 7573 7369 616e 5f66 696c 7465  ..gaussian_filte
-000000b0: 72da 076c 6170 6c61 6365 2901 da09 6d65  r..laplace)...me
-000000c0: 6466 696c 7432 64da 0369 6d67 da0e 636c  dfilt2d..img..cl
-000000d0: 6970 7069 6e67 5f76 616c 7565 da0e 6761  ipping_value..ga
-000000e0: 7573 7369 616e 5f73 6967 6d61 da06 7265  ussian_sigma..re
-000000f0: 7475 726e 6303 0000 0000 0000 0000 0000  turnc...........
-00000100: 0005 0000 0003 0000 00f3 1a01 0000 9700  ................
-00000110: 7c00 6a00 0000 0000 0000 0000 0000 0000  |.j.............
-00000120: 0000 0000 0000 7d03 7403 0000 0000 0000  ......}.t.......
-00000130: 0000 7c00 6a05 0000 0000 0000 0000 0000  ..|.j...........
-00000140: 0000 0000 0000 0000 7406 0000 0000 0000  ........t.......
-00000150: 0000 6a08 0000 0000 0000 0000 0000 0000  ..j.............
-00000160: 0000 0000 0000 ab01 0000 0000 0000 ab01  ................
-00000170: 0000 0000 0000 7d04 740b 0000 0000 0000  ......}.t.......
-00000180: 0000 7c04 7c02 ab02 0000 0000 0000 7d04  ..|.|.........}.
-00000190: 740d 0000 0000 0000 0000 7c04 ab01 0000  t.........|.....
-000001a0: 0000 0000 7d04 7c04 6401 7a12 0000 7d04  ....}.|.d.z...}.
-000001b0: 7c04 7c04 6a0f 0000 0000 0000 0000 0000  |.|.j...........
-000001c0: 0000 0000 0000 0000 ab00 0000 0000 0000  ................
-000001d0: 7a17 0000 7d04 7c04 7c04 6a11 0000 0000  z...}.|.|.j.....
-000001e0: 0000 0000 0000 0000 0000 0000 0000 ab00  ................
-000001f0: 0000 0000 0000 7a18 0000 7d04 7c04 7c01  ......z...}.|.|.
-00000200: 7a12 0000 7d04 7c04 6a05 0000 0000 0000  z...}.|.j.......
-00000210: 0000 0000 0000 0000 0000 0000 7c03 ab01  ............|...
-00000220: 0000 0000 0000 5300 2902 61b6 0200 000a  ......S.).a.....
-00000230: 2020 2020 456e 6861 6e63 6573 2074 6865      Enhances the
-00000240: 2070 6561 6b73 2028 6272 6967 6874 2070   peaks (bright p
-00000250: 6978 656c 7329 2069 6e20 616e 2069 6e70  ixels) in an inp
-00000260: 7574 2069 6d61 6765 2e0a 0a20 2020 2050  ut image...    P
-00000270: 6172 616d 6574 6572 733a 0a20 2020 202d  arameters:.    -
-00000280: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 696d  ---------.    im
-00000290: 6720 3a20 6e70 2e6e 6461 7272 6179 0a20  g : np.ndarray. 
-000002a0: 2020 2020 2020 2049 6e70 7574 2069 6d61         Input ima
-000002b0: 6765 2e0a 2020 2020 636c 6970 7069 6e67  ge..    clipping
-000002c0: 5f76 616c 7565 203a 2066 6c6f 6174 0a20  _value : float. 
-000002d0: 2020 2020 2020 204d 6178 696d 756d 2076         Maximum v
-000002e0: 616c 7565 2066 6f72 2074 6865 2065 6e68  alue for the enh
-000002f0: 616e 6365 6420 696d 6167 652e 0a20 2020  anced image..   
-00000300: 2067 6175 7373 6961 6e5f 7369 676d 6120   gaussian_sigma 
-00000310: 3a20 666c 6f61 742c 206f 7074 696f 6e61  : float, optiona
-00000320: 6c0a 2020 2020 2020 2020 5374 616e 6461  l.        Standa
-00000330: 7264 2064 6576 6961 7469 6f6e 2066 6f72  rd deviation for
-00000340: 2074 6865 2047 6175 7373 6961 6e20 6669   the Gaussian fi
-00000350: 6c74 6572 2e20 4465 6661 756c 7420 6973  lter. Default is
-00000360: 2032 2e35 2e0a 0a20 2020 2052 6574 7572   2.5...    Retur
-00000370: 6e73 3a0a 2020 2020 2d2d 2d2d 2d2d 2d0a  ns:.    -------.
-00000380: 2020 2020 6e70 2e6e 6461 7272 6179 0a20      np.ndarray. 
-00000390: 2020 2020 2020 2045 6e68 616e 6365 6420         Enhanced 
-000003a0: 696d 6167 6520 7769 7468 2070 6561 6b73  image with peaks
-000003b0: 2e0a 0a20 2020 204e 6f74 6573 3a0a 2020  ...    Notes:.  
-000003c0: 2020 2d2d 2d2d 2d2d 0a20 2020 2054 6865    ------.    The
-000003d0: 2065 6e68 616e 6365 6d65 6e74 2070 726f   enhancement pro
-000003e0: 6365 7373 2069 6e63 6c75 6465 7320 7468  cess includes th
-000003f0: 6520 666f 6c6c 6f77 696e 6720 7374 6570  e following step
-00000400: 733a 0a20 2020 2031 2e20 4170 706c 7969  s:.    1. Applyi
-00000410: 6e67 2061 2032 4420 6d65 6469 616e 2066  ng a 2D median f
-00000420: 696c 7465 722e 0a20 2020 2032 2e20 4170  ilter..    2. Ap
-00000430: 706c 7969 6e67 2061 204c 6170 6c61 6369  plying a Laplaci
-00000440: 616e 206f 6620 4761 7573 7369 616e 2066  an of Gaussian f
-00000450: 696c 7465 7220 284c 6f47 292e 0a20 2020  ilter (LoG)..   
-00000460: 2033 2e20 4d75 6c74 6970 6c79 696e 6720   3. Multiplying 
-00000470: 6279 202d 3120 2862 7269 6768 7420 7370  by -1 (bright sp
-00000480: 6f74 7320 7265 7370 6f6e 6420 6e65 6761  ots respond nega
-00000490: 7469 7665 2069 6e20 6120 4c6f 4729 2e0a  tive in a LoG)..
-000004a0: 2020 2020 342e 2052 6573 6361 6c69 6e67      4. Rescaling
-000004b0: 2069 6d61 6765 2076 616c 7565 7320 746f   image values to
-000004c0: 2072 616e 6765 2066 726f 6d20 3020 746f   range from 0 to
-000004d0: 2063 6c69 7070 696e 6720 7661 6c75 652e   clipping value.
-000004e0: 0a20 2020 20e9 ffff ffff 2909 da05 6474  .    .....)...dt
-000004f0: 7970 6572 0500 0000 da06 6173 7479 7065  yper......astype
-00000500: da02 6e70 da07 666c 6f61 7436 3472 0300  ..np..float64r..
-00000510: 0000 7204 0000 00da 036d 696e da03 6d61  ..r......min..ma
-00000520: 7829 0572 0600 0000 7207 0000 0072 0800  x).r....r....r..
-00000530: 0000 da07 7479 7065 5f69 6eda 0c66 696c  ....type_in..fil
-00000540: 7465 7265 645f 696d 6773 0500 0000 2020  tered_imgs....  
-00000550: 2020 20fa 622f 686f 6d65 2f61 6461 6d2f     .b/home/adam/
-00000560: 7072 6f6a 6563 7473 2f62 7261 696e 676c  projects/braingl
-00000570: 6f62 652f 6365 6c6c 6669 6e64 6572 2f63  obe/cellfinder/c
-00000580: 656c 6c66 696e 6465 722f 636f 7265 2f64  ellfinder/core/d
-00000590: 6574 6563 742f 6669 6c74 6572 732f 706c  etect/filters/pl
-000005a0: 616e 652f 636c 6173 7369 6361 6c5f 6669  ane/classical_fi
-000005b0: 6c74 6572 2e70 79da 0d65 6e68 616e 6365  lter.py..enhance
-000005c0: 5f70 6561 6b73 7215 0000 0006 0000 0073  _peaksr........s
-000005d0: 8700 0000 8000 f038 000f 128f 6989 6980  .......8....i.i.
-000005e0: 47dc 131c 9853 9f5a 995a ac02 af0a a90a  G....S.Z.Z......
-000005f0: d31d 33d3 1334 804c dc13 22a0 3cb0 1ed3  ..3..4.L..".<...
-00000600: 1340 804c dc13 1a98 3cd3 1328 804c d804  .@.L....<..(.L..
-00000610: 1090 42d1 0416 804c e004 1090 4cd7 1424  ..B....L....L..$
-00000620: d114 24d3 1426 d104 2680 4cd8 0410 904c  ..$..&..&.L....L
-00000630: d714 24d1 1424 d314 26d1 0426 804c f006  ..$..$..&..&.L..
-00000640: 0005 1190 4ed1 0422 804c d80b 17d7 0b1e  ....N..".L......
-00000650: d10b 1e98 77d3 0b27 d004 27f3 0000 0000  ....w..'..'.....
-00000660: 2901 6700 0000 0000 0004 4029 0ada 056e  ).g.......@)...n
-00000670: 756d 7079 720e 0000 00da 0d73 6369 7079  umpyr......scipy
-00000680: 2e6e 6469 6d61 6765 7203 0000 0072 0400  .ndimager....r..
-00000690: 0000 da0c 7363 6970 792e 7369 676e 616c  ....scipy.signal
-000006a0: 7205 0000 00da 076e 6461 7272 6179 da05  r......ndarray..
-000006b0: 666c 6f61 7472 1500 0000 a900 7216 0000  floatr......r...
-000006c0: 0072 1400 0000 fa08 3c6d 6f64 756c 653e  .r......<module>
-000006d0: 721d 0000 0001 0000 0073 4200 0000 f003  r........sB.....
-000006e0: 0101 01db 0012 df00 32dd 0022 f008 0045  ........2.."...E
-000006f0: 0148 01f1 0327 0128 d809 0b8f 1a89 1af0  .H...'.(........
-00000700: 0327 0128 d825 2af0 0327 0128 d83c 41f0  .'.(.%*..'.(.<A.
-00000710: 0327 0128 e005 0787 5a81 5af4 0527 0128  .'.(....Z.Z..'.(
-00000720: 7216 0000 00                             r....
+00000000: 696d 706f 7274 206e 756d 7079 2061 7320  import numpy as 
+00000010: 6e70 0a66 726f 6d20 7363 6970 792e 6e64  np.from scipy.nd
+00000020: 696d 6167 6520 696d 706f 7274 2067 6175  image import gau
+00000030: 7373 6961 6e5f 6669 6c74 6572 2c20 6c61  ssian_filter, la
+00000040: 706c 6163 650a 6672 6f6d 2073 6369 7079  place.from scipy
+00000050: 2e73 6967 6e61 6c20 696d 706f 7274 206d  .signal import m
+00000060: 6564 6669 6c74 3264 0a0a 0a64 6566 2065  edfilt2d...def e
+00000070: 6e68 616e 6365 5f70 6561 6b73 280a 2020  nhance_peaks(.  
+00000080: 2020 696d 673a 206e 702e 6e64 6172 7261    img: np.ndarra
+00000090: 792c 2063 6c69 7070 696e 675f 7661 6c75  y, clipping_valu
+000000a0: 653a 2066 6c6f 6174 2c20 6761 7573 7369  e: float, gaussi
+000000b0: 616e 5f73 6967 6d61 3a20 666c 6f61 7420  an_sigma: float 
+000000c0: 3d20 322e 350a 2920 2d3e 206e 702e 6e64  = 2.5.) -> np.nd
+000000d0: 6172 7261 793a 0a20 2020 2022 2222 0a20  array:.    """. 
+000000e0: 2020 2045 6e68 616e 6365 7320 7468 6520     Enhances the 
+000000f0: 7065 616b 7320 2862 7269 6768 7420 7069  peaks (bright pi
+00000100: 7865 6c73 2920 696e 2061 6e20 696e 7075  xels) in an inpu
+00000110: 7420 696d 6167 652e 0a0a 2020 2020 5061  t image...    Pa
+00000120: 7261 6d65 7465 7273 3a0a 2020 2020 2d2d  rameters:.    --
+00000130: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2069 6d67  --------.    img
+00000140: 203a 206e 702e 6e64 6172 7261 790a 2020   : np.ndarray.  
+00000150: 2020 2020 2020 496e 7075 7420 696d 6167        Input imag
+00000160: 652e 0a20 2020 2063 6c69 7070 696e 675f  e..    clipping_
+00000170: 7661 6c75 6520 3a20 666c 6f61 740a 2020  value : float.  
+00000180: 2020 2020 2020 4d61 7869 6d75 6d20 7661        Maximum va
+00000190: 6c75 6520 666f 7220 7468 6520 656e 6861  lue for the enha
+000001a0: 6e63 6564 2069 6d61 6765 2e0a 2020 2020  nced image..    
+000001b0: 6761 7573 7369 616e 5f73 6967 6d61 203a  gaussian_sigma :
+000001c0: 2066 6c6f 6174 2c20 6f70 7469 6f6e 616c   float, optional
+000001d0: 0a20 2020 2020 2020 2053 7461 6e64 6172  .        Standar
+000001e0: 6420 6465 7669 6174 696f 6e20 666f 7220  d deviation for 
+000001f0: 7468 6520 4761 7573 7369 616e 2066 696c  the Gaussian fil
+00000200: 7465 722e 2044 6566 6175 6c74 2069 7320  ter. Default is 
+00000210: 322e 352e 0a0a 2020 2020 5265 7475 726e  2.5...    Return
+00000220: 733a 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  s:.    -------. 
+00000230: 2020 206e 702e 6e64 6172 7261 790a 2020     np.ndarray.  
+00000240: 2020 2020 2020 456e 6861 6e63 6564 2069        Enhanced i
+00000250: 6d61 6765 2077 6974 6820 7065 616b 732e  mage with peaks.
+00000260: 0a0a 2020 2020 4e6f 7465 733a 0a20 2020  ..    Notes:.   
+00000270: 202d 2d2d 2d2d 2d0a 2020 2020 5468 6520   ------.    The 
+00000280: 656e 6861 6e63 656d 656e 7420 7072 6f63  enhancement proc
+00000290: 6573 7320 696e 636c 7564 6573 2074 6865  ess includes the
+000002a0: 2066 6f6c 6c6f 7769 6e67 2073 7465 7073   following steps
+000002b0: 3a0a 2020 2020 312e 2041 7070 6c79 696e  :.    1. Applyin
+000002c0: 6720 6120 3244 206d 6564 6961 6e20 6669  g a 2D median fi
+000002d0: 6c74 6572 2e0a 2020 2020 322e 2041 7070  lter..    2. App
+000002e0: 6c79 696e 6720 6120 4c61 706c 6163 6961  lying a Laplacia
+000002f0: 6e20 6f66 2047 6175 7373 6961 6e20 6669  n of Gaussian fi
+00000300: 6c74 6572 2028 4c6f 4729 2e0a 2020 2020  lter (LoG)..    
+00000310: 332e 204d 756c 7469 706c 7969 6e67 2062  3. Multiplying b
+00000320: 7920 2d31 2028 6272 6967 6874 2073 706f  y -1 (bright spo
+00000330: 7473 2072 6573 706f 6e64 206e 6567 6174  ts respond negat
+00000340: 6976 6520 696e 2061 204c 6f47 292e 0a20  ive in a LoG).. 
+00000350: 2020 2034 2e20 5265 7363 616c 696e 6720     4. Rescaling 
+00000360: 696d 6167 6520 7661 6c75 6573 2074 6f20  image values to 
+00000370: 7261 6e67 6520 6672 6f6d 2030 2074 6f20  range from 0 to 
+00000380: 636c 6970 7069 6e67 2076 616c 7565 2e0a  clipping value..
+00000390: 2020 2020 2222 220a 2020 2020 7479 7065      """.    type
+000003a0: 5f69 6e20 3d20 696d 672e 6474 7970 650a  _in = img.dtype.
+000003b0: 2020 2020 6669 6c74 6572 6564 5f69 6d67      filtered_img
+000003c0: 203d 206d 6564 6669 6c74 3264 2869 6d67   = medfilt2d(img
+000003d0: 2e61 7374 7970 6528 6e70 2e66 6c6f 6174  .astype(np.float
+000003e0: 3634 2929 0a20 2020 2066 696c 7465 7265  64)).    filtere
+000003f0: 645f 696d 6720 3d20 6761 7573 7369 616e  d_img = gaussian
+00000400: 5f66 696c 7465 7228 6669 6c74 6572 6564  _filter(filtered
+00000410: 5f69 6d67 2c20 6761 7573 7369 616e 5f73  _img, gaussian_s
+00000420: 6967 6d61 290a 2020 2020 6669 6c74 6572  igma).    filter
+00000430: 6564 5f69 6d67 203d 206c 6170 6c61 6365  ed_img = laplace
+00000440: 2866 696c 7465 7265 645f 696d 6729 0a20  (filtered_img). 
+00000450: 2020 2066 696c 7465 7265 645f 696d 6720     filtered_img 
+00000460: 2a3d 202d 310a 0a20 2020 2066 696c 7465  *= -1..    filte
+00000470: 7265 645f 696d 6720 2d3d 2066 696c 7465  red_img -= filte
+00000480: 7265 645f 696d 672e 6d69 6e28 290a 2020  red_img.min().  
+00000490: 2020 6669 6c74 6572 6564 5f69 6d67 202f    filtered_img /
+000004a0: 3d20 6669 6c74 6572 6564 5f69 6d67 2e6d  = filtered_img.m
+000004b0: 6178 2829 0a0a 2020 2020 2320 546f 206c  ax()..    # To l
+000004c0: 6561 7665 2072 6f6f 6d20 746f 206c 6162  eave room to lab
+000004d0: 656c 2069 6e20 7468 6520 3364 2064 6574  el in the 3d det
+000004e0: 6563 7469 6f6e 2e0a 2020 2020 6669 6c74  ection..    filt
+000004f0: 6572 6564 5f69 6d67 202a 3d20 636c 6970  ered_img *= clip
+00000500: 7069 6e67 5f76 616c 7565 0a20 2020 2072  ping_value.    r
+00000510: 6574 7572 6e20 6669 6c74 6572 6564 5f69  eturn filtered_i
+00000520: 6d67 2e61 7374 7970 6528 7479 7065 5f69  mg.astype(type_i
+00000530: 6e29 0a                                  n).
```

### Comparing `cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/plane_filter.py` & `cellfinder-1.3.0rc1/cellfinder/core/detect/filters/plane/plane_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/core/detect/filters/plane/tile_walker.py` & `cellfinder-1.3.0rc1/cellfinder/core/detect/filters/plane/tile_walker.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/core/detect/filters/setup_filters.py` & `cellfinder-1.3.0rc1/cellfinder/core/detect/filters/setup_filters.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/ball_filter.py` & `cellfinder-1.3.0rc1/cellfinder/core/detect/filters/volume/ball_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/structure_detection.py` & `cellfinder-1.3.0rc1/cellfinder/core/detect/filters/volume/structure_detection.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/structure_splitting.py` & `cellfinder-1.3.0rc1/cellfinder/core/detect/filters/volume/structure_splitting.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/core/detect/filters/volume/volume_filter.py` & `cellfinder-1.3.0rc1/cellfinder/core/detect/filters/volume/volume_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/core/download/cli.py` & `cellfinder-1.3.0rc1/cellfinder/core/download/cli.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/core/download/download.py` & `cellfinder-1.3.0rc1/cellfinder/core/download/download.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/core/main.py` & `cellfinder-1.3.0rc1/cellfinder/core/main.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/core/tools/__pycache__/source_files.cpython-311.pyc` & `cellfinder-1.3.0rc1/cellfinder/core/tools/source_files.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,84 +1,54 @@
-00000000: a70d 0d0a 0000 0000 bda8 3c66 5803 0000  ..........<fX...
-00000010: e300 0000 0000 0000 0000 0000 0002 0000  ................
-00000020: 0000 0000 00f3 2a00 0000 9700 6400 6401  ......*.....d.d.
-00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 6d03  l.m.Z...d.d.l.m.
-00000040: 5a03 0100 6403 8400 5a04 6404 8400 5a05  Z...d...Z.d...Z.
-00000050: 6405 5300 2906 e900 0000 0029 01da 0450  d.S.)......)...P
-00000060: 6174 68a9 01da 1c44 4546 4155 4c54 5f43  ath....DEFAULT_C
-00000070: 454c 4c46 494e 4445 525f 4449 5245 4354  ELLFINDER_DIRECT
-00000080: 4f52 5963 0000 0000 0000 0000 0000 0000  ORYc............
-00000090: 0300 0000 0300 0000 f34a 0000 0097 0074  .........J.....t
-000000a0: 0100 0000 0000 0000 0000 0074 0200 0000  ...........t....
-000000b0: 0000 0000 0000 00a6 0100 00ab 0100 0000  ................
-000000c0: 0000 0000 006a 0200 0000 0000 0000 006a  .....j.........j
-000000d0: 0200 0000 0000 0000 0064 017a 0b00 0064  .........d.z...d
-000000e0: 027a 0b00 0053 0029 037a 7c0a 2020 2020  .z...S.).z|.    
-000000f0: 5265 7475 726e 7320 7468 6520 6465 6661  Returns the defa
-00000100: 756c 7420 636f 6e66 6967 7572 6174 696f  ult configuratio
-00000110: 6e20 7061 7468 2066 6f72 2063 656c 6c66  n path for cellf
-00000120: 696e 6465 722e 0a0a 2020 2020 5265 7475  inder...    Retu
-00000130: 726e 733a 0a20 2020 2020 2020 2050 6174  rns:.        Pat
-00000140: 683a 2054 6865 2064 6566 6175 6c74 2063  h: The default c
-00000150: 6f6e 6669 6775 7261 7469 6f6e 2070 6174  onfiguration pat
-00000160: 682e 0a20 2020 20da 0663 6f6e 6669 677a  h..    ..configz
-00000170: 0f63 656c 6c66 696e 6465 722e 636f 6e66  .cellfinder.conf
-00000180: 2903 7203 0000 00da 085f 5f66 696c 655f  ).r......__file_
-00000190: 5fda 0670 6172 656e 74a9 00f3 0000 0000  _..parent.......
-000001a0: fa4f 2f68 6f6d 652f 6164 616d 2f70 726f  .O/home/adam/pro
-000001b0: 6a65 6374 732f 6272 6169 6e67 6c6f 6265  jects/brainglobe
-000001c0: 2f63 656c 6c66 696e 6465 722f 6365 6c6c  /cellfinder/cell
-000001d0: 6669 6e64 6572 2f63 6f72 652f 746f 6f6c  finder/core/tool
-000001e0: 732f 736f 7572 6365 5f66 696c 6573 2e70  s/source_files.p
-000001f0: 79da 1a64 6566 6175 6c74 5f63 6f6e 6669  y..default_confi
-00000200: 6775 7261 7469 6f6e 5f70 6174 6872 0d00  guration_pathr..
-00000210: 0000 0600 0000 7321 0000 0080 00f5 0e00  ......s!........
-00000220: 0c10 9508 893e 8c3e d40b 20d4 0b27 a828  .....>.>.. ..'.(
-00000230: d10b 32d0 3546 d10b 46d0 0446 720b 0000  ..2.5F..F..Fr...
-00000240: 0063 0000 0000 0000 0000 0000 0000 0200  .c..............
-00000250: 0000 0300 0000 f316 0000 0097 0074 0000  .............t..
-00000260: 0000 0000 0000 0000 0064 017a 0b00 0053  .........d.z...S
-00000270: 0029 0261 a001 0000 0a20 2020 2052 6574  .).a.....    Ret
-00000280: 7572 6e73 2074 6865 2070 6174 6820 746f  urns the path to
-00000290: 2074 6865 2075 7365 722d 7370 6563 6966   the user-specif
-000002a0: 6963 2063 6f6e 6669 6775 7261 7469 6f6e  ic configuration
-000002b0: 2066 696c 6520 666f 7220 6365 6c6c 6669   file for cellfi
-000002c0: 6e64 6572 2e0a 0a20 2020 2054 6869 7320  nder...    This 
-000002d0: 6675 6e63 7469 6f6e 2072 6574 7572 6e73  function returns
-000002e0: 2074 6865 2070 6174 6820 746f 2074 6865   the path to the
-000002f0: 2075 7365 722d 7370 6563 6966 6963 2063   user-specific c
-00000300: 6f6e 6669 6775 7261 7469 6f6e 2066 696c  onfiguration fil
-00000310: 650a 2020 2020 666f 7220 6365 6c6c 6669  e.    for cellfi
-00000320: 6e64 6572 2e20 5468 6520 7573 6572 2d73  nder. The user-s
-00000330: 7065 6369 6669 6320 636f 6e66 6967 7572  pecific configur
-00000340: 6174 696f 6e20 6669 6c65 2069 7320 6c6f  ation file is lo
-00000350: 6361 7465 6420 696e 2074 6865 0a20 2020  cated in the.   
-00000360: 2075 7365 7227 7320 686f 6d65 2064 6972   user's home dir
-00000370: 6563 746f 7279 2075 6e64 6572 2074 6865  ectory under the
-00000380: 2022 2e62 7261 696e 676c 6f62 652f 6365   ".brainglobe/ce
-00000390: 6c6c 6669 6e64 6572 2220 666f 6c64 6572  llfinder" folder
-000003a0: 0a20 2020 2061 6e64 2069 7320 6e61 6d65  .    and is name
-000003b0: 6420 2263 656c 6c66 696e 6465 722e 636f  d "cellfinder.co
-000003c0: 6e66 2e63 7573 746f 6d22 2e0a 0a20 2020  nf.custom"...   
-000003d0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-000003e0: 2020 5061 7468 3a20 5468 6520 7061 7468    Path: The path
-000003f0: 2074 6f20 7468 6520 6375 7374 6f6d 2063   to the custom c
-00000400: 6f6e 6669 6775 7261 7469 6f6e 2066 696c  onfiguration fil
-00000410: 652e 0a0a 2020 2020 7a16 6365 6c6c 6669  e...    z.cellfi
-00000420: 6e64 6572 2e63 6f6e 662e 6375 7374 6f6d  nder.conf.custom
-00000430: 7204 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
-00000440: 0c00 0000 da20 7573 6572 5f73 7065 6369  ..... user_speci
-00000450: 6669 635f 636f 6e66 6967 7572 6174 696f  fic_configuratio
-00000460: 6e5f 7061 7468 720f 0000 0010 0000 0073  n_pathr........s
-00000470: 1000 0000 8000 f51a 000c 28d0 2a42 d10b  ..........(.*B..
-00000480: 42d0 0442 720b 0000 004e 2906 da07 7061  B..Br....N)...pa
-00000490: 7468 6c69 6272 0300 0000 da0a 6365 6c6c  thlibr......cell
-000004a0: 6669 6e64 6572 7205 0000 0072 0d00 0000  finderr....r....
-000004b0: 720f 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
-000004c0: 0c00 0000 fa08 3c6d 6f64 756c 653e 7212  ......<module>r.
-000004d0: 0000 0001 0000 0073 5900 0000 f003 0101  .......sY.......
-000004e0: 01d8 0018 d000 18d0 0018 d000 18d0 0018  ................
-000004f0: d000 18e0 0033 d000 33d0 0033 d000 33d0  .....3..3..3..3.
-00000500: 0033 d000 33f0 0607 0147 01f0 0007 0147  .3..3....G.....G
-00000510: 01f0 0007 0147 01f0 140d 0143 01f0 000d  .....G.....C....
-00000520: 0143 01f0 000d 0143 01f0 000d 0143 01f0  .C.....C.....C..
-00000530: 000d 0143 0172 0b00 0000                 ...C.r....
+00000000: 6672 6f6d 2070 6174 686c 6962 2069 6d70  from pathlib imp
+00000010: 6f72 7420 5061 7468 0a0a 6672 6f6d 2063  ort Path..from c
+00000020: 656c 6c66 696e 6465 7220 696d 706f 7274  ellfinder import
+00000030: 2044 4546 4155 4c54 5f43 454c 4c46 494e   DEFAULT_CELLFIN
+00000040: 4445 525f 4449 5245 4354 4f52 590a 0a0a  DER_DIRECTORY...
+00000050: 6465 6620 6465 6661 756c 745f 636f 6e66  def default_conf
+00000060: 6967 7572 6174 696f 6e5f 7061 7468 2829  iguration_path()
+00000070: 3a0a 2020 2020 2222 220a 2020 2020 5265  :.    """.    Re
+00000080: 7475 726e 7320 7468 6520 6465 6661 756c  turns the defaul
+00000090: 7420 636f 6e66 6967 7572 6174 696f 6e20  t configuration 
+000000a0: 7061 7468 2066 6f72 2063 656c 6c66 696e  path for cellfin
+000000b0: 6465 722e 0a0a 2020 2020 5265 7475 726e  der...    Return
+000000c0: 733a 0a20 2020 2020 2020 2050 6174 683a  s:.        Path:
+000000d0: 2054 6865 2064 6566 6175 6c74 2063 6f6e   The default con
+000000e0: 6669 6775 7261 7469 6f6e 2070 6174 682e  figuration path.
+000000f0: 0a20 2020 2022 2222 0a20 2020 2072 6574  .    """.    ret
+00000100: 7572 6e20 5061 7468 285f 5f66 696c 655f  urn Path(__file_
+00000110: 5f29 2e70 6172 656e 742e 7061 7265 6e74  _).parent.parent
+00000120: 202f 2022 636f 6e66 6967 2220 2f20 2263   / "config" / "c
+00000130: 656c 6c66 696e 6465 722e 636f 6e66 220a  ellfinder.conf".
+00000140: 0a0a 6465 6620 7573 6572 5f73 7065 6369  ..def user_speci
+00000150: 6669 635f 636f 6e66 6967 7572 6174 696f  fic_configuratio
+00000160: 6e5f 7061 7468 2829 3a0a 2020 2020 2222  n_path():.    ""
+00000170: 220a 2020 2020 5265 7475 726e 7320 7468  ".    Returns th
+00000180: 6520 7061 7468 2074 6f20 7468 6520 7573  e path to the us
+00000190: 6572 2d73 7065 6369 6669 6320 636f 6e66  er-specific conf
+000001a0: 6967 7572 6174 696f 6e20 6669 6c65 2066  iguration file f
+000001b0: 6f72 2063 656c 6c66 696e 6465 722e 0a0a  or cellfinder...
+000001c0: 2020 2020 5468 6973 2066 756e 6374 696f      This functio
+000001d0: 6e20 7265 7475 726e 7320 7468 6520 7061  n returns the pa
+000001e0: 7468 2074 6f20 7468 6520 7573 6572 2d73  th to the user-s
+000001f0: 7065 6369 6669 6320 636f 6e66 6967 7572  pecific configur
+00000200: 6174 696f 6e20 6669 6c65 0a20 2020 2066  ation file.    f
+00000210: 6f72 2063 656c 6c66 696e 6465 722e 2054  or cellfinder. T
+00000220: 6865 2075 7365 722d 7370 6563 6966 6963  he user-specific
+00000230: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
+00000240: 696c 6520 6973 206c 6f63 6174 6564 2069  ile is located i
+00000250: 6e20 7468 650a 2020 2020 7573 6572 2773  n the.    user's
+00000260: 2068 6f6d 6520 6469 7265 6374 6f72 7920   home directory 
+00000270: 756e 6465 7220 7468 6520 222e 6272 6169  under the ".brai
+00000280: 6e67 6c6f 6265 2f63 656c 6c66 696e 6465  nglobe/cellfinde
+00000290: 7222 2066 6f6c 6465 720a 2020 2020 616e  r" folder.    an
+000002a0: 6420 6973 206e 616d 6564 2022 6365 6c6c  d is named "cell
+000002b0: 6669 6e64 6572 2e63 6f6e 662e 6375 7374  finder.conf.cust
+000002c0: 6f6d 222e 0a0a 2020 2020 5265 7475 726e  om"...    Return
+000002d0: 733a 0a20 2020 2020 2020 2050 6174 683a  s:.        Path:
+000002e0: 2054 6865 2070 6174 6820 746f 2074 6865   The path to the
+000002f0: 2063 7573 746f 6d20 636f 6e66 6967 7572   custom configur
+00000300: 6174 696f 6e20 6669 6c65 2e0a 0a20 2020  ation file...   
+00000310: 2022 2222 0a20 2020 2072 6574 7572 6e20   """.    return 
+00000320: 4445 4641 554c 545f 4345 4c4c 4649 4e44  DEFAULT_CELLFIND
+00000330: 4552 5f44 4952 4543 544f 5259 202f 2022  ER_DIRECTORY / "
+00000340: 6365 6c6c 6669 6e64 6572 2e63 6f6e 662e  cellfinder.conf.
+00000350: 6375 7374 6f6d 220a                      custom".
```

### Comparing `cellfinder-1.3.0rc0/cellfinder/core/tools/array_operations.py` & `cellfinder-1.3.0rc1/cellfinder/core/tools/array_operations.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/core/tools/geometry.py` & `cellfinder-1.3.0rc1/cellfinder/core/tools/geometry.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/core/tools/image_processing.py` & `cellfinder-1.3.0rc1/cellfinder/core/tools/image_processing.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/core/tools/prep.py` & `cellfinder-1.3.0rc1/cellfinder/core/tools/prep.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/core/tools/system.py` & `cellfinder-1.3.0rc1/cellfinder/core/tools/system.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pathlib import Path
 
+import keras
 from brainglobe_utils.general.exceptions import CommandLineInputError
 
 
 def get_subdirectories(directory, names_only=False):
     """
     Return all subdirectories in a given directory
     :param directory:
@@ -76,7 +77,16 @@
     if unit not in supported_units:
         raise NotImplementedError(
             f"Unit: {unit} is not supported. Please "
             f"use one of {list(supported_units.keys())}"
         )
     else:
         return memory_amount * 10 ** supported_units[unit]
+
+
+def force_cpu():
+    """
+    Forces the CPU to be used, even if a GPU is available
+    """
+    keras.src.backend.common.global_state.set_global_attribute(
+        "torch_device", "cpu"
+    )
```

### Comparing `cellfinder-1.3.0rc0/cellfinder/core/tools/tiff.py` & `cellfinder-1.3.0rc1/cellfinder/core/tools/tiff.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/core/tools/tools.py` & `cellfinder-1.3.0rc1/cellfinder/core/tools/tools.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/core/train/train_yml.py` & `cellfinder-1.3.0rc1/cellfinder/core/train/train_yml.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/napari/curation.py` & `cellfinder-1.3.0rc1/cellfinder/napari/curation.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/napari/detect/detect.py` & `cellfinder-1.3.0rc1/cellfinder/napari/detect/detect.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/napari/detect/detect_containers.py` & `cellfinder-1.3.0rc1/cellfinder/napari/detect/detect_containers.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/napari/detect/thread_worker.py` & `cellfinder-1.3.0rc1/cellfinder/napari/detect/thread_worker.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/napari/input_container.py` & `cellfinder-1.3.0rc1/cellfinder/napari/input_container.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/napari/napari.yaml` & `cellfinder-1.3.0rc1/cellfinder/napari/napari.yaml`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/napari/sample_data.py` & `cellfinder-1.3.0rc1/cellfinder/napari/sample_data.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/napari/train/train.py` & `cellfinder-1.3.0rc1/cellfinder/napari/train/train.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/napari/train/train_containers.py` & `cellfinder-1.3.0rc1/cellfinder/napari/train/train_containers.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder/napari/utils.py` & `cellfinder-1.3.0rc1/cellfinder/napari/utils.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.3.0rc0/cellfinder.egg-info/PKG-INFO` & `cellfinder-1.3.0rc1/cellfinder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellfinder
-Version: 1.3.0rc0
+Version: 1.3.0rc1
 Summary: Automated 3D cell detection in large microscopy images
 Author-email: "Adam Tyson, Christian Niedworok, Charly Rousseau" <code@adamltyson.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://brainglobe.info/documentation/cellfinder/index.html
 Project-URL: Source Code, https://github.com/brainglobe/cellfinder
 Project-URL: Bug Tracker, https://github.com/brainglobe/cellfinder/issues
 Project-URL: Documentation, https://brainglobe.info/documentation/cellfinder/index.html
@@ -14,14 +14,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: brainglobe-utils>=0.5.0
 Requires-Dist: brainglobe-napari-io>=0.3.4
 Requires-Dist: dask[array]
```

### Comparing `cellfinder-1.3.0rc0/pyproject.toml` & `cellfinder-1.3.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: Image Recognition",
 ]
 requires-python = ">=3.9"
 dependencies = [
     "brainglobe-utils>=0.5.0",
     "brainglobe-napari-io>=0.3.4",
     "dask[array]",
```

