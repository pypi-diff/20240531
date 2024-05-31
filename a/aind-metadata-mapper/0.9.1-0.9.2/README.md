# Comparing `tmp/aind_metadata_mapper-0.9.1.tar.gz` & `tmp/aind_metadata_mapper-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_metadata_mapper-0.9.1.tar", last modified: Thu May 23 19:12:36 2024, max compression
+gzip compressed data, was "aind_metadata_mapper-0.9.2.tar", last modified: Fri May 31 17:45:29 2024, max compression
```

## Comparing `aind_metadata_mapper-0.9.1.tar` & `aind_metadata_mapper-0.9.2.tar`

### file list

```diff
@@ -1,145 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.260825 aind_metadata_mapper-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.236826 aind_metadata_mapper-0.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.240826 aind_metadata_mapper-0.9.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.240826 aind_metadata_mapper-0.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-23 19:12:36.256826 aind_metadata_mapper-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-05-23 19:12:27.000000 aind_metadata_mapper-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.240826 aind_metadata_mapper-0.9.1/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.240826 aind_metadata_mapper-0.9.1/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.240826 aind_metadata_mapper-0.9.1/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/doc_template/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.240826 aind_metadata_mapper-0.9.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/examples/bergamo_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.240826 aind_metadata_mapper-0.9.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/scripts/singularity_build.def
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 19:12:36.260825 aind_metadata_mapper-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.236826 aind_metadata_mapper-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.244825 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-23 19:12:27.000000 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.244825 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/bergamo/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/bergamo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23425 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/bergamo/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.244825 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/dynamic_routing/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/dynamic_routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/dynamic_routing/mvr_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/dynamic_routing/neuropixels_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/dynamic_routing/sync_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/dynamic_routing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.244825 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/exaspim/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/exaspim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.244825 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/fip/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/fip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/fip/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    12051 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/gather_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.244825 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/mesoscope/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/mesoscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/mesoscope/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.244825 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/open_ephys/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/open_ephys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/open_ephys/rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/open_ephys/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.244825 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/smartspim/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/smartspim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8649 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/smartspim/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/smartspim/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.256826 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-23 19:12:36.000000 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-23 19:12:36.000000 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 19:12:36.000000 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-23 19:12:36.000000 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 19:12:36.000000 aind_metadata_mapper-0.9.1/src/aind_metadata_mapper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.248825 aind_metadata_mapper-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.236826 aind_metadata_mapper-0.9.1/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.248825 aind_metadata_mapper-0.9.1/tests/resources/bergamo/
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/bergamo/cropped_neuron50_00001.tif
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/bergamo/example_description0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    76696 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/bergamo/example_metadata.txt.gz
--rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/bergamo/expected_session.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.248825 aind_metadata_mapper-0.9.1/tests/resources/dynamic_routing/
--rw-r--r--   0 runner    (1001) docker     (127)    39424 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/dynamic_routing/base-missing-probe_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    40853 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/dynamic_routing/base_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/dynamic_routing/mvr.ini
--rw-r--r--   0 runner    (1001) docker     (127)    42611 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/dynamic_routing/mvr_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/dynamic_routing/sync.yml
--rw-r--r--   0 runner    (1001) docker     (127)    46653 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/dynamic_routing/sync_rig.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.248825 aind_metadata_mapper-0.9.1/tests/resources/fip/
--rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/fip/000000_ophys_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/fip/000000_ophys_session.json
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/fip/example_from_teensy.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.248825 aind_metadata_mapper-0.9.1/tests/resources/gather_metadata_job/
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/gather_metadata_job/example_funding_multiple_response.json
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/gather_metadata_job/example_funding_response.json
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/gather_metadata_job/example_procedures_response.json
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/gather_metadata_job/example_subject_response.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.248825 aind_metadata_mapper-0.9.1/tests/resources/gather_metadata_job/metadata_files/
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/gather_metadata_job/metadata_files/data_description.json
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/gather_metadata_job/metadata_files/procedures.json
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/gather_metadata_job/metadata_files/processing.json
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/gather_metadata_job/metadata_files/subject.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.252825 aind_metadata_mapper-0.9.1/tests/resources/mesoscope/
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/mesoscope/0123456789_Face_20240212T091444.json
--rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/mesoscope/example_extract.json
--rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/mesoscope/example_platform.json
--rw-r--r--   0 runner    (1001) docker     (127)    12605 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/mesoscope/expected_session.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.252825 aind_metadata_mapper-0.9.1/tests/resources/open_ephys/
--rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/open_ephys/ephys_session.json
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/open_ephys/newscale_main.csv
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/open_ephys/newscale_surface_finding.csv
--rw-r--r--   0 runner    (1001) docker     (127)    42283 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/open_ephys/open-ephys-inferred_rig.json
--rw-r--r--   0 runner    (1001) docker     (127)    42266 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/open_ephys/open-ephys_rig.json
--rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/open_ephys/settings.mislabeled-probes-0.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/open_ephys/settings.mislabeled-probes-1.xml
--rw-r--r--   0 runner    (1001) docker     (127)   132751 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/open_ephys/settings.xml
--rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/open_ephys/settings_main.xml
--rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/open_ephys/settings_surface_finding.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.252825 aind_metadata_mapper-0.9.1/tests/resources/smartspim/
--rw-r--r--   0 runner    (1001) docker     (127)    17048 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/smartspim/example_ASI_logging_afternoon.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17048 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/smartspim/example_ASI_logging_morning.txt
--rw-r--r--   0 runner    (1001) docker     (127)    38440 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/smartspim/example_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/resources/smartspim/local_json.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.252825 aind_metadata_mapper-0.9.1/tests/test_bergamo/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/test_bergamo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/test_bergamo/test_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.256826 aind_metadata_mapper-0.9.1/tests/test_dynamic_routing/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/test_dynamic_routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/test_dynamic_routing/test_mvr_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/test_dynamic_routing/test_neuropixels_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/test_dynamic_routing/test_sync_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/test_dynamic_routing/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.256826 aind_metadata_mapper-0.9.1/tests/test_fip/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/test_fip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/test_fip/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    18232 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/test_gather_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/test_legacy_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.256826 aind_metadata_mapper-0.9.1/tests/test_mesoscope/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/test_mesoscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7761 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/test_mesoscope/test_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.256826 aind_metadata_mapper-0.9.1/tests/test_open_ephys/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/test_open_ephys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/test_open_ephys/test_rig.py
--rw-r--r--   0 runner    (1001) docker     (127)     9935 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/test_open_ephys/test_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:12:36.256826 aind_metadata_mapper-0.9.1/tests/test_smartspim/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/test_smartspim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/test_smartspim/test_acquisition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-23 19:12:26.000000 aind_metadata_mapper-0.9.1/tests/test_smartspim/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.200739 aind_metadata_mapper-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.172739 aind_metadata_mapper-0.9.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.176739 aind_metadata_mapper-0.9.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.176739 aind_metadata_mapper-0.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-31 17:45:29.200739 aind_metadata_mapper-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.176739 aind_metadata_mapper-0.9.2/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.180739 aind_metadata_mapper-0.9.2/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.180739 aind_metadata_mapper-0.9.2/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/doc_template/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.180739 aind_metadata_mapper-0.9.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/examples/bergamo_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.180739 aind_metadata_mapper-0.9.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/scripts/singularity_build.def
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 17:45:29.200739 aind_metadata_mapper-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.172739 aind_metadata_mapper-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.180739 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.180739 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/bergamo/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/bergamo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23425 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/bergamo/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.180739 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/dynamic_routing/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/dynamic_routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/dynamic_routing/mvr_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/dynamic_routing/neuropixels_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/dynamic_routing/sync_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/dynamic_routing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.184738 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/exaspim/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/exaspim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.184738 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/fip/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/fip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/fip/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18873 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/gather_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.184738 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/mesoscope/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/mesoscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/mesoscope/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.184738 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/open_ephys/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/open_ephys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/open_ephys/rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/open_ephys/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.184738 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/smartspim/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/smartspim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8649 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/smartspim/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/smartspim/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.196739 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-31 17:45:29.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-05-31 17:45:29.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 17:45:29.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-31 17:45:29.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-31 17:45:29.000000 aind_metadata_mapper-0.9.2/src/aind_metadata_mapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.184738 aind_metadata_mapper-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.176739 aind_metadata_mapper-0.9.2/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.184738 aind_metadata_mapper-0.9.2/tests/resources/bergamo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/bergamo/cropped_neuron50_00001.tif
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/bergamo/example_description0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    76696 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/bergamo/example_metadata.txt.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/bergamo/expected_session.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.188738 aind_metadata_mapper-0.9.2/tests/resources/dynamic_routing/
+-rw-r--r--   0 runner    (1001) docker     (127)    39424 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/dynamic_routing/base-missing-probe_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    40853 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/dynamic_routing/base_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/dynamic_routing/mvr.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    42611 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/dynamic_routing/mvr_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/dynamic_routing/sync.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    46653 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/dynamic_routing/sync_rig.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.188738 aind_metadata_mapper-0.9.2/tests/resources/fip/
+-rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/fip/000000_ophys_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/fip/000000_ophys_session.json
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/fip/example_from_teensy.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.188738 aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/example_funding_multiple_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/example_funding_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/example_procedures_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/example_subject_response.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.188738 aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/metadata_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/metadata_files/acquisition.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/metadata_files/data_description.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/metadata_files/instrument.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/metadata_files/procedures.json
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/metadata_files/processing.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20774 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/metadata_files/rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13803 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/metadata_files/session.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/metadata_files/subject.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.192739 aind_metadata_mapper-0.9.2/tests/resources/mesoscope/
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/mesoscope/0123456789_Face_20240212T091444.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/mesoscope/example_extract.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/mesoscope/example_platform.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12605 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/mesoscope/expected_session.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.192739 aind_metadata_mapper-0.9.2/tests/resources/open_ephys/
+-rw-r--r--   0 runner    (1001) docker     (127)    11653 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/open_ephys/ephys_session.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/open_ephys/newscale_main.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/open_ephys/newscale_surface_finding.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    42283 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/open_ephys/open-ephys-inferred_rig.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42266 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/open_ephys/open-ephys_rig.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/open_ephys/settings.mislabeled-probes-0.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)   136805 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/open_ephys/settings.mislabeled-probes-1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   132751 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/open_ephys/settings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/open_ephys/settings_main.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    53714 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/open_ephys/settings_surface_finding.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.192739 aind_metadata_mapper-0.9.2/tests/resources/smartspim/
+-rw-r--r--   0 runner    (1001) docker     (127)    17048 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/smartspim/example_ASI_logging_afternoon.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17048 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/smartspim/example_ASI_logging_morning.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38440 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/smartspim/example_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/resources/smartspim/local_json.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.196739 aind_metadata_mapper-0.9.2/tests/test_bergamo/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_bergamo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_bergamo/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.196739 aind_metadata_mapper-0.9.2/tests/test_dynamic_routing/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_dynamic_routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_dynamic_routing/test_mvr_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_dynamic_routing/test_neuropixels_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_dynamic_routing/test_sync_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_dynamic_routing/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.196739 aind_metadata_mapper-0.9.2/tests/test_fip/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_fip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_fip/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28919 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_gather_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_legacy_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.196739 aind_metadata_mapper-0.9.2/tests/test_mesoscope/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_mesoscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7761 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_mesoscope/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.196739 aind_metadata_mapper-0.9.2/tests/test_open_ephys/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_open_ephys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_open_ephys/test_rig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9935 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_open_ephys/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:45:29.196739 aind_metadata_mapper-0.9.2/tests/test_smartspim/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_smartspim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_smartspim/test_acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-31 17:45:19.000000 aind_metadata_mapper-0.9.2/tests/test_smartspim/test_utils.py
```

### Comparing `aind_metadata_mapper-0.9.1/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_metadata_mapper-0.9.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_metadata_mapper-0.9.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/.github/ISSUE_TEMPLATE/user-story.md` & `aind_metadata_mapper-0.9.2/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/.github/workflows/tag_and_publish.yml` & `aind_metadata_mapper-0.9.2/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/.github/workflows/test_and_lint.yml` & `aind_metadata_mapper-0.9.2/.github/workflows/test_and_lint.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/.gitignore` & `aind_metadata_mapper-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/CONTRIBUTING.md` & `aind_metadata_mapper-0.9.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/LICENSE` & `aind_metadata_mapper-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/PKG-INFO` & `aind_metadata_mapper-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-metadata-mapper
-Version: 0.9.1
+Version: 0.9.2
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_metadata_mapper-0.9.1/README.md` & `aind_metadata_mapper-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/doc_template/Makefile` & `aind_metadata_mapper-0.9.2/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/doc_template/make.bat` & `aind_metadata_mapper-0.9.2/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/doc_template/source/_static/dark-logo.svg` & `aind_metadata_mapper-0.9.2/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/doc_template/source/_static/favicon.ico` & `aind_metadata_mapper-0.9.2/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/doc_template/source/_static/light-logo.svg` & `aind_metadata_mapper-0.9.2/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/doc_template/source/conf.py` & `aind_metadata_mapper-0.9.2/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/examples/bergamo_session.py` & `aind_metadata_mapper-0.9.2/examples/bergamo_session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/pyproject.toml` & `aind_metadata_mapper-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/bergamo/session.py` & `aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/bergamo/session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/core.py` & `aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/core.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/dynamic_routing/mvr_rig.py` & `aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/dynamic_routing/mvr_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/dynamic_routing/neuropixels_rig.py` & `aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/dynamic_routing/neuropixels_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/dynamic_routing/sync_rig.py` & `aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/dynamic_routing/sync_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/dynamic_routing/utils.py` & `aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/dynamic_routing/utils.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/fip/session.py` & `aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/fip/session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/mesoscope/session.py` & `aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/mesoscope/session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/open_ephys/rig.py` & `aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/open_ephys/rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/open_ephys/session.py` & `aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/open_ephys/session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/smartspim/acquisition.py` & `aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/smartspim/acquisition.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/src/aind_metadata_mapper/smartspim/utils.py` & `aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/smartspim/utils.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/src/aind_metadata_mapper.egg-info/PKG-INFO` & `aind_metadata_mapper-0.9.2/src/aind_metadata_mapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-metadata-mapper
-Version: 0.9.1
+Version: 0.9.2
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_metadata_mapper-0.9.1/src/aind_metadata_mapper.egg-info/SOURCES.txt` & `aind_metadata_mapper-0.9.2/src/aind_metadata_mapper.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -61,17 +61,21 @@
 tests/resources/fip/000000_ophys_rig.json
 tests/resources/fip/000000_ophys_session.json
 tests/resources/fip/example_from_teensy.txt
 tests/resources/gather_metadata_job/example_funding_multiple_response.json
 tests/resources/gather_metadata_job/example_funding_response.json
 tests/resources/gather_metadata_job/example_procedures_response.json
 tests/resources/gather_metadata_job/example_subject_response.json
