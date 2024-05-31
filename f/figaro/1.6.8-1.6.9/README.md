# Comparing `tmp/figaro-1.6.8.tar.gz` & `tmp/figaro-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "figaro-1.6.8.tar", last modified: Wed May 29 13:46:36 2024, max compression
+gzip compressed data, was "figaro-1.6.9.tar", last modified: Fri May 31 07:28:58 2024, max compression
```

## Comparing `figaro-1.6.8.tar` & `figaro-1.6.9.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-29 13:46:36.515103 figaro-1.6.8/
--rw-r--r--   0 rinaldi    (503) staff       (20)     1072 2023-11-15 13:14:25.000000 figaro-1.6.8/LICENSE
--rw-r--r--   0 rinaldi    (503) staff       (20)       67 2024-02-10 17:20:30.000000 figaro-1.6.8/MANIFEST.in
--rw-r--r--   0 rinaldi    (503) staff       (20)     6755 2024-05-29 13:46:36.514861 figaro-1.6.8/PKG-INFO
--rw-r--r--   0 rinaldi    (503) staff       (20)     4036 2024-05-26 08:09:23.000000 figaro-1.6.8/README.md
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-29 13:46:36.495303 figaro-1.6.8/docs/
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-29 13:46:36.503625 figaro-1.6.8/docs/source/
--rw-r--r--   0 rinaldi    (503) staff       (20)      332 2024-05-15 12:04:57.000000 figaro-1.6.8/docs/source/api.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      136 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/figaro.cosmology.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      159 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/figaro.credible_regions.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/figaro.cumulative.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/figaro.decorators.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/figaro.diagnostic.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      121 2024-04-24 14:23:00.000000 figaro-1.6.8/docs/source/figaro.load.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      133 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/figaro.marginal.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      130 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/figaro.mixture.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/figaro.montecarlo.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      121 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/figaro.plot.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      121 2024-05-15 12:04:57.000000 figaro-1.6.8/docs/source/figaro.rate.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      308 2024-05-15 12:04:57.000000 figaro-1.6.8/docs/source/figaro.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      136 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/figaro.transform.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      124 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/figaro.utils.rst
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-29 13:46:36.505981 figaro-1.6.8/docs/source/generated/
--rw-r--r--   0 rinaldi    (503) staff       (20)      207 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/generated/figaro.cosmology.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      363 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/generated/figaro.credible_regions.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      231 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/generated/figaro.cumulative.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      263 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/generated/figaro.decorators.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      397 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/generated/figaro.diagnostic.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      267 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/generated/figaro.load.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      211 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/generated/figaro.marginal.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      225 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/generated/figaro.mixture.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      201 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/generated/figaro.montecarlo.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      357 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/generated/figaro.plot.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      385 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/generated/figaro.transform.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      320 2023-11-15 13:14:25.000000 figaro-1.6.8/docs/source/generated/figaro.utils.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)     1928 2024-05-26 08:07:27.000000 figaro-1.6.8/docs/source/index.rst
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-29 13:46:36.511801 figaro-1.6.8/figaro/
--rw-r--r--   0 rinaldi    (503) staff       (20)        0 2024-01-16 16:50:38.000000 figaro-1.6.8/figaro/__init__.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     5033 2024-05-16 07:03:14.000000 figaro-1.6.8/figaro/_likelihood.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     1604 2024-05-16 06:51:29.000000 figaro-1.6.8/figaro/_numba_functions.py
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-29 13:46:36.513492 figaro-1.6.8/figaro/_pipelines/
--rw-r--r--   0 rinaldi    (503) staff       (20)        0 2024-02-10 17:20:30.000000 figaro-1.6.8/figaro/_pipelines/__init__.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    20100 2024-05-15 12:04:57.000000 figaro-1.6.8/figaro/_pipelines/hierarchical_inference.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    23562 2024-05-15 12:04:57.000000 figaro-1.6.8/figaro/_pipelines/par_hierarchical_inference.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    10988 2024-05-15 12:04:57.000000 figaro-1.6.8/figaro/_pipelines/par_probability_density.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     9798 2024-05-15 12:04:57.000000 figaro-1.6.8/figaro/_pipelines/probability_density.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     2822 2024-05-15 12:04:57.000000 figaro-1.6.8/figaro/cosmology.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     7490 2024-02-10 17:20:30.000000 figaro-1.6.8/figaro/credible_regions.py
--rw-r--r--   0 rinaldi    (503) staff       (20)      785 2024-04-22 12:27:42.000000 figaro-1.6.8/figaro/cumulative.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     1364 2024-05-15 12:04:57.000000 figaro-1.6.8/figaro/decorators.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     8385 2024-05-23 11:09:00.000000 figaro-1.6.8/figaro/diagnostic.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     1249 2024-02-06 14:42:23.000000 figaro-1.6.8/figaro/exceptions.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    36516 2024-05-29 13:41:29.000000 figaro-1.6.8/figaro/load.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     6328 2024-05-16 06:52:05.000000 figaro-1.6.8/figaro/marginal.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    55447 2024-05-23 11:09:57.000000 figaro-1.6.8/figaro/mixture.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     2590 2024-02-10 17:20:30.000000 figaro-1.6.8/figaro/montecarlo.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    40609 2024-05-16 06:53:39.000000 figaro-1.6.8/figaro/plot.py
--rw-r--r--   0 rinaldi    (503) staff       (20)      933 2024-04-23 20:48:47.000000 figaro-1.6.8/figaro/plot_settings.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    12100 2024-05-16 06:37:26.000000 figaro-1.6.8/figaro/rate.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     3462 2024-02-13 11:17:19.000000 figaro-1.6.8/figaro/transform.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    16137 2024-05-29 13:43:50.000000 figaro-1.6.8/figaro/utils.py
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-29 13:46:36.514535 figaro-1.6.8/figaro.egg-info/
--rw-r--r--   0 rinaldi    (503) staff       (20)     6755 2024-05-29 13:46:36.000000 figaro-1.6.8/figaro.egg-info/PKG-INFO
--rw-r--r--   0 rinaldi    (503) staff       (20)     1809 2024-05-29 13:46:36.000000 figaro-1.6.8/figaro.egg-info/SOURCES.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)        1 2024-05-29 13:46:36.000000 figaro-1.6.8/figaro.egg-info/dependency_links.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)      290 2024-05-29 13:46:36.000000 figaro-1.6.8/figaro.egg-info/entry_points.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)       76 2024-05-29 13:46:36.000000 figaro-1.6.8/figaro.egg-info/requires.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)        7 2024-05-29 13:46:36.000000 figaro-1.6.8/figaro.egg-info/top_level.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)     1988 2024-05-29 13:45:58.000000 figaro-1.6.8/pyproject.toml
--rw-r--r--   0 rinaldi    (503) staff       (20)       38 2024-05-29 13:46:36.515149 figaro-1.6.8/setup.cfg
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-29 13:46:36.513662 figaro-1.6.8/test/
--rw-r--r--   0 rinaldi    (503) staff       (20)     2577 2024-05-15 12:04:57.000000 figaro-1.6.8/test/test_figaro.py
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-31 07:28:58.749030 figaro-1.6.9/
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1072 2023-11-15 13:14:25.000000 figaro-1.6.9/LICENSE
+-rw-r--r--   0 rinaldi    (503) staff       (20)       67 2024-02-10 17:20:30.000000 figaro-1.6.9/MANIFEST.in
+-rw-r--r--   0 rinaldi    (503) staff       (20)     6755 2024-05-31 07:28:58.748774 figaro-1.6.9/PKG-INFO
+-rw-r--r--   0 rinaldi    (503) staff       (20)     4036 2024-05-26 08:09:23.000000 figaro-1.6.9/README.md
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-31 07:28:58.732500 figaro-1.6.9/docs/
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-31 07:28:58.738110 figaro-1.6.9/docs/source/
+-rw-r--r--   0 rinaldi    (503) staff       (20)      332 2024-05-15 12:04:57.000000 figaro-1.6.9/docs/source/api.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      136 2023-11-15 13:14:25.000000 figaro-1.6.9/docs/source/figaro.cosmology.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      159 2023-11-15 13:14:25.000000 figaro-1.6.9/docs/source/figaro.credible_regions.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.9/docs/source/figaro.cumulative.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.9/docs/source/figaro.decorators.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.9/docs/source/figaro.diagnostic.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      121 2024-04-24 14:23:00.000000 figaro-1.6.9/docs/source/figaro.load.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      133 2023-11-15 13:14:25.000000 figaro-1.6.9/docs/source/figaro.marginal.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      130 2023-11-15 13:14:25.000000 figaro-1.6.9/docs/source/figaro.mixture.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.9/docs/source/figaro.montecarlo.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      121 2023-11-15 13:14:25.000000 figaro-1.6.9/docs/source/figaro.plot.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      121 2024-05-15 12:04:57.000000 figaro-1.6.9/docs/source/figaro.rate.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      308 2024-05-15 12:04:57.000000 figaro-1.6.9/docs/source/figaro.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      136 2023-11-15 13:14:25.000000 figaro-1.6.9/docs/source/figaro.transform.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      124 2023-11-15 13:14:25.000000 figaro-1.6.9/docs/source/figaro.utils.rst
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-31 07:28:58.740397 figaro-1.6.9/docs/source/generated/
+-rw-r--r--   0 rinaldi    (503) staff       (20)      207 2023-11-15 13:14:25.000000 figaro-1.6.9/docs/source/generated/figaro.cosmology.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      363 2023-11-15 13:14:25.000000 figaro-1.6.9/docs/source/generated/figaro.credible_regions.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      231 2023-11-15 13:14:25.000000 figaro-1.6.9/docs/source/generated/figaro.cumulative.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      263 2023-11-15 13:14:25.000000 figaro-1.6.9/docs/source/generated/figaro.decorators.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      397 2023-11-15 13:14:25.000000 figaro-1.6.9/docs/source/generated/figaro.diagnostic.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      267 2023-11-15 13:14:25.000000 figaro-1.6.9/docs/source/generated/figaro.load.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      211 2023-11-15 13:14:25.000000 figaro-1.6.9/docs/source/generated/figaro.marginal.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      225 2023-11-15 13:14:25.000000 figaro-1.6.9/docs/source/generated/figaro.mixture.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      201 2023-11-15 13:14:25.000000 figaro-1.6.9/docs/source/generated/figaro.montecarlo.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      357 2023-11-15 13:14:25.000000 figaro-1.6.9/docs/source/generated/figaro.plot.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      385 2023-11-15 13:14:25.000000 figaro-1.6.9/docs/source/generated/figaro.transform.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      320 2023-11-15 13:14:25.000000 figaro-1.6.9/docs/source/generated/figaro.utils.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1928 2024-05-26 08:07:27.000000 figaro-1.6.9/docs/source/index.rst
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-31 07:28:58.746258 figaro-1.6.9/figaro/
+-rw-r--r--   0 rinaldi    (503) staff       (20)        0 2024-01-16 16:50:38.000000 figaro-1.6.9/figaro/__init__.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     5033 2024-05-30 09:51:22.000000 figaro-1.6.9/figaro/_likelihood.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1604 2024-05-16 06:51:29.000000 figaro-1.6.9/figaro/_numba_functions.py
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-31 07:28:58.747992 figaro-1.6.9/figaro/_pipelines/
+-rw-r--r--   0 rinaldi    (503) staff       (20)        0 2024-02-10 17:20:30.000000 figaro-1.6.9/figaro/_pipelines/__init__.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    20100 2024-05-15 12:04:57.000000 figaro-1.6.9/figaro/_pipelines/hierarchical_inference.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    23562 2024-05-15 12:04:57.000000 figaro-1.6.9/figaro/_pipelines/par_hierarchical_inference.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    10988 2024-05-15 12:04:57.000000 figaro-1.6.9/figaro/_pipelines/par_probability_density.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     9798 2024-05-15 12:04:57.000000 figaro-1.6.9/figaro/_pipelines/probability_density.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     2822 2024-05-15 12:04:57.000000 figaro-1.6.9/figaro/cosmology.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     7490 2024-02-10 17:20:30.000000 figaro-1.6.9/figaro/credible_regions.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)      785 2024-04-22 12:27:42.000000 figaro-1.6.9/figaro/cumulative.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1364 2024-05-15 12:04:57.000000 figaro-1.6.9/figaro/decorators.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     8385 2024-05-23 11:09:00.000000 figaro-1.6.9/figaro/diagnostic.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1249 2024-02-06 14:42:23.000000 figaro-1.6.9/figaro/exceptions.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    36516 2024-05-29 13:41:29.000000 figaro-1.6.9/figaro/load.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     6328 2024-05-16 06:52:05.000000 figaro-1.6.9/figaro/marginal.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    55457 2024-05-31 07:19:59.000000 figaro-1.6.9/figaro/mixture.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     2590 2024-02-10 17:20:30.000000 figaro-1.6.9/figaro/montecarlo.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    40609 2024-05-16 06:53:39.000000 figaro-1.6.9/figaro/plot.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)      933 2024-04-23 20:48:47.000000 figaro-1.6.9/figaro/plot_settings.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    12100 2024-05-16 06:37:26.000000 figaro-1.6.9/figaro/rate.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     3462 2024-02-13 11:17:19.000000 figaro-1.6.9/figaro/transform.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    16137 2024-05-29 13:47:17.000000 figaro-1.6.9/figaro/utils.py
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-31 07:28:58.748466 figaro-1.6.9/figaro.egg-info/
+-rw-r--r--   0 rinaldi    (503) staff       (20)     6755 2024-05-31 07:28:58.000000 figaro-1.6.9/figaro.egg-info/PKG-INFO
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1809 2024-05-31 07:28:58.000000 figaro-1.6.9/figaro.egg-info/SOURCES.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)        1 2024-05-31 07:28:58.000000 figaro-1.6.9/figaro.egg-info/dependency_links.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)      290 2024-05-31 07:28:58.000000 figaro-1.6.9/figaro.egg-info/entry_points.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)       76 2024-05-31 07:28:58.000000 figaro-1.6.9/figaro.egg-info/requires.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)        7 2024-05-31 07:28:58.000000 figaro-1.6.9/figaro.egg-info/top_level.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1988 2024-05-31 07:22:01.000000 figaro-1.6.9/pyproject.toml
+-rw-r--r--   0 rinaldi    (503) staff       (20)       38 2024-05-31 07:28:58.749081 figaro-1.6.9/setup.cfg
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-05-31 07:28:58.748162 figaro-1.6.9/test/
+-rw-r--r--   0 rinaldi    (503) staff       (20)     2577 2024-05-15 12:04:57.000000 figaro-1.6.9/test/test_figaro.py
```

### Comparing `figaro-1.6.8/LICENSE` & `figaro-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `figaro-1.6.8/PKG-INFO` & `figaro-1.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: figaro
-Version: 1.6.8
+Version: 1.6.9
 Summary: FIGARO: Fast Inference for GW Astronomy, Research & Observations
 Author-email: Stefano Rinaldi <stefano.rinaldi@uni-heidelberg.de>, Walter Del Pozzo <walter.delpozzo@unipi.it>, Daniele Sanfratello <daniele.sanfratello@studenti.unipi.it>
 License: MIT License
         
         Copyright (c) 2022 Stefano Rinaldi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `figaro-1.6.8/README.md` & `figaro-1.6.9/README.md`

 * *Files identical despite different names*

### Comparing `figaro-1.6.8/docs/source/index.rst` & `figaro-1.6.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `figaro-1.6.8/figaro/_likelihood.py` & `figaro-1.6.9/figaro/_likelihood.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.8/figaro/_numba_functions.py` & `figaro-1.6.9/figaro/_numba_functions.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.8/figaro/_pipelines/hierarchical_inference.py` & `figaro-1.6.9/figaro/_pipelines/hierarchical_inference.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.8/figaro/_pipelines/par_hierarchical_inference.py` & `figaro-1.6.9/figaro/_pipelines/par_hierarchical_inference.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.8/figaro/_pipelines/par_probability_density.py` & `figaro-1.6.9/figaro/_pipelines/par_probability_density.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.8/figaro/_pipelines/probability_density.py` & `figaro-1.6.9/figaro/_pipelines/probability_density.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.8/figaro/cosmology.py` & `figaro-1.6.9/figaro/cosmology.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.8/figaro/credible_regions.py` & `figaro-1.6.9/figaro/credible_regions.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.8/figaro/cumulative.py` & `figaro-1.6.9/figaro/cumulative.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.8/figaro/decorators.py` & `figaro-1.6.9/figaro/decorators.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.8/figaro/diagnostic.py` & `figaro-1.6.9/figaro/diagnostic.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.8/figaro/exceptions.py` & `figaro-1.6.9/figaro/exceptions.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.8/figaro/load.py` & `figaro-1.6.9/figaro/load.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.8/figaro/marginal.py` & `figaro-1.6.9/figaro/marginal.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.8/figaro/mixture.py` & `figaro-1.6.9/figaro/mixture.py`

 * *Files 0% similar despite different names*

