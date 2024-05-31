# Comparing `tmp/textdescriptives-2.8.1.tar.gz` & `tmp/textdescriptives-2.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textdescriptives-2.8.1.tar", last modified: Tue May  7 13:29:32 2024, max compression
+gzip compressed data, was "textdescriptives-2.8.2.tar", last modified: Fri May 31 11:29:30 2024, max compression
```

## Comparing `textdescriptives-2.8.1.tar` & `textdescriptives-2.8.2.tar`

### file list

```diff
@@ -1,103 +1,101 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:29:32.404860 textdescriptives-2.8.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:29:32.380860 textdescriptives-2.8.1/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:29:32.384860 textdescriptives-2.8.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      582 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/.github/ISSUE_TEMPLATE/01_bugs.md
--rw-r--r--   0 root         (0) root         (0)      418 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/.github/ISSUE_TEMPLATE/02_docs.md
--rw-r--r--   0 root         (0) root         (0)      291 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/.github/ISSUE_TEMPLATE/03_feature-request.md
--rw-r--r--   0 root         (0) root         (0)      632 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 root         (0) root         (0)      776 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:29:32.384860 textdescriptives-2.8.1/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1047 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)     1247 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)      669 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/.github/workflows/draft-pdf.yml
--rw-r--r--   0 root         (0) root         (0)     2592 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)      867 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/.github/workflows/stale.yml
--rw-r--r--   0 root         (0) root         (0)     2254 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/.github/workflows/tests.yml
--rw-r--r--   0 root         (0) root         (0)     2140 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1395 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      907 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/.zenodo.json
--rw-r--r--   0 root         (0) root         (0)   187345 2024-05-07 13:29:28.000000 textdescriptives-2.8.1/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1361 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/CITATION.cff
--rw-r--r--   0 root         (0) root         (0)     5242 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     4473 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)    11357 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    24980 2024-05-07 13:29:32.404860 textdescriptives-2.8.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9398 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:29:32.388860 textdescriptives-2.8.1/docs/
--rw-r--r--   0 root         (0) root         (0)      634 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:29:32.388860 textdescriptives-2.8.1/docs/_static/
--rw-r--r--   0 root         (0) root         (0)   642030 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)   139565 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/_static/icon_dark_old.png
--rw-r--r--   0 root         (0) root         (0)   125611 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/_static/icon_old.png
--rw-r--r--   0 root         (0) root         (0)     3540 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/coherence.rst
--rw-r--r--   0 root         (0) root         (0)     3547 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     3189 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/dependencydistance.rst
--rw-r--r--   0 root         (0) root         (0)     3198 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/descriptivestats.rst
--rw-r--r--   0 root         (0) root         (0)      477 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/extractors.rst
--rw-r--r--   0 root         (0) root         (0)     1909 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)     2752 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     2374 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/information_theory.rst
--rw-r--r--   0 root         (0) root         (0)      859 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)      795 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)      987 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/news.rst
--rw-r--r--   0 root         (0) root         (0)     2790 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/posstats.rst
--rw-r--r--   0 root         (0) root         (0)     8242 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/quality.rst
--rw-r--r--   0 root         (0) root         (0)     7051 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/readability.rst
--rw-r--r--   0 root         (0) root         (0)      388 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/tutorial.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:29:32.388860 textdescriptives-2.8.1/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)    86776 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/tutorials/filter_corpus_using_quality.ipynb
--rw-r--r--   0 root         (0) root         (0)   115780 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/tutorials/introductory_tutorial.ipynb
--rw-r--r--   0 root         (0) root         (0)      273 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/tutorials/requirements.txt
--rw-r--r--   0 root         (0) root         (0)    13090 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/tutorials/sklearn_integration.ipynb
--rw-r--r--   0 root         (0) root         (0)     7465 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/docs/usingthepackage.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:29:32.392860 textdescriptives-2.8.1/paper/
--rw-r--r--   0 root         (0) root         (0)    23688 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/paper/paper.bib
--rw-r--r--   0 root         (0) root         (0)     9237 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/paper/paper.md
--rw-r--r--   0 root         (0) root         (0)    42220 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/paper/paper_quarto.pdf
--rw-r--r--   0 root         (0) root         (0)     9724 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/paper/paper_quarto.qmd
--rw-r--r--   0 root         (0) root         (0)      473 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/paper/readme.md
--rw-r--r--   0 root         (0) root         (0)     2989 2024-05-07 13:29:28.000000 textdescriptives-2.8.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 13:29:32.404860 textdescriptives-2.8.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:29:32.380860 textdescriptives-2.8.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:29:32.392860 textdescriptives-2.8.1/src/textdescriptives/
--rw-r--r--   0 root         (0) root         (0)      328 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/__init__.py
--rw-r--r--   0 root         (0) root         (0)      492 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/about.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:29:32.396860 textdescriptives-2.8.1/src/textdescriptives/components/
--rw-r--r--   0 root         (0) root         (0)      396 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/components/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5395 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/components/coherence.py
--rw-r--r--   0 root         (0) root         (0)     5748 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/components/dependency_distance.py
--rw-r--r--   0 root         (0) root         (0)     8377 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/components/descriptive_stats.py
--rw-r--r--   0 root         (0) root         (0)     6261 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/components/information_theory.py
--rw-r--r--   0 root         (0) root         (0)     4416 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/components/pos_proportions.py
--rw-r--r--   0 root         (0) root         (0)    21832 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/components/quality.py
--rw-r--r--   0 root         (0) root         (0)    10429 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/components/quality_data_classes.py
--rw-r--r--   0 root         (0) root         (0)     8209 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/components/readability.py
--rw-r--r--   0 root         (0) root         (0)     1241 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/components/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:29:32.396860 textdescriptives-2.8.1/src/textdescriptives/data/
--rw-r--r--   0 root         (0) root         (0)   503663 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/data/spam.csv
--rw-r--r--   0 root         (0) root         (0)     6127 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/extractors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:29:32.396860 textdescriptives-2.8.1/src/textdescriptives/integrations/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/integrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4355 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/integrations/sklearn_featurizer.py
--rw-r--r--   0 root         (0) root         (0)     1331 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/load_components.py
--rw-r--r--   0 root         (0) root         (0)     6212 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/src/textdescriptives/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:29:32.400859 textdescriptives-2.8.1/src/textdescriptives.egg-info/
--rw-r--r--   0 root         (0) root         (0)    24980 2024-05-07 13:29:32.000000 textdescriptives-2.8.1/src/textdescriptives.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2508 2024-05-07 13:29:32.000000 textdescriptives-2.8.1/src/textdescriptives.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 13:29:32.000000 textdescriptives-2.8.1/src/textdescriptives.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      500 2024-05-07 13:29:32.000000 textdescriptives-2.8.1/src/textdescriptives.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-07 13:29:32.000000 textdescriptives-2.8.1/src/textdescriptives.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 13:29:32.400859 textdescriptives-2.8.1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28399 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/tests/books.py
--rw-r--r--   0 root         (0) root         (0)      382 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/tests/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     2821 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/tests/test_coherence.py
--rw-r--r--   0 root         (0) root         (0)     2930 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/tests/test_dependency_distance.py
--rw-r--r--   0 root         (0) root         (0)     3505 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/tests/test_descriptive_stats.py
--rw-r--r--   0 root         (0) root         (0)     5331 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/tests/test_extractors.py
--rw-r--r--   0 root         (0) root         (0)     1384 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/tests/test_information.py
--rw-r--r--   0 root         (0) root         (0)      705 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/tests/test_load_components.py
--rw-r--r--   0 root         (0) root         (0)     2898 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/tests/test_pos_proportions.py
--rw-r--r--   0 root         (0) root         (0)     9278 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/tests/test_quality.py
--rw-r--r--   0 root         (0) root         (0)     5308 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/tests/test_readability.py
--rw-r--r--   0 root         (0) root         (0)      572 2024-05-07 13:29:17.000000 textdescriptives-2.8.1/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 11:29:30.082342 textdescriptives-2.8.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 11:29:30.054341 textdescriptives-2.8.2/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 11:29:30.062342 textdescriptives-2.8.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      582 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/.github/ISSUE_TEMPLATE/01_bugs.md
+-rw-r--r--   0 root         (0) root         (0)      418 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/.github/ISSUE_TEMPLATE/02_docs.md
+-rw-r--r--   0 root         (0) root         (0)      291 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/.github/ISSUE_TEMPLATE/03_feature-request.md
+-rw-r--r--   0 root         (0) root         (0)      632 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/.github/ISSUE_TEMPLATE/config.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 11:29:30.062342 textdescriptives-2.8.2/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1247 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)      669 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/.github/workflows/draft-pdf.yml
+-rw-r--r--   0 root         (0) root         (0)     2592 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)      867 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/.github/workflows/stale.yml
+-rw-r--r--   0 root         (0) root         (0)     2254 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/.github/workflows/tests.yml
+-rw-r--r--   0 root         (0) root         (0)     2140 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1395 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      907 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/.zenodo.json
+-rw-r--r--   0 root         (0) root         (0)   188426 2024-05-31 11:29:26.000000 textdescriptives-2.8.2/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1361 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/CITATION.cff
+-rw-r--r--   0 root         (0) root         (0)     5242 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     4473 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    24965 2024-05-31 11:29:30.082342 textdescriptives-2.8.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9398 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 11:29:30.066341 textdescriptives-2.8.2/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 11:29:30.066341 textdescriptives-2.8.2/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)   642030 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)   139565 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/docs/_static/icon_dark_old.png
+-rw-r--r--   0 root         (0) root         (0)   125611 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/docs/_static/icon_old.png
+-rw-r--r--   0 root         (0) root         (0)     3540 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/docs/coherence.rst
+-rw-r--r--   0 root         (0) root         (0)     3547 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     3189 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/docs/dependencydistance.rst
+-rw-r--r--   0 root         (0) root         (0)     3198 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/docs/descriptivestats.rst
+-rw-r--r--   0 root         (0) root         (0)      477 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/docs/extractors.rst
+-rw-r--r--   0 root         (0) root         (0)     1909 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)     2752 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     2374 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/docs/information_theory.rst
+-rw-r--r--   0 root         (0) root         (0)      859 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)      795 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)      987 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/docs/news.rst
+-rw-r--r--   0 root         (0) root         (0)     2790 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/docs/posstats.rst
+-rw-r--r--   0 root         (0) root         (0)     8242 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/docs/quality.rst
+-rw-r--r--   0 root         (0) root         (0)     7051 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/docs/readability.rst
+-rw-r--r--   0 root         (0) root         (0)      388 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/docs/tutorial.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 11:29:30.066341 textdescriptives-2.8.2/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)    86776 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/docs/tutorials/filter_corpus_using_quality.ipynb
+-rw-r--r--   0 root         (0) root         (0)   115780 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/docs/tutorials/introductory_tutorial.ipynb
+-rw-r--r--   0 root         (0) root         (0)      273 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/docs/tutorials/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)    13090 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/docs/tutorials/sklearn_integration.ipynb
+-rw-r--r--   0 root         (0) root         (0)     7465 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/docs/usingthepackage.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 11:29:30.070342 textdescriptives-2.8.2/paper/
+-rw-r--r--   0 root         (0) root         (0)    23688 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/paper/paper.bib
+-rw-r--r--   0 root         (0) root         (0)     9237 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/paper/paper.md
+-rw-r--r--   0 root         (0) root         (0)    42220 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/paper/paper_quarto.pdf
+-rw-r--r--   0 root         (0) root         (0)     9724 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/paper/paper_quarto.qmd
+-rw-r--r--   0 root         (0) root         (0)      473 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/paper/readme.md
+-rw-r--r--   0 root         (0) root         (0)     2974 2024-05-31 11:29:26.000000 textdescriptives-2.8.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-31 11:29:30.082342 textdescriptives-2.8.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 11:29:30.058341 textdescriptives-2.8.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 11:29:30.070342 textdescriptives-2.8.2/src/textdescriptives/
+-rw-r--r--   0 root         (0) root         (0)      328 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/src/textdescriptives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      492 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/src/textdescriptives/about.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 11:29:30.074342 textdescriptives-2.8.2/src/textdescriptives/components/
+-rw-r--r--   0 root         (0) root         (0)      396 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/src/textdescriptives/components/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5395 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/src/textdescriptives/components/coherence.py
+-rw-r--r--   0 root         (0) root         (0)     5748 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/src/textdescriptives/components/dependency_distance.py
+-rw-r--r--   0 root         (0) root         (0)     8377 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/src/textdescriptives/components/descriptive_stats.py
+-rw-r--r--   0 root         (0) root         (0)     6261 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/src/textdescriptives/components/information_theory.py
+-rw-r--r--   0 root         (0) root         (0)     4416 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/src/textdescriptives/components/pos_proportions.py
+-rw-r--r--   0 root         (0) root         (0)    21832 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/src/textdescriptives/components/quality.py
+-rw-r--r--   0 root         (0) root         (0)    10429 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/src/textdescriptives/components/quality_data_classes.py
+-rw-r--r--   0 root         (0) root         (0)     8209 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/src/textdescriptives/components/readability.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/src/textdescriptives/components/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 11:29:30.074342 textdescriptives-2.8.2/src/textdescriptives/data/
+-rw-r--r--   0 root         (0) root         (0)   503663 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/src/textdescriptives/data/spam.csv
+-rw-r--r--   0 root         (0) root         (0)     6127 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/src/textdescriptives/extractors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 11:29:30.074342 textdescriptives-2.8.2/src/textdescriptives/integrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/src/textdescriptives/integrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4355 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/src/textdescriptives/integrations/sklearn_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)     1331 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/src/textdescriptives/load_components.py
+-rw-r--r--   0 root         (0) root         (0)     6212 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/src/textdescriptives/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 11:29:30.078342 textdescriptives-2.8.2/src/textdescriptives.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    24965 2024-05-31 11:29:30.000000 textdescriptives-2.8.2/src/textdescriptives.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2442 2024-05-31 11:29:30.000000 textdescriptives-2.8.2/src/textdescriptives.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 11:29:30.000000 textdescriptives-2.8.2/src/textdescriptives.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2024-05-31 11:29:30.000000 textdescriptives-2.8.2/src/textdescriptives.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-31 11:29:30.000000 textdescriptives-2.8.2/src/textdescriptives.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 11:29:30.078342 textdescriptives-2.8.2/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28399 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/tests/books.py
+-rw-r--r--   0 root         (0) root         (0)      382 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/tests/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     2821 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/tests/test_coherence.py
+-rw-r--r--   0 root         (0) root         (0)     2930 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/tests/test_dependency_distance.py
+-rw-r--r--   0 root         (0) root         (0)     3505 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/tests/test_descriptive_stats.py
+-rw-r--r--   0 root         (0) root         (0)     5331 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/tests/test_extractors.py
+-rw-r--r--   0 root         (0) root         (0)     1384 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/tests/test_information.py
+-rw-r--r--   0 root         (0) root         (0)      705 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/tests/test_load_components.py
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/tests/test_pos_proportions.py
+-rw-r--r--   0 root         (0) root         (0)     9278 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/tests/test_quality.py
+-rw-r--r--   0 root         (0) root         (0)     5308 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/tests/test_readability.py
+-rw-r--r--   0 root         (0) root         (0)      572 2024-05-31 11:29:16.000000 textdescriptives-2.8.2/tests/test_utils.py
```

### Comparing `textdescriptives-2.8.1/.github/ISSUE_TEMPLATE/01_bugs.md` & `textdescriptives-2.8.2/.github/ISSUE_TEMPLATE/01_bugs.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/.github/ISSUE_TEMPLATE/config.yml` & `textdescriptives-2.8.2/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/.github/workflows/documentation.yml` & `textdescriptives-2.8.2/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/.github/workflows/draft-pdf.yml` & `textdescriptives-2.8.2/.github/workflows/draft-pdf.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/.github/workflows/release.yml` & `textdescriptives-2.8.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/.github/workflows/stale.yml` & `textdescriptives-2.8.2/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/.github/workflows/tests.yml` & `textdescriptives-2.8.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/.gitignore` & `textdescriptives-2.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/.pre-commit-config.yaml` & `textdescriptives-2.8.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/.zenodo.json` & `textdescriptives-2.8.2/.zenodo.json`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/CHANGELOG.md` & `textdescriptives-2.8.2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,34 @@
 # CHANGELOG
 
 
 
+## v2.8.2 (2024-05-31)
+
+### Ci
+
+* ci: remove dependabot ([`1dcfd7a`](https://github.com/HLasse/TextDescriptives/commit/1dcfd7acf57f0bea0feec76845c3d3fe6d513780))
+
+### Fix
+
+* fix: don&#39;t cap core dependency versions ([`0d29c69`](https://github.com/HLasse/TextDescriptives/commit/0d29c69f76b9bed146518786b8612fb8324d6e7a))
+
+### Unknown
+
+* Merge pull request #354 from HLasse/dont-cap-versions
+
+Remove upper bound of core dependencies and remove dependabot ([`53a4e03`](https://github.com/HLasse/TextDescriptives/commit/53a4e039e8b13d8a9f48a552eb0220b5873bc4c4))
+
+* Merge branch &#39;main&#39; into dont-cap-versions ([`889afef`](https://github.com/HLasse/TextDescriptives/commit/889afefa5f029a7e5e68fa71dac858cff2d99ded))
+
+* Merge pull request #352 from Rested/main
+
+:arrow_up: be more lenient with ftfy dependency ([`d2e22f3`](https://github.com/HLasse/TextDescriptives/commit/d2e22f39ffa7487d5a5d2cb39760b80d40cbc3f6))
+
+
 ## v2.8.1 (2024-05-07)
 
 ### Documentation
 
 * docs: fix link to document in readme ([`096a6b8`](https://github.com/HLasse/TextDescriptives/commit/096a6b8f92b4b2ccf03ec70e5caf320830ce113b))
 
 ### Fix
@@ -20,14 +43,16 @@
 
 * Merge pull request #353 from HLasse/fix-quality-threshold-not-set
 
 fix: `contains` and `symbols` not updated in `Quality` ([`cfe9b87`](https://github.com/HLasse/TextDescriptives/commit/cfe9b876885e052d8b3e62a24d7c559e0e064718))
 
 * tests: update test ([`7915eeb`](https://github.com/HLasse/TextDescriptives/commit/7915eeba0768c699dedb99f0ea6c3419e2f9104d))
 
+* :arrow_up: be more lenient with ftfy dependency ([`067eb99`](https://github.com/HLasse/TextDescriptives/commit/067eb99019f3cf84c4f9647085026a2795443775))
+
 * Merge pull request #344 from HLasse/HLasse-patch-1
 
 docs: fix link to document in readme ([`e470db7`](https://github.com/HLasse/TextDescriptives/commit/e470db7cc759309e318aa1eaba675f755fae7ae9))
 
 * Merge pull request #342 from HLasse/update-docs
 
 Update docs ([`93b1d59`](https://github.com/HLasse/TextDescriptives/commit/93b1d59278dc86cd4e8df80247e8a1a5afda2f59))
```

