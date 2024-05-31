# Comparing `tmp/hlink-3.5.4.tar.gz` & `tmp/hlink-3.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hlink-3.5.4.tar", last modified: Tue Feb 20 20:30:28 2024, max compression
+gzip compressed data, was "hlink-3.5.5.tar", last modified: Fri May 31 17:40:09 2024, max compression
```

## Comparing `hlink-3.5.4.tar` & `hlink-3.5.5.tar`

### file list

```diff
@@ -1,429 +1,430 @@
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:28.842321 hlink-3.5.4/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       38 2022-12-08 21:42:38.000000 hlink-3.5.4/.dockerignore
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      185 2023-10-31 13:38:40.000000 hlink-3.5.4/.flake8
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:24.544027 hlink-3.5.4/.github/
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:24.936328 hlink-3.5.4/.github/workflows/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1120 2023-10-31 13:38:40.000000 hlink-3.5.4/.github/workflows/docker-build.yml
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      244 2022-12-08 21:42:38.000000 hlink-3.5.4/.gitignore
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      365 2022-12-08 21:42:38.000000 hlink-3.5.4/.pre-commit-config.yaml
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      226 2023-10-02 20:36:04.000000 hlink-3.5.4/Dockerfile
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    16726 2022-12-08 21:42:38.000000 hlink-3.5.4/LICENSE.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      615 2022-12-13 16:10:13.000000 hlink-3.5.4/NOTICE.txt
--rw-r--r--   0 rileyh   (42243) rileyh   (23521)    26257 2024-02-20 20:30:28.836799 hlink-3.5.4/PKG-INFO
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     5188 2023-11-01 19:00:05.000000 hlink-3.5.4/README.md
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      107 2022-12-13 16:04:48.000000 hlink-3.5.4/conftest.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:24.944128 hlink-3.5.4/doc/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4004 2023-10-03 19:12:10.000000 hlink-3.5.4/doc/developer.md
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:25.100129 hlink-3.5.4/docs/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      230 2024-02-20 20:19:26.000000 hlink-3.5.4/docs/.buildinfo
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:25.445464 hlink-3.5.4/docs/.doctrees/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    42484 2023-10-12 15:50:11.000000 hlink-3.5.4/docs/.doctrees/column_mapping_transforms.doctree
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)   163686 2023-10-12 15:50:11.000000 hlink-3.5.4/docs/.doctrees/comparison_types.doctree
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)   135404 2023-10-12 15:50:11.000000 hlink-3.5.4/docs/.doctrees/config.doctree
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    85920 2023-10-12 15:50:11.000000 hlink-3.5.4/docs/.doctrees/environment.pickle
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     5278 2023-10-12 15:50:11.000000 hlink-3.5.4/docs/.doctrees/example_workflow.doctree
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4591 2023-10-12 15:50:11.000000 hlink-3.5.4/docs/.doctrees/feature_selection_transforms.doctree
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     5278 2023-10-12 15:50:11.000000 hlink-3.5.4/docs/.doctrees/index.doctree
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     8241 2023-10-12 15:50:11.000000 hlink-3.5.4/docs/.doctrees/installation.doctree
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     9987 2023-10-12 15:50:11.000000 hlink-3.5.4/docs/.doctrees/introduction.doctree
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    10613 2023-10-12 15:50:11.000000 hlink-3.5.4/docs/.doctrees/link_tasks.doctree
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    21501 2023-10-12 15:50:11.000000 hlink-3.5.4/docs/.doctrees/models.doctree
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     8890 2023-10-12 15:50:11.000000 hlink-3.5.4/docs/.doctrees/pipeline_features.doctree
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    38499 2023-10-12 15:50:11.000000 hlink-3.5.4/docs/.doctrees/running_the_program.doctree
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    13195 2023-10-12 15:50:11.000000 hlink-3.5.4/docs/.doctrees/substitutions.doctree
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    30048 2023-10-12 15:50:11.000000 hlink-3.5.4/docs/.doctrees/use_examples.doctree
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2023-10-12 15:50:11.000000 hlink-3.5.4/docs/.nojekyll
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       20 2023-10-12 15:50:11.000000 hlink-3.5.4/docs/CNAME
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:25.587716 hlink-3.5.4/docs/_sources/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    10184 2023-12-01 18:23:26.000000 hlink-3.5.4/docs/_sources/column_mappings.md.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    39349 2023-10-16 18:49:31.000000 hlink-3.5.4/docs/_sources/comparison_types.md.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    30395 2023-12-01 18:18:19.000000 hlink-3.5.4/docs/_sources/config.md.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2773 2022-12-08 21:42:45.000000 hlink-3.5.4/docs/_sources/feature_selection_transforms.md.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      741 2023-12-01 18:18:19.000000 hlink-3.5.4/docs/_sources/index.rst.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1004 2023-11-01 19:00:05.000000 hlink-3.5.4/docs/_sources/installation.md.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2574 2022-12-08 21:42:45.000000 hlink-3.5.4/docs/_sources/introduction.md.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     7637 2023-12-01 18:18:19.000000 hlink-3.5.4/docs/_sources/link_tasks.md.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3703 2023-10-03 19:12:11.000000 hlink-3.5.4/docs/_sources/models.md.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1731 2022-12-08 21:42:45.000000 hlink-3.5.4/docs/_sources/pipeline_features.md.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    11301 2022-12-08 21:42:45.000000 hlink-3.5.4/docs/_sources/running_the_program.md.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1978 2022-12-08 21:42:45.000000 hlink-3.5.4/docs/_sources/substitutions.md.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     7114 2022-12-08 21:42:45.000000 hlink-3.5.4/docs/_sources/use_examples.md.txt
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:25.766193 hlink-3.5.4/docs/_static/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4418 2023-08-08 15:35:44.000000 hlink-3.5.4/docs/_static/_sphinx_javascript_frameworks_compat.js
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    11143 2024-02-20 20:19:26.000000 hlink-3.5.4/docs/_static/alabaster.css
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    15096 2024-02-20 20:19:26.000000 hlink-3.5.4/docs/_static/basic.css
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       42 2023-08-08 15:32:32.000000 hlink-3.5.4/docs/_static/custom.css
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4472 2024-02-20 19:59:37.000000 hlink-3.5.4/docs/_static/doctools.js
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      328 2024-02-20 20:19:26.000000 hlink-3.5.4/docs/_static/documentation_options.js
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      286 2023-10-31 13:43:49.000000 hlink-3.5.4/docs/_static/file.png
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)   287630 2022-03-02 16:32:08.000000 hlink-3.5.4/docs/_static/jquery-3.5.1.js
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)   288580 2023-08-08 15:35:44.000000 hlink-3.5.4/docs/_static/jquery-3.6.0.js
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    89476 2024-02-20 20:19:26.000000 hlink-3.5.4/docs/_static/jquery.js
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4758 2024-02-20 20:02:18.000000 hlink-3.5.4/docs/_static/language_data.js
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       90 2023-10-31 13:43:49.000000 hlink-3.5.4/docs/_static/minus.png
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       90 2023-10-31 13:43:49.000000 hlink-3.5.4/docs/_static/plus.png
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     5359 2024-02-20 20:19:26.000000 hlink-3.5.4/docs/_static/pygments.css
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    18732 2024-02-20 19:59:37.000000 hlink-3.5.4/docs/_static/searchtools.js
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     5123 2023-10-31 13:43:49.000000 hlink-3.5.4/docs/_static/sphinx_highlight.js
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    68420 2022-03-02 16:32:08.000000 hlink-3.5.4/docs/_static/underscore-1.13.1.js
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    19530 2022-03-02 16:32:08.000000 hlink-3.5.4/docs/_static/underscore.js
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    33865 2024-02-20 20:19:26.000000 hlink-3.5.4/docs/column_mappings.html
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)   124690 2024-02-20 20:19:26.000000 hlink-3.5.4/docs/comparison_types.html
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)   100403 2024-02-20 20:19:26.000000 hlink-3.5.4/docs/config.html
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    14070 2024-02-20 20:19:27.000000 hlink-3.5.4/docs/feature_selection_transforms.html
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3629 2024-02-20 20:19:27.000000 hlink-3.5.4/docs/genindex.html
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    12376 2024-02-20 20:19:27.000000 hlink-3.5.4/docs/index.html
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     6488 2024-02-20 20:19:27.000000 hlink-3.5.4/docs/installation.html
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     7686 2024-02-20 20:19:27.000000 hlink-3.5.4/docs/introduction.html
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    19893 2024-02-20 20:19:27.000000 hlink-3.5.4/docs/link_tasks.html
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    14220 2024-02-20 20:19:27.000000 hlink-3.5.4/docs/models.html
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      528 2024-02-20 20:19:27.000000 hlink-3.5.4/docs/objects.inv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     9451 2024-02-20 20:19:27.000000 hlink-3.5.4/docs/pipeline_features.html
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    25938 2024-02-20 20:19:27.000000 hlink-3.5.4/docs/running_the_program.html
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3906 2024-02-20 20:19:27.000000 hlink-3.5.4/docs/search.html
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    37109 2024-02-20 20:02:20.000000 hlink-3.5.4/docs/searchindex.js
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     9778 2024-02-20 20:19:27.000000 hlink-3.5.4/docs/substitutions.html
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    22557 2024-02-20 20:19:27.000000 hlink-3.5.4/docs/use_examples.html
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:24.680629 hlink-3.5.4/examples/
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:25.813488 hlink-3.5.4/examples/tutorial/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       29 2022-12-08 21:42:39.000000 hlink-3.5.4/examples/tutorial/.gitignore
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     6627 2022-12-08 21:42:39.000000 hlink-3.5.4/examples/tutorial/README.md
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:25.828446 hlink-3.5.4/examples/tutorial/data/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      285 2022-12-08 21:42:39.000000 hlink-3.5.4/examples/tutorial/data/A.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      226 2022-12-08 21:42:39.000000 hlink-3.5.4/examples/tutorial/data/B.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2985 2022-12-09 21:06:40.000000 hlink-3.5.4/examples/tutorial/tutorial.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1012 2022-12-08 21:42:39.000000 hlink-3.5.4/examples/tutorial/tutorial_config.toml
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:25.841271 hlink-3.5.4/hlink/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:39.000000 hlink-3.5.4/hlink/__init__.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:25.903107 hlink-3.5.4/hlink/configs/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:39.000000 hlink-3.5.4/hlink/configs/__init__.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     2172 2022-12-09 21:06:40.000000 hlink-3.5.4/hlink/configs/load_config.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)      479 2022-12-13 16:04:48.000000 hlink-3.5.4/hlink/errors.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:25.962185 hlink-3.5.4/hlink/linking/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      718 2022-12-08 21:42:39.000000 hlink-3.5.4/hlink/linking/README.md
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:39.000000 hlink-3.5.4/hlink/linking/__init__.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:26.059835 hlink-3.5.4/hlink/linking/core/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:39.000000 hlink-3.5.4/hlink/linking/core/__init__.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3406 2022-12-09 21:06:40.000000 hlink-3.5.4/hlink/linking/core/classifier.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     2219 2023-12-06 16:40:14.000000 hlink-3.5.4/hlink/linking/core/column_mapping.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     3083 2023-10-31 13:38:40.000000 hlink-3.5.4/hlink/linking/core/comparison.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    23236 2023-12-06 16:59:55.000000 hlink-3.5.4/hlink/linking/core/comparison_feature.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4196 2022-12-08 21:42:39.000000 hlink-3.5.4/hlink/linking/core/dist_table.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     8788 2023-11-01 21:30:51.000000 hlink-3.5.4/hlink/linking/core/pipeline.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3865 2022-12-09 21:06:40.000000 hlink-3.5.4/hlink/linking/core/substitutions.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4082 2023-10-30 19:42:28.000000 hlink-3.5.4/hlink/linking/core/threshold.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    22452 2023-11-20 22:06:54.000000 hlink-3.5.4/hlink/linking/core/transforms.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:26.116438 hlink-3.5.4/hlink/linking/hh_matching/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      265 2022-12-08 21:42:40.000000 hlink-3.5.4/hlink/linking/hh_matching/__init__.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      804 2022-12-09 21:06:40.000000 hlink-3.5.4/hlink/linking/hh_matching/hh_matching.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3229 2022-12-08 21:42:40.000000 hlink-3.5.4/hlink/linking/hh_matching/link_step_block_on_households.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2234 2022-12-09 21:06:40.000000 hlink-3.5.4/hlink/linking/hh_matching/link_step_filter.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:26.132976 hlink-3.5.4/hlink/linking/hh_matching/templates/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      413 2022-12-08 21:42:40.000000 hlink-3.5.4/hlink/linking/hh_matching/templates/hh_blocked_matches.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      566 2022-12-08 21:42:40.000000 hlink-3.5.4/hlink/linking/hh_matching/templates/hh_potential_matches.sql
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:26.155876 hlink-3.5.4/hlink/linking/hh_model_exploration/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      282 2022-12-08 21:42:40.000000 hlink-3.5.4/hlink/linking/hh_model_exploration/__init__.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      992 2022-12-09 21:06:40.000000 hlink-3.5.4/hlink/linking/hh_model_exploration/hh_model_exploration.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:26.163162 hlink-3.5.4/hlink/linking/hh_model_exploration/templates/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:40.000000 hlink-3.5.4/hlink/linking/hh_model_exploration/templates/.gitkeep
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:26.181180 hlink-3.5.4/hlink/linking/hh_training/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      265 2022-12-08 21:42:40.000000 hlink-3.5.4/hlink/linking/hh_training/__init__.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      940 2022-12-09 21:06:40.000000 hlink-3.5.4/hlink/linking/hh_training/hh_training.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:26.189068 hlink-3.5.4/hlink/linking/hh_training/templates/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:40.000000 hlink-3.5.4/hlink/linking/hh_training/templates/.gitkeep
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4518 2022-12-09 21:06:40.000000 hlink-3.5.4/hlink/linking/link_run.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1699 2023-11-20 22:19:38.000000 hlink-3.5.4/hlink/linking/link_step.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     6887 2023-10-31 13:38:40.000000 hlink-3.5.4/hlink/linking/link_task.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:26.264685 hlink-3.5.4/hlink/linking/matching/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      260 2022-12-08 21:42:40.000000 hlink-3.5.4/hlink/linking/matching/__init__.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      519 2022-12-08 21:42:40.000000 hlink-3.5.4/hlink/linking/matching/_helpers.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     7185 2024-02-20 19:22:56.000000 hlink-3.5.4/hlink/linking/matching/link_step_explode.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4228 2022-12-09 21:06:40.000000 hlink-3.5.4/hlink/linking/matching/link_step_match.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     8555 2023-10-23 19:28:03.000000 hlink-3.5.4/hlink/linking/matching/link_step_score.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      658 2022-12-09 21:06:40.000000 hlink-3.5.4/hlink/linking/matching/matching.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:26.290662 hlink-3.5.4/hlink/linking/matching/templates/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      772 2022-12-08 21:42:40.000000 hlink-3.5.4/hlink/linking/matching/templates/potential_matches.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      404 2022-12-08 21:42:40.000000 hlink-3.5.4/hlink/linking/matching/templates/potential_matches_count.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      503 2022-12-08 21:42:40.000000 hlink-3.5.4/hlink/linking/matching/templates/potential_matches_universe.sql
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:26.401453 hlink-3.5.4/hlink/linking/model_exploration/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      277 2022-12-08 21:42:40.000000 hlink-3.5.4/hlink/linking/model_exploration/__init__.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4731 2022-12-09 21:06:40.000000 hlink-3.5.4/hlink/linking/model_exploration/link_step_create_features.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      872 2022-12-08 21:42:40.000000 hlink-3.5.4/hlink/linking/model_exploration/link_step_ingest_file.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    21393 2022-12-13 16:04:48.000000 hlink-3.5.4/hlink/linking/model_exploration/link_step_train_test_models.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      828 2023-10-23 19:28:03.000000 hlink-3.5.4/hlink/linking/model_exploration/model_exploration.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:26.409541 hlink-3.5.4/hlink/linking/model_exploration/templates/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:40.000000 hlink-3.5.4/hlink/linking/model_exploration/templates/.gitkeep
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:26.437903 hlink-3.5.4/hlink/linking/preprocessing/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      270 2022-12-08 21:42:40.000000 hlink-3.5.4/hlink/linking/preprocessing/__init__.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4431 2023-11-16 18:36:06.000000 hlink-3.5.4/hlink/linking/preprocessing/link_step_prep_dataframes.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     8308 2023-11-16 18:36:06.000000 hlink-3.5.4/hlink/linking/preprocessing/link_step_register_raw_dfs.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      509 2022-12-09 21:06:41.000000 hlink-3.5.4/hlink/linking/preprocessing/preprocessing.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:26.489436 hlink-3.5.4/hlink/linking/preprocessing/templates/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      431 2022-12-08 21:42:40.000000 hlink-3.5.4/hlink/linking/preprocessing/templates/attach_family_col.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      359 2022-12-08 21:42:40.000000 hlink-3.5.4/hlink/linking/preprocessing/templates/attach_neighbor_col.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      660 2022-12-08 21:42:40.000000 hlink-3.5.4/hlink/linking/preprocessing/templates/attach_related_col.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      885 2022-12-08 21:42:40.000000 hlink-3.5.4/hlink/linking/preprocessing/templates/attach_related_cols_as_rows.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      471 2022-12-08 21:42:40.000000 hlink-3.5.4/hlink/linking/preprocessing/templates/hh_nbor.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      738 2022-12-08 21:42:40.000000 hlink-3.5.4/hlink/linking/preprocessing/templates/hh_nbor_rank.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      430 2022-12-08 21:42:40.000000 hlink-3.5.4/hlink/linking/preprocessing/templates/training_data_subset.sql
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:26.706111 hlink-3.5.4/hlink/linking/reporting/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      262 2022-12-08 21:42:40.000000 hlink-3.5.4/hlink/linking/reporting/__init__.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2874 2022-12-13 16:04:48.000000 hlink-3.5.4/hlink/linking/reporting/link_step_export_crosswalk.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3664 2022-12-09 21:06:41.000000 hlink-3.5.4/hlink/linking/reporting/link_step_report_r2_percent_linked.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    24145 2022-12-13 16:04:48.000000 hlink-3.5.4/hlink/linking/reporting/link_step_report_representivity.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      687 2022-12-09 21:06:41.000000 hlink-3.5.4/hlink/linking/reporting/reporting.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:26.715187 hlink-3.5.4/hlink/linking/reporting/templates/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.5.4/hlink/linking/reporting/templates/.gitkeep
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1817 2022-12-09 17:39:25.000000 hlink-3.5.4/hlink/linking/table.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4001 2023-10-26 14:28:01.000000 hlink-3.5.4/hlink/linking/table_definitions.csv
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:24.751134 hlink-3.5.4/hlink/linking/templates/
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:26.808936 hlink-3.5.4/hlink/linking/templates/shared/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1003 2022-12-08 21:42:41.000000 hlink-3.5.4/hlink/linking/templates/shared/aggregate_features.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1201 2022-12-08 21:42:41.000000 hlink-3.5.4/hlink/linking/templates/shared/all_household_members.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      374 2022-12-08 21:42:41.000000 hlink-3.5.4/hlink/linking/templates/shared/attach_variable.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1021 2022-12-08 21:42:41.000000 hlink-3.5.4/hlink/linking/templates/shared/drop_links.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2205 2022-12-08 21:42:41.000000 hlink-3.5.4/hlink/linking/templates/shared/hh_aggregate_features.sql
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:26.829307 hlink-3.5.4/hlink/linking/templates/shared/includes/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1586 2022-12-08 21:42:41.000000 hlink-3.5.4/hlink/linking/templates/shared/includes/all_household_members_selects_a.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1600 2022-12-08 21:42:41.000000 hlink-3.5.4/hlink/linking/templates/shared/includes/all_household_members_selects_b.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      487 2022-12-08 21:42:41.000000 hlink-3.5.4/hlink/linking/templates/shared/pl_easy_features.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      653 2022-12-08 21:42:41.000000 hlink-3.5.4/hlink/linking/templates/shared/potential_matches_base_features.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      412 2022-12-08 21:42:41.000000 hlink-3.5.4/hlink/linking/templates/shared/scored_potential_matches.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      420 2022-12-08 21:42:41.000000 hlink-3.5.4/hlink/linking/templates/shared/select_columns.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      591 2022-12-08 21:42:41.000000 hlink-3.5.4/hlink/linking/templates/shared/tfam_tables.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      702 2022-12-08 21:42:41.000000 hlink-3.5.4/hlink/linking/templates/shared/training_features.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      510 2022-12-08 21:42:41.000000 hlink-3.5.4/hlink/linking/templates/shared/training_prepped.sql
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:26.878247 hlink-3.5.4/hlink/linking/training/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      260 2022-12-08 21:42:41.000000 hlink-3.5.4/hlink/linking/training/__init__.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3834 2022-12-09 21:06:41.000000 hlink-3.5.4/hlink/linking/training/link_step_create_comparison_features.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      872 2022-12-08 21:42:41.000000 hlink-3.5.4/hlink/linking/training/link_step_ingest_file.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     5323 2023-10-26 14:44:11.000000 hlink-3.5.4/hlink/linking/training/link_step_save_model_metadata.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3230 2023-10-26 14:28:01.000000 hlink-3.5.4/hlink/linking/training/link_step_train_and_save_model.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:26.886147 hlink-3.5.4/hlink/linking/training/templates/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.5.4/hlink/linking/training/templates/.gitkeep
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      927 2023-10-23 19:28:03.000000 hlink-3.5.4/hlink/linking/training/training.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:26.917269 hlink-3.5.4/hlink/linking/transformers/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.5.4/hlink/linking/transformers/__init__.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1202 2022-12-09 21:06:41.000000 hlink-3.5.4/hlink/linking/transformers/float_cast_transformer.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2821 2023-10-09 17:50:59.000000 hlink-3.5.4/hlink/linking/transformers/interaction_transformer.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      615 2022-12-09 21:06:41.000000 hlink-3.5.4/hlink/linking/transformers/rename_prob_column.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      648 2022-12-09 21:06:41.000000 hlink-3.5.4/hlink/linking/util.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:26.939156 hlink-3.5.4/hlink/scripts/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.5.4/hlink/scripts/__init__.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:26.991726 hlink-3.5.4/hlink/scripts/lib/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.5.4/hlink/scripts/lib/__init__.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    16597 2024-02-20 19:22:56.000000 hlink-3.5.4/hlink/scripts/lib/conf_validations.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:27.013139 hlink-3.5.4/hlink/scripts/lib/experimental/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.5.4/hlink/scripts/lib/experimental/__init__.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     4044 2022-12-13 16:04:48.000000 hlink-3.5.4/hlink/scripts/lib/experimental/reporting.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     8493 2022-12-08 21:42:41.000000 hlink-3.5.4/hlink/scripts/lib/experimental/tfam.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3252 2022-12-08 21:42:41.000000 hlink-3.5.4/hlink/scripts/lib/io.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2654 2023-10-31 13:38:40.000000 hlink-3.5.4/hlink/scripts/lib/linking_ops.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     5314 2023-08-09 20:43:52.000000 hlink-3.5.4/hlink/scripts/lib/table_ops.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      812 2022-12-09 21:06:41.000000 hlink-3.5.4/hlink/scripts/lib/util.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     8534 2023-11-02 15:30:46.000000 hlink-3.5.4/hlink/scripts/main.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    20808 2023-11-02 15:30:46.000000 hlink-3.5.4/hlink/scripts/main_loop.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:27.041792 hlink-3.5.4/hlink/spark/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.5.4/hlink/spark/__init__.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2494 2022-12-08 21:42:41.000000 hlink-3.5.4/hlink/spark/factory.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:27.049764 hlink-3.5.4/hlink/spark/jars/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)  6446850 2022-12-08 21:42:41.000000 hlink-3.5.4/hlink/spark/jars/hlink_lib-assembly-1.0.jar
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4786 2022-12-13 16:04:48.000000 hlink-3.5.4/hlink/spark/session.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:27.386606 hlink-3.5.4/hlink/tests/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.5.4/hlink/tests/__init__.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:27.529867 hlink-3.5.4/hlink/tests/conf/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      294 2023-10-30 19:42:28.000000 hlink-3.5.4/hlink/tests/conf/duplicate_col_maps.toml
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      720 2023-10-30 19:42:28.000000 hlink-3.5.4/hlink/tests/conf/duplicate_comp_features.toml
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      513 2023-10-30 19:42:29.000000 hlink-3.5.4/hlink/tests/conf/duplicate_feature_sel.toml
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1629 2022-12-08 21:42:41.000000 hlink-3.5.4/hlink/tests/conf/integration.toml
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       17 2022-12-08 21:42:41.000000 hlink-3.5.4/hlink/tests/conf/missing_datasource_a.toml
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       87 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/conf/missing_datasource_b.toml
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      258 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/conf/no_id_column_a.toml
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      258 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/conf/no_id_column_b.toml
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      123 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/conf/test.json
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       81 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/conf/test1.toml
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      133 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/conf/test_conf_flag_run.json
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      131 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/conf/test_run.json
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     7710 2024-02-20 19:22:56.000000 hlink-3.5.4/hlink/tests/conf_validations_test.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      920 2022-12-09 21:06:41.000000 hlink-3.5.4/hlink/tests/config_loader_test.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    49636 2022-12-13 16:04:48.000000 hlink-3.5.4/hlink/tests/conftest.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:27.568127 hlink-3.5.4/hlink/tests/core/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/core/__init__.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     9062 2023-12-06 16:40:14.000000 hlink-3.5.4/hlink/tests/core/column_mapping_test.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    14157 2023-10-16 18:49:31.000000 hlink-3.5.4/hlink/tests/core/comparison_feature_test.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1200 2023-10-16 18:49:31.000000 hlink-3.5.4/hlink/tests/core/pipeline_test.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    10639 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/hh_matching_test.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4245 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/hh_model_exploration_test.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:28.190482 hlink-3.5.4/hlink/tests/input_data/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      706 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/19thc_nativity_test_hhs.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2250 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/19thc_nativity_test_hhs_a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      989 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/19thc_nativity_test_hhs_b.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      221 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/birthyr_replace.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      630 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/calc_mfbpl_a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      553 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/calc_mfbpl_b.csv
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:28.213252 hlink-3.5.4/hlink/tests/input_data/conf_validation/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       29 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/conf_validation/a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       29 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/conf_validation/b.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/conf_validation/empty.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      155 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/county_distances.csv
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:28.246266 hlink-3.5.4/hlink/tests/input_data/crosswalk/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       29 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/crosswalk/hh_predicted_matches.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       53 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/crosswalk/predicted_matches.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      514 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/crosswalk/raw_df_a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      526 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/crosswalk/raw_df_b.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       67 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/female.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1034 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/ha_source.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      687 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/handle_null.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1272 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/hb_source.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     7441 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/hh_matching_a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     8135 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/hh_matching_b.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       82 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/hh_predicted_matches_reporting.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      231 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/hh_year_a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      290 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/hh_year_b.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    35038 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/hhpm_agg_test.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    12461 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/households_b.parquet
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       99 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/integration_a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      102 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/integration_b.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      283 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/jw_blocking_test_a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      112 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/jw_blocking_test_b.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       32 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/male.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1893 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/matched_men.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3479 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/matching_test_a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1614 2022-12-08 21:42:42.000000 hlink-3.5.4/hlink/tests/input_data/matching_test_b.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      196 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/nativity_test_data_a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      208 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/nativity_test_data_b.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    87678 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/new_hh_test_td.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      255 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/popularity.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3712 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/potential_matches.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4634 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/potential_matches_agg.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       75 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/potential_matches_ids_only.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      254 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/potential_matches_sql_condition_marst_warn.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       82 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/predicted_matches_reporting.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      332 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/predicted_matches_test.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1068 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/prepped_df_reporting.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      534 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/raw_df_reporting.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1022 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/region.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      361 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/regioncode.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    39511 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/rel_rows_test_a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    33360 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/rel_rows_test_b.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       75 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/reporting_hh_predicted_matches.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      102 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/reporting_predicted_matches.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      302 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/reporting_prepped_df_a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     6834 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/representivity.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      379 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/scored_matches_household_test.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      109 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/scored_matches_test_data.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      304 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/sql_condition_marst_warn_a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      227 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/sql_condition_marst_warn_b.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    46345 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/statedist.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     6776 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/street_abbrevs.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      820 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/street_abbrevs_most_common.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       90 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/test_csv_data_a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       88 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/test_csv_data_b.csv
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:28.275671 hlink-3.5.4/hlink/tests/input_data/test_parquet_data_a.parquet/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        8 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/test_parquet_data_a.parquet/._SUCCESS.crc
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       20 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/test_parquet_data_a.parquet/.part-00000-8465f06e-9bb0-4817-81eb-813ccf07429a-c000.snappy.parquet.crc
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/test_parquet_data_a.parquet/_SUCCESS
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1140 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/test_parquet_data_a.parquet/part-00000-8465f06e-9bb0-4817-81eb-813ccf07429a-c000.snappy.parquet
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:28.309850 hlink-3.5.4/hlink/tests/input_data/test_parquet_data_b.parquet/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        8 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/test_parquet_data_b.parquet/._SUCCESS.crc
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       20 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/test_parquet_data_b.parquet/.part-00000-bb515275-04b4-4a16-80f1-5cc21450b93f-c000.snappy.parquet.crc
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/test_parquet_data_b.parquet/_SUCCESS
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1116 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/test_parquet_data_b.parquet/part-00000-bb515275-04b4-4a16-80f1-5cc21450b93f-c000.snappy.parquet
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       94 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/test_prepped_data_a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       97 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/test_prepped_data_b.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      159 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/test_street_names_data.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      234 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/threshold_ratio_test.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      191 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/threshold_ratio_test_data_2.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       99 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/training_data.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      180 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/training_data_doubled.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     5567 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/training_data_households.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    13866 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/training_data_households.parquet
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1863 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/training_data_long.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1527 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/training_data_long_a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1472 2022-12-08 21:42:43.000000 hlink-3.5.4/hlink/tests/input_data/training_data_long_b.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    36252 2023-10-03 14:42:19.000000 hlink-3.5.4/hlink/tests/integration_score_with_trained_models_test.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1488 2022-12-08 21:42:44.000000 hlink-3.5.4/hlink/tests/integration_test.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      395 2022-12-08 21:42:44.000000 hlink-3.5.4/hlink/tests/linking_util_test.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      514 2022-12-08 21:42:44.000000 hlink-3.5.4/hlink/tests/logging_test.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     4973 2022-12-09 21:06:41.000000 hlink-3.5.4/hlink/tests/main_loop_test.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     9905 2023-10-31 13:38:40.000000 hlink-3.5.4/hlink/tests/main_test.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     4216 2022-12-09 21:06:41.000000 hlink-3.5.4/hlink/tests/matching_blocking_explode_test.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    42082 2022-12-09 21:06:41.000000 hlink-3.5.4/hlink/tests/matching_comparison_features_test.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    14145 2022-12-09 21:06:41.000000 hlink-3.5.4/hlink/tests/matching_geo_distance_test.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     3065 2022-12-08 21:42:44.000000 hlink-3.5.4/hlink/tests/matching_potential_matches_test.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     2624 2022-12-08 21:42:44.000000 hlink-3.5.4/hlink/tests/matching_potential_matches_universe_test.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     6715 2022-12-09 21:06:41.000000 hlink-3.5.4/hlink/tests/matching_scoring_test.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     7109 2023-10-31 13:38:40.000000 hlink-3.5.4/hlink/tests/matching_test.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    23930 2023-11-01 21:30:51.000000 hlink-3.5.4/hlink/tests/model_exploration_test.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:28.336595 hlink-3.5.4/hlink/tests/plugins/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:44.000000 hlink-3.5.4/hlink/tests/plugins/__init__.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    31942 2023-10-16 18:49:31.000000 hlink-3.5.4/hlink/tests/plugins/datasources.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    12650 2022-12-09 21:06:42.000000 hlink-3.5.4/hlink/tests/plugins/external_data_paths.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    63730 2023-10-31 13:38:40.000000 hlink-3.5.4/hlink/tests/preprocessing_test.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3510 2023-10-31 13:38:40.000000 hlink-3.5.4/hlink/tests/reporting_test.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1163 2022-12-08 21:42:44.000000 hlink-3.5.4/hlink/tests/scala_udf_test.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2490 2022-12-09 21:06:42.000000 hlink-3.5.4/hlink/tests/table_test.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    12761 2023-11-01 21:30:51.000000 hlink-3.5.4/hlink/tests/training_test.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:24.817746 hlink-3.5.4/hlink/tests/validation_data/
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:28.354115 hlink-3.5.4/hlink/tests/validation_data/crosswalks/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      106 2022-12-08 21:42:44.000000 hlink-3.5.4/hlink/tests/validation_data/crosswalks/crosswalk.csv
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)      126 2022-12-08 21:42:44.000000 hlink-3.5.4/hlink/tests/validation_data/crosswalks/crosswalk_with_round.csv
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:28.387915 hlink-3.5.4/hlink/tests/validation_data/training_p_all.parquet/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        8 2022-12-08 21:42:44.000000 hlink-3.5.4/hlink/tests/validation_data/training_p_all.parquet/._SUCCESS.crc
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      116 2022-12-08 21:42:44.000000 hlink-3.5.4/hlink/tests/validation_data/training_p_all.parquet/.part-00000-6c9e5760-174a-4652-b687-6823087ed5bf-c000.snappy.parquet.crc
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:44.000000 hlink-3.5.4/hlink/tests/validation_data/training_p_all.parquet/_SUCCESS
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    13348 2022-12-08 21:42:44.000000 hlink-3.5.4/hlink/tests/validation_data/training_p_all.parquet/part-00000-6c9e5760-174a-4652-b687-6823087ed5bf-c000.snappy.parquet
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:28.826919 hlink-3.5.4/hlink.egg-info/
--rw-r--r--   0 rileyh   (42243) rileyh   (23521)    26257 2024-02-20 20:30:23.000000 hlink-3.5.4/hlink.egg-info/PKG-INFO
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    14972 2024-02-20 20:30:24.000000 hlink-3.5.4/hlink.egg-info/SOURCES.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        1 2024-02-20 20:30:23.000000 hlink-3.5.4/hlink.egg-info/dependency_links.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       49 2024-02-20 20:30:23.000000 hlink-3.5.4/hlink.egg-info/entry_points.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      238 2024-02-20 20:30:23.000000 hlink-3.5.4/hlink.egg-info/requires.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       19 2024-02-20 20:30:23.000000 hlink-3.5.4/hlink.egg-info/top_level.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1573 2024-02-20 20:19:27.000000 hlink-3.5.4/pyproject.toml
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      110 2022-12-08 21:42:44.000000 hlink-3.5.4/pytest.ini
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:28.409421 hlink-3.5.4/scala_jar/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3774 2023-10-03 14:41:03.000000 hlink-3.5.4/scala_jar/build.sbt
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:28.447080 hlink-3.5.4/scala_jar/project/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      277 2022-12-08 21:42:44.000000 hlink-3.5.4/scala_jar/project/assembly.sbt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       18 2022-12-08 21:42:44.000000 hlink-3.5.4/scala_jar/project/build.properties
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:24.828261 hlink-3.5.4/scala_jar/src/
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:24.831555 hlink-3.5.4/scala_jar/src/main/
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:24.836927 hlink-3.5.4/scala_jar/src/main/scala/
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:24.841175 hlink-3.5.4/scala_jar/src/main/scala/com/
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:24.845353 hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:28.658911 hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      535 2022-12-08 21:42:44.000000 hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/ArrayToString.scala
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2249 2022-12-08 21:42:44.000000 hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/AttachHHColumn.scala
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     3382 2022-12-08 21:42:44.000000 hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/AttachRelatedRows.scala
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3170 2022-12-08 21:42:44.000000 hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/ExtraChildren.scala
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      556 2022-12-08 21:42:44.000000 hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/ExtractNeighbors.scala
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1494 2022-12-08 21:42:44.000000 hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/HHCompare.scala
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      703 2022-12-08 21:42:44.000000 hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/HHDrop.scala
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)      764 2022-12-08 21:42:44.000000 hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/HHGetFirstValue.scala
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      889 2022-12-08 21:42:44.000000 hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/HasMatchingElement.scala
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      473 2022-12-08 21:42:44.000000 hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/JWCompare.scala
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      898 2022-12-08 21:42:44.000000 hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/JWRate.scala
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1689 2022-12-08 21:42:44.000000 hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/JWRelatedRows.scala
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      662 2022-12-08 21:42:44.000000 hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/MaxJWCompare.scala
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      549 2022-12-08 21:42:44.000000 hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/ParseProbabilityVector.scala
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1272 2022-12-08 21:42:45.000000 hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/SerJaroWinklerSimilarity.scala
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      545 2022-12-08 21:42:45.000000 hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/VectorToString.scala
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       38 2024-02-20 20:30:28.846126 hlink-3.5.4/setup.cfg
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-02-20 20:30:28.813704 hlink-3.5.4/sphinx-docs/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      692 2022-12-08 21:42:45.000000 hlink-3.5.4/sphinx-docs/Makefile
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    10184 2023-12-06 16:40:14.000000 hlink-3.5.4/sphinx-docs/column_mappings.md
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    39349 2023-10-16 18:49:31.000000 hlink-3.5.4/sphinx-docs/comparison_types.md
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2099 2023-10-31 13:38:40.000000 hlink-3.5.4/sphinx-docs/conf.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    30395 2023-12-06 16:40:14.000000 hlink-3.5.4/sphinx-docs/config.md
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2773 2022-12-08 21:42:45.000000 hlink-3.5.4/sphinx-docs/feature_selection_transforms.md
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      741 2023-12-06 16:40:14.000000 hlink-3.5.4/sphinx-docs/index.rst
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1004 2023-11-01 19:00:05.000000 hlink-3.5.4/sphinx-docs/installation.md
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2574 2022-12-08 21:42:45.000000 hlink-3.5.4/sphinx-docs/introduction.md
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     7637 2023-12-06 16:40:14.000000 hlink-3.5.4/sphinx-docs/link_tasks.md
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      795 2022-12-08 21:42:45.000000 hlink-3.5.4/sphinx-docs/make.bat
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3703 2023-10-03 19:12:11.000000 hlink-3.5.4/sphinx-docs/models.md
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1731 2022-12-08 21:42:45.000000 hlink-3.5.4/sphinx-docs/pipeline_features.md
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    11301 2022-12-08 21:42:45.000000 hlink-3.5.4/sphinx-docs/running_the_program.md
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1978 2022-12-08 21:42:45.000000 hlink-3.5.4/sphinx-docs/substitutions.md
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     7114 2022-12-08 21:42:45.000000 hlink-3.5.4/sphinx-docs/use_examples.md
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:09.962757 hlink-3.5.5/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       38 2022-12-08 21:42:38.000000 hlink-3.5.5/.dockerignore
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      185 2023-10-31 13:38:40.000000 hlink-3.5.5/.flake8
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:06.332024 hlink-3.5.5/.github/
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:06.598175 hlink-3.5.5/.github/workflows/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1120 2023-10-31 13:38:40.000000 hlink-3.5.5/.github/workflows/docker-build.yml
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      244 2022-12-08 21:42:38.000000 hlink-3.5.5/.gitignore
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      365 2022-12-08 21:42:38.000000 hlink-3.5.5/.pre-commit-config.yaml
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      226 2023-10-02 20:36:04.000000 hlink-3.5.5/Dockerfile
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    16726 2022-12-08 21:42:38.000000 hlink-3.5.5/LICENSE.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      615 2022-12-13 16:10:13.000000 hlink-3.5.5/NOTICE.txt
+-rw-r--r--   0 rileyh   (42243) rileyh   (23521)    26257 2024-05-31 17:40:09.956911 hlink-3.5.5/PKG-INFO
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     5188 2023-11-01 19:00:05.000000 hlink-3.5.5/README.md
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      107 2022-12-13 16:04:48.000000 hlink-3.5.5/conftest.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:06.606729 hlink-3.5.5/doc/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4004 2023-10-03 19:12:10.000000 hlink-3.5.5/doc/developer.md
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:06.750609 hlink-3.5.5/docs/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      230 2024-05-31 17:29:00.000000 hlink-3.5.5/docs/.buildinfo
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:07.283817 hlink-3.5.5/docs/.doctrees/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    42484 2023-10-12 15:50:11.000000 hlink-3.5.5/docs/.doctrees/column_mapping_transforms.doctree
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)   163686 2023-10-12 15:50:11.000000 hlink-3.5.5/docs/.doctrees/comparison_types.doctree
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)   135404 2023-10-12 15:50:11.000000 hlink-3.5.5/docs/.doctrees/config.doctree
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    85920 2023-10-12 15:50:11.000000 hlink-3.5.5/docs/.doctrees/environment.pickle
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     5278 2023-10-12 15:50:11.000000 hlink-3.5.5/docs/.doctrees/example_workflow.doctree
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4591 2023-10-12 15:50:11.000000 hlink-3.5.5/docs/.doctrees/feature_selection_transforms.doctree
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     5278 2023-10-12 15:50:11.000000 hlink-3.5.5/docs/.doctrees/index.doctree
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     8241 2023-10-12 15:50:11.000000 hlink-3.5.5/docs/.doctrees/installation.doctree
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     9987 2023-10-12 15:50:11.000000 hlink-3.5.5/docs/.doctrees/introduction.doctree
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    10613 2023-10-12 15:50:11.000000 hlink-3.5.5/docs/.doctrees/link_tasks.doctree
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    21501 2023-10-12 15:50:11.000000 hlink-3.5.5/docs/.doctrees/models.doctree
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     8890 2023-10-12 15:50:11.000000 hlink-3.5.5/docs/.doctrees/pipeline_features.doctree
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    38499 2023-10-12 15:50:11.000000 hlink-3.5.5/docs/.doctrees/running_the_program.doctree
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    13195 2023-10-12 15:50:11.000000 hlink-3.5.5/docs/.doctrees/substitutions.doctree
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    30048 2023-10-12 15:50:11.000000 hlink-3.5.5/docs/.doctrees/use_examples.doctree
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2023-10-12 15:50:11.000000 hlink-3.5.5/docs/.nojekyll
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       20 2023-10-12 15:50:11.000000 hlink-3.5.5/docs/CNAME
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:07.460359 hlink-3.5.5/docs/_sources/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    10184 2023-12-01 18:23:26.000000 hlink-3.5.5/docs/_sources/column_mappings.md.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    39349 2023-10-16 18:49:31.000000 hlink-3.5.5/docs/_sources/comparison_types.md.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    30395 2023-12-01 18:18:19.000000 hlink-3.5.5/docs/_sources/config.md.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2793 2024-05-30 21:38:13.000000 hlink-3.5.5/docs/_sources/feature_selection_transforms.md.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      741 2023-12-01 18:18:19.000000 hlink-3.5.5/docs/_sources/index.rst.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1004 2023-11-01 19:00:05.000000 hlink-3.5.5/docs/_sources/installation.md.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2574 2022-12-08 21:42:45.000000 hlink-3.5.5/docs/_sources/introduction.md.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     7637 2023-12-01 18:18:19.000000 hlink-3.5.5/docs/_sources/link_tasks.md.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3703 2023-10-03 19:12:11.000000 hlink-3.5.5/docs/_sources/models.md.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1731 2022-12-08 21:42:45.000000 hlink-3.5.5/docs/_sources/pipeline_features.md.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    11301 2022-12-08 21:42:45.000000 hlink-3.5.5/docs/_sources/running_the_program.md.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1978 2022-12-08 21:42:45.000000 hlink-3.5.5/docs/_sources/substitutions.md.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     7114 2022-12-08 21:42:45.000000 hlink-3.5.5/docs/_sources/use_examples.md.txt
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:07.612497 hlink-3.5.5/docs/_static/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4418 2023-08-08 15:35:44.000000 hlink-3.5.5/docs/_static/_sphinx_javascript_frameworks_compat.js
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    11143 2024-05-31 17:14:19.000000 hlink-3.5.5/docs/_static/alabaster.css
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    15096 2024-05-31 17:14:19.000000 hlink-3.5.5/docs/_static/basic.css
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       42 2023-08-08 15:32:32.000000 hlink-3.5.5/docs/_static/custom.css
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4472 2024-02-20 19:59:37.000000 hlink-3.5.5/docs/_static/doctools.js
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      328 2024-05-31 17:29:00.000000 hlink-3.5.5/docs/_static/documentation_options.js
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      286 2023-10-31 13:43:49.000000 hlink-3.5.5/docs/_static/file.png
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)   287630 2022-03-02 16:32:08.000000 hlink-3.5.5/docs/_static/jquery-3.5.1.js
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)   288580 2023-08-08 15:35:44.000000 hlink-3.5.5/docs/_static/jquery-3.6.0.js
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    89476 2022-03-02 16:32:08.000000 hlink-3.5.5/docs/_static/jquery.js
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4758 2024-05-31 17:14:19.000000 hlink-3.5.5/docs/_static/language_data.js
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       90 2023-10-31 13:43:49.000000 hlink-3.5.5/docs/_static/minus.png
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       90 2023-10-31 13:43:49.000000 hlink-3.5.5/docs/_static/plus.png
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     5359 2024-05-31 17:14:19.000000 hlink-3.5.5/docs/_static/pygments.css
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    18732 2024-02-20 19:59:37.000000 hlink-3.5.5/docs/_static/searchtools.js
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     5123 2023-10-31 13:43:49.000000 hlink-3.5.5/docs/_static/sphinx_highlight.js
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    68420 2022-03-02 16:32:08.000000 hlink-3.5.5/docs/_static/underscore-1.13.1.js
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    19530 2022-03-02 16:32:08.000000 hlink-3.5.5/docs/_static/underscore.js
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    33865 2024-05-31 17:29:00.000000 hlink-3.5.5/docs/column_mappings.html
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)   124690 2024-05-31 17:29:00.000000 hlink-3.5.5/docs/comparison_types.html
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)   100403 2024-05-31 17:29:00.000000 hlink-3.5.5/docs/config.html
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    14090 2024-05-31 17:29:00.000000 hlink-3.5.5/docs/feature_selection_transforms.html
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3629 2024-05-31 17:29:00.000000 hlink-3.5.5/docs/genindex.html
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    12376 2024-05-31 17:29:00.000000 hlink-3.5.5/docs/index.html
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     6488 2024-05-31 17:29:00.000000 hlink-3.5.5/docs/installation.html
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     7686 2024-05-31 17:29:00.000000 hlink-3.5.5/docs/introduction.html
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    19893 2024-05-31 17:29:00.000000 hlink-3.5.5/docs/link_tasks.html
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    14220 2024-05-31 17:29:00.000000 hlink-3.5.5/docs/models.html
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      528 2024-05-31 17:29:00.000000 hlink-3.5.5/docs/objects.inv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     9451 2024-05-31 17:29:00.000000 hlink-3.5.5/docs/pipeline_features.html
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    25938 2024-05-31 17:29:00.000000 hlink-3.5.5/docs/running_the_program.html
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3906 2024-05-31 17:29:00.000000 hlink-3.5.5/docs/search.html
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    37115 2024-05-31 17:29:00.000000 hlink-3.5.5/docs/searchindex.js
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     9778 2024-05-31 17:29:00.000000 hlink-3.5.5/docs/substitutions.html
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    22557 2024-05-31 17:29:00.000000 hlink-3.5.5/docs/use_examples.html
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:06.350823 hlink-3.5.5/examples/
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:07.643999 hlink-3.5.5/examples/tutorial/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       29 2022-12-08 21:42:39.000000 hlink-3.5.5/examples/tutorial/.gitignore
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     6627 2022-12-08 21:42:39.000000 hlink-3.5.5/examples/tutorial/README.md
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:07.659264 hlink-3.5.5/examples/tutorial/data/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      285 2022-12-08 21:42:39.000000 hlink-3.5.5/examples/tutorial/data/A.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      226 2022-12-08 21:42:39.000000 hlink-3.5.5/examples/tutorial/data/B.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2985 2022-12-09 21:06:40.000000 hlink-3.5.5/examples/tutorial/tutorial.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1012 2022-12-08 21:42:39.000000 hlink-3.5.5/examples/tutorial/tutorial_config.toml
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:07.671888 hlink-3.5.5/hlink/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:39.000000 hlink-3.5.5/hlink/__init__.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:07.746476 hlink-3.5.5/hlink/configs/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:39.000000 hlink-3.5.5/hlink/configs/__init__.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     2172 2022-12-09 21:06:40.000000 hlink-3.5.5/hlink/configs/load_config.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)      479 2022-12-13 16:04:48.000000 hlink-3.5.5/hlink/errors.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:07.804248 hlink-3.5.5/hlink/linking/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      718 2022-12-08 21:42:39.000000 hlink-3.5.5/hlink/linking/README.md
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:39.000000 hlink-3.5.5/hlink/linking/__init__.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:07.880932 hlink-3.5.5/hlink/linking/core/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:39.000000 hlink-3.5.5/hlink/linking/core/__init__.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3406 2022-12-09 21:06:40.000000 hlink-3.5.5/hlink/linking/core/classifier.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     2219 2023-12-06 16:40:14.000000 hlink-3.5.5/hlink/linking/core/column_mapping.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     3083 2023-10-31 13:38:40.000000 hlink-3.5.5/hlink/linking/core/comparison.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    23236 2023-12-06 16:59:55.000000 hlink-3.5.5/hlink/linking/core/comparison_feature.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4196 2022-12-08 21:42:39.000000 hlink-3.5.5/hlink/linking/core/dist_table.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     8788 2023-11-01 21:30:51.000000 hlink-3.5.5/hlink/linking/core/pipeline.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3865 2022-12-09 21:06:40.000000 hlink-3.5.5/hlink/linking/core/substitutions.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4082 2023-10-30 19:42:28.000000 hlink-3.5.5/hlink/linking/core/threshold.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    22688 2024-05-31 17:09:25.000000 hlink-3.5.5/hlink/linking/core/transforms.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:07.913205 hlink-3.5.5/hlink/linking/hh_matching/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      265 2022-12-08 21:42:40.000000 hlink-3.5.5/hlink/linking/hh_matching/__init__.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      804 2022-12-09 21:06:40.000000 hlink-3.5.5/hlink/linking/hh_matching/hh_matching.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3229 2022-12-08 21:42:40.000000 hlink-3.5.5/hlink/linking/hh_matching/link_step_block_on_households.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2234 2022-12-09 21:06:40.000000 hlink-3.5.5/hlink/linking/hh_matching/link_step_filter.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:07.927720 hlink-3.5.5/hlink/linking/hh_matching/templates/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      413 2022-12-08 21:42:40.000000 hlink-3.5.5/hlink/linking/hh_matching/templates/hh_blocked_matches.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      566 2022-12-08 21:42:40.000000 hlink-3.5.5/hlink/linking/hh_matching/templates/hh_potential_matches.sql
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:07.942824 hlink-3.5.5/hlink/linking/hh_model_exploration/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      282 2022-12-08 21:42:40.000000 hlink-3.5.5/hlink/linking/hh_model_exploration/__init__.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      992 2022-12-09 21:06:40.000000 hlink-3.5.5/hlink/linking/hh_model_exploration/hh_model_exploration.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:07.950510 hlink-3.5.5/hlink/linking/hh_model_exploration/templates/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:40.000000 hlink-3.5.5/hlink/linking/hh_model_exploration/templates/.gitkeep
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:07.964054 hlink-3.5.5/hlink/linking/hh_training/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      265 2022-12-08 21:42:40.000000 hlink-3.5.5/hlink/linking/hh_training/__init__.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      940 2022-12-09 21:06:40.000000 hlink-3.5.5/hlink/linking/hh_training/hh_training.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:07.972019 hlink-3.5.5/hlink/linking/hh_training/templates/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:40.000000 hlink-3.5.5/hlink/linking/hh_training/templates/.gitkeep
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4518 2022-12-09 21:06:40.000000 hlink-3.5.5/hlink/linking/link_run.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1699 2023-11-20 22:19:38.000000 hlink-3.5.5/hlink/linking/link_step.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     6887 2023-10-31 13:38:40.000000 hlink-3.5.5/hlink/linking/link_task.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:08.019198 hlink-3.5.5/hlink/linking/matching/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      260 2022-12-08 21:42:40.000000 hlink-3.5.5/hlink/linking/matching/__init__.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      519 2022-12-08 21:42:40.000000 hlink-3.5.5/hlink/linking/matching/_helpers.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     7185 2024-02-20 19:22:56.000000 hlink-3.5.5/hlink/linking/matching/link_step_explode.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4228 2022-12-09 21:06:40.000000 hlink-3.5.5/hlink/linking/matching/link_step_match.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     8555 2023-10-23 19:28:03.000000 hlink-3.5.5/hlink/linking/matching/link_step_score.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      658 2022-12-09 21:06:40.000000 hlink-3.5.5/hlink/linking/matching/matching.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:08.039905 hlink-3.5.5/hlink/linking/matching/templates/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      772 2022-12-08 21:42:40.000000 hlink-3.5.5/hlink/linking/matching/templates/potential_matches.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      404 2022-12-08 21:42:40.000000 hlink-3.5.5/hlink/linking/matching/templates/potential_matches_count.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      503 2022-12-08 21:42:40.000000 hlink-3.5.5/hlink/linking/matching/templates/potential_matches_universe.sql
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:08.076350 hlink-3.5.5/hlink/linking/model_exploration/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      277 2022-12-08 21:42:40.000000 hlink-3.5.5/hlink/linking/model_exploration/__init__.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4731 2022-12-09 21:06:40.000000 hlink-3.5.5/hlink/linking/model_exploration/link_step_create_features.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      872 2022-12-08 21:42:40.000000 hlink-3.5.5/hlink/linking/model_exploration/link_step_ingest_file.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    21393 2022-12-13 16:04:48.000000 hlink-3.5.5/hlink/linking/model_exploration/link_step_train_test_models.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      828 2023-10-23 19:28:03.000000 hlink-3.5.5/hlink/linking/model_exploration/model_exploration.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:08.083913 hlink-3.5.5/hlink/linking/model_exploration/templates/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:40.000000 hlink-3.5.5/hlink/linking/model_exploration/templates/.gitkeep
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:08.142526 hlink-3.5.5/hlink/linking/preprocessing/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      270 2022-12-08 21:42:40.000000 hlink-3.5.5/hlink/linking/preprocessing/__init__.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4431 2023-11-16 18:36:06.000000 hlink-3.5.5/hlink/linking/preprocessing/link_step_prep_dataframes.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     8308 2023-11-16 18:36:06.000000 hlink-3.5.5/hlink/linking/preprocessing/link_step_register_raw_dfs.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      509 2022-12-09 21:06:41.000000 hlink-3.5.5/hlink/linking/preprocessing/preprocessing.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:08.198437 hlink-3.5.5/hlink/linking/preprocessing/templates/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      431 2022-12-08 21:42:40.000000 hlink-3.5.5/hlink/linking/preprocessing/templates/attach_family_col.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      359 2022-12-08 21:42:40.000000 hlink-3.5.5/hlink/linking/preprocessing/templates/attach_neighbor_col.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      660 2022-12-08 21:42:40.000000 hlink-3.5.5/hlink/linking/preprocessing/templates/attach_related_col.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      885 2022-12-08 21:42:40.000000 hlink-3.5.5/hlink/linking/preprocessing/templates/attach_related_cols_as_rows.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      471 2022-12-08 21:42:40.000000 hlink-3.5.5/hlink/linking/preprocessing/templates/hh_nbor.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      738 2022-12-08 21:42:40.000000 hlink-3.5.5/hlink/linking/preprocessing/templates/hh_nbor_rank.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      430 2022-12-08 21:42:40.000000 hlink-3.5.5/hlink/linking/preprocessing/templates/training_data_subset.sql
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:08.235292 hlink-3.5.5/hlink/linking/reporting/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      262 2022-12-08 21:42:40.000000 hlink-3.5.5/hlink/linking/reporting/__init__.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2874 2022-12-13 16:04:48.000000 hlink-3.5.5/hlink/linking/reporting/link_step_export_crosswalk.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3664 2022-12-09 21:06:41.000000 hlink-3.5.5/hlink/linking/reporting/link_step_report_r2_percent_linked.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    24145 2022-12-13 16:04:48.000000 hlink-3.5.5/hlink/linking/reporting/link_step_report_representivity.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      687 2022-12-09 21:06:41.000000 hlink-3.5.5/hlink/linking/reporting/reporting.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:08.243727 hlink-3.5.5/hlink/linking/reporting/templates/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.5.5/hlink/linking/reporting/templates/.gitkeep
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1817 2022-12-09 17:39:25.000000 hlink-3.5.5/hlink/linking/table.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4001 2023-10-26 14:28:01.000000 hlink-3.5.5/hlink/linking/table_definitions.csv
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:06.415608 hlink-3.5.5/hlink/linking/templates/
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:08.329428 hlink-3.5.5/hlink/linking/templates/shared/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1003 2022-12-08 21:42:41.000000 hlink-3.5.5/hlink/linking/templates/shared/aggregate_features.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1201 2022-12-08 21:42:41.000000 hlink-3.5.5/hlink/linking/templates/shared/all_household_members.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      374 2022-12-08 21:42:41.000000 hlink-3.5.5/hlink/linking/templates/shared/attach_variable.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1021 2022-12-08 21:42:41.000000 hlink-3.5.5/hlink/linking/templates/shared/drop_links.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2205 2022-12-08 21:42:41.000000 hlink-3.5.5/hlink/linking/templates/shared/hh_aggregate_features.sql
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:08.345932 hlink-3.5.5/hlink/linking/templates/shared/includes/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1586 2022-12-08 21:42:41.000000 hlink-3.5.5/hlink/linking/templates/shared/includes/all_household_members_selects_a.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1600 2022-12-08 21:42:41.000000 hlink-3.5.5/hlink/linking/templates/shared/includes/all_household_members_selects_b.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      487 2022-12-08 21:42:41.000000 hlink-3.5.5/hlink/linking/templates/shared/pl_easy_features.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      653 2022-12-08 21:42:41.000000 hlink-3.5.5/hlink/linking/templates/shared/potential_matches_base_features.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      412 2022-12-08 21:42:41.000000 hlink-3.5.5/hlink/linking/templates/shared/scored_potential_matches.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      420 2022-12-08 21:42:41.000000 hlink-3.5.5/hlink/linking/templates/shared/select_columns.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      591 2022-12-08 21:42:41.000000 hlink-3.5.5/hlink/linking/templates/shared/tfam_tables.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      702 2022-12-08 21:42:41.000000 hlink-3.5.5/hlink/linking/templates/shared/training_features.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      510 2022-12-08 21:42:41.000000 hlink-3.5.5/hlink/linking/templates/shared/training_prepped.sql
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:08.415337 hlink-3.5.5/hlink/linking/training/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      260 2022-12-08 21:42:41.000000 hlink-3.5.5/hlink/linking/training/__init__.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3834 2022-12-09 21:06:41.000000 hlink-3.5.5/hlink/linking/training/link_step_create_comparison_features.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      872 2022-12-08 21:42:41.000000 hlink-3.5.5/hlink/linking/training/link_step_ingest_file.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     5323 2023-10-26 14:44:11.000000 hlink-3.5.5/hlink/linking/training/link_step_save_model_metadata.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3230 2023-10-26 14:28:01.000000 hlink-3.5.5/hlink/linking/training/link_step_train_and_save_model.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:08.423971 hlink-3.5.5/hlink/linking/training/templates/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.5.5/hlink/linking/training/templates/.gitkeep
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      927 2023-10-23 19:28:03.000000 hlink-3.5.5/hlink/linking/training/training.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:08.453271 hlink-3.5.5/hlink/linking/transformers/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.5.5/hlink/linking/transformers/__init__.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1202 2022-12-09 21:06:41.000000 hlink-3.5.5/hlink/linking/transformers/float_cast_transformer.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2821 2023-10-09 17:50:59.000000 hlink-3.5.5/hlink/linking/transformers/interaction_transformer.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      615 2022-12-09 21:06:41.000000 hlink-3.5.5/hlink/linking/transformers/rename_prob_column.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      648 2022-12-09 21:06:41.000000 hlink-3.5.5/hlink/linking/util.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:08.473095 hlink-3.5.5/hlink/scripts/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.5.5/hlink/scripts/__init__.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:08.536203 hlink-3.5.5/hlink/scripts/lib/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.5.5/hlink/scripts/lib/__init__.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    16597 2024-02-20 19:22:56.000000 hlink-3.5.5/hlink/scripts/lib/conf_validations.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:08.559107 hlink-3.5.5/hlink/scripts/lib/experimental/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.5.5/hlink/scripts/lib/experimental/__init__.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     4044 2022-12-13 16:04:48.000000 hlink-3.5.5/hlink/scripts/lib/experimental/reporting.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     8493 2022-12-08 21:42:41.000000 hlink-3.5.5/hlink/scripts/lib/experimental/tfam.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3252 2022-12-08 21:42:41.000000 hlink-3.5.5/hlink/scripts/lib/io.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2654 2023-10-31 13:38:40.000000 hlink-3.5.5/hlink/scripts/lib/linking_ops.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     5314 2023-08-09 20:43:52.000000 hlink-3.5.5/hlink/scripts/lib/table_ops.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      812 2022-12-09 21:06:41.000000 hlink-3.5.5/hlink/scripts/lib/util.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     8534 2023-11-02 15:30:46.000000 hlink-3.5.5/hlink/scripts/main.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    20808 2023-11-02 15:30:46.000000 hlink-3.5.5/hlink/scripts/main_loop.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:08.583851 hlink-3.5.5/hlink/spark/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.5.5/hlink/spark/__init__.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2494 2022-12-08 21:42:41.000000 hlink-3.5.5/hlink/spark/factory.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:08.592187 hlink-3.5.5/hlink/spark/jars/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)  6446850 2022-12-08 21:42:41.000000 hlink-3.5.5/hlink/spark/jars/hlink_lib-assembly-1.0.jar
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4786 2022-12-13 16:04:48.000000 hlink-3.5.5/hlink/spark/session.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:08.827437 hlink-3.5.5/hlink/tests/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.5.5/hlink/tests/__init__.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:08.924766 hlink-3.5.5/hlink/tests/conf/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      294 2023-10-30 19:42:28.000000 hlink-3.5.5/hlink/tests/conf/duplicate_col_maps.toml
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      720 2023-10-30 19:42:28.000000 hlink-3.5.5/hlink/tests/conf/duplicate_comp_features.toml
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      513 2023-10-30 19:42:29.000000 hlink-3.5.5/hlink/tests/conf/duplicate_feature_sel.toml
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1629 2022-12-08 21:42:41.000000 hlink-3.5.5/hlink/tests/conf/integration.toml
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       17 2022-12-08 21:42:41.000000 hlink-3.5.5/hlink/tests/conf/missing_datasource_a.toml
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       87 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/conf/missing_datasource_b.toml
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      258 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/conf/no_id_column_a.toml
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      258 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/conf/no_id_column_b.toml
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      123 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/conf/test.json
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       81 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/conf/test1.toml
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      133 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/conf/test_conf_flag_run.json
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      131 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/conf/test_run.json
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     7710 2024-02-20 19:22:56.000000 hlink-3.5.5/hlink/tests/conf_validations_test.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      920 2022-12-09 21:06:41.000000 hlink-3.5.5/hlink/tests/config_loader_test.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    49636 2022-12-13 16:04:48.000000 hlink-3.5.5/hlink/tests/conftest.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:08.966804 hlink-3.5.5/hlink/tests/core/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/core/__init__.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     9062 2023-12-06 16:40:14.000000 hlink-3.5.5/hlink/tests/core/column_mapping_test.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    14157 2023-10-16 18:49:31.000000 hlink-3.5.5/hlink/tests/core/comparison_feature_test.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1200 2023-10-16 18:49:31.000000 hlink-3.5.5/hlink/tests/core/pipeline_test.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2760 2024-05-31 17:09:25.000000 hlink-3.5.5/hlink/tests/core/transforms_test.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    10639 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/hh_matching_test.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4245 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/hh_model_exploration_test.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:09.489955 hlink-3.5.5/hlink/tests/input_data/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      706 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/19thc_nativity_test_hhs.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2250 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/19thc_nativity_test_hhs_a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      989 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/19thc_nativity_test_hhs_b.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      221 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/birthyr_replace.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      630 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/calc_mfbpl_a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      553 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/calc_mfbpl_b.csv
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:09.510468 hlink-3.5.5/hlink/tests/input_data/conf_validation/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       29 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/conf_validation/a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       29 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/conf_validation/b.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/conf_validation/empty.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      155 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/county_distances.csv
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:09.537655 hlink-3.5.5/hlink/tests/input_data/crosswalk/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       29 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/crosswalk/hh_predicted_matches.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       53 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/crosswalk/predicted_matches.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      514 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/crosswalk/raw_df_a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      526 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/crosswalk/raw_df_b.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       67 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/female.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1034 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/ha_source.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      687 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/handle_null.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1272 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/hb_source.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     7441 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/hh_matching_a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     8135 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/hh_matching_b.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       82 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/hh_predicted_matches_reporting.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      231 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/hh_year_a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      290 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/hh_year_b.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    35038 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/hhpm_agg_test.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    12461 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/households_b.parquet
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       99 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/integration_a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      102 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/integration_b.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      283 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/jw_blocking_test_a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      112 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/jw_blocking_test_b.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       32 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/male.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1893 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/matched_men.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3479 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/matching_test_a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1614 2022-12-08 21:42:42.000000 hlink-3.5.5/hlink/tests/input_data/matching_test_b.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      196 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/nativity_test_data_a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      208 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/nativity_test_data_b.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    87678 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/new_hh_test_td.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      255 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/popularity.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3712 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/potential_matches.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4634 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/potential_matches_agg.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       75 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/potential_matches_ids_only.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      254 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/potential_matches_sql_condition_marst_warn.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       82 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/predicted_matches_reporting.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      332 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/predicted_matches_test.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1068 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/prepped_df_reporting.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      534 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/raw_df_reporting.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1022 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/region.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      361 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/regioncode.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    39511 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/rel_rows_test_a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    33360 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/rel_rows_test_b.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       75 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/reporting_hh_predicted_matches.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      102 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/reporting_predicted_matches.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      302 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/reporting_prepped_df_a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     6834 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/representivity.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      379 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/scored_matches_household_test.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      109 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/scored_matches_test_data.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      304 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/sql_condition_marst_warn_a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      227 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/sql_condition_marst_warn_b.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    46345 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/statedist.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     6776 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/street_abbrevs.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      820 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/street_abbrevs_most_common.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       90 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/test_csv_data_a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       88 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/test_csv_data_b.csv
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:09.565076 hlink-3.5.5/hlink/tests/input_data/test_parquet_data_a.parquet/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        8 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/test_parquet_data_a.parquet/._SUCCESS.crc
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       20 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/test_parquet_data_a.parquet/.part-00000-8465f06e-9bb0-4817-81eb-813ccf07429a-c000.snappy.parquet.crc
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/test_parquet_data_a.parquet/_SUCCESS
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1140 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/test_parquet_data_a.parquet/part-00000-8465f06e-9bb0-4817-81eb-813ccf07429a-c000.snappy.parquet
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:09.592322 hlink-3.5.5/hlink/tests/input_data/test_parquet_data_b.parquet/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        8 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/test_parquet_data_b.parquet/._SUCCESS.crc
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       20 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/test_parquet_data_b.parquet/.part-00000-bb515275-04b4-4a16-80f1-5cc21450b93f-c000.snappy.parquet.crc
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/test_parquet_data_b.parquet/_SUCCESS
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1116 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/test_parquet_data_b.parquet/part-00000-bb515275-04b4-4a16-80f1-5cc21450b93f-c000.snappy.parquet
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       94 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/test_prepped_data_a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       97 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/test_prepped_data_b.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      159 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/test_street_names_data.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      234 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/threshold_ratio_test.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      191 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/threshold_ratio_test_data_2.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       99 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/training_data.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      180 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/training_data_doubled.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     5567 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/training_data_households.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    13866 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/training_data_households.parquet
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1863 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/training_data_long.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1527 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/training_data_long_a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1472 2022-12-08 21:42:43.000000 hlink-3.5.5/hlink/tests/input_data/training_data_long_b.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    36252 2023-10-03 14:42:19.000000 hlink-3.5.5/hlink/tests/integration_score_with_trained_models_test.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1488 2022-12-08 21:42:44.000000 hlink-3.5.5/hlink/tests/integration_test.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      395 2022-12-08 21:42:44.000000 hlink-3.5.5/hlink/tests/linking_util_test.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      514 2022-12-08 21:42:44.000000 hlink-3.5.5/hlink/tests/logging_test.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     4973 2022-12-09 21:06:41.000000 hlink-3.5.5/hlink/tests/main_loop_test.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     9905 2023-10-31 13:38:40.000000 hlink-3.5.5/hlink/tests/main_test.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     4216 2022-12-09 21:06:41.000000 hlink-3.5.5/hlink/tests/matching_blocking_explode_test.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    42082 2022-12-09 21:06:41.000000 hlink-3.5.5/hlink/tests/matching_comparison_features_test.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    14145 2022-12-09 21:06:41.000000 hlink-3.5.5/hlink/tests/matching_geo_distance_test.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     3065 2022-12-08 21:42:44.000000 hlink-3.5.5/hlink/tests/matching_potential_matches_test.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     2624 2022-12-08 21:42:44.000000 hlink-3.5.5/hlink/tests/matching_potential_matches_universe_test.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     6715 2022-12-09 21:06:41.000000 hlink-3.5.5/hlink/tests/matching_scoring_test.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     7109 2023-10-31 13:38:40.000000 hlink-3.5.5/hlink/tests/matching_test.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    23930 2023-11-01 21:30:51.000000 hlink-3.5.5/hlink/tests/model_exploration_test.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:09.614818 hlink-3.5.5/hlink/tests/plugins/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:44.000000 hlink-3.5.5/hlink/tests/plugins/__init__.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    31942 2023-10-16 18:49:31.000000 hlink-3.5.5/hlink/tests/plugins/datasources.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    12650 2022-12-09 21:06:42.000000 hlink-3.5.5/hlink/tests/plugins/external_data_paths.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    63730 2023-10-31 13:38:40.000000 hlink-3.5.5/hlink/tests/preprocessing_test.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3510 2023-10-31 13:38:40.000000 hlink-3.5.5/hlink/tests/reporting_test.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1163 2022-12-08 21:42:44.000000 hlink-3.5.5/hlink/tests/scala_udf_test.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2490 2022-12-09 21:06:42.000000 hlink-3.5.5/hlink/tests/table_test.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    12761 2023-11-01 21:30:51.000000 hlink-3.5.5/hlink/tests/training_test.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:06.475830 hlink-3.5.5/hlink/tests/validation_data/
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:09.628847 hlink-3.5.5/hlink/tests/validation_data/crosswalks/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      106 2022-12-08 21:42:44.000000 hlink-3.5.5/hlink/tests/validation_data/crosswalks/crosswalk.csv
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)      126 2022-12-08 21:42:44.000000 hlink-3.5.5/hlink/tests/validation_data/crosswalks/crosswalk_with_round.csv
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:09.657098 hlink-3.5.5/hlink/tests/validation_data/training_p_all.parquet/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        8 2022-12-08 21:42:44.000000 hlink-3.5.5/hlink/tests/validation_data/training_p_all.parquet/._SUCCESS.crc
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      116 2022-12-08 21:42:44.000000 hlink-3.5.5/hlink/tests/validation_data/training_p_all.parquet/.part-00000-6c9e5760-174a-4652-b687-6823087ed5bf-c000.snappy.parquet.crc
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:44.000000 hlink-3.5.5/hlink/tests/validation_data/training_p_all.parquet/_SUCCESS
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    13348 2022-12-08 21:42:44.000000 hlink-3.5.5/hlink/tests/validation_data/training_p_all.parquet/part-00000-6c9e5760-174a-4652-b687-6823087ed5bf-c000.snappy.parquet
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:09.944287 hlink-3.5.5/hlink.egg-info/
+-rw-r--r--   0 rileyh   (42243) rileyh   (23521)    26257 2024-05-31 17:40:05.000000 hlink-3.5.5/hlink.egg-info/PKG-INFO
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    15008 2024-05-31 17:40:06.000000 hlink-3.5.5/hlink.egg-info/SOURCES.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        1 2024-05-31 17:40:05.000000 hlink-3.5.5/hlink.egg-info/dependency_links.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       49 2024-05-31 17:40:05.000000 hlink-3.5.5/hlink.egg-info/entry_points.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      238 2024-05-31 17:40:05.000000 hlink-3.5.5/hlink.egg-info/requires.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       19 2024-05-31 17:40:05.000000 hlink-3.5.5/hlink.egg-info/top_level.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1573 2024-05-31 17:29:00.000000 hlink-3.5.5/pyproject.toml
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      110 2022-12-08 21:42:44.000000 hlink-3.5.5/pytest.ini
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:09.664306 hlink-3.5.5/scala_jar/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3774 2023-10-03 14:41:03.000000 hlink-3.5.5/scala_jar/build.sbt
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:09.678693 hlink-3.5.5/scala_jar/project/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      277 2022-12-08 21:42:44.000000 hlink-3.5.5/scala_jar/project/assembly.sbt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       18 2022-12-08 21:42:44.000000 hlink-3.5.5/scala_jar/project/build.properties
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:06.491437 hlink-3.5.5/scala_jar/src/
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:06.495561 hlink-3.5.5/scala_jar/src/main/
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:06.500123 hlink-3.5.5/scala_jar/src/main/scala/
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:06.503862 hlink-3.5.5/scala_jar/src/main/scala/com/
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:06.506731 hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:09.818798 hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      535 2022-12-08 21:42:44.000000 hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/ArrayToString.scala
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2249 2022-12-08 21:42:44.000000 hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/AttachHHColumn.scala
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     3382 2022-12-08 21:42:44.000000 hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/AttachRelatedRows.scala
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3170 2022-12-08 21:42:44.000000 hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/ExtraChildren.scala
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      556 2022-12-08 21:42:44.000000 hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/ExtractNeighbors.scala
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1494 2022-12-08 21:42:44.000000 hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/HHCompare.scala
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      703 2022-12-08 21:42:44.000000 hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/HHDrop.scala
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)      764 2022-12-08 21:42:44.000000 hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/HHGetFirstValue.scala
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      889 2022-12-08 21:42:44.000000 hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/HasMatchingElement.scala
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      473 2022-12-08 21:42:44.000000 hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/JWCompare.scala
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      898 2022-12-08 21:42:44.000000 hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/JWRate.scala
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1689 2022-12-08 21:42:44.000000 hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/JWRelatedRows.scala
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      662 2022-12-08 21:42:44.000000 hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/MaxJWCompare.scala
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      549 2022-12-08 21:42:44.000000 hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/ParseProbabilityVector.scala
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1272 2022-12-08 21:42:45.000000 hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/SerJaroWinklerSimilarity.scala
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      545 2022-12-08 21:42:45.000000 hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/VectorToString.scala
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       38 2024-05-31 17:40:09.964424 hlink-3.5.5/setup.cfg
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2024-05-31 17:40:09.934672 hlink-3.5.5/sphinx-docs/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      692 2022-12-08 21:42:45.000000 hlink-3.5.5/sphinx-docs/Makefile
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    10184 2023-12-06 16:40:14.000000 hlink-3.5.5/sphinx-docs/column_mappings.md
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    39349 2023-10-16 18:49:31.000000 hlink-3.5.5/sphinx-docs/comparison_types.md
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2099 2023-10-31 13:38:40.000000 hlink-3.5.5/sphinx-docs/conf.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    30395 2023-12-06 16:40:14.000000 hlink-3.5.5/sphinx-docs/config.md
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2793 2024-05-31 17:09:25.000000 hlink-3.5.5/sphinx-docs/feature_selection_transforms.md
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      741 2023-12-06 16:40:14.000000 hlink-3.5.5/sphinx-docs/index.rst
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1004 2023-11-01 19:00:05.000000 hlink-3.5.5/sphinx-docs/installation.md
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2574 2022-12-08 21:42:45.000000 hlink-3.5.5/sphinx-docs/introduction.md
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     7637 2023-12-06 16:40:14.000000 hlink-3.5.5/sphinx-docs/link_tasks.md
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      795 2022-12-08 21:42:45.000000 hlink-3.5.5/sphinx-docs/make.bat
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3703 2023-10-03 19:12:11.000000 hlink-3.5.5/sphinx-docs/models.md
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1731 2022-12-08 21:42:45.000000 hlink-3.5.5/sphinx-docs/pipeline_features.md
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    11301 2022-12-08 21:42:45.000000 hlink-3.5.5/sphinx-docs/running_the_program.md
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1978 2022-12-08 21:42:45.000000 hlink-3.5.5/sphinx-docs/substitutions.md
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     7114 2022-12-08 21:42:45.000000 hlink-3.5.5/sphinx-docs/use_examples.md
```

### Comparing `hlink-3.5.4/.github/workflows/docker-build.yml` & `hlink-3.5.5/.github/workflows/docker-build.yml`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/LICENSE.txt` & `hlink-3.5.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/NOTICE.txt` & `hlink-3.5.5/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/PKG-INFO` & `hlink-3.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hlink
-Version: 3.5.4
+Version: 3.5.5
 Summary: Fast supervised pyspark record linkage software
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
```