```diff
@@ -1408,15 +1408,15 @@
             alpha_factor       = self.compute_alpha_factor()
             N_pts              = self.w*self.n_pts/alpha_factor
             self.log_w, self.w = log_w, w
         else:
             alpha_factor = 1.
             N_pts = np.exp(N_pts)
         w = dirichlet(N_pts+self.alpha/self.n_cl).rvs()[0]
-        return mixture(np.array([comp.mu for comp in np.array(self.mixture)[idx]]), np.array([comp.sigma for comp in np.array(self.mixture)[idx]]), w, self.bounds, self.dim, (np.array(self.N_list) > 0).sum(), self.n_pts, self.alpha, probit = self.probit, make_comp = make_comp, alpha_factor = alpha_factor)
+        return mixture(np.array([comp.mu.flatten() for comp in np.array(self.mixture)[idx]]), np.array([comp.sigma for comp in np.array(self.mixture)[idx]]), w, self.bounds, self.dim, (np.array(self.N_list) > 0).sum(), self.n_pts, self.alpha, probit = self.probit, make_comp = make_comp, alpha_factor = alpha_factor)
     
     def compute_alpha_factor(self):
         """
         Compute the integral \\int pdet(theta)p(theta|lambda) dtheta conditioned on the specific DPGMM parameters
         
         Returns:
             double: value of the integral
```

