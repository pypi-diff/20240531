# Comparing `tmp/pyAFQ-1.3.1.tar.gz` & `tmp/pyafq-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyAFQ-1.3.1.tar", last modified: Thu Apr  4 23:15:21 2024, max compression
+gzip compressed data, was "pyafq-1.3.2.tar", last modified: Fri May 31 18:45:09 2024, max compression
```

## Comparing `pyAFQ-1.3.1.tar` & `pyafq-1.3.2.tar`

### file list

```diff
@@ -1,503 +1,503 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.344086 pyAFQ-1.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.272085 pyAFQ-1.3.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.github/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)    16080 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.272085 pyAFQ-1.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.github/workflows/docbuild.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.github/workflows/docker_pyafq.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.github/workflows/docker_pyafq_cuda12.yml
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.github/workflows/nightly_anisotropic_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.github/workflows/nightly_basic_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.github/workflows/nightly_custom_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.github/workflows/nightly_pft_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.github/workflows/nightly_reco80_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.github/workflows/nightly_reco_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.github/workflows/nightly_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.mailmap
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.272085 pyAFQ-1.3.1/.maintenance/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1395 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.maintenance/update_changes.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2870 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.maintenance/update_zenodo.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.pep8speaks.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/.zenodo.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.276085 pyAFQ-1.3.1/AFQ/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/_fixes.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/afq_bids_entities.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.276085 pyAFQ-1.3.1/AFQ/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46835 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/api/bundle_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    40386 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/api/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/api/participant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.276085 pyAFQ-1.3.1/AFQ/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    67032 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/data/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.276085 pyAFQ-1.3.1/AFQ/definitions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26362 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/definitions/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    14181 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/definitions/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/definitions/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.280085 pyAFQ-1.3.1/AFQ/models/
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/models/QBallTP.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/models/csd.py
--rw-r--r--   0 runner    (1001) docker     (127)    11296 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/models/dki.py
--rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/models/dti.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/models/fwdti.py
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)    58329 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.280085 pyAFQ-1.3.1/AFQ/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32761 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tasks/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tasks/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8699 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tasks/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    14062 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tasks/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12273 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tasks/tractography.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tasks/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15295 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tasks/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.284085 pyAFQ-1.3.1/AFQ/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.284085 pyAFQ-1.3.1/AFQ/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)    53305 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/MoriGroups_Test.mat
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/WholeBrainFG_test.mat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.256085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.284085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.284085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/.datalad/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/.datalad/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/.datalad/config
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/CHANGES
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/README
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/T1w.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/annex-uuid
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/dataset_description.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.256085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.292086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/aMRIQC.csv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_group.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-01.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-02.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-03.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-04.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-05.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-06.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-07.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-08.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-09.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-10.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-11.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-12.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-13.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-14.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-15.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-16.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-17.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-18.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-19.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-20.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-21.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-22.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-23.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-24.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-25.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-26.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/fMRIQC.csv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_group.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-01.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-02.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-03.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-04.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-05.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-06.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-07.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-08.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-09.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-10.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-11.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-12.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-13.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-14.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-15.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-16.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-17.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-18.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-19.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-20.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-21.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-22.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-23.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-24.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-25.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-26.pdf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/participants.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.256085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.292086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/anat/sub-01_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.296085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/func/sub-01_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/func/sub-01_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/func/sub-01_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/func/sub-01_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.256085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.296085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/anat/sub-02_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.296085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/func/sub-02_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/func/sub-02_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/func/sub-02_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/func/sub-02_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.256085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.296085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/anat/sub-03_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.296085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/func/sub-03_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/func/sub-03_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/func/sub-03_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/func/sub-03_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.256085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.296085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/anat/sub-04_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.296085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/func/sub-04_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/func/sub-04_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/func/sub-04_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/func/sub-04_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.256085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.296085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/anat/sub-05_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.296085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/func/sub-05_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/func/sub-05_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/func/sub-05_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/func/sub-05_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.256085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.296085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/anat/sub-06_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.300086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/func/sub-06_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/func/sub-06_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/func/sub-06_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/func/sub-06_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.256085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.300086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/anat/sub-07_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.300086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/func/sub-07_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/func/sub-07_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/func/sub-07_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/func/sub-07_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.260085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.300086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/anat/sub-08_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.300086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/func/sub-08_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/func/sub-08_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/func/sub-08_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/func/sub-08_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.260085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.300086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/anat/sub-09_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.300086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/func/sub-09_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/func/sub-09_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/func/sub-09_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/func/sub-09_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.260085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.300086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/anat/sub-10_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.300086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/func/sub-10_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/func/sub-10_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/func/sub-10_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/func/sub-10_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.260085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.300086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/anat/sub-11_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.304086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/func/sub-11_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/func/sub-11_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/func/sub-11_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/func/sub-11_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.260085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.304086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/anat/sub-12_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.304086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/func/sub-12_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/func/sub-12_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/func/sub-12_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/func/sub-12_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.260085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.304086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/anat/sub-13_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.304086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/func/sub-13_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/func/sub-13_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/func/sub-13_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/func/sub-13_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.260085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.304086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/anat/sub-14_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.304086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/func/sub-14_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/func/sub-14_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/func/sub-14_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/func/sub-14_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.260085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.304086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/anat/sub-15_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.304086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/func/sub-15_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/func/sub-15_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/func/sub-15_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/func/sub-15_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.260085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.304086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/anat/sub-16_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.308086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/func/sub-16_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/func/sub-16_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/func/sub-16_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/func/sub-16_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.260085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.308086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/anat/sub-17_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.308086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/func/sub-17_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/func/sub-17_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/func/sub-17_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/func/sub-17_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.260085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.308086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/anat/sub-18_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.308086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/func/sub-18_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/func/sub-18_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/func/sub-18_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/func/sub-18_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.264085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.308086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/anat/sub-19_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.308086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/func/sub-19_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/func/sub-19_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/func/sub-19_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/func/sub-19_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.264085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.308086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/anat/sub-20_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.308086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/func/sub-20_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/func/sub-20_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/func/sub-20_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/func/sub-20_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.264085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.308086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/anat/sub-21_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.312086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/func/sub-21_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/func/sub-21_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/func/sub-21_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/func/sub-21_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.264085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.312086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/anat/sub-22_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.312086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/func/sub-22_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/func/sub-22_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/func/sub-22_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/func/sub-22_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.264085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.312086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/anat/sub-23_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.312086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/func/sub-23_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/func/sub-23_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/func/sub-23_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/func/sub-23_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.264085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.312086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/anat/sub-24_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.312086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/func/sub-24_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/func/sub-24_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/func/sub-24_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/func/sub-24_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.264085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.312086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/anat/sub-25_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.312086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/func/sub-25_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/func/sub-25_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/func/sub-25_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/func/sub-25_task-flanker_run-2_events.tsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.264085 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.312086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/anat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/anat/sub-26_T1w.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.316086 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/func/sub-26_task-flanker_run-1_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/func/sub-26_task-flanker_run-1_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/func/sub-26_task-flanker_run-2_bold.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/func/sub-26_task-flanker_run-2_events.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/task-flanker_bold.json
--rw-r--r--   0 runner    (1001) docker     (127)    30829 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/test_bundle_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/test_csd.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/test_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/test_dki.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/test_dti.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/test_fixes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/test_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)    12017 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/test_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/test_tractography.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tests/test_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.316086 pyAFQ-1.3.1/AFQ/tractography/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tractography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tractography/gputractography.py
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tractography/tractography.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/tractography/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.316086 pyAFQ-1.3.1/AFQ/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15159 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/bin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/streamlines.py
--rw-r--r--   0 runner    (1001) docker     (127)    10021 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.316086 pyAFQ-1.3.1/AFQ/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/tests/test_conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/tests/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/tests/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/tests/test_streamlines.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/tests/test_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/utils/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-04 23:15:21.000000 pyAFQ-1.3.1/AFQ/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.320086 pyAFQ-1.3.1/AFQ/viz/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6880 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/viz/altair.py
--rw-r--r--   0 runner    (1001) docker     (127)    18554 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/viz/fury_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    58032 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/viz/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    25572 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/viz/plotly_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    22824 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/AFQ/viz/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    35389 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/CITATION
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-04-04 23:15:21.344086 pyAFQ-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.320086 pyAFQ-1.3.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4994 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/bin/pyAFQ
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.320086 pyAFQ-1.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.320086 pyAFQ-1.3.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/_progressbars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.320086 pyAFQ-1.3.1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)   272903 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/_static/BDE_Banner_revised20160211-01.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)    56025 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/_static/eScience_Logo_HR.png
--rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/_static/escience-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)   112939 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.320086 pyAFQ-1.3.1/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.324086 pyAFQ-1.3.1/docs/source/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.324086 pyAFQ-1.3.1/docs/source/explanations/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    14803 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/explanations/_static/down_left_arrow.png
--rw-r--r--   0 runner    (1001) docker     (127)    14739 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/explanations/_static/down_right_arrow.png
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/explanations/_static/greencheck.png
--rw-r--r--   0 runner    (1001) docker     (127)    99285 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/explanations/_static/tract_modeling2.png
--rw-r--r--   0 runner    (1001) docker     (127)   207285 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/explanations/_static/tract_profiling.png
--rw-r--r--   0 runner    (1001) docker     (127)   220157 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/explanations/_static/tract_recognition.png
--rw-r--r--   0 runner    (1001) docker     (127)   254342 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/explanations/_static/tract_tractography.png
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/explanations/bundle_orientation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/explanations/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/explanations/modeling.rst
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/explanations/profiling.rst
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/explanations/recognition.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/explanations/tractography.rst
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/explanations/tractometry_pipeline.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.328086 pyAFQ-1.3.1/docs/source/howto/
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/cite.rst
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.328086 pyAFQ-1.3.1/docs/source/howto/developing/
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/developing/definitions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/developing/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/developing/releasing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/developing/tasks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/getting_help.rst
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/installation_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.328086 pyAFQ-1.3.1/docs/source/howto/usage/
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/usage/converter.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/usage/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/usage/docker.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/usage/image.rst
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/usage/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/usage/kwargs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/usage/methods.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/howto/usage/scalars.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.328086 pyAFQ-1.3.1/docs/source/reference/
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/reference/bundledict.rst
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/reference/kwargs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/reference/mapping.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8574 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/reference/methods.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/reference/viz_backend.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.332086 pyAFQ-1.3.1/docs/source/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/sphinxext/kwargsdocs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/sphinxext/methodsdocs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/sphinxext/updatedocs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.332086 pyAFQ-1.3.1/docs/source/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/source/tutorials/index.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)      887 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/docs/upload-gh-pages.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.268085 pyAFQ-1.3.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.332086 pyAFQ-1.3.1/examples/howto_examples/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/howto_examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10022 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/howto_examples/add_custom_bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/howto_examples/baby_afq.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/howto_examples/cerebellar_peduncles.py
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/howto_examples/cloudknot_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/howto_examples/cloudknot_hcp_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/howto_examples/plot_acoustic_radiations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/howto_examples/plot_afq_callosal.py
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/howto_examples/plot_afq_fwdti.py
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/howto_examples/plot_optic_radiations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/howto_examples/plot_recobundles.py
--rw-r--r--   0 runner    (1001) docker     (127)    19258 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/howto_examples/plot_stages_of_tractometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/howto_examples/use_subject_space_rois_from_freesurfer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/howto_examples/vof_example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.332086 pyAFQ-1.3.1/examples/tutorial_examples/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/tutorial_examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9029 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/tutorial_examples/plot_001_afq_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/tutorial_examples/plot_002_bids_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    19513 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/examples/tutorial_examples/plot_003_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.336086 pyAFQ-1.3.1/gpu_docker/
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/gpu_docker/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (127)      401 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/gpu_docker/cuda_build.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/gpu_docker/cuda_track_template.def
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/gpu_docker/docker-build.sh
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/gpu_docker/docker-push.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.336086 pyAFQ-1.3.1/pyAFQ.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-04-04 23:15:21.000000 pyAFQ-1.3.1/pyAFQ.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21170 2024-04-04 23:15:21.000000 pyAFQ-1.3.1/pyAFQ.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 23:15:21.000000 pyAFQ-1.3.1/pyAFQ.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 23:15:21.000000 pyAFQ-1.3.1/pyAFQ.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-04 23:15:21.000000 pyAFQ-1.3.1/pyAFQ.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-04 23:15:21.000000 pyAFQ-1.3.1/pyAFQ.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:15:21.336086 pyAFQ-1.3.1/pyafq_docker/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/pyafq_docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/pyafq_docker/docker-build.sh
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/pyafq_docker/docker-push.sh
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-04 23:15:21.344086 pyAFQ-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-04 23:15:16.000000 pyAFQ-1.3.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.897009 pyafq-1.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.825008 pyafq-1.3.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-31 18:45:04.000000 pyafq-1.3.2/.github/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)    16080 2024-05-31 18:45:04.000000 pyafq-1.3.2/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.825008 pyafq-1.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-31 18:45:04.000000 pyafq-1.3.2/.github/workflows/docbuild.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-31 18:45:04.000000 pyafq-1.3.2/.github/workflows/docker_pyafq.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-31 18:45:04.000000 pyafq-1.3.2/.github/workflows/docker_pyafq_cuda12.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-31 18:45:04.000000 pyafq-1.3.2/.github/workflows/nightly_anisotropic_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-31 18:45:04.000000 pyafq-1.3.2/.github/workflows/nightly_basic_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-31 18:45:04.000000 pyafq-1.3.2/.github/workflows/nightly_custom_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-31 18:45:04.000000 pyafq-1.3.2/.github/workflows/nightly_pft_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-31 18:45:04.000000 pyafq-1.3.2/.github/workflows/nightly_reco80_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-31 18:45:04.000000 pyafq-1.3.2/.github/workflows/nightly_reco_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-31 18:45:04.000000 pyafq-1.3.2/.github/workflows/nightly_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-31 18:45:04.000000 pyafq-1.3.2/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-31 18:45:04.000000 pyafq-1.3.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-31 18:45:04.000000 pyafq-1.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-31 18:45:04.000000 pyafq-1.3.2/.mailmap
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.825008 pyafq-1.3.2/.maintenance/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1395 2024-05-31 18:45:04.000000 pyafq-1.3.2/.maintenance/update_changes.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2870 2024-05-31 18:45:04.000000 pyafq-1.3.2/.maintenance/update_zenodo.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-31 18:45:04.000000 pyafq-1.3.2/.pep8speaks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-31 18:45:04.000000 pyafq-1.3.2/.zenodo.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.829008 pyafq-1.3.2/AFQ/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/afq_bids_entities.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.829008 pyafq-1.3.2/AFQ/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46350 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/api/bundle_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49373 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/api/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13651 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/api/participant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.829008 pyafq-1.3.2/AFQ/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67034 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/data/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.829008 pyafq-1.3.2/AFQ/definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26250 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/definitions/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14140 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/definitions/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/definitions/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.833008 pyafq-1.3.2/AFQ/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/models/QBallTP.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/models/csd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11296 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/models/dki.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/models/dti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/models/fwdti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58329 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.833008 pyafq-1.3.2/AFQ/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36037 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tasks/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7625 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tasks/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tasks/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14060 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tasks/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15316 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tasks/tractography.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tasks/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15291 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tasks/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.837009 pyafq-1.3.2/AFQ/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.837009 pyafq-1.3.2/AFQ/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    53305 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/MoriGroups_Test.mat
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/WholeBrainFG_test.mat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.809008 pyafq-1.3.2/AFQ/tests/data/mocks3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.837009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.837009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/.datalad/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/.datalad/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/.datalad/config
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/README
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/T1w.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/annex-uuid
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/dataset_description.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.809008 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.845009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/aMRIQC.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_group.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-01.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-02.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-03.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-04.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-05.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-06.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-07.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-08.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-09.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-10.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-11.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-12.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-13.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-14.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-15.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-16.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-17.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-18.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-19.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-20.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-21.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-22.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-23.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-24.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-25.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/anatomical_sub-26.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/fMRIQC.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_group.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-01.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-02.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-03.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-04.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-05.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-06.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-07.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-08.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-09.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-10.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-11.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-12.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-13.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-14.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-15.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-16.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-17.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-18.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-19.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-20.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-21.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-22.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-23.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-24.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-25.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/derivatives/mriqc/functional_sub-26.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/participants.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.809008 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.845009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/anat/sub-01_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.849009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/func/sub-01_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/func/sub-01_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/func/sub-01_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-01/func/sub-01_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.809008 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.849009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/anat/sub-02_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.849009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/func/sub-02_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/func/sub-02_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/func/sub-02_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-02/func/sub-02_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.809008 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.849009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/anat/sub-03_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.849009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/func/sub-03_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/func/sub-03_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/func/sub-03_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-03/func/sub-03_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.809008 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.849009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/anat/sub-04_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.849009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/func/sub-04_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/func/sub-04_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/func/sub-04_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-04/func/sub-04_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.809008 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.849009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/anat/sub-05_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.849009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/func/sub-05_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/func/sub-05_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/func/sub-05_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-05/func/sub-05_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.809008 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.849009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/anat/sub-06_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.853009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/func/sub-06_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/func/sub-06_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/func/sub-06_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-06/func/sub-06_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.813008 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.853009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/anat/sub-07_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.853009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/func/sub-07_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/func/sub-07_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/func/sub-07_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-07/func/sub-07_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.813008 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.853009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/anat/sub-08_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.853009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/func/sub-08_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/func/sub-08_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/func/sub-08_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-08/func/sub-08_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.813008 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.853009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/anat/sub-09_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.853009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/func/sub-09_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/func/sub-09_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/func/sub-09_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-09/func/sub-09_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.813008 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.853009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/anat/sub-10_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.853009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/func/sub-10_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/func/sub-10_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/func/sub-10_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-10/func/sub-10_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.813008 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.853009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/anat/sub-11_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.857009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/func/sub-11_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/func/sub-11_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/func/sub-11_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-11/func/sub-11_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.813008 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.857009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/anat/sub-12_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.857009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/func/sub-12_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/func/sub-12_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/func/sub-12_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-12/func/sub-12_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.813008 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.857009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/anat/sub-13_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.857009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/func/sub-13_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/func/sub-13_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/func/sub-13_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-13/func/sub-13_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.813008 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.857009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/anat/sub-14_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.857009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/func/sub-14_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/func/sub-14_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/func/sub-14_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-14/func/sub-14_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.813008 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.857009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/anat/sub-15_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.857009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/func/sub-15_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/func/sub-15_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/func/sub-15_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-15/func/sub-15_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.813008 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.857009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/anat/sub-16_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.861009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/func/sub-16_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/func/sub-16_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/func/sub-16_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-16/func/sub-16_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.813008 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.861009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/anat/sub-17_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.861009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/func/sub-17_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/func/sub-17_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/func/sub-17_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-17/func/sub-17_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.813008 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.861009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/anat/sub-18_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.861009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/func/sub-18_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/func/sub-18_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/func/sub-18_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-18/func/sub-18_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.817008 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.861009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/anat/sub-19_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.861009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/func/sub-19_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/func/sub-19_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/func/sub-19_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-19/func/sub-19_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.817008 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.861009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/anat/sub-20_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.861009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/func/sub-20_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/func/sub-20_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/func/sub-20_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-20/func/sub-20_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.817008 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.861009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/anat/sub-21_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.865009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/func/sub-21_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/func/sub-21_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/func/sub-21_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-21/func/sub-21_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.817008 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.865009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/anat/sub-22_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.865009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/func/sub-22_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/func/sub-22_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/func/sub-22_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-22/func/sub-22_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.817008 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.865009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/anat/sub-23_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.865009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/func/sub-23_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/func/sub-23_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/func/sub-23_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-23/func/sub-23_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.817008 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.865009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/anat/sub-24_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.865009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/func/sub-24_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/func/sub-24_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/func/sub-24_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-24/func/sub-24_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.817008 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.865009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/anat/sub-25_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.865009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/func/sub-25_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/func/sub-25_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/func/sub-25_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-25/func/sub-25_task-flanker_run-2_events.tsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.817008 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.865009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/anat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/anat/sub-26_T1w.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.869009 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/func/sub-26_task-flanker_run-1_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/func/sub-26_task-flanker_run-1_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/func/sub-26_task-flanker_run-2_bold.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/sub-26/func/sub-26_task-flanker_run-2_events.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/task-flanker_bold.json
+-rw-r--r--   0 runner    (1001) docker     (127)    31050 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/test_bundle_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/test_csd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/test_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/test_dki.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/test_dti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/test_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/test_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12017 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/test_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/test_tractography.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tests/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.869009 pyafq-1.3.2/AFQ/tractography/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tractography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tractography/gputractography.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10235 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tractography/tractography.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/tractography/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.869009 pyafq-1.3.2/AFQ/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15159 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/utils/bin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/utils/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/utils/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/utils/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/utils/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/utils/streamlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10021 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/utils/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.869009 pyafq-1.3.2/AFQ/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/utils/tests/test_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/utils/tests/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/utils/tests/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/utils/tests/test_streamlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/utils/tests/test_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/utils/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-31 18:45:09.000000 pyafq-1.3.2/AFQ/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.873009 pyafq-1.3.2/AFQ/viz/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6880 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/viz/altair.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18554 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/viz/fury_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58032 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/viz/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25572 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/viz/plotly_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23112 2024-05-31 18:45:04.000000 pyafq-1.3.2/AFQ/viz/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36226 2024-05-31 18:45:04.000000 pyafq-1.3.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-31 18:45:04.000000 pyafq-1.3.2/CITATION
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-31 18:45:04.000000 pyafq-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-31 18:45:04.000000 pyafq-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-31 18:45:04.000000 pyafq-1.3.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-05-31 18:45:09.897009 pyafq-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-31 18:45:04.000000 pyafq-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.873009 pyafq-1.3.2/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4994 2024-05-31 18:45:04.000000 pyafq-1.3.2/bin/pyAFQ
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.873009 pyafq-1.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.873009 pyafq-1.3.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/_progressbars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.873009 pyafq-1.3.2/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)   272903 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/_static/BDE_Banner_revised20160211-01.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    56025 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/_static/eScience_Logo_HR.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/_static/escience-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   112939 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.873009 pyafq-1.3.2/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.877009 pyafq-1.3.2/docs/source/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.877009 pyafq-1.3.2/docs/source/explanations/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    14803 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/explanations/_static/down_left_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14739 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/explanations/_static/down_right_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/explanations/_static/greencheck.png
+-rw-r--r--   0 runner    (1001) docker     (127)    99285 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/explanations/_static/tract_modeling2.png
+-rw-r--r--   0 runner    (1001) docker     (127)   207285 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/explanations/_static/tract_profiling.png
+-rw-r--r--   0 runner    (1001) docker     (127)   220157 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/explanations/_static/tract_recognition.png
+-rw-r--r--   0 runner    (1001) docker     (127)   254342 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/explanations/_static/tract_tractography.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/explanations/bundle_orientation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/explanations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/explanations/modeling.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/explanations/profiling.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/explanations/recognition.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/explanations/tractography.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/explanations/tractometry_pipeline.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.877009 pyafq-1.3.2/docs/source/howto/
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/howto/cite.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/howto/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.881009 pyafq-1.3.2/docs/source/howto/developing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/howto/developing/definitions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/howto/developing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/howto/developing/releasing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/howto/developing/tasks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/howto/getting_help.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/howto/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/howto/installation_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.881009 pyafq-1.3.2/docs/source/howto/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/howto/usage/converter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/howto/usage/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/howto/usage/docker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/howto/usage/image.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/howto/usage/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/howto/usage/kwargs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/howto/usage/methods.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/howto/usage/scalars.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.881009 pyafq-1.3.2/docs/source/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/reference/bundledict.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8975 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/reference/kwargs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/reference/mapping.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8574 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/reference/methods.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/reference/viz_backend.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.881009 pyafq-1.3.2/docs/source/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/sphinxext/kwargsdocs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/sphinxext/methodsdocs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/sphinxext/updatedocs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.881009 pyafq-1.3.2/docs/source/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/source/tutorials/index.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      887 2024-05-31 18:45:04.000000 pyafq-1.3.2/docs/upload-gh-pages.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.821008 pyafq-1.3.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.885009 pyafq-1.3.2/examples/howto_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-31 18:45:04.000000 pyafq-1.3.2/examples/howto_examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10022 2024-05-31 18:45:04.000000 pyafq-1.3.2/examples/howto_examples/add_custom_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-05-31 18:45:04.000000 pyafq-1.3.2/examples/howto_examples/baby_afq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-31 18:45:04.000000 pyafq-1.3.2/examples/howto_examples/cerebellar_peduncles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-05-31 18:45:04.000000 pyafq-1.3.2/examples/howto_examples/cloudknot_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-05-31 18:45:04.000000 pyafq-1.3.2/examples/howto_examples/cloudknot_hcp_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-31 18:45:04.000000 pyafq-1.3.2/examples/howto_examples/plot_acoustic_radiations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-31 18:45:04.000000 pyafq-1.3.2/examples/howto_examples/plot_afq_callosal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-05-31 18:45:04.000000 pyafq-1.3.2/examples/howto_examples/plot_afq_fwdti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-31 18:45:04.000000 pyafq-1.3.2/examples/howto_examples/plot_optic_radiations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-31 18:45:04.000000 pyafq-1.3.2/examples/howto_examples/plot_recobundles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19258 2024-05-31 18:45:04.000000 pyafq-1.3.2/examples/howto_examples/plot_stages_of_tractometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-05-31 18:45:04.000000 pyafq-1.3.2/examples/howto_examples/use_subject_space_rois_from_freesurfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-31 18:45:04.000000 pyafq-1.3.2/examples/howto_examples/vof_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.885009 pyafq-1.3.2/examples/tutorial_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-31 18:45:04.000000 pyafq-1.3.2/examples/tutorial_examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-05-31 18:45:04.000000 pyafq-1.3.2/examples/tutorial_examples/plot_001_afq_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-05-31 18:45:04.000000 pyafq-1.3.2/examples/tutorial_examples/plot_002_bids_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19513 2024-05-31 18:45:04.000000 pyafq-1.3.2/examples/tutorial_examples/plot_003_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.885009 pyafq-1.3.2/gpu_docker/
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-31 18:45:04.000000 pyafq-1.3.2/gpu_docker/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (127)      401 2024-05-31 18:45:04.000000 pyafq-1.3.2/gpu_docker/cuda_build.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-31 18:45:04.000000 pyafq-1.3.2/gpu_docker/cuda_track_template.def
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-31 18:45:04.000000 pyafq-1.3.2/gpu_docker/docker-build.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-31 18:45:04.000000 pyafq-1.3.2/gpu_docker/docker-push.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.889009 pyafq-1.3.2/pyAFQ.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-05-31 18:45:09.000000 pyafq-1.3.2/pyAFQ.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21170 2024-05-31 18:45:09.000000 pyafq-1.3.2/pyAFQ.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 18:45:09.000000 pyafq-1.3.2/pyAFQ.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 18:45:09.000000 pyafq-1.3.2/pyAFQ.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-31 18:45:09.000000 pyafq-1.3.2/pyAFQ.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-31 18:45:09.000000 pyafq-1.3.2/pyAFQ.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:09.889009 pyafq-1.3.2/pyafq_docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-31 18:45:04.000000 pyafq-1.3.2/pyafq_docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-31 18:45:04.000000 pyafq-1.3.2/pyafq_docker/docker-build.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-31 18:45:04.000000 pyafq-1.3.2/pyafq_docker/docker-push.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-31 18:45:04.000000 pyafq-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-31 18:45:09.897009 pyafq-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-31 18:45:04.000000 pyafq-1.3.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-31 18:45:04.000000 pyafq-1.3.2/tox.ini
```

### Comparing `pyAFQ-1.3.1/.github/CONTRIBUTING.md` & `pyafq-1.3.2/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/.github/workflows/docbuild.yml` & `pyafq-1.3.2/.github/workflows/docbuild.yml`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/.github/workflows/docker_pyafq.yml` & `pyafq-1.3.2/.github/workflows/docker_pyafq.yml`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/.github/workflows/docker_pyafq_cuda12.yml` & `pyafq-1.3.2/.github/workflows/docker_pyafq_cuda12.yml`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/.github/workflows/nightly_anisotropic_test.yml` & `pyafq-1.3.2/.github/workflows/nightly_anisotropic_test.yml`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/.github/workflows/nightly_basic_test.yml` & `pyafq-1.3.2/.github/workflows/nightly_basic_test.yml`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/.github/workflows/nightly_custom_test.yml` & `pyafq-1.3.2/.github/workflows/nightly_custom_test.yml`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/.github/workflows/nightly_pft_test.yml` & `pyafq-1.3.2/.github/workflows/nightly_pft_test.yml`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/.github/workflows/nightly_reco80_test.yml` & `pyafq-1.3.2/.github/workflows/nightly_reco80_test.yml`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/.github/workflows/nightly_reco_test.yml` & `pyafq-1.3.2/.github/workflows/nightly_reco_test.yml`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/.github/workflows/nightly_test.yml` & `pyafq-1.3.2/.github/workflows/nightly_test.yml`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/.github/workflows/publish-to-test-pypi.yml` & `pyafq-1.3.2/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/.github/workflows/test.yml` & `pyafq-1.3.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/.mailmap` & `pyafq-1.3.2/.mailmap`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/.maintenance/update_changes.sh` & `pyafq-1.3.2/.maintenance/update_changes.sh`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/.maintenance/update_zenodo.py` & `pyafq-1.3.2/.maintenance/update_zenodo.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/.zenodo.json` & `pyafq-1.3.2/.zenodo.json`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/_fixes.py` & `pyafq-1.3.2/AFQ/_fixes.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/api/bundle_dict.py` & `pyafq-1.3.2/AFQ/api/bundle_dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -771,15 +771,14 @@
                 f" currently a {type(bundle_info)}"))
         self.seg_algo = seg_algo.lower()
         if resample_to is None:
             resample_to = afd.read_mni_template()
         self.resample_to = resample_to
         self.resample_subject_to = resample_subject_to
         self.keep_in_memory = keep_in_memory
-        self.has_bids_info = False
         self.max_includes = 3
 
         self._dict = {}
         self.bundle_names = []
         for key, item in bundle_info.items():
             self.__setitem__(key, item)
 
@@ -810,41 +809,31 @@
                     " Only Callosum Anterior Frontal will be used."))
                 self.bundle_names.remove("Forceps Minor")
 
     def update_max_includes(self, new_max):
         if new_max > self.max_includes:
             self.max_includes = new_max
 
-    def set_bids_info(self, bids_layout, bids_path, subject, session):
-        """
-        Provide the bids_layout, a nearest path,
-        and the subject and session information
-        to load ROIS from BIDS
-        """
-        self.has_bids_info = True
-        self._bids_info = bids_layout
-        self._bids_path = bids_path
-        self._subject = subject
-        self._session = session
-
-    def _cond_load(self, roi_or_sl, resample_to):
-        """
-        Load ROI or streamline if not already loaded
-        """
+    def _use_bids_info(self, roi_or_sl, bids_layout, bids_path,
+                       subject, session):
         if isinstance(roi_or_sl, dict):
-            if not self.has_bids_info:
-                raise ValueError((
-                    "Attempted to load an ROI using BIDS description without "
-                    "First providing BIDS information."))
             suffix = roi_or_sl.get("suffix", "dwi")
             roi_or_sl = find_file(
-                self._bids_info, self._bids_path,
+                bids_layout, bids_path,
                 roi_or_sl,
                 suffix,
-                self._session, self._subject)
+                session, subject)
+            return roi_or_sl
+        else:
+            return roi_or_sl
+
+    def _cond_load(self, roi_or_sl, resample_to):
+        """
+        Load ROI or streamline if not already loaded
+        """
         if isinstance(roi_or_sl, str):
             if self.seg_algo == "afq":
                 return afd.read_resample_roi(
                     roi_or_sl,
                     resample_to=resample_to)
             elif self.seg_algo.startswith("reco"):
                 return load_tractogram(
```

