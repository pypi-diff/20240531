# Comparing `tmp/ez_zarr-0.1.5.tar.gz` & `tmp/ez_zarr-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez_zarr-0.1.5.tar", last modified: Fri Feb  9 12:55:42 2024, max compression
+gzip compressed data, was "ez_zarr-0.2.0.tar", last modified: Fri May 31 06:39:17 2024, max compression
```

## Comparing `ez_zarr-0.1.5.tar` & `ez_zarr-0.2.0.tar`

### file list

```diff
@@ -1,299 +1,305 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.239000 ez_zarr-0.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.194999 ez_zarr-0.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.206999 ez_zarr-0.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/.github/workflows/documentation.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/.github/workflows/test_and_deploy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-02-09 12:55:42.239000 ez_zarr-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.210999 ez_zarr-0.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/docs/doc-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/docs/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/docs/hcs_wrappers.md
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/docs/plotting.md
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/docs/qmd-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15351 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/docs/quickstart.qmd
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/docs/testing.md
--rw-r--r--   0 runner    (1001) docker     (127)  2706736 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/docs/vignette.html
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-09 12:55:42.239000 ez_zarr-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.194999 ez_zarr-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.214999 ez_zarr-0.1.5/src/ez_zarr/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/src/ez_zarr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/src/ez_zarr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-09 12:55:42.000000 ez_zarr-0.1.5/src/ez_zarr/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    71156 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/src/ez_zarr/hcs_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20763 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/src/ez_zarr/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.239000 ez_zarr-0.1.5/src/ez_zarr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-02-09 12:55:42.000000 ez_zarr-0.1.5/src/ez_zarr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-02-09 12:55:42.000000 ez_zarr-0.1.5/src/ez_zarr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 12:55:42.000000 ez_zarr-0.1.5/src/ez_zarr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-09 12:55:42.000000 ez_zarr-0.1.5/src/ez_zarr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-09 12:55:42.000000 ez_zarr-0.1.5/src/ez_zarr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-09 12:55:42.000000 ez_zarr-0.1.5/src/ez_zarr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.214999 ez_zarr-0.1.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.214999 ez_zarr-0.1.5/tests/example_data/
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/generate_example_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.214999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.214999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.214999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.214999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.214999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/.zarray
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.194999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.194999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.214999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/0/0/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/0/0/0
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/0/0/1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.214999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/0/1/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/0/1/0
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/0/1/1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.194999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.218999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/1/0/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/1/0/0
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/1/0/1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.218999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/1/1/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/1/1/0
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/1/1/1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.194999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.218999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/2/0/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/2/0/0
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/2/0/1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.218999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/2/1/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/2/1/0
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/2/1/1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.198999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.198999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.218999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/0/0/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/0/0/0
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/0/0/1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.218999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/0/1/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/0/1/0
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/0/1/1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.198999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.218999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/1/0/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/1/0/0
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/1/0/1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.218999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/1/1/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/1/1/0
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/1/1/1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.198999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.218999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/2/0/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/2/0/0
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/2/0/1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.218999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/2/1/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/2/1/0
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/2/1/1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.218999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/1/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/1/.zarray
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.198999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/1/0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.198999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/1/0/0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.218999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/1/0/0/0/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/1/0/0/0/0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.198999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/1/0/1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.218999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/1/0/1/0/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/1/0/1/0/0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.198999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/1/0/2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.218999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/1/0/2/0/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/1/0/2/0/0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.198999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/1/1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.198999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/1/1/0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.218999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/1/1/0/0/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/1/1/0/0/0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.198999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/1/1/1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.222999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/1/1/1/0/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/1/1/1/0/0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.198999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/1/1/2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.222999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/1/1/2/0/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/1/1/2/0/0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.222999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/2/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/2/.zarray
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.198999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/2/0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.198999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/2/0/0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.222999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/2/0/0/0/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/2/0/0/0/0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.198999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/2/0/1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.222999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/2/0/1/0/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/2/0/1/0/0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.198999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/2/0/2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.222999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/2/0/2/0/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/2/0/2/0/0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.198999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/2/1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.198999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/2/1/0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.222999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/2/1/0/0/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/2/1/0/0/0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.198999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/2/1/1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.222999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/2/1/1/0/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/2/1/1/0/0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.198999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/2/1/2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.222999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/2/1/2/0/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/2/1/2/0/0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.222999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.222999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.222999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/X/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/X/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/X/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/X/0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.222999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/layers/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/layers/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/layers/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.222999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/obs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/obs/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/obs/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.222999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/obs/_index/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/obs/_index/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/obs/_index/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/obs/_index/0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.222999 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/obsm/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/obsm/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/obsm/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.227000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/obsp/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/obsp/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/obsp/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.227000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/uns/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/uns/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/uns/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.227000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/var/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/var/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/var/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.227000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/var/_index/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/var/_index/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/var/_index/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/var/_index/0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.227000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/varm/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/varm/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/varm/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.227000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/varp/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/varp/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/varp/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.227000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.227000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.227000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.227000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.227000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/0/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/0/.zarray
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.202999 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/0/0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.202999 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/0/0/0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.227000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/0/0/0/0/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/0/0/0/0/0
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/0/0/0/0/1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.227000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/0/0/0/1/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/0/0/0/1/0
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/0/0/0/1/1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.202999 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/0/1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.202999 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/0/1/0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.227000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/0/1/0/0/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/0/1/0/0/0
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/0/1/0/0/1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.231000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/0/1/0/1/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/0/1/0/1/0
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/0/1/0/1/1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.231000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/1/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/1/.zarray
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.202999 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/1/0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.202999 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/1/0/0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.231000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/1/0/0/0/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/1/0/0/0/0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.202999 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/1/1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.202999 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/1/1/0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.231000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/1/1/0/0/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/1/1/0/0/0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.231000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/2/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/2/.zarray
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.202999 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/2/0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.202999 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/2/0/0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.231000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/2/0/0/0/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/2/0/0/0/0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.202999 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/2/1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.202999 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/2/1/0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.231000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/2/1/0/0/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/2/1/0/0/0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.231000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.231000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.231000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/0/
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/0/.zarray
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.206999 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/0/0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.231000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/0/0/0/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/0/0/0/0
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/0/0/0/1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.231000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/0/0/1/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/0/0/1/0
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/0/0/1/1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.231000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/1/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/1/.zarray
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.206999 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/1/0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.231000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/1/0/0/
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/1/0/0/0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.231000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/2/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/2/.zarray
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.206999 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/2/0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.231000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/2/0/0/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/2/0/0/0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.231000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.231000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.235000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/X/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/X/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/X/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/X/0.0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.235000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/layers/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/layers/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/layers/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.235000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/obs/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/obs/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/obs/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.235000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/obs/_index/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/obs/_index/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/obs/_index/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/obs/_index/0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.235000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/obsm/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/obsm/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/obsm/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.235000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/obsp/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/obsp/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/obsp/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.235000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/uns/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/uns/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/uns/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.235000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/var/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/var/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/var/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.235000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/var/_index/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/var/_index/.zarray
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/var/_index/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/var/_index/0
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.235000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/varm/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/varm/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/varm/.zgroup
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:55:42.235000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/varp/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/varp/.zattrs
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/varp/.zgroup
--rw-r--r--   0 runner    (1001) docker     (127)    29575 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/test_hcs_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-02-09 12:55:25.000000 ez_zarr-0.1.5/tests/test_plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.708777 ez_zarr-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.668777 ez_zarr-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.684777 ez_zarr-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/.github/workflows/documentation.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/.github/workflows/test_and_deploy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-05-31 06:39:17.708777 ez_zarr-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.684777 ez_zarr-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/docs/doc-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/docs/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)    13455 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/docs/getting_started_Image.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    15545 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/docs/getting_started_hcs_wrappers.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/docs/hcs_wrappers.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/docs/ome_zarr.md
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/docs/plotting.md
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/docs/qmd-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/docs/testing.md
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/docs/utils.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 06:39:17.708777 ez_zarr-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.668777 ez_zarr-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.684777 ez_zarr-0.2.0/src/ez_zarr/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/src/ez_zarr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/src/ez_zarr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-31 06:39:17.000000 ez_zarr-0.2.0/src/ez_zarr/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72018 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/src/ez_zarr/hcs_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44964 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/src/ez_zarr/ome_zarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22389 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/src/ez_zarr/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9604 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/src/ez_zarr/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.708777 ez_zarr-0.2.0/src/ez_zarr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-05-31 06:39:17.000000 ez_zarr-0.2.0/src/ez_zarr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-05-31 06:39:17.000000 ez_zarr-0.2.0/src/ez_zarr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 06:39:17.000000 ez_zarr-0.2.0/src/ez_zarr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-31 06:39:17.000000 ez_zarr-0.2.0/src/ez_zarr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-31 06:39:17.000000 ez_zarr-0.2.0/src/ez_zarr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-31 06:39:17.000000 ez_zarr-0.2.0/src/ez_zarr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.688777 ez_zarr-0.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.688777 ez_zarr-0.2.0/tests/example_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     8159 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/generate_example_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.688777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.688777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.688777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.688777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.688777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/.zarray
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.672777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.672777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.688777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/0/0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/0/0/0
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/0/0/1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.688777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/0/1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/0/1/0
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/0/1/1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.672777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.688777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/1/0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/1/0/0
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/1/0/1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.692777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/1/1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/1/1/0
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/1/1/1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.672777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.692777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/2/0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/2/0/0
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/2/0/1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.692777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/2/1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/2/1/0
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/2/1/1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.672777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.672777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.692777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/0/0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/0/0/0
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/0/0/1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.692777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/0/1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/0/1/0
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/0/1/1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.672777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.692777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/1/0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/1/0/0
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/1/0/1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.692777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/1/1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/1/1/0
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/1/1/1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.672777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.692777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/2/0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/2/0/0
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/2/0/1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.692777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/2/1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/2/1/0
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/2/1/1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.692777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/1/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/1/.zarray
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.672777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/1/0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.672777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/1/0/0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.692777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/1/0/0/0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/1/0/0/0/0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.672777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/1/0/1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.692777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/1/0/1/0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/1/0/1/0/0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.672777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/1/0/2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.692777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/1/0/2/0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/1/0/2/0/0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.672777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/1/1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.672777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/1/1/0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.692777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/1/1/0/0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/1/1/0/0/0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.672777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/1/1/1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.692777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/1/1/1/0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/1/1/1/0/0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.672777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/1/1/2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.692777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/1/1/2/0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/1/1/2/0/0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.692777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/2/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/2/.zarray
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.676777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/2/0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.672777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/2/0/0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.692777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/2/0/0/0/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/2/0/0/0/0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.672777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/2/0/1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.692777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/2/0/1/0/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/2/0/1/0/0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.676777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/2/0/2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.696777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/2/0/2/0/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/2/0/2/0/0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.676777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/2/1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.676777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/2/1/0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.696777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/2/1/0/0/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/2/1/0/0/0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.676777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/2/1/1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.696777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/2/1/1/0/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/2/1/1/0/0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.676777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/2/1/2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.696777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/2/1/2/0/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/2/1/2/0/0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.696777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.696777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.696777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/X/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/X/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/X/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/X/0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.696777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/layers/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/layers/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.696777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/obs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/obs/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/obs/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.696777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/obs/_index/
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/obs/_index/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/obs/_index/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/obs/_index/0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.696777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/obsm/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/obsm/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/obsm/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.696777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/obsp/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/obsp/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/obsp/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.696777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/uns/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/uns/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/uns/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.696777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/var/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/var/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/var/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.700777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/var/_index/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/var/_index/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/var/_index/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/var/_index/0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.700777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/varm/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/varm/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/varm/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.700777 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/varp/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/varp/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/tables/FOV_ROI_table/varp/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.700777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.700777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.700777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.700777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.700777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/0/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/0/.zarray
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.676777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/0/0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.676777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/0/0/0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.700777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/0/0/0/0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/0/0/0/0/0
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/0/0/0/0/1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.700777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/0/0/0/1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/0/0/0/1/0
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/0/0/0/1/1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.676777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/0/1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.676777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/0/1/0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.700777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/0/1/0/0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/0/1/0/0/0
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/0/1/0/0/1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.700777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/0/1/0/1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/0/1/0/1/0
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/0/1/0/1/1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.700777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/1/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/1/.zarray
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.676777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/1/0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.676777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/1/0/0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.700777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/1/0/0/0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/1/0/0/0/0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.676777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/1/1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.680777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/1/1/0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.700777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/1/1/0/0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/1/1/0/0/0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.700777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/2/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/2/.zarray
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.680777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/2/0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.680777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/2/0/0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.700777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/2/0/0/0/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/2/0/0/0/0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.680777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/2/1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.680777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/2/1/0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.700777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/2/1/0/0/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/2/1/0/0/0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.704777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.704777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.704777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/0/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/0/.zarray
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.680777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/0/0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.704777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/0/0/0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/0/0/0/0
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/0/0/0/1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.704777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/0/0/1/
+-rw-r--r--   0 runner    (1001) docker     (127)     9906 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/0/0/1/0
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/0/0/1/1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.704777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/1/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/1/.zarray
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.680777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/1/0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.704777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/1/0/0/
+-rw-r--r--   0 runner    (1001) docker     (127)     9415 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/1/0/0/0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.704777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/2/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/2/.zarray
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.680777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/2/0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.704777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/2/0/0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/2/0/0/0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.704777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.704777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.704777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/X/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/X/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/X/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/X/0.0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.704777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/layers/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/layers/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.704777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/obs/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/obs/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/obs/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.704777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/obs/_index/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/obs/_index/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/obs/_index/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/obs/_index/0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.708777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/obsm/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/obsm/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/obsm/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.708777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/obsp/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/obsp/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/obsp/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.708777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/uns/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/uns/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/uns/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.708777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/var/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/var/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/var/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.708777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/var/_index/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/var/_index/.zarray
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/var/_index/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/var/_index/0
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.708777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/varm/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/varm/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/varm/.zgroup
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:39:17.708777 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/varp/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/varp/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/tables/FOV_ROI_table/varp/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (127)    29584 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/test_hcs_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29604 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/test_ome_zarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-31 06:39:07.000000 ez_zarr-0.2.0/tests/test_utils.py
```

### Comparing `ez_zarr-0.1.5/.github/workflows/documentation.yaml` & `ez_zarr-0.2.0/.github/workflows/documentation.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -25,19 +25,25 @@
         run: |
           python -m pip install -r docs/qmd-requirements.txt
           python -m pip install .
 
       - name: Set up Quarto
         uses: quarto-dev/quarto-actions/setup@v2
       
