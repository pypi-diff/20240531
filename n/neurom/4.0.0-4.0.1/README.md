# Comparing `tmp/neurom-4.0.0.tar.gz` & `tmp/neurom-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurom-4.0.0.tar", last modified: Mon May 27 07:47:53 2024, max compression
+gzip compressed data, was "neurom-4.0.1.tar", last modified: Fri May 31 08:43:56 2024, max compression
```

## Comparing `neurom-4.0.0.tar` & `neurom-4.0.1.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.484569 neurom-4.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.468569 neurom-4.0.0/.binder/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-27 07:47:47.000000 neurom-4.0.0/.binder/postBuild
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 07:47:47.000000 neurom-4.0.0/.binder/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-27 07:47:47.000000 neurom-4.0.0/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-27 07:47:47.000000 neurom-4.0.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-27 07:47:47.000000 neurom-4.0.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.464569 neurom-4.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.468569 neurom-4.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-27 07:47:47.000000 neurom-4.0.0/.github/workflows/mirror-ebrains.yml
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-27 07:47:47.000000 neurom-4.0.0/.github/workflows/publish-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-27 07:47:47.000000 neurom-4.0.0/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-27 07:47:47.000000 neurom-4.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-27 07:47:47.000000 neurom-4.0.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-27 07:47:47.000000 neurom-4.0.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-27 07:47:47.000000 neurom-4.0.0/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-27 07:47:47.000000 neurom-4.0.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-05-27 07:47:47.000000 neurom-4.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-27 07:47:47.000000 neurom-4.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-27 07:47:47.000000 neurom-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-05-27 07:47:53.484569 neurom-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-05-27 07:47:47.000000 neurom-4.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-05-27 07:47:47.000000 neurom-4.0.0/asv.conf.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.464569 neurom-4.0.0/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.472569 neurom-4.0.0/doc/source/
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9481 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/definitions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/developer.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/documentation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/features.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/heterogeneous.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.472569 neurom-4.0.0/doc/source/images/
--rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/images/heterogeneous_neurite.png
--rw-r--r--   0 runner    (1001) docker     (127)    32564 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/images/heterogeneous_neuron.png
--rw-r--r--   0 runner    (1001) docker     (127)    27330 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/images/spherical_coordinates.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/images/spherical_coordinates.tex
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/license.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.472569 neurom-4.0.0/doc/source/logo/
--rw-r--r--   0 runner    (1001) docker     (127)   403060 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/logo/NeuroM.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/migration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/morph_check.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/morph_stats.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/spherical_coordinates.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-27 07:47:47.000000 neurom-4.0.0/doc/source/validation.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.476569 neurom-4.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-27 07:47:47.000000 neurom-4.0.0/examples/boxplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-27 07:47:47.000000 neurom-4.0.0/examples/density_plot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4549 2024-05-27 07:47:47.000000 neurom-4.0.0/examples/end_to_end_distance.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2959 2024-05-27 07:47:47.000000 neurom-4.0.0/examples/extract_distribution.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3713 2024-05-27 07:47:47.000000 neurom-4.0.0/examples/features_graph_table.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6847 2024-05-27 07:47:47.000000 neurom-4.0.0/examples/get_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-05-27 07:47:47.000000 neurom-4.0.0/examples/histogram.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6065 2024-05-27 07:47:47.000000 neurom-4.0.0/examples/iteration_analysis.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3272 2024-05-27 07:47:47.000000 neurom-4.0.0/examples/nl_fst_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2826 2024-05-27 07:47:47.000000 neurom-4.0.0/examples/plot_somas.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4922 2024-05-27 07:47:47.000000 neurom-4.0.0/examples/radius_of_gyration.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2576 2024-05-27 07:47:47.000000 neurom-4.0.0/examples/section_ids.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2869 2024-05-27 07:47:47.000000 neurom-4.0.0/examples/soma_radius_fit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.476569 neurom-4.0.0/neurom/
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.480569 neurom-4.0.0/neurom/apps/
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/apps/annotate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/apps/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.480569 neurom-4.0.0/neurom/apps/config/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/apps/config/morph_check.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/apps/config/morph_stats.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/apps/morph_check.py
--rw-r--r--   0 runner    (1001) docker     (127)    15459 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/apps/morph_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.480569 neurom-4.0.0/neurom/check/
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14277 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/check/morphology_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    12076 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/check/morphtree.py
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/check/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.480569 neurom-4.0.0/neurom/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/core/dataformat.py
--rw-r--r--   0 runner    (1001) docker     (127)    22149 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/core/morphology.py
--rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/core/population.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17859 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/core/soma.py
--rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/core/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.484569 neurom-4.0.0/neurom/features/
--rw-r--r--   0 runner    (1001) docker     (127)    10639 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8420 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/features/bifurcation.py
--rw-r--r--   0 runner    (1001) docker     (127)    30454 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/features/morphology.py
--rw-r--r--   0 runner    (1001) docker     (127)    19575 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/features/neurite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/features/population.py
--rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/features/section.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.484569 neurom-4.0.0/neurom/geom/
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/geom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/geom/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.484569 neurom-4.0.0/neurom/io/
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8679 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/io/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17209 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/morphmath.py
--rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.484569 neurom-4.0.0/neurom/view/
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/view/dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    17707 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/view/matplotlib_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)    16391 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/view/matplotlib_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-05-27 07:47:47.000000 neurom-4.0.0/neurom/view/plotly_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:47:53.484569 neurom-4.0.0/neurom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-05-27 07:47:53.000000 neurom-4.0.0/neurom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-05-27 07:47:53.000000 neurom-4.0.0/neurom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 07:47:53.000000 neurom-4.0.0/neurom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-27 07:47:53.000000 neurom-4.0.0/neurom.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-27 07:47:53.000000 neurom-4.0.0/neurom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-27 07:47:53.000000 neurom-4.0.0/neurom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-27 07:47:47.000000 neurom-4.0.0/pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-27 07:47:47.000000 neurom-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 07:47:53.484569 neurom-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 07:47:47.000000 neurom-4.0.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-27 07:47:47.000000 neurom-4.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:43:56.089984 neurom-4.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:43:56.073984 neurom-4.0.1/.binder/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-31 08:43:50.000000 neurom-4.0.1/.binder/postBuild
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 08:43:50.000000 neurom-4.0.1/.binder/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-31 08:43:50.000000 neurom-4.0.1/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-31 08:43:50.000000 neurom-4.0.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-31 08:43:50.000000 neurom-4.0.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:43:56.065984 neurom-4.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:43:56.073984 neurom-4.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-31 08:43:50.000000 neurom-4.0.1/.github/workflows/mirror-ebrains.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-31 08:43:50.000000 neurom-4.0.1/.github/workflows/publish-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-31 08:43:50.000000 neurom-4.0.1/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-31 08:43:50.000000 neurom-4.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-31 08:43:50.000000 neurom-4.0.1/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-31 08:43:50.000000 neurom-4.0.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-31 08:43:50.000000 neurom-4.0.1/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-31 08:43:50.000000 neurom-4.0.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-05-31 08:43:50.000000 neurom-4.0.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-31 08:43:50.000000 neurom-4.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-31 08:43:50.000000 neurom-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-05-31 08:43:56.089984 neurom-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-05-31 08:43:50.000000 neurom-4.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-05-31 08:43:50.000000 neurom-4.0.1/asv.conf.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:43:56.065984 neurom-4.0.1/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:43:56.077984 neurom-4.0.1/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-31 08:43:50.000000 neurom-4.0.1/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-31 08:43:50.000000 neurom-4.0.1/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-31 08:43:50.000000 neurom-4.0.1/doc/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9481 2024-05-31 08:43:50.000000 neurom-4.0.1/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-31 08:43:50.000000 neurom-4.0.1/doc/source/definitions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-31 08:43:50.000000 neurom-4.0.1/doc/source/developer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-31 08:43:50.000000 neurom-4.0.1/doc/source/documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-31 08:43:50.000000 neurom-4.0.1/doc/source/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-05-31 08:43:50.000000 neurom-4.0.1/doc/source/features.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-05-31 08:43:50.000000 neurom-4.0.1/doc/source/heterogeneous.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:43:56.077984 neurom-4.0.1/doc/source/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-05-31 08:43:50.000000 neurom-4.0.1/doc/source/images/heterogeneous_neurite.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32564 2024-05-31 08:43:50.000000 neurom-4.0.1/doc/source/images/heterogeneous_neuron.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27330 2024-05-31 08:43:50.000000 neurom-4.0.1/doc/source/images/spherical_coordinates.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-31 08:43:50.000000 neurom-4.0.1/doc/source/images/spherical_coordinates.tex
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-31 08:43:50.000000 neurom-4.0.1/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-31 08:43:50.000000 neurom-4.0.1/doc/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-05-31 08:43:50.000000 neurom-4.0.1/doc/source/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:43:56.077984 neurom-4.0.1/doc/source/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)   403060 2024-05-31 08:43:50.000000 neurom-4.0.1/doc/source/logo/NeuroM.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-05-31 08:43:50.000000 neurom-4.0.1/doc/source/migration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-05-31 08:43:50.000000 neurom-4.0.1/doc/source/morph_check.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-05-31 08:43:50.000000 neurom-4.0.1/doc/source/morph_stats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-05-31 08:43:50.000000 neurom-4.0.1/doc/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-31 08:43:50.000000 neurom-4.0.1/doc/source/spherical_coordinates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-31 08:43:50.000000 neurom-4.0.1/doc/source/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-31 08:43:50.000000 neurom-4.0.1/doc/source/validation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:43:56.081984 neurom-4.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-31 08:43:50.000000 neurom-4.0.1/examples/boxplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-31 08:43:50.000000 neurom-4.0.1/examples/density_plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4549 2024-05-31 08:43:50.000000 neurom-4.0.1/examples/end_to_end_distance.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2959 2024-05-31 08:43:50.000000 neurom-4.0.1/examples/extract_distribution.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3713 2024-05-31 08:43:50.000000 neurom-4.0.1/examples/features_graph_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6847 2024-05-31 08:43:50.000000 neurom-4.0.1/examples/get_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-05-31 08:43:50.000000 neurom-4.0.1/examples/histogram.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6065 2024-05-31 08:43:50.000000 neurom-4.0.1/examples/iteration_analysis.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3272 2024-05-31 08:43:50.000000 neurom-4.0.1/examples/nl_fst_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2826 2024-05-31 08:43:50.000000 neurom-4.0.1/examples/plot_somas.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4922 2024-05-31 08:43:50.000000 neurom-4.0.1/examples/radius_of_gyration.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2576 2024-05-31 08:43:50.000000 neurom-4.0.1/examples/section_ids.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2869 2024-05-31 08:43:50.000000 neurom-4.0.1/examples/soma_radius_fit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:43:56.081984 neurom-4.0.1/neurom/
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:43:56.081984 neurom-4.0.1/neurom/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/apps/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/apps/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:43:56.081984 neurom-4.0.1/neurom/apps/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/apps/config/morph_check.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/apps/config/morph_stats.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/apps/morph_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15459 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/apps/morph_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:43:56.085984 neurom-4.0.1/neurom/check/
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14277 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/check/morphology_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12076 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/check/morphtree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/check/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:43:56.085984 neurom-4.0.1/neurom/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/core/dataformat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22295 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/core/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/core/population.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17859 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/core/soma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:43:56.085984 neurom-4.0.1/neurom/features/
+-rw-r--r--   0 runner    (1001) docker     (127)    10639 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/features/bifurcation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30454 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/features/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19575 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/features/neurite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/features/population.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/features/section.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:43:56.085984 neurom-4.0.1/neurom/geom/
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/geom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/geom/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:43:56.085984 neurom-4.0.1/neurom/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8679 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17209 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/morphmath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:43:56.089984 neurom-4.0.1/neurom/view/
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/view/dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17707 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/view/matplotlib_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16391 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/view/matplotlib_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-05-31 08:43:50.000000 neurom-4.0.1/neurom/view/plotly_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:43:56.089984 neurom-4.0.1/neurom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-05-31 08:43:55.000000 neurom-4.0.1/neurom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-05-31 08:43:56.000000 neurom-4.0.1/neurom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 08:43:55.000000 neurom-4.0.1/neurom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-31 08:43:55.000000 neurom-4.0.1/neurom.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-31 08:43:55.000000 neurom-4.0.1/neurom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-31 08:43:55.000000 neurom-4.0.1/neurom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-31 08:43:50.000000 neurom-4.0.1/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-31 08:43:50.000000 neurom-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 08:43:56.089984 neurom-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 08:43:50.000000 neurom-4.0.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-31 08:43:50.000000 neurom-4.0.1/tox.ini
```

### Comparing `neurom-4.0.0/.github/workflows/mirror-ebrains.yml` & `neurom-4.0.1/.github/workflows/mirror-ebrains.yml`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/.github/workflows/publish-sdist.yml` & `neurom-4.0.1/.github/workflows/publish-sdist.yml`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/.github/workflows/run-tox.yml` & `neurom-4.0.1/.github/workflows/run-tox.yml`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/.gitlab-ci.yml` & `neurom-4.0.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/.zenodo.json` & `neurom-4.0.1/.zenodo.json`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/CHANGELOG.rst` & `neurom-4.0.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/LICENSE.txt` & `neurom-4.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/PKG-INFO` & `neurom-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurom
-Version: 4.0.0
+Version: 4.0.1
 Summary: NeuroM: a light-weight neuron morphology analysis package
 Author: Blue Brain Project, EPFL
 License: Copyright (c) 2015-2022 Blue Brain Project/EPFL 
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `neurom-4.0.0/README.md` & `neurom-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/asv.conf.json` & `neurom-4.0.1/asv.conf.json`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/doc/source/api.rst` & `neurom-4.0.1/doc/source/api.rst`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/doc/source/cli.rst` & `neurom-4.0.1/doc/source/cli.rst`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/doc/source/conf.py` & `neurom-4.0.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/doc/source/definitions.rst` & `neurom-4.0.1/doc/source/definitions.rst`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/doc/source/developer.rst` & `neurom-4.0.1/doc/source/developer.rst`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/doc/source/documentation.rst` & `neurom-4.0.1/doc/source/documentation.rst`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/doc/source/examples.rst` & `neurom-4.0.1/doc/source/examples.rst`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/doc/source/features.rst` & `neurom-4.0.1/doc/source/features.rst`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/doc/source/heterogeneous.rst` & `neurom-4.0.1/doc/source/heterogeneous.rst`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/doc/source/images/heterogeneous_neurite.png` & `neurom-4.0.1/doc/source/images/heterogeneous_neurite.png`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/doc/source/images/heterogeneous_neuron.png` & `neurom-4.0.1/doc/source/images/heterogeneous_neuron.png`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/doc/source/images/spherical_coordinates.svg` & `neurom-4.0.1/doc/source/images/spherical_coordinates.svg`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/doc/source/images/spherical_coordinates.tex` & `neurom-4.0.1/doc/source/images/spherical_coordinates.tex`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/doc/source/index.rst` & `neurom-4.0.1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/doc/source/install.rst` & `neurom-4.0.1/doc/source/install.rst`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/doc/source/license.rst` & `neurom-4.0.1/doc/source/license.rst`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/doc/source/logo/NeuroM.jpg` & `neurom-4.0.1/doc/source/logo/NeuroM.jpg`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/doc/source/migration.rst` & `neurom-4.0.1/doc/source/migration.rst`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/doc/source/morph_check.rst` & `neurom-4.0.1/doc/source/morph_check.rst`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/doc/source/morph_stats.rst` & `neurom-4.0.1/doc/source/morph_stats.rst`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/doc/source/quickstart.rst` & `neurom-4.0.1/doc/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/doc/source/spherical_coordinates.rst` & `neurom-4.0.1/doc/source/spherical_coordinates.rst`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/doc/source/tutorial.rst` & `neurom-4.0.1/doc/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/doc/source/validation.rst` & `neurom-4.0.1/doc/source/validation.rst`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/examples/boxplot.py` & `neurom-4.0.1/examples/boxplot.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/examples/density_plot.py` & `neurom-4.0.1/examples/density_plot.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/examples/end_to_end_distance.py` & `neurom-4.0.1/examples/end_to_end_distance.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/examples/extract_distribution.py` & `neurom-4.0.1/examples/extract_distribution.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/examples/features_graph_table.py` & `neurom-4.0.1/examples/features_graph_table.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/examples/get_features.py` & `neurom-4.0.1/examples/get_features.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/examples/histogram.py` & `neurom-4.0.1/examples/histogram.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/examples/iteration_analysis.py` & `neurom-4.0.1/examples/iteration_analysis.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/examples/nl_fst_compat.py` & `neurom-4.0.1/examples/nl_fst_compat.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/examples/plot_somas.py` & `neurom-4.0.1/examples/plot_somas.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/examples/radius_of_gyration.py` & `neurom-4.0.1/examples/radius_of_gyration.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/examples/section_ids.py` & `neurom-4.0.1/examples/section_ids.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/examples/soma_radius_fit.py` & `neurom-4.0.1/examples/soma_radius_fit.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/__init__.py` & `neurom-4.0.1/neurom/__init__.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/apps/__init__.py` & `neurom-4.0.1/neurom/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/apps/annotate.py` & `neurom-4.0.1/neurom/apps/annotate.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/apps/cli.py` & `neurom-4.0.1/neurom/apps/cli.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/apps/config/morph_check.yaml` & `neurom-4.0.1/neurom/apps/config/morph_check.yaml`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/apps/morph_check.py` & `neurom-4.0.1/neurom/apps/morph_check.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/apps/morph_stats.py` & `neurom-4.0.1/neurom/apps/morph_stats.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/check/__init__.py` & `neurom-4.0.1/neurom/check/__init__.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/check/morphology_checks.py` & `neurom-4.0.1/neurom/check/morphology_checks.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/check/morphtree.py` & `neurom-4.0.1/neurom/check/morphtree.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/check/runner.py` & `neurom-4.0.1/neurom/check/runner.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/core/__init__.py` & `neurom-4.0.1/neurom/core/__init__.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/core/dataformat.py` & `neurom-4.0.1/neurom/core/dataformat.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/core/morphology.py` & `neurom-4.0.1/neurom/core/morphology.py`

 * *Files 1% similar despite different names*