### Comparing `pyAFQ-1.3.1/AFQ/api/group.py` & `pyafq-1.3.2/AFQ/api/group.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # -*- coding: utf-8 -*-# -*- coding: utf-8 -*-
 import warnings
 import tempfile
 
 from AFQ.definitions.mapping import SynMap
+from AFQ.definitions.utils import Definition
+import AFQ.api.bundle_dict as abd
 warnings.simplefilter(action='ignore', category=FutureWarning)  # noqa
 
 import logging
 from AFQ.api.participant import ParticipantAFQ
 from AFQ.api.utils import (
     check_attribute, AFQclass_doc,
     export_all_helper, valid_exports_string)
@@ -18,24 +20,26 @@
 import dipy.tracking.streamlinespeed as dps
 import dipy.tracking.streamline as dts
 from dipy.io.streamline import save_tractogram
 
 from AFQ.version import version as pyafq_version
 from AFQ.viz.utils import trim
 import pandas as pd
+import pydra
 import numpy as np
 import os
 import os.path as op
 from tqdm import tqdm
 import json
 import s3fs
 from time import time
 import nibabel as nib
 from PIL import Image
 from s3bids.utils import S3BIDSStudy
+import glob
 
 from bids.layout import BIDSLayout, BIDSLayoutIndexer
 try:
     import afqbrowser as afqb
     using_afqb = True
 except ImportError:
     using_afqb = False
@@ -56,14 +60,25 @@
 
 
 def get_afq_bids_entities_fname():
     return op.dirname(op.dirname(op.abspath(
         aus.__file__))) + "/afq_bids_entities.json"
 
 