-      - name: Compile quarto documents
+      - name: Compile quarto documents (ome_zarr.Image)
         uses: quarto-dev/quarto-actions/render@v2
         with:
           to: md,ipynb # If set, it will be equivalent to `quarto render --to X`
-          path: docs/quickstart.qmd # By default, the current working dir is used i.e `quarto render .`
+          path: docs/getting_started_Image.qmd # runs in current working dir, i.e `quarto render .`
+
+      - name: Compile quarto documents (legacy classes)
+        uses: quarto-dev/quarto-actions/render@v2
+        with:
+          to: md,ipynb
+          path: docs/getting_started_hcs_wrappers.qmd
 
       - name: Clean up docs
         run: |
           rm -rf docs/20200812-CardiomyocyteDifferentiation14-Cycle1.zarr
 
       - name: Deploy docs
         uses: mhausenblas/mkdocs-deploy-gh-pages@master
```

### Comparing `ez_zarr-0.1.5/.github/workflows/test_and_deploy.yaml` & `ez_zarr-0.2.0/.github/workflows/test_and_deploy.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       matrix:
       #  platform: [ubuntu-latest, windows-latest, macos-latest]
         platform: [ubuntu-latest]
         python-version: ['3.9', '3.10', '3.11', '3.12']
 
     steps:
       - name: Check out repo
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
           cache-dependency-path: 'pyproject.toml'
           cache: 'pip'
@@ -33,31 +33,31 @@
         run: |
           python -m pip install --upgrade pip
           pip install pytest pytest-cov
           pip install -e .
 
       - name: Run tests
         shell: bash -l {0}
-        run: pytest --color=yes -v --cov=./ --cov-report=xml --cov-report=term-missing
+        run: pytest --color=yes -v --cov=./src --cov-report=xml --cov-report=term-missing tests
 
       - name: Upload coverage to Codecov
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
         env:
           CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
 
   deploy:
     # this will run when you have tagged a commit, starting with "v*"
     # and requires that you have put your twine API key in your
     # github secrets (see readme for details)
     needs: [test]
     runs-on: ubuntu-latest
     if: contains(github.ref, 'tags')
     steps:
       - name: Check out repo
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
 
       - name: Set up Python
         uses: actions/setup-python@v5
         with:
           python-version: '3.11'
 
       - name: Install dependencies
```

### Comparing `ez_zarr-0.1.5/.gitignore` & `ez_zarr-0.2.0/.gitignore`

 * *Files 20% similar despite different names*

```diff
@@ -163,11 +163,15 @@
 src/ez_zarr/_version.py
 
 # example data
 docs/20200812-CardiomyocyteDifferentiation*
 docs/__MACOSX
 
 # local vignette files (will be re-created online)
-docs/quickstart.md
-docs/quickstart_files
-docs/quickstart.ipynb
-docs/quickstart.html
+docs/getting_started_Image.md
+docs/getting_started_Image_files
+docs/getting_started_Image.ipynb
+docs/getting_started_Image.html
+docs/getting_started_hcs_wrappers.md
+docs/getting_started_hcs_wrappers_files
+docs/getting_started_hcs_wrappers.ipynb
+docs/getting_started_hcs_wrappers.html
```

### Comparing `ez_zarr-0.1.5/LICENSE` & `ez_zarr-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/PKG-INFO` & `ez_zarr-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez_zarr
-Version: 0.1.5
+Version: 0.2.0
 Summary: Give easy, high-level access to ome-zarr filesets.
 Author: Silvia Barbiero, Charlotte Soneson, Michael Stadler
 Maintainer-email: Michael Stadler <michael.stadler@fmi.ch>
 License: MIT License
         
         Copyright (c) 2023 Friedrich Miescher Institute for Biomedical Research
         
@@ -47,14 +47,15 @@
 License-File: LICENSE
 Requires-Dist: anndata
 Requires-Dist: dask
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: zarr
 Requires-Dist: matplotlib
+Requires-Dist: scikit-image
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 
 # ez_zarr
 
 ## Goals
@@ -89,17 +90,29 @@
 #   n_wells: 1
 #   n_channels: 2 (some-label-1, some-label-2)
 #   n_pyramid_levels: 3
 #   pyramid_zyx_scalefactor: {'0': array([1. 2. 2.])}
 #   full_resolution_zyx_spacing: [1.0, 0.1625, 0.1625]
 #   segmentations: 
 #   tables (measurements): FOV_ROI_table
+
+from ez_zarr import ome_zarr
+img = ome_zarr.Image('tests/example_data/plate_ones_mip.zarr/B/03/0')
+img
+# Image 0
+#   path: tests/example_data/plate_ones_mip.zarr/B/03/0
+#   n_channels: 2 (some-label-1, some-label-2)
+#   n_pyramid_levels: 3
+#   pyramid_zyx_scalefactor: [1. 2. 2.]
+#   full_resolution_zyx_spacing (micrometer): [1.0, 0.1625, 0.1625]
+#   segmentations: organoids
+#   tables (measurements): FOV_ROI_table
 ```
 
-A more extensive example is available from [here](https://fmicompbio.github.io/ez_zarr/quickstart/), also available as an [ipynb notebook](https://fmicompbio.github.io/ez_zarr/quickstart.ipynb).
+A more extensive example is available from [here](https://fmicompbio.github.io/ez_zarr/getting_started_hcs_wrappers/), also available as an [ipynb notebook](https://fmicompbio.github.io/ez_zarr/getting_started_hcs_wrappers.ipynb).
 
 ## Install
 The release version of `ez_zarr` can be installed using:
 ```
 pip install ez-zarr
 ```
```

### Comparing `ez_zarr-0.1.5/README.md` & `ez_zarr-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -32,17 +32,29 @@
 #   n_wells: 1
 #   n_channels: 2 (some-label-1, some-label-2)
 #   n_pyramid_levels: 3
 #   pyramid_zyx_scalefactor: {'0': array([1. 2. 2.])}
 #   full_resolution_zyx_spacing: [1.0, 0.1625, 0.1625]
 #   segmentations: 
 #   tables (measurements): FOV_ROI_table