### Comparing `textdescriptives-2.8.1/CITATION.cff` & `textdescriptives-2.8.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/CODE_OF_CONDUCT.md` & `textdescriptives-2.8.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/CONTRIBUTING.md` & `textdescriptives-2.8.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/LICENSE` & `textdescriptives-2.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/PKG-INFO` & `textdescriptives-2.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textdescriptives
-Version: 2.8.1
+Version: 2.8.2
 Summary: A library for calculating a variety of features from text using spaCy
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -224,16 +224,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: spacy[lookups]>=3.6.0
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: pandas>=1.0.0
-Requires-Dist: pyphen<0.15.0,>=0.11.0
-Requires-Dist: ftfy<6.1.0,>=6.0.3
+Requires-Dist: pyphen>=0.11.0
+Requires-Dist: ftfy>=6.0.3
 Requires-Dist: pydantic>=2.0
 Provides-Extra: style
 Requires-Dist: black==24.1.1; extra == "style"
 Requires-Dist: pre-commit==3.6.0; extra == "style"
 Requires-Dist: ruff==0.1.15; extra == "style"
 Requires-Dist: mypy==1.8.0; extra == "style"
 Provides-Extra: tests
```

### Comparing `textdescriptives-2.8.1/README.md` & `textdescriptives-2.8.2/README.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/docs/Makefile` & `textdescriptives-2.8.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/docs/_static/icon.png` & `textdescriptives-2.8.2/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/docs/_static/icon_dark_old.png` & `textdescriptives-2.8.2/docs/_static/icon_dark_old.png`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/docs/_static/icon_old.png` & `textdescriptives-2.8.2/docs/_static/icon_old.png`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/docs/coherence.rst` & `textdescriptives-2.8.2/docs/coherence.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/docs/conf.py` & `textdescriptives-2.8.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/docs/dependencydistance.rst` & `textdescriptives-2.8.2/docs/dependencydistance.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/docs/descriptivestats.rst` & `textdescriptives-2.8.2/docs/descriptivestats.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/docs/faq.rst` & `textdescriptives-2.8.2/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/docs/index.rst` & `textdescriptives-2.8.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/docs/information_theory.rst` & `textdescriptives-2.8.2/docs/information_theory.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/docs/installation.rst` & `textdescriptives-2.8.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/docs/make.bat` & `textdescriptives-2.8.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/docs/news.rst` & `textdescriptives-2.8.2/docs/news.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/docs/posstats.rst` & `textdescriptives-2.8.2/docs/posstats.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/docs/quality.rst` & `textdescriptives-2.8.2/docs/quality.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/docs/readability.rst` & `textdescriptives-2.8.2/docs/readability.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/docs/tutorials/filter_corpus_using_quality.ipynb` & `textdescriptives-2.8.2/docs/tutorials/filter_corpus_using_quality.ipynb`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/docs/tutorials/introductory_tutorial.ipynb` & `textdescriptives-2.8.2/docs/tutorials/introductory_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/docs/tutorials/sklearn_integration.ipynb` & `textdescriptives-2.8.2/docs/tutorials/sklearn_integration.ipynb`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/docs/usingthepackage.rst` & `textdescriptives-2.8.2/docs/usingthepackage.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/paper/paper.bib` & `textdescriptives-2.8.2/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/paper/paper.md` & `textdescriptives-2.8.2/paper/paper.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/paper/paper_quarto.pdf` & `textdescriptives-2.8.2/paper/paper_quarto.pdf`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/paper/paper_quarto.qmd` & `textdescriptives-2.8.2/paper/paper_quarto.qmd`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/pyproject.toml` & `textdescriptives-2.8.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "textdescriptives"
-version = "2.8.1"
+version = "2.8.2"
 description = "A library for calculating a variety of features from text using spaCy"
 authors = [
     { name = "Lasse Hansen", email = "lasseh0310@gmail.com" },
     { name = "Kenneth Enevoldsen" },
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -33,16 +33,16 @@
     "text mining",
 ]
 
 dependencies = [
     "spacy[lookups]>=3.6.0",
     "numpy>=1.20.0",
     "pandas>=1.0.0",
-    "pyphen>=0.11.0,<0.15.0",
-    "ftfy>=6.0.3,<6.1.0",
+    "pyphen>=0.11.0",
+    "ftfy>=6.0.3",
     "pydantic>=2.0",
 ]
 
 requires-python = ">=3.8"
 
 [project.urls]
 homepage = "https://hlasse.github.io/TextDescriptives/"