+tests/resources/gather_metadata_job/metadata_files/acquisition.json
 tests/resources/gather_metadata_job/metadata_files/data_description.json
+tests/resources/gather_metadata_job/metadata_files/instrument.json
 tests/resources/gather_metadata_job/metadata_files/procedures.json
 tests/resources/gather_metadata_job/metadata_files/processing.json
+tests/resources/gather_metadata_job/metadata_files/rig.json
+tests/resources/gather_metadata_job/metadata_files/session.json
 tests/resources/gather_metadata_job/metadata_files/subject.json
 tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json
 tests/resources/mesoscope/0123456789_Eye_20240212T091443.json
 tests/resources/mesoscope/0123456789_Face_20240212T091444.json
 tests/resources/mesoscope/example_extract.json
 tests/resources/mesoscope/example_platform.json
 tests/resources/mesoscope/expected_session.json
```

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/bergamo/cropped_neuron50_00001.tif` & `aind_metadata_mapper-0.9.2/tests/resources/bergamo/cropped_neuron50_00001.tif`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/bergamo/example_description0.txt` & `aind_metadata_mapper-0.9.2/tests/resources/bergamo/example_description0.txt`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/bergamo/example_metadata.txt.gz` & `aind_metadata_mapper-0.9.2/tests/resources/bergamo/example_metadata.txt.gz`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/bergamo/expected_session.json` & `aind_metadata_mapper-0.9.2/tests/resources/bergamo/expected_session.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/dynamic_routing/base-missing-probe_rig.json` & `aind_metadata_mapper-0.9.2/tests/resources/dynamic_routing/base-missing-probe_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/dynamic_routing/base_rig.json` & `aind_metadata_mapper-0.9.2/tests/resources/dynamic_routing/base_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/dynamic_routing/mvr.ini` & `aind_metadata_mapper-0.9.2/tests/resources/dynamic_routing/mvr.ini`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/dynamic_routing/mvr_rig.json` & `aind_metadata_mapper-0.9.2/tests/resources/dynamic_routing/mvr_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/dynamic_routing/sync.yml` & `aind_metadata_mapper-0.9.2/tests/resources/dynamic_routing/sync.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/dynamic_routing/sync_rig.json` & `aind_metadata_mapper-0.9.2/tests/resources/dynamic_routing/sync_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/fip/000000_ophys_rig.json` & `aind_metadata_mapper-0.9.2/tests/resources/fip/000000_ophys_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/fip/000000_ophys_session.json` & `aind_metadata_mapper-0.9.2/tests/resources/fip/000000_ophys_session.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/gather_metadata_job/example_funding_multiple_response.json` & `aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/example_funding_multiple_response.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/gather_metadata_job/example_procedures_response.json` & `aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/example_procedures_response.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/gather_metadata_job/example_subject_response.json` & `aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/example_subject_response.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/gather_metadata_job/metadata_files/data_description.json` & `aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/metadata_files/data_description.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/gather_metadata_job/metadata_files/procedures.json` & `aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/metadata_files/procedures.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/gather_metadata_job/metadata_files/processing.json` & `aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/metadata_files/processing.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/gather_metadata_job/metadata_files/subject.json` & `aind_metadata_mapper-0.9.2/tests/resources/gather_metadata_job/metadata_files/subject.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json` & `aind_metadata_mapper-0.9.2/tests/resources/mesoscope/0123456789_Behavior_20240212T091443.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json` & `aind_metadata_mapper-0.9.2/tests/resources/mesoscope/0123456789_Eye_20240212T091443.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/mesoscope/0123456789_Face_20240212T091444.json` & `aind_metadata_mapper-0.9.2/tests/resources/mesoscope/0123456789_Face_20240212T091444.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/mesoscope/example_extract.json` & `aind_metadata_mapper-0.9.2/tests/resources/mesoscope/example_extract.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/mesoscope/example_platform.json` & `aind_metadata_mapper-0.9.2/tests/resources/mesoscope/example_platform.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/mesoscope/expected_session.json` & `aind_metadata_mapper-0.9.2/tests/resources/mesoscope/expected_session.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/open_ephys/ephys_session.json` & `aind_metadata_mapper-0.9.2/tests/resources/open_ephys/ephys_session.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/open_ephys/newscale_main.csv` & `aind_metadata_mapper-0.9.2/tests/resources/open_ephys/newscale_main.csv`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/open_ephys/newscale_surface_finding.csv` & `aind_metadata_mapper-0.9.2/tests/resources/open_ephys/newscale_surface_finding.csv`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/open_ephys/open-ephys-inferred_rig.json` & `aind_metadata_mapper-0.9.2/tests/resources/open_ephys/open-ephys-inferred_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/open_ephys/open-ephys_rig.json` & `aind_metadata_mapper-0.9.2/tests/resources/open_ephys/open-ephys_rig.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/open_ephys/settings.mislabeled-probes-0.xml` & `aind_metadata_mapper-0.9.2/tests/resources/open_ephys/settings.mislabeled-probes-0.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/open_ephys/settings.mislabeled-probes-1.xml` & `aind_metadata_mapper-0.9.2/tests/resources/open_ephys/settings.mislabeled-probes-1.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/open_ephys/settings.xml` & `aind_metadata_mapper-0.9.2/tests/resources/open_ephys/settings.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/open_ephys/settings_main.xml` & `aind_metadata_mapper-0.9.2/tests/resources/open_ephys/settings_main.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/open_ephys/settings_surface_finding.xml` & `aind_metadata_mapper-0.9.2/tests/resources/open_ephys/settings_surface_finding.xml`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/smartspim/example_ASI_logging_afternoon.txt` & `aind_metadata_mapper-0.9.2/tests/resources/smartspim/example_ASI_logging_afternoon.txt`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/smartspim/example_ASI_logging_morning.txt` & `aind_metadata_mapper-0.9.2/tests/resources/smartspim/example_ASI_logging_morning.txt`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/resources/smartspim/example_metadata.py` & `aind_metadata_mapper-0.9.2/tests/resources/smartspim/example_metadata.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/test_bergamo/test_session.py` & `aind_metadata_mapper-0.9.2/tests/test_bergamo/test_session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/test_dynamic_routing/test_mvr_rig.py` & `aind_metadata_mapper-0.9.2/tests/test_dynamic_routing/test_mvr_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/test_dynamic_routing/test_neuropixels_rig.py` & `aind_metadata_mapper-0.9.2/tests/test_dynamic_routing/test_neuropixels_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/test_dynamic_routing/test_sync_rig.py` & `aind_metadata_mapper-0.9.2/tests/test_dynamic_routing/test_sync_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/test_dynamic_routing/test_utils.py` & `aind_metadata_mapper-0.9.2/tests/test_dynamic_routing/test_utils.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/test_fip/test_session.py` & `aind_metadata_mapper-0.9.2/tests/test_fip/test_session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/test_gather_metadata.py` & `aind_metadata_mapper-0.9.2/src/aind_metadata_mapper/gather_metadata.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,455 +1,529 @@
-"""Tests gather_metadata module"""
+"""Module to gather metadata from different sources."""
 