+class _ParticipantAFQInputs:
+    def __init__(
+            self, dwi_data_file, bval_file, bvec_file, results_dir,
+            kwargs):
+        self.dwi_data_file = dwi_data_file
+        self.bval_file = bval_file
+        self.bvec_file = bvec_file
+        self.results_dir = results_dir
+        self.kwargs = kwargs
+
+
 class GroupAFQ(object):
     f"""{AFQclass_doc}"""
 
     def __init__(self,
                  bids_path,
                  bids_filters={"suffix": "dwi"},
                  preproc_pipeline="all",
@@ -142,14 +157,15 @@
             raise TypeError(
                 "output_dir must be either a str or None")
         if not isinstance(parallel_params, dict):
             raise TypeError("parallel_params must be a dict")
         if not isinstance(bids_layout_kwargs, dict):
             raise TypeError("bids_layout_kwargs must be a dict")
 
+
         self.logger = logger
 
         self.parallel_params = parallel_params
         self.wf_dict = {}
 
         # validate input and fail early
         if not op.exists(bids_path):
@@ -248,14 +264,15 @@
                 kwargs["segmentation_params"]["parallel_segmentation"] = {}
             kwargs["segmentation_params"]["parallel_segmentation"]["engine"] =\
                 "serial"
 
         self.valid_sub_list = []
         self.valid_ses_list = []
         self.pAFQ_list = []
+        self.pAFQ_inputs_list = []
         for subject in self.subjects:
             self.wf_dict[subject] = {}
             for session in self.sessions:
                 this_kwargs = kwargs.copy()
                 results_dir = op.join(self.afq_path, 'sub-' + subject)
 
                 if session is not None:
@@ -292,28 +309,98 @@
                     **bids_filters)
                 bval_file = bids_layout.get_bval(
                     dwi_data_file,
                     **bids_filters)
                 if suffix is not None:
                     bids_filters["suffix"] = suffix
 
+                # Call find path for all definitions
+                for key, value in this_kwargs.items():
+                    if key == "scalars":
+                        for scalar in this_kwargs["scalars"]:
+                            if isinstance(scalar, Definition):
+                                scalar_found = scalar.find_path(
+                                    bids_layout,
+                                    dwi_data_file,
+                                    subject,
+                                    session,
+                                    required=False)
+                                if scalar_found is False:
+                                    this_kwargs["scalars"].remove(scalar)
+                    elif key == "import_tract":
+                        if isinstance(this_kwargs["import_tract"], dict):
+                            it_res = \
+                                bids_layout.get(
+                                    subject=subject,
+                                    session=session,
+                                    extension=[
+                                        '.trk',
+                                        '.tck',
+                                        '.vtk',
+                                        '.fib',
+                                        '.dpy'],
+                                    return_type='filename',
+                                    **this_kwargs["import_tract"])
+                            if len(it_res) < 1:
+                                raise ValueError((
+                                    "No custom tractography found for"
+                                    f" subject {subject}"
+                                    " and session "
+                                    f"{session}."))
+                            elif len(it_res) > 1:
+                                this_kwargs["import_tract"] = it_res[0]
+                                logger.warning((
+                                    f"Multiple viable custom tractographies found for"
+                                    f" subject "
+                                    f"{subject} and session "
+                                    f"{session}. Will use: {it_res[0]}"))
+                            else:
+                                this_kwargs["import_tract"] = it_res[0]
+                    elif isinstance(value, dict):
+                        for _, subvalue in value.items():
+                            if isinstance(subvalue, Definition):
+                                subvalue.find_path(
+                                    bids_layout,
+                                    dwi_data_file,
+                                    subject,
+                                    session)
+                    elif isinstance(value, Definition):
+                        value.find_path(
+                            bids_layout,
+                            dwi_data_file,
+                            subject,
+                            session)
+
+                # call find path for all ROIs
+                if "bundle_info" in this_kwargs and isinstance(
+                        this_kwargs["bundle_info"], abd.BundleDict):
+                    for b_name in this_kwargs["bundle_info"].bundle_names:
+                        this_kwargs["bundle_info"].apply_to_rois(
+                            b_name,
+                            this_kwargs["bundle_info"]._use_bids_info,
+                            bids_layout, bids_path, subject, session,
+                            dry_run=False)
+
                 self.valid_sub_list.append(subject)
                 self.valid_ses_list.append(str(session))
 
-                this_pAFQ = ParticipantAFQ(
+                this_pAFQ_inputs = _ParticipantAFQInputs(
                     dwi_data_file,
                     bval_file, bvec_file,
                     results_dir,
-                    _bids_info={
-                        "bids_layout": bids_layout,
-                        "subject": subject,
-                        "session": session},
-                    **this_kwargs)
+                    this_kwargs)
+                this_pAFQ = ParticipantAFQ(
+                    this_pAFQ_inputs.dwi_data_file,
+                    this_pAFQ_inputs.bval_file,
+                    this_pAFQ_inputs.bvec_file,
+                    this_pAFQ_inputs.results_dir,
+                    **this_pAFQ_inputs.kwargs)
                 self.wf_dict[subject][str(session)] = this_pAFQ.wf_dict
                 self.pAFQ_list.append(this_pAFQ)
+                self.pAFQ_inputs_list.append(this_pAFQ_inputs)
 
     def combine_profiles(self):
         tract_profiles_dict = self.export("profiles")
         if len(self.sessions) > 1:
             tract_profiles_list = []
             for _, subject_dict in tract_profiles_dict.items():
                 tract_profiles_list.extend(subject_dict.values())
@@ -912,14 +999,147 @@
             streamlines=sls_json_fname,
             title=page_title,
             subtitle=page_subtitle,
             link=page_title_link,
             sublink=page_subtitle_link)
 
 
+class ParallelGroupAFQ():
+    def __init__(self, *args, **kwargs):
+        orig = GroupAFQ(*args, **kwargs)
+
+        orig.parallel_params["submitter_params"] = \
+            orig.parallel_params.get("submitter_params", {"plugin": "cf"})
+        
+        orig.parallel_params["cache_dir"] = \
+            orig.parallel_params.get("cache_dir", None)
+
+        self.parallel_params = orig.parallel_params
+        self.pAFQ_kwargs = orig.pAFQ_inputs_list
+
+        self.finishing_params = dict()
+        self.finishing_params["args"] = args
+        self.finishing_params["kwargs"] = kwargs
+        self.finishing_params["output_dirs"] = [pAFQ.kwargs["output_dir"]
+                                                for pAFQ in orig.pAFQ_list]
+
+    def _submit_pydra(self, runnable):
+        try:
+            with pydra.Submitter(
+                **self.parallel_params["submitter_params"],
+            ) as sub:
+                sub(runnable=runnable)
+        # Addresses https://github.com/nipype/pydra/issues/630
+        except AttributeError as e:
+            if "'NoneType' object has no attribute 'replace'" not in str(e):
+                raise
+
+    def export(self, attr_name="help", collapse=True):
+        f"""
+        Export a specific output. To print a list of available outputs,
+        call export without arguments.
+        {valid_exports_string}
+
+        Parameters
+        ----------
+        attr_name : str
+            Name of the output to export. Default: "help"
+        collapse : bool
+            Whether to collapse session dimension if there is only 1 session.
+            Default: True
+
+        Returns
+        -------
+        output : dict
+            The specific output as a dictionary. Keys are subjects.
+            Values are dictionaries with keys of sessions
+            if multiple sessions are used. Otherwise, values are
+            the output.
+            None if called without arguments.
+        """
+
+        @pydra.mark.task
+        def export_sub(pAFQ_kwargs, attr_name):
+            pAFQ = ParticipantAFQ(
+                pAFQ_kwargs.dwi_data_file,
+                pAFQ_kwargs.bval_file,
+                pAFQ_kwargs.bvec_file,
+                pAFQ_kwargs.results_dir,
+                **pAFQ_kwargs.kwargs)
+            pAFQ.export(attr_name)
+
+        # Submit to pydra
+        export_sub_task = export_sub(
+            attr_name=attr_name,
+            cache_dir=self.parallel_params["cache_dir"]
+        ).split("pAFQ_kwargs", pAFQ_kwargs=self.pAFQ_kwargs)
+        self._submit_pydra(export_sub_task)
+
+    def export_all(self, viz=True, afqbrowser=True, xforms=True, indiv=True):
+        """ Exports all the possible outputs
+
+        Parameters
+        ----------
+        viz : bool
+            Whether to output visualizations. This includes tract profile
+            plots, a figure containing all bundles, and, if using the AFQ
+            segmentation algorithm, individual bundle figures.
+            Default: True
+        afqbrowser : bool
+            Whether to output an AFQ-Browser from this AFQ instance.
+            Default: True
+        xforms : bool
+            Whether to output the reg_template image in subject space and,
+            depending on if it is possible based on the mapping used, to
+            output the b0 in template space.
+            Default: True
+        indiv : bool
+            Whether to output individual bundles in their own files, in
+            addition to the one file containing all bundles. If using
+            the AFQ segmentation algorithm, individual ROIs are also
+            output.
+            Default: True
+        """
+        @pydra.mark.task
+        def export_sub(
+            pAFQ_kwargs,
+            finishing_params,
+            viz,
+            afqbrowser,
+            xforms,
+            indiv
+        ):
+            pAFQ = ParticipantAFQ(
+                pAFQ_kwargs.dwi_data_file,
+                pAFQ_kwargs.bval_file,
+                pAFQ_kwargs.bvec_file,
+                pAFQ_kwargs.results_dir,
+                **pAFQ_kwargs.kwargs)
+            pAFQ.export_all(viz, xforms, indiv)
+
+            for dir in finishing_params["output_dirs"]:
+                if not glob.glob(op.join(dir, "*_desc-profiles_dwi.csv")):
+                    return
+
+            gAFQ = GroupAFQ(*finishing_params["args"],
+                            **finishing_params["kwargs"])
+            gAFQ.export_all(viz, afqbrowser, xforms, indiv)
+
+        # Submit to pydra
+        export_sub_task = export_sub(
+            finishing_params=self.finishing_params,
+            viz=viz,
+            afqbrowser=afqbrowser,
+            xforms=xforms,
+            indiv=indiv,
+            cache_dir=self.parallel_params["cache_dir"]
+        ).split("pAFQ_kwargs", pAFQ_kwargs=self.pAFQ_kwargs)
+        self._submit_pydra(export_sub_task)
+
+
 def download_and_combine_afq_profiles(bucket,
                                       study_s3_prefix="", deriv_name=None,
                                       out_file=None,
                                       upload=False, session=None,
                                       **kwargs):
     """
     Download and combine tract profiles from different subjects / sessions
```

### Comparing `pyAFQ-1.3.1/AFQ/api/participant.py` & `pyafq-1.3.2/AFQ/api/participant.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,33 +30,28 @@
 class ParticipantAFQ(object):
     f"""{AFQclass_doc}"""
 
     def __init__(self,
                  dwi_data_file,
                  bval_file, bvec_file,
                  output_dir,
-                 _bids_info=None,
                  **kwargs):
         """
-        Initialize a ParticipantAFQ object from a BIDS dataset.
+        Initialize a ParticipantAFQ object.
 
         Parameters
         ----------
         dwi_data_file : str
             Path to DWI data file.
         bval_file : str
             Path to bval file.
         bvec_file : str
             Path to bvec file.
         output_dir : str
             Path to output directory.
-        _bids_info : dict or None, optional
-            This should be left as None in most cases. It
-            is used by GroupAFQ to provide information about
-            the BIDS layout to each participant.
         kwargs : additional optional parameters
             You can set additional parameters for any step
             of the process. See :ref:`usage/kwargs` for more details.
 
         Examples
         --------
         api.ParticipantAFQ(
@@ -67,17 +62,14 @@
             reg_template_spec="mni_t2", reg_subject_spec="b0")
 
         Notes
         -----
         In tracking_params, parameters with the suffix mask which are also
         an image from AFQ.definitions.image will be handled automatically by
         the api.
-
-        It is recommended that you leave the bids_info parameter as None,
-        and instead pass in the paths to the files you want to use directly.
         """
         if not isinstance(output_dir, str):
             raise TypeError(
                 "output_dir must be a str")
         if not isinstance(dwi_data_file, str):
             raise TypeError(
                 "dwi_data_file must be a str")
@@ -92,41 +84,46 @@
                 f"output_dir does not exist: {output_dir}")
         if "tractography_params" in kwargs:
             raise ValueError((
                 "unrecognized parameter tractography_params, "
                 "did you mean tracking_params ?"))
 
         self.logger = logging.getLogger('AFQ')
-        self.output_dir = output_dir
 
         self.kwargs = dict(
-            dwi_path=dwi_data_file,
-            bval=bval_file,
-            bvec=bvec_file,
-            results_dir=output_dir,
-            bids_info=_bids_info,
+            dwi_data_file=dwi_data_file,
+            bval_file=bval_file,
+            bvec_file=bvec_file,
+            output_dir=output_dir,
             base_fname=get_base_fname(output_dir, dwi_data_file),
             **kwargs)
         self.make_workflow()
 
     def make_workflow(self):
         # construct pimms plans
         if "mapping_definition" in self.kwargs and isinstance(
                 self.kwargs["mapping_definition"], SlrMap):
             plans = {  # if using SLR map, do tractography first
                 "data": get_data_plan(self.kwargs),
-                "tractography": get_tractography_plan(self.kwargs),
-                "mapping": get_mapping_plan(self.kwargs, use_sls=True),
+                "tractography": get_tractography_plan(
+                    self.kwargs
+                ),
+                "mapping": get_mapping_plan(
+                    self.kwargs,
+                    use_sls=True
+                ),
                 "segmentation": get_segmentation_plan(self.kwargs),
                 "viz": get_viz_plan(self.kwargs)}
         else:
             plans = {  # Otherwise, do mapping first
                 "data": get_data_plan(self.kwargs),
                 "mapping": get_mapping_plan(self.kwargs),
-                "tractography": get_tractography_plan(self.kwargs),
+                "tractography": get_tractography_plan(
+                    self.kwargs
+                ),
                 "segmentation": get_segmentation_plan(self.kwargs),
                 "viz": get_viz_plan(self.kwargs)}
 
         # chain together a complete plan from individual plans
         previous_data = {}
         for name, plan in plans.items():
             previous_data[f"{name}_imap"] = plan(
@@ -276,15 +273,15 @@
                     focal_point=data_shape // 2,
                     view_up=(0, 0, 1))
                 figure.zoom(0.5)
                 window.snapshot(figure, fname=this_fname, size=(600, 600))
 
         def _save_file(curr_img):
             save_path = op.abspath(op.join(
-                self.output_dir,
+                self.kwargs["output_dir"],
                 "bundle_montage.png"))
             curr_img.save(save_path)
             all_fnames.append(save_path)
 
         this_img_trimmed = {}
         max_height = 0
         max_width = 0
@@ -370,15 +367,15 @@
                 exception_file_names.append(file_name)
             else:
                 self.logger.warn((
                     f"The exception '{exception}' does not correspond"
                     " to a filename and will be ignored."))
 
         apply_cmd_to_afq_derivs(
-            self.output_dir,
+            self.kwargs["output_dir"],
             self.export("base_fname"),
             cmd=cmd,
             exception_file_names=exception_file_names,
             suffix=suffix,
             dependent_on=dependent_on
         )
```

### Comparing `pyAFQ-1.3.1/AFQ/api/utils.py` & `pyafq-1.3.2/AFQ/api/utils.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/data/fetch.py` & `pyafq-1.3.2/AFQ/data/fetch.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,15 +259,15 @@
     "2efe0deb19ac9e175404bf0cb29d9dbd", "c2e07cd50699527bd7b0cbbe88703c56",
     "76b36d8d6759df58131644281ed16bd2", "645102225bad33da30bafd41d24b3ab0",
     "45ec94d42fdc9448afa6760c656920e9", "54e3cb1b8c242be279f1410d8bb3c383",
     "1ee9f7e8b21ef8ceee81d5a7a178ef33", "4f11097f7ae317aa8d612511be79e2f1",
     "1c4c0823c23b676d6d35004d93b9c695", "d4830d558cc8f707ebec912b32d197a5",
     "c405e0dbd9a4091c77b3d1ad200229b4", "ec0aeccc6661d2ee5ed79259383cdcee",
     "2802cd227b550f6e85df0fec1d515c29", "385addb999dc6d76957d2a35c4ee74bb",
-    "b79f01829bd95682faaf545c72b1d52c", "b79f01829bd95682faaf545c72b1d52c",
+    "0dd14c02b272263adbe2246880979c9d", "99dac5a00c10d81d222f020162fd6194",
     "e49ba370edca96734d9376f551d413db", "f59e9e69e06325198f70047cd63c3bdc",
     "ae3bd2931f95adae0280a8f75cd3ca9b", "c409a0036b8c2dd4d03d11fbc6bfbdcd",
     "c2597a474ea5ec9e3126c35fd238f6b2", "67af59c934147c9f9ff6e0b76c4cc6eb",
     "72d0bbc0b6162e9291fdc450c103a1f0", "51f5041be63ad0ac10d1ac09e3bf1a8e",
     "6200f5cdc1402dce46dedd505468b147", "83cb5bf6b9b1eda63c8643871e84a6d4",
     "2a5d8d309b1256d6e48958e112201c2c", "ba24d0915fdff215a403480d0a7745c9",
     "1001e833d1344274d543ffd02a66af80", "03e20c5eebcd4d439c4ffb36d26a10d9",
@@ -299,15 +299,15 @@
     "0ecabd68fa9c56614e2a694359c0a545",
     "4c93bea7a72ac2b7475201acef5a1fc4",
 ]
 
 pediatric_remote_fnames = [
     "24880625", "24880628", "24880631", "24880634", "24880637", "24880640",
     "24880643", "24880646", "24880649", "24880652", "24880655", "24880661",
-    "24880664", "24880667", "24880670", "24880673", "24880676", "24880679",
+    "24880664", "24880667", "46407571", "46407568", "24880676", "24880679",
     "24880685", "24880688", "24880691", "24880694", "24880697", "24880700",
     "24880703", "24880706", "24880712", "24880715", "24880718", "24880721",
     "24880724", "24880727", "24880730", "24880733", "24880736", "24880748",
     "24880739", "24880742", "24880754", "24880757", "24880760", "24880763",
     "24880769", "24880772", "24880775", "24880778", "24880781", "24880787",
     "24880790", "24880793", "24880796", "24880802", "24880805", "24880808",
     "24880616", "24880613", "24986396",
@@ -534,15 +534,15 @@
                    "ATR_L_start.nii.gz"]
 
 
 template_remote_fnames = ["5273680", "5273683", "5273686", "5273689",
                           "11458274", "11458277",
                           "5273695", "5273692", "5273698", "5273701",
                           "11458268", "11458271",
-                          "5273704", "5273707", "5273710", "5273713",
+                          "5273704", "5273707", "46407574", "46407577",
                           "11458262", "11458265",
                           "5273716", "5273719",
                           "11458220",
                           "5273722", "5273725",
                           "11458226",
                           "5273728", "5273731", "5273734", "5273746",
                           "11458259", "11458256",
@@ -608,16 +608,16 @@
                        "c5fa4e6e685e695c006823b6784d2407",
                        "e1fab77f21d5303ed52285f015e24f0b",
                        "5f89defec3753fd75cd688c7bfb20a36",
                        "a4f3cd65b06fb25f63d5dab7592f00f2",
                        "7e73ab02db30a3ad6bd9e82148c2486e",
                        "f9db3154955a20b67c2dda758800d14c",
                        "73941510c798c1ed1b03e2bd481cd5c7",
-                       "660cdc031ee0716d60159c7d933119ea",
-                       "660cdc031ee0716d60159c7d933119ea",
+                       "b20e0caa54cf35002cd06cf6033b964f",
+                       "e751306df304af32c3ce7617913bbd30",
                        "fd012bc89f6bed7bd54530195496bac4",
                        "3406906a86e633cc102127cf210a1063",
                        "9040a7953dcbbf131d135c866182d8ef",
                        "a72e17194824fcd838a594a2eb50c72e",
                        "627d7bb2e6d55f8243da815a36d9ff1a",
                        "55adbe9b8279185eedbe342149e1ff90",
                        "5a7412a3cf0fb185eec53d1989df2f7c",
```

### Comparing `pyAFQ-1.3.1/AFQ/data/utils.py` & `pyafq-1.3.2/AFQ/data/utils.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/definitions/image.py` & `pyafq-1.3.2/AFQ/definitions/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,39 +134,36 @@
         nearest_image = find_file(
             bids_layout, from_path, self.filters, self.suffix, session,
             subject, required=required)
 
         if nearest_image is None:
             return False
 
-        if session not in self.fnames:
-            self.fnames[session] = {}
-        self.fnames[session][subject] = nearest_image
+        self.fnames[from_path] = nearest_image
 
-    def get_path_data_affine(self, bids_info):
+    def get_path_data_affine(self, dwi_path):
         if self._from_path:
             image_file = self.fname
         else:
-            image_file = self.fnames[
-                bids_info['session']][bids_info['subject']]
+            image_file = self.fnames[dwi_path]
         image_img = nib.load(image_file)
         return image_file, image_img.get_fdata(), image_img.affine
 
     # This function is set up to be overriden by other images
     def apply_conditions(self, image_data_orig, image_file):
         return image_data_orig, dict(source=image_file)
 
     def get_name(self):
         return name_from_path(self.fname) if self._from_path else self.suffix
 
     def get_image_getter(self, task_name):
-        def _image_getter_helper(dwi, bids_info):
+        def _image_getter_helper(dwi, dwi_data_file):
             # Load data
             image_file, image_data_orig, image_affine = \
-                self.get_path_data_affine(bids_info)
+                self.get_path_data_affine(dwi_data_file)
 
             # Apply any conditions on the data
             image_data, meta = self.apply_conditions(
                 image_data_orig, image_file)
 
             # Resample to DWI data:
             image_data = _resample_image(
@@ -174,19 +171,19 @@
                 dwi.get_fdata(),
                 image_affine,
                 dwi.affine)
             return nib.Nifti1Image(
                 image_data.astype(np.float32),
                 dwi.affine), meta
         if task_name == "data":
-            def image_getter(dwi, bids_info):
-                return _image_getter_helper(dwi, bids_info)
+            def image_getter(dwi, dwi_data_file):
+                return _image_getter_helper(dwi, dwi_data_file)
         else:
-            def image_getter(data_imap, bids_info):
-                return _image_getter_helper(data_imap["dwi"], bids_info)
+            def image_getter(data_imap, dwi_data_file):
+                return _image_getter_helper(data_imap["dwi"], dwi_data_file)
         return image_getter
 
 
 class FullImage(ImageDefinition):
     """
     Define an image which covers a full volume.