```

### Comparing `textdescriptives-2.8.1/src/textdescriptives/components/coherence.py` & `textdescriptives-2.8.2/src/textdescriptives/components/coherence.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/src/textdescriptives/components/dependency_distance.py` & `textdescriptives-2.8.2/src/textdescriptives/components/dependency_distance.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/src/textdescriptives/components/descriptive_stats.py` & `textdescriptives-2.8.2/src/textdescriptives/components/descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/src/textdescriptives/components/information_theory.py` & `textdescriptives-2.8.2/src/textdescriptives/components/information_theory.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/src/textdescriptives/components/pos_proportions.py` & `textdescriptives-2.8.2/src/textdescriptives/components/pos_proportions.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/src/textdescriptives/components/quality.py` & `textdescriptives-2.8.2/src/textdescriptives/components/quality.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/src/textdescriptives/components/quality_data_classes.py` & `textdescriptives-2.8.2/src/textdescriptives/components/quality_data_classes.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/src/textdescriptives/components/readability.py` & `textdescriptives-2.8.2/src/textdescriptives/components/readability.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/src/textdescriptives/components/utils.py` & `textdescriptives-2.8.2/src/textdescriptives/components/utils.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/src/textdescriptives/data/spam.csv` & `textdescriptives-2.8.2/src/textdescriptives/data/spam.csv`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/src/textdescriptives/extractors.py` & `textdescriptives-2.8.2/src/textdescriptives/extractors.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/src/textdescriptives/integrations/sklearn_featurizer.py` & `textdescriptives-2.8.2/src/textdescriptives/integrations/sklearn_featurizer.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/src/textdescriptives/load_components.py` & `textdescriptives-2.8.2/src/textdescriptives/load_components.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/src/textdescriptives/utils.py` & `textdescriptives-2.8.2/src/textdescriptives/utils.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/src/textdescriptives.egg-info/PKG-INFO` & `textdescriptives-2.8.2/src/textdescriptives.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textdescriptives
-Version: 2.8.1
+Version: 2.8.2
 Summary: A library for calculating a variety of features from text using spaCy
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -224,16 +224,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: spacy[lookups]>=3.6.0
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: pandas>=1.0.0
-Requires-Dist: pyphen<0.15.0,>=0.11.0
-Requires-Dist: ftfy<6.1.0,>=6.0.3
+Requires-Dist: pyphen>=0.11.0
+Requires-Dist: ftfy>=6.0.3
 Requires-Dist: pydantic>=2.0
 Provides-Extra: style
 Requires-Dist: black==24.1.1; extra == "style"
 Requires-Dist: pre-commit==3.6.0; extra == "style"
 Requires-Dist: ruff==0.1.15; extra == "style"
 Requires-Dist: mypy==1.8.0; extra == "style"
 Provides-Extra: tests
```