+import argparse
 import json
-import os
-import unittest
-from datetime import datetime, timezone
+import sys
 from pathlib import Path
-from unittest.mock import MagicMock, mock_open, patch
+from typing import List, Optional, Type
 
-from aind_data_schema.core.processing import DataProcess, PipelineProcess
+import requests
+from aind_data_schema.base import AindCoreModel
+from aind_data_schema.core.acquisition import Acquisition
+from aind_data_schema.core.data_description import (
+    DataDescription,
+    RawDataDescription,
+)
+from aind_data_schema.core.instrument import Instrument
+from aind_data_schema.core.metadata import Metadata
+from aind_data_schema.core.procedures import Procedures
+from aind_data_schema.core.processing import PipelineProcess, Processing
+from aind_data_schema.core.rig import Rig
+from aind_data_schema.core.session import Session
+from aind_data_schema.core.subject import Subject
 from aind_data_schema_models.modalities import Modality
-from aind_data_schema_models.process_names import ProcessName
-from requests import Response
+from aind_data_schema_models.organizations import Organization
+from aind_data_schema_models.pid_names import PIDName
+from pydantic import Field, ValidationError
+from pydantic_settings import BaseSettings
 
-from aind_metadata_mapper.gather_metadata import (
-    GatherMetadataJob,
-    JobSettings,
-    MetadataSettings,
-    ProceduresSettings,
-    ProcessingSettings,
-    RawDataDescriptionSettings,
-    SubjectSettings,
-)
 