+
+from ez_zarr import ome_zarr
+img = ome_zarr.Image('tests/example_data/plate_ones_mip.zarr/B/03/0')
+img
+# Image 0
+#   path: tests/example_data/plate_ones_mip.zarr/B/03/0
+#   n_channels: 2 (some-label-1, some-label-2)
+#   n_pyramid_levels: 3
+#   pyramid_zyx_scalefactor: [1. 2. 2.]
+#   full_resolution_zyx_spacing (micrometer): [1.0, 0.1625, 0.1625]
+#   segmentations: organoids
+#   tables (measurements): FOV_ROI_table
 ```
 
-A more extensive example is available from [here](https://fmicompbio.github.io/ez_zarr/quickstart/), also available as an [ipynb notebook](https://fmicompbio.github.io/ez_zarr/quickstart.ipynb).
+A more extensive example is available from [here](https://fmicompbio.github.io/ez_zarr/getting_started_hcs_wrappers/), also available as an [ipynb notebook](https://fmicompbio.github.io/ez_zarr/getting_started_hcs_wrappers.ipynb).
 
 ## Install
 The release version of `ez_zarr` can be installed using:
 ```
 pip install ez-zarr
 ```
```

### Comparing `ez_zarr-0.1.5/docs/index.md` & `ez_zarr-0.2.0/docs/index.md`

 * *Files 13% similar despite different names*

```diff
@@ -34,23 +34,26 @@
 #   n_pyramid_levels: 3
 #   pyramid_zyx_scalefactor: {'0': array([1. 2. 2.])}
 #   full_resolution_zyx_spacing: [1.0, 0.1625, 0.1625]
 #   segmentations: 
 #   tables (measurements): FOV_ROI_table
 ```
 