### Comparing `hlink-3.5.4/README.md` & `hlink-3.5.5/README.md`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/doc/developer.md` & `hlink-3.5.5/doc/developer.md`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/.doctrees/column_mapping_transforms.doctree` & `hlink-3.5.5/docs/.doctrees/column_mapping_transforms.doctree`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/.doctrees/comparison_types.doctree` & `hlink-3.5.5/docs/.doctrees/comparison_types.doctree`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/.doctrees/config.doctree` & `hlink-3.5.5/docs/.doctrees/config.doctree`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/.doctrees/environment.pickle` & `hlink-3.5.5/docs/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/.doctrees/example_workflow.doctree` & `hlink-3.5.5/docs/.doctrees/example_workflow.doctree`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/.doctrees/feature_selection_transforms.doctree` & `hlink-3.5.5/docs/.doctrees/feature_selection_transforms.doctree`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/.doctrees/index.doctree` & `hlink-3.5.5/docs/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/.doctrees/installation.doctree` & `hlink-3.5.5/docs/.doctrees/installation.doctree`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/.doctrees/introduction.doctree` & `hlink-3.5.5/docs/.doctrees/introduction.doctree`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/.doctrees/link_tasks.doctree` & `hlink-3.5.5/docs/.doctrees/link_tasks.doctree`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/.doctrees/models.doctree` & `hlink-3.5.5/docs/.doctrees/models.doctree`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/.doctrees/pipeline_features.doctree` & `hlink-3.5.5/docs/.doctrees/pipeline_features.doctree`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/.doctrees/running_the_program.doctree` & `hlink-3.5.5/docs/.doctrees/running_the_program.doctree`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/.doctrees/substitutions.doctree` & `hlink-3.5.5/docs/.doctrees/substitutions.doctree`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/.doctrees/use_examples.doctree` & `hlink-3.5.5/docs/.doctrees/use_examples.doctree`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/_sources/column_mappings.md.txt` & `hlink-3.5.5/docs/_sources/column_mappings.md.txt`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/_sources/comparison_types.md.txt` & `hlink-3.5.5/docs/_sources/comparison_types.md.txt`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/_sources/config.md.txt` & `hlink-3.5.5/docs/_sources/config.md.txt`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/_sources/feature_selection_transforms.md.txt` & `hlink-3.5.5/docs/_sources/feature_selection_transforms.md.txt`

 * *Files 2% similar despite different names*