-RESOURCES_DIR = (
-    Path(os.path.dirname(os.path.realpath(__file__)))
-    / "resources"
-    / "gather_metadata_job"
-)
-METADATA_DIR = RESOURCES_DIR / "metadata_files"
+class SubjectSettings(BaseSettings):
+    """Fields needed to retrieve subject metadata"""
 
+    subject_id: str
+    metadata_service_path: str = "subject"
 
-class TestGatherMetadataJob(unittest.TestCase):
-    """Tests methods in GatherMetadataJob class"""
 
-    @classmethod
-    def setUpClass(cls):
-        """Load json files."""
-        with open(RESOURCES_DIR / "example_subject_response.json", "r") as f:
-            example_subject_response = json.load(f)
-        with open(
-            RESOURCES_DIR / "example_procedures_response.json", "r"
-        ) as f:
-            example_procedures_response = json.load(f)
-        with open(RESOURCES_DIR / "example_funding_response.json", "r") as f:
-            example_funding_response = json.load(f)
-        with open(
-            RESOURCES_DIR / "example_funding_multiple_response.json", "r"
-        ) as f:
-            example_funding_multi_response = json.load(f)
-        cls.example_subject_response = example_subject_response
-        cls.example_procedures_response = example_procedures_response
-        cls.example_funding_response = example_funding_response
-        cls.example_funding_multi_response = example_funding_multi_response
-
-    def test_class_constructor(self):
-        """Tests class is constructed properly"""
-        job_settings = JobSettings(directory_to_write_to=RESOURCES_DIR)
-        metadata_job = GatherMetadataJob(settings=job_settings)
-        self.assertIsNotNone(metadata_job)
-
-    @patch("requests.get")
-    def test_get_subject(self, mock_get: MagicMock):
-        """Tests get_subject method"""
-        mock_response = Response()
-        mock_response.status_code = 200
-        body = json.dumps(self.example_subject_response)
-        mock_response._content = body.encode("utf-8")
-        mock_get.return_value = mock_response
-
-        job_settings = JobSettings(
-            metadata_service_domain="http://acme.test",
-            directory_to_write_to=RESOURCES_DIR,
-            subject_settings=SubjectSettings(
-                subject_id="632269",
-            ),
-        )
-        metadata_job = GatherMetadataJob(settings=job_settings)
-        contents = metadata_job.get_subject()
-        self.assertEqual("632269", contents["subject_id"])
-        mock_get.assert_called_once_with("http://acme.test/subject/632269")
-
-    @patch("requests.get")
-    def test_get_subject_error(self, mock_get: MagicMock):
-        """Tests get_subject when an error is raised"""
-        mock_response = Response()
-        mock_response.status_code = 500
-        body = json.dumps({"message": "Internal Server Error"})
-        mock_response._content = body.encode("utf-8")
-        mock_get.return_value = mock_response
-
-        job_settings = JobSettings(
-            directory_to_write_to=RESOURCES_DIR,
-            metadata_service_domain="http://acme.test",
-            subject_settings=SubjectSettings(
-                subject_id="632269",
-            ),
-        )
-        metadata_job = GatherMetadataJob(settings=job_settings)
-        with self.assertRaises(AssertionError) as e:
-            metadata_job.get_subject()
-        expected_error_message = (
-            "Subject metadata is not valid! "
-            "{'message': 'Internal Server Error'}"
-        )
-        self.assertTrue(expected_error_message in str(e.exception))
-
-    @patch("requests.get")
-    def test_get_procedures(self, mock_get: MagicMock):
-        """Tests get_procedures method"""
-        mock_response = Response()
-        mock_response.status_code = 406
-        body = json.dumps(self.example_procedures_response)
-        mock_response._content = body.encode("utf-8")
-        mock_get.return_value = mock_response
-
-        job_settings = JobSettings(
-            directory_to_write_to=RESOURCES_DIR,
-            metadata_service_domain="http://acme.test",
-            procedures_settings=ProceduresSettings(
-                subject_id="632269",
-            ),
-        )
-        metadata_job = GatherMetadataJob(settings=job_settings)
-        contents = metadata_job.get_procedures()
-        self.assertEqual("632269", contents["subject_id"])
-        mock_get.assert_called_once_with("http://acme.test/procedures/632269")
-
-    @patch("requests.get")
-    def test_get_procedures_error(self, mock_get: MagicMock):
-        """Tests get_procedures when an error is raised"""
-        mock_response = Response()
-        mock_response.status_code = 500
-        body = json.dumps({"message": "Internal Server Error"})
-        mock_response._content = body.encode("utf-8")
-        mock_get.return_value = mock_response
-
-        job_settings = JobSettings(
-            directory_to_write_to=RESOURCES_DIR,
-            metadata_service_domain="http://acme.test",
-            procedures_settings=ProceduresSettings(
-                subject_id="632269",
-            ),
-        )
-        metadata_job = GatherMetadataJob(settings=job_settings)
-        with self.assertRaises(AssertionError) as e:
-            metadata_job.get_procedures()
-        expected_error_message = (
-            "Procedures metadata is not valid! "
-            "{'message': 'Internal Server Error'}"
-        )
-        self.assertTrue(expected_error_message in str(e.exception))
-
-    @patch("requests.get")
-    def test_get_raw_data_description(self, mock_get: MagicMock):
-        """Tests get_raw_data_description method with valid model"""
-
-        mock_response = Response()
-        mock_response.status_code = 200
-        body = json.dumps(self.example_funding_response)
-        mock_response._content = body.encode("utf-8")
-        mock_get.return_value = mock_response
-
-        job_settings = JobSettings(
-            directory_to_write_to=RESOURCES_DIR,
-            metadata_service_domain="http://acme.test",
-            raw_data_description_settings=RawDataDescriptionSettings(
-                project_name="Ephys Platform",
-                name="ecephys_632269_2023-10-10_10-10-10",
-                modality=[Modality.ECEPHYS, Modality.BEHAVIOR_VIDEOS],
-            ),
-        )
-        metadata_job = GatherMetadataJob(settings=job_settings)
-        contents = metadata_job.get_raw_data_description()
-        expected_investigators = ["Anna Apple", "John Smith"]
-        actual_investigators = [i["name"] for i in contents["investigators"]]
-        self.assertEqual(expected_investigators, actual_investigators)
-        self.assertEqual("ecephys", contents["platform"]["abbreviation"])
-        self.assertEqual("632269", contents["subject_id"])
-        self.assertEqual(
-            "ecephys_632269_2023-10-10_10-10-10", contents["name"]
-        )
-        mock_get.assert_called_once_with(
-            "http://acme.test/funding/Ephys Platform"
-        )
-
-    @patch("requests.get")
-    def test_get_raw_data_description_multi_response(
-        self, mock_get: MagicMock
-    ):
-        """Tests get_raw_data_description method with valid model and multiple
-        items in funding response"""
-
-        mock_response = Response()
-        mock_response.status_code = 300
-        body = json.dumps(self.example_funding_multi_response)
-        mock_response._content = body.encode("utf-8")
-        mock_get.return_value = mock_response
-
-        job_settings = JobSettings(
-            directory_to_write_to=RESOURCES_DIR,
-            metadata_service_domain="http://acme.test",
-            raw_data_description_settings=RawDataDescriptionSettings(
-                project_name="Ephys Platform",
-                name="ecephys_632269_2023-10-10_10-10-10",
-                modality=[Modality.ECEPHYS, Modality.BEHAVIOR_VIDEOS],
-            ),
-        )
-        metadata_job = GatherMetadataJob(settings=job_settings)
-        contents = metadata_job.get_raw_data_description()
-        expected_investigators = ["Anna Apple", "Don Key", "John Smith"]
-        actual_investigators = [i["name"] for i in contents["investigators"]]
-        self.assertEqual(2, len(contents["funding_source"]))
-        self.assertEqual(expected_investigators, actual_investigators)
-        self.assertEqual("ecephys", contents["platform"]["abbreviation"])
-        self.assertEqual("632269", contents["subject_id"])
-        self.assertEqual(
-            "ecephys_632269_2023-10-10_10-10-10", contents["name"]
-        )
-        mock_get.assert_called_once_with(
-            "http://acme.test/funding/Ephys Platform"
-        )
-
-    @patch("requests.get")
-    def test_get_raw_data_description_invalid(self, mock_get: MagicMock):
-        """Tests get_raw_data_description method with invalid model"""
-        mock_response = Response()
-        mock_response.status_code = 500
-        body = json.dumps({"message": "Internal Server Error"})
-        mock_response._content = body.encode("utf-8")
-        mock_get.return_value = mock_response
-
-        job_settings = JobSettings(
-            directory_to_write_to=RESOURCES_DIR,
-            metadata_service_domain="http://acme.test",
-            raw_data_description_settings=RawDataDescriptionSettings(
-                project_name="foo",
-                name="ecephys_632269_2023-10-10_10-10-10",
-                modality=[Modality.ECEPHYS, Modality.BEHAVIOR_VIDEOS],
-            ),
-        )
-        metadata_job = GatherMetadataJob(settings=job_settings)
-        # with self.assertWarns(UserWarning) as w:
-        contents = metadata_job.get_raw_data_description()
-        self.assertEqual("ecephys", contents["platform"]["abbreviation"])
-        self.assertEqual("632269", contents["subject_id"])
-        self.assertEqual(
-            "ecephys_632269_2023-10-10_10-10-10", contents["name"]
-        )
-        self.assertEqual([], contents["investigators"])
-
-    def test_get_processing_metadata(self):
-        """Tests get_processing_metadata method"""
-        data_process = DataProcess(
-            name=ProcessName.COMPRESSION,
-            software_version="0.0.15",
-            start_date_time=datetime(
-                2020, 10, 10, 10, 10, 10, tzinfo=timezone.utc
-            ),
-            end_date_time=datetime(
-                2020, 10, 10, 11, 10, 10, tzinfo=timezone.utc
-            ),
-            input_location="/source/open_ephys",
-            output_location="/tmp/stage",
-            code_url=(
-                "https://github.com/AllenNeuralDynamics/"
-                "aind-data-transformation"
-            ),
-            parameters={},
-            outputs={},
-        )
-        processing_pipeline = PipelineProcess(
-            data_processes=[data_process], processor_full_name="Anna Apple"
-        )
-
-        job_settings = JobSettings(
-            directory_to_write_to=RESOURCES_DIR,
-            processing_settings=ProcessingSettings(
-                pipeline_process=processing_pipeline
-            ),
-        )
-        metadata_job = GatherMetadataJob(settings=job_settings)
-        contents = metadata_job.get_processing_metadata()
-        self.assertEqual(
-            "Compression",
-            contents["processing_pipeline"]["data_processes"][0]["name"],
-        )
-
-    def test_get_main_metadata_with_warnings(self):
-        """Tests get_main_metadata method raises validation warnings"""
-        job_settings = JobSettings(
-            directory_to_write_to=RESOURCES_DIR,
-            metadata_settings=MetadataSettings(
-                name="ecephys_632269_2023-10-10_10-10-10",
-                location="s3://some-bucket/ecephys_632269_2023-10-10_10-10-10",
-                subject_filepath=(METADATA_DIR / "subject.json"),
-                data_description_filepath=(
-                    METADATA_DIR / "data_description.json"
-                ),
-                procedures_filepath=(METADATA_DIR / "procedures.json"),
-                session_filepath=None,
-                rig_filepath=None,
-                processing_filepath=(METADATA_DIR / "processing.json"),
-                acquisition_filepath=None,
-                instrument_filepath=None,
-            ),
-        )
-        metadata_job = GatherMetadataJob(settings=job_settings)
-        with self.assertWarns(UserWarning) as w:
-            main_metadata = metadata_job.get_main_metadata()
-        # Issues with incomplete Procedures model raises warnings
-        expected_warnings = (
-            "Pydantic serializer warnings:\n"
-            "  Expected `date` but got `str`"
-            " - serialized value may not be as expected\n"
-            "  Expected `Union[CallithrixJacchus, HomoSapiens, MacacaMulatta, "
-            "MusMusculus, RattusNorvegicus]` but got `dict`"
-            " - serialized value may not be as expected\n"
-            "  Expected `BreedingInfo` but got `dict`"
-            " - serialized value may not be as expected\n"
-            "  Expected `Union[AllenInstitute, ColumbiaUniversity,"
-            " HuazhongUniversityOfScienceAndTechnology, JacksonLaboratory,"
-            " NewYorkUniversity, Other]` but got `dict`"
-            " - serialized value may not be as expected"
-        )
-
-        self.assertEqual(expected_warnings, str(w.warning))
-        self.assertEqual(
-            "s3://some-bucket/ecephys_632269_2023-10-10_10-10-10",
-            main_metadata.location,
-        )
-        self.assertEqual("Invalid", main_metadata.metadata_status.value)
-        self.assertEqual("632269", main_metadata.subject.subject_id)
-
-    @patch("builtins.open", new_callable=mock_open())
-    @patch("json.dump")
-    def test_write_json_file(
-        self, mock_json_dump: MagicMock, mock_file: MagicMock
-    ):
-        """Tests write_json_file method"""
-        mock_file.return_value.__enter__.return_value = (
-            RESOURCES_DIR / "subject.json"
-        )
-
-        job_settings = JobSettings(directory_to_write_to=RESOURCES_DIR)
-        metadata_job = GatherMetadataJob(settings=job_settings)
-        metadata_job._write_json_file(
-            filename="subject.json", contents={"subject_id": "123456"}
-        )
+class ProceduresSettings(BaseSettings):
+    """Fields needed to retrieve procedures metadata"""
 