-A more extensive example is available from [here](https://fmicompbio.github.io/ez_zarr/quickstart/), also available as an [ipynb notebook](https://fmicompbio.github.io/ez_zarr/quickstart.ipynb).
+A more extensive example is available from [here](https://fmicompbio.github.io/ez_zarr/getting_started_hcs_wrappers/), also available as an [ipynb notebook](https://fmicompbio.github.io/ez_zarr/getting_started_hcs_wrappers.ipynb).
 
 ## Install
+
+`ez_zarr` is hosted on GitHub at [github.com/fmicompbio/ez_zarr](https://github.com/fmicompbio/ez_zarr) and the documentation can be found at [fmicompbio.github.io/ez_zarr](https://fmicompbio.github.io/ez_zarr/).
+
 The release version of `ez_zarr` can be installed using:
 ```
 pip install ez-zarr
 ```
 
-The current (development) `ez_zarr` can be installed from github.com using:
+The current (development) version of `ez_zarr` can be installed from github.com using:
 ```
 pip install git+ssh://git@github.com/fmicompbio/ez_zarr.git
 ```
 
 ## Software status
 [![unit-tests](https://github.com/fmicompbio/ez_zarr/actions/workflows/test_and_deploy.yaml/badge.svg)](https://github.com/fmicompbio/ez_zarr/actions/workflows/test_and_deploy.yaml)
 [![codecov](https://codecov.io/gh/fmicompbio/ez_zarr/graph/badge.svg?token=GEBLX8ENJ1)](https://codecov.io/gh/fmicompbio/ez_zarr)
```

### Comparing `ez_zarr-0.1.5/docs/quickstart.qmd` & `ez_zarr-0.2.0/docs/getting_started_hcs_wrappers.qmd`

 * *Files 2% similar despite different names*

```diff
@@ -8,28 +8,30 @@
 
 The aim of `ez_zarr` is to provide easy, high-level access to high content screening microscopy data, stored as OME-Zarr filesets according to the [NGFF](https://ngff.openmicroscopy.org/latest/) specifications with additional metadata fields, for example the ones generated by the [Fractal](https://fractal-analytics-platform.github.io/fractal-tasks-core/) platform.
 
 The goal is that users can write simple scripts working with plates, wells and fields of view, without having to understand how these are represented within an OME-Zarr fileset.
 
 # Installation
 
-`ez_zarr` is hosted on GitHub at [github.com/fmicompbio/ez_zarr](https://github.com/fmicompbio/ez_zarr) and the documentation of can be found at [fmicompbio.github.io/ez_zarr](https://fmicompbio.github.io/ez_zarr/).
+`ez_zarr` is hosted on GitHub at [github.com/fmicompbio/ez_zarr](https://github.com/fmicompbio/ez_zarr) and the documentation can be found at [fmicompbio.github.io/ez_zarr](https://fmicompbio.github.io/ez_zarr/).
 
 The release version of `ez_zarr` can be installed using:
 ```{.bash}
 pip install ez-zarr
 ```
 
-The current (development) `ez_zarr` can be installed from github.com using:
+The current (development) version of `ez_zarr` can be installed from github.com using:
 ```{.bash}
 pip install git+ssh://git@github.com/fmicompbio/ez_zarr.git
 ```
 
 # Quickstart
 
+Note: If you prefer to run these examples interactively, you can also download them as an [ipynb notebook](https://fmicompbio.github.io/ez_zarr/getting_started_hcs_wrappers.ipynb).
+
 Here are some examples of how you can use `ez_zarr`:
 
 ## Download example data
 
 To run the code below, you will first need to download some Fractal output data.
 You can do this for example by running the following from a terminal:
 ```{.bash}
@@ -79,19 +81,19 @@
 We open a single OME-Zarr directory, typically representing a single plate:
 ```{python}
 zarr_directory = '20200812-CardiomyocyteDifferentiation14-Cycle1_mip.zarr'
 plate = hcs_wrappers.FractalZarr(zarr_directory, name = 'cardio-d14')
 plate
 ```
 
-`plate` represents a maximum intensity projection of an acquisition with 1 wells and 1 channel.
+`plate` represents a maximum intensity projection of an acquisition with 1 well and 1 channel.
 
 There are 5 `pyramid_levels` available (0 to 4), meaning that in addition to the full resolution data (level 0), we have four more levels that provide the data in 2-fold lower resolutions (see `pyramid_zyx_scalefactor`), for example for faster plotting.
 
-This OME-Zarr fileset also contains a segmentation (`nuclei`), for which measurements ahve been extracted and saved in table `nuclei`. In addition, there are some further tables, such as `FOV_ROI_table`, which contains the coordinates of the fields of view, or `nuclei_ROI_table`, which contains the bounding box coordinates for the segmented nuclei.
+This OME-Zarr fileset also contains a segmentation (`nuclei`), for which measurements have been extracted and saved in the table `nuclei`. In addition, there are some further tables, such as `FOV_ROI_table`, which contains the coordinates of the fields of view, or `nuclei_ROI_table`, which contains the bounding box coordinates for the segmented nuclei.
 
 ## Get information from `plate`
 
 You can obtain information on the content available in the fileset:
 ```{python}
 # path to the OME-Zarr fileset
 plate.get_path()
@@ -121,15 +123,15 @@
 ```{python}
 # ... for labels
 plate.level_zyx_spacing_labels
 ```
 
 ## Extract a table from the OME-Zarr fileset
 
-The tables are stored within the fileset as describe in the [Fractal documentation](https://fractal-analytics-platform.github.io/fractal-tasks-core/tables/).
+The tables are stored within the fileset as described in the [Fractal documentation](https://fractal-analytics-platform.github.io/fractal-tasks-core/tables/).
 
 As mentioned the goal of `ez_zarr` is to abstract the internal structure and make it simple to obtain these tables, if necessary accumulated over many wells, as a `pandas.DataFrame` :
 ```{python}
 #| output: false
 df = plate.get_table(table_name='FOV_ROI_table')
 df
 ```
```

### Comparing `ez_zarr-0.1.5/pyproject.toml` & `ez_zarr-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ez_zarr"
-version = "0.1.5"
+version = "0.2.0"
 description = "Give easy, high-level access to ome-zarr filesets."
 readme = { file = "README.md", content-type = "text/markdown" }
 authors = [
     { name = "Silvia Barbiero" },
     { name = "Charlotte Soneson" },
     { name = "Michael Stadler" }
 ]
@@ -34,15 +34,16 @@
 keywords = ["ome_zarr", "image analysis", "Fractal"]
 dependencies = [
     "anndata",
     "dask",
     "numpy",
     "pandas",
     "zarr",
-    "matplotlib"
+    "matplotlib",
+    "scikit-image"
 ]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = ["pytest", "pytest-cov"]
 
 [project.urls]
```

### Comparing `ez_zarr-0.1.5/src/ez_zarr/__main__.py` & `ez_zarr-0.2.0/src/ez_zarr/__main__.py`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/src/ez_zarr/hcs_wrappers.py` & `ez_zarr-0.2.0/src/ez_zarr/hcs_wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-"""Wrap ome-zarr filesets in a class.
+"""Wrap OME-Zarr filesets in a class.
 
-Represent an ome-zarr fileset as a class to give high-level
+Represent an OME-Zarr fileset as a class to give high-level
 access to its contents.
 
 Classes:
-    FractalZarr: Contains a single .zarr fileset, typically a plate.
-    FractalZarrSet: Contains one or several .zarr filesets, typically a plate
+    FractalZarr: Contains a single `.zarr` fileset, typically a plate.
+    FractalZarrSet: Contains one or several `.zarr` filesets, typically a plate
         (4 dimensional data) and a maximum-intensity projection derived from it.
 """
 
 __all__ = ['FractalZarr', 'FractalZarrSet']
 __version__ = '0.1.5'
 __author__ = 'Silvia Barbiero, Michael Stadler'
 
@@ -24,36 +24,36 @@
 import warnings
 import random
 from typing import Union, Optional, Any
 
 
 # FractalZarr class ---------------------------------------------------------------
 class FractalZarr:
-    """Represents a ome-zarr fileset."""
+    """Represents an OME-Zarr fileset."""
 
     # constructor and helper functions ----------------------------------------
     def __init__(self, zarr_path: str, name: Optional[str]=None) -> None:
         """
-        Initializes an ome-zarr fileset (.zarr) from its path.
+        Initializes an OME-Zarr fileset (.zarr) from its path.
         Typically, the fileset represents a single assay plate, and 
-        we assume that the structures (pyramid levels, labels, table, etc.)
+        we assume that the structures (pyramid levels, labels, tables, etc.)
         are consistent across wells.
 
         Parameters:
             zarr_path (str): Path containing the plate ome-zarr fileset.
             name (str, optional): Optional name for the plate.
         
         Examples:
             Get an object corresponding to a plate.
 
             >>> from ez_zarr import hcs_wrappers
             >>> plateA = hcs_wrappers.FractalZarr('path/to/plate.zarr')
             >>> plateA
 
-            This will print information on the plate.
+            This will print information about the plate.
         """
 
         self.path: str = zarr_path
         self.name: str = ''
         if name:
             self.name = name
         else:
@@ -177,15 +177,15 @@
             else:
                 pyramid_level = int(self.level_paths_labels[pyramid_ref[1]][-1])
         else:
             # make sure it is an integer
             pyramid_level = int(pyramid_level)
         return pyramid_level
     
-    def _calculate_regular_grid_coordsinates(self, y, x, num_y=10, num_x=10):
+    def _calculate_regular_grid_coordinates(self, y, x, num_y=10, num_x=10):
         """
         [internal] Calculate the cell coordinates for a regular rectangular grid of total size (y, x)
         by splitting the dimensions into num_y and num_x cells.
         
         Returns a list of (y_start, y_end, x_start, x_end) tuples. The coordinates are
         inclusive at the start and exclusive at the end.
 
@@ -220,65 +220,65 @@
         return f"FractalZarr {self.name}\n  path: {self.path}\n  n_wells: {nwells}\n  n_channels: {nch} ({chlabs})\n  n_pyramid_levels: {npl}\n  pyramid_zyx_scalefactor: {self.level_zyx_scalefactor}\n  full_resolution_zyx_spacing (µm): {self.level_zyx_spacing_images[self.image_names[0]][0]}\n  segmentations: {segnames}\n  tables (measurements): {tabnames}\n"
     
     def __repr__(self):
         return str(self)
     
     # accessors ---------------------------------------------------------------
     def get_path(self) -> str:
-        """Gets the path of the ome-zarr fileset.
+        """Get the path of an OME-Zarr fileset.
         
         Returns:
-            The path to the ome-zarr fileset.
+            The path to the OME-Zarr fileset.
         """
         return self.path
 
     def get_wells(self, simplify: bool=False) -> Union[list[dict[str, Any]], list[str]]:
-        """Gets info on wells in the ome-zarr fileset.
+        """Get info on wells in an OME-Zarr fileset.
 
         Parameters:
             simplify (bool): If `True`, the well names are returned in human readable form (e.g. 'B03').
         
         Returns:
             A list of wells in the plate, either name strings (if `simplify=True`) or dicts with well attributes.
         """
         if simplify:
             return [w['path'].replace('/', '') for w in self.wells]
         else:
             return self.wells
 
     def get_channels(self) -> list:
-        """Gets info on channels in the ome-zarr fileset.
+        """Get info on channels in an OME-Zarr fileset.
         
         Returns:
             A list of dicts with information on channels.
         """
         return self.channels
     
     def get_label_names(self) -> list:
-        """Gets list of label names in the ome-zarr fileset.
+        """Get list of label names in an OME-Zarr fileset.
         
         Returns:
             A list of label names (str) available in the plate.
         """
         return self.label_names
 
     def get_table_names(self) -> list:
-        """Gets list of table names in the ome-zarr fileset.
+        """Get list of table names in an OME-Zarr fileset.
         
         Returns:
             A list of table names (str) available in the plate.
         """
         return self.table_names
 
     # query methods -----------------------------------------------------------
     def get_table(self,
                   table_name: str,
                   include_wells: Union[str, list[str]]=[],
                   as_AnnData: bool=False) -> Any:
-        """Extract table for wells in a ome-zarr fileset.
+        """Extract table for wells in an OME-Zarr fileset.
         
         Parameters:
             table_name (str): The name of the table to extract.
             include_wells (str or list): List of well names to include. If empty `[]`, all wells are included.
             as_AnnData (bool): If `True`, the table is returned as an `AnnData` object, otherwise it is converted to a `pandas.DataFrame`.
         
         Returns:
@@ -323,15 +323,15 @@
                       image_name: str='0',
                       pyramid_level: Optional[int]=None,
                       pyramid_level_coord: Optional[int]=None,
                       as_NumPy: bool=False) -> Union[dask.array.Array, np.ndarray]:
         """
         Extract a region of interest from a well image by coordinates.
 
-        None or at least two of `upper_left_yx`, `lower_right_yx` and `size_yx` need to be given.
+        None or exactly two of `upper_left_yx`, `lower_right_yx` and `size_yx` need to be given.
         If none are given, it will return the full image (the whole well).
         Otherwise, `upper_left_yx` contains the lower indices than `lower_right_yx`
         (origin on the top-left, zero-based coordinates), and each of them is
         a tuple of (y, x). No z coordinate needs to be given, all z planes are returned
         if there are several ones.
 
         Parameters:
@@ -391,15 +391,15 @@
                                                              pyramid_ref_from=('image', image_name),
                                                              pyramid_ref_to=('image', image_name))[1:]
             img = img[:,
                       :,
                       slice(upper_left_yx[0], lower_right_yx[0] + 1),
                       slice(upper_left_yx[1], lower_right_yx[1] + 1)]
         elif num_unknowns != 3:
-            raise ValueError("Either none or two of `upper_left_yx`, `lower_rigth` and `size_yx` have to be given")
+            raise ValueError("Either none or two of `upper_left_yx`, `lower_right_yx` and `size_yx` have to be given")
 
         # convert if needed and return
         if as_NumPy:
             img = np.array(img)
         return img
 
     def get_image_table_idx(self,
@@ -477,16 +477,16 @@
                             sample_method: str='sum',
                             channel: int=0,
                             seed: int=42,
                             as_NumPy: bool=False) -> Union[tuple[list[tuple[int]], list[dask.array.Array]], tuple[list[tuple[int]], list[np.ndarray]]]:
         """
         Split a well image into a regular grid and extract a subset of grid cells (all z planes if several).
 
-        `num_y` and `num_x` define the grid by specifying the number of cell in y and x.
-        `num_select` picks that many from the total number of grid cells and returns them as a list.
+        `num_y` and `num_x` define the grid by specifying the number of cells in y and x.
+        `num_select` grid cells are picked from the total number and returned as a list.
         All returned grid cells are guaranteed to be of equal size, but a few pixels from the image
         may not be included in grid cells of the last row or column if the image shape
         is not divisible by `num_y` or `num_x`.
 
         Parameters:
             well (str):  The well (e.g. 'B03') from which an image should be extracted.
             pyramid_level (int): The pyramid level (resolution level), from which the
@@ -506,17 +506,17 @@
                 - 'random': order grid cells randomly (use `seed`)
             channel (int): Selects the channel on which `sample_method` is calculated.
             seed (int): Used in `random.seed()` to make sampling for `sample_method='random'` reproducible.
             as_NumPy (bool): If `True`, return the grid cell image as `numpy.ndarray` objects with
                 shapes (c,z,y,x). Otherwise, return the (on-disk) `dask` arrays of the same dimensions.
         
         Returns:
-            A tuple of two lists (coord_list, img_list), each with `num_select` elements
-            corresponding to the coordinates and images of selected grid cells.
-            The coordinates are tuples of the form  (y_start, y_end, x_start, x_end).
+            A tuple of two lists (coord_list, img_list), each with `num_select` elements 
+                corresponding to the coordinates and images of selected grid cells. 
+                The coordinates are tuples of the form  (y_start, y_end, x_start, x_end).
 
         Examples:
             Obtain grid cells with highest signal sum in channel 0 from well 'A02':
 
             >>> plateA.get_image_grid_ROIs(well='A02')
         """
         # digest arguments
@@ -530,21 +530,21 @@
         img = dask.array.from_zarr(img_path)
         img_path_lowres = os.path.join(self.path, well, '0', str(lowres_level))
         img_lowres = dask.array.from_zarr(img_path_lowres)
 
         # calculate grid coordinates as a list of (y_start, y_end, x_start, x_end)
         # (images are always of 4D shape c,z,y,x)
         ch, z, y, x = img.shape
-        grid = self._calculate_regular_grid_coordsinates(y=y, x=x,
-                                                         num_y=num_y,
-                                                         num_x=num_x)
+        grid = self._calculate_regular_grid_coordinates(y=y, x=x,
+                                                        num_y=num_y,
+                                                        num_x=num_x)
         ch_lr, z_lr, y_lr, x_lr = img_lowres.shape
-        grid_lowres = self._calculate_regular_grid_coordsinates(y=y_lr, x=x_lr,
-                                                                num_y=num_y,
-                                                                num_x=num_x)
+        grid_lowres = self._calculate_regular_grid_coordinates(y=y_lr, x=x_lr,
+                                                               num_y=num_y,
+                                                               num_x=num_x)
 
         # select and extract grid cells
         sel_coords = []
         sel_img_cells = []
 
         if sample_method == 'sum':
             grid_values = [
@@ -593,15 +593,15 @@
                       upper_left_yx: Optional[tuple[int]]=None,
                       lower_right_yx: Optional[tuple[int]]=None,
                       size_yx: Optional[tuple[int]]=None,
                       as_NumPy: bool=False) -> Union[dask.array.Array, np.ndarray]:
         """
         Extract a region of interest from a label mask (segmentation) by coordinates.
 
-        None or at least two of `upper_left_yx`, `lower_right_yx` and `size_yx` need to be given.
+        None or exactly two of `upper_left_yx`, `lower_right_yx` and `size_yx` need to be given.
         If none are given, it will return the full image (the whole well).
         Otherwise, `upper_left_yx` contains the lower indices than `lower_right_yx`
         (origin on the top-left, zero-based coordinates), and each of them is
         a tuple of (y, x). No z coordinate needs to be given, all z planes are returned
         if there are several ones.
 
         Parameters:
@@ -621,15 +621,15 @@
             as_NumPy (bool): If `True`, return the image as 4D `numpy.ndarray` object (c,z,y,x).
                 Otherwise, return the (on-disk) `dask` array of the same dimensions.
         
         Returns:
             The extracted label mask, either as a `dask.array.Array` on-disk array, or as an in-memory `numpy.ndarray` if `as_NumPy=True`.
         
         Examples:
-            Obtain the label mask of the lowest-resolution for the full well 'A02':
+            Obtain the label mask of the lowest-resolution pyramid level for the full well 'A02':
 
             >>> plateA.get_label_ROI(well='A02')
         """
         # digest arguments
         well = self._digest_well_argument(well)
         assert label_name in self.label_names, f"Unknown label_name {label_name}, should be one of " + ', '.join(self.label_names)
         pyramid_level = self._digest_pyramid_level_argument(pyramid_level, ('image', image_name))
@@ -661,30 +661,30 @@
                                                              pyramid_level_to=pyramid_level,
                                                              pyramid_ref_from=('image', image_name),
                                                              pyramid_ref_to=('image', image_name))[1:]
             msk = msk[:,
                       slice(upper_left_yx[0], lower_right_yx[0] + 1),
                       slice(upper_left_yx[1], lower_right_yx[1] + 1)]
         elif num_unknowns != 3:
-            raise ValueError("Either none or two of `upper_left_yx`, `lower_rigth` and `size_yx` have to be given")
+            raise ValueError("Either none or two of `upper_left_yx`, `lower_right_yx` and `size_yx` have to be given")
 
         # convert if needed and return
         if as_NumPy:
             msk = np.array(msk)
         return msk
 
     def get_label_table_idx(self,
                             label_name: str,
                             table_name: str,
                             table_idx: int,
                             well: Optional[str]=None,
                             pyramid_level: Optional[int]=None,
                             as_NumPy: bool=False) -> Union[dask.array.Array, np.ndarray]:
         """
-        Extract a region of interest from a label maks (segmentation) by table name and row index.
+        Extract a region of interest from a label mask (segmentation) by table name and row index.
 
         Bounding box coordinates will be automatically obtained from the table
         `table_name` and row `row_idx` (zero-based row index).
         All z planes are returned if there are several ones.
 
         Parameters:
             label_name (str): The name of the segmentation
@@ -749,18 +749,18 @@
                                     pyramid_ref: tuple[str]=('image', '0')) -> tuple[int]:
         """
         Convert micrometers to pixels for a given pyramid level.
 
         Parameters:
             zyx (tuple): The micrometer coordinates in the form (z, y, x) to be converted
                 to pixels.
-            pyramid_level (int): The pyramid level (resolution), to which the output
+            pyramid_level (int): The pyramid level (resolution), which the output
                 pixel coordinates will refer to.  If `None`, the lowest-resolution
                 (highest) pyramid level will be selected.
-            pyramid_ref (tuple(str, str)): reference to which the `pyramid_level` refers
+            pyramid_ref (tuple(str, str)): The reference that the `pyramid_level` refers
                 to. It is given as a tuple with two `str` elements, the first being
                 either 'image' or 'label', and the second being the name of the
                 image or label. The default is ('image', '0').
         
         Returns:
             A tuple (z, y, x) with pixel coordinates.
         
@@ -790,18 +790,18 @@
                                     pyramid_ref: tuple[str]=('image', '0')) -> tuple[float]:
         """
         Convert pixels to micrometers for a given pyramid level.
 
         Parameters:
             zyx (tuple): The pixel coordinates in the form (z, y, x) to be converted
                 to micrometers.
-            pyramid_level (int): The pyramid level (resolution), to which the input
+            pyramid_level (int): The pyramid level (resolution), which the input
                 pixel coordinates refer to. If `None`, the lowest-resolution
                 (highest) pyramid level will be selected.
-            pyramid_ref (tuple(str, str)): reference to which the `pyramid_level` refers
+            pyramid_ref (tuple(str, str)): The reference that the `pyramid_level` refers
                 to. It is given as a tuple with two `str` elements, the first being
                 either 'image' or 'label', and the second being the name of the
                 image or label. The default is ('image', '0').
         
         Returns:
             A tuple (z, y, x) with micrometer coordinates.
         
@@ -830,25 +830,25 @@
                                pyramid_ref_from: tuple[str]=('image', '0'),
                                pyramid_ref_to: tuple[str]=('image', '0')) -> tuple[int]:
         """
         Convert pixel coordinates between pyramid levels.
 
         Parameters:
             zyx (tuple): The pixel coordinates in the form (z, y, x) to be converted.
-            pyramid_level_from (int): The pyramid level (resolution), to which the input
+            pyramid_level_from (int): The pyramid level (resolution), which the input
                 pixel coordinates refer to. If `None`, the lowest-resolution
                 (highest) pyramid level will be selected.
-            pyramid_level_to (int): The pyramid level (resolution), to which the output
+            pyramid_level_to (int): The pyramid level (resolution), which the output
                 pixel coordinates will refer to. If `None`, the lowest-resolution
                 (highest) pyramid level will be selected.
-            pyramid_ref_from (tuple(str, str)): reference to which the `pyramid_level_from` refers
+            pyramid_ref_from (tuple(str, str)): The reference that the `pyramid_level_from` refers
                 to. It is given as a tuple with two `str` elements, the first being
                 either 'image' or 'label', and the second being the name of the
                 image or label. The default is ('image', '0').
-            pyramid_ref_to (tuple(str, str)): reference to which the `pyramid_level_to` refers
+            pyramid_ref_to (tuple(str, str)): The reference that the `pyramid_level_to` refers
                 to. It is given as a tuple with two `str` elements, the first being
                 either 'image' or 'label', and the second being the name of the
                 image or label. The default is ('image', '0').
         
         Returns:
             A tuple (z, y, x) with pixel coordinates in the new pyramid level.
         
@@ -882,15 +882,15 @@
     def calc_average_FOV(self,
                          include_wells: Union[str, list[str]]=[],
                          pyramid_level: Optional[int]=None,
                          channel: int=0) -> np.ndarray:
         """
         Calculate the average field of view.
          
-        Using the coordinates stored in table 'FOV_ROI_table', calculate the averge
+        Using the coordinates stored in table 'FOV_ROI_table', calculate the averaged
         field of view for wells in `include_wells`, for `channel` at resolution `pyramid_level`.
 
         Parameters:
             include_wells (str or list): List of well names to include. If empty `[]`, all wells are included.
             pyramid_level (int): The pyramid level (resolution level), from which the image
                 should be extracted. If `None`, the lowest-resolution (highest) pyramid level
                 will be selected.
@@ -959,44 +959,45 @@
                   upper_left_yx: Optional[tuple[int]]=None,
                   lower_right_yx: Optional[tuple[int]]=None,
                   size_yx: Optional[tuple[int]]=None,
                   image_name: str='0',
                   label_name: Optional[str]=None,
                   label_alpha: float=0.3,
                   pyramid_level: Optional[int]=None,
-                  pyramid_level_coord: Optional[int]=None,                  
+                  pyramid_level_coord: Optional[int]=None,
                   channels: list[int]=[0],
                   channel_colors: list[str]=['white'],
                   channel_ranges: list[list[float]]=[[0.01, 0.95]],
                   z_projection_method: str='maximum',
                   axis_style: str='pixel',
                   title: Optional[str]=None,
                   scalebar_micrometer: int=0,
                   scalebar_color: str='white',
                   scalebar_position: str='bottomright',
                   scalebar_label: bool=False,
+                  call_show: bool=True,
                   fig_width_inch: float=8.0,
                   fig_height_inch: float=8.0,
                   fig_dpi: int=200,
                   fig_style: str='dark_background'):
         """
-        Plot microtiter plate.
+        Plot a well from a microtiter plate.
          
-        Plot an overview of all wells in plate arrangement, for `channel` at
+        Plot an overview of a single well, for `channel` at
         resolution `pyramid_level`.
 
         Parameters:
             well (str): The well (e.g. 'B03') to be plotted.
             upper_left_yx (tuple): Tuple of (y, x) coordinates for the upper-left
                 (lower) coordinates defining the region of interest.
             lower_right_yx (tuple): Tuple of (y, x) coordinates for the lower-right
                 (higher) coordinates defining the region of interest.
             size_yx (tuple): Tuple of (size_y, size_x) defining the size of the
                 region of interest.
-            image_name (str): The name of the image in each well to be plotted.
+            image_name (str): The name of the image in the well to be plotted.
                 Default: '0'.
             label_name (str): The name of the a segmentation mask to be plotted
                 semi-transparently over the images. If `None`, just the image
                 is plotted.
             label_alpha (float): A scalar value between 0 (fully transparent)
                 and 1 (solid) defining the transparency of the label masks.
             pyramid_level (int): The pyramid level (resolution level), from
@@ -1020,29 +1021,38 @@
                 (default: 'maximum').
             axis_style (str): A string scalar defining how to draw the axis. Should
                 be one of 'none' (no axis), 'pixel' (show pixel labels, the default)
                 or 'micrometer' (show micrometer labels). If `axis_style='micrometer'`,
                 `spacing_yx` is used to convert pixel to micrometer.
             title (str): String scalar to add as title. If `None`, `well` will
                 be used as `title`.
-            scalebar_micrometer (int): If non-zero, add a scale bar corresonding
+            scalebar_micrometer (int): If non-zero, add a scale bar corresponding
                 to `scalebar_micrometer` to the bottom right.
             scalebar_label (bool): If `True`, add micrometer label to scale bar.
-            fig_width_inch (float): Figure width (inch).
-            fig_height_inch (float): Figure height (inch).
+            call_show (bool): If `True`, the call to `matplotlib.pyplot.imshow` is
+                embedded between `matplotlib.pyplot.figure` and
+                `matplotlib.pyplot.show`/`matplotlib.pyplot.close` calls.
+                This is the default behaviour and typically used when an individual
+                image should be plotted and displayed. It can be set to `False`
+                if multiple images should be plotted and their arrangement
+                is controlled outside of `plotting.plot_image`. The parameters
+                `fig_width_inch`, `fig_height_inch` and `fig_dpi` are ignored
+                in that case.
+            fig_width_inch (float): Figure width (in inches).
+            fig_height_inch (float): Figure height (in inches).
             fig_dpi (int): Figure resolution (dots per inch).
             fig_style (str): Style for the figure. Supported are 'brightfield', which
                 is a special mode for single-channel brightfield microscopic images
                 (it will automatically set `channels=[0]`, `channel_colors=['white']`
-                `z_projection_method='minimum' and `fig_style='default'`), and any
-                other styles that can bepassed to `matplotlib.pyplot.style.context`
+                `z_projection_method='minimum'` and `fig_style='default'`), and any
+                other styles that can be passed to `matplotlib.pyplot.style.context`
                 (default: 'dark_background')
 
         Examples:
-            Overview plot of a well 'B03'.
+            Overview plot of the well 'B03'.
 
             >>> plateA.plot_well(well='B03')
         """
         # digest arguments
         well = self._digest_well_argument(well, as_path=False)
         assert image_name in self.image_names, (
             f"Unknown image_name ({image_name}), should be one of "
@@ -1120,15 +1130,15 @@
                             axis_style=axis_style,
                             spacing_yx=self.level_zyx_spacing_images[image_name][img_pl][1:],
                             title=title,
                             scalebar_pixel=scalebar_pixel,
                             scalebar_color=scalebar_color,
                             scalebar_position=scalebar_position,
                             scalebar_label=scalebar_label,
-                            call_show=True,
+                            call_show=call_show,
                             fig_width_inch=fig_width_inch,
                             fig_height_inch=fig_height_inch,
                             fig_dpi=fig_dpi,
                             fig_style=fig_style)
 
     def plot_plate(self,
                    image_name: str='0',
@@ -1150,15 +1160,15 @@
          
         Plot an overview of all wells in plate arrangement, for `channel` at
         resolution `pyramid_level`.
 
         Parameters:
             image_name (str): The name of the image in each well to be plotted.
                 Default: '0'.
-            label_name (str): The name of the a segmentation mask to be plotted
+            label_name (str): The name of the segmentation mask to be plotted
                 semi-transparently over the images. If `None`, just the image
                 is plotted.
             label_alpha (float): A scalar value between 0 (fully transparent)
                 and 1 (solid) defining the transparency of the label masks.
             pyramid_level (int): The pyramid level (resolution level), from
                 which the image should be extracted. If `None`, the
                 lowest-resolution (highest) pyramid level will be selected.
@@ -1176,22 +1186,22 @@
                 For available methods, see ez_zarr.plotting.zproject
                 (default: 'maximum').
             plate_layout (str): Defines the layout of the plate
                 (default: '96well').
             fig_title (str): String scalar to use as overall figure title
                 (default: the `.name` attribute of the object). Use `fig_title=''`
                 to not add any title to the plot.
-            fig_width_inch (float): Figure width (inch).
-            fig_height_inch (float): Figure height (inch).
+            fig_width_inch (float): Figure width (in inches).
+            fig_height_inch (float): Figure height (in inches).
             fig_dpi (int): Figure resolution (dots per inch).
             fig_style (str): Style for the figure. Supported are 'brightfield', which
                 is a special mode for single-channel brightfield microscopic images
                 (it will automatically set `channels=[0]`, `channel_colors=['white']`
-                `z_projection_method='minimum' and `fig_style='default'`), and any
-                other styles that can bepassed to `matplotlib.pyplot.style.context`
+                `z_projection_method='minimum'` and `fig_style='default'`), and any
+                other styles that can be passed to `matplotlib.pyplot.style.context`
                 (default: 'dark_background')
 
         Examples:
             Overview plot of a plate for image channel 1.
 
             >>> plateA.plot_plate(channels=[1])
         """
@@ -1315,52 +1325,55 @@
 # FractalZarrSet class ------------------------------------------------------
 class FractalZarrSet:
     """Represents a folder containing one or several ome-zarr fileset(s)."""
 
     # constructor and helper functions ----------------------------------------
     def __init__(self, path: str, name=None) -> None:
         """
-        Initializes a container for a folder containing one or several ome-zarr
+        Initializes a container for a folder containing one or several OME-Zarr
         fileset(s) (.zarr). Typically, the object is used for a folder which
-        contains exactly two related .zarr objects, one corresponding to the
+        contains exactly two related `.zarr` objects, one corresponding to the
         four-dimensional (c,z,y,x) plate dataset, and a second one corresponding to
         a three-dimensional maximum intensity projection derived from it.
 
         Parameters:
-            path (str): Path containing the ome-zarr fileset(s).
+            path (str): Path containing the OME-Zarr fileset(s).
             name (str): Optional name for the experiment.
         
         Examples:
-            Get an object corresponding to a set of .zarr's.
+            Get an object corresponding to a set of `.zarr`s.
 
             >>> from ez_zarr import hcs_wrappers
             >>> plate_set = hcs_wrappers.FractalZarrSet('path/to/zarrs')
             >>> plate_set
 
-            This will print information on the zarrs.
+            This will print information on the `.zarr`s.
         """
         if not os.path.isdir(path):
             raise ValueError(f'`{path}` does not exist')
         self.path: str = path
         self.name: str = ''
         if name is None:
             self.name = os.path.basename(self.path)
         else:
             self.name = name
         self.zarr_paths: list[str] = [f for f in os.listdir(self.path) if f[-5:] == '.zarr']
         if len(self.zarr_paths) == 0:
-            raise ValueError(f'no .zarr filesets found in `{path}`')
-        self.zarr: list[FractalZarr] = [FractalZarr(os.path.join(self.path, f)) for f in self.zarr_paths]
-        self.zarr_names: list[str] = [x.name for x in self.zarr]
+            raise ValueError(f'no `.zarr` filesets found in `{path}`')
         self.zarr_mip_idx: Optional[int] = None
         self.zarr_3d_idx: Optional[int] = None
-        if len(self.zarr) == 2 and self.zarr_names[0].replace('_mip.zarr', '.zarr') == self.zarr_names[1]:
-            # special case of 3D plate plus derived maximum intensity projection?
-            self.zarr_mip_idx = 0
-            self.zarr_3d_idx = 1
+        if len(self.zarr_paths) == 2:
+            if self.zarr_paths[1].replace('_mip.zarr', '.zarr') == self.zarr_paths[0]:
+                self.zarr_paths.reverse()
+            if self.zarr_paths[0].replace('_mip.zarr', '.zarr') == self.zarr_paths[1]:
+                # special case of 3D plate plus derived maximum intensity projection?
+                self.zarr_mip_idx = 0
+                self.zarr_3d_idx = 1
+        self.zarr: list[FractalZarr] = [FractalZarr(os.path.join(self.path, f)) for f in self.zarr_paths]
+        self.zarr_names: list[str] = [x.name for x in self.zarr]
 
     # string representation ---------------------------------------------------
     def __str__(self) -> str:
         nplates = len(self.zarr)
         platenames = ''.join(f'    {i}: {self.zarr[i].name}\n' for i in range(len(self.zarr)))
         return f"FractalZarrSet {self.name}\n  path: {self.path}\n  n_plates: {nplates}\n{platenames}\n"
```

### Comparing `ez_zarr-0.1.5/src/ez_zarr/plotting.py` & `ez_zarr-0.2.0/src/ez_zarr/plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from copy import deepcopy
 import dask.array
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.colors as mcolors
 import matplotlib.patches as patches
 import matplotlib.ticker as ticker
+import importlib
 
 # global variables ------------------------------------------------------------
 plate_layouts = {
     '6well': {'rows': ['A','B'],
               'columns': [str(i+1).zfill(2) for i in range(3)]},
     '24well': {'rows': ['A','B','C','D'],
                'columns': [str(i+1).zfill(2) for i in range(6)]},
@@ -58,23 +59,26 @@
              img_bit: Optional[int]=16) -> Union[dask.array.Array, np.ndarray]:
     """
     Project a 4D or 3D image along z-axis according to desired projection method.
 
     Helper function to conveniently project multi-dimensional images along z-axis according to desired projection method. 
 
     Parameters:
-        im (dask.array or np.ndarray): The array to be projected
+        im (dask.array or np.ndarray): The array to be projected.
         axis (int): The axis on which to perform the projection (typically
-            the z-axis). Unless otherwise specified, it defaults to axis 1 (by convention Fractal outputs have shape ch,z,y,x). Note: if masks are projected, Fractal output have usually shape z,y,x, so use `axis=0` in that case.
-        method (str): The projection method of choice. Available are 
-            'maximum' (default), 'minimum' (typically used for brightfield images), 'sum', 'average'
+            the z-axis). Unless otherwise specified, it defaults to axis 1 (by convention Fractal 
+            outputs have shape ch,z,y,x). Note: if masks are projected, Fractal output have usually 
+            shape z,y,x, so use `axis=0` in that case.
+        method (str): The projection method of choice. Available options are 
+            'maximum' (default), 'minimum' (typically used for brightfield images), 'sum', 'average'.
         keepdims (bool): Should the output array keep the same dimensions 
-            as the input array, or should the z-axis been squeezed (default behaviour of e.g. np.min())
+            as the input array (`True`), or should the z-axis been squeezed 
+            (`False`, default behaviour of e.g. np.min())
         img_bit (int): Is the image 8- or 16-bit? Relevant for 'sum' 
-            projection, where clipping might be necessary
+            projection, where clipping might be necessary.
     
     Returns:
         The input array where the z-axis has been projected according to the method of choice.
     
     Examples:
         Project np.array along z-axis:
 
@@ -152,15 +156,15 @@
             values are calculated on the channel non-zero values, otherwise they
             are directly used as intensities. Values outside of this range will
             be clipped.
 
     Returns:
         An RGB image of shape (y, x, 3), where the third axis corresponds to
             red, green and blue channels. The image is suitable for plotting with
-            `matplotlib.pyplot.imshow` and oriented such that is results in the
+            `matplotlib.pyplot.imshow` and oriented such that it results in the
             same orentiation as when directly plotting a single channel.
 
     Examples:
         Convert an image `img` from (2, y, x) to (y, x, 3), using the
         channels as yellow and blue intensities:
 
         >>> img_rgb = convert_to_rgb(img, ['yellow', 'blue'])   
@@ -204,14 +208,17 @@
 
     return rgb_im
 
 # helper functions to plot image arrays ---------------------------------------
 def plot_image(im: np.ndarray,
                msk: Optional[np.ndarray]=None,
                msk_alpha: float=0.3,
+               show_label_values: bool=False,
+               label_text_colour: str='white',
+               label_fontsize: Union[float, str]='xx-large',
                channels: list[int]=[0],
                channel_colors: list[str]=['white'],
                channel_ranges: list[list[float]]=[[0.01, 0.95]],
                z_projection_method: str='maximum',
                pad_to_yx: list[int]=[0, 0],
                pad_value: int=0,
                axis_style: str='none',
@@ -225,31 +232,40 @@
                fig_width_inch: float=24.0,
                fig_height_inch: float=16.0,
                fig_dpi: int=150,
                fig_style: str='dark_background'):
         """
         Plot an image array, optionally overlaid with a segmentation mask.
          
-        Plot an image (provided as an array with shape (ch,z,y,x) or (ch,y,x))
+        Plot an image (provided as an array with shape (ch,z,y,x), (ch,y,x) or (y,x))
         by summarizing multiple z planes using `z_projection_method` (if needed),
         mapping channels values (in the range of `channel_ranges`) to colors
         (given by `channel_colors`), converting it to an RGB array of shape
         (x,y,3) and plotting it using `matplotlib.pyplot.imshow`.
         If `msk` is provided, it is assumed to contain a compatible segmentation
         mask and will be plotted transparently (controlled by `msk_alpha`)
         on top of the image.
 
         Parameters:
-            im (numpy.ndarray): An array with four (ch,z,y,x) or three (ch,y,x)
-                dimensions with image intensities.
+            im (numpy.ndarray): An array with four (ch,z,y,x), three (ch,y,x)
+                or two (y,x) dimensions with image intensities.
             msk (numpy.ndarray): An optional cooresponding mask array with
-                shape `im.shape[1:]`. If given, label values will be mapped
-                to discrete colors and plotted transparently on top of the image.
+                a shape compatible to `im` (typically without `ch` axis).
+                If given, label values will be mapped to discrete colors
+                and plotted transparently on top of the image.
             msk_alpha (float): A scalar value between 0 (fully transparent)
                 and 1 (solid) defining the transparency of the mask.
+            show_label_values (bool): Whether to show the label values at
+                the centroid of each label.
+            label_text_colour (str): The colour of the label text, if
+                `show_label_values` is True. Ignored otherwise.
+            label_fontsize (float or str): The font size of the label text, if
+                `show_label_values` is True. Ignored otherwise. Values accepted
+                by `matplotlib.axes.Axes.text` are supported, such a the size
+                in points (e.g. `12.5`) or a relative size (e.g. `'xx-large'`).
             channels (list[int]): The image channel(s) to be plotted. For example,
                 to plot the first and third channel of a 4-channel image with
                 shape (4,1,500,600), you can use `channels=[0, 2]`.
             channel_colors (list[str]): A list with python color strings
                 (e.g. 'red') defining the color for each channel in `channels`.
                 For example, to map the selected `channels=[0, 2]` to
                 cyan and magenta, respectively, you can use
@@ -262,57 +278,59 @@
                 channel non-zero values, otherwise they are directly used as
                 intensities. Values outside of this range will be clipped.
             z_projection_method (str): Method for combining multiple z planes.
                 For available methods, see ez_zarr.plotting.zproject
                 (default: 'maximum').
             pad_to_yx (list[int]): If the image or label mask are smaller, pad
                 them by `pad_value` to this total y and x size. 
-            pad_value (int): value to use for contant-value image padding.
+            pad_value (int): Value to use for constant-value image padding.
             axis_style (str): A string scalar defining how to draw the axis. Should
                 be one of 'none' (no axis, the default), 'pixel' (show pixel labels),
                 'frame' (show just a frame around the plot without ticks)
                 or 'micrometer' (show micrometer labels). If `axis_style='micrometer'`,
                 `spacing_yx` is used to convert pixel to micrometer.
             spacing_yx (list[float]): The spacing of pixels in y and x direction,
                 in micrometer, used to convert pixels to micrometer when
                 `axis_style='micrometer'`.
             title (str): String to add as a title on top of the image. If `None`
                 (the default), no title will be added.
-            scalebar_pixel (int): If non-zero, draw a scalebar at the lower right
-                corner of the image of size `scalebar_pixel`.
+            scalebar_pixel (int): If non-zero, draw a scalebar of size `scalebar_pixel`
+                in the corner of the image defined by `scalebar_position`.
             scalebar_color (str): Scalebar color.
             scalebar_position (str): position of the scale bar, one of 'topleft',
                 'topright', 'bottomleft' or 'bottomright'
             scalebar_label (str): If not `None` (default), a string scalar to show
                 as a label for the scale bar.
-            call_show (bool): If true, the call to `matplotlib.pyplot.imshow` is
+            call_show (bool): If `True`, the call to `matplotlib.pyplot.imshow` is
                 embedded between `matplotlib.pyplot.figure` and
                 `matplotlib.pyplot.show`/`matplotlib.pyplot.close` calls.
-                This is the default behaviour and typically used when an indiviual
+                This is the default behaviour and typically used when an individual
                 image should be plotted and displayed. It can be set to `False`
                 if multiple images should be plotted and their arrangement
                 is controlled outside of `plotting.plot_image`. The parameters
-                `fig_width_inch`, `fig_height_inch`, `fig_dpi` and `fig_style`
-                are ignored in that case.
-            fig_width_inch (float): Figure width (inch).
-            fig_height_inch (float): Figure height (inch).
+                `fig_width_inch`, `fig_height_inch` and `fig_dpi` are ignored
+                in that case.
+            fig_width_inch (float): Figure width (in inches).
+            fig_height_inch (float): Figure height (in inches).
             fig_dpi (int): Figure resolution (dots per inch).
             fig_style (str): Style for the figure. Supported are 'brightfield', which
                 is a special mode for single-channel brightfield microscopic images
                 (it will automatically set `channels=[0]`, `channel_colors=['white']`
                 `z_projection_method='minimum'`, `pad_value=1` and `fig_style='default'`),
                 and any other styles that can be passed to `matplotlib.pyplot.style.context`
                 (default: 'dark_background')
 
         Examples:
             Plot the first channel of `img` in gray-scale.
 
             >>> plot_image(img, channels=[0], channel_colors=['white'])
         """
         # digest arguments
+        if im.ndim == 2:
+            im = im[np.newaxis, :]
         ndim = len(im.shape)
         assert ndim == 3 or ndim == 4, (
             f"Unsupported image dimension ({im.shape}), ",
             "should be either (ch,z,y,x) or (ch,y,x)"
         )
         assert msk is None or msk.shape == im.shape[1:], (
             f"`msk` dimension ({msk.shape}) is not compatible with `im` "
@@ -329,14 +347,16 @@
         # adjust parameters for brightfield images
         if fig_style == 'brightfield':
             channels = [0]
             channel_colors = ['white']
             pad_value = 1
             z_projection_method = 'minimum'
             fig_style = 'default'
+            if label_text_colour == 'white':
+                label_text_colour = 'black'
 
         # combine z planes if needed
         if ndim == 4:
             # im: (ch,z,y,x) -> (ch,y,x))
             im = zproject(im=im, method=z_projection_method,
                           axis=1, keepdims=False)
             if not msk is None:
@@ -363,14 +383,25 @@
         def _do_plot():
             plt.imshow(im_rgb)
             if not msk is None and np.max(msk) > 0:
                 plt.imshow(msk,
                            interpolation='none',
                            cmap=get_shuffled_cmap(),
                            alpha=np.multiply(msk_alpha, msk > 0))
+                if show_label_values:
+                    skim = importlib.import_module('skimage.measure')
+                    props = skim.regionprops(msk)
+                    for j in range(len(props)):
+                        plt.text(x=props[j].centroid[1],
+                                 y=props[j].centroid[0],
+                                 s=props[j].label,
+                                 ha='center',
+                                 va='center',
+                                 color=label_text_colour,
+                                 fontsize=label_fontsize)
             if axis_style == 'none':
                 plt.axis('off')
             elif axis_style == 'pixel':
                 pass
             elif axis_style == 'frame':
                 plt.xticks([]) # remove axis ticks
                 plt.yticks([])
```

### Comparing `ez_zarr-0.1.5/src/ez_zarr.egg-info/PKG-INFO` & `ez_zarr-0.2.0/src/ez_zarr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez_zarr
-Version: 0.1.5
+Version: 0.2.0
 Summary: Give easy, high-level access to ome-zarr filesets.
 Author: Silvia Barbiero, Charlotte Soneson, Michael Stadler
 Maintainer-email: Michael Stadler <michael.stadler@fmi.ch>
 License: MIT License
         
         Copyright (c) 2023 Friedrich Miescher Institute for Biomedical Research
         
@@ -47,14 +47,15 @@
 License-File: LICENSE
 Requires-Dist: anndata
 Requires-Dist: dask
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: zarr
 Requires-Dist: matplotlib
+Requires-Dist: scikit-image
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 
 # ez_zarr
 
 ## Goals
@@ -89,17 +90,29 @@
 #   n_wells: 1
 #   n_channels: 2 (some-label-1, some-label-2)
 #   n_pyramid_levels: 3
 #   pyramid_zyx_scalefactor: {'0': array([1. 2. 2.])}
 #   full_resolution_zyx_spacing: [1.0, 0.1625, 0.1625]
 #   segmentations: 
 #   tables (measurements): FOV_ROI_table
+
+from ez_zarr import ome_zarr
+img = ome_zarr.Image('tests/example_data/plate_ones_mip.zarr/B/03/0')
+img
+# Image 0
+#   path: tests/example_data/plate_ones_mip.zarr/B/03/0
+#   n_channels: 2 (some-label-1, some-label-2)
+#   n_pyramid_levels: 3
+#   pyramid_zyx_scalefactor: [1. 2. 2.]
+#   full_resolution_zyx_spacing (micrometer): [1.0, 0.1625, 0.1625]
+#   segmentations: organoids
+#   tables (measurements): FOV_ROI_table
 ```
 
-A more extensive example is available from [here](https://fmicompbio.github.io/ez_zarr/quickstart/), also available as an [ipynb notebook](https://fmicompbio.github.io/ez_zarr/quickstart.ipynb).
+A more extensive example is available from [here](https://fmicompbio.github.io/ez_zarr/getting_started_hcs_wrappers/), also available as an [ipynb notebook](https://fmicompbio.github.io/ez_zarr/getting_started_hcs_wrappers.ipynb).
 
 ## Install
 The release version of `ez_zarr` can be installed using:
 ```
 pip install ez-zarr
 ```
```

### Comparing `ez_zarr-0.1.5/src/ez_zarr.egg-info/SOURCES.txt` & `ez_zarr-0.2.0/src/ez_zarr.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -4,34 +4,40 @@
 mkdocs.yml
 pyproject.toml
 requirements.txt
 .github/workflows/documentation.yaml
 .github/workflows/test_and_deploy.yaml
 docs/doc-requirements.txt
 docs/extra.css
+docs/getting_started_Image.qmd
+docs/getting_started_hcs_wrappers.qmd
 docs/hcs_wrappers.md
 docs/index.md
+docs/ome_zarr.md
 docs/plotting.md
 docs/qmd-requirements.txt
-docs/quickstart.qmd
 docs/testing.md
-docs/vignette.html
+docs/utils.md
 src/ez_zarr/__init__.py
 src/ez_zarr/__main__.py
 src/ez_zarr/_version.py
 src/ez_zarr/hcs_wrappers.py
+src/ez_zarr/ome_zarr.py
 src/ez_zarr/plotting.py
+src/ez_zarr/utils.py
 src/ez_zarr.egg-info/PKG-INFO
 src/ez_zarr.egg-info/SOURCES.txt
 src/ez_zarr.egg-info/dependency_links.txt
 src/ez_zarr.egg-info/entry_points.txt
 src/ez_zarr.egg-info/requires.txt
 src/ez_zarr.egg-info/top_level.txt
 tests/test_hcs_wrappers.py
+tests/test_ome_zarr.py
 tests/test_plotting.py
+tests/test_utils.py
 tests/example_data/generate_example_data.py
 tests/example_data/plate_ones.zarr/.zattrs
 tests/example_data/plate_ones.zarr/.zgroup
 tests/example_data/plate_ones.zarr/B/.zgroup
 tests/example_data/plate_ones.zarr/B/03/.zgroup
 tests/example_data/plate_ones.zarr/B/03/0/.zattrs
 tests/example_data/plate_ones.zarr/B/03/0/.zgroup
```

### Comparing `ez_zarr-0.1.5/tests/example_data/generate_example_data.py` & `ez_zarr-0.2.0/tests/example_data/generate_example_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,38 @@
 import pandas as pd
 import zarr
 from anndata._io.specs import write_elem
 import itertools
 
 from fractal_tasks_core.roi import prepare_FOV_ROI_table
 
+# helper functions
+def generate_circular_mask(shape, radius, center=(0, 0)):
+  """
+  Generates a 2D numpy array with values of 1 in a circular region and zero values everywhere else.
+
+  Args:
+      shape: Tuple representing the shape of the desired array (rows, columns).
+      radius: Float representing the radius of the circle.
+      center: Tuple representing the center coordinates of the circle (default: (0, 0)).
+
+  Returns:
+      A 2D numpy array with the specified shape.
+  """
+  # Create arrays with coordinates
+  y_range = da.arange(shape[0])
+  x_range = da.arange(shape[1])
+  # Reshape for broadcasting
+  y = y_range.reshape((shape[0], 1))
+  x = x_range.reshape((1, shape[1]))
+  # Calculate distance from center
+  dist_from_center = da.sqrt(((x - center[0])**2) + ((y - center[1])**2))
+  mask = da.where(dist_from_center <= radius, 1, 0).astype(np.uint16)
+  return mask
+
 # gloabl parameters
 axes = [
     {"name": "c", "type": "channel"},
     {"name": "z", "type": "space", "unit": "micrometer"},
     {"name": "y", "type": "space", "unit": "micrometer"},
     {"name": "x", "type": "space", "unit": "micrometer"},
 ]
@@ -125,15 +149,15 @@
     }
     with open(f"{zarrurl[i]}{component}.zattrs", "w") as jsonfile:
         json.dump(zattrs, jsonfile, indent=4)
 
     label_org_zattrs = {
         "multiscales": [
             {
-                "axes": axes,
+                "axes": axes[1:],
                 "datasets": [
                     {
                         "path": level,
                         cT: [
                             {
                                 "type": "scale",
                                 "scale": [
@@ -192,17 +216,19 @@
     group_tables = zarr.group(f"{zarrurl[i]}{component}/tables")
     write_elem(group_tables, "FOV_ROI_table", FOV_ROI_table)
     with open(f"{zarrurl[i]}{component}tables/.zattrs", "w") as jsonfile:
         json.dump(table_zattrs, jsonfile, indent=4)
     
     if create_labels[i]:
         group_labels = zarr.group(f"{zarrurl[i]}{component}/labels")
+        xl = generate_circular_mask(x.shape[-2:], radius=100, center=(200,300)) * 1 + generate_circular_mask(x.shape[-2:], radius=200, center=(200,800)) * 2 + generate_circular_mask(x.shape[-2:], radius=300, center=(700,700)) * 3
+        xl = da.expand_dims(xl, axis=0)
         for ind_level in range(num_levels):
             scale = 2**ind_level
-            yl = da.coarsen(np.min, x[0], {1: scale, 2: scale}).rechunk(
+            yl = da.coarsen(np.min, xl, {1: scale, 2: scale}).rechunk(
                 (1, size_y, size_x), balance=True
             )
             yl.to_zarr(
                 zarrurl[i], component=f"{component}/labels/organoids/{ind_level}", dimension_separator="/"
             )
         with open(f"{zarrurl[i]}{component}labels/.zattrs", "w") as jsonfile:
             json.dump(label_zattrs, jsonfile, indent=4)
```

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/.zattrs` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/.zattrs`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/0/0/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/0/0/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/0/0/1` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/0/0/1`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/0/1/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/0/1/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/0/1/1` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/0/1/1`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/1/0/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/1/0/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/1/0/1` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/1/0/1`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/1/1/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/1/1/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/1/1/1` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/1/1/1`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/2/0/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/2/0/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/2/0/1` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/2/0/1`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/2/1/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/2/1/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/0/2/1/1` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/0/2/1/1`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/0/0/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/0/0/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/0/0/1` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/0/0/1`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/0/1/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/0/1/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/0/1/1` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/0/1/1`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/1/0/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/1/0/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/1/0/1` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/1/0/1`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/1/1/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/1/1/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/1/1/1` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/1/1/1`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/2/0/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/2/0/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/2/0/1` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/2/0/1`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/2/1/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/2/1/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/0/1/2/1/1` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/0/1/2/1/1`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/1/0/0/0/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/1/0/0/0/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/1/0/1/0/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/1/0/1/0/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/1/0/2/0/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/1/0/2/0/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/1/1/0/0/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/1/1/0/0/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/1/1/1/0/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/1/1/1/0/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/1/1/2/0/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/1/1/2/0/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/2/0/0/0/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/2/0/0/0/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/2/0/1/0/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/2/0/1/0/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/2/0/2/0/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/2/0/2/0/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/2/1/0/0/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/2/1/0/0/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/2/1/1/0/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/2/1/1/0/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones.zarr/B/03/0/2/1/2/0/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones.zarr/B/03/0/2/1/2/0/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/.zattrs` & `ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/.zattrs`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/0/0/0/0/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/0/0/0/0/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/0/0/0/0/1` & `ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/0/0/0/0/1`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/0/0/0/1/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/0/0/0/1/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/0/0/0/1/1` & `ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/0/0/0/1/1`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/0/1/0/0/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/0/1/0/0/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/0/1/0/0/1` & `ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/0/1/0/0/1`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/0/1/0/1/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/0/1/0/1/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/0/1/0/1/1` & `ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/0/1/0/1/1`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/1/0/0/0/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/1/0/0/0/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/1/1/0/0/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/1/1/0/0/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/2/0/0/0/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/2/0/0/0/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/2/1/0/0/0` & `ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/2/1/0/0/0`

 * *Files identical despite different names*

### Comparing `ez_zarr-0.1.5/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/.zattrs` & `ez_zarr-0.2.0/tests/example_data/plate_ones_mip.zarr/B/03/0/labels/organoids/.zattrs`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666667%*

 * *Differences: {"'multiscales'": "{0: {'axes': {delete: [0]}}}"}*

```diff
@@ -1,16 +1,12 @@
 {
     "multiscales": [
         {
             "axes": [
                 {
-                    "name": "c",
-                    "type": "channel"
-                },
-                {
                     "name": "z",
                     "type": "space",
                     "unit": "micrometer"
                 },
                 {
                     "name": "y",
                     "type": "space",
```

### Comparing `ez_zarr-0.1.5/tests/test_hcs_wrappers.py` & `ez_zarr-0.2.0/tests/test_hcs_wrappers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # for testing, run the following from the project folder:
 #     pip install -e .
-#     pytest --color=yes -v --cov=./ --cov-report=term-missing
+#     pytest --color=yes -v --cov=./src --cov-report=term-missing tests
 
 import pytest
 import anndata as ad
 import json
 import pandas as pd
 import shutil
 import zarr
```

### Comparing `ez_zarr-0.1.5/tests/test_plotting.py` & `ez_zarr-0.2.0/tests/test_plotting.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # for testing, run the following from the project folder:
 #     pip install -e .
-#     pytest --color=yes -v --cov=./ --cov-report=term-missing
+#     pytest --color=yes -v --cov=./src --cov-report=term-missing tests
 
 import pytest
 import numpy as np
 import dask.array
 import matplotlib
 import matplotlib.colors as mcolors
 import matplotlib.pyplot as plt
@@ -134,14 +134,24 @@
                        spacing_yx=[0.325, 0.325])
         # image with masks
         plot_image(im=npa4d, msk=npa3d,
                    channels=[1],
                    channel_colors=['white'],
                    channel_ranges=[[0.01, 0.99]],
                    title='test', call_show=True)
+        plot_image(im=npa4d, msk=npa3d,
+                   channels=[1],
+                   channel_colors=['white'],
+                   channel_ranges=[[0.01, 0.99]],
+                   show_label_values=True,
+                   label_text_colour='red', label_fontsize=12,
+                   title='test', call_show=True)
         # brightfield image
         plot_image(im=npa4d[slice(0,1)],
                    call_show=True,
                    fig_style='brightfield')
+        # 2D image
+        plot_image(im=npa4d[0, 0],
+                   call_show=True)
     plt.savefig(tmpdir.join('output.png'))
     assert True # check if the plotting ran through
```