```diff
@@ -42,18 +42,18 @@
 output_column = "replaced_birthyr"
 condition = "case when clean_birthyr is null or clean_birthyr == '' then year - age else clean_birthyr end"
 transform = "sql_condition"
 ```
 
 ## array
 
-Combine two input columns into an array output column.
+Combine any number of input columns into a single array output column.
 
 * Attributes:
-  * `input_columns` - Type: list of strings. Required. The two input columns.
+  * `input_columns` - Type: list of strings. Required. The list of input columns.
   * `output_column` - Type: `string`. Required.
 
 ```
 [[feature_selections]]
 input_columns = ["namelast_clean_bigrams", "namefrst_unstd_bigrams"]
 output_column = "namelast_frst_bigrams"
 transform = "array"
```

### Comparing `hlink-3.5.4/docs/_sources/index.rst.txt` & `hlink-3.5.5/docs/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/_sources/installation.md.txt` & `hlink-3.5.5/docs/_sources/installation.md.txt`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/_sources/introduction.md.txt` & `hlink-3.5.5/docs/_sources/introduction.md.txt`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/_sources/link_tasks.md.txt` & `hlink-3.5.5/docs/_sources/link_tasks.md.txt`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/_sources/models.md.txt` & `hlink-3.5.5/docs/_sources/models.md.txt`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/_sources/pipeline_features.md.txt` & `hlink-3.5.5/docs/_sources/pipeline_features.md.txt`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/_sources/running_the_program.md.txt` & `hlink-3.5.5/docs/_sources/running_the_program.md.txt`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/_sources/substitutions.md.txt` & `hlink-3.5.5/docs/_sources/substitutions.md.txt`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/_sources/use_examples.md.txt` & `hlink-3.5.5/docs/_sources/use_examples.md.txt`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/_static/_sphinx_javascript_frameworks_compat.js` & `hlink-3.5.5/docs/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/_static/alabaster.css` & `hlink-3.5.5/docs/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/_static/basic.css` & `hlink-3.5.5/docs/_static/basic.css`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/_static/doctools.js` & `hlink-3.5.5/docs/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/_static/jquery-3.5.1.js` & `hlink-3.5.5/docs/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/_static/jquery-3.6.0.js` & `hlink-3.5.5/docs/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/_static/jquery.js` & `hlink-3.5.5/docs/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/_static/language_data.js` & `hlink-3.5.5/docs/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/_static/pygments.css` & `hlink-3.5.5/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/_static/searchtools.js` & `hlink-3.5.5/docs/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/_static/sphinx_highlight.js` & `hlink-3.5.5/docs/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/_static/underscore-1.13.1.js` & `hlink-3.5.5/docs/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/_static/underscore.js` & `hlink-3.5.5/docs/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/docs/column_mappings.html` & `hlink-3.5.5/docs/column_mappings.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Column Mappings &#8212; hlink 3.5.4 documentation</title>
+    <title>Column Mappings &#8212; hlink 3.5.5 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=3d47302e"></script>
+    <script src="_static/documentation_options.js?v=993fb437"></script>
     <script src="_static/doctools.js?v=888ff710"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Comparison types, transform add-ons, aggregate features, and household aggregate features" href="comparison_types.html" />
     <link rel="prev" title="Configuration" href="config.html" />
