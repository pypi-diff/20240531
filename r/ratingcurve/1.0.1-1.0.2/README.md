# Comparing `tmp/ratingcurve-1.0.1.tar.gz` & `tmp/ratingcurve-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ratingcurve-1.0.1.tar", last modified: Wed Mar  6 21:42:50 2024, max compression
+gzip compressed data, was "ratingcurve-1.0.2.tar", last modified: Thu May 30 23:12:49 2024, max compression
```

## Comparing `ratingcurve-1.0.1.tar` & `ratingcurve-1.0.2.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:42:50.845040 ratingcurve-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:42:50.837040 ratingcurve-1.0.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/.devcontainer/noop.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:42:50.833040 ratingcurve-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:42:50.837040 ratingcurve-1.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/.github/ISSUE_TEMPLATE/review-checklist.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:42:50.837040 ratingcurve-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/.github/workflows/deploy-book.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     8788 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/DISCLAIMER.md
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-03-06 21:42:50.845040 ratingcurve-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/code.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:42:50.837040 ratingcurve-1.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/docs/_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/docs/_toc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/docs/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:42:50.837040 ratingcurve-1.0.1/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    29183 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/docs/assets/green-channel-rating-plot.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:42:50.837040 ratingcurve-1.0.1/docs/meta/
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/docs/meta/background.md
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/docs/meta/implementation.md
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/docs/meta/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/docs/meta/intro.md
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/docs/meta/troubleshooting.md
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/docs/meta/tutorials.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:42:50.841040 ratingcurve-1.0.1/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/docs/notebooks/getting-started-tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/docs/notebooks/model-selection-tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9034 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/docs/notebooks/segmented-power-law-tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/docs/notebooks/spline-tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/docs/references.bib
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/docs/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:42:50.841040 ratingcurve-1.0.1/ratingcurve/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/ratingcurve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-06 21:42:50.000000 ratingcurve-1.0.1/ratingcurve/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:42:50.845040 ratingcurve-1.0.1/ratingcurve/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/ratingcurve/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/ratingcurve/data/chalk_artificial.csv
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/ratingcurve/data/chalk_artificial.md
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/ratingcurve/data/co_channel.csv
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/ratingcurve/data/co_channel.md
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/ratingcurve/data/green_channel.csv
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/ratingcurve/data/green_channel.md
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/ratingcurve/data/isere.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/ratingcurve/data/isere.md
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/ratingcurve/data/mahurangi_artificial.csv
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/ratingcurve/data/mahurangi_artificial.md
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/ratingcurve/data/nordura.csv
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/ratingcurve/data/nordura.md
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/ratingcurve/data/provo_natural.csv
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/ratingcurve/data/provo_natural.md
--rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/ratingcurve/data/simulated_rating.csv
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/ratingcurve/data/simulated_rating.md
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/ratingcurve/data/skajalfandafljot.csv
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/ratingcurve/data/skajalfandafljot.md
--rw-r--r--   0 runner    (1001) docker     (127)    15604 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/ratingcurve/experimental_ratings.py
--rw-r--r--   0 runner    (1001) docker     (127)    26551 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/ratingcurve/model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7232 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/ratingcurve/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    21172 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/ratingcurve/ratingmodel_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    13677 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/ratingcurve/ratings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:42:50.845040 ratingcurve-1.0.1/ratingcurve/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/ratingcurve/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/ratingcurve/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/ratingcurve/tests/test_fitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/ratingcurve/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/ratingcurve/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:42:50.845040 ratingcurve-1.0.1/ratingcurve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-03-06 21:42:50.000000 ratingcurve-1.0.1/ratingcurve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-03-06 21:42:50.000000 ratingcurve-1.0.1/ratingcurve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 21:42:50.000000 ratingcurve-1.0.1/ratingcurve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-06 21:42:50.000000 ratingcurve-1.0.1/ratingcurve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-06 21:42:50.000000 ratingcurve-1.0.1/ratingcurve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 21:42:50.845040 ratingcurve-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-06 21:42:34.000000 ratingcurve-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:12:49.607356 ratingcurve-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:12:49.595356 ratingcurve-1.0.2/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/.devcontainer/noop.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:12:49.591356 ratingcurve-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:12:49.595356 ratingcurve-1.0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/.github/ISSUE_TEMPLATE/review-checklist.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:12:49.595356 ratingcurve-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/.github/workflows/deploy-book.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     8788 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/DISCLAIMER.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-05-30 23:12:49.607356 ratingcurve-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/code.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:12:49.599356 ratingcurve-1.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/docs/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/docs/_toc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/docs/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:12:49.599356 ratingcurve-1.0.2/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    29183 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/docs/assets/green-channel-rating-plot.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:12:49.599356 ratingcurve-1.0.2/docs/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/docs/meta/background.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/docs/meta/implementation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/docs/meta/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/docs/meta/intro.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/docs/meta/troubleshooting.md
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/docs/meta/tutorials.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:12:49.599356 ratingcurve-1.0.2/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/docs/notebooks/getting-started-tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/docs/notebooks/model-selection-tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9034 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/docs/notebooks/segmented-power-law-tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/docs/notebooks/spline-tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/docs/references.bib
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/docs/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:12:49.599356 ratingcurve-1.0.2/ratingcurve/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/ratingcurve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-30 23:12:49.000000 ratingcurve-1.0.2/ratingcurve/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:12:49.603356 ratingcurve-1.0.2/ratingcurve/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/ratingcurve/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/ratingcurve/data/chalk_artificial.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/ratingcurve/data/chalk_artificial.md
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/ratingcurve/data/co_channel.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/ratingcurve/data/co_channel.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/ratingcurve/data/green_channel.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/ratingcurve/data/green_channel.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/ratingcurve/data/isere.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/ratingcurve/data/isere.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/ratingcurve/data/mahurangi_artificial.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/ratingcurve/data/mahurangi_artificial.md
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/ratingcurve/data/nordura.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/ratingcurve/data/nordura.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/ratingcurve/data/provo_natural.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/ratingcurve/data/provo_natural.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/ratingcurve/data/simulated_rating.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/ratingcurve/data/simulated_rating.md
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/ratingcurve/data/skajalfandafljot.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/ratingcurve/data/skajalfandafljot.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15604 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/ratingcurve/experimental_ratings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26551 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/ratingcurve/model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7232 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/ratingcurve/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21172 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/ratingcurve/ratingmodel_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13677 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/ratingcurve/ratings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:12:49.603356 ratingcurve-1.0.2/ratingcurve/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/ratingcurve/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/ratingcurve/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/ratingcurve/tests/test_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/ratingcurve/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/ratingcurve/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:12:49.607356 ratingcurve-1.0.2/ratingcurve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-05-30 23:12:49.000000 ratingcurve-1.0.2/ratingcurve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-30 23:12:49.000000 ratingcurve-1.0.2/ratingcurve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 23:12:49.000000 ratingcurve-1.0.2/ratingcurve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 23:12:49.000000 ratingcurve-1.0.2/ratingcurve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 23:12:49.000000 ratingcurve-1.0.2/ratingcurve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 23:12:49.607356 ratingcurve-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-30 23:12:33.000000 ratingcurve-1.0.2/setup.py
```

### Comparing `ratingcurve-1.0.1/.devcontainer/Dockerfile` & `ratingcurve-1.0.2/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/.devcontainer/devcontainer.json` & `ratingcurve-1.0.2/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/.github/ISSUE_TEMPLATE/feature_request.md` & `ratingcurve-1.0.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/.github/ISSUE_TEMPLATE/review-checklist.md` & `ratingcurve-1.0.2/.github/ISSUE_TEMPLATE/review-checklist.md`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/.github/workflows/deploy-book.yml` & `ratingcurve-1.0.2/.github/workflows/deploy-book.yml`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/.github/workflows/python-package.yml` & `ratingcurve-1.0.2/.github/workflows/python-package.yml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
   build:
 
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest]
-        python-version: ["3.9", "3.10", "3.11"]
+        python-version: ["3.10", "3.11", "3.12"]
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
```

### Comparing `ratingcurve-1.0.1/.github/workflows/python-publish.yml` & `ratingcurve-1.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/.gitignore` & `ratingcurve-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/CONTRIBUTING.md` & `ratingcurve-1.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/DISCLAIMER.md` & `ratingcurve-1.0.2/DISCLAIMER.md`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/LICENSE.md` & `ratingcurve-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/PKG-INFO` & `ratingcurve-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratingcurve
-Version: 1.0.1
+Version: 1.0.2
 Summary: A library for fitting multi-segment stage-discharge rating curves.
 Maintainer-email: Timothy Hodson <thodson@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, this project is in the public domain in the United
         States because it contains materials that originally came from the United
@@ -50,15 +50,15 @@
         
         [1]: https://creativecommons.org/publicdomain/zero/1.0/legalcode
         
 Project-URL: homepage, https://github.com/thodson-usgs/ratingcurve
 Project-URL: repository, https://github.com/thodson-usgs/ratingcurve.git
 Keywords: USGS,streamflow,rating curve
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: pymc>=5.0.0
 Requires-Dist: patsy
 Provides-Extra: test
 Requires-Dist: pytest>5.0.0; extra == "test"
 Requires-Dist: pytest-cov[all]; extra == "test"
@@ -127,7 +127,25 @@
 ## Disclaimer
 
 This software is preliminary or provisional and is subject to revision. 
 It is being provided to meet the need for timely best science.
 The software has not received final approval by the U.S. Geological Survey (USGS).
 No warranty, expressed or implied, is made by the USGS or the U.S. Government as to the functionality of the software and related material nor shall the fact of release constitute any such warranty. 
 The software is provided on the condition that neither the USGS nor the U.S. Government shall be held liable for any damages resulting from the authorized or unauthorized use of the software.
+
+## Citation
+Hodson, T.O., Doore, K.J., Kenney, T.A., Over T.M., and Yeheyis, M.B., 2024, Ratingcurve: A Python Package for Fitting Streamflow Rating Curves, Hydrology 11, no. 2: 14. https://doi.org/10.3390/hydrology11020014
+
+```
+@Article{hydrology11020014,
+AUTHOR = {Hodson, Timothy O. and Doore, Keith J. and Kenney, Terry A. and Over, Thomas M. and Yeheyis, Muluken B.},
+TITLE = {Ratingcurve: A Python Package for Fitting Streamflow Rating Curves},
+JOURNAL = {Hydrology},
+VOLUME = {11},
+YEAR = {2024},
+NUMBER = {2},
+ARTICLE-NUMBER = {14},
+URL = {https://www.mdpi.com/2306-5338/11/2/14},
+ISSN = {2306-5338},
+DOI = {10.3390/hydrology11020014}
+}
+```
```

### Comparing `ratingcurve-1.0.1/README.md` & `ratingcurve-1.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -62,7 +62,25 @@
 ## Disclaimer
 
 This software is preliminary or provisional and is subject to revision. 
 It is being provided to meet the need for timely best science.
 The software has not received final approval by the U.S. Geological Survey (USGS).
 No warranty, expressed or implied, is made by the USGS or the U.S. Government as to the functionality of the software and related material nor shall the fact of release constitute any such warranty. 
 The software is provided on the condition that neither the USGS nor the U.S. Government shall be held liable for any damages resulting from the authorized or unauthorized use of the software.
+
+## Citation
+Hodson, T.O., Doore, K.J., Kenney, T.A., Over T.M., and Yeheyis, M.B., 2024, Ratingcurve: A Python Package for Fitting Streamflow Rating Curves, Hydrology 11, no. 2: 14. https://doi.org/10.3390/hydrology11020014
+
+```
+@Article{hydrology11020014,
+AUTHOR = {Hodson, Timothy O. and Doore, Keith J. and Kenney, Terry A. and Over, Thomas M. and Yeheyis, Muluken B.},
+TITLE = {Ratingcurve: A Python Package for Fitting Streamflow Rating Curves},
+JOURNAL = {Hydrology},
+VOLUME = {11},
+YEAR = {2024},
+NUMBER = {2},
+ARTICLE-NUMBER = {14},
+URL = {https://www.mdpi.com/2306-5338/11/2/14},
+ISSN = {2306-5338},
+DOI = {10.3390/hydrology11020014}
+}
+```
```

### Comparing `ratingcurve-1.0.1/code.json` & `ratingcurve-1.0.2/code.json`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/docs/_config.yml` & `ratingcurve-1.0.2/docs/_config.yml`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/docs/assets/green-channel-rating-plot.png` & `ratingcurve-1.0.2/docs/assets/green-channel-rating-plot.png`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/docs/meta/background.md` & `ratingcurve-1.0.2/docs/meta/background.md`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/docs/meta/implementation.md` & `ratingcurve-1.0.2/docs/meta/implementation.md`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 similar to how different controls become active as stage increases in the channel.
 Once stage rises beyond the range of a particular control, that control is "drowned out" and its flow ceases to increase with stage.
 Our parameterization is simpler though less physical.
 As stage increases, new segments are activated, but their effect never drowns out:
 each successive $w_i$ term makes cumulative adjustments to the base slope $w_1$.
 
 The current priors and optimizer settings are documented in the package;
-in general, they do not need to modified.
+in general, they do not need to be modified.
 Besides selecting the number of segments, the user can specify a prior distribution on the breakpoints.
 The default assumes the breakpoints are uniformly distributed, which works well for general use.
 Alternatively, the user can specify the approximate location of each breakpoint using a normal distribution,
 like if they had other evidence that a breakpoint occurred at a particular stage. 
 With the normal prior, the user specifies the expected stage for each breakpoint and their uncertainty about it.
 
 Like {cite:t}`Reitan_2008`, we assume $\epsilon$ is normally distributed with mean zero and variance $\sigma^2$, $\epsilon \sim N(0, \sigma^2)$.
```

### Comparing `ratingcurve-1.0.1/docs/meta/installation.md` & `ratingcurve-1.0.2/docs/meta/installation.md`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/docs/meta/intro.md` & `ratingcurve-1.0.2/docs/meta/intro.md`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/docs/meta/troubleshooting.md` & `ratingcurve-1.0.2/docs/meta/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/docs/notebooks/getting-started-tutorial.ipynb` & `ratingcurve-1.0.2/docs/notebooks/getting-started-tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/docs/notebooks/model-selection-tutorial.ipynb` & `ratingcurve-1.0.2/docs/notebooks/model-selection-tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/docs/notebooks/segmented-power-law-tutorial.ipynb` & `ratingcurve-1.0.2/docs/notebooks/segmented-power-law-tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/docs/notebooks/spline-tutorial.ipynb` & `ratingcurve-1.0.2/docs/notebooks/spline-tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/docs/references.bib` & `ratingcurve-1.0.2/docs/references.bib`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/pyproject.toml` & `ratingcurve-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=45", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ratingcurve"
 description = "A library for fitting multi-segment stage-discharge rating curves."
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 keywords = ["USGS", "streamflow", "rating curve"]
 license = {file = "LICENSE.md"}
 maintainers = [
   {name = "Timothy Hodson", email = "thodson@usgs.gov"},
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `ratingcurve-1.0.1/ratingcurve/data/__init__.py` & `ratingcurve-1.0.2/ratingcurve/data/__init__.py`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/ratingcurve/data/chalk_artificial.csv` & `ratingcurve-1.0.2/ratingcurve/data/chalk_artificial.csv`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/ratingcurve/data/chalk_artificial.md` & `ratingcurve-1.0.2/ratingcurve/data/chalk_artificial.md`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/ratingcurve/data/co_channel.csv` & `ratingcurve-1.0.2/ratingcurve/data/co_channel.csv`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/ratingcurve/data/green_channel.csv` & `ratingcurve-1.0.2/ratingcurve/data/green_channel.csv`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/ratingcurve/data/green_channel.md` & `ratingcurve-1.0.2/ratingcurve/data/green_channel.md`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/ratingcurve/data/isere.csv` & `ratingcurve-1.0.2/ratingcurve/data/isere.csv`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/ratingcurve/data/isere.md` & `ratingcurve-1.0.2/ratingcurve/data/isere.md`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/ratingcurve/data/mahurangi_artificial.csv` & `ratingcurve-1.0.2/ratingcurve/data/mahurangi_artificial.csv`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/ratingcurve/data/mahurangi_artificial.md` & `ratingcurve-1.0.2/ratingcurve/data/mahurangi_artificial.md`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/ratingcurve/data/nordura.md` & `ratingcurve-1.0.2/ratingcurve/data/nordura.md`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/ratingcurve/data/provo_natural.csv` & `ratingcurve-1.0.2/ratingcurve/data/provo_natural.csv`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/ratingcurve/data/provo_natural.md` & `ratingcurve-1.0.2/ratingcurve/data/provo_natural.md`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/ratingcurve/data/simulated_rating.csv` & `ratingcurve-1.0.2/ratingcurve/data/simulated_rating.csv`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/ratingcurve/data/simulated_rating.md` & `ratingcurve-1.0.2/ratingcurve/data/simulated_rating.md`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/ratingcurve/data/skajalfandafljot.csv` & `ratingcurve-1.0.2/ratingcurve/data/skajalfandafljot.csv`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/ratingcurve/data/skajalfandafljot.md` & `ratingcurve-1.0.2/ratingcurve/data/skajalfandafljot.md`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/ratingcurve/experimental_ratings.py` & `ratingcurve-1.0.2/ratingcurve/experimental_ratings.py`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/ratingcurve/model_builder.py` & `ratingcurve-1.0.2/ratingcurve/model_builder.py`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/ratingcurve/plot.py` & `ratingcurve-1.0.2/ratingcurve/plot.py`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/ratingcurve/ratingmodel_builder.py` & `ratingcurve-1.0.2/ratingcurve/ratingmodel_builder.py`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/ratingcurve/ratings.py` & `ratingcurve-1.0.2/ratingcurve/ratings.py`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/ratingcurve/tests/test_fitting.py` & `ratingcurve-1.0.2/ratingcurve/tests/test_fitting.py`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/ratingcurve/tests/test_transform.py` & `ratingcurve-1.0.2/ratingcurve/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/ratingcurve/transform.py` & `ratingcurve-1.0.2/ratingcurve/transform.py`

 * *Files identical despite different names*

### Comparing `ratingcurve-1.0.1/ratingcurve.egg-info/PKG-INFO` & `ratingcurve-1.0.2/ratingcurve.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratingcurve
-Version: 1.0.1
+Version: 1.0.2
 Summary: A library for fitting multi-segment stage-discharge rating curves.
 Maintainer-email: Timothy Hodson <thodson@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, this project is in the public domain in the United
         States because it contains materials that originally came from the United
@@ -50,15 +50,15 @@
         
         [1]: https://creativecommons.org/publicdomain/zero/1.0/legalcode
         
 Project-URL: homepage, https://github.com/thodson-usgs/ratingcurve
 Project-URL: repository, https://github.com/thodson-usgs/ratingcurve.git
 Keywords: USGS,streamflow,rating curve
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: pymc>=5.0.0
 Requires-Dist: patsy
 Provides-Extra: test
 Requires-Dist: pytest>5.0.0; extra == "test"
 Requires-Dist: pytest-cov[all]; extra == "test"
@@ -127,7 +127,25 @@
 ## Disclaimer
 
 This software is preliminary or provisional and is subject to revision. 
 It is being provided to meet the need for timely best science.
 The software has not received final approval by the U.S. Geological Survey (USGS).
 No warranty, expressed or implied, is made by the USGS or the U.S. Government as to the functionality of the software and related material nor shall the fact of release constitute any such warranty. 
 The software is provided on the condition that neither the USGS nor the U.S. Government shall be held liable for any damages resulting from the authorized or unauthorized use of the software.
+
+## Citation
+Hodson, T.O., Doore, K.J., Kenney, T.A., Over T.M., and Yeheyis, M.B., 2024, Ratingcurve: A Python Package for Fitting Streamflow Rating Curves, Hydrology 11, no. 2: 14. https://doi.org/10.3390/hydrology11020014
+
+```
+@Article{hydrology11020014,
+AUTHOR = {Hodson, Timothy O. and Doore, Keith J. and Kenney, Terry A. and Over, Thomas M. and Yeheyis, Muluken B.},
+TITLE = {Ratingcurve: A Python Package for Fitting Streamflow Rating Curves},
+JOURNAL = {Hydrology},
+VOLUME = {11},
+YEAR = {2024},
+NUMBER = {2},
+ARTICLE-NUMBER = {14},
+URL = {https://www.mdpi.com/2306-5338/11/2/14},
+ISSN = {2306-5338},
+DOI = {10.3390/hydrology11020014}
+}
+```
```

### Comparing `ratingcurve-1.0.1/ratingcurve.egg-info/SOURCES.txt` & `ratingcurve-1.0.2/ratingcurve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