### Comparing `figaro-1.6.8/figaro/montecarlo.py` & `figaro-1.6.9/figaro/montecarlo.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.8/figaro/plot.py` & `figaro-1.6.9/figaro/plot.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.8/figaro/plot_settings.py` & `figaro-1.6.9/figaro/plot_settings.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.8/figaro/rate.py` & `figaro-1.6.9/figaro/rate.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.8/figaro/transform.py` & `figaro-1.6.9/figaro/transform.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.8/figaro/utils.py` & `figaro-1.6.9/figaro/utils.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.8/figaro.egg-info/PKG-INFO` & `figaro-1.6.9/figaro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: figaro
-Version: 1.6.8
+Version: 1.6.9
 Summary: FIGARO: Fast Inference for GW Astronomy, Research & Observations
 Author-email: Stefano Rinaldi <stefano.rinaldi@uni-heidelberg.de>, Walter Del Pozzo <walter.delpozzo@unipi.it>, Daniele Sanfratello <daniele.sanfratello@studenti.unipi.it>
 License: MIT License
         
         Copyright (c) 2022 Stefano Rinaldi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `figaro-1.6.8/figaro.egg-info/SOURCES.txt` & `figaro-1.6.9/figaro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `figaro-1.6.8/pyproject.toml` & `figaro-1.6.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 [tool.setuptools]
 packages = ['figaro', 'figaro._pipelines']
 
 [project]
 name = 'figaro'
 description = 'FIGARO: Fast Inference for GW Astronomy, Research & Observations'
-version = '1.6.8'
+version = '1.6.9'
 requires-python = '< 3.12'
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 keywords = ['DPGMM', 'figaro', 'hierarchical', 'inference', 'HDPGMM']
 authors = [
   {name = "Stefano Rinaldi", email = "stefano.rinaldi@uni-heidelberg.de"},
   {name = "Walter Del Pozzo", email = "walter.delpozzo@unipi.it"},
```

### Comparing `figaro-1.6.8/test/test_figaro.py` & `figaro-1.6.9/test/test_figaro.py`

 * *Files identical despite different names*