```

### Comparing `hlink-3.5.4/docs/comparison_types.html` & `hlink-3.5.5/docs/comparison_types.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Comparison types, transform add-ons, aggregate features, and household aggregate features &#8212; hlink 3.5.4 documentation</title>
+    <title>Comparison types, transform add-ons, aggregate features, and household aggregate features &#8212; hlink 3.5.5 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=3d47302e"></script>
+    <script src="_static/documentation_options.js?v=993fb437"></script>
     <script src="_static/doctools.js?v=888ff710"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Feature Selection transforms" href="feature_selection_transforms.html" />
     <link rel="prev" title="Column Mappings" href="column_mappings.html" />
```

### Comparing `hlink-3.5.4/docs/config.html` & `hlink-3.5.5/docs/config.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Configuration &#8212; hlink 3.5.4 documentation</title>
+    <title>Configuration &#8212; hlink 3.5.5 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=3d47302e"></script>
+    <script src="_static/documentation_options.js?v=993fb437"></script>
     <script src="_static/doctools.js?v=888ff710"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Column Mappings" href="column_mappings.html" />
     <link rel="prev" title="Advanced Workflow Examples" href="use_examples.html" />
```

### Comparing `hlink-3.5.4/docs/feature_selection_transforms.html` & `hlink-3.5.5/docs/feature_selection_transforms.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Feature Selection transforms &#8212; hlink 3.5.4 documentation</title>
+    <title>Feature Selection transforms &#8212; hlink 3.5.5 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=3d47302e"></script>
+    <script src="_static/documentation_options.js?v=993fb437"></script>
     <script src="_static/doctools.js?v=888ff710"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Pipeline generated features" href="pipeline_features.html" />
     <link rel="prev" title="Comparison types, transform add-ons, aggregate features, and household aggregate features" href="comparison_types.html" />
    