```diff
@@ -450,16 +450,18 @@
         if not self._process_subtrees:
             return NeuriteType(self.morphio_root_node.type)
 
         it = self.root_node.ipreorder()
         subtree_types = [next(it).to_morphio().type]
 
         for section in it:
-            if section.type != section.parent.type:
-                subtree_types.append(NeuriteType(section.to_morphio().type))
+            # A subtree can start from a single branch or as a fork of the same type from a parent
+            # with different type.
+            if section.type not in (section.parent.type, subtree_types[-1]):
+                subtree_types.append(section.to_morphio().type)
 
         return subtree_types
 
     @property
     def sections(self):
         """The array of all sections."""
         return list(iter_sections(self))
```

### Comparing `neurom-4.0.0/neurom/core/population.py` & `neurom-4.0.1/neurom/core/population.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/core/soma.py` & `neurom-4.0.1/neurom/core/soma.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/core/types.py` & `neurom-4.0.1/neurom/core/types.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/exceptions.py` & `neurom-4.0.1/neurom/exceptions.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/features/__init__.py` & `neurom-4.0.1/neurom/features/__init__.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/features/bifurcation.py` & `neurom-4.0.1/neurom/features/bifurcation.py`

 * *Files 5% similar despite different names*

```diff
@@ -149,24 +149,24 @@
     The sibling ratio is the ratio between the diameters of the
     smallest and the largest child. It is a real number between
     0 and 1. Method argument allows one to consider mean diameters
     along the child section instead of diameter of the first point.
     """
     _raise_if_not_bifurcation(bif_point)
 
-    if method not in {'first', 'mean'}:
-        raise ValueError('Please provide a valid method for sibling ratio, found %s' % method)
-
     if method == 'first':
         # the first point is the same as the parent last point
         n = bif_point.children[0].points[1, COLS.R]
         m = bif_point.children[1].points[1, COLS.R]
-    if method == 'mean':
+    elif method == 'mean':
         n = neurom.features.section.section_mean_radius(bif_point.children[0])
         m = neurom.features.section.section_mean_radius(bif_point.children[1])
+    else:
+        raise ValueError('Please provide a valid method for sibling ratio, found %s' % method)
+
     return min(n, m) / max(n, m)
 
 
 def diameter_power_relation(bif_point, method='first'):
     """Calculate the diameter power relation at a bifurcation point.
 
     The diameter power relation is defined in https://www.ncbi.nlm.nih.gov/pubmed/18568015
@@ -174,26 +174,26 @@
     This quantity gives an indication of how far the branching is from
     the Rall ratio
 
     diameter_power_relation==1 means perfect Rall ratio
     """
     _raise_if_not_bifurcation(bif_point)
 
-    if method not in {'first', 'mean'}:
-        raise ValueError('Please provide a valid method for sibling ratio, found %s' % method)
-
     if method == 'first':
         # the first point is the same as the parent last point
         d_child = bif_point.points[-1, COLS.R]
         d_child1 = bif_point.children[0].points[1, COLS.R]
         d_child2 = bif_point.children[1].points[1, COLS.R]
-    if method == 'mean':
+    elif method == 'mean':
         d_child = neurom.features.section.section_mean_radius(bif_point)
         d_child1 = neurom.features.section.section_mean_radius(bif_point.children[0])
         d_child2 = neurom.features.section.section_mean_radius(bif_point.children[1])
+    else:
+        raise ValueError('Please provide a valid method for sibling ratio, found %s' % method)
+
     return (d_child / d_child1) ** (1.5) + (d_child / d_child2) ** (1.5)
 
 
 def downstream_pathlength_asymmetry(
     bif_point, normalization_length=1.0, iterator_type=Section.ipreorder
 ):
     """Calculates the downstream pathlength asymmetry at a bifurcation point.
```