### Comparing `textdescriptives-2.8.1/src/textdescriptives.egg-info/SOURCES.txt` & `textdescriptives-2.8.2/src/textdescriptives.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,18 @@
 CHANGELOG.md
 CITATION.cff
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 README.md
 pyproject.toml
-.github/dependabot.yml
 .github/ISSUE_TEMPLATE/01_bugs.md
 .github/ISSUE_TEMPLATE/02_docs.md
 .github/ISSUE_TEMPLATE/03_feature-request.md
 .github/ISSUE_TEMPLATE/config.yml
-.github/workflows/dependabot_automerge.yml
 .github/workflows/documentation.yml
 .github/workflows/draft-pdf.yml
 .github/workflows/release.yml
 .github/workflows/stale.yml
 .github/workflows/tests.yml
 docs/Makefile
 docs/coherence.rst
```

### Comparing `textdescriptives-2.8.1/tests/books.py` & `textdescriptives-2.8.2/tests/books.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/tests/test_coherence.py` & `textdescriptives-2.8.2/tests/test_coherence.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/tests/test_dependency_distance.py` & `textdescriptives-2.8.2/tests/test_dependency_distance.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/tests/test_descriptive_stats.py` & `textdescriptives-2.8.2/tests/test_descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/tests/test_extractors.py` & `textdescriptives-2.8.2/tests/test_extractors.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/tests/test_information.py` & `textdescriptives-2.8.2/tests/test_information.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/tests/test_load_components.py` & `textdescriptives-2.8.2/tests/test_load_components.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/tests/test_pos_proportions.py` & `textdescriptives-2.8.2/tests/test_pos_proportions.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/tests/test_quality.py` & `textdescriptives-2.8.2/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/tests/test_readability.py` & `textdescriptives-2.8.2/tests/test_readability.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.8.1/tests/test_utils.py` & `textdescriptives-2.8.2/tests/test_utils.py`

 * *Files identical despite different names*