@@ -79,19 +79,19 @@
 <span class="n">condition</span> <span class="o">=</span> <span class="s2">&quot;case when clean_birthyr is null or clean_birthyr == &#39;&#39; then year - age else clean_birthyr end&quot;</span>
 <span class="n">transform</span> <span class="o">=</span> <span class="s2">&quot;sql_condition&quot;</span>
 </pre></div>
 </div>
 </section>
 <section id="array">
 <h2>array<a class="headerlink" href="#array" title="Link to this heading">¶</a></h2>
-<p>Combine two input columns into an array output column.</p>
+<p>Combine any number of input columns into a single array output column.</p>
 <ul class="simple">
 <li><p>Attributes:</p>
 <ul>
-<li><p><code class="docutils literal notranslate"><span class="pre">input_columns</span></code> - Type: list of strings. Required. The two input columns.</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">input_columns</span></code> - Type: list of strings. Required. The list of input columns.</p></li>
 <li><p><code class="docutils literal notranslate"><span class="pre">output_column</span></code> - Type: <code class="docutils literal notranslate"><span class="pre">string</span></code>. Required.</p></li>
 </ul>
 </li>
 </ul>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="p">[[</span><span class="n">feature_selections</span><span class="p">]]</span>
 <span class="n">input_columns</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;namelast_clean_bigrams&quot;</span><span class="p">,</span> <span class="s2">&quot;namefrst_unstd_bigrams&quot;</span><span class="p">]</span>
 <span class="n">output_column</span> <span class="o">=</span> <span class="s2">&quot;namelast_frst_bigrams&quot;</span>