```

### Comparing `pyAFQ-1.3.1/AFQ/definitions/mapping.py` & `pyafq-1.3.2/AFQ/definitions/mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,23 +116,22 @@
             bids_layout, from_path, self.warp_filters, self.warp_suffix,
             session, subject, required=required)
 
         nearest_space = find_file(
             bids_layout, from_path, self.space_filters, self.space_suffix,
             session, subject, required=required)
 
-        self.fnames[session][subject] = (nearest_warp, nearest_space)
+        self.fnames[from_path] = (nearest_warp, nearest_space)
 
-    def get_for_subses(self, base_fname, dwi, bids_info, reg_subject,
+    def get_for_subses(self, base_fname, dwi, dwi_data_file, reg_subject,
                        reg_template):
         if self._from_path:
             nearest_warp, nearest_space = self.fnames
         else:
-            nearest_warp, nearest_space = self.fnames[
-                bids_info['session']][bids_info['subject']]
+            nearest_warp, nearest_space = self.fnames[dwi_data_file]
 
         our_templ = reg_template
         subj = Image(dwi)
         their_templ = Image(nearest_space)
         warp = readFnirt(nearest_warp, their_templ, subj)
 
         return ConformedFnirtMapping(warp, our_templ.affine)
@@ -178,15 +177,15 @@
     my_example_mapping = IdentityMap()
     api.GroupAFQ(mapping=my_example_mapping)
     """
 
     def __init__(self):
         pass
 
-    def get_for_subses(self, base_fname, dwi, bids_info, reg_subject,
+    def get_for_subses(self, base_fname, dwi, dwi_data_file, reg_subject,
                        reg_template):
         return ConformedAffineMapping(
             np.identity(4),
             domain_grid_shape=reg.reduce_shape(
                 reg_subject.shape),
             domain_grid2world=reg_subject.affine,
             codomain_grid_shape=reg.reduce_shape(
@@ -227,15 +226,15 @@
             logger.info(f"Saving {prealign_file}")
             np.save(prealign_file, aff)
             meta_fname = get_fname(
                 base_fname, f'{prealign_file_desc}.json')
             write_json(meta_fname, meta)
         return prealign_file if save else np.load(prealign_file)
 
-    def get_for_subses(self, base_fname, dwi, bids_info, reg_subject,
+    def get_for_subses(self, base_fname, dwi, dwi_data_file, reg_subject,
                        reg_template, subject_sls=None, template_sls=None):
         mapping_file, meta_fname = self.get_fnames(
             self.extension, base_fname)
 
         if self.use_prealign:
             reg_prealign = np.load(self.prealign(
                 base_fname, reg_subject, reg_template))
```

### Comparing `pyAFQ-1.3.1/AFQ/definitions/utils.py` & `pyafq-1.3.2/AFQ/definitions/utils.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/models/QBallTP.py` & `pyafq-1.3.2/AFQ/models/QBallTP.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/models/csd.py` & `pyafq-1.3.2/AFQ/models/csd.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 __all__ = ["fit_csd"]
 
 
 class CsdNanResponseError(Exception):
     pass
 
 
-def _model(gtab, data, response=None, sh_order=None):
+def _model(gtab, data, response=None, sh_order=None, csd_fa_thr=0.7):
     """
     Helper function that defines a CSD model.
     """
     if sh_order is None:
         ndata = np.sum(~gtab.b0s_mask)
         # See dipy.reconst.shm.calculate_max_order
         L1 = (-3 + np.sqrt(1 + 8 * ndata)) / 2.0
@@ -46,28 +46,30 @@
                                            gtab.bvecs[low_shell_idx])
             data = data[..., low_shell_idx]
         else:
             response_gtab = gtab
         response, _ = csd.auto_response_ssst(response_gtab,
                                              data,
                                              roi_radii=10,
-                                             fa_thr=0.7)
+                                             fa_thr=csd_fa_thr)
     # Catch conditions where an auto-response could not be calculated:
     if np.all(np.isnan(response[0])):
         raise CsdNanResponseError
 
     csdmodel = my_model(gtab, response, sh_order=sh_order)
     return csdmodel
 
 
-def _fit(gtab, data, mask, response=None, sh_order=None, lambda_=1, tau=0.1):
+def _fit(gtab, data, mask, response=None, sh_order=None,
+         lambda_=1, tau=0.1, csd_fa_thr=0.7):
     """
     Helper function that does the core of fitting a model to data.
     """
-    return _model(gtab, data, response, sh_order).fit(data, mask=mask)
+    return _model(gtab, data, response, sh_order, csd_fa_thr).fit(
+        data, mask=mask)
 
 
 def fit_csd(data_files, bval_files, bvec_files, mask=None, response=None,
             b0_threshold=50, sh_order=None, lambda_=1, tau=0.1, out_dir=None):
     """
     Fit the CSD model and save file with SH coefficients.
```

### Comparing `pyAFQ-1.3.1/AFQ/models/dki.py` & `pyafq-1.3.2/AFQ/models/dki.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/models/dti.py` & `pyafq-1.3.2/AFQ/models/dti.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/models/fwdti.py` & `pyafq-1.3.2/AFQ/models/fwdti.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/registration.py` & `pyafq-1.3.2/AFQ/registration.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/segmentation.py` & `pyafq-1.3.2/AFQ/segmentation.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/tasks/data.py` & `pyafq-1.3.2/AFQ/tasks/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import nibabel as nib
 import numpy as np
 import logging
 
 from dipy.io.gradients import read_bvals_bvecs
 import dipy.core.gradients as dpg
+from dipy.data import default_sphere
 
 import pimms
 
 import dipy.reconst.dki as dpy_dki
 import dipy.reconst.dti as dpy_dti
 import dipy.reconst.fwdti as dpy_fwdti
 import dipy.reconst.msdki as dpy_msdki
 from dipy.reconst.gqi import GeneralizedQSamplingModel
+from dipy.reconst.rumba import RumbaSDModel, RumbaFit
 from dipy.reconst import shm
 from dipy.reconst.dki_micro import axonal_water_fraction
 
 from AFQ.tasks.decorators import as_file, as_img, as_fit_deriv
 from AFQ.tasks.utils import get_fname, with_name, str_to_desc
 import AFQ.api.bundle_dict as abd
 import AFQ.data.fetch as afd
@@ -38,15 +40,15 @@
 logger = logging.getLogger('AFQ')
 
 
 DIPY_GH = "https://github.com/dipy/dipy/blob/master/dipy/"
 
 
 @pimms.calc("data", "gtab", "dwi", "dwi_affine")
-def get_data_gtab(dwi_path, bval, bvec, min_bval=None,
+def get_data_gtab(dwi_data_file, bval_file, bvec_file, min_bval=None,
                   max_bval=None, filter_b=True, b0_threshold=50):
     """
     DWI data as an ndarray for selected b values,
     A DIPY GradientTable with all the gradient information,
     and DWI data in a Nifti1Image,
     and the affine transformation of the DWI data.
 
@@ -63,16 +65,16 @@
     filter_b : bool, optional
         Whether to filter the DWI data based on min or max bvals.
         Default: True
     b0_threshold : int, optional
         The value of b under which
         it is considered to be b0. Default: 50.
     """
-    img = nib.load(dwi_path)
-    bvals, bvecs = read_bvals_bvecs(bval, bvec)
+    img = nib.load(dwi_data_file)
+    bvals, bvecs = read_bvals_bvecs(bval_file, bvec_file)
 
     data = img.get_fdata()
     if filter_b and (min_bval is not None):
         valid_b = np.logical_or(
             (bvals >= min_bval), (bvals <= b0_threshold))
         data = data[..., valid_b]
         bvals = bvals[valid_b]
@@ -88,23 +90,23 @@
         b0_threshold=b0_threshold)
     img = nib.Nifti1Image(data, img.affine)
     return data, gtab, img, img.affine
 
 
 @pimms.calc("b0")
 @as_file('_desc-b0_dwi.nii.gz')
-def b0(dwi_path, gtab):
+def b0(dwi_data_file, gtab):
     """
     full path to a nifti file containing the mean b0
     """
-    data = nib.load(dwi_path)
+    data = nib.load(dwi_data_file)
     mean_b0 = np.mean(data.get_fdata()[..., gtab.b0s_mask], -1)
     mean_b0_img = nib.Nifti1Image(mean_b0, data.affine)
     meta = dict(b0_threshold=gtab.b0_threshold,
-                source=dwi_path)
+                source=dwi_data_file)
     return mean_b0_img, meta
 
 
 @pimms.calc("masked_b0")
 @as_file('_desc-maskedb0_dwi.nii.gz')
 def b0_mask(b0, brain_mask):
     """
@@ -132,15 +134,16 @@
     return dpy_dti.TensorFit(tm, dti_params)
 
 
 @pimms.calc("dti_params")
 @as_file(suffix='_odfmodel-DTI_desc-diffmodel_dwi.nii.gz')
 @as_img
 def dti_params(brain_mask, data, gtab,
-               bval, bvec, b0_threshold=50, robust_tensor_fitting=False):
+               bval_file, bvec_file, b0_threshold=50,
+               robust_tensor_fitting=False):
     """
     full path to a nifti file containing parameters
     for the DTI fit
 
     Parameters
     ----------
     robust_tensor_fitting : bool, optional
@@ -151,15 +154,15 @@
         The value of b under which
         it is considered to be b0. Default: 50.
     """
     mask =\
         nib.load(brain_mask).get_fdata()
     if robust_tensor_fitting:
         bvals, _ = read_bvals_bvecs(
-            bval, bvec)
+            bval_file, bvec_file)
         sigma = noise_from_b0(
             data, gtab, bvals,
             mask=mask, b0_threshold=b0_threshold)
     else:
         sigma = None
     dtf = dti_fit_model(
         gtab, data,
@@ -212,14 +215,19 @@
 @as_file(suffix='_odfmodel-DKI_desc-diffmodel_dwi.nii.gz')
 @as_img
 def dki_params(brain_mask, gtab, data):
     """
     full path to a nifti file containing
     parameters for the DKI fit
     """
+    if len(dpg.unique_bvals_magnitude(gtab.bvals)) < 3:
+        raise ValueError((
+            "The DKI model requires at least 2 non-zero b-values, "
+            f"but you provided {len(dpg.unique_bvals_magnitude(gtab.bvals))}"
+            " b-values (including b=0)."))
     mask =\
         nib.load(brain_mask).get_fdata()
     dkf = dki_fit_model(
         gtab, data,
         mask=mask)
     meta = dict(
         Parameters=dict(
@@ -277,15 +285,16 @@
 
 
 @pimms.calc("csd_params")
 @as_file(suffix='_odfmodel-CSD_desc-diffmodel_dwi.nii.gz')
 @as_img
 def csd_params(dwi, brain_mask, gtab, data,
                csd_response=None, csd_sh_order=None,
-               csd_lambda_=1, csd_tau=0.1):
+               csd_lambda_=1, csd_tau=0.1,
+               csd_fa_thr=0.7):
     """
     full path to a nifti file containing
     parameters for the CSD fit
 
     Parameters
     ----------
     csd_response : tuple or None, optional.
@@ -305,14 +314,17 @@
     csd_tau : float, optional.
         threshold controlling the amplitude below which the corresponding
         fODF is assumed to be zero.  Ideally, tau should be set to
         zero. However, to improve the stability of the algorithm, tau is
         set to tau*100 percent of the mean fODF amplitude (here, 10 percent
         by default)
         (see [1]_). Default: 0.1
+    csd_fa_thr : float, optional.
+        The threshold on the FA used to calculate the single shell auto
+        response. Can be useful to reduce for baby subjects. Default: 0.7
 
     References
     ----------
     .. [1] Tournier, J.D., et al. NeuroImage 2007. Robust determination of
             the fibre orientation distribution in diffusion MRI:
             Non-negativity constrained super-resolved spherical
             deconvolution