-        mock_json_dump.assert_called_once_with(
-            {"subject_id": "123456"}, RESOURCES_DIR / "subject.json", indent=3
-        )
+    subject_id: str
+    metadata_service_path: str = "procedures"
 
-    @patch(
-        "aind_metadata_mapper.gather_metadata.GatherMetadataJob.get_subject"
-    )
-    @patch(
-        "aind_metadata_mapper.gather_metadata.GatherMetadataJob.get_procedures"
-    )
-    @patch(
-        "aind_metadata_mapper.gather_metadata.GatherMetadataJob"
-        ".get_raw_data_description"
-    )
-    @patch(
-        "aind_metadata_mapper.gather_metadata.GatherMetadataJob"
-        ".get_processing_metadata"
-    )
-    @patch(
-        "aind_metadata_mapper.gather_metadata.GatherMetadataJob"
-        ".get_main_metadata"
+
+class RawDataDescriptionSettings(BaseSettings):
+    """Fields needed to retrieve data description metadata"""
+
+    name: str
+    project_name: str
+    modality: List[Modality.ONE_OF]
+    institution: Optional[Organization.ONE_OF] = Organization.AIND
+    metadata_service_path: str = "funding"
+
+
+class ProcessingSettings(BaseSettings):
+    """Fields needed to retrieve processing metadata"""
+
+    pipeline_process: PipelineProcess
+
+
+class MetadataSettings(BaseSettings):
+    """Fields needed to retrieve main Metadata"""
+
+    name: str
+    location: str
+    subject_filepath: Optional[Path] = None
+    data_description_filepath: Optional[Path] = None
+    procedures_filepath: Optional[Path] = None
+    session_filepath: Optional[Path] = None
+    rig_filepath: Optional[Path] = None
+    processing_filepath: Optional[Path] = None
+    acquisition_filepath: Optional[Path] = None
+    instrument_filepath: Optional[Path] = None
+
+
+class JobSettings(BaseSettings):
+    """Fields needed to gather all metadata"""
+
+    metadata_service_domain: Optional[str] = None
+    subject_settings: Optional[SubjectSettings] = None
+    raw_data_description_settings: Optional[RawDataDescriptionSettings] = None
+    procedures_settings: Optional[ProceduresSettings] = None
+    processing_settings: Optional[ProcessingSettings] = None
+    metadata_settings: Optional[MetadataSettings] = None
+    directory_to_write_to: Path
+    metadata_dir: Optional[Path] = Field(
+        default=None,
+        description="Optional path where user defined metadata files might be",
     )
-    @patch(
-        "aind_metadata_mapper.gather_metadata.GatherMetadataJob"
-        "._write_json_file"
+    metadata_dir_force: bool = Field(
+        default=False,
+        description=(
+            "Whether to override the user defined files in metadata_dir with "
+            "those pulled from metadata service"
+        ),
     )
-    def test_run_job(
-        self,
-        mock_write_json_file: MagicMock,
-        mock_get_main_metadata: MagicMock,
-        mock_get_processing_metadata: MagicMock,
-        mock_get_raw_data_description: MagicMock,
-        mock_get_procedures: MagicMock,
-        mock_get_subject: MagicMock,
-    ):
-        """Tests run_job calls all the sub processes"""
-        data_process = DataProcess(
-            name=ProcessName.COMPRESSION,
-            software_version="0.0.15",
-            start_date_time=datetime(
-                2020, 10, 10, 10, 10, 10, tzinfo=timezone.utc
-            ),
-            end_date_time=datetime(
-                2020, 10, 10, 11, 10, 10, tzinfo=timezone.utc
-            ),
-            input_location="/source/open_ephys",
-            output_location="/tmp/stage",
-            code_url=(
-                "https://github.com/AllenNeuralDynamics/"
-                "aind-data-transformation"
-            ),
-            parameters={},
-            outputs={},
-        )
-        processing_pipeline = PipelineProcess(
-            data_processes=[data_process], processor_full_name="Anna Apple"
-        )
-
-        job_settings = JobSettings(
-            directory_to_write_to=RESOURCES_DIR,
-            metadata_service_domain="http://acme.test",
-            subject_settings=SubjectSettings(
-                subject_id="632269",
-            ),
-            procedures_settings=ProceduresSettings(
-                subject_id="632269",
-            ),
-            raw_data_description_settings=RawDataDescriptionSettings(
-                project_name="Ephys Platform",
-                name="ecephys_632269_2023-10-10_10-10-10",
-                modality=[Modality.ECEPHYS, Modality.BEHAVIOR_VIDEOS],
-            ),
-            processing_settings=ProcessingSettings(
-                pipeline_process=processing_pipeline
-            ),
-            metadata_settings=MetadataSettings(
-                name="ecephys_632269_2023-10-10_10-10-10",
-                location="s3://some-bucket/ecephys_632269_2023-10-10_10-10-10",
-                subject_filepath=(METADATA_DIR / "subject.json"),
-                data_description_filepath=(
-                    METADATA_DIR / "data_description.json"
-                ),
-                procedures_filepath=(METADATA_DIR / "procedures.json"),
-                session_filepath=None,
-                rig_filepath=None,
-                processing_filepath=(METADATA_DIR / "processing.json"),
-                acquisition_filepath=None,
-                instrument_filepath=None,
-            ),
-        )
-
-        metadata_job = GatherMetadataJob(settings=job_settings)
-
-        metadata_job.run_job()
-
-        mock_get_subject.assert_called_once()
-        mock_get_procedures.assert_called_once()
-        mock_get_raw_data_description.assert_called_once()
-        mock_get_processing_metadata.assert_called_once()
-        mock_get_main_metadata.assert_called_once()
-        mock_write_json_file.assert_called()
+
+
+class GatherMetadataJob:
+    """Class to handle retrieving metadata"""
+
+    def __init__(self, settings: JobSettings):
+        """
+        Class constructor
+        Parameters
+        ----------
+        settings : JobSettings
+        """
+        self.settings = settings
+
+    def _does_file_exist_in_user_defined_dir(self, file_name: str) -> bool:
+        """
+        Check whether a file exists in a directory.
+        Parameters
+        ----------
+        file_name : str
+          Something like subject.json
+
+        Returns
+        -------
+        True if self.settings.metadata_dir is not None and file is in that dir
+
+        """
+        if self.settings.metadata_dir is not None:
+            file_path_to_check = self.settings.metadata_dir / file_name
+            if file_path_to_check.is_file():
+                return True
+            else:
+                return False
+        else:
+            return False
+
+    def _get_file_from_user_defined_directory(self, file_name: str) -> dict:
+        """
+        Get a file from a user defined directory
+        Parameters
+        ----------
+        file_name : str
+          Like subject.json
+
+        Returns
+        -------
+        File contents as a dictionary
+
+        """
+        file_path = self.settings.metadata_dir / file_name
+        # TODO: Add error handler in case json.load fails
+        with open(file_path, "r") as f:
+            contents = json.load(f)
+        return contents
+
+    def get_subject(self) -> dict:
+        """Get subject metadata"""
+        file_name = Subject.default_filename()
+        should_use_service: bool = (
+            not self.settings.metadata_dir_force
+            or not self._does_file_exist_in_user_defined_dir(
+                file_name=file_name
+            )
+        )
+        if should_use_service:
+            response = requests.get(
+                self.settings.metadata_service_domain
+                + f"/{self.settings.subject_settings.metadata_service_path}/"
+                + f"{self.settings.subject_settings.subject_id}"
+            )
+
+            if response.status_code < 300 or response.status_code == 406:
+                json_content = response.json()
+                return json_content["data"]
+            else:
+                raise AssertionError(
+                    f"Subject metadata is not valid! {response.json()}"
+                )
+        else:
+            contents = self._get_file_from_user_defined_directory(
+                file_name=file_name
+            )
+            return contents
+
+    def get_procedures(self) -> dict:
+        """Get procedures metadata"""
+        file_name = Procedures.default_filename()
+        should_use_service: bool = (
+            not self.settings.metadata_dir_force
+            or not self._does_file_exist_in_user_defined_dir(
+                file_name=file_name
+            )
+        )
+        if should_use_service:
+            procedures_file_path = (
+                self.settings.procedures_settings.metadata_service_path
+            )
+            response = requests.get(
+                self.settings.metadata_service_domain
+                + f"/{procedures_file_path}/"
+                + f"{self.settings.procedures_settings.subject_id}"
+            )
+
+            if response.status_code < 300 or response.status_code == 406:
+                json_content = response.json()
+                return json_content["data"]
+            else:
+                raise AssertionError(
+                    f"Procedures metadata is not valid! {response.json()}"
+                )
+        else:
+            contents = self._get_file_from_user_defined_directory(
+                file_name=file_name
+            )
+            return contents
+
+    def get_raw_data_description(self) -> dict:
+        """Get raw data description metadata"""
+
+        def get_funding_info(domain: str, url_path: str, project_name: str):
+            """Utility method to retrieve funding info from metadata service"""
+            response = requests.get("/".join([domain, url_path, project_name]))
+            if response.status_code == 200:
+                funding_info = [response.json().get("data")]
+            elif response.status_code == 300:
+                funding_info = response.json().get("data")
+            else:
+                funding_info = []
+            investigators = set()
+            for f in funding_info:
+                project_fundees = f.get("fundee", "").split(",")
+                pid_names = [
+                    PIDName(name=p.strip()).model_dump_json()
+                    for p in project_fundees
+                ]
+                if project_fundees is not [""]:
+                    investigators.update(pid_names)
+            investigators = [
+                PIDName.model_validate_json(i) for i in investigators
+            ]
+            investigators.sort(key=lambda x: x.name)
+            return funding_info, investigators
+
+        # Returns a dict with platform, subject_id, and acq_datetime
+        file_name = RawDataDescription.default_filename()
+        should_use_service: bool = (
+            not self.settings.metadata_dir_force
+            or not self._does_file_exist_in_user_defined_dir(
+                file_name=file_name
+            )
+        )
+        if should_use_service:
+            basic_settings = RawDataDescription.parse_name(
+                name=self.settings.raw_data_description_settings.name
+            )
+            ds_settings = self.settings.raw_data_description_settings
+            funding_source, investigator_list = get_funding_info(
+                self.settings.metadata_service_domain,
+                ds_settings.metadata_service_path,
+                self.settings.raw_data_description_settings.project_name,
+            )
+
+            try:
+                institution = (
+                    self.settings.raw_data_description_settings.institution
+                )
+                modality = self.settings.raw_data_description_settings.modality
+                return json.loads(
+                    RawDataDescription(
+                        name=self.settings.raw_data_description_settings.name,
+                        institution=institution,
+                        modality=modality,
+                        funding_source=funding_source,
+                        investigators=investigator_list,
+                        **basic_settings,
+                    ).model_dump_json()
+                )
+            except ValidationError:
+                institution = (
+                    self.settings.raw_data_description_settings.institution
+                )
+                modality = self.settings.raw_data_description_settings.modality
+                return json.loads(
+                    RawDataDescription.model_construct(
+                        name=self.settings.raw_data_description_settings.name,
+                        institution=institution,
+                        modality=modality,
+                        funding_source=funding_source,
+                        investigators=investigator_list,
+                        **basic_settings,
+                    ).model_dump_json()
+                )
+        else:
+            contents = self._get_file_from_user_defined_directory(
+                file_name=file_name
+            )
+            return contents
+
+    def get_processing_metadata(self):
+        """Get processing metadata"""
+
+        file_name = Processing.default_filename()
+        should_use_service: bool = (
+            not self.settings.metadata_dir_force
+            or not self._does_file_exist_in_user_defined_dir(
+                file_name=file_name
+            )
+        )
+        if should_use_service:
+            processing_instance = Processing(
+                processing_pipeline=(
+                    self.settings.processing_settings.pipeline_process
+                )
+            )
+            return json.loads(processing_instance.model_dump_json())
+        else:
+            contents = self._get_file_from_user_defined_directory(
+                file_name=file_name
+            )
+            return contents
+
+    def get_session_metadata(self) -> Optional[dict]:
+        """Get session metadata"""
+        file_name = Session.default_filename()
+        if self._does_file_exist_in_user_defined_dir(file_name=file_name):
+            contents = self._get_file_from_user_defined_directory(
+                file_name=file_name
+            )
+            return contents
+        else:
+            return None
+
+    def get_rig_metadata(self) -> Optional[dict]:
+        """Get rig metadata"""
+        file_name = Rig.default_filename()
+        if self._does_file_exist_in_user_defined_dir(file_name=file_name):
+            contents = self._get_file_from_user_defined_directory(
+                file_name=file_name
+            )
+            return contents
+        else:
+            return None
+
+    def get_acquisition_metadata(self) -> Optional[dict]:
+        """Get acquisition metadata"""
+        file_name = Acquisition.default_filename()
+        if self._does_file_exist_in_user_defined_dir(file_name=file_name):
+            contents = self._get_file_from_user_defined_directory(
+                file_name=file_name
+            )
+            return contents
+        else:
+            return None
+
+    def get_instrument_metadata(self) -> Optional[dict]:
+        """Get instrument metadata"""
+        file_name = Instrument.default_filename()
+        if self._does_file_exist_in_user_defined_dir(file_name=file_name):
+            contents = self._get_file_from_user_defined_directory(
+                file_name=file_name
+            )
+            return contents
+        else:
+            return None
+
+    def get_main_metadata(self) -> Metadata:
+        """Get main Metadata model"""
+
+        def load_model(
+            filepath: Optional[Path], model: Type[AindCoreModel]
+        ) -> Optional[AindCoreModel]:
+            """
+            Validates contents of file with an AindCoreModel
+            Parameters
+            ----------
+            filepath : Optional[Path]
+            model : Type[AindCoreModel]
+
+            Returns
+            -------
+            Optional[AindCodeModel]
+
+            """
+            if filepath is not None and filepath.is_file():
+                with open(filepath, "r") as f:
+                    contents = json.load(f)
+                try:
+                    output = model.model_validate_json(json.dumps(contents))
+                except ValidationError:
+                    output = model.model_construct(**contents)
+
+                return output
+            else:
+                return None
+
+        subject = load_model(
+            self.settings.metadata_settings.subject_filepath, Subject
+        )
+        data_description = load_model(
+            self.settings.metadata_settings.data_description_filepath,
+            DataDescription,
+        )
+        procedures = load_model(
+            self.settings.metadata_settings.procedures_filepath, Procedures
+        )
+        session = load_model(
+            self.settings.metadata_settings.session_filepath, Session
+        )
+        rig = load_model(self.settings.metadata_settings.rig_filepath, Rig)
+        acquisition = load_model(
+            self.settings.metadata_settings.acquisition_filepath, Acquisition
+        )
+        instrument = load_model(
+            self.settings.metadata_settings.instrument_filepath, Instrument
+        )
+        processing = load_model(
+            self.settings.metadata_settings.processing_filepath, Processing
+        )
+
+        metadata = Metadata(
+            name=self.settings.metadata_settings.name,
+            location=self.settings.metadata_settings.location,
+            subject=subject,
+            data_description=data_description,
+            procedures=procedures,
+            session=session,
+            rig=rig,
+            processing=processing,
+            acquisition=acquisition,
+            instrument=instrument,
+        )
+        return metadata
+
+    def _write_json_file(self, filename: str, contents: dict) -> None:
+        """
+        Write a json file
+        Parameters
+        ----------
+        filename : str
+          Name of the file to write to (e.g., subject.json)
+        contents : dict
+          Contents to write to the json file
+
+        Returns
+        -------
+        None
+
+        """
+        output_path = self.settings.directory_to_write_to / filename
+        with open(output_path, "w") as f:
+            json.dump(contents, f, indent=3)
+
+    def _gather_automated_metadata(self):
+        """Gather metadata that can be retrieved automatically or from a
+        user defined directory"""
+        if self.settings.subject_settings is not None:
+            contents = self.get_subject()
+            self._write_json_file(
+                filename=Subject.default_filename(), contents=contents
+            )
+        if self.settings.procedures_settings is not None:
+            contents = self.get_procedures()
+            self._write_json_file(
+                filename=Procedures.default_filename(), contents=contents
+            )
+        if self.settings.raw_data_description_settings is not None:
+            contents = self.get_raw_data_description()
+            self._write_json_file(
+                filename=DataDescription.default_filename(), contents=contents
+            )
+        if self.settings.processing_settings is not None:
+            contents = self.get_processing_metadata()
+            self._write_json_file(
+                filename=Processing.default_filename(), contents=contents
+            )
+
+    def _gather_non_automated_metadata(self):
+        """Gather metadata that cannot yet be retrieved automatically but
+        may be in a user defined directory."""
+        if self.settings.metadata_settings is None:
+            rig_contents = self.get_rig_metadata()
+            if rig_contents:
+                self._write_json_file(
+                    filename=Rig.default_filename(), contents=rig_contents
+                )
+            session_contents = self.get_session_metadata()
+            if session_contents:
+                self._write_json_file(
+                    filename=Session.default_filename(),
+                    contents=session_contents,
+                )
+            acq_contents = self.get_acquisition_metadata()
+            if acq_contents:
+                self._write_json_file(
+                    filename=Acquisition.default_filename(),
+                    contents=acq_contents,
+                )
+            instrument_contents = self.get_instrument_metadata()
+            if instrument_contents:
+                self._write_json_file(
+                    filename=Instrument.default_filename(),
+                    contents=instrument_contents,
+                )
+
+    def run_job(self) -> None:
+        """Run job"""
+        self._gather_automated_metadata()
+        self._gather_non_automated_metadata()
+        if self.settings.metadata_settings is not None:
+            metadata = self.get_main_metadata()
+            metadata.write_standard_file(
+                output_directory=self.settings.directory_to_write_to
+            )
 
 
 if __name__ == "__main__":
-    unittest.main()
+    sys_args = sys.argv[1:]
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
+        "-j",
+        "--job-settings",
+        required=True,
+        type=str,
+        help=(
+            r"""
+            Instead of init args the job settings can optionally be passed in
+            as a json string in the command line.
+            """
+        ),
+    )
+    cli_args = parser.parse_args(sys_args)
+    main_job_settings = JobSettings.model_validate_json(cli_args.job_settings)
+    job = GatherMetadataJob(settings=main_job_settings)
+    job.run_job()
```

### Comparing `aind_metadata_mapper-0.9.1/tests/test_legacy_core.py` & `aind_metadata_mapper-0.9.2/tests/test_legacy_core.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/test_mesoscope/test_session.py` & `aind_metadata_mapper-0.9.2/tests/test_mesoscope/test_session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/test_open_ephys/test_rig.py` & `aind_metadata_mapper-0.9.2/tests/test_open_ephys/test_rig.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/test_open_ephys/test_session.py` & `aind_metadata_mapper-0.9.2/tests/test_open_ephys/test_session.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/test_smartspim/test_acquisition.py` & `aind_metadata_mapper-0.9.2/tests/test_smartspim/test_acquisition.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_mapper-0.9.1/tests/test_smartspim/test_utils.py` & `aind_metadata_mapper-0.9.2/tests/test_smartspim/test_utils.py`

 * *Files identical despite different names*