```

#### html2text {}

```diff
@@ -29,17 +29,17 @@
 [[feature_selections]]
 input_column = "clean_birthyr"
 output_column = "replaced_birthyr"
 condition = "case when clean_birthyr is null or clean_birthyr == '' then year -
 age else clean_birthyr end"
 transform = "sql_condition"
 ********** aarrrraayy_?¶ **********
-Combine two input columns into an array output column.
+Combine any number of input columns into a single array output column.
     * Attributes:
-          o input_columns - Type: list of strings. Required. The two input
+          o input_columns - Type: list of strings. Required. The list of input
             columns.
           o output_column - Type: string. Required.
 [[feature_selections]]
 input_columns = ["namelast_clean_bigrams", "namefrst_unstd_bigrams"]
 output_column = "namelast_frst_bigrams"
 transform = "array"
 ********** uunniioonn_?¶ **********
```

### Comparing `hlink-3.5.4/docs/genindex.html` & `hlink-3.5.5/docs/genindex.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Index &#8212; hlink 3.5.4 documentation</title>
+    <title>Index &#8212; hlink 3.5.5 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=3d47302e"></script>
+    <script src="_static/documentation_options.js?v=993fb437"></script>
     <script src="_static/doctools.js?v=888ff710"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="#" />
     <link rel="search" title="Search" href="search.html" />
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
```

### Comparing `hlink-3.5.4/docs/index.html` & `hlink-3.5.5/docs/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Welcome to hlink’s documentation! &#8212; hlink 3.5.4 documentation</title>
+    <title>Welcome to hlink’s documentation! &#8212; hlink 3.5.5 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=3d47302e"></script>
+    <script src="_static/documentation_options.js?v=993fb437"></script>
     <script src="_static/doctools.js?v=888ff710"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Introduction" href="introduction.html" />
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
```

### Comparing `hlink-3.5.4/docs/installation.html` & `hlink-3.5.5/docs/installation.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Installation &#8212; hlink 3.5.4 documentation</title>
+    <title>Installation &#8212; hlink 3.5.5 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=3d47302e"></script>
+    <script src="_static/documentation_options.js?v=993fb437"></script>
     <script src="_static/doctools.js?v=888ff710"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Link Tasks" href="link_tasks.html" />
     <link rel="prev" title="Introduction" href="introduction.html" />
```

### Comparing `hlink-3.5.4/docs/introduction.html` & `hlink-3.5.5/docs/introduction.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Introduction &#8212; hlink 3.5.4 documentation</title>
+    <title>Introduction &#8212; hlink 3.5.5 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=3d47302e"></script>
+    <script src="_static/documentation_options.js?v=993fb437"></script>
     <script src="_static/doctools.js?v=888ff710"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Installation" href="installation.html" />
     <link rel="prev" title="Welcome to hlink’s documentation!" href="index.html" />
```

### Comparing `hlink-3.5.4/docs/link_tasks.html` & `hlink-3.5.5/docs/link_tasks.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Link Tasks &#8212; hlink 3.5.4 documentation</title>
+    <title>Link Tasks &#8212; hlink 3.5.5 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=3d47302e"></script>
+    <script src="_static/documentation_options.js?v=993fb437"></script>
     <script src="_static/doctools.js?v=888ff710"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Running hlink" href="running_the_program.html" />
     <link rel="prev" title="Installation" href="installation.html" />
```

### Comparing `hlink-3.5.4/docs/models.html` & `hlink-3.5.5/docs/models.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Models &#8212; hlink 3.5.4 documentation</title>
+    <title>Models &#8212; hlink 3.5.5 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=3d47302e"></script>
+    <script src="_static/documentation_options.js?v=993fb437"></script>
     <script src="_static/doctools.js?v=888ff710"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="prev" title="Substitutions" href="substitutions.html" />
    
   <link rel="stylesheet" href="_static/custom.css" type="text/css" />
```

### Comparing `hlink-3.5.4/docs/objects.inv` & `hlink-3.5.5/docs/objects.inv`

 * *Files 2% similar despite different names*

#### Sphinx inventory

```diff
@@ -1,10 +1,10 @@
 # Sphinx inventory version 2
 # Project: hlink
-# Version: 3.5.4
+# Version: 3.5.5
 # The remainder of this file is compressed using zlib.
 
 column_mappings std:doc -1 column_mappings.html Column Mappings
 comparison_types std:doc -1 comparison_types.html Comparison types, transform add-ons, aggregate features, and household aggregate features
 config std:doc -1 config.html Configuration
 feature_selection_transforms std:doc -1 feature_selection_transforms.html Feature Selection transforms
 genindex std:label -1 genindex.html Index