@@ -320,25 +332,27 @@
     mask =\
         nib.load(brain_mask).get_fdata()
     try:
         csdf = csd_fit_model(
             gtab, data,
             mask=mask,
             response=csd_response, sh_order=csd_sh_order,
-            lambda_=csd_lambda_, tau=csd_tau)
+            lambda_=csd_lambda_, tau=csd_tau,
+            csd_fa_thr=csd_fa_thr)
     except CsdNanResponseError as e:
         raise CsdNanResponseError(
             'Could not compute CSD response function for file: '
             f'{dwi}.') from e
 
     meta = dict(
         SphericalHarmonicDegree=csd_sh_order,
         ResponseFunctionTensor=csd_response,
         lambda_=csd_lambda_,
-        tau=csd_tau)
+        tau=csd_tau,
+        csd_fa_thr=csd_fa_thr)
     meta["SphericalHarmonicBasis"] = "DESCOTEAUX"
     meta["ModelURL"] = f"{DIPY_GH}reconst/csdeconv.py"
     return csdf.shm_coeff, meta
 
 
 @pimms.calc("csd_pmap")
 @as_file(suffix='_odfmodel-CSD_desc-APM_dwi.nii.gz')
@@ -439,14 +453,114 @@
     the anisotropic index from GQ
     """
     sh_coeff = nib.load(gq_params).get_fdata()
     AI = anisotropic_index(sh_coeff)
     return AI, dict(GQParamsFile=gq_params)
 
 
+@pimms.calc("rumba_model")
+def rumba_model(gtab,
+                rumba_wm_response=[0.0017, 0.0002, 0.0002],
+                rumba_gm_response=0.0008,
+                rumba_csf_response=0.003,
+                rumba_n_iter=600):
+    """
+    fit for RUMBA-SD model as documented on dipy reconstruction options
+
+    Parameters
+    ----------
+    rumba_wm_response: 1D or 2D ndarray or AxSymShResponse.
+        Able to take response[0] from auto_response_ssst.
+        default: array([0.0017, 0.0002, 0.0002])
+    rumba_gm_response: float, optional
+        Mean diffusivity for GM compartment.
+        If None, then grey matter volume fraction is not computed.
+        Default: 0.8e-3
+    rumba_csf_response: float, optional
+        Mean diffusivity for CSF compartment.
+        If None, then CSF volume fraction is not computed.
+        Default: 3.0e-3
+    rumba_n_iter: int, optional
+        Number of iterations for fODF estimation.
+        Must be a positive int.
+        Default: 600
+    """
+    return RumbaSDModel(
+        gtab,
+        wm_response=np.asarray(rumba_wm_response),
+        gm_response=rumba_gm_response,
+        csf_response=rumba_csf_response,
+        n_iter=rumba_n_iter,
+        recon_type='smf',
+        n_coils=1,
+        R=1,
+        voxelwise=False,
+        use_tv=False,
+        sphere=default_sphere,
+        verbose=True)
+
+
+@pimms.calc("rumba_params")
+@as_file(suffix='_odfmodel-RUMBA_desc-diffmodel_dwi.nii.gz')
+@as_img
+def rumba_params(rumba_model, data, brain_mask):
+    """
+    Takes the fitted RUMBA-SD model as input and returns
+    the spherical harmonics coefficients (SHM).
+    """
+    rumba_fit = rumba_model.fit(
+        data,
+        mask=nib.load(brain_mask).get_fdata())
+    odf = rumba_fit.odf(sphere=default_sphere)
+    rumba_shm, _, _ = extract_odf(odf)
+    meta = dict()
+    return rumba_shm, meta
+
+
+@pimms.calc("rumba_fit")
+def rumba_fit(rumba_model, rumba_params):
+    """RUMBA FIT"""
+    return RumbaFit(
+        rumba_model,
+        nib.load(rumba_params).get_fdata())
+
+
+@pimms.calc("rumba_f_csf")
+@as_file(suffix='_odfmodel-RUMBA_desc-CSF_probseg.nii.gz')
+@as_fit_deriv('RUMBA')
+def rumba_f_csf(rumba_fit):
+    """
+    full path to a nifti file containing
+    the CSF volume fraction for each voxel.
+    """
+    return rumba_fit.f_csf  # CSF volume fractions
+
+
+@pimms.calc("rumba_f_gm")
+@as_file(suffix='_odfmodel-RUMBA_desc-GM_probseg.nii.gz')
+@as_fit_deriv('RUMBA')
+def rumba_f_gm(rumba_fit):
+    """
+    full path to a nifti file containing
+    the GM volume fraction for each voxel.
+    """
+    return rumba_fit.f_gm  # gray matter volume fractions
+
+
+@pimms.calc("rumba_f_wm")
+@as_file(suffix='_odfmodel-RUMBA_desc-WM_probseg.nii.gz')
+@as_fit_deriv('RUMBA')
+def rumba_f_wm(rumba_fit):
+    """
+    full path to a nifti file containing
+    the white matter volume fraction for each voxel.
+    """
+    return rumba_fit.f_wm  # white matter volume fractions
+
+
 @pimms.calc("opdt_params", "opdt_gfa")
 def opdt_params(base_fname, data, gtab,
                 dwi_affine, brain_mask,
                 opdt_sh_order=8):
     """
     full path to a nifti file containing
     parameters for the Orientation Probability Density Transform
@@ -914,15 +1028,15 @@
     # is handled in get_data_plan
     # This is just the default
     return B0Image().get_image_getter("data")(b0)
 
 
 @pimms.calc("bundle_dict", "reg_template")
 def get_bundle_dict(segmentation_params,
-                    brain_mask, bids_info, b0,
+                    brain_mask, b0,
                     bundle_info=None, reg_template_spec="mni_T1"):
     """
     Dictionary defining the different bundles to be segmented,
     and a Nifti1Image containing the template for registration
 
     Parameters
     ----------
@@ -991,20 +1105,14 @@
         bundle_dict = bundle_info.copy()
     else:
         bundle_dict = abd.BundleDict(
             bundle_info,
             seg_algo=segmentation_params["seg_algo"],
             resample_to=reg_template)
 
-    if bids_info is not None:
-        bundle_dict.set_bids_info(
-            bids_info["bids_layout"],
-            b0,
-            bids_info["subject"],
-            bids_info["session"])
     return bundle_dict, reg_template
 
 
 def get_data_plan(kwargs):
     if "scalars" in kwargs and not (
         isinstance(kwargs["scalars"], list) and isinstance(
             kwargs["scalars"][0], (str, Definition))):
@@ -1020,18 +1128,20 @@
         gq, gq_pmap, gq_ai, opdt_params, opdt_pmap, opdt_ai,
         csa_params, csa_pmap, csa_ai,
         fwdti_fa, fwdti_md, fwdti_fwf,
         msdki_fit, msdki_params, msdki_msd, msdki_msk,
         dki_md, dki_awf, dki_mk, dki_kfa, dki_ga, dki_rd,
         dti_ga, dti_rd, dti_ad,
         dki_ad, dki_rk, dki_ak, dti_params, dki_params, fwdti_params,
+        rumba_fit, rumba_params, rumba_model,
+        rumba_f_csf, rumba_f_gm, rumba_f_wm,
         csd_params, get_bundle_dict])
 
     if "scalars" not in kwargs:
-        bvals, _ = read_bvals_bvecs(kwargs["bval"], kwargs["bvec"])
+        bvals, _ = read_bvals_bvecs(kwargs["bval_file"], kwargs["bvec_file"])
         if len(dpg.unique_bvals_magnitude(bvals)) > 2:
             kwargs["scalars"] = [
                 "dki_fa", "dki_md",
                 "dki_kfa", "dki_mk"]
         else:
             kwargs["scalars"] = [
                 "dti_fa", "dti_md"]
@@ -1046,19 +1156,13 @@
 
     bm_def = kwargs.get(
         "brain_mask_definition", None)
     if bm_def is not None:
         if not isinstance(bm_def, Definition):
             raise TypeError(
                 "brain_mask_definition must be a Definition")
-        if kwargs["bids_info"] is not None:
-            bm_def.find_path(
-                kwargs["bids_info"]["bids_layout"],
-                kwargs["dwi_path"],
-                kwargs["bids_info"]["subject"],
-                kwargs["bids_info"]["session"])
         data_tasks["brain_mask_res"] = pimms.calc("brain_mask")(
             as_file((
                 f'_desc-{str_to_desc(bm_def.get_name())}'
                 '_dwi.nii.gz'))(bm_def.get_image_getter("data")))
 
     return pimms.plan(**data_tasks)
```

### Comparing `pyAFQ-1.3.1/AFQ/tasks/decorators.py` & `pyafq-1.3.2/AFQ/tasks/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,28 +112,28 @@
 
 def as_file(suffix, include_track=False, include_seg=False):
     """
     return img and meta as saved file path, with json,
     and only run if not already found
     """
     def _as_file(func):
-        needed_args = ["base_fname", "results_dir"]
+        needed_args = ["base_fname", "output_dir"]
         if include_track:
             needed_args.append("tracking_params")
         if include_seg:
             needed_args.append("segmentation_params")
 
         @functools.wraps(func)
         @has_args(func, needed_args)
         def wrapper_as_file(*args, **kwargs):
-            og_arg_count, base_fname, results_dir, \
+            og_arg_count, base_fname, output_dir, \
                 tracking_params, segmentation_params =\
                 extract_added_args(
                     func,
-                    ["base_fname", "results_dir",
+                    ["base_fname", "output_dir",
                      "tracking_params", "segmentation_params"],
                     args,
                     includes=[True, True, include_track, include_seg])
             this_file = get_fname(
                 base_fname, suffix,
                 tracking_params=tracking_params,
                 segmentation_params=segmentation_params)
@@ -170,15 +170,15 @@
                 elif include_track:
                     meta["dependent"] = "trk"
                 else:
                     meta["dependent"] = "dwi"
 
                 # modify meta source to be relative
                 if "source" in meta:
-                    meta["source"] = op.relpath(meta["source"], results_dir)
+                    meta["source"] = op.relpath(meta["source"], output_dir)
 
                 meta_fname = get_fname(
                     base_fname, f"{drop_extension(suffix)}.json",
                     tracking_params=tracking_params,
                     segmentation_params=segmentation_params)
                 write_json(meta_fname, meta)
             return this_file
```

### Comparing `pyAFQ-1.3.1/AFQ/tasks/mapping.py` & `pyafq-1.3.2/AFQ/tasks/mapping.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,21 +43,21 @@
     template_xform = mapping.transform_inverse(
         data_imap["reg_template"].get_fdata())
     template_xform = nib.Nifti1Image(template_xform, data_imap["dwi_affine"])
     return template_xform, dict()
 
 
 @pimms.calc("rois")
-def export_rois(base_fname, results_dir, data_imap, mapping):
+def export_rois(base_fname, output_dir, data_imap, mapping):
     """
     dictionary of full paths to Nifti1Image files of ROIs
     transformed to subject space
     """
     bundle_dict = data_imap["bundle_dict"]
-    rois_dir = op.join(results_dir, 'ROIs')
+    rois_dir = op.join(output_dir, 'ROIs')
     os.makedirs(rois_dir, exist_ok=True)
     roi_files = {}
     base_roi_fname = op.join(rois_dir, op.split(base_fname)[1])
     for bundle_name in bundle_dict:
         roi_files[bundle_name] = []
         for roi_fname in bundle_dict.transform_rois(
                 bundle_name, mapping, data_imap["dwi_affine"],
@@ -67,15 +67,15 @@
             meta = {}
             meta_fname = f'{drop_extension(roi_fname)}.json'
             write_json(meta_fname, meta)
     return {'rois': roi_files}
 
 
 @pimms.calc("mapping")
-def mapping(base_fname, dwi_path, reg_subject, data_imap, bids_info,
+def mapping(base_fname, dwi_data_file, reg_subject, data_imap,
             mapping_definition=None):
     """
     mapping from subject to template space.
 
     Parameters
     ----------
     mapping_definition : instance of `AFQ.definitions.mapping`, optional
@@ -89,27 +89,21 @@
     reg_template = data_imap["reg_template"]
     if mapping_definition is None:
         mapping_definition = SynMap()
     if not isinstance(mapping_definition, Definition):
         raise TypeError(
             "mapping must be a mapping defined"
             + " in `AFQ.definitions.mapping`")
-    if bids_info is not None:
-        mapping_definition.find_path(
-            bids_info["bids_layout"],
-            dwi_path,
-            bids_info["subject"],
-            bids_info["session"])
     return mapping_definition.get_for_subses(
-        base_fname, data_imap["dwi"], bids_info,
+        base_fname, data_imap["dwi"], dwi_data_file,
         reg_subject, reg_template)
 
 
 @pimms.calc("mapping")