### Comparing `neurom-4.0.0/neurom/features/morphology.py` & `neurom-4.0.1/neurom/features/morphology.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/features/neurite.py` & `neurom-4.0.1/neurom/features/neurite.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/features/population.py` & `neurom-4.0.1/neurom/features/population.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/features/section.py` & `neurom-4.0.1/neurom/features/section.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/geom/__init__.py` & `neurom-4.0.1/neurom/geom/__init__.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/geom/transform.py` & `neurom-4.0.1/neurom/geom/transform.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/io/__init__.py` & `neurom-4.0.1/neurom/io/__init__.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/io/utils.py` & `neurom-4.0.1/neurom/io/utils.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/morphmath.py` & `neurom-4.0.1/neurom/morphmath.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/stats.py` & `neurom-4.0.1/neurom/stats.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/utils.py` & `neurom-4.0.1/neurom/utils.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/view/__init__.py` & `neurom-4.0.1/neurom/view/__init__.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/view/dendrogram.py` & `neurom-4.0.1/neurom/view/dendrogram.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/view/matplotlib_impl.py` & `neurom-4.0.1/neurom/view/matplotlib_impl.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/view/matplotlib_utils.py` & `neurom-4.0.1/neurom/view/matplotlib_utils.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom/view/plotly_impl.py` & `neurom-4.0.1/neurom/view/plotly_impl.py`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/neurom.egg-info/PKG-INFO` & `neurom-4.0.1/neurom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurom
-Version: 4.0.0
+Version: 4.0.1
 Summary: NeuroM: a light-weight neuron morphology analysis package
 Author: Blue Brain Project, EPFL
 License: Copyright (c) 2015-2022 Blue Brain Project/EPFL 
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `neurom-4.0.0/neurom.egg-info/SOURCES.txt` & `neurom-4.0.1/neurom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/pylintrc` & `neurom-4.0.1/pylintrc`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/pyproject.toml` & `neurom-4.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `neurom-4.0.0/tox.ini` & `neurom-4.0.1/tox.ini`

 * *Files identical despite different names*