```

### Comparing `hlink-3.5.4/docs/pipeline_features.html` & `hlink-3.5.5/docs/pipeline_features.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Pipeline generated features &#8212; hlink 3.5.4 documentation</title>
+    <title>Pipeline generated features &#8212; hlink 3.5.5 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=3d47302e"></script>
+    <script src="_static/documentation_options.js?v=993fb437"></script>
     <script src="_static/doctools.js?v=888ff710"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Substitutions" href="substitutions.html" />
     <link rel="prev" title="Feature Selection transforms" href="feature_selection_transforms.html" />
```

### Comparing `hlink-3.5.4/docs/running_the_program.html` & `hlink-3.5.5/docs/running_the_program.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Running hlink &#8212; hlink 3.5.4 documentation</title>
+    <title>Running hlink &#8212; hlink 3.5.5 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=3d47302e"></script>
+    <script src="_static/documentation_options.js?v=993fb437"></script>
     <script src="_static/doctools.js?v=888ff710"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Advanced Workflow Examples" href="use_examples.html" />
     <link rel="prev" title="Link Tasks" href="link_tasks.html" />
```

### Comparing `hlink-3.5.4/docs/search.html` & `hlink-3.5.5/docs/search.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Search &#8212; hlink 3.5.4 documentation</title>
+    <title>Search &#8212; hlink 3.5.5 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
     
-    <script src="_static/documentation_options.js?v=3d47302e"></script>
+    <script src="_static/documentation_options.js?v=993fb437"></script>
     <script src="_static/doctools.js?v=888ff710"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <script src="_static/searchtools.js"></script>
     <script src="_static/language_data.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="#" />
   <script src="searchindex.js" defer></script>
```

### Comparing `hlink-3.5.4/docs/searchindex.js` & `hlink-3.5.5/docs/searchindex.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -16,15 +16,15 @@
         "which": [0, 1, 2, 3, 6, 7, 9, 10, 12],
         "specifi": [0, 1, 2, 6, 7, 9, 10, 11],
         "name": [0, 1, 2, 10, 11],
         "both": [0, 1, 2, 7, 12],
         "option": [0, 1, 2, 3, 6, 7, 8, 10, 12],
         "mai": [0, 2, 6, 7, 10],
         "have": [0, 1, 2, 5, 6, 7, 8, 10, 12],
-        "an": [0, 1, 2, 3, 6, 8, 10],
+        "an": [0, 1, 2, 6, 8, 10],
         "alia": [0, 2, 7],
         "give": [0, 2],
         "new": [0, 2, 12],
         "us": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 11, 12],
         "support": [0, 7, 8],
         "some": [0, 1, 2, 3, 6, 7, 10],
         "make": [0, 1, 2, 5, 12],
@@ -62,15 +62,15 @@
         "overrid": [0, 2],
         "also": [0, 1, 2, 5, 6, 7, 9, 10, 12],
         "provid": [0, 2, 3, 6, 7, 9, 10],
         "override_transform": [0, 2],
         "describ": [0, 2, 10],
         "type": [0, 2, 3, 4, 7, 8, 10, 11, 12],
         "oper": [0, 2],
-        "singl": [0, 2, 10, 12],
+        "singl": [0, 2, 3, 10, 12],
         "output": [0, 1, 2, 3, 6, 7, 10, 12],
         "more": [0, 1, 2, 9, 10, 12],
         "than": [0, 1, 2, 8],
         "one": [0, 1, 2, 7],
         "order": [0, 2, 7],
         "so": [0, 1, 2, 5, 12],
         "anoth": [0, 1, 3, 7],
@@ -239,15 +239,15 @@
         "we": [0, 1, 10, 12],
         "simpli": [0, 2],
         "drop": [0, 2, 10],
         "100": [0, 2, 12],
         "round": [0, 2],
         "lowest": 0,
         "whole": [0, 6],
-        "number": [0, 1, 2, 7, 8, 10],
+        "number": [0, 1, 2, 3, 7, 8, 10],
         "floor": 0,
         "function": [0, 1, 2, 6, 10],
         "bpl": [0, 1, 2],
         "bpl_root": 0,
         "condit": [0, 1, 2, 3, 4, 7],
         "logic": 0,
         "work": [0, 1, 2, 5, 7, 10, 12],
@@ -333,15 +333,15 @@
         "related_individual_max_jw": 1,
         "namefrst_rel": 1,
         "assert": [1, 10],
         "NOT": 1,
         "distinct": 1,
         "f1": 1,
         "evalu": [1, 2, 6, 7, 8],
-        "ani": [1, 2, 5, 8],
+        "ani": [1, 2, 3, 5, 8],
         "potenti": [1, 4, 7],
         "mismatch": 1,
         "queri": [1, 2],
         "fi": 1,
         "OR": 1,
         "mi0": 1,
         "mi1": 1,
```

### Comparing `hlink-3.5.4/docs/substitutions.html` & `hlink-3.5.5/docs/substitutions.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Substitutions &#8212; hlink 3.5.4 documentation</title>
+    <title>Substitutions &#8212; hlink 3.5.5 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=3d47302e"></script>
+    <script src="_static/documentation_options.js?v=993fb437"></script>
     <script src="_static/doctools.js?v=888ff710"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Models" href="models.html" />
     <link rel="prev" title="Pipeline generated features" href="pipeline_features.html" />
```

### Comparing `hlink-3.5.4/docs/use_examples.html` & `hlink-3.5.5/docs/use_examples.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Advanced Workflow Examples &#8212; hlink 3.5.4 documentation</title>
+    <title>Advanced Workflow Examples &#8212; hlink 3.5.5 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=d1102ebc" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css?v=12dfc556" />
-    <script src="_static/documentation_options.js?v=3d47302e"></script>
+    <script src="_static/documentation_options.js?v=993fb437"></script>
     <script src="_static/doctools.js?v=888ff710"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Configuration" href="config.html" />
     <link rel="prev" title="Running hlink" href="running_the_program.html" />
```

### Comparing `hlink-3.5.4/examples/tutorial/README.md` & `hlink-3.5.5/examples/tutorial/README.md`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/examples/tutorial/tutorial.py` & `hlink-3.5.5/examples/tutorial/tutorial.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/examples/tutorial/tutorial_config.toml` & `hlink-3.5.5/examples/tutorial/tutorial_config.toml`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/configs/load_config.py` & `hlink-3.5.5/hlink/configs/load_config.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/README.md` & `hlink-3.5.5/hlink/linking/README.md`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/core/classifier.py` & `hlink-3.5.5/hlink/linking/core/classifier.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/core/column_mapping.py` & `hlink-3.5.5/hlink/linking/core/column_mapping.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/core/comparison.py` & `hlink-3.5.5/hlink/linking/core/comparison.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/core/comparison_feature.py` & `hlink-3.5.5/hlink/linking/core/comparison_feature.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/core/dist_table.py` & `hlink-3.5.5/hlink/linking/core/dist_table.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/core/pipeline.py` & `hlink-3.5.5/hlink/linking/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/core/substitutions.py` & `hlink-3.5.5/hlink/linking/core/substitutions.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/core/threshold.py` & `hlink-3.5.5/hlink/linking/core/threshold.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/core/transforms.py` & `hlink-3.5.5/hlink/linking/core/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # This file is part of the ISRDI's hlink.
 # For copyright and licensing information, see the NOTICE and LICENSE files
 # in this project's top-level directory, and also on-line at:
 #   https://github.com/ipums/hlink
 
+from typing import Any
+
 from pyspark.sql.functions import (
     array,
     collect_list,
     concat,
     count,
     expr,
     floor,
@@ -20,34 +22,41 @@
     struct,
     trim,
     udf,
     when,
 )
 from pyspark.sql.types import ArrayType, LongType, StringType
 from pyspark.ml import Pipeline
-from pyspark.sql import Window
+from pyspark.sql import DataFrame, SparkSession, Window
 from pyspark.ml.feature import NGram, RegexTokenizer, CountVectorizer, MinHashLSH
 
 
 def generate_transforms(
-    spark, df_selected, feature_selections, link_task, is_a, id_col
-):
+    spark: SparkSession,
+    df_selected: DataFrame,
+    feature_selections: list[dict[str, Any]],
+    link_task,
+    is_a: bool,
+    id_col: str,
+) -> DataFrame:
     not_skipped_feature_selections = [
         c
         for c in feature_selections
         if ("skip" not in c or not (c["skip"]))
         and ("post_agg_feature" not in c or not (c["post_agg_feature"]))
     ]
     post_agg_feature_selections = [
         c
         for c in feature_selections
         if ("post_agg_feature" in c) and c["post_agg_feature"]
     ]
 
-    def parse_feature_selections(df_selected, feature_selection, is_a):
+    def parse_feature_selections(
+        df_selected: DataFrame, feature_selection: dict[str, Any], is_a: bool
+    ) -> DataFrame:
         transform = feature_selection["transform"]
 
         if not feature_selection.get("output_column", False):
             feature_selection["output_column"] = feature_selection["output_col"]
 
         if "checkpoint" in feature_selection and feature_selection["checkpoint"]:
             df_selected = df_selected.checkpoint()
@@ -110,17 +119,17 @@
         elif transform == "sql_condition":
             cond = feature_selection["condition"]
             output_col = feature_selection["output_column"]
             df_selected = df_selected.withColumn(output_col, expr(cond))
             return df_selected
 
         elif transform == "array":
-            col1, col2 = feature_selection["input_columns"]
+            input_cols = feature_selection["input_columns"]
             output_col = feature_selection["output_column"]
-            df_selected = df_selected.withColumn(output_col, array(col1, col2))
+            df_selected = df_selected.withColumn(output_col, array(input_cols))
             return df_selected
 
         elif transform == "union":
             col1, col2 = feature_selection["input_columns"]
             output_col = feature_selection["output_column"]
 
             def union_list(list_a, list_b):
@@ -296,15 +305,15 @@
 
         else:
             raise ValueError(f"Invalid transform type for {transform}")
 
     for feature_selection in not_skipped_feature_selections:
         df_selected = parse_feature_selections(df_selected, feature_selection, is_a)
 
-    def get_transforms(name, is_a):
+    def get_transforms(name: str, is_a: bool) -> list[dict[str, Any]]:
         to_process = []
         for f in not_skipped_feature_selections:
             if ("override_column_a" in f) and is_a:
                 pass
             elif ("override_column_b" in f) and not is_a:
                 pass
             elif ("set_value_column_a" in f) and is_a:
```