-def sls_mapping(base_fname, dwi_path, reg_subject, data_imap, bids_info,
+def sls_mapping(base_fname, dwi_data_file, reg_subject, data_imap,
                 tractography_imap, mapping_definition=None):
     """
     mapping from subject to template space.
 
     Parameters
     ----------
     mapping_definition : instance of `AFQ.definitions.mapping`, optional
@@ -123,20 +117,14 @@
     reg_template = data_imap["reg_template"]
     if mapping_definition is None:
         mapping_definition = SynMap()
     if not isinstance(mapping_definition, Definition):
         raise TypeError(
             "mapping must be a mapping defined"
             + " in `AFQ.definitions.mapping`")
-    if bids_info is not None:
-        mapping_definition.find_path(
-            bids_info["bids_layout"],
-            dwi_path,
-            bids_info["subject"],
-            bids_info["session"])
     streamlines_file = tractography_imap["streamlines"]
     tg = load_tractogram(
         streamlines_file, reg_subject,
         Space.VOX, bbox_valid_check=False)
     tg.to_rasmm()
 
     atlas_fname = op.join(
@@ -147,15 +135,16 @@
         'whole_brain_MNI.trk')
     if not op.exists(atlas_fname):
         afd.fetch_hcp_atlas_16_bundles()
     hcp_atlas = load_tractogram(
         atlas_fname,
         'same', bbox_valid_check=False)
     return mapping_definition.get_for_subses(
-        base_fname, data_imap["dwi"], bids_info,
+        base_fname, data_imap["dwi"],
+        dwi_data_file,
         reg_subject, reg_template,
         subject_sls=tg.streamlines,
         template_sls=hcp_atlas.streamlines)
 
 
 @pimms.calc("reg_subject")
 def get_reg_subject(data_imap,
@@ -201,50 +190,29 @@
 
 
 def get_mapping_plan(kwargs, use_sls=False):
     mapping_tasks = with_name([
         export_registered_b0, template_xform, export_rois, mapping,
         get_reg_subject])
 
-    bids_info = kwargs.get("bids_info", None)
     # add custom scalars
     for scalar in kwargs["scalars"]:
         if isinstance(scalar, Definition):
-            if bids_info is None:
-                scalar.find_path(
-                    None,
-                    kwargs["dwi_path"],
-                    None,
-                    None)
-                scalar_found = True
-            else:
-                scalar_found = scalar.find_path(
-                    bids_info["bids_layout"],
-                    kwargs["dwi_path"],
-                    bids_info["subject"],
-                    bids_info["session"],
-                    required=False)
-            if scalar_found != False:
-                mapping_tasks[f"{scalar.get_name()}_res"] =\
-                    pimms.calc(f"{scalar.get_name()}")(
-                        as_file((
-                            f'_desc-{str_to_desc(scalar.get_name())}'
-                            '_dwi.nii.gz'))(
-                                scalar.get_image_getter("mapping")))
+            mapping_tasks[f"{scalar.get_name()}_res"] =\
+                pimms.calc(f"{scalar.get_name()}")(
+                    as_file((
+                        f'_desc-{str_to_desc(scalar.get_name())}'
+                        '_dwi.nii.gz'))(
+                            scalar.get_image_getter("mapping")))
 
     if use_sls:
         mapping_tasks["mapping_res"] = sls_mapping
 
     reg_ss = kwargs.get("reg_subject_spec", None)
     if isinstance(reg_ss, ImageDefinition):
-        reg_ss.find_path(
-            bids_info["bids_layout"],
-            kwargs["dwi_path"],
-            bids_info["subject"],
-            bids_info["session"])
         del kwargs["reg_subject_spec"]
         mapping_tasks["reg_subject_spec_res"] = pimms.calc("reg_subject_spec")(
             as_file((
                 f'_desc-{str_to_desc(reg_ss.get_name())}'
                 '_dwi.nii.gz'))(reg_ss.get_image_getter("mapping")))
 
     return pimms.plan(**mapping_tasks)
```

### Comparing `pyAFQ-1.3.1/AFQ/tasks/segmentation.py` & `pyafq-1.3.2/AFQ/tasks/segmentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,29 +105,29 @@
     meta["Recognition Parameters"] = seg_params_out
     meta["Bundle Parameters"] = bundle_meta
     meta["Timing"] = time() - start_time
     return tgram, meta
 
 
 @pimms.calc("indiv_bundles")
-def export_bundles(base_fname, results_dir,
+def export_bundles(base_fname, output_dir,
                    bundles,
                    tracking_params,
                    segmentation_params):
     """
     dictionary of paths, where each path is
     a full path to a trk file containing the streamlines of a given bundle.
     """
     is_trx = tracking_params.get("trx", False)
     if is_trx:
         extension = ".trx"
     else:
         extension = ".trk"
 
-    bundles_dir = op.join(results_dir, "bundles")
+    bundles_dir = op.join(output_dir, "bundles")
     os.makedirs(bundles_dir, exist_ok=True)
     seg_sft = aus.SegmentedSFT.fromfile(bundles)
     for bundle in seg_sft.bundle_names:
         if bundle != "whole_brain":
             fname = op.split(
                 get_fname(
                     base_fname,
```

### Comparing `pyAFQ-1.3.1/AFQ/tasks/tractography.py` & `pyafq-1.3.2/AFQ/tasks/tractography.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 import nibabel as nib
 import numpy as np
 from time import time
 import logging
 
 import pimms
+import multiprocessing
 
 from AFQ.tasks.decorators import as_file, as_img
 from AFQ.tasks.utils import with_name
 from AFQ.definitions.utils import Definition
 import AFQ.tractography.tractography as aft
 from AFQ.tasks.utils import get_default_args
 from AFQ.definitions.image import ScalarImage
+from AFQ.tractography.utils import gen_seeds
 
 try:
+    import ray
+    has_ray = True
+except ModuleNotFoundError:
+    has_ray = False
+try:
     from trx.trx_file_memmap import TrxFile
+    from trx.trx_file_memmap import concatenate as trx_concatenate
     has_trx = True
 except ModuleNotFoundError:
     has_trx = False
 
 try:
     from AFQ.tractography.gputractography import gpu_track
     has_gputrack = True
@@ -115,97 +123,161 @@
         params_file = data_imap["dti_params"]
     elif odf_model == "CSD":
         params_file = data_imap["csd_params"]
     elif odf_model == "DKI":
         params_file = data_imap["dki_params"]
     elif odf_model == "GQ":
         params_file = data_imap["gq_params"]
+    elif odf_model == "RUMBA":
+        params_file = data_imap["rumba_params"]
     else:
         raise TypeError((
             f"The ODF model you gave ({odf_model}) was not recognized"))
 
     # get masks
     this_tracking_params['seed_mask'] = nib.load(seed).get_fdata()
     if isinstance(stop, str):
         this_tracking_params['stop_mask'] = nib.load(stop).get_fdata()
     else:
         this_tracking_params['stop_mask'] = stop
 
     is_trx = this_tracking_params.get("trx", False)
 
+    num_chunks = this_tracking_params.pop("num_chunks", False)
+
+    if num_chunks is True:
+        num_chunks = multiprocessing.cpu_count() - 1
+
     if is_trx:
         start_time = time()
         dtype_dict = {'positions': np.float16, 'offsets': np.uint32}
-        lazyt = aft.track(params_file, **this_tracking_params)
-        sft = TrxFile.from_lazy_tractogram(
-            lazyt,
-            seed,
-            dtype_dict=dtype_dict)
+        if num_chunks and num_chunks > 1:
+            if not has_ray:
+                raise ImportError("Ray is required to perform tractography in"
+                                  "parallel, please install ray or remove the"
+                                  " 'num_chunks' arg")
+
+            @ray.remote
+            class TractActor():
+                def __init__(self):
+                    self.TrxFile = TrxFile
+                    self.aft = aft
+                    self.objects = {}
+
+                def trx_from_lazy_tractogram(self, lazyt_id, seed, dtype_dict):
+                    id = self.objects[lazyt_id]
+                    return self.TrxFile.from_lazy_tractogram(
+                        id,
+                        seed,
+                        dtype_dict=dtype_dict)
+
+                def create_lazyt(self, id, *args, **kwargs):
+                    self.objects[id] = self.aft.track(*args, **kwargs)
+                    return id
+
+                def delete_lazyt(self, id):
+                    if id in self.objects:
+                        del self.objects[id]
+            actors = [TractActor.remote() for _ in range(num_chunks)]
+            object_id = 1
+            tracking_params_list = []
+
+            # random seeds case
+            if isinstance(this_tracking_params.get("n_seeds"), int) and \
+               this_tracking_params.get("random_seeds"):
+
+                remainder = this_tracking_params['n_seeds'] % num_chunks
+                for i in range(num_chunks):
+                    # create copy of tracking params
+                    copy = this_tracking_params.copy()
+                    n_seeds = this_tracking_params['n_seeds']
+                    copy['n_seeds'] = n_seeds // num_chunks
+                    # add remainder to 1st list
+                    if i == 0:
+                        copy['n_seeds'] += remainder
+                    tracking_params_list.append(copy)
+
+            elif isinstance(this_tracking_params['n_seeds'], (np.ndarray,
+                                                              list)):
+                n_seeds = np.array(this_tracking_params['n_seeds'])
+                seed_chunks = np.array_split(n_seeds, num_chunks)
+                tracking_params_list = [this_tracking_params.copy() for _ in
+                                        range(num_chunks)]
+
+                for i in range(num_chunks):
+                    tracking_params_list[i]['n_seeds'] = seed_chunks[i]
+
+            else:
+                seeds = gen_seeds(
+                    this_tracking_params['seed_mask'],
+                    this_tracking_params['seed_threshold'],
+                    this_tracking_params['n_seeds'],
+                    this_tracking_params['thresholds_as_percentages'],
+                    this_tracking_params['random_seeds'],
+                    this_tracking_params['rng_seed'],
+                    data_imap["dwi_affine"])
+                seed_chunks = np.array_split(seeds, num_chunks)
+                tracking_params_list = [this_tracking_params.copy() for _
+                                        in range(num_chunks)]
+                for i in range(num_chunks):
+                    tracking_params_list[i]['n_seeds'] = seed_chunks[i]
+
+            # create lazyt inside each actor
+            tasks = [ray_actor.create_lazyt.remote(object_id, params_file,
+                     **tracking_params_list[i]) for i, ray_actor in
+                     enumerate(actors)]
+            ray.get(tasks)
+
+            # create trx from lazyt
+            tasks = [ray_actor.trx_from_lazy_tractogram.remote(object_id, seed,
+                     dtype_dict=dtype_dict) for ray_actor in actors]
+            sfts = ray.get(tasks)
+
+            # cleanup objects
+            tasks = [ray_actor.delete_lazyt.remote(object_id) for ray_actor in
+                     actors]
+            ray.get(tasks)
+
+            sft = trx_concatenate(sfts)
+        else:
+            lazyt = aft.track(params_file, **this_tracking_params)
+            sft = TrxFile.from_lazy_tractogram(
+                lazyt,
+                seed,
+                dtype_dict=dtype_dict)
         n_streamlines = len(sft)
 
     else:
         start_time = time()
         sft = aft.track(params_file, **this_tracking_params)
         sft.to_vox()
         n_streamlines = len(sft.streamlines)
 
     return sft, _meta_from_tracking_params(
         tracking_params, start_time,
         n_streamlines, seed, stop)
 
 
 @pimms.calc("streamlines")
-def custom_tractography(bids_info, import_tract=None):
+def custom_tractography(import_tract=None):
     """
     full path to the complete, unsegmented tractography file
 
     Parameters
     ----------
     import_tract : dict or str or None, optional
         BIDS filters for inputing a user made tractography file,
         or a path to the tractography file. If None, DIPY is used
         to generate the tractography.
         Default: None
     """
-    if not isinstance(import_tract, dict) and\
-            not isinstance(import_tract, str):
+    if not isinstance(import_tract, str):
         raise TypeError(
             "import_tract must be"
             + " either a dict or a str")
-    if isinstance(import_tract, dict):
-        if bids_info is None:
-            raise ValueError((
-                "bids_info must be provided if using"
-                " bids filters to find imported tracts"))
-        import_tract = \
-            bids_info["bids_layout"].get(
-                subject=bids_info["subject"],
-                session=bids_info["session"],
-                extension=[
-                    '.trk',
-                    '.tck',
-                    '.vtk',
-                    '.fib',
-                    '.dpy'],
-                return_type='filename',
-                **import_tract)
-        if len(import_tract) < 1:
-            raise ValueError((
-                "No custom tractography found for subject "
-                f"{bids_info['subject']} and session "
-                f"{bids_info['session']}."))
-        elif len(import_tract) > 1:
-            import_tract = import_tract[0]
-            logger.warning((
-                f"Multiple viable custom tractographies found for"
-                f" subject "
-                f"{bids_info['subject']} and session "
-                f"{bids_info['session']}. Will use: {import_tract}"))
-        else:
-            import_tract = import_tract[0]
     return import_tract
 
 
 @pimms.calc("streamlines")
 @as_file('_tractography', include_track=True)
 def gpu_tractography(data_imap, tracking_params, seed, stop,
                      tractography_ngpus=0, chunk_size=100000):
@@ -308,29 +380,14 @@
         kwargs["tracking_params"]["stop_threshold"] = 0.2
         logger.info((
             "No stop mask given, using FA (or first scalar if none are FA)"
             "thresholded to 0.2"))
 
     stop_mask = kwargs["tracking_params"]['stop_mask']
     seed_mask = kwargs["tracking_params"]['seed_mask']
-    bids_info = kwargs["bids_info"]
-
-    if bids_info is not None:
-        if isinstance(stop_mask, Definition):
-            stop_mask.find_path(
-                bids_info["bids_layout"],
-                kwargs["dwi_path"],
-                bids_info["subject"],
-                bids_info["session"])
-        if isinstance(seed_mask, Definition):
-            seed_mask.find_path(
-                bids_info["bids_layout"],
-                kwargs["dwi_path"],
-                bids_info["subject"],
-                bids_info["session"])
 
     if kwargs["tracking_params"]["tracker"] == "pft":
         probseg_funcs = stop_mask.get_image_getter("tractography")
         tractography_tasks["wm_res"] = pimms.calc("pve_wm")(probseg_funcs[0])
         tractography_tasks["gm_res"] = pimms.calc("pve_gm")(probseg_funcs[1])
         tractography_tasks["csf_res"] = pimms.calc("pve_csf")(probseg_funcs[2])
         tractography_tasks["export_stop_mask_res"] = \
@@ -342,7 +399,22 @@
 
     if isinstance(seed_mask, Definition):
         tractography_tasks["export_seed_mask_res"] = pimms.calc("seed")(
             as_file('_desc-seed_mask.nii.gz', include_track=True)(
                 seed_mask.get_image_getter("tractography")))
 
     return pimms.plan(**tractography_tasks)
+
+
+def _gen_seeds(n_seeds, params_file, seed_mask=None, seed_threshold=0,
+               thresholds_as_percentages=False,
+               random_seeds=False, rng_seed=None):
+    if isinstance(params_file, str):
+        params_img = nib.load(params_file)
+    else:
+        params_img = params_file
+
+    affine = params_img.affine
+
+    return gen_seeds(seed_mask, seed_threshold, n_seeds,
+                     thresholds_as_percentages,
+                     random_seeds, rng_seed, affine)
```

### Comparing `pyAFQ-1.3.1/AFQ/tasks/utils.py` & `pyafq-1.3.2/AFQ/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/tasks/viz.py` & `pyafq-1.3.2/AFQ/tasks/viz.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         return figure
     else:
         return [figure, fname]
 
 
 @pimms.calc("indiv_bundles_figures")
 def viz_indivBundle(base_fname,
-                    results_dir,
+                    output_dir,
                     viz_backend,
                     data_imap,
                     mapping_imap,
                     segmentation_imap,
                     tracking_params,
                     segmentation_params,
                     best_scalar,
@@ -269,44 +269,44 @@
                 roi_fname,
                 name=roi_fname.split("desc-")[1].split("_")[0],
                 flip_axes=flip_axes,
                 inline=False,
                 interact=False,
                 figure=figure)
 
-        roi_dir = op.join(results_dir, 'viz_bundles')
+        roi_dir = op.join(output_dir, 'viz_bundles')
         os.makedirs(roi_dir, exist_ok=True)
         figures[bundle_name] = figure
         if "no_gif" not in viz_backend.backend:
             fname = op.split(
                 get_fname(
                     base_fname,
                     f'_desc-{str_to_desc(bundle_name)}viz'
                     f'_dwi.gif',
                     tracking_params=tracking_params,
                     segmentation_params=segmentation_params))
 
             fname = op.join(roi_dir, fname[1])
             viz_backend.create_gif(figure, fname)
         if "plotly" in viz_backend.backend:
-            roi_dir = op.join(results_dir, 'viz_bundles')
+            roi_dir = op.join(output_dir, 'viz_bundles')
             os.makedirs(roi_dir, exist_ok=True)
             fname = op.split(
                 get_fname(
                     base_fname,
                     f'_desc-{str_to_desc(bundle_name)}viz'
                     f'_dwi.html',
                     tracking_params=tracking_params,
                     segmentation_params=segmentation_params))
 
             fname = op.join(roi_dir, fname[1])
             figure.write_html(fname)
 
             # also do the core visualizations when using the plotly backend
-            core_dir = op.join(results_dir, 'viz_core_bundles')
+            core_dir = op.join(output_dir, 'viz_core_bundles')
             os.makedirs(core_dir, exist_ok=True)
             indiv_profile = profiles[
                 profiles.tractID == bundle_name][best_scalar].to_numpy()
             if len(indiv_profile) > 1:
                 fname = op.split(
                     get_fname(
                         base_fname,
```

### Comparing `pyAFQ-1.3.1/AFQ/tests/data/MoriGroups_Test.mat` & `pyafq-1.3.2/AFQ/tests/data/MoriGroups_Test.mat`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/tests/data/WholeBrainFG_test.mat` & `pyafq-1.3.2/AFQ/tests/data/WholeBrainFG_test.mat`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/tests/data/mocks3/ds000102-mimic/task-flanker_bold.json` & `pyafq-1.3.2/AFQ/tests/data/mocks3/ds000102-mimic/task-flanker_bold.json`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/tests/test_api.py` & `pyafq-1.3.2/AFQ/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import tempfile
 import os
 import os.path as op
 import shutil
 import subprocess
 import gc
 import random
+import concurrent.futures
 
 import toml
 
 import numpy as np
 import numpy.testing as npt
 import pytest
 
@@ -21,15 +22,15 @@
 import dipy.tracking.utils as dtu
 import dipy.tracking.streamline as dts
 from dipy.data import get_fnames
 from dipy.testing.decorators import xvfb_it
 from dipy.io.streamline import load_tractogram
 
 import AFQ.api.bundle_dict as abd
-from AFQ.api.group import GroupAFQ
+from AFQ.api.group import GroupAFQ, ParallelGroupAFQ
 from AFQ.api.participant import ParticipantAFQ
 import AFQ.data.fetch as afd
 import AFQ.utils.streamlines as aus
 import AFQ.utils.bin as afb
 from AFQ.definitions.mapping import SynMap, AffMap, SlrMap, IdentityMap
 from AFQ.definitions.image import (RoiImage, PFTImage, ImageFile,
                                    TemplateImage, LabelledImageFile)
@@ -416,15 +417,15 @@
     bvals_in_range_or_0 = \
         np.logical_or(bvals_in_range, gtab.b0s_mask)
     npt.assert_equal(bvals_in_range_or_0, np.ones(160, dtype=bool))
 
     # check that the apm map was made
     myafq.export("mapping")
     assert op.exists(op.join(
-        myafq.export("results_dir")["01"],
+        myafq.export("output_dir")["01"],
         'sub-01_ses-01_odfmodel-CSD_desc-APM_dwi.nii.gz'))
 
 
 def test_API_type_checking():
     _, bids_path, _ = get_temp_hardi()
     seed = 2022
     np.random.seed(seed)
@@ -593,14 +594,20 @@
             'rng': 42})
 
     seg_sft = aus.SegmentedSFT.fromfile(
         myafq.export("bundles")["01"])
     npt.assert_(len(seg_sft.get_bundle('CCMid').streamlines) > 0)
 
 
+def test_AFQ_pydra():
+    _, bids_path = afd.fetch_hbn_preproc(["NDARAA948VFH", "NDARAV554TP2"])
+    pga = ParallelGroupAFQ(bids_path, preproc_pipeline="qsiprep")
+    pga.export("dti_fa")
+
+
 @pytest.mark.nightly_pft
 def test_AFQ_pft():
     """
     Test pft interface for AFQ
     """
     _, bids_path, sub_path = get_temp_hardi()
 
@@ -834,70 +841,70 @@
     dwi_affine = myafq.export("dwi_affine")
     streamlines = dts.Streamlines(
         dtu.transform_tracking_output(
             [s for s in streamlines if s.shape[0] > 100],
             np.linalg.inv(dwi_affine)))
 
     mapping_file = op.join(
-        myafq.export("results_dir"),
+        myafq.export("output_dir"),
         'sub-01_ses-01_desc-mapping_from-DWI_to-MNI_xform.nii.gz')
     nib.save(mapping, mapping_file)
     reg_prealign_file = op.join(
-        myafq.export("results_dir"),
+        myafq.export("output_dir"),
         'sub-01_ses-01_desc-prealign_from-DWI_to-MNI_xform.npy')
     np.save(reg_prealign_file, np.eye(4))
 
     # Test ROI exporting:
     myafq.export("rois")
     assert op.exists(op.join(
-        myafq.export("results_dir"),
+        myafq.export("output_dir"),
         'ROIs',
         'sub-01_ses-01_space-subject_desc-RightCorticospinalinclude1_mask.json'))  # noqa
 
     seg_sft = aus.SegmentedSFT.fromfile(
         myafq.export("bundles"))
     npt.assert_(len(seg_sft.get_bundle(
         'Left Corticospinal').streamlines) > 0)
 
     # Test bundles exporting:
     myafq.export("indiv_bundles")
     assert op.exists(op.join(
-        myafq.export("results_dir"),
+        myafq.export("output_dir"),
         'bundles',
         'sub-01_ses-01_coordsys-RASMM_trkmethod-probCSD_recogmethod-AFQ_desc-LeftCorticospinal_tractography.trk'))  # noqa
 
     tract_profile_fname = myafq.export("profiles")
     tract_profiles = pd.read_csv(tract_profile_fname)
 
     assert tract_profiles.select_dtypes(include=[np.number]).sum().sum() != 0
     assert tract_profiles.shape[0] >= 200
     assert tract_profiles.shape[1] == 9
 
     myafq.export("indiv_bundles_figures")
     assert op.exists(op.join(
-        myafq.export("results_dir"),
+        myafq.export("output_dir"),
         "viz_bundles",
         'sub-01_ses-01_coordsys-RASMM_trkmethod-probCSD_recogmethod-AFQ_desc-LeftSuperiorLongitudinalviz_dwi.html'))  # noqa
 
     assert op.exists(op.join(
-        myafq.export("results_dir"),
+        myafq.export("output_dir"),
         "viz_bundles",
         'sub-01_ses-01_coordsys-RASMM_trkmethod-probCSD_recogmethod-AFQ_desc-LeftSuperiorLongitudinalviz_dwi.html'))  # noqa
 
     # Before we run the CLI, we'll remove the bundles and ROI folders, to see
     # that the CLI generates them
-    shutil.rmtree(op.join(myafq.export("results_dir"),
+    shutil.rmtree(op.join(myafq.export("output_dir"),
                           'bundles'))
 
-    shutil.rmtree(op.join(myafq.export("results_dir"),
+    shutil.rmtree(op.join(myafq.export("output_dir"),
                           'ROIs'))
     os.remove(tract_profile_fname)
 
     # save memory
-    results_dir = myafq.export("results_dir")
+    output_dir = myafq.export("output_dir")
     del myafq
     gc.collect()
 
     # Test the CLI:
     print("Running the CLI:")
 
     # Set up config to use the same parameters as above:
@@ -953,15 +960,15 @@
 
     assert from_file.shape[0] >= 200
     assert from_file.shape[1] == 9
     assert_series_equal(tract_profiles['dti_fa'], from_file['dti_fa'])
 
     # Make sure the CLI did indeed generate these:
     assert op.exists(op.join(
-        results_dir,
+        output_dir,
         'ROIs',
         'sub-01_ses-01_space-subject_desc-RightSuperiorLongitudinalinclude1_mask.json'))  # noqa
 
     assert op.exists(op.join(
-        results_dir,
+        output_dir,
         'bundles',
         'sub-01_ses-01_coordsys-RASMM_trkmethod-probCSD_recogmethod-AFQ_desc-RightSuperiorLongitudinal_tractography.trk'))  # noqa
```

### Comparing `pyAFQ-1.3.1/AFQ/tests/test_bundle_dict.py` & `pyafq-1.3.2/AFQ/tests/test_bundle_dict.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/tests/test_csd.py` & `pyafq-1.3.2/AFQ/tests/test_csd.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/tests/test_definitions.py` & `pyafq-1.3.2/AFQ/tests/test_definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         subject=subject, session=session, return_type="filename",
         suffix="dwi", extension="nii.gz"
     )[0]
 
     image_file = ImageFile(suffix="seg", filters={'scope': 'synthetic'})
     image_file.find_path(bids_layout, test_dwi_path, subject, session)
 
-    assert image_file.fnames[session][subject] == op.join(
+    assert image_file.fnames[test_dwi_path] == op.join(
         bids_dir, "derivatives", "dmriprep", "sub-" + subject,
         "ses-" + session, "anat", "seg.nii.gz"
     )
 
     other_sub = "01" if subject == "02" else "02"
     with pytest.raises(ValueError):
         image_file.find_path(
```

### Comparing `pyAFQ-1.3.1/AFQ/tests/test_dki.py` & `pyafq-1.3.2/AFQ/tests/test_dki.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/tests/test_dti.py` & `pyafq-1.3.2/AFQ/tests/test_dti.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/tests/test_fixes.py` & `pyafq-1.3.2/AFQ/tests/test_fixes.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/tests/test_registration.py` & `pyafq-1.3.2/AFQ/tests/test_registration.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/tests/test_segmentation.py` & `pyafq-1.3.2/AFQ/tests/test_segmentation.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/tests/test_tractography.py` & `pyafq-1.3.2/AFQ/tests/test_tractography.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/tractography/gputractography.py` & `pyafq-1.3.2/AFQ/tractography/gputractography.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/tractography/tractography.py` & `pyafq-1.3.2/AFQ/tractography/tractography.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,30 +146,32 @@
         raise ValueError(f"Unrecognized direction '{directions}'.")
 
     if odf_model == "DTI" or odf_model == "DKI":
         evals = model_params[..., :3]
         evecs = model_params[..., 3:12].reshape(params_img.shape[:3] + (3, 3))
         odf = tensor_odf(evals, evecs, sphere)
         dg = dg.from_pmf(odf, max_angle=max_angle, sphere=sphere)
-    elif odf_model == "CSD" or odf_model == "GQ":
+    else:
         dg = dg.from_shcoeff(model_params, max_angle=max_angle, sphere=sphere)
 
     if tracker == "local":
         if stop_mask is None:
             stop_mask = np.ones(params_img.shape[:3])
 
         if len(np.unique(stop_mask)) <= 2:
             stopping_criterion = ThresholdStoppingCriterion(stop_mask,
                                                             0.5)
         else:
             if thresholds_as_percentages:
                 stop_threshold = get_percentile_threshold(
                     stop_mask, stop_threshold)
-            stopping_criterion = ThresholdStoppingCriterion(stop_mask,
-                                                            stop_threshold)
+            stop_mask_copy = np.copy(stop_mask)
+            stop_thresh_copy = np.copy(stop_threshold)
+            stopping_criterion = ThresholdStoppingCriterion(stop_mask_copy,
+                                                            stop_thresh_copy)
 
         my_tracker = LocalTracking
 
     elif tracker == "pft":
         if not isinstance(stop_threshold, str):
             raise RuntimeError(
                 "You are using PFT tracking, but did not provide a string ",
```

### Comparing `pyAFQ-1.3.1/AFQ/tractography/utils.py` & `pyafq-1.3.2/AFQ/tractography/utils.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/utils/bin.py` & `pyafq-1.3.2/AFQ/utils/bin.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/utils/docs.py` & `pyafq-1.3.2/AFQ/utils/docs.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/utils/models.py` & `pyafq-1.3.2/AFQ/utils/models.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/utils/path.py` & `pyafq-1.3.2/AFQ/utils/path.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/utils/stats.py` & `pyafq-1.3.2/AFQ/utils/stats.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/utils/streamlines.py` & `pyafq-1.3.2/AFQ/utils/streamlines.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/utils/testing.py` & `pyafq-1.3.2/AFQ/utils/testing.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/utils/tests/test_conversions.py` & `pyafq-1.3.2/AFQ/utils/tests/test_conversions.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/utils/tests/test_streamlines.py` & `pyafq-1.3.2/AFQ/utils/tests/test_streamlines.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/utils/tests/test_volume.py` & `pyafq-1.3.2/AFQ/utils/tests/test_volume.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/utils/volume.py` & `pyafq-1.3.2/AFQ/utils/volume.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/viz/altair.py` & `pyafq-1.3.2/AFQ/viz/altair.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/viz/fury_backend.py` & `pyafq-1.3.2/AFQ/viz/fury_backend.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/viz/plot.py` & `pyafq-1.3.2/AFQ/viz/plot.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/viz/plotly_backend.py` & `pyafq-1.3.2/AFQ/viz/plotly_backend.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/AFQ/viz/utils.py` & `pyafq-1.3.2/AFQ/viz/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,15 +183,15 @@
             bbox=dict(
                 facecolor='none',
                 edgecolor='none'))
         self.panel_label_kwargs.update(panel_label_kwargs)
 
     def add_img(self, fname, x_coord, y_coord, reduct_count=1,
                 subplot_label_pos=(0.1, 1.0), legend=None, legend_kwargs={},
-                add_panel_label=True):
+                add_panel_label=True, panel_label_kwargs={}):
         """
         Add image from fname into figure as a panel.
 
         Parameters
         ----------
         fname : str
             path to image file to add to subplot
@@ -210,14 +210,17 @@
             and values are colors
             Default: None
         legend_kwargs : dict
             ADditional arguments for matplotlib's legend method
         add_panel_label : bool
             Whether or not to add a panel label to the subplot
             Default: True
+        panel_label_kwargs : dict
+            Additional arguments for matplotlib's text method,
+            which is used to add panel labels to each subplot.
         """
         ax = self.fig.add_subplot(self.grid[y_coord, x_coord])
         im1 = Image.open(fname)
         for _ in range(reduct_count):
             im1 = trim(im1)
         if legend is not None:
             patches = []
@@ -225,19 +228,21 @@
                 patches.append(mpatches.Patch(
                     color=color,
                     label=value))
             ax.legend(handles=patches, borderaxespad=0., **legend_kwargs)
         if add_panel_label:
             trans = mtransforms.ScaledTranslation(
                 10 / 72, -5 / 72, self.fig.dpi_scale_trans)
+            this_pl_kwargs = self.panel_label_kwargs.copy()
+            this_pl_kwargs.update(panel_label_kwargs)
             ax.text(
                 subplot_label_pos[0], subplot_label_pos[1],
                 f"{chr(65+self.subplot_count)}",
                 transform=ax.transAxes + trans,
-                **self.panel_label_kwargs)
+                **this_pl_kwargs)
         ax.imshow(np.asarray(im1), aspect=1)
         ax.axis('off')
         self.subplot_count = self.subplot_count + 1
         return ax
 
     def format_and_save_figure(self, fname, trim_final=True):
         """
```

### Comparing `pyAFQ-1.3.1/CHANGES.rst` & `pyafq-1.3.2/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+1.3.2 (May 31, 2024)
+====================
+This release adds the ability to do tractography in parallel using ray.
+It also adds Pydra integration into GroupAFQ (ParallelGroupAFQ).
+We also added RUMBA-SD from DIPY and made other minor changes.
+  * Streamlines task in parallel using ray (#1136)
+  * Check bvals on dki (#1139)
+  * [FIX] different CST ROI 2 for L/R (#1138)
+  * Adds ParallelGroupAFQ (#1124)
+  * [DOC] Update kwargs.rst (#1135)
+  * [ENH] Added RUMBA-SD to data.py (#1129)
+  * [DOC] Update baby_afq.py (#1131)
+  * Add conversion dictionary for old acronyms (#1107)
+  * [ENH] small change to viz utils panel code (#1123)
+  * Make altair required (#1130)
+  * [DOC] Some improvements to the documentation based on conversations during the hackathon (#1126)
+  * [ENH] expose FA thresh param for autoresponse ssst for csd (#1127)
+
 1.3.1 (April 04, 2024)
 ======================
 Adds the mean signal diffusion kurtosis model as an option.
 Adds more information in JSON sidecars. Adds an explanation
 of our current bundle orientation system to the documentation.
   * [ENH] add mean signal diffusion kurtosis model (#1121)
   * [ENH] make source field relative in json sidecars (#1118)
```

### Comparing `pyAFQ-1.3.1/LICENSE` & `pyafq-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/PKG-INFO` & `pyafq-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyAFQ
-Version: 1.3.1
+Version: 1.3.2
 Summary: pyAFQ: Automated Fiber Quantification ... in Python
 Home-page: https://yeatmanlab.github.io/pyAFQ
 Download-URL: https://github.com/yeatmanlab/pyAFQ
 Author: pyAFQ developers
 Author-email: arokem@gmail.com
 Maintainer: Ariel Rokem
 Maintainer-email: arokem@gmail.com
@@ -22,14 +22,15 @@
 License-File: LICENSE
 Requires-Dist: scikit_image>=0.14.2
 Requires-Dist: dipy<1.9.0,>=1.8.0
 Requires-Dist: pandas
 Requires-Dist: pybids>=0.16.2
 Requires-Dist: templateflow>=0.8
 Requires-Dist: pimms
+Requires-Dist: pydra
 Requires-Dist: joblib>=1.3.2
 Requires-Dist: dask>=1.1
 Requires-Dist: s3bids>=0.1.7
 Requires-Dist: boto3>=1.14.0
 Requires-Dist: s3fs~=0.4.2
 Requires-Dist: toml>=0.10.0
 Requires-Dist: setuptools_scm[toml]<5.1.0,>=3.4.0
@@ -37,14 +38,15 @@
 Requires-Dist: popylar==0.2.*
 Requires-Dist: plotly==5.3.0
 Requires-Dist: kaleido==0.2.1
 Requires-Dist: imageio>=2.0.0
 Requires-Dist: Pillow
 Requires-Dist: matplotlib
 Requires-Dist: numpy==1.23.5
+Requires-Dist: altair
 Provides-Extra: dev
 Requires-Dist: docutils==0.15.2; extra == "dev"
 Requires-Dist: astroid<=2.15.8; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: memory-profiler; extra == "dev"
 Requires-Dist: pytest==7.2.0; extra == "dev"
 Requires-Dist: pytest-cov==2.10.0; extra == "dev"
@@ -69,17 +71,17 @@
 Requires-Dist: fslpy; extra == "fsl"
 Provides-Extra: afqbrowser
 Requires-Dist: AFQ-Browser>=0.3; extra == "afqbrowser"
 Provides-Extra: plot
 Requires-Dist: pingouin>=0.3; extra == "plot"
 Requires-Dist: seaborn>=0.11.0; extra == "plot"
 Requires-Dist: ipython<=7.20.0,>=7.13.0; extra == "plot"
-Requires-Dist: altair; extra == "plot"
 Provides-Extra: trx
 Requires-Dist: trx-python; extra == "trx"
+Requires-Dist: ray; extra == "trx"
 Provides-Extra: all
 Requires-Dist: docutils==0.15.2; extra == "all"
 Requires-Dist: astroid<=2.15.8; extra == "all"
 Requires-Dist: sphinx; extra == "all"
 Requires-Dist: memory-profiler; extra == "all"
 Requires-Dist: pytest==7.2.0; extra == "all"
 Requires-Dist: pytest-cov==2.10.0; extra == "all"
@@ -100,16 +102,16 @@
 Requires-Dist: xvfbwrapper==0.2.9; extra == "all"
 Requires-Dist: ipython<=7.20.0,>=7.13.0; extra == "all"
 Requires-Dist: fslpy; extra == "all"
 Requires-Dist: AFQ-Browser>=0.3; extra == "all"
 Requires-Dist: pingouin>=0.3; extra == "all"
 Requires-Dist: seaborn>=0.11.0; extra == "all"
 Requires-Dist: ipython<=7.20.0,>=7.13.0; extra == "all"
-Requires-Dist: altair; extra == "all"
 Requires-Dist: trx-python; extra == "all"
+Requires-Dist: ray; extra == "all"
 
 # pyAFQ
 Automated Fiber Quantification ... in Python.
 
 For details, see [Documentation](https://yeatmanlab.github.io/pyAFQ)
 
 For further analysis of results, see [AFQ-Insight](https://github.com/richford/AFQ-Insight)
```

### Comparing `pyAFQ-1.3.1/README.md` & `pyafq-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/bin/pyAFQ` & `pyafq-1.3.2/bin/pyAFQ`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/Makefile` & `pyafq-1.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/_progressbars.py` & `pyafq-1.3.2/docs/source/_progressbars.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/_static/BDE_Banner_revised20160211-01.jpg` & `pyafq-1.3.2/docs/source/_static/BDE_Banner_revised20160211-01.jpg`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/_static/custom.css` & `pyafq-1.3.2/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/_static/eScience_Logo_HR.png` & `pyafq-1.3.2/docs/source/_static/eScience_Logo_HR.png`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/_static/escience-logo.png` & `pyafq-1.3.2/docs/source/_static/escience-logo.png`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/_static/logo.png` & `pyafq-1.3.2/docs/source/_static/logo.png`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/conf.py` & `pyafq-1.3.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/explanations/_static/down_left_arrow.png` & `pyafq-1.3.2/docs/source/explanations/_static/down_left_arrow.png`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/explanations/_static/down_right_arrow.png` & `pyafq-1.3.2/docs/source/explanations/_static/down_right_arrow.png`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/explanations/_static/greencheck.png` & `pyafq-1.3.2/docs/source/explanations/_static/greencheck.png`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/explanations/_static/tract_modeling2.png` & `pyafq-1.3.2/docs/source/explanations/_static/tract_modeling2.png`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/explanations/_static/tract_profiling.png` & `pyafq-1.3.2/docs/source/explanations/_static/tract_profiling.png`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/explanations/_static/tract_recognition.png` & `pyafq-1.3.2/docs/source/explanations/_static/tract_recognition.png`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/explanations/_static/tract_tractography.png` & `pyafq-1.3.2/docs/source/explanations/_static/tract_tractography.png`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/explanations/bundle_orientation.rst` & `pyafq-1.3.2/docs/source/explanations/bundle_orientation.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/explanations/index.rst` & `pyafq-1.3.2/docs/source/explanations/index.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/explanations/modeling.rst` & `pyafq-1.3.2/docs/source/explanations/modeling.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/explanations/profiling.rst` & `pyafq-1.3.2/docs/source/explanations/profiling.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/explanations/recognition.rst` & `pyafq-1.3.2/docs/source/explanations/recognition.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/explanations/tractography.rst` & `pyafq-1.3.2/docs/source/explanations/tractography.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/explanations/tractometry_pipeline.rst` & `pyafq-1.3.2/docs/source/explanations/tractometry_pipeline.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/howto/cite.rst` & `pyafq-1.3.2/docs/source/howto/cite.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/howto/contributing.rst` & `pyafq-1.3.2/docs/source/howto/contributing.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/howto/developing/definitions.rst` & `pyafq-1.3.2/docs/source/howto/developing/definitions.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/howto/developing/index.rst` & `pyafq-1.3.2/docs/source/howto/developing/index.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/howto/developing/releasing.rst` & `pyafq-1.3.2/docs/source/howto/developing/releasing.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/howto/developing/tasks.rst` & `pyafq-1.3.2/docs/source/howto/developing/tasks.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/howto/getting_help.rst` & `pyafq-1.3.2/docs/source/howto/getting_help.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/howto/installation_guide.rst` & `pyafq-1.3.2/docs/source/howto/installation_guide.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/howto/usage/converter.rst` & `pyafq-1.3.2/docs/source/howto/usage/converter.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/howto/usage/data.rst` & `pyafq-1.3.2/docs/source/howto/usage/data.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/howto/usage/docker.rst` & `pyafq-1.3.2/docs/source/howto/usage/docker.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/howto/usage/image.rst` & `pyafq-1.3.2/docs/source/howto/usage/image.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/howto/usage/kwargs.rst` & `pyafq-1.3.2/docs/source/howto/usage/kwargs.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/howto/usage/methods.rst` & `pyafq-1.3.2/docs/source/howto/usage/methods.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/howto/usage/scalars.rst` & `pyafq-1.3.2/docs/source/howto/usage/scalars.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/index.rst` & `pyafq-1.3.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/reference/kwargs.rst` & `pyafq-1.3.2/docs/source/reference/kwargs.rst`

 * *Files 4% similar despite different names*

```diff
@@ -173,19 +173,25 @@
 	The parameters for tracking. Default: use the default behavior of
 	the aft.track function. Seed mask and seed threshold, if not
 	specified, are replaced with scalar masks from scalar[0]
 	thresholded to 0.2. The ``seed_mask`` and ``stop_mask`` items of
 	this dict may be ``AFQ.definitions.image.ImageFile`` instances.
 	If ``tracker`` is set to "pft" then ``stop_mask`` should be
 	an instance of ``AFQ.definitions.image.PFTImage``.
+	num_chunks can be specified to cause tracking to be done in
+	parallel using ray. If set to True it will use the number of
+	cores available on the machine - 1.
 
 import_tract: dict or str or None, optional
 	BIDS filters for inputing a user made tractography file,
 	or a path to the tractography file. If None, DIPY is used
-	to generate the tractography.
+	to generate the tractography. Note that if you are importing 
+	tractography, you do not need to specify tracking_params as pyAFQ
+	will just load the provided tractogram rather than perform
+	tractography again.
 	Default: None
 
 tractography_ngpus: int, optional
 	Number of GPUs to use in tractography. If non-0,
 	this algorithm is used for tractography,
 	https://github.com/dipy/GPUStreamlines
 	Default: 0
```

### Comparing `pyAFQ-1.3.1/docs/source/reference/mapping.rst` & `pyafq-1.3.2/docs/source/reference/mapping.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/reference/methods.rst` & `pyafq-1.3.2/docs/source/reference/methods.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/reference/viz_backend.rst` & `pyafq-1.3.2/docs/source/reference/viz_backend.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/sphinxext/kwargsdocs.py` & `pyafq-1.3.2/docs/source/sphinxext/kwargsdocs.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/sphinxext/methodsdocs.py` & `pyafq-1.3.2/docs/source/sphinxext/methodsdocs.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/sphinxext/updatedocs.py` & `pyafq-1.3.2/docs/source/sphinxext/updatedocs.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/source/tutorials/index.rst` & `pyafq-1.3.2/docs/source/tutorials/index.rst`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/docs/upload-gh-pages.sh` & `pyafq-1.3.2/docs/upload-gh-pages.sh`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/examples/howto_examples/add_custom_bundle.py` & `pyafq-1.3.2/examples/howto_examples/add_custom_bundle.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/examples/howto_examples/baby_afq.py` & `pyafq-1.3.2/examples/howto_examples/baby_afq.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,18 @@
 # `sub-01_ses-01_dwi_space-RASMM_model-probCSD_algo-AFQ_desc-viz_dwi.html`
 # in your browser. This is a visualization of the tractography and segmentation
 # results for all of the bundles. You can navigate this visualization by
 # clicking on the different bundles in the legend on the right side of the
 # screen. You can also zoom in and out using the mouse wheel, and rotate the
 # view by clicking and dragging with the mouse. You can also view the FA tract
 # profiles in a plot on the left side of the page.
+#
+# If the baby bundles appear dark in the html visualization due to low FA values, you
+# can reduce the upper limit of the range in the `sbv_lims_bundles` option when 
+# building your GroupAFQ object (e.g. `GroupAFQ(..., sbv_lims_bundles=[0, 0.5])`).
 
 
 ##########################################################################
 # References:
 # -------------------------
 # .. [Grotheer2021] Grotheer, Mareike, Mona Rosenke, Hua Wu, Holly Kular,
 #                   Francesca R. Querdasi, Vaidehi S. Natu, Jason D. Yeatman,
```

### Comparing `pyAFQ-1.3.1/examples/howto_examples/cerebellar_peduncles.py` & `pyafq-1.3.2/examples/howto_examples/cerebellar_peduncles.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/examples/howto_examples/cloudknot_example.py` & `pyafq-1.3.2/examples/howto_examples/cloudknot_example.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/examples/howto_examples/cloudknot_hcp_example.py` & `pyafq-1.3.2/examples/howto_examples/cloudknot_hcp_example.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/examples/howto_examples/plot_acoustic_radiations.py` & `pyafq-1.3.2/examples/howto_examples/plot_acoustic_radiations.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/examples/howto_examples/plot_afq_callosal.py` & `pyafq-1.3.2/examples/howto_examples/plot_afq_callosal.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/examples/howto_examples/plot_afq_fwdti.py` & `pyafq-1.3.2/examples/howto_examples/plot_afq_fwdti.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/examples/howto_examples/plot_optic_radiations.py` & `pyafq-1.3.2/examples/howto_examples/plot_optic_radiations.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/examples/howto_examples/plot_recobundles.py` & `pyafq-1.3.2/examples/howto_examples/plot_recobundles.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/examples/howto_examples/plot_stages_of_tractometry.py` & `pyafq-1.3.2/examples/howto_examples/plot_stages_of_tractometry.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/examples/howto_examples/use_subject_space_rois_from_freesurfer.py` & `pyafq-1.3.2/examples/howto_examples/use_subject_space_rois_from_freesurfer.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/examples/howto_examples/vof_example.py` & `pyafq-1.3.2/examples/howto_examples/vof_example.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/examples/tutorial_examples/plot_001_afq_api.py` & `pyafq-1.3.2/examples/tutorial_examples/plot_001_afq_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,22 +51,25 @@
 afd.organize_stanford_data(clear_previous_afq="track")
 
 ##########################################################################
 # Set tractography parameters (optional)
 # ---------------------------------------
 # We make create a `tracking_params` variable, which we will pass to the
 # GroupAFQ object which specifies that we want 25,000 seeds randomly
-# distributed in the white matter.
-#
-# We only do this to make this example faster and consume less space.
+# distributed in the white matter. We only do this to make this example 
+# faster and consume less space. We also set ``num_chunks`` to `True`,
+# which will use ray to parallelize the tracking across all cores.
+# This can be removed to process in serial, or set to use a particular
+# distribution of work by setting `n_chunks` to an integer number.
 
 tracking_params = dict(n_seeds=25000,
                        random_seeds=True,
                        rng_seed=2022,
-                       trx=True)
+                       trx=True,
+                       num_chunks=True)
 
 ##########################################################################
 # Initialize a GroupAFQ object:
 # -------------------------
 #
 # Creates a GroupAFQ object, that encapsulates tractometry. This object can be
 # used to manage the entire :doc:`AFQ pipeline`, including:
```

### Comparing `pyAFQ-1.3.1/examples/tutorial_examples/plot_002_bids_layout.py` & `pyafq-1.3.2/examples/tutorial_examples/plot_002_bids_layout.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/examples/tutorial_examples/plot_003_viz.py` & `pyafq-1.3.2/examples/tutorial_examples/plot_003_viz.py`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/gpu_docker/Dockerfile` & `pyafq-1.3.2/gpu_docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/gpu_docker/cuda_track_template.def` & `pyafq-1.3.2/gpu_docker/cuda_track_template.def`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/pyAFQ.egg-info/PKG-INFO` & `pyafq-1.3.2/pyAFQ.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyAFQ
-Version: 1.3.1
+Version: 1.3.2
 Summary: pyAFQ: Automated Fiber Quantification ... in Python
 Home-page: https://yeatmanlab.github.io/pyAFQ
 Download-URL: https://github.com/yeatmanlab/pyAFQ
 Author: pyAFQ developers
 Author-email: arokem@gmail.com
 Maintainer: Ariel Rokem
 Maintainer-email: arokem@gmail.com
@@ -22,14 +22,15 @@
 License-File: LICENSE
 Requires-Dist: scikit_image>=0.14.2
 Requires-Dist: dipy<1.9.0,>=1.8.0
 Requires-Dist: pandas
 Requires-Dist: pybids>=0.16.2
 Requires-Dist: templateflow>=0.8
 Requires-Dist: pimms
+Requires-Dist: pydra
 Requires-Dist: joblib>=1.3.2
 Requires-Dist: dask>=1.1
 Requires-Dist: s3bids>=0.1.7
 Requires-Dist: boto3>=1.14.0
 Requires-Dist: s3fs~=0.4.2
 Requires-Dist: toml>=0.10.0
 Requires-Dist: setuptools_scm[toml]<5.1.0,>=3.4.0
@@ -37,14 +38,15 @@
 Requires-Dist: popylar==0.2.*
 Requires-Dist: plotly==5.3.0
 Requires-Dist: kaleido==0.2.1
 Requires-Dist: imageio>=2.0.0
 Requires-Dist: Pillow
 Requires-Dist: matplotlib
 Requires-Dist: numpy==1.23.5
+Requires-Dist: altair
 Provides-Extra: dev
 Requires-Dist: docutils==0.15.2; extra == "dev"
 Requires-Dist: astroid<=2.15.8; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: memory-profiler; extra == "dev"
 Requires-Dist: pytest==7.2.0; extra == "dev"
 Requires-Dist: pytest-cov==2.10.0; extra == "dev"
@@ -69,17 +71,17 @@
 Requires-Dist: fslpy; extra == "fsl"
 Provides-Extra: afqbrowser
 Requires-Dist: AFQ-Browser>=0.3; extra == "afqbrowser"
 Provides-Extra: plot
 Requires-Dist: pingouin>=0.3; extra == "plot"
 Requires-Dist: seaborn>=0.11.0; extra == "plot"
 Requires-Dist: ipython<=7.20.0,>=7.13.0; extra == "plot"
-Requires-Dist: altair; extra == "plot"
 Provides-Extra: trx
 Requires-Dist: trx-python; extra == "trx"
+Requires-Dist: ray; extra == "trx"
 Provides-Extra: all
 Requires-Dist: docutils==0.15.2; extra == "all"
 Requires-Dist: astroid<=2.15.8; extra == "all"
 Requires-Dist: sphinx; extra == "all"
 Requires-Dist: memory-profiler; extra == "all"
 Requires-Dist: pytest==7.2.0; extra == "all"
 Requires-Dist: pytest-cov==2.10.0; extra == "all"
@@ -100,16 +102,16 @@
 Requires-Dist: xvfbwrapper==0.2.9; extra == "all"
 Requires-Dist: ipython<=7.20.0,>=7.13.0; extra == "all"
 Requires-Dist: fslpy; extra == "all"
 Requires-Dist: AFQ-Browser>=0.3; extra == "all"
 Requires-Dist: pingouin>=0.3; extra == "all"
 Requires-Dist: seaborn>=0.11.0; extra == "all"
 Requires-Dist: ipython<=7.20.0,>=7.13.0; extra == "all"
-Requires-Dist: altair; extra == "all"
 Requires-Dist: trx-python; extra == "all"
+Requires-Dist: ray; extra == "all"
 
 # pyAFQ
 Automated Fiber Quantification ... in Python.
 
 For details, see [Documentation](https://yeatmanlab.github.io/pyAFQ)
 
 For further analysis of results, see [AFQ-Insight](https://github.com/richford/AFQ-Insight)
```

### Comparing `pyAFQ-1.3.1/pyAFQ.egg-info/SOURCES.txt` & `pyafq-1.3.2/pyAFQ.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyAFQ-1.3.1/pyAFQ.egg-info/requires.txt` & `pyafq-1.3.2/pyAFQ.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 scikit_image>=0.14.2
 dipy<1.9.0,>=1.8.0
 pandas
 pybids>=0.16.2
 templateflow>=0.8
 pimms
+pydra
 joblib>=1.3.2
 dask>=1.1
 s3bids>=0.1.7
 boto3>=1.14.0
 s3fs~=0.4.2
 toml>=0.10.0
 setuptools_scm[toml]<5.1.0,>=3.4.0
@@ -15,14 +16,15 @@
 popylar==0.2.*
 plotly==5.3.0
 kaleido==0.2.1
 imageio>=2.0.0
 Pillow
 matplotlib
 numpy==1.23.5
+altair
 
 [afqbrowser]
 AFQ-Browser>=0.3
 
 [all]
 docutils==0.15.2
 astroid<=2.15.8
@@ -45,16 +47,16 @@
 wget
 fury==0.9.0
 ipython<=7.20.0,>=7.13.0
 fslpy
 AFQ-Browser>=0.3
 pingouin>=0.3
 seaborn>=0.11.0
-altair
 trx-python
+ray
 
 [dev]
 docutils==0.15.2
 astroid<=2.15.8
 sphinx
 memory-profiler
 pytest==7.2.0
@@ -81,11 +83,11 @@
 xvfbwrapper==0.2.9
 ipython<=7.20.0,>=7.13.0
 
 [plot]
 pingouin>=0.3
 seaborn>=0.11.0
 ipython<=7.20.0,>=7.13.0
-altair
 
 [trx]
 trx-python
+ray
```

### Comparing `pyAFQ-1.3.1/setup.cfg` & `pyafq-1.3.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 install_requires = 
 	scikit_image>=0.14.2
 	dipy>=1.8.0,<1.9.0
 	pandas
 	pybids>=0.16.2
 	templateflow>=0.8
 	pimms
+	pydra
 	joblib>=1.3.2
 	dask>=1.1
 	s3bids>=0.1.7
 	boto3>=1.14.0
 	s3fs~=0.4.2
 	toml>=0.10.0
 	setuptools_scm[toml]>=3.4.0,<5.1.0
@@ -42,14 +43,15 @@
 	popylar==0.2.*
 	plotly==5.3.0
 	kaleido==0.2.1
 	imageio>=2.0.0
 	Pillow
 	matplotlib
 	numpy==1.23.5
+	altair
 zip_safe = False
 include_package_data = True
 packages = find:
 
 [options.extras_require]
 dev = 
 	docutils==0.15.2
@@ -79,17 +81,17 @@
 	fslpy
 afqbrowser = 
 	AFQ-Browser>=0.3
 plot = 
 	pingouin>=0.3
 	seaborn>=0.11.0
 	ipython>=7.13.0,<=7.20.0
-	altair
 trx = 
 	trx-python
+	ray
 all = 
 	%(dev)s
 	%(fury)s
 	%(fsl)s
 	%(afqbrowser)s
 	%(plot)s
 	%(trx)s
```

### Comparing `pyAFQ-1.3.1/setup.py` & `pyafq-1.3.2/setup.py`

 * *Files identical despite different names*