### Comparing `hlink-3.5.4/hlink/linking/hh_matching/hh_matching.py` & `hlink-3.5.5/hlink/linking/hh_matching/hh_matching.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/hh_matching/link_step_block_on_households.py` & `hlink-3.5.5/hlink/linking/hh_matching/link_step_block_on_households.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/hh_matching/link_step_filter.py` & `hlink-3.5.5/hlink/linking/hh_matching/link_step_filter.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/hh_matching/templates/hh_potential_matches.sql` & `hlink-3.5.5/hlink/linking/hh_matching/templates/hh_potential_matches.sql`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/hh_model_exploration/hh_model_exploration.py` & `hlink-3.5.5/hlink/linking/hh_model_exploration/hh_model_exploration.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/hh_training/hh_training.py` & `hlink-3.5.5/hlink/linking/hh_training/hh_training.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/link_run.py` & `hlink-3.5.5/hlink/linking/link_run.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/link_step.py` & `hlink-3.5.5/hlink/linking/link_step.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/link_task.py` & `hlink-3.5.5/hlink/linking/link_task.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/matching/_helpers.py` & `hlink-3.5.5/hlink/linking/matching/_helpers.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/matching/link_step_explode.py` & `hlink-3.5.5/hlink/linking/matching/link_step_explode.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/matching/link_step_match.py` & `hlink-3.5.5/hlink/linking/matching/link_step_match.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/matching/link_step_score.py` & `hlink-3.5.5/hlink/linking/matching/link_step_score.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/matching/matching.py` & `hlink-3.5.5/hlink/linking/matching/matching.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/matching/templates/potential_matches.sql` & `hlink-3.5.5/hlink/linking/matching/templates/potential_matches.sql`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/model_exploration/link_step_create_features.py` & `hlink-3.5.5/hlink/linking/model_exploration/link_step_create_features.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/model_exploration/link_step_ingest_file.py` & `hlink-3.5.5/hlink/linking/model_exploration/link_step_ingest_file.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/model_exploration/link_step_train_test_models.py` & `hlink-3.5.5/hlink/linking/model_exploration/link_step_train_test_models.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/model_exploration/model_exploration.py` & `hlink-3.5.5/hlink/linking/model_exploration/model_exploration.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/preprocessing/link_step_prep_dataframes.py` & `hlink-3.5.5/hlink/linking/preprocessing/link_step_prep_dataframes.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/preprocessing/link_step_register_raw_dfs.py` & `hlink-3.5.5/hlink/linking/preprocessing/link_step_register_raw_dfs.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/preprocessing/templates/attach_related_col.sql` & `hlink-3.5.5/hlink/linking/preprocessing/templates/attach_related_col.sql`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/preprocessing/templates/attach_related_cols_as_rows.sql` & `hlink-3.5.5/hlink/linking/preprocessing/templates/attach_related_cols_as_rows.sql`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/preprocessing/templates/hh_nbor_rank.sql` & `hlink-3.5.5/hlink/linking/preprocessing/templates/hh_nbor_rank.sql`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/reporting/link_step_export_crosswalk.py` & `hlink-3.5.5/hlink/linking/reporting/link_step_export_crosswalk.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/reporting/link_step_report_r2_percent_linked.py` & `hlink-3.5.5/hlink/linking/reporting/link_step_report_r2_percent_linked.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/reporting/link_step_report_representivity.py` & `hlink-3.5.5/hlink/linking/reporting/link_step_report_representivity.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/reporting/reporting.py` & `hlink-3.5.5/hlink/linking/reporting/reporting.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/table.py` & `hlink-3.5.5/hlink/linking/table.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/table_definitions.csv` & `hlink-3.5.5/hlink/linking/table_definitions.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/templates/shared/aggregate_features.sql` & `hlink-3.5.5/hlink/linking/templates/shared/aggregate_features.sql`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/templates/shared/all_household_members.sql` & `hlink-3.5.5/hlink/linking/templates/shared/all_household_members.sql`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/templates/shared/drop_links.sql` & `hlink-3.5.5/hlink/linking/templates/shared/drop_links.sql`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/templates/shared/hh_aggregate_features.sql` & `hlink-3.5.5/hlink/linking/templates/shared/hh_aggregate_features.sql`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/templates/shared/includes/all_household_members_selects_a.sql` & `hlink-3.5.5/hlink/linking/templates/shared/includes/all_household_members_selects_a.sql`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/templates/shared/includes/all_household_members_selects_b.sql` & `hlink-3.5.5/hlink/linking/templates/shared/includes/all_household_members_selects_b.sql`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/templates/shared/potential_matches_base_features.sql` & `hlink-3.5.5/hlink/linking/templates/shared/potential_matches_base_features.sql`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/templates/shared/tfam_tables.sql` & `hlink-3.5.5/hlink/linking/templates/shared/tfam_tables.sql`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/templates/shared/training_features.sql` & `hlink-3.5.5/hlink/linking/templates/shared/training_features.sql`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/training/link_step_create_comparison_features.py` & `hlink-3.5.5/hlink/linking/training/link_step_create_comparison_features.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/training/link_step_ingest_file.py` & `hlink-3.5.5/hlink/linking/training/link_step_ingest_file.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/training/link_step_save_model_metadata.py` & `hlink-3.5.5/hlink/linking/training/link_step_save_model_metadata.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/training/link_step_train_and_save_model.py` & `hlink-3.5.5/hlink/linking/training/link_step_train_and_save_model.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/training/training.py` & `hlink-3.5.5/hlink/linking/training/training.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/transformers/float_cast_transformer.py` & `hlink-3.5.5/hlink/linking/transformers/float_cast_transformer.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/transformers/interaction_transformer.py` & `hlink-3.5.5/hlink/linking/transformers/interaction_transformer.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/transformers/rename_prob_column.py` & `hlink-3.5.5/hlink/linking/transformers/rename_prob_column.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/linking/util.py` & `hlink-3.5.5/hlink/linking/util.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/scripts/lib/conf_validations.py` & `hlink-3.5.5/hlink/scripts/lib/conf_validations.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/scripts/lib/experimental/reporting.py` & `hlink-3.5.5/hlink/scripts/lib/experimental/reporting.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/scripts/lib/experimental/tfam.py` & `hlink-3.5.5/hlink/scripts/lib/experimental/tfam.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/scripts/lib/io.py` & `hlink-3.5.5/hlink/scripts/lib/io.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/scripts/lib/linking_ops.py` & `hlink-3.5.5/hlink/scripts/lib/linking_ops.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/scripts/lib/table_ops.py` & `hlink-3.5.5/hlink/scripts/lib/table_ops.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/scripts/lib/util.py` & `hlink-3.5.5/hlink/scripts/lib/util.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/scripts/main.py` & `hlink-3.5.5/hlink/scripts/main.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/scripts/main_loop.py` & `hlink-3.5.5/hlink/scripts/main_loop.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/spark/factory.py` & `hlink-3.5.5/hlink/spark/factory.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/spark/jars/hlink_lib-assembly-1.0.jar` & `hlink-3.5.5/hlink/spark/jars/hlink_lib-assembly-1.0.jar`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/spark/session.py` & `hlink-3.5.5/hlink/spark/session.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/conf/duplicate_comp_features.toml` & `hlink-3.5.5/hlink/tests/conf/duplicate_comp_features.toml`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/conf/duplicate_feature_sel.toml` & `hlink-3.5.5/hlink/tests/conf/duplicate_feature_sel.toml`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/conf/integration.toml` & `hlink-3.5.5/hlink/tests/conf/integration.toml`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/conf_validations_test.py` & `hlink-3.5.5/hlink/tests/conf_validations_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/config_loader_test.py` & `hlink-3.5.5/hlink/tests/config_loader_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/conftest.py` & `hlink-3.5.5/hlink/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/core/column_mapping_test.py` & `hlink-3.5.5/hlink/tests/core/column_mapping_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/core/comparison_feature_test.py` & `hlink-3.5.5/hlink/tests/core/comparison_feature_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/core/pipeline_test.py` & `hlink-3.5.5/hlink/tests/core/pipeline_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/hh_matching_test.py` & `hlink-3.5.5/hlink/tests/hh_matching_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/hh_model_exploration_test.py` & `hlink-3.5.5/hlink/tests/hh_model_exploration_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/19thc_nativity_test_hhs.csv` & `hlink-3.5.5/hlink/tests/input_data/19thc_nativity_test_hhs.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/19thc_nativity_test_hhs_a.csv` & `hlink-3.5.5/hlink/tests/input_data/19thc_nativity_test_hhs_a.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/19thc_nativity_test_hhs_b.csv` & `hlink-3.5.5/hlink/tests/input_data/19thc_nativity_test_hhs_b.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/calc_mfbpl_a.csv` & `hlink-3.5.5/hlink/tests/input_data/calc_mfbpl_a.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/calc_mfbpl_b.csv` & `hlink-3.5.5/hlink/tests/input_data/calc_mfbpl_b.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/crosswalk/raw_df_a.csv` & `hlink-3.5.5/hlink/tests/input_data/crosswalk/raw_df_a.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/crosswalk/raw_df_b.csv` & `hlink-3.5.5/hlink/tests/input_data/crosswalk/raw_df_b.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/ha_source.csv` & `hlink-3.5.5/hlink/tests/input_data/ha_source.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/handle_null.csv` & `hlink-3.5.5/hlink/tests/input_data/handle_null.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/hb_source.csv` & `hlink-3.5.5/hlink/tests/input_data/hb_source.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/hh_matching_a.csv` & `hlink-3.5.5/hlink/tests/input_data/hh_matching_a.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/hh_matching_b.csv` & `hlink-3.5.5/hlink/tests/input_data/hh_matching_b.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/hhpm_agg_test.csv` & `hlink-3.5.5/hlink/tests/input_data/hhpm_agg_test.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/households_b.parquet` & `hlink-3.5.5/hlink/tests/input_data/households_b.parquet`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/matched_men.csv` & `hlink-3.5.5/hlink/tests/input_data/matched_men.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/matching_test_a.csv` & `hlink-3.5.5/hlink/tests/input_data/matching_test_a.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/matching_test_b.csv` & `hlink-3.5.5/hlink/tests/input_data/matching_test_b.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/new_hh_test_td.csv` & `hlink-3.5.5/hlink/tests/input_data/new_hh_test_td.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/potential_matches.csv` & `hlink-3.5.5/hlink/tests/input_data/potential_matches.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/potential_matches_agg.csv` & `hlink-3.5.5/hlink/tests/input_data/potential_matches_agg.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/prepped_df_reporting.csv` & `hlink-3.5.5/hlink/tests/input_data/prepped_df_reporting.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/raw_df_reporting.csv` & `hlink-3.5.5/hlink/tests/input_data/raw_df_reporting.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/region.csv` & `hlink-3.5.5/hlink/tests/input_data/region.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/rel_rows_test_a.csv` & `hlink-3.5.5/hlink/tests/input_data/rel_rows_test_a.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/rel_rows_test_b.csv` & `hlink-3.5.5/hlink/tests/input_data/rel_rows_test_b.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/representivity.csv` & `hlink-3.5.5/hlink/tests/input_data/representivity.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/statedist.csv` & `hlink-3.5.5/hlink/tests/input_data/statedist.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/street_abbrevs.csv` & `hlink-3.5.5/hlink/tests/input_data/street_abbrevs.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/street_abbrevs_most_common.csv` & `hlink-3.5.5/hlink/tests/input_data/street_abbrevs_most_common.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/test_parquet_data_a.parquet/part-00000-8465f06e-9bb0-4817-81eb-813ccf07429a-c000.snappy.parquet` & `hlink-3.5.5/hlink/tests/input_data/test_parquet_data_a.parquet/part-00000-8465f06e-9bb0-4817-81eb-813ccf07429a-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/test_parquet_data_b.parquet/part-00000-bb515275-04b4-4a16-80f1-5cc21450b93f-c000.snappy.parquet` & `hlink-3.5.5/hlink/tests/input_data/test_parquet_data_b.parquet/part-00000-bb515275-04b4-4a16-80f1-5cc21450b93f-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/training_data_households.csv` & `hlink-3.5.5/hlink/tests/input_data/training_data_households.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/training_data_households.parquet` & `hlink-3.5.5/hlink/tests/input_data/training_data_households.parquet`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/training_data_long.csv` & `hlink-3.5.5/hlink/tests/input_data/training_data_long.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/training_data_long_a.csv` & `hlink-3.5.5/hlink/tests/input_data/training_data_long_a.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/input_data/training_data_long_b.csv` & `hlink-3.5.5/hlink/tests/input_data/training_data_long_b.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/integration_score_with_trained_models_test.py` & `hlink-3.5.5/hlink/tests/integration_score_with_trained_models_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/integration_test.py` & `hlink-3.5.5/hlink/tests/integration_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/logging_test.py` & `hlink-3.5.5/hlink/tests/logging_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/main_loop_test.py` & `hlink-3.5.5/hlink/tests/main_loop_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/main_test.py` & `hlink-3.5.5/hlink/tests/main_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/matching_blocking_explode_test.py` & `hlink-3.5.5/hlink/tests/matching_blocking_explode_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/matching_comparison_features_test.py` & `hlink-3.5.5/hlink/tests/matching_comparison_features_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/matching_geo_distance_test.py` & `hlink-3.5.5/hlink/tests/matching_geo_distance_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/matching_potential_matches_test.py` & `hlink-3.5.5/hlink/tests/matching_potential_matches_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/matching_potential_matches_universe_test.py` & `hlink-3.5.5/hlink/tests/matching_potential_matches_universe_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/matching_scoring_test.py` & `hlink-3.5.5/hlink/tests/matching_scoring_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/matching_test.py` & `hlink-3.5.5/hlink/tests/matching_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/model_exploration_test.py` & `hlink-3.5.5/hlink/tests/model_exploration_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/plugins/datasources.py` & `hlink-3.5.5/hlink/tests/plugins/datasources.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/plugins/external_data_paths.py` & `hlink-3.5.5/hlink/tests/plugins/external_data_paths.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/preprocessing_test.py` & `hlink-3.5.5/hlink/tests/preprocessing_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/reporting_test.py` & `hlink-3.5.5/hlink/tests/reporting_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/scala_udf_test.py` & `hlink-3.5.5/hlink/tests/scala_udf_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/table_test.py` & `hlink-3.5.5/hlink/tests/table_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/training_test.py` & `hlink-3.5.5/hlink/tests/training_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink/tests/validation_data/training_p_all.parquet/part-00000-6c9e5760-174a-4652-b687-6823087ed5bf-c000.snappy.parquet` & `hlink-3.5.5/hlink/tests/validation_data/training_p_all.parquet/part-00000-6c9e5760-174a-4652-b687-6823087ed5bf-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/hlink.egg-info/PKG-INFO` & `hlink-3.5.5/hlink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hlink
-Version: 3.5.4
+Version: 3.5.5
 Summary: Fast supervised pyspark record linkage software
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
```

### Comparing `hlink-3.5.4/hlink.egg-info/SOURCES.txt` & `hlink-3.5.5/hlink.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -233,14 +233,15 @@
 hlink/tests/conf/test1.toml
 hlink/tests/conf/test_conf_flag_run.json
 hlink/tests/conf/test_run.json
 hlink/tests/core/__init__.py
 hlink/tests/core/column_mapping_test.py
 hlink/tests/core/comparison_feature_test.py
 hlink/tests/core/pipeline_test.py
+hlink/tests/core/transforms_test.py
 hlink/tests/input_data/19thc_nativity_test_hhs.csv
 hlink/tests/input_data/19thc_nativity_test_hhs_a.csv
 hlink/tests/input_data/19thc_nativity_test_hhs_b.csv
 hlink/tests/input_data/birthyr_replace.csv
 hlink/tests/input_data/calc_mfbpl_a.csv
 hlink/tests/input_data/calc_mfbpl_b.csv
 hlink/tests/input_data/county_distances.csv
```

### Comparing `hlink-3.5.4/pyproject.toml` & `hlink-3.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hlink"
-version = "3.5.4"
+version = "3.5.5"
 description = "Fast supervised pyspark record linkage software"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE.txt"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
```

### Comparing `hlink-3.5.4/scala_jar/build.sbt` & `hlink-3.5.5/scala_jar/build.sbt`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/ArrayToString.scala` & `hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/ArrayToString.scala`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/AttachHHColumn.scala` & `hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/AttachHHColumn.scala`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/AttachRelatedRows.scala` & `hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/AttachRelatedRows.scala`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/ExtraChildren.scala` & `hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/ExtraChildren.scala`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/ExtractNeighbors.scala` & `hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/ExtractNeighbors.scala`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/HHCompare.scala` & `hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/HHCompare.scala`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/HHDrop.scala` & `hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/HHDrop.scala`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/HHGetFirstValue.scala` & `hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/HHGetFirstValue.scala`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/HasMatchingElement.scala` & `hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/HasMatchingElement.scala`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/JWRate.scala` & `hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/JWRate.scala`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/JWRelatedRows.scala` & `hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/JWRelatedRows.scala`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/MaxJWCompare.scala` & `hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/MaxJWCompare.scala`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/ParseProbabilityVector.scala` & `hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/ParseProbabilityVector.scala`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/SerJaroWinklerSimilarity.scala` & `hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/SerJaroWinklerSimilarity.scala`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/scala_jar/src/main/scala/com/isrdi/udfs/VectorToString.scala` & `hlink-3.5.5/scala_jar/src/main/scala/com/isrdi/udfs/VectorToString.scala`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/sphinx-docs/Makefile` & `hlink-3.5.5/sphinx-docs/Makefile`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/sphinx-docs/column_mappings.md` & `hlink-3.5.5/sphinx-docs/column_mappings.md`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/sphinx-docs/comparison_types.md` & `hlink-3.5.5/sphinx-docs/comparison_types.md`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/sphinx-docs/conf.py` & `hlink-3.5.5/sphinx-docs/conf.py`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/sphinx-docs/config.md` & `hlink-3.5.5/sphinx-docs/config.md`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/sphinx-docs/feature_selection_transforms.md` & `hlink-3.5.5/sphinx-docs/feature_selection_transforms.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,18 +42,18 @@
 output_column = "replaced_birthyr"
 condition = "case when clean_birthyr is null or clean_birthyr == '' then year - age else clean_birthyr end"
 transform = "sql_condition"
 ```
 
 ## array
 
-Combine two input columns into an array output column.
+Combine any number of input columns into a single array output column.
 
 * Attributes:
-  * `input_columns` - Type: list of strings. Required. The two input columns.
+  * `input_columns` - Type: list of strings. Required. The list of input columns.
   * `output_column` - Type: `string`. Required.
 
 ```
 [[feature_selections]]
 input_columns = ["namelast_clean_bigrams", "namefrst_unstd_bigrams"]
 output_column = "namelast_frst_bigrams"
 transform = "array"
```

### Comparing `hlink-3.5.4/sphinx-docs/index.rst` & `hlink-3.5.5/sphinx-docs/index.rst`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/sphinx-docs/installation.md` & `hlink-3.5.5/sphinx-docs/installation.md`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/sphinx-docs/introduction.md` & `hlink-3.5.5/sphinx-docs/introduction.md`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/sphinx-docs/link_tasks.md` & `hlink-3.5.5/sphinx-docs/link_tasks.md`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/sphinx-docs/make.bat` & `hlink-3.5.5/sphinx-docs/make.bat`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/sphinx-docs/models.md` & `hlink-3.5.5/sphinx-docs/models.md`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/sphinx-docs/pipeline_features.md` & `hlink-3.5.5/sphinx-docs/pipeline_features.md`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/sphinx-docs/running_the_program.md` & `hlink-3.5.5/sphinx-docs/running_the_program.md`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/sphinx-docs/substitutions.md` & `hlink-3.5.5/sphinx-docs/substitutions.md`

 * *Files identical despite different names*

### Comparing `hlink-3.5.4/sphinx-docs/use_examples.md` & `hlink-3.5.5/sphinx-docs/use_examples.md`

 * *Files identical despite different names*

