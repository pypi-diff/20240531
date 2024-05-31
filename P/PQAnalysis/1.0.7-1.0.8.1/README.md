# Comparing `tmp/pqanalysis-1.0.7.tar.gz` & `tmp/pqanalysis-1.0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqanalysis-1.0.7.tar", last modified: Fri May 31 13:09:24 2024, max compression
+gzip compressed data, was "pqanalysis-1.0.8.1.tar", last modified: Fri May 31 14:00:01 2024, max compression
```

## Comparing `pqanalysis-1.0.7.tar` & `pqanalysis-1.0.8.1.tar`

### file list

```diff
@@ -1,459 +1,463 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.882113 pqanalysis-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/.docstr.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.798113 pqanalysis-1.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.810113 pqanalysis-1.0.7/.github/.pylint_cache/
--rw-r--r--   0 runner    (1001) docker     (127)    16993 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/.github/.pylint_cache/PQAnalysis_1.stats
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.810113 pqanalysis-1.0.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.810113 pqanalysis-1.0.7/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/.github/scripts/parse_pylint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.810113 pqanalysis-1.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    22319 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/.style.yapf
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-31 13:09:24.882113 pqanalysis-1.0.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.810113 pqanalysis-1.0.7/PQAnalysis/
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/PQAnalysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-31 13:09:24.000000 pqanalysis-1.0.7/PQAnalysis/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.810113 pqanalysis-1.0.7/PQAnalysis/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/PQAnalysis/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.814113 pqanalysis-1.0.7/PQAnalysis/analysis/rdf/
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/PQAnalysis/analysis/rdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/PQAnalysis/analysis/rdf/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/PQAnalysis/analysis/rdf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    28845 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/PQAnalysis/analysis/rdf/rdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/PQAnalysis/analysis/rdf/rdf_input_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/PQAnalysis/analysis/rdf/rdf_output_file_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.814113 pqanalysis-1.0.7/PQAnalysis/atomic_system/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/PQAnalysis/atomic_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/PQAnalysis/atomic_system/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/PQAnalysis/atomic_system/_positions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/PQAnalysis/atomic_system/_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/PQAnalysis/atomic_system/_standard_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    24494 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/PQAnalysis/atomic_system/atomic_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/PQAnalysis/atomic_system/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.814113 pqanalysis-1.0.7/PQAnalysis/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/PQAnalysis/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/PQAnalysis/cli/_argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/PQAnalysis/cli/_cli_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7829 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/PQAnalysis/cli/add_molecules.py
--rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/PQAnalysis/cli/build_nep_traj.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/PQAnalysis/cli/continue_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/PQAnalysis/cli/gen2xyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/PQAnalysis/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/PQAnalysis/cli/rdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/PQAnalysis/cli/rst2xyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/PQAnalysis/cli/traj2box.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/PQAnalysis/cli/traj2qmcfc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/PQAnalysis/cli/xyz2gen.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/PQAnalysis/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.814113 pqanalysis-1.0.7/PQAnalysis/core/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-31 13:09:13.000000 pqanalysis-1.0.7/PQAnalysis/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/core/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.818113 pqanalysis-1.0.7/PQAnalysis/core/atom/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/core/atom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/core/atom/atom.py
--rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/core/atom/element.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.818113 pqanalysis-1.0.7/PQAnalysis/core/cell/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/core/cell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/core/cell/_standard_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/core/cell/cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/core/residue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/formats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.818113 pqanalysis-1.0.7/PQAnalysis/grammar/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/grammar/PQ_inputGrammar.lark
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/grammar/inputGrammar.lark
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/grammar/rules.lark
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/grammar/selection.lark
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/grammar/terminals.lark
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.818113 pqanalysis-1.0.7/PQAnalysis/io/
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/box_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/conversion_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/energy_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9726 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/formats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.822113 pqanalysis-1.0.7/PQAnalysis/io/gen_file/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/gen_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/gen_file/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/gen_file/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/gen_file/gen_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/gen_file/gen_file_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/info_file_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.822113 pqanalysis-1.0.7/PQAnalysis/io/input_file_reader/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/input_file_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/input_file_reader/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/input_file_reader/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)    17742 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/input_file_reader/input_file_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.822113 pqanalysis-1.0.7/PQAnalysis/io/input_file_reader/pq/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/input_file_reader/pq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/input_file_reader/pq/output_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     9932 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/input_file_reader/pq/pq_input_file_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.822113 pqanalysis-1.0.7/PQAnalysis/io/input_file_reader/pq_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/input_file_reader/pq_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/input_file_reader/pq_analysis/_file_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/input_file_reader/pq_analysis/_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/input_file_reader/pq_analysis/_positions_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/input_file_reader/pq_analysis/_selection_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/input_file_reader/pq_analysis/pqanalysis_input_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/moldescriptor_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.822113 pqanalysis-1.0.7/PQAnalysis/io/nep/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/nep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/nep/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    37872 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/nep/nep_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.822113 pqanalysis-1.0.7/PQAnalysis/io/restart_file/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/restart_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/restart_file/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/restart_file/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/restart_file/restart_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/restart_file/restart_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.826113 pqanalysis-1.0.7/PQAnalysis/io/topology_file/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/topology_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/topology_file/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/topology_file/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13349 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/topology_file/topology_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13355 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/topology_file/topology_file_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.826113 pqanalysis-1.0.7/PQAnalysis/io/traj_file/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/traj_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/traj_file/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/traj_file/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/traj_file/frame_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    22313 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/traj_file/trajectory_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/traj_file/trajectory_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.826113 pqanalysis-1.0.7/PQAnalysis/io/virial/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/virial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/virial/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/virial/virial_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/io/write_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.826113 pqanalysis-1.0.7/PQAnalysis/physical_data/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/physical_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/physical_data/energy.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/physical_data/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.826113 pqanalysis-1.0.7/PQAnalysis/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17228 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/tools/add_molecule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/tools/traj_to_com_traj.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.826113 pqanalysis-1.0.7/PQAnalysis/topology/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/topology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/topology/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.830113 pqanalysis-1.0.7/PQAnalysis/topology/bonded_topology/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/topology/bonded_topology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/topology/bonded_topology/_topology_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/topology/bonded_topology/angle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/topology/bonded_topology/bond.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/topology/bonded_topology/bonded_topology.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/topology/bonded_topology/dihedral.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/topology/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    23565 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/topology/selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7291 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/topology/shake_topology.py
--rw-r--r--   0 runner    (1001) docker     (127)    18809 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/topology/topology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.830113 pqanalysis-1.0.7/PQAnalysis/traj/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/traj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/traj/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/traj/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/traj/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)    13798 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/traj/trajectory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/type_checking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.830113 pqanalysis-1.0.7/PQAnalysis/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    13171 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/utils/custom_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/utils/math.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/PQAnalysis/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.878113 pqanalysis-1.0.7/PQAnalysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-31 13:09:24.000000 pqanalysis-1.0.7/PQAnalysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15124 2024-05-31 13:09:24.000000 pqanalysis-1.0.7/PQAnalysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:09:24.000000 pqanalysis-1.0.7/PQAnalysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-31 13:09:24.000000 pqanalysis-1.0.7/PQAnalysis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-31 13:09:24.000000 pqanalysis-1.0.7/PQAnalysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 13:09:24.000000 pqanalysis-1.0.7/PQAnalysis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.830113 pqanalysis-1.0.7/benchmarks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.830113 pqanalysis-1.0.7/benchmarks/core/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/benchmarks/core/benchmark_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/benchmarks/core/benchmark_traj_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/benchmarks/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.830113 pqanalysis-1.0.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)       73 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/autodoc.sh
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.830113 pqanalysis-1.0.7/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.802113 pqanalysis-1.0.7/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.830113 pqanalysis-1.0.7/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.834113 pqanalysis-1.0.7/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/_templates/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/_templates/package.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.850113 pqanalysis-1.0.7/docs/source/code/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.analysis.rdf.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.analysis.rdf.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.analysis.rdf.rdf.rst
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.analysis.rdf.rdf_input_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.analysis.rdf.rdf_output_file_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.analysis.rdf.rst
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.atomic_system.atomic_system.rst
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.atomic_system.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.atomic_system.rst
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.cli.add_molecules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.cli.build_nep_traj.rst
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.cli.continue_input.rst
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.cli.gen2xyz.rst
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.cli.rdf.rst
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.cli.rst2xyz.rst
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.cli.traj2box.rst
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.cli.traj2qmcfc.rst
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.cli.xyz2gen.rst
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.config.rst
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.core.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.core.atom.atom.rst
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.core.atom.element.rst
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.core.atom.rst
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.core.cell.cell.rst
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.core.cell.rst
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.core.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.core.residue.rst
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.core.rst
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.formats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.box_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.conversion_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.energy_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.formats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.gen_file.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.gen_file.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.gen_file.gen_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.gen_file.gen_file_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.gen_file.rst
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.info_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.input_file_reader.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.input_file_reader.formats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.input_file_reader.input_file_parser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.input_file_reader.pq.output_files.rst
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.input_file_reader.pq.pq_input_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.input_file_reader.pq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.pqanalysis_input_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.input_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.moldescriptor_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.nep.nep_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.nep.rst
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.restart_file.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.restart_file.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.restart_file.restart_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.restart_file.restart_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.restart_file.rst
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.rst
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.topology_file.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.topology_file.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.topology_file.rst
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.topology_file.topology_file_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.topology_file.topology_file_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.traj_file.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.traj_file.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.traj_file.frame_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.traj_file.rst
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.traj_file.trajectory_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.traj_file.trajectory_writer.rst
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.virial.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.virial.rst
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.virial.virial_reader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.write_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.physical_data.energy.rst
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.physical_data.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.physical_data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.tools.add_molecule.rst
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.tools.traj_to_com_traj.rst
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.topology.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.topology.bonded_topology.angle.rst
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.topology.bonded_topology.bond.rst
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.topology.bonded_topology.bonded_topology.rst
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.topology.bonded_topology.dihedral.rst
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.topology.bonded_topology.rst
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.topology.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.topology.rst
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.topology.selection.rst
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.topology.shake_topology.rst
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.topology.topology.rst
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.traj.api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.traj.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.traj.formats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.traj.rst
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.traj.trajectory.rst
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.type_checking.rst
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.types.rst
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.utils.common.rst
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.utils.custom_logging.rst
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.utils.decorators.rst
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.utils.files.rst
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.utils.random.rst
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/PQAnalysis.utils.units.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/code/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.850113 pqanalysis-1.0.7/docs/source/developerGuide/
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/developerGuide/developerGuide.rst
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.850113 pqanalysis-1.0.7/docs/source/logo/
--rw-r--r--   0 runner    (1001) docker     (127)   204575 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/logo/PQAnalysis.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.850113 pqanalysis-1.0.7/docs/source/userGuide/
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/userGuide/inputFile.rst
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/docs/source/userGuide/userGuide.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.802113 pqanalysis-1.0.7/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.854113 pqanalysis-1.0.7/examples/traj2box/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/examples/traj2box/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/examples/traj2box/acof_triclinic.xyz
--rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/examples/traj2box/acof_triclinic_2.xyz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.854113 pqanalysis-1.0.7/examples/traj2comtraj/
--rw-r--r--   0 runner    (1001) docker     (127)  2600700 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/examples/traj2comtraj/umcm-9-md-01.xyz
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/pytest.sh
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-31 13:09:24.882113 pqanalysis-1.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.858113 pqanalysis-1.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.858113 pqanalysis-1.0.7/tests/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.858113 pqanalysis-1.0.7/tests/analysis/rdf/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/analysis/rdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/analysis/rdf/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    14793 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/analysis/rdf/test_rdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/analysis/rdf/test_rdfInputFileReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/analysis/rdf/test_rdfOutputFileReader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.858113 pqanalysis-1.0.7/tests/atomicSystem/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/atomicSystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25879 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/atomicSystem/test_atomic_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/atomicSystem/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/atomicSystem/test_positions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.862113 pqanalysis-1.0.7/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/cli/test_continue_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/cli/test_rst2xyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/cli/test_traj2box.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/cli/test_traj2qmcfc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.862113 pqanalysis-1.0.7/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.862113 pqanalysis-1.0.7/tests/core/atom/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/core/atom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/core/atom/test_atom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/core/atom/test_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/core/test_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/core/test_residue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.806113 pqanalysis-1.0.7/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.862113 pqanalysis-1.0.7/tests/data/inputFileReader/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.862113 pqanalysis-1.0.7/tests/data/inputFileReader/PQ_input/
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/inputFileReader/PQ_input/n_not_matching.in
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/inputFileReader/PQ_input/n_not_matching_input_file_n-08.in
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/inputFileReader/PQ_input/no_output_files.in
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/inputFileReader/PQ_input/no_start_file.in
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/inputFileReader/PQ_input/old_n_not_less_one_than_actual_n-09.in
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/inputFileReader/PQ_input/run-08.in
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/inputFileReader/PQ_input/run-08.rpmd.in
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/inputFileReader/PQ_input/run-09.in.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/inputFileReader/PQ_input/run-09.rpmd.in.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/inputFileReader/PQ_input/run-10.in.ref
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/inputFileReader/PQ_input/run-10.rpmd.in.ref
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/inputFileReader/input.in
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/inputFileReader/input_PQ.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.862113 pqanalysis-1.0.7/tests/data/rdf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/rdf/input.in
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/rdf/required_keys_not_given.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.862113 pqanalysis-1.0.7/tests/data/readEnergyFile/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/readEnergyFile/md-01.en
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/readEnergyFile/md-01.info
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/readEnergyFile/md-01_noinfo.en
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.866113 pqanalysis-1.0.7/tests/data/readInfoFile/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/readInfoFile/md-01.info
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/readInfoFile/md-01.qmcfc.info
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.866113 pqanalysis-1.0.7/tests/data/readMoldescriptor/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/readMoldescriptor/moldescriptor.dat
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/readMoldescriptor/moldescriptor_withError.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.866113 pqanalysis-1.0.7/tests/data/readRestartFile/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/readRestartFile/md-01.rst
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/readRestartFile/moldescriptor.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.866113 pqanalysis-1.0.7/tests/data/rst2xyz/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/rst2xyz/md-01.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.866113 pqanalysis-1.0.7/tests/data/traj2box/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/traj2box/box.dat
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/traj2box/box.vmd.xyz
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/traj2box/test.xyz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.870113 pqanalysis-1.0.7/tests/data/traj2qmcfc/
--rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/traj2qmcfc/acof_triclinic.xyz
--rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/traj2qmcfc/acof_triclinic_2.xyz
--rw-r--r--   0 runner    (1001) docker     (127)  2301740 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/data/traj2qmcfc/traj.qmcfc.xyz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.874113 pqanalysis-1.0.7/tests/io/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.874113 pqanalysis-1.0.7/tests/io/inputFileReader/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.874113 pqanalysis-1.0.7/tests/io/inputFileReader/PQ/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/io/inputFileReader/PQ/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8594 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/io/inputFileReader/PQ/test_PQ_inputFileReader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.874113 pqanalysis-1.0.7/tests/io/inputFileReader/PQAnalysis/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/io/inputFileReader/PQAnalysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/io/inputFileReader/PQAnalysis/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/io/inputFileReader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/io/inputFileReader/test_inputDictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/io/inputFileReader/test_inputFileParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/io/inputFileReader/test_transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/io/inputFileReader/test_visitors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/io/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/io/test_boxWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/io/test_energyFileReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/io/test_frameReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/io/test_infoFileReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/io/test_moldescriptorReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6746 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/io/test_restartReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/io/test_restartWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)    23202 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/io/test_trajectoryReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/io/test_trajectoryWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/io/test_write_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.874113 pqanalysis-1.0.7/tests/physicalData/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/physicalData/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/physicalData/test_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/test_formats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.874113 pqanalysis-1.0.7/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/tools/test_traj_to_com_traj.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.878113 pqanalysis-1.0.7/tests/topology/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/topology/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.878113 pqanalysis-1.0.7/tests/topology/bonded_topology/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/topology/bonded_topology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/topology/bonded_topology/test_angle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/topology/bonded_topology/test_bond.py
--rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/topology/bonded_topology/test_bondedTopology.py
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/topology/bonded_topology/test_dihedral.py
--rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/topology/test_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/topology/test_selectionTransformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/topology/test_shakeTopology.py
--rw-r--r--   0 runner    (1001) docker     (127)    12759 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/topology/test_topology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.878113 pqanalysis-1.0.7/tests/traj/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/traj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/traj/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13220 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/traj/test_trajectory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:09:24.878113 pqanalysis-1.0.7/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/utils/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/utils/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-31 13:09:14.000000 pqanalysis-1.0.7/tests/utils/test_math.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.582885 pqanalysis-1.0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/.docstr.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.502884 pqanalysis-1.0.8.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.510884 pqanalysis-1.0.8.1/.github/.pylint_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)    16885 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/.github/.pylint_cache/PQAnalysis_1.stats
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.510884 pqanalysis-1.0.8.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.510884 pqanalysis-1.0.8.1/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/.github/scripts/parse_pylint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.510884 pqanalysis-1.0.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    22319 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/.style.yapf
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-31 14:00:01.582885 pqanalysis-1.0.8.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.514884 pqanalysis-1.0.8.1/PQAnalysis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-31 14:00:01.000000 pqanalysis-1.0.8.1/PQAnalysis/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.514884 pqanalysis-1.0.8.1/PQAnalysis/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.514884 pqanalysis-1.0.8.1/PQAnalysis/analysis/rdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/analysis/rdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/analysis/rdf/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/analysis/rdf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28845 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/analysis/rdf/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/analysis/rdf/rdf_input_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/analysis/rdf/rdf_output_file_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.514884 pqanalysis-1.0.8.1/PQAnalysis/atomic_system/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/atomic_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/atomic_system/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/atomic_system/_positions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/atomic_system/_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/atomic_system/_standard_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24591 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/atomic_system/atomic_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/atomic_system/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.518884 pqanalysis-1.0.8.1/PQAnalysis/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/cli/_argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/cli/_cli_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7829 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/cli/add_molecules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/cli/build_nep_traj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/cli/continue_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/cli/gen2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/cli/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/cli/rst2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/cli/traj2box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/cli/traj2qmcfc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/cli/xyz2gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.518884 pqanalysis-1.0.8.1/PQAnalysis/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/core/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.518884 pqanalysis-1.0.8.1/PQAnalysis/core/atom/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/core/atom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/core/atom/atom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/core/atom/element.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.518884 pqanalysis-1.0.8.1/PQAnalysis/core/cell/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/core/cell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/core/cell/_standard_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/core/cell/cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/core/residue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/formats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.518884 pqanalysis-1.0.8.1/PQAnalysis/grammar/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/grammar/PQ_inputGrammar.lark
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/grammar/inputGrammar.lark
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/grammar/rules.lark
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/grammar/selection.lark
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/grammar/terminals.lark
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.522884 pqanalysis-1.0.8.1/PQAnalysis/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/box_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/conversion_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/energy_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9742 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/formats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.522884 pqanalysis-1.0.8.1/PQAnalysis/io/gen_file/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/gen_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/gen_file/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/gen_file/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/gen_file/gen_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/gen_file/gen_file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/info_file_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.522884 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17742 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/input_file_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.522884 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq/output_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9820 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq/pq_input_file_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.526884 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq_analysis/_file_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq_analysis/_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq_analysis/_positions_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq_analysis/_selection_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq_analysis/pqanalysis_input_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/moldescriptor_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.526884 pqanalysis-1.0.8.1/PQAnalysis/io/nep/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/nep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/nep/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37872 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/nep/nep_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.526884 pqanalysis-1.0.8.1/PQAnalysis/io/restart_file/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/restart_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/restart_file/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/restart_file/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9950 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/restart_file/restart_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/restart_file/restart_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.526884 pqanalysis-1.0.8.1/PQAnalysis/io/topology_file/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/topology_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/topology_file/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/topology_file/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13349 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/topology_file/topology_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13355 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/topology_file/topology_file_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.526884 pqanalysis-1.0.8.1/PQAnalysis/io/traj_file/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/traj_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/traj_file/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/traj_file/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/traj_file/frame_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22313 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/traj_file/trajectory_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/traj_file/trajectory_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.526884 pqanalysis-1.0.8.1/PQAnalysis/io/virial/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/virial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/virial/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/virial/virial_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/io/write_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.530884 pqanalysis-1.0.8.1/PQAnalysis/physical_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/physical_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/physical_data/energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/physical_data/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.530884 pqanalysis-1.0.8.1/PQAnalysis/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17268 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/tools/add_molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/tools/traj_to_com_traj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.530884 pqanalysis-1.0.8.1/PQAnalysis/topology/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/topology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/topology/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.530884 pqanalysis-1.0.8.1/PQAnalysis/topology/bonded_topology/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/topology/bonded_topology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/topology/bonded_topology/_topology_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/topology/bonded_topology/angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/topology/bonded_topology/bond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/topology/bonded_topology/bonded_topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/topology/bonded_topology/dihedral.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/topology/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23565 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/topology/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7291 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/topology/shake_topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18809 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/topology/topology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.530884 pqanalysis-1.0.8.1/PQAnalysis/traj/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/traj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/traj/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/traj/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/traj/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13798 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/traj/trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/type_checking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.534884 pqanalysis-1.0.8.1/PQAnalysis/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13171 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/utils/custom_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/utils/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/PQAnalysis/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.582885 pqanalysis-1.0.8.1/PQAnalysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-31 14:00:01.000000 pqanalysis-1.0.8.1/PQAnalysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15249 2024-05-31 14:00:01.000000 pqanalysis-1.0.8.1/PQAnalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 14:00:01.000000 pqanalysis-1.0.8.1/PQAnalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-31 14:00:01.000000 pqanalysis-1.0.8.1/PQAnalysis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-31 14:00:01.000000 pqanalysis-1.0.8.1/PQAnalysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 14:00:01.000000 pqanalysis-1.0.8.1/PQAnalysis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.534884 pqanalysis-1.0.8.1/benchmarks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.534884 pqanalysis-1.0.8.1/benchmarks/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/benchmarks/core/benchmark_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/benchmarks/core/benchmark_traj_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/benchmarks/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.534884 pqanalysis-1.0.8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)       73 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/autodoc.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.534884 pqanalysis-1.0.8.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.506884 pqanalysis-1.0.8.1/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.534884 pqanalysis-1.0.8.1/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.534884 pqanalysis-1.0.8.1/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/_templates/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/_templates/package.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.554885 pqanalysis-1.0.8.1/docs/source/code/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.analysis.rdf.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.analysis.rdf.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.analysis.rdf.rdf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.analysis.rdf.rdf_input_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.analysis.rdf.rdf_output_file_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.analysis.rdf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.atomic_system.atomic_system.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.atomic_system.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.atomic_system.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.cli.add_molecules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.cli.build_nep_traj.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.cli.continue_input.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.cli.gen2xyz.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.cli.rdf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.cli.rst2xyz.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.cli.traj2box.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.cli.traj2qmcfc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.cli.xyz2gen.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.core.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.core.atom.atom.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.core.atom.element.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.core.atom.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.core.cell.cell.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.core.cell.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.core.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.core.residue.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.core.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.box_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.conversion_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.energy_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.gen_file.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.gen_file.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.gen_file.gen_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.gen_file.gen_file_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.gen_file.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.info_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.input_file_reader.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.input_file_reader.formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.input_file_reader.input_file_parser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.input_file_reader.pq.output_files.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.input_file_reader.pq.pq_input_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.input_file_reader.pq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.pqanalysis_input_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.input_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.moldescriptor_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.nep.nep_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.nep.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.restart_file.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.restart_file.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.restart_file.restart_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.restart_file.restart_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.restart_file.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.topology_file.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.topology_file.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.topology_file.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.topology_file.topology_file_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.topology_file.topology_file_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.traj_file.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.traj_file.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.traj_file.frame_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.traj_file.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.traj_file.trajectory_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.traj_file.trajectory_writer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.virial.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.virial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.virial.virial_reader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.write_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.physical_data.energy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.physical_data.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.physical_data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.tools.add_molecule.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.tools.traj_to_com_traj.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.topology.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.topology.bonded_topology.angle.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.topology.bonded_topology.bond.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.topology.bonded_topology.bonded_topology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.topology.bonded_topology.dihedral.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.topology.bonded_topology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.topology.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.topology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.topology.selection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.topology.shake_topology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.topology.topology.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.traj.api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.traj.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.traj.formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.traj.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.traj.trajectory.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.type_checking.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.types.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.utils.common.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.utils.custom_logging.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.utils.decorators.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.utils.files.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.utils.random.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.utils.units.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/code/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.554885 pqanalysis-1.0.8.1/docs/source/developerGuide/
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/developerGuide/developerGuide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.554885 pqanalysis-1.0.8.1/docs/source/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)   204575 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/logo/PQAnalysis.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.554885 pqanalysis-1.0.8.1/docs/source/userGuide/
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/userGuide/inputFile.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/docs/source/userGuide/userGuide.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.506884 pqanalysis-1.0.8.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.554885 pqanalysis-1.0.8.1/examples/add_molecules/
+-rw-r--r--   0 runner    (1001) docker     (127)   119066 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/examples/add_molecules/mil68ga-md-01.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/examples/add_molecules/perylene-md-05.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/examples/add_molecules/perylene-md-05.xyz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.554885 pqanalysis-1.0.8.1/examples/traj2box/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/examples/traj2box/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/examples/traj2box/acof_triclinic.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/examples/traj2box/acof_triclinic_2.xyz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.558884 pqanalysis-1.0.8.1/examples/traj2comtraj/
+-rw-r--r--   0 runner    (1001) docker     (127)  2600700 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/examples/traj2comtraj/umcm-9-md-01.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/pytest.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-31 14:00:01.586885 pqanalysis-1.0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.562885 pqanalysis-1.0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.562885 pqanalysis-1.0.8.1/tests/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.562885 pqanalysis-1.0.8.1/tests/analysis/rdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/analysis/rdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/analysis/rdf/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14793 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/analysis/rdf/test_rdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/analysis/rdf/test_rdfInputFileReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/analysis/rdf/test_rdfOutputFileReader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.562885 pqanalysis-1.0.8.1/tests/atomicSystem/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/atomicSystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25879 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/atomicSystem/test_atomic_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/atomicSystem/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/atomicSystem/test_positions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.562885 pqanalysis-1.0.8.1/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/cli/test_continue_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/cli/test_rst2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/cli/test_traj2box.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/cli/test_traj2qmcfc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.562885 pqanalysis-1.0.8.1/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.566885 pqanalysis-1.0.8.1/tests/core/atom/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:59:49.000000 pqanalysis-1.0.8.1/tests/core/atom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/core/atom/test_atom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/core/atom/test_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/core/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/core/test_residue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.506884 pqanalysis-1.0.8.1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.566885 pqanalysis-1.0.8.1/tests/data/inputFileReader/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.566885 pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/n_not_matching.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/n_not_matching_input_file_n-08.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/no_output_files.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/no_start_file.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/old_n_not_less_one_than_actual_n-09.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/run-08.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/run-08.rpmd.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/run-09.in.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/run-09.rpmd.in.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/run-10.in.ref
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/run-10.rpmd.in.ref
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/inputFileReader/input.in
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/inputFileReader/input_PQ.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.566885 pqanalysis-1.0.8.1/tests/data/rdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/rdf/input.in
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/rdf/required_keys_not_given.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.566885 pqanalysis-1.0.8.1/tests/data/readEnergyFile/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/readEnergyFile/md-01.en
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/readEnergyFile/md-01.info
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/readEnergyFile/md-01_noinfo.en
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.566885 pqanalysis-1.0.8.1/tests/data/readInfoFile/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/readInfoFile/md-01.info
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/readInfoFile/md-01.qmcfc.info
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.570885 pqanalysis-1.0.8.1/tests/data/readMoldescriptor/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/readMoldescriptor/moldescriptor.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/readMoldescriptor/moldescriptor_withError.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.570885 pqanalysis-1.0.8.1/tests/data/readRestartFile/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/readRestartFile/md-01.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/readRestartFile/moldescriptor.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.570885 pqanalysis-1.0.8.1/tests/data/rst2xyz/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/rst2xyz/md-01.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.570885 pqanalysis-1.0.8.1/tests/data/traj2box/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/traj2box/box.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/traj2box/box.vmd.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/traj2box/test.xyz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.574885 pqanalysis-1.0.8.1/tests/data/traj2qmcfc/
+-rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/traj2qmcfc/acof_triclinic.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)  1170470 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/traj2qmcfc/acof_triclinic_2.xyz
+-rw-r--r--   0 runner    (1001) docker     (127)  2301740 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/data/traj2qmcfc/traj.qmcfc.xyz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.578885 pqanalysis-1.0.8.1/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.578885 pqanalysis-1.0.8.1/tests/io/inputFileReader/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.578885 pqanalysis-1.0.8.1/tests/io/inputFileReader/PQ/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/inputFileReader/PQ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8594 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/inputFileReader/PQ/test_PQ_inputFileReader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.578885 pqanalysis-1.0.8.1/tests/io/inputFileReader/PQAnalysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/inputFileReader/PQAnalysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/inputFileReader/PQAnalysis/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/inputFileReader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/inputFileReader/test_inputDictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/inputFileReader/test_inputFileParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/inputFileReader/test_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/inputFileReader/test_visitors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/test_boxWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/test_energyFileReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/test_frameReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/test_infoFileReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/test_moldescriptorReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/test_restartReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/test_restartWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23202 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/test_trajectoryReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/test_trajectoryWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/io/test_write_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.578885 pqanalysis-1.0.8.1/tests/physicalData/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/physicalData/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/physicalData/test_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/test_formats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.578885 pqanalysis-1.0.8.1/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/tools/test_traj_to_com_traj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.578885 pqanalysis-1.0.8.1/tests/topology/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/topology/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.582885 pqanalysis-1.0.8.1/tests/topology/bonded_topology/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/topology/bonded_topology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/topology/bonded_topology/test_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/topology/bonded_topology/test_bond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/topology/bonded_topology/test_bondedTopology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/topology/bonded_topology/test_dihedral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/topology/test_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/topology/test_selectionTransformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/topology/test_shakeTopology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12759 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/topology/test_topology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.582885 pqanalysis-1.0.8.1/tests/traj/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/traj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/traj/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13220 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/traj/test_trajectory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:00:01.582885 pqanalysis-1.0.8.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/utils/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/utils/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-31 13:59:50.000000 pqanalysis-1.0.8.1/tests/utils/test_math.py
```

### Comparing `pqanalysis-1.0.7/.codecov.yml` & `pqanalysis-1.0.8.1/.codecov.yml`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/.github/.pylint_cache/PQAnalysis_1.stats` & `pqanalysis-1.0.8.1/.github/.pylint_cache/PQAnalysis_1.stats`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 9556 4200 0000 0000 008c 1870 796c  ...VB........pyl
+00000000: 8004 95ea 4100 0000 0000 008c 1870 796c  ....A........pyl
 00000010: 696e 742e 7574 696c 732e 6c69 6e74 6572  int.utils.linter
 00000020: 7374 6174 7394 8c0b 4c69 6e74 6572 5374  stats...LinterSt
 00000030: 6174 7394 9394 2981 947d 9428 8c09 6261  ats...)..}.(..ba
 00000040: 645f 6e61 6d65 7394 7d94 288c 0861 7267  d_names.}.(..arg
 00000050: 756d 656e 7494 4b00 8c04 6174 7472 944b  ument.K...attr.K
 00000060: 008c 056b 6c61 7373 944b 008c 0f63 6c61  ...klass.K...cla
 00000070: 7373 5f61 7474 7269 6275 7465 944b 008c  ss_attribute.K..
@@ -10,1054 +10,1047 @@
 00000090: 0563 6f6e 7374 944b 0c8c 0969 6e6c 696e  .const.K...inlin
 000000a0: 6576 6172 944b 008c 0866 756e 6374 696f  evar.K...functio
 000000b0: 6e94 4b00 8c06 6d65 7468 6f64 944b 028c  n.K...method.K..
 000000c0: 066d 6f64 756c 6594 4b01 8c08 7661 7269  .module.K...vari
 000000d0: 6162 6c65 944b 008c 0774 7970 6576 6172  able.K...typevar
 000000e0: 944b 008c 0974 7970 6561 6c69 6173 944b  .K...typealias.K
 000000f0: 0075 8c09 6279 5f6d 6f64 756c 6594 7d94  .u..by_module.}.
-00000100: 288c 272f 686f 6d65 2f6a 6167 2f70 726f  (.'/home/jag/pro
-00000110: 6a65 6374 732f 7071 616e 616c 7973 6973  jects/pqanalysis
-00000120: 2f2e 7079 6c69 6e74 7263 947d 9428 8c0a  /.pylintrc.}.(..
-00000130: 636f 6e76 656e 7469 6f6e 944b 008c 0565  convention.K...e
-00000140: 7272 6f72 944b 008c 0566 6174 616c 944b  rror.K...fatal.K
-00000150: 008c 0469 6e66 6f94 4b00 8c08 7265 6661  ...info.K...refa
-00000160: 6374 6f72 944b 008c 0973 7461 7465 6d65  ctor.K...stateme
-00000170: 6e74 944b 008c 0777 6172 6e69 6e67 944b  nt.K...warning.K
-00000180: 0075 8c0c 436f 6d6d 616e 6420 6c69 6e65  .u..Command line
-00000190: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
-000001a0: 681b 4b00 681c 4b00 681d 4b00 681e 4b00  h.K.h.K.h.K.h.K.
-000001b0: 758c 2243 6f6d 6d61 6e64 206c 696e 6520  u."Command line 
-000001c0: 6f72 2063 6f6e 6669 6775 7261 7469 6f6e  or configuration
-000001d0: 2066 696c 6594 7d94 2868 184b 0068 194b   file.}.(h.K.h.K
-000001e0: 0068 1a4b 0068 1b4b 0068 1c4b 0068 1d4b  .h.K.h.K.h.K.h.K
-000001f0: 0068 1e4b 0075 8c0a 5051 416e 616c 7973  .h.K.u..PQAnalys
-00000200: 6973 947d 9428 6818 4b00 6819 4b01 681a  is.}.(h.K.h.K.h.
-00000210: 4b00 681b 4b00 681c 4b00 681d 4b1c 681e  K.h.K.h.K.h.K.h.
-00000220: 4b01 758c 1550 5141 6e61 6c79 7369 732e  K.u..PQAnalysis.
-00000230: 6578 6365 7074 696f 6e73 947d 9428 6818  exceptions.}.(h.
-00000240: 4b00 6819 4b00 681a 4b00 681b 4b00 681c  K.h.K.h.K.h.K.h.
-00000250: 4b00 681d 4b11 681e 4b00 758c 1150 5141  K.h.K.h.K.u..PQA
-00000260: 6e61 6c79 7369 732e 636f 6e66 6967 947d  nalysis.config.}
-00000270: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
-00000280: 4b00 681c 4b00 681d 4b06 681e 4b00 758c  K.h.K.h.K.h.K.u.
-00000290: 1250 5141 6e61 6c79 7369 732e 666f 726d  .PQAnalysis.form
-000002a0: 6174 7394 7d94 2868 184b 0068 194b 0068  ats.}.(h.K.h.K.h
-000002b0: 1a4b 0068 1b4b 0068 1c4b 0068 1d4b 1468  .K.h.K.h.K.h.K.h
-000002c0: 1e4b 0075 8c10 5051 416e 616c 7973 6973  .K.u..PQAnalysis
-000002d0: 2e74 7970 6573 947d 9428 6818 4b00 6819  .types.}.(h.K.h.
-000002e0: 4b00 681a 4b00 681b 4b00 681c 4b00 681d  K.h.K.h.K.h.K.h.
-000002f0: 4b0f 681e 4b00 758c 1850 5141 6e61 6c79  K.h.K.u..PQAnaly
-00000300: 7369 732e 7479 7065 5f63 6865 636b 696e  sis.type_checkin
-00000310: 6794 7d94 2868 184b 0068 194b 0068 1a4b  g.}.(h.K.h.K.h.K
-00000320: 0068 1b4b 0068 1c4b 0068 1d4b 3768 1e4b  .h.K.h.K.h.K7h.K
-00000330: 0075 8c16 5051 416e 616c 7973 6973 2e75  .u..PQAnalysis.u
-00000340: 7469 6c73 2e66 696c 6573 947d 9428 6818  tils.files.}.(h.
-00000350: 4b00 6819 4b00 681a 4b00 681b 4b00 681c  K.h.K.h.K.h.K.h.
-00000360: 4b00 681d 4b0a 681e 4b00 758c 1650 5141  K.h.K.h.K.u..PQA
-00000370: 6e61 6c79 7369 732e 7574 696c 732e 756e  nalysis.utils.un
-00000380: 6974 7394 7d94 2868 184b 0068 194b 0068  its.}.(h.K.h.K.h
-00000390: 1a4b 0068 1b4b 0068 1c4b 0068 1d4b 0768  .K.h.K.h.K.h.K.h
-000003a0: 1e4b 0075 8c19 5051 416e 616c 7973 6973  .K.u..PQAnalysis
-000003b0: 2e75 7469 6c73 2e5f 5f69 6e69 745f 5f94  .utils.__init__.
-000003c0: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
-000003d0: 1b4b 0068 1c4b 0068 1d4b 0268 1e4b 0075  .K.h.K.h.K.h.K.u
-000003e0: 8c17 5051 416e 616c 7973 6973 2e75 7469  ..PQAnalysis.uti
-000003f0: 6c73 2e63 6f6d 6d6f 6e94 7d94 2868 184b  ls.common.}.(h.K
-00000400: 0068 194b 0068 1a4b 0068 1b4b 0068 1c4b  .h.K.h.K.h.K.h.K
-00000410: 0068 1d4b 0968 1e4b 0075 8c1f 5051 416e  .h.K.h.K.u..PQAn
-00000420: 616c 7973 6973 2e75 7469 6c73 2e63 7573  alysis.utils.cus
-00000430: 746f 6d5f 6c6f 6767 696e 6794 7d94 2868  tom_logging.}.(h
-00000440: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
-00000450: 1c4b 0068 1d4b 6568 1e4b 0075 8c15 5051  .K.h.Keh.K.u..PQ
-00000460: 416e 616c 7973 6973 2e75 7469 6c73 2e6d  Analysis.utils.m
-00000470: 6174 6894 7d94 2868 184b 0068 194b 0068  ath.}.(h.K.h.K.h
-00000480: 1a4b 0068 1b4b 0068 1c4b 0068 1d4b 0768  .K.h.K.h.K.h.K.h
-00000490: 1e4b 0075 8c1b 5051 416e 616c 7973 6973  .K.u..PQAnalysis
-000004a0: 2e75 7469 6c73 2e64 6563 6f72 6174 6f72  .utils.decorator
-000004b0: 7394 7d94 2868 184b 0068 194b 0068 1a4b  s.}.(h.K.h.K.h.K
-000004c0: 0068 1b4b 0068 1c4b 0068 1d4b 2068 1e4b  .h.K.h.K.h.K h.K
-000004d0: 0075 8c17 5051 416e 616c 7973 6973 2e75  .u..PQAnalysis.u
-000004e0: 7469 6c73 2e72 616e 646f 6d94 7d94 2868  tils.random.}.(h
-000004f0: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
-00000500: 1c4b 0068 1d4b 0668 1e4b 0075 8c1c 5051  .K.h.K.h.K.u..PQ
-00000510: 416e 616c 7973 6973 2e61 6e61 6c79 7369  Analysis.analysi
-00000520: 732e 5f5f 696e 6974 5f5f 947d 9428 6818  s.__init__.}.(h.
-00000530: 4b00 6819 4b00 681a 4b00 681b 4b00 681c  K.h.K.h.K.h.K.h.
-00000540: 4b00 681d 4b01 681e 4b00 758c 2250 5141  K.h.K.h.K.u."PQA
-00000550: 6e61 6c79 7369 732e 616e 616c 7973 6973  nalysis.analysis
-00000560: 2e72 6466 2e65 7863 6570 7469 6f6e 7394  .rdf.exceptions.
-00000570: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
-00000580: 1b4b 0068 1c4b 0068 1d4b 0968 1e4b 0075  .K.h.K.h.K.h.K.u
-00000590: 8c2e 5051 416e 616c 7973 6973 2e61 6e61  ..PQAnalysis.ana
-000005a0: 6c79 7369 732e 7264 662e 7264 665f 6f75  lysis.rdf.rdf_ou
-000005b0: 7470 7574 5f66 696c 655f 7772 6974 6572  tput_file_writer
-000005c0: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
-000005d0: 681b 4b00 681c 4b00 681d 4b33 681e 4b00  h.K.h.K.h.K3h.K.
-000005e0: 758c 1b50 5141 6e61 6c79 7369 732e 616e  u..PQAnalysis.an
-000005f0: 616c 7973 6973 2e72 6466 2e72 6466 947d  alysis.rdf.rdf.}
-00000600: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
-00000610: 4b00 681c 4b03 681d 4b9a 681e 4b00 758c  K.h.K.h.K.h.K.u.
-00000620: 2d50 5141 6e61 6c79 7369 732e 616e 616c  -PQAnalysis.anal
-00000630: 7973 6973 2e72 6466 2e72 6466 5f69 6e70  ysis.rdf.rdf_inp
-00000640: 7574 5f66 696c 655f 7265 6164 6572 947d  ut_file_reader.}
-00000650: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
-00000660: 4b00 681c 4b00 681d 4b18 681e 4b00 758c  K.h.K.h.K.h.K.u.
-00000670: 1b50 5141 6e61 6c79 7369 732e 616e 616c  .PQAnalysis.anal
-00000680: 7973 6973 2e72 6466 2e61 7069 947d 9428  ysis.rdf.api.}.(
-00000690: 6818 4b00 6819 4b00 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
-000006a0: 681c 4b00 681d 4b1e 681e 4b00 758c 2050  h.K.h.K.h.K.u. P
-000006b0: 5141 6e61 6c79 7369 732e 616e 616c 7973  QAnalysis.analys
-000006c0: 6973 2e72 6466 2e5f 5f69 6e69 745f 5f94  is.rdf.__init__.
-000006d0: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
-000006e0: 1b4b 0068 1c4b 0068 1d4b 0568 1e4b 0075  .K.h.K.h.K.h.K.u
-000006f0: 8c19 5051 416e 616c 7973 6973 2e74 6f6f  ..PQAnalysis.too
-00000700: 6c73 2e5f 5f69 6e69 745f 5f94 7d94 2868  ls.__init__.}.(h
-00000710: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
-00000720: 1c4b 0068 1d4b 0168 1e4b 0075 8c21 5051  .K.h.K.h.K.u.!PQ
-00000730: 416e 616c 7973 6973 2e74 6f6f 6c73 2e74  Analysis.tools.t
-00000740: 7261 6a5f 746f 5f63 6f6d 5f74 7261 6a94  raj_to_com_traj.
-00000750: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
-00000760: 1b4b 0068 1c4b 0068 1d4b 0c68 1e4b 0275  .K.h.K.h.K.h.K.u
-00000770: 8c1d 5051 416e 616c 7973 6973 2e74 6f6f  ..PQAnalysis.too
-00000780: 6c73 2e61 6464 5f6d 6f6c 6563 756c 6594  ls.add_molecule.
-00000790: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
-000007a0: 1b4b 0068 1c4b 0468 1d4b 5268 1e4b 0075  .K.h.K.h.KRh.K.u
-000007b0: 8c12 5051 416e 616c 7973 6973 2e63 6c69  ..PQAnalysis.cli
-000007c0: 2e72 6466 947d 9428 6818 4b00 6819 4b00  .rdf.}.(h.K.h.K.
-000007d0: 681a 4b00 681b 4b00 681c 4b00 681d 4b1f  h.K.h.K.h.K.h.K.
-000007e0: 681e 4b00 758c 1d50 5141 6e61 6c79 7369  h.K.u..PQAnalysi
-000007f0: 732e 636c 692e 6275 696c 645f 6e65 705f  s.cli.build_nep_
-00000800: 7472 616a 947d 9428 6818 4b00 6819 4b00  traj.}.(h.K.h.K.
-00000810: 681a 4b00 681b 4b00 681c 4b00 681d 4b1f  h.K.h.K.h.K.h.K.
-00000820: 681e 4b00 758c 1650 5141 6e61 6c79 7369  h.K.u..PQAnalysi
-00000830: 732e 636c 692e 7879 7a32 6765 6e94 7d94  s.cli.xyz2gen.}.
-00000840: 2868 184b 0068 194b 0068 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
-00000850: 0068 1c4b 0068 1d4b 1b68 1e4b 0075 8c18  .h.K.h.K.h.K.u..
-00000860: 5051 416e 616c 7973 6973 2e63 6c69 2e5f  PQAnalysis.cli._
-00000870: 636c 695f 6261 7365 947d 9428 6818 4b00  cli_base.}.(h.K.
-00000880: 6819 4b00 681a 4b00 681b 4b00 681c 4b00  h.K.h.K.h.K.h.K.
-00000890: 681d 4b05 681e 4b00 758c 1750 5141 6e61  h.K.h.K.u..PQAna
-000008a0: 6c79 7369 732e 636c 692e 7472 616a 3262  lysis.cli.traj2b
-000008b0: 6f78 947d 9428 6818 4b00 6819 4b00 681a  ox.}.(h.K.h.K.h.
-000008c0: 4b00 681b 4b00 681c 4b00 681d 4b1a 681e  K.h.K.h.K.h.K.h.
-000008d0: 4b00 758c 1c50 5141 6e61 6c79 7369 732e  K.u..PQAnalysis.
-000008e0: 636c 692e 6164 645f 6d6f 6c65 6375 6c65  cli.add_molecule
-000008f0: 7394 7d94 2868 184b 0068 194b 0068 1a4b  s.}.(h.K.h.K.h.K
-00000900: 0068 1b4b 0068 1c4b 0068 1d4b 2868 1e4b  .h.K.h.K.h.K(h.K
-00000910: 0075 8c17 5051 416e 616c 7973 6973 2e63  .u..PQAnalysis.c
-00000920: 6c69 2e5f 5f69 6e69 745f 5f94 7d94 2868  li.__init__.}.(h
-00000930: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
-00000940: 1c4b 0068 1d4b 0268 1e4b 0075 8c1d 5051  .K.h.K.h.K.u..PQ
-00000950: 416e 616c 7973 6973 2e63 6c69 2e63 6f6e  Analysis.cli.con
-00000960: 7469 6e75 655f 696e 7075 7494 7d94 2868  tinue_input.}.(h
-00000970: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
-00000980: 1c4b 0068 1d4b 1a68 1e4b 0075 8c16 5051  .K.h.K.h.K.u..PQ
-00000990: 416e 616c 7973 6973 2e63 6c69 2e72 7374  Analysis.cli.rst
-000009a0: 3278 797a 947d 9428 6818 4b00 6819 4b00  2xyz.}.(h.K.h.K.
-000009b0: 681a 4b00 681b 4b00 681c 4b00 681d 4b1b  h.K.h.K.h.K.h.K.
-000009c0: 681e 4b00 758c 1650 5141 6e61 6c79 7369  h.K.u..PQAnalysi
-000009d0: 732e 636c 692e 6765 6e32 7879 7a94 7d94  s.cli.gen2xyz.}.
-000009e0: 2868 184b 0068 194b 0068 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
-000009f0: 0068 1c4b 0068 1d4b 1b68 1e4b 0075 8c13  .h.K.h.K.h.K.u..
-00000a00: 5051 416e 616c 7973 6973 2e63 6c69 2e6d  PQAnalysis.cli.m
-00000a10: 6169 6e94 7d94 2868 184b 0068 194b 0068  ain.}.(h.K.h.K.h
-00000a20: 1a4b 0068 1b4b 0068 1c4b 0068 1d4b 1c68  .K.h.K.h.K.h.K.h
-00000a30: 1e4b 0075 8c1f 5051 416e 616c 7973 6973  .K.u..PQAnalysis
-00000a40: 2e63 6c69 2e5f 6172 6775 6d65 6e74 5f70  .cli._argument_p
-00000a50: 6172 7365 7294 7d94 2868 184b 0068 194b  arser.}.(h.K.h.K
-00000a60: 0068 1a4b 0068 1b4b 0068 1c4b 0068 1d4b  .h.K.h.K.h.K.h.K
-00000a70: 3368 1e4b 0075 8c19 5051 416e 616c 7973  3h.K.u..PQAnalys
-00000a80: 6973 2e63 6c69 2e74 7261 6a32 716d 6366  is.cli.traj2qmcf
-00000a90: 6394 7d94 2868 184b 0068 194b 0068 1a4b  c.}.(h.K.h.K.h.K
-00000aa0: 0068 1b4b 0068 1c4b 0068 1d4b 1968 1e4b  .h.K.h.K.h.K.h.K
-00000ab0: 0075 8c23 5051 416e 616c 7973 6973 2e70  .u.#PQAnalysis.p
-00000ac0: 6879 7369 6361 6c5f 6461 7461 2e65 7863  hysical_data.exc
-00000ad0: 6570 7469 6f6e 7394 7d94 2868 184b 0068  eptions.}.(h.K.h
-00000ae0: 194b 0068 1a4b 0068 1b4b 0068 1c4b 0068  .K.h.K.h.K.h.K.h
-00000af0: 1d4b 0568 1e4b 0075 8c1f 5051 416e 616c  .K.h.K.u..PQAnal
-00000b00: 7973 6973 2e70 6879 7369 6361 6c5f 6461  ysis.physical_da
-00000b10: 7461 2e65 6e65 7267 7994 7d94 2868 184b  ta.energy.}.(h.K
-00000b20: 0068 194b 0068 1a4b 0068 1b4b 0068 1c4b  .h.K.h.K.h.K.h.K
-00000b30: 0068 1d4b 3e68 1e4b 0075 8c21 5051 416e  .h.K>h.K.u.!PQAn
-00000b40: 616c 7973 6973 2e70 6879 7369 6361 6c5f  alysis.physical_
-00000b50: 6461 7461 2e5f 5f69 6e69 745f 5f94 7d94  data.__init__.}.
-00000b60: 2868 184b 0068 194b 0068 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
-00000b70: 0068 1c4b 0068 1d4b 0268 1e4b 0075 8c23  .h.K.h.K.h.K.u.#
-00000b80: 5051 416e 616c 7973 6973 2e61 746f 6d69  PQAnalysis.atomi
-00000b90: 635f 7379 7374 656d 2e65 7863 6570 7469  c_system.excepti
-00000ba0: 6f6e 7394 7d94 2868 184b 0068 194b 0068  ons.}.(h.K.h.K.h
-00000bb0: 1a4b 0068 1b4b 0068 1c4b 0068 1d4b 1268  .K.h.K.h.K.h.K.h
-00000bc0: 1e4b 0075 8c24 5051 416e 616c 7973 6973  .K.u.$PQAnalysis
-00000bd0: 2e61 746f 6d69 635f 7379 7374 656d 2e5f  .atomic_system._
-00000be0: 6465 636f 7261 746f 7273 947d 9428 6818  decorators.}.(h.
-00000bf0: 4b00 6819 4b00 681a 4b00 681b 4b00 681c  K.h.K.h.K.h.K.h.
-00000c00: 4b00 681d 4b18 681e 4b00 758c 2650 5141  K.h.K.h.K.u.&PQA
-00000c10: 6e61 6c79 7369 732e 6174 6f6d 6963 5f73  nalysis.atomic_s
-00000c20: 7973 7465 6d2e 6174 6f6d 6963 5f73 7973  ystem.atomic_sys
-00000c30: 7465 6d94 7d94 2868 184b 0068 194b 0068  tem.}.(h.K.h.K.h
-00000c40: 1a4b 0068 1b4b 0068 1c4b 0668 1d4b a568  .K.h.K.h.K.h.K.h
-00000c50: 1e4b 0175 8c21 5051 416e 616c 7973 6973  .K.u.!PQAnalysis
-00000c60: 2e61 746f 6d69 635f 7379 7374 656d 2e5f  .atomic_system._
-00000c70: 5f69 6e69 745f 5f94 7d94 2868 184b 0068  _init__.}.(h.K.h
-00000c80: 194b 0068 1a4b 0068 1b4b 0068 1c4b 0068  .K.h.K.h.K.h.K.h
-00000c90: 1d4b 0268 1e4b 0075 8c24 5051 416e 616c  .K.h.K.u.$PQAnal
-00000ca0: 7973 6973 2e61 746f 6d69 635f 7379 7374  ysis.atomic_syst
-00000cb0: 656d 2e5f 7072 6f70 6572 7469 6573 947d  em._properties.}
-00000cc0: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
-00000cd0: 4b00 681c 4b00 681d 4b28 681e 4b00 758c  K.h.K.h.K(h.K.u.
-00000ce0: 2350 5141 6e61 6c79 7369 732e 6174 6f6d  #PQAnalysis.atom
-00000cf0: 6963 5f73 7973 7465 6d2e 5f70 6f73 6974  ic_system._posit
-00000d00: 696f 6e73 947d 9428 6818 4b00 6819 4b00  ions.}.(h.K.h.K.
-00000d10: 681a 4b00 681b 4b00 681c 4b00 681d 4b19  h.K.h.K.h.K.h.K.
-00000d20: 681e 4b00 758c 2d50 5141 6e61 6c79 7369  h.K.u.-PQAnalysi
-00000d30: 732e 6174 6f6d 6963 5f73 7973 7465 6d2e  s.atomic_system.
-00000d40: 5f73 7461 6e64 6172 645f 7072 6f70 6572  _standard_proper
-00000d50: 7469 6573 947d 9428 6818 4b00 6819 4b00  ties.}.(h.K.h.K.
-00000d60: 681a 4b00 681b 4b00 681c 4b02 681d 4b44  h.K.h.K.h.K.h.KD
-00000d70: 681e 4b00 758c 1a50 5141 6e61 6c79 7369  h.K.u..PQAnalysi
-00000d80: 732e 7472 616a 2e65 7863 6570 7469 6f6e  s.traj.exception
-00000d90: 7394 7d94 2868 184b 0068 194b 0068 1a4b  s.}.(h.K.h.K.h.K
-00000da0: 0068 1b4b 0068 1c4b 0068 1d4b 0768 1e4b  .h.K.h.K.h.K.h.K
-00000db0: 0075 8c17 5051 416e 616c 7973 6973 2e74  .u..PQAnalysis.t
-00000dc0: 7261 6a2e 666f 726d 6174 7394 7d94 2868  raj.formats.}.(h
-00000dd0: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
-00000de0: 1c4b 0168 1d4b 2d68 1e4b 0075 8c13 5051  .K.h.K-h.K.u..PQ
-00000df0: 416e 616c 7973 6973 2e74 7261 6a2e 6170  Analysis.traj.ap
-00000e00: 6994 7d94 2868 184b 0068 194b 0068 1a4b  i.}.(h.K.h.K.h.K
-00000e10: 0068 1b4b 0068 1c4b 0068 1d4b 0868 1e4b  .h.K.h.K.h.K.h.K
-00000e20: 0075 8c1a 5051 416e 616c 7973 6973 2e74  .u..PQAnalysis.t
-00000e30: 7261 6a2e 7472 616a 6563 746f 7279 947d  raj.trajectory.}
-00000e40: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
-00000e50: 4b00 681c 4b00 681d 4b66 681e 4b00 758c  K.h.K.h.Kfh.K.u.
-00000e60: 1850 5141 6e61 6c79 7369 732e 7472 616a  .PQAnalysis.traj
-00000e70: 2e5f 5f69 6e69 745f 5f94 7d94 2868 184b  .__init__.}.(h.K
-00000e80: 0068 194b 0068 1a4b 0068 1b4b 0068 1c4b  .h.K.h.K.h.K.h.K
-00000e90: 0068 1d4b 0468 1e4b 0075 8c1a 5051 416e  .h.K.h.K.u..PQAn
-00000ea0: 616c 7973 6973 2e63 6f72 652e 6578 6365  alysis.core.exce
-00000eb0: 7074 696f 6e73 947d 9428 6818 4b00 6819  ptions.}.(h.K.h.
-00000ec0: 4b00 681a 4b00 681b 4b00 681c 4b00 681d  K.h.K.h.K.h.K.h.
-00000ed0: 4b10 681e 4b00 758c 1350 5141 6e61 6c79  K.h.K.u..PQAnaly
-00000ee0: 7369 732e 636f 7265 2e61 7069 947d 9428  sis.core.api.}.(
-00000ef0: 6818 4b00 6819 4b00 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
-00000f00: 681c 4b00 681d 4b09 681e 4b01 758c 1750  h.K.h.K.h.K.u..P
-00000f10: 5141 6e61 6c79 7369 732e 636f 7265 2e72  QAnalysis.core.r
-00000f20: 6573 6964 7565 947d 9428 6818 4b00 6819  esidue.}.(h.K.h.
-00000f30: 4b00 681a 4b00 681b 4b00 681c 4b02 681d  K.h.K.h.K.h.K.h.
-00000f40: 4b50 681e 4b00 758c 1850 5141 6e61 6c79  KPh.K.u..PQAnaly
-00000f50: 7369 732e 636f 7265 2e5f 5f69 6e69 745f  sis.core.__init_
-00000f60: 5f94 7d94 2868 184b 0068 194b 0068 1a4b  _.}.(h.K.h.K.h.K
-00000f70: 0068 1b4b 0068 1c4b 0068 1d4b 0568 1e4b  .h.K.h.K.h.K.h.K
-00000f80: 0075 8c1d 5051 416e 616c 7973 6973 2e63  .u..PQAnalysis.c
-00000f90: 6f72 652e 6174 6f6d 2e5f 5f69 6e69 745f  ore.atom.__init_
-00000fa0: 5f94 7d94 2868 184b 0068 194b 0068 1a4b  _.}.(h.K.h.K.h.K
-00000fb0: 0068 1b4b 0068 1c4b 0068 1d4b 0268 1e4b  .h.K.h.K.h.K.h.K
-00000fc0: 0075 8c19 5051 416e 616c 7973 6973 2e63  .u..PQAnalysis.c
-00000fd0: 6f72 652e 6174 6f6d 2e61 746f 6d94 7d94  ore.atom.atom.}.
-00000fe0: 2868 184b 0068 194b 0068 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
-00000ff0: 0068 1c4b 0068 1d4b 3968 1e4b 0075 8c1c  .h.K.h.K9h.K.u..
-00001000: 5051 416e 616c 7973 6973 2e63 6f72 652e  PQAnalysis.core.
-00001010: 6174 6f6d 2e65 6c65 6d65 6e74 947d 9428  atom.element.}.(
-00001020: 6818 4b00 6819 4b00 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
-00001030: 681c 4b00 681d 4b34 681e 4b00 758c 1950  h.K.h.K4h.K.u..P
-00001040: 5141 6e61 6c79 7369 732e 636f 7265 2e63  QAnalysis.core.c
-00001050: 656c 6c2e 6365 6c6c 947d 9428 6818 4b00  ell.cell.}.(h.K.
-00001060: 6819 4b00 681a 4b00 681b 4b00 681c 4b01  h.K.h.K.h.K.h.K.
-00001070: 681d 4b53 681e 4b00 758c 1d50 5141 6e61  h.KSh.K.u..PQAna
-00001080: 6c79 7369 732e 636f 7265 2e63 656c 6c2e  lysis.core.cell.
-00001090: 5f5f 696e 6974 5f5f 947d 9428 6818 4b00  __init__.}.(h.K.
-000010a0: 6819 4b00 681a 4b00 681b 4b00 681c 4b00  h.K.h.K.h.K.h.K.
-000010b0: 681d 4b01 681e 4b00 758c 2950 5141 6e61  h.K.h.K.u.)PQAna
-000010c0: 6c79 7369 732e 636f 7265 2e63 656c 6c2e  lysis.core.cell.
-000010d0: 5f73 7461 6e64 6172 645f 7072 6f70 6572  _standard_proper
-000010e0: 7469 6573 947d 9428 6818 4b00 6819 4b00  ties.}.(h.K.h.K.
-000010f0: 681a 4b00 681b 4b00 681c 4b00 681d 4b24  h.K.h.K.h.K.h.K$
-00001100: 681e 4b00 758c 1e50 5141 6e61 6c79 7369  h.K.u..PQAnalysi
-00001110: 732e 746f 706f 6c6f 6779 2e65 7863 6570  s.topology.excep
-00001120: 7469 6f6e 7394 7d94 2868 184b 0068 194b  tions.}.(h.K.h.K
-00001130: 0068 1a4b 0068 1b4b 0068 1c4b 0068 1d4b  .h.K.h.K.h.K.h.K
-00001140: 0568 1e4b 0075 8c1c 5051 416e 616c 7973  .h.K.u..PQAnalys
-00001150: 6973 2e74 6f70 6f6c 6f67 792e 746f 706f  is.topology.topo
-00001160: 6c6f 6779 947d 9428 6818 4b00 6819 4b00  logy.}.(h.K.h.K.
-00001170: 681a 4b00 681b 4b00 681c 4b02 681d 4ba7  h.K.h.K.h.K.h.K.
-00001180: 681e 4b00 758c 1750 5141 6e61 6c79 7369  h.K.u..PQAnalysi
-00001190: 732e 746f 706f 6c6f 6779 2e61 7069 947d  s.topology.api.}
-000011a0: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
-000011b0: 4b00 681c 4b00 681d 4b11 681e 4b00 758c  K.h.K.h.K.h.K.u.
-000011c0: 1c50 5141 6e61 6c79 7369 732e 746f 706f  .PQAnalysis.topo
-000011d0: 6c6f 6779 2e5f 5f69 6e69 745f 5f94 7d94  logy.__init__.}.
-000011e0: 2868 184b 0068 194b 0068 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
-000011f0: 0068 1c4b 0068 1d4b 0768 1e4b 0275 8c1d  .h.K.h.K.h.K.u..
-00001200: 5051 416e 616c 7973 6973 2e74 6f70 6f6c  PQAnalysis.topol
-00001210: 6f67 792e 7365 6c65 6374 696f 6e94 7d94  ogy.selection.}.
-00001220: 2868 184b 0068 194b 0068 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
-00001230: 0068 1c4b 0168 1d4b 9268 1e4b 0075 8c22  .h.K.h.K.h.K.u."
-00001240: 5051 416e 616c 7973 6973 2e74 6f70 6f6c  PQAnalysis.topol
-00001250: 6f67 792e 7368 616b 655f 746f 706f 6c6f  ogy.shake_topolo
-00001260: 6779 947d 9428 6818 4b00 6819 4b00 681a  gy.}.(h.K.h.K.h.
-00001270: 4b00 681b 4b00 681c 4b00 681d 4b48 681e  K.h.K.h.K.h.KHh.
-00001280: 4b00 758c 2c50 5141 6e61 6c79 7369 732e  K.u.,PQAnalysis.
-00001290: 746f 706f 6c6f 6779 2e62 6f6e 6465 645f  topology.bonded_
-000012a0: 746f 706f 6c6f 6779 2e64 6968 6564 7261  topology.dihedra
-000012b0: 6c94 7d94 2868 184b 0068 194b 0068 1a4b  l.}.(h.K.h.K.h.K
-000012c0: 0068 1b4b 0068 1c4b 0268 1d4b 1268 1e4b  .h.K.h.K.h.K.h.K
-000012d0: 0075 8c38 5051 416e 616c 7973 6973 2e74  .u.8PQAnalysis.t
-000012e0: 6f70 6f6c 6f67 792e 626f 6e64 6564 5f74  opology.bonded_t
-000012f0: 6f70 6f6c 6f67 792e 5f74 6f70 6f6c 6f67  opology._topolog
-00001300: 795f 7072 6f70 6572 7469 6573 947d 9428  y_properties.}.(
-00001310: 6818 4b00 6819 4b00 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
-00001320: 681c 4b00 681d 4b2e 681e 4b00 758c 2c50  h.K.h.K.h.K.u.,P
-00001330: 5141 6e61 6c79 7369 732e 746f 706f 6c6f  QAnalysis.topolo
-00001340: 6779 2e62 6f6e 6465 645f 746f 706f 6c6f  gy.bonded_topolo
-00001350: 6779 2e5f 5f69 6e69 745f 5f94 7d94 2868  gy.__init__.}.(h
-00001360: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
-00001370: 1c4b 0068 1d4b 0068 1e4b 0075 8c28 5051  .K.h.K.h.K.u.(PQ
-00001380: 416e 616c 7973 6973 2e74 6f70 6f6c 6f67  Analysis.topolog
-00001390: 792e 626f 6e64 6564 5f74 6f70 6f6c 6f67  y.bonded_topolog
-000013a0: 792e 626f 6e64 947d 9428 6818 4b00 6819  y.bond.}.(h.K.h.
-000013b0: 4b00 681a 4b00 681b 4b00 681c 4b01 681d  K.h.K.h.K.h.K.h.
-000013c0: 4b10 681e 4b00 758c 3350 5141 6e61 6c79  K.h.K.u.3PQAnaly
-000013d0: 7369 732e 746f 706f 6c6f 6779 2e62 6f6e  sis.topology.bon
-000013e0: 6465 645f 746f 706f 6c6f 6779 2e62 6f6e  ded_topology.bon
-000013f0: 6465 645f 746f 706f 6c6f 6779 947d 9428  ded_topology.}.(
-00001400: 6818 4b00 6819 4b00 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
-00001410: 681c 4b01 681d 4b24 681e 4b00 758c 2950  h.K.h.K$h.K.u.)P
-00001420: 5141 6e61 6c79 7369 732e 746f 706f 6c6f  QAnalysis.topolo
-00001430: 6779 2e62 6f6e 6465 645f 746f 706f 6c6f  gy.bonded_topolo
-00001440: 6779 2e61 6e67 6c65 947d 9428 6818 4b00  gy.angle.}.(h.K.
-00001450: 6819 4b00 681a 4b00 681b 4b00 681c 4b01  h.K.h.K.h.K.h.K.
-00001460: 681d 4b10 681e 4b00 758c 1850 5141 6e61  h.K.h.K.u..PQAna
-00001470: 6c79 7369 732e 696f 2e65 7863 6570 7469  lysis.io.excepti
-00001480: 6f6e 7394 7d94 2868 184b 0068 194b 0068  ons.}.(h.K.h.K.h
-00001490: 1a4b 0068 1b4b 0068 1c4b 0068 1d4b 0668  .K.h.K.h.K.h.K.h
-000014a0: 1e4b 0075 8c15 5051 416e 616c 7973 6973  .K.u..PQAnalysis
-000014b0: 2e69 6f2e 666f 726d 6174 7394 7d94 2868  .io.formats.}.(h
-000014c0: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
-000014d0: 1c4b 0168 1d4b 5168 1e4b 0075 8c11 5051  .K.h.KQh.K.u..PQ
-000014e0: 416e 616c 7973 6973 2e69 6f2e 6170 6994  Analysis.io.api.
-000014f0: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
-00001500: 1b4b 0068 1c4b 0068 1d4b 1168 1e4b 0075  .K.h.K.h.K.h.K.u
-00001510: 8c20 5051 416e 616c 7973 6973 2e69 6f2e  . PQAnalysis.io.
-00001520: 656e 6572 6779 5f66 696c 655f 7265 6164  energy_file_read
-00001530: 6572 947d 9428 6818 4b00 6819 4b00 681a  er.}.(h.K.h.K.h.
-00001540: 4b00 681b 4b00 681c 4b00 681d 4b2e 681e  K.h.K.h.K.h.K.h.
-00001550: 4b00 758c 1c50 5141 6e61 6c79 7369 732e  K.u..PQAnalysis.
-00001560: 696f 2e63 6f6e 7665 7273 696f 6e5f 6170  io.conversion_ap
-00001570: 6994 7d94 2868 184b 0068 194b 0068 1a4b  i.}.(h.K.h.K.h.K
-00001580: 0068 1b4b 0068 1c4b 0068 1d4b 2768 1e4b  .h.K.h.K.h.K'h.K
-00001590: 0075 8c12 5051 416e 616c 7973 6973 2e69  .u..PQAnalysis.i
-000015a0: 6f2e 6261 7365 947d 9428 6818 4b00 6819  o.base.}.(h.K.h.
-000015b0: 4b00 681a 4b00 681b 4b00 681c 4b00 681d  K.h.K.h.K.h.K.h.
-000015c0: 4b32 681e 4b00 758c 1e50 5141 6e61 6c79  K2h.K.u..PQAnaly
-000015d0: 7369 732e 696f 2e69 6e66 6f5f 6669 6c65  sis.io.info_file
-000015e0: 5f72 6561 6465 7294 7d94 2868 184b 0068  _reader.}.(h.K.h
-000015f0: 194b 0068 1a4b 0068 1b4b 0068 1c4b 0168  .K.h.K.h.K.h.K.h
-00001600: 1d4b 3768 1e4b 0075 8c16 5051 416e 616c  .K7h.K.u..PQAnal
-00001610: 7973 6973 2e69 6f2e 5f5f 696e 6974 5f5f  ysis.io.__init__
-00001620: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
-00001630: 681b 4b00 681c 4b00 681d 4b1a 681e 4b00  h.K.h.K.h.K.h.K.
-00001640: 758c 1750 5141 6e61 6c79 7369 732e 696f  u..PQAnalysis.io
-00001650: 2e77 7269 7465 5f61 7069 947d 9428 6818  .write_api.}.(h.
-00001660: 4b00 6819 4b00 681a 4b00 681b 4b00 681c  K.h.K.h.K.h.K.h.
-00001670: 4b00 681d 4b14 681e 4b01 758c 1850 5141  K.h.K.h.K.u..PQA
-00001680: 6e61 6c79 7369 732e 696f 2e62 6f78 5f77  nalysis.io.box_w
-00001690: 7269 7465 7294 7d94 2868 184b 0068 194b  riter.}.(h.K.h.K
-000016a0: 0068 1a4b 0068 1b4b 0068 1c4b 0068 1d4b  .h.K.h.K.h.K.h.K
-000016b0: 2c68 1e4b 0075 8c22 5051 416e 616c 7973  ,h.K.u."PQAnalys
-000016c0: 6973 2e69 6f2e 6d6f 6c64 6573 6372 6970  is.io.moldescrip
-000016d0: 746f 725f 7265 6164 6572 947d 9428 6818  tor_reader.}.(h.
-000016e0: 4b00 6819 4b00 681a 4b00 681b 4b00 681c  K.h.K.h.K.h.K.h.
-000016f0: 4b00 681d 4b39 681e 4b02 758c 2250 5141  K.h.K9h.K.u."PQA
-00001700: 6e61 6c79 7369 732e 696f 2e74 7261 6a5f  nalysis.io.traj_
-00001710: 6669 6c65 2e65 7863 6570 7469 6f6e 7394  file.exceptions.
-00001720: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
-00001730: 1b4b 0068 1c4b 0068 1d4b 0368 1e4b 0075  .K.h.K.h.K.h.K.u
-00001740: 8c29 5051 416e 616c 7973 6973 2e69 6f2e  .)PQAnalysis.io.
-00001750: 7472 616a 5f66 696c 652e 7472 616a 6563  traj_file.trajec
-00001760: 746f 7279 5f77 7269 7465 7294 7d94 2868  tory_writer.}.(h
-00001770: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
-00001780: 1c4b 0068 1d4b 4f68 1e4b 0075 8c1b 5051  .K.h.KOh.K.u..PQ
-00001790: 416e 616c 7973 6973 2e69 6f2e 7472 616a  Analysis.io.traj
-000017a0: 5f66 696c 652e 6170 6994 7d94 2868 184b  _file.api.}.(h.K
-000017b0: 0068 194b 0168 1a4b 0068 1b4b 0068 1c4b  .h.K.h.K.h.K.h.K
-000017c0: 0068 1d4b 1368 1e4b 0075 8c20 5051 416e  .h.K.h.K.u. PQAn
-000017d0: 616c 7973 6973 2e69 6f2e 7472 616a 5f66  alysis.io.traj_f
-000017e0: 696c 652e 5f5f 696e 6974 5f5f 947d 9428  ile.__init__.}.(
-000017f0: 6818 4b00 6819 4b00 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
-00001800: 681c 4b00 681d 4b03 681e 4b00 758c 2450  h.K.h.K.h.K.u.$P
-00001810: 5141 6e61 6c79 7369 732e 696f 2e74 7261  QAnalysis.io.tra
-00001820: 6a5f 6669 6c65 2e66 7261 6d65 5f72 6561  j_file.frame_rea
-00001830: 6465 7294 7d94 2868 184b 0068 194b 0268  der.}.(h.K.h.K.h
-00001840: 1a4b 0068 1b4b 0068 1c4b 0268 1d4b 6e68  .K.h.K.h.K.h.Knh
-00001850: 1e4b 0075 8c29 5051 416e 616c 7973 6973  .K.u.)PQAnalysis
-00001860: 2e69 6f2e 7472 616a 5f66 696c 652e 7472  .io.traj_file.tr
-00001870: 616a 6563 746f 7279 5f72 6561 6465 7294  ajectory_reader.
-00001880: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
-00001890: 1b4b 0068 1c4b 0568 1d4b a768 1e4b 0075  .K.h.K.h.K.h.K.u
-000018a0: 8c21 5051 416e 616c 7973 6973 2e69 6f2e  .!PQAnalysis.io.
-000018b0: 6765 6e5f 6669 6c65 2e65 7863 6570 7469  gen_file.excepti
-000018c0: 6f6e 7394 7d94 2868 184b 0068 194b 0068  ons.}.(h.K.h.K.h
-000018d0: 1a4b 0068 1b4b 0068 1c4b 0068 1d4b 0268  .K.h.K.h.K.h.K.h
-000018e0: 1e4b 0075 8c1a 5051 416e 616c 7973 6973  .K.u..PQAnalysis
-000018f0: 2e69 6f2e 6765 6e5f 6669 6c65 2e61 7069  .io.gen_file.api
-00001900: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
-00001910: 681b 4b00 681c 4b00 681d 4b09 681e 4b00  h.K.h.K.h.K.h.K.
-00001920: 758c 1f50 5141 6e61 6c79 7369 732e 696f  u..PQAnalysis.io
-00001930: 2e67 656e 5f66 696c 652e 5f5f 696e 6974  .gen_file.__init
-00001940: 5f5f 947d 9428 6818 4b00 6819 4b00 681a  __.}.(h.K.h.K.h.
-00001950: 4b00 681b 4b00 681c 4b00 681d 4b03 681e  K.h.K.h.K.h.K.h.
-00001960: 4b00 758c 2650 5141 6e61 6c79 7369 732e  K.u.&PQAnalysis.
-00001970: 696f 2e67 656e 5f66 696c 652e 6765 6e5f  io.gen_file.gen_
-00001980: 6669 6c65 5f77 7269 7465 7294 7d94 2868  file_writer.}.(h
-00001990: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
-000019a0: 1c4b 0068 1d4b 2c68 1e4b 0075 8c26 5051  .K.h.K,h.K.u.&PQ
-000019b0: 416e 616c 7973 6973 2e69 6f2e 6765 6e5f  Analysis.io.gen_
-000019c0: 6669 6c65 2e67 656e 5f66 696c 655f 7265  file.gen_file_re
-000019d0: 6164 6572 947d 9428 6818 4b00 6819 4b01  ader.}.(h.K.h.K.
-000019e0: 681a 4b00 681b 4b00 681c 4b00 681d 4b2f  h.K.h.K.h.K.h.K/
-000019f0: 681e 4b00 758c 1850 5141 6e61 6c79 7369  h.K.u..PQAnalysi
-00001a00: 732e 696f 2e76 6972 6961 6c2e 6170 6994  s.io.virial.api.
-00001a10: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
-00001a20: 1b4b 0068 1c4b 0068 1d4b 0968 1e4b 0075  .K.h.K.h.K.h.K.u
-00001a30: 8c1d 5051 416e 616c 7973 6973 2e69 6f2e  ..PQAnalysis.io.
-00001a40: 7669 7269 616c 2e5f 5f69 6e69 745f 5f94  virial.__init__.
-00001a50: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
-00001a60: 1b4b 0068 1c4b 0068 1d4b 0168 1e4b 0075  .K.h.K.h.K.h.K.u
-00001a70: 8c22 5051 416e 616c 7973 6973 2e69 6f2e  ."PQAnalysis.io.
-00001a80: 7669 7269 616c 2e76 6972 6961 6c5f 7265  virial.virial_re
-00001a90: 6164 6572 947d 9428 6818 4b00 6819 4b00  ader.}.(h.K.h.K.
-00001aa0: 681a 4b00 681b 4b00 681c 4b00 681d 4b14  h.K.h.K.h.K.h.K.
-00001ab0: 681e 4b00 758c 2650 5141 6e61 6c79 7369  h.K.u.&PQAnalysi
-00001ac0: 732e 696f 2e74 6f70 6f6c 6f67 795f 6669  s.io.topology_fi
-00001ad0: 6c65 2e65 7863 6570 7469 6f6e 7394 7d94  le.exceptions.}.
-00001ae0: 2868 184b 0068 194b 0068 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
-00001af0: 0068 1c4b 0068 1d4b 0268 1e4b 0075 8c1f  .h.K.h.K.h.K.u..
-00001b00: 5051 416e 616c 7973 6973 2e69 6f2e 746f  PQAnalysis.io.to
-00001b10: 706f 6c6f 6779 5f66 696c 652e 6170 6994  pology_file.api.
-00001b20: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
-00001b30: 1b4b 0068 1c4b 0068 1d4b 0968 1e4b 0075  .K.h.K.h.K.h.K.u
-00001b40: 8c30 5051 416e 616c 7973 6973 2e69 6f2e  .0PQAnalysis.io.
-00001b50: 746f 706f 6c6f 6779 5f66 696c 652e 746f  topology_file.to
-00001b60: 706f 6c6f 6779 5f66 696c 655f 7265 6164  pology_file_read
-00001b70: 6572 947d 9428 6818 4b00 6819 4b15 681a  er.}.(h.K.h.K.h.
-00001b80: 4b00 681b 4b00 681c 4b00 681d 4b71 681e  K.h.K.h.K.h.Kqh.
-00001b90: 4b00 758c 2450 5141 6e61 6c79 7369 732e  K.u.$PQAnalysis.
-00001ba0: 696f 2e74 6f70 6f6c 6f67 795f 6669 6c65  io.topology_file
-00001bb0: 2e5f 5f69 6e69 745f 5f94 7d94 2868 184b  .__init__.}.(h.K
-00001bc0: 0068 194b 0068 1a4b 0068 1b4b 0068 1c4b  .h.K.h.K.h.K.h.K
-00001bd0: 0068 1d4b 0268 1e4b 0075 8c30 5051 416e  .h.K.h.K.u.0PQAn
-00001be0: 616c 7973 6973 2e69 6f2e 746f 706f 6c6f  alysis.io.topolo
-00001bf0: 6779 5f66 696c 652e 746f 706f 6c6f 6779  gy_file.topology
-00001c00: 5f66 696c 655f 7772 6974 6572 947d 9428  _file_writer.}.(
-00001c10: 6818 4b00 6819 4b00 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
-00001c20: 681c 4b00 681d 4b6b 681e 4b00 758c 2550  h.K.h.Kkh.K.u.%P
-00001c30: 5141 6e61 6c79 7369 732e 696f 2e72 6573  QAnalysis.io.res
-00001c40: 7461 7274 5f66 696c 652e 6578 6365 7074  tart_file.except
-00001c50: 696f 6e73 947d 9428 6818 4b00 6819 4b00  ions.}.(h.K.h.K.
-00001c60: 681a 4b00 681b 4b00 681c 4b00 681d 4b03  h.K.h.K.h.K.h.K.
-00001c70: 681e 4b00 758c 2950 5141 6e61 6c79 7369  h.K.u.)PQAnalysi
-00001c80: 732e 696f 2e72 6573 7461 7274 5f66 696c  s.io.restart_fil
-00001c90: 652e 7265 7374 6172 745f 7265 6164 6572  e.restart_reader
-00001ca0: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
-00001cb0: 681b 4b00 681c 4b01 681d 4b49 681e 4b00  h.K.h.K.h.KIh.K.
-00001cc0: 758c 2950 5141 6e61 6c79 7369 732e 696f  u.)PQAnalysis.io
-00001cd0: 2e72 6573 7461 7274 5f66 696c 652e 7265  .restart_file.re
-00001ce0: 7374 6172 745f 7772 6974 6572 947d 9428  start_writer.}.(
-00001cf0: 6818 4b00 6819 4b00 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
-00001d00: 681c 4b00 681d 4b3d 681e 4b00 758c 1e50  h.K.h.K=h.K.u..P
-00001d10: 5141 6e61 6c79 7369 732e 696f 2e72 6573  QAnalysis.io.res
-00001d20: 7461 7274 5f66 696c 652e 6170 6994 7d94  tart_file.api.}.
-00001d30: 2868 184b 0068 194b 0068 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
-00001d40: 0068 1c4b 0068 1d4b 0868 1e4b 0075 8c23  .h.K.h.K.h.K.u.#
-00001d50: 5051 416e 616c 7973 6973 2e69 6f2e 7265  PQAnalysis.io.re
-00001d60: 7374 6172 745f 6669 6c65 2e5f 5f69 6e69  start_file.__ini
-00001d70: 745f 5f94 7d94 2868 184b 0068 194b 0068  t__.}.(h.K.h.K.h
-00001d80: 1a4b 0068 1b4b 0068 1c4b 0068 1d4b 0268  .K.h.K.h.K.h.K.h
-00001d90: 1e4b 0075 8c2a 5051 416e 616c 7973 6973  .K.u.*PQAnalysis
-00001da0: 2e69 6f2e 696e 7075 745f 6669 6c65 5f72  .io.input_file_r
-00001db0: 6561 6465 722e 6578 6365 7074 696f 6e73  eader.exceptions
-00001dc0: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
-00001dd0: 681b 4b00 681c 4b00 681d 4b0e 681e 4b00  h.K.h.K.h.K.h.K.
-00001de0: 758c 2750 5141 6e61 6c79 7369 732e 696f  u.'PQAnalysis.io
-00001df0: 2e69 6e70 7574 5f66 696c 655f 7265 6164  .input_file_read
-00001e00: 6572 2e66 6f72 6d61 7473 947d 9428 6818  er.formats.}.(h.
-00001e10: 4b00 6819 4b00 681a 4b00 681b 4b00 681c  K.h.K.h.K.h.K.h.
-00001e20: 4b00 681d 4b0f 681e 4b00 758c 2850 5141  K.h.K.h.K.u.(PQA
-00001e30: 6e61 6c79 7369 732e 696f 2e69 6e70 7574  nalysis.io.input
-00001e40: 5f66 696c 655f 7265 6164 6572 2e5f 5f69  _file_reader.__i
-00001e50: 6e69 745f 5f94 7d94 2868 184b 0068 194b  nit__.}.(h.K.h.K
-00001e60: 0068 1a4b 0068 1b4b 0068 1c4b 0068 1d4b  .h.K.h.K.h.K.h.K
-00001e70: 0468 1e4b 0075 8c31 5051 416e 616c 7973  .h.K.u.1PQAnalys
-00001e80: 6973 2e69 6f2e 696e 7075 745f 6669 6c65  is.io.input_file
-00001e90: 5f72 6561 6465 722e 696e 7075 745f 6669  _reader.input_fi
-00001ea0: 6c65 5f70 6172 7365 7294 7d94 2868 184b  le_parser.}.(h.K
-00001eb0: 0068 194b 0168 1a4b 0068 1b4b 0068 1c4b  .h.K.h.K.h.K.h.K
-00001ec0: 0168 1d4b 7f68 1e4b 0075 8c32 5051 416e  .h.K.h.K.u.2PQAn
-00001ed0: 616c 7973 6973 2e69 6f2e 696e 7075 745f  alysis.io.input_
-00001ee0: 6669 6c65 5f72 6561 6465 722e 7071 5f61  file_reader.pq_a
-00001ef0: 6e61 6c79 7369 732e 5f70 6172 7365 947d  nalysis._parse.}
-00001f00: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
-00001f10: 4b00 681c 4b01 681d 4b44 681e 4b00 758c  K.h.K.h.KDh.K.u.
-00001f20: 3450 5141 6e61 6c79 7369 732e 696f 2e69  4PQAnalysis.io.i
-00001f30: 6e70 7574 5f66 696c 655f 7265 6164 6572  nput_file_reader
-00001f40: 2e70 715f 616e 616c 7973 6973 2e5f 5f69  .pq_analysis.__i
-00001f50: 6e69 745f 5f94 7d94 2868 184b 0068 194b  nit__.}.(h.K.h.K
-00001f60: 0068 1a4b 0068 1b4b 0068 1c4b 0068 1d4b  .h.K.h.K.h.K.h.K
-00001f70: 0168 1e4b 0075 8c48 5051 416e 616c 7973  .h.K.u.HPQAnalys
-00001f80: 6973 2e69 6f2e 696e 7075 745f 6669 6c65  is.io.input_file
-00001f90: 5f72 6561 6465 722e 7071 5f61 6e61 6c79  _reader.pq_analy
-00001fa0: 7369 732e 7071 616e 616c 7973 6973 5f69  sis.pqanalysis_i
-00001fb0: 6e70 7574 5f66 696c 655f 7265 6164 6572  nput_file_reader
-00001fc0: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
-00001fd0: 681b 4b00 681c 4b00 681d 4b3b 681e 4b00  h.K.h.K.h.K;h.K.
-00001fe0: 758c 3c50 5141 6e61 6c79 7369 732e 696f  u.<PQAnalysis.io
-00001ff0: 2e69 6e70 7574 5f66 696c 655f 7265 6164  .input_file_read
-00002000: 6572 2e70 715f 616e 616c 7973 6973 2e5f  er.pq_analysis._
-00002010: 7365 6c65 6374 696f 6e5f 6d69 7869 6e94  selection_mixin.
-00002020: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
-00002030: 1b4b 0068 1c4b 0068 1d4b 0c68 1e4b 0075  .K.h.K.h.K.h.K.u
-00002040: 8c3c 5051 416e 616c 7973 6973 2e69 6f2e  .<PQAnalysis.io.
-00002050: 696e 7075 745f 6669 6c65 5f72 6561 6465  input_file_reade
-00002060: 722e 7071 5f61 6e61 6c79 7369 732e 5f70  r.pq_analysis._p
-00002070: 6f73 6974 696f 6e73 5f6d 6978 696e 947d  ositions_mixin.}
-00002080: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
-00002090: 4b00 681c 4b00 681d 4b0b 681e 4b00 758c  K.h.K.h.K.h.K.u.
-000020a0: 3750 5141 6e61 6c79 7369 732e 696f 2e69  7PQAnalysis.io.i
-000020b0: 6e70 7574 5f66 696c 655f 7265 6164 6572  nput_file_reader
-000020c0: 2e70 715f 616e 616c 7973 6973 2e5f 6669  .pq_analysis._fi
-000020d0: 6c65 5f6d 6978 696e 947d 9428 6818 4b00  le_mixin.}.(h.K.
-000020e0: 6819 4b00 681a 4b00 681b 4b00 681c 4b00  h.K.h.K.h.K.h.K.
-000020f0: 681d 4b0d 681e 4b00 758c 3750 5141 6e61  h.K.h.K.u.7PQAna
-00002100: 6c79 7369 732e 696f 2e69 6e70 7574 5f66  lysis.io.input_f
-00002110: 696c 655f 7265 6164 6572 2e70 712e 7071  ile_reader.pq.pq
-00002120: 5f69 6e70 7574 5f66 696c 655f 7265 6164  _input_file_read
-00002130: 6572 947d 9428 6818 4b00 6819 4b00 681a  er.}.(h.K.h.K.h.
-00002140: 4b00 681b 4b00 681c 4b01 681d 4b58 681e  K.h.K.h.K.h.KXh.
-00002150: 4b00 758c 2b50 5141 6e61 6c79 7369 732e  K.u.+PQAnalysis.
-00002160: 696f 2e69 6e70 7574 5f66 696c 655f 7265  io.input_file_re
-00002170: 6164 6572 2e70 712e 5f5f 696e 6974 5f5f  ader.pq.__init__
-00002180: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
-00002190: 681b 4b00 681c 4b00 681d 4b01 681e 4b00  h.K.h.K.h.K.h.K.
-000021a0: 758c 2f50 5141 6e61 6c79 7369 732e 696f  u./PQAnalysis.io
-000021b0: 2e69 6e70 7574 5f66 696c 655f 7265 6164  .input_file_read
-000021c0: 6572 2e70 712e 6f75 7470 7574 5f66 696c  er.pq.output_fil
-000021d0: 6573 947d 9428 6818 4b00 6819 4b00 681a  es.}.(h.K.h.K.h.
-000021e0: 4b00 681b 4b00 681c 4b00 681d 4b32 681e  K.h.K.h.K.h.K2h.
-000021f0: 4b00 758c 1c50 5141 6e61 6c79 7369 732e  K.u..PQAnalysis.
-00002200: 696f 2e6e 6570 2e65 7863 6570 7469 6f6e  io.nep.exception
-00002210: 7394 7d94 2868 184b 0068 194b 0068 1a4b  s.}.(h.K.h.K.h.K
-00002220: 0068 1b4b 0068 1c4b 0068 1d4b 0268 1e4b  .h.K.h.K.h.K.h.K
-00002230: 0075 8c1a 5051 416e 616c 7973 6973 2e69  .u..PQAnalysis.i
-00002240: 6f2e 6e65 702e 5f5f 696e 6974 5f5f 947d  o.nep.__init__.}
-00002250: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
-00002260: 4b00 681c 4b00 681d 4b00 681e 4b00 758c  K.h.K.h.K.h.K.u.
-00002270: 1c50 5141 6e61 6c79 7369 732e 696f 2e6e  .PQAnalysis.io.n
-00002280: 6570 2e6e 6570 5f77 7269 7465 7294 7d94  ep.nep_writer.}.
-00002290: 2868 184b 0168 194b 0468 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
-000022a0: 0068 1c4b 0b68 1d4d 1601 681e 4b00 7575  .h.K.h.M..h.K.uu
-000022b0: 8c06 6279 5f6d 7367 947d 9428 8c05 6669  ..by_msg.}.(..fi
-000022c0: 786d 6594 4b09 8c1f 706f 7373 6962 6c79  xme.K...possibly
-000022d0: 2d75 7365 642d 6265 666f 7265 2d61 7373  -used-before-ass
-000022e0: 6967 6e6d 656e 7494 4b1e 8c1c 746f 6f2d  ignment.K...too-
-000022f0: 6d61 6e79 2d69 6e73 7461 6e63 652d 6174  many-instance-at
-00002300: 7472 6962 7574 6573 944b 0a8c 1274 6f6f  tributes.K...too
-00002310: 2d6d 616e 792d 6172 6775 6d65 6e74 7394  -many-arguments.
-00002320: 4b12 8c0f 746f 6f2d 6d61 6e79 2d6c 6f63  K...too-many-loc
-00002330: 616c 7394 4b03 8c1a 746f 6f2d 6d61 6e79  als.K...too-many
-00002340: 2d72 6574 7572 6e2d 7374 6174 656d 656e  -return-statemen
-00002350: 7473 944b 018c 1774 6f6f 2d6d 616e 792d  ts.K...too-many-
-00002360: 7075 626c 6963 2d6d 6574 686f 6473 944b  public-methods.K
-00002370: 018c 1e69 6e63 6f6e 7369 7374 656e 742d  ...inconsistent-
-00002380: 7265 7475 726e 2d73 7461 7465 6d65 6e74  return-statement
-00002390: 7394 4b09 8c0f 756e 7573 6564 2d61 7267  s.K...unused-arg
-000023a0: 756d 656e 7494 4b01 8c09 6e6f 2d6d 656d  ument.K...no-mem
-000023b0: 6265 7294 4b01 8c0b 746f 6f2d 636f 6d70  ber.K...too-comp
-000023c0: 6c65 7894 4b03 8c11 746f 6f2d 6d61 6e79  lex.K...too-many
-000023d0: 2d62 7261 6e63 6865 7394 4b02 8c0e 746f  -branches.K...to
-000023e0: 6f2d 6d61 6e79 2d6c 696e 6573 944b 018c  o-many-lines.K..
-000023f0: 1374 6f6f 2d6d 616e 792d 7374 6174 656d  .too-many-statem
-00002400: 656e 7473 944b 018c 0e64 7570 6c69 6361  ents.K...duplica
-00002410: 7465 2d63 6f64 6594 4b03 758c 0f63 6f64  te-code.K.u..cod
-00002420: 655f 7479 7065 5f63 6f75 6e74 947d 9428  e_type_count.}.(
-00002430: 8c04 636f 6465 944d 811e 8c07 636f 6d6d  ..code.M....comm
-00002440: 656e 7494 4d09 018c 0964 6f63 7374 7269  ent.M....docstri
-00002450: 6e67 944d 9621 8c05 656d 7074 7994 4d36  ng.M.!..empty.M6
-00002460: 0b8c 0574 6f74 616c 944d 564c 758c 0c64  ...total.MVLu..d
-00002470: 6570 656e 6465 6e63 6965 7394 7d94 288c  ependencies.}.(.
-00002480: 0d62 6561 7274 7970 652e 636c 6177 948f  .beartype.claw..
-00002490: 9428 6823 908c 1150 5141 6e61 6c79 7369  .(h#...PQAnalysi
-000024a0: 732e 636f 6e66 6967 948f 9428 6869 686b  s.config...(hihk
-000024b0: 6855 685d 6857 68d7 685b 6a1b 0100 0068  hUh]hWh.h[j....h
-000024c0: 5368 6568 4568 2368 6768 6168 6368 3790  ShehEh#hghahch7.
-000024d0: 8c1f 5051 416e 616c 7973 6973 2e75 7469  ..PQAnalysis.uti
-000024e0: 6c73 2e63 7573 746f 6d5f 6c6f 6767 696e  ls.custom_loggin
-000024f0: 6794 8f94 2868 b968 ed68 f18c 2950 5141  g...(h.h.h..)PQA
-00002500: 6e61 6c79 7369 732e 696f 2e72 6573 7461  nalysis.io.resta
-00002510: 7274 5f66 696c 652e 7265 7374 6172 745f  rt_file.restart_
-00002520: 7265 6164 6572 948c 1250 5141 6e61 6c79  reader...PQAnaly
-00002530: 7369 732e 696f 2e62 6173 6594 68d5 6a1b  sis.io.base.h.j.
-00002540: 0100 006a 1101 0000 6851 6897 6a05 0100  ...j....hQh.j...
-00002550: 0068 bb68 4768 b368 c968 2368 6f68 c38c  .h.hGh.h.h#hoh..
-00002560: 4850 5141 6e61 6c79 7369 732e 696f 2e69  HPQAnalysis.io.i
-00002570: 6e70 7574 5f66 696c 655f 7265 6164 6572  nput_file_reader
-00002580: 2e70 715f 616e 616c 7973 6973 2e70 7161  .pq_analysis.pqa
-00002590: 6e61 6c79 7369 735f 696e 7075 745f 6669  nalysis_input_fi
-000025a0: 6c65 5f72 6561 6465 7294 6895 68c7 68a1  le_reader.h.h.h.
-000025b0: 6877 68bd 68d7 68a9 68cb 68a7 68df 6883  hwh.h.h.h.h.h.h.
-000025c0: 6a03 0100 0068 8768 8f68 458c 2650 5141  j....h.h.hE.&PQA
-000025d0: 6e61 6c79 7369 732e 696f 2e67 656e 5f66  nalysis.io.gen_f
-000025e0: 696c 652e 6765 6e5f 6669 6c65 5f72 6561  ile.gen_file_rea
-000025f0: 6465 7294 68f7 682d 908c 0b6d 756c 7469  der.h.h-...multi
-00002600: 6d65 7468 6f64 948f 9428 6825 908c 0f62  method...(h%...b
-00002610: 6561 7274 7970 652e 7479 7069 6e67 948f  eartype.typing..
-00002620: 9428 68b9 68ed 683b 68f1 6a3d 0100 006a  .(h.h.h;h.j=...j
-00002630: 3e01 0000 68d5 6a1b 0100 0068 a368 5168  >...h.j....h.hQh
-00002640: cf68 4368 976a 0501 0000 8c37 5051 416e  .hCh.j.....7PQAn
-00002650: 616c 7973 6973 2e69 6f2e 696e 7075 745f  alysis.io.input_
-00002660: 6669 6c65 5f72 6561 6465 722e 7071 5f61  file_reader.pq_a
-00002670: 6e61 6c79 7369 732e 5f66 696c 655f 6d69  nalysis._file_mi
-00002680: 7869 6e94 68b3 68ad 688b 686f 682b 6869  xin.h.h.h.hoh+hi
-00002690: 68c3 6a3f 0100 0068 9568 c768 2f68 a168  h.j?...h.h.h/h.h
-000026a0: 7768 d768 7568 a968 cb68 a768 998c 2350  wh.huh.h.h.h..#P
-000026b0: 5141 6e61 6c79 7369 732e 6174 6f6d 6963  QAnalysis.atomic
-000026c0: 5f73 7973 7465 6d2e 5f70 6f73 6974 696f  _system._positio
-000026d0: 6e73 9468 e368 ff68 838c 2450 5141 6e61  ns.h.h.h..$PQAna
-000026e0: 6c79 7369 732e 6174 6f6d 6963 5f73 7973  lysis.atomic_sys
-000026f0: 7465 6d2e 5f70 726f 7065 7274 6965 7394  tem._properties.
-00002700: 6829 68bf 6887 6a03 0100 0068 8f68 d168  h)h.h.j....h.h.h
-00002710: 456a 4001 0000 68f7 6837 682d 908c 056e  Ej@...h.h7h-...n
-00002720: 756d 7079 948f 9428 6a3d 0100 0068 3968  umpy...(j=...h9h
-00002730: d56a 1b01 0000 6851 688d 8c29 5051 416e  .j....hQh..)PQAn
-00002740: 616c 7973 6973 2e63 6f72 652e 6365 6c6c  alysis.core.cell
-00002750: 2e5f 7374 616e 6461 7264 5f70 726f 7065  ._standard_prope
-00002760: 7274 6965 7394 686f 682b 682f 68a1 6877  rties.hoh+h/h.hw
-00002770: 68bd 6875 68e7 68a9 68cb 68a7 68df 6899  h.huh.h.h.h.h.h.
-00002780: 6a46 0100 006a 4701 0000 6887 688f 6845  jF...jG...h.h.hE
-00002790: 6a40 0100 0068 f790 8c0d 6265 6172 7479  j@...h....bearty
-000027a0: 7065 2e76 616c 6594 8f94 2868 9768 2b68  pe.vale...(h.h+h
-000027b0: 9990 8c09 6465 636f 7261 746f 7294 8f94  ....decorator...
-000027c0: 2868 7568 3b68 2d90 8c0d 6265 6172 7479  (huh;h-...bearty
-000027d0: 7065 2e64 6f6f 7294 8f94 2868 2d90 8c15  pe.door...(h-...
-000027e0: 5051 416e 616c 7973 6973 2e65 7863 6570  PQAnalysis.excep
-000027f0: 7469 6f6e 7394 8f94 286a 1701 0000 6a3e  tions...(j....j>
-00002800: 0100 0068 f368 7368 fd68 b768 5168 6d6a  ...h.hsh.h.hQhmj
-00002810: 0501 0000 68bb 68cd 68b3 688b 8c2f 5051  ....h.h.h.h../PQ
-00002820: 416e 616c 7973 6973 2e69 6f2e 696e 7075  Analysis.io.inpu
-00002830: 745f 6669 6c65 5f72 6561 6465 722e 7071  t_file_reader.pq
-00002840: 2e6f 7574 7075 745f 6669 6c65 7394 6881  .output_files.h.
-00002850: 6895 68c7 6877 68bd 68d7 68a9 68a7 68df  h.h.hwh.h.h.h.h.
-00002860: 6841 689f 6a03 0100 0068 8768 d968 e96a  hAh.j....h.h.h.j
-00002870: 1101 0000 6837 682d 908c 1050 5141 6e61  ....h7h-...PQAna
-00002880: 6c79 7369 732e 7479 7065 7394 8f94 2868  lysis.types...(h
-00002890: ab68 b568 3968 d56a 1b01 0000 68a3 6a11  .h.h9h.j....h.j.
-000028a0: 0100 0068 5168 cf68 4368 8d6a 4a01 0000  ...hQh.hCh.jJ...
-000028b0: 68bb 6a05 0100 0068 b168 b368 ad68 6f8c  h.j....h.h.h.ho.
-000028c0: 3c50 5141 6e61 6c79 7369 732e 696f 2e69  <PQAnalysis.io.i
-000028d0: 6e70 7574 5f66 696c 655f 7265 6164 6572  nput_file_reader
-000028e0: 2e70 715f 616e 616c 7973 6973 2e5f 706f  .pq_analysis._po
-000028f0: 7369 7469 6f6e 735f 6d69 7869 6e94 8c2d  sitions_mixin..-
-00002900: 5051 416e 616c 7973 6973 2e61 746f 6d69  PQAnalysis.atomi
-00002910: 635f 7379 7374 656d 2e5f 7374 616e 6461  c_system._standa
-00002920: 7264 5f70 726f 7065 7274 6965 7394 68a1  rd_properties.h.
-00002930: 6877 68e7 68a9 68a7 6899 6a46 0100 006a  hwh.h.h.h.jF...j
-00002940: 4701 0000 6a03 0100 0068 8768 8f68 456a  G...j....h.h.hEj
-00002950: 4001 0000 68f7 682d 908c 1750 5141 6e61  @...h.h-...PQAna
-00002960: 6c79 7369 732e 7574 696c 732e 636f 6d6d  lysis.utils.comm
-00002970: 6f6e 948f 9428 8c10 5051 416e 616c 7973  on...(..PQAnalys
-00002980: 6973 2e75 7469 6c73 9468 6990 8c1b 5051  is.utils.hi...PQ
-00002990: 416e 616c 7973 6973 2e75 7469 6c73 2e64  Analysis.utils.d
-000029a0: 6563 6f72 6174 6f72 7394 8f94 286a 5a01  ecorators...(jZ.
-000029b0: 0000 908c 1350 5141 6e61 6c79 7369 732e  .....PQAnalysis.
-000029c0: 5f76 6572 7369 6f6e 948f 9428 6835 6869  _version...(h5hi
-000029d0: 908c 1050 5141 6e61 6c79 7369 732e 7574  ...PQAnalysis.ut
-000029e0: 696c 7394 8f94 2868 4368 c98c 0e50 5141  ils...(hCh...PQA
-000029f0: 6e61 6c79 7369 732e 636c 6994 6845 6837  nalysis.cli.hEh7
-00002a00: 908c 1750 5141 6e61 6c79 7369 732e 616e  ...PQAnalysis.an
-00002a10: 616c 7973 6973 2e72 6466 948f 9428 8c13  alysis.rdf...(..
-00002a20: 5051 416e 616c 7973 6973 2e61 6e61 6c79  PQAnalysis.analy
-00002a30: 7369 7394 908c 1b50 5141 6e61 6c79 7369  sis....PQAnalysi
-00002a40: 732e 616e 616c 7973 6973 2e72 6466 2e72  s.analysis.rdf.r
-00002a50: 6466 948f 9428 6843 6a64 0100 0068 5368  df...(hCjd...hSh
-00002a60: 498c 1750 5141 6e61 6c79 7369 732e 616e  I..PQAnalysis.an
-00002a70: 616c 7973 6973 2e72 6466 9490 8c0d 5051  alysis.rdf....PQ
-00002a80: 416e 616c 7973 6973 2e69 6f94 8f94 2868  Analysis.io...(h
-00002a90: 4368 6b68 5768 4768 5b68 a968 e76a 1b01  ChkhWhGh[h.h.j..
-00002aa0: 0000 68a3 6865 6851 6845 6861 6863 6849  ..h.hehQhEhahchI
-00002ab0: 908c 1850 5141 6e61 6c79 7369 732e 7479  ...PQAnalysis.ty
-00002ac0: 7065 5f63 6865 636b 696e 6794 8f94 2868  pe_checking...(h
-00002ad0: ab68 ed68 f16a 3d01 0000 68b5 6a1b 0100  .h.h.j=...h.j...
-00002ae0: 0068 a368 5168 cf68 4368 8d68 978c 1e50  .h.hQh.hCh.h...P
-00002af0: 5141 6e61 6c79 7369 732e 696f 2e72 6573  QAnalysis.io.res
-00002b00: 7461 7274 5f66 696c 652e 6170 6994 6a4a  tart_file.api.jJ
-00002b10: 0100 0068 bb68 4768 b168 b368 c968 8568  ...h.hGh.h.h.h.h
-00002b20: 6f68 c368 9568 c76a 5701 0000 68a1 6877  oh.h.h.jW...h.hw
-00002b30: 68bd 68d7 684f 8c1a 5051 416e 616c 7973  h.h.hO..PQAnalys
-00002b40: 6973 2e69 6f2e 6765 6e5f 6669 6c65 2e61  is.io.gen_file.a
-00002b50: 7069 9468 e768 a968 cb68 a768 df68 eb68  pi.h.h.h.h.h.h.h
-00002b60: 996a 4601 0000 68e3 68bf 6887 688f 68d1  .jF...h.h.h.h.h.
-00002b70: 6845 6849 6a40 0100 0068 f790 8c09 7471  hEhIj@...h....tq
-00002b80: 646d 2e61 7574 6f94 8f94 2868 4568 d790  dm.auto...(hEh..
-00002b90: 8c0f 5051 416e 616c 7973 6973 2e63 6f72  ..PQAnalysis.cor
-00002ba0: 6594 8f94 286a 6c01 0000 6a57 0100 0068  e...(jl...jW...h
-00002bb0: a168 776a 4701 0000 68d7 68bf 6887 6a3d  .hwjG...h.h.h.j=
-00002bc0: 0100 0068 cb68 d568 a768 8568 4568 cf6a  ...h.h.h.h.hEh.j
-00002bd0: 4001 0000 68f7 6a46 0100 0090 8c0f 5051  @...h.jF......PQ
-00002be0: 416e 616c 7973 6973 2e74 7261 6a94 8f94  Analysis.traj...
-00002bf0: 286a 3d01 0000 68d5 6a1b 0100 0068 a368  (j=...h.j....h.h
-00002c00: 5168 cf6a 6c01 0000 68c9 6869 68c3 68c7  Qh.jl...h.hih.h.
-00002c10: 68d7 68bd 684f 68a9 68bf 68d1 6845 6849  h.h.hOh.h.h.hEhI
-00002c20: 68f7 908c 1350 5141 6e61 6c79 7369 732e  h....PQAnalysis.
-00002c30: 746f 706f 6c6f 6779 948f 9428 6a57 0100  topology...(jW..
-00002c40: 0068 ed68 7768 d768 f16a 3d01 0000 6887  .h.hwh.h.j=...h.
-00002c50: 68d5 68d1 6845 6849 68eb 6a46 0100 0090  h.h.hEhIh.jF....
-00002c60: 8c0a 5051 416e 616c 7973 6973 948f 9428  ..PQAnalysis...(
-00002c70: 68b9 68ed 68f1 6a3d 0100 006a 3e01 0000  h.h.h.j=...j>...
-00002c80: 68d5 6a1b 0100 006a 1101 0000 6851 6897  h.j....j....hQh.
-00002c90: 6a05 0100 0068 bb68 4768 b368 c968 6f68  j....h.hGh.h.hoh
-00002ca0: c36a 3f01 0000 6895 68c7 68a1 6877 68bd  .j?...h.h.h.hwh.
-00002cb0: 68d7 68a9 68cb 68a7 68df 6883 6a03 0100  h.h.h.h.h.h.j...
-00002cc0: 0068 8768 8f68 456a 4001 0000 68f7 908c  .h.h.hEj@...h...
-00002cd0: 2250 5141 6e61 6c79 7369 732e 616e 616c  "PQAnalysis.anal
-00002ce0: 7973 6973 2e72 6466 2e65 7863 6570 7469  ysis.rdf.excepti
-00002cf0: 6f6e 7394 8f94 286a 6701 0000 6845 908c  ons...(jg...hE..
-00002d00: 2a50 5141 6e61 6c79 7369 732e 696f 2e69  *PQAnalysis.io.i
-00002d10: 6e70 7574 5f66 696c 655f 7265 6164 6572  nput_file_reader
-00002d20: 2e65 7863 6570 7469 6f6e 7394 8f94 2868  .exceptions...(h
-00002d30: ff6a 3f01 0000 6847 6a05 0100 0090 8c2d  .j?...hGj......-
-00002d40: 5051 416e 616c 7973 6973 2e61 6e61 6c79  PQAnalysis.analy
-00002d50: 7369 732e 7264 662e 7264 665f 696e 7075  sis.rdf.rdf_inpu
-00002d60: 745f 6669 6c65 5f72 6561 6465 7294 8f94  t_file_reader...
-00002d70: 286a 6701 0000 6853 6849 908c 2e50 5141  (jg...hShI...PQA
-00002d80: 6e61 6c79 7369 732e 616e 616c 7973 6973  nalysis.analysis
-00002d90: 2e72 6466 2e72 6466 5f6f 7574 7075 745f  .rdf.rdf_output_
-00002da0: 6669 6c65 5f77 7269 7465 7294 8f94 286a  file_writer...(j
-00002db0: 6701 0000 6849 908c 1b50 5141 6e61 6c79  g...hI...PQAnaly
-00002dc0: 7369 732e 616e 616c 7973 6973 2e72 6466  sis.analysis.rdf
-00002dd0: 2e61 7069 948f 9428 6a67 0100 0090 8c21  .api...(jg.....!
-00002de0: 5051 416e 616c 7973 6973 2e74 6f6f 6c73  PQAnalysis.tools
-00002df0: 2e74 7261 6a5f 746f 5f63 6f6d 5f74 7261  .traj_to_com_tra
-00002e00: 6a94 8f94 288c 1050 5141 6e61 6c79 7369  j...(..PQAnalysi
-00002e10: 732e 746f 6f6c 7394 908c 1550 5141 6e61  s.tools....PQAna
-00002e20: 6c79 7369 732e 696f 2e66 6f72 6d61 7473  lysis.io.formats
-00002e30: 948f 9428 68c7 685d 68f1 68eb 68bf 6a6d  ...(h.h]h.h.h.jm
-00002e40: 0100 006a 3e01 0000 8c0d 5051 416e 616c  ...j>.....PQAnal
-00002e50: 7973 6973 2e69 6f94 68c9 68d1 6851 68cf  ysis.io.h.h.hQh.
-00002e60: 68df 68f7 6869 908c 1850 5141 6e61 6c79  h.h.hi...PQAnaly
-00002e70: 7369 732e 6174 6f6d 6963 5f73 7973 7465  sis.atomic_syste
-00002e80: 6d94 8f94 286a 6c01 0000 68c7 68d7 6a3d  m...(jl...h.h.j=
-00002e90: 0100 0068 876a 6d01 0000 68d5 68d1 6a1b  ...h.jm...h.h.j.
-00002ea0: 0100 0068 5168 cf68 df6a 4001 0000 68f7  ...hQh.h.j@...h.
-00002eb0: 908c 1f50 5141 6e61 6c79 7369 732e 636c  ...PQAnalysis.cl
-00002ec0: 692e 5f61 7267 756d 656e 745f 7061 7273  i._argument_pars
-00002ed0: 6572 948f 9428 686b 6855 685d 6857 685b  er...(hkhUh]hWh[
-00002ee0: 6853 6865 6867 6861 6863 908c 1850 5141  hShehghahc...PQA
-00002ef0: 6e61 6c79 7369 732e 636c 692e 5f63 6c69  nalysis.cli._cli
-00002f00: 5f62 6173 6594 8f94 2868 6b68 5568 5d68  _base...(hkhUh]h
-00002f10: 5768 5b68 5368 6568 6168 6390 8c1c 5051  Wh[hShehahc...PQ
-00002f20: 416e 616c 7973 6973 2e69 6f2e 6e65 702e  Analysis.io.nep.
-00002f30: 6e65 705f 7772 6974 6572 948f 9428 6855  nep_writer...(hU
-00002f40: 908c 1d50 5141 6e61 6c79 7369 732e 746f  ...PQAnalysis.to
-00002f50: 6f6c 732e 6164 645f 6d6f 6c65 6375 6c65  ols.add_molecule
-00002f60: 948f 9428 685d 908c 1650 5141 6e61 6c79  ...(h]...PQAnaly
-00002f70: 7369 732e 636c 692e 7879 7a32 6765 6e94  sis.cli.xyz2gen.
-00002f80: 8f94 2868 6790 8c19 5051 416e 616c 7973  ..(hg...PQAnalys
-00002f90: 6973 2e63 6c69 2e74 7261 6a32 716d 6366  is.cli.traj2qmcf
-00002fa0: 6394 8f94 2868 6790 8c17 5051 416e 616c  c...(hg...PQAnal
-00002fb0: 7973 6973 2e63 6c69 2e74 7261 6a32 626f  ysis.cli.traj2bo
-00002fc0: 7894 8f94 2868 6790 8c16 5051 416e 616c  x...(hg...PQAnal
-00002fd0: 7973 6973 2e63 6c69 2e72 7374 3278 797a  ysis.cli.rst2xyz
-00002fe0: 948f 9428 6867 908c 1250 5141 6e61 6c79  ...(hg...PQAnaly
-00002ff0: 7369 732e 636c 692e 7264 6694 8f94 2868  sis.cli.rdf...(h
-00003000: 6790 8c16 5051 416e 616c 7973 6973 2e63  g...PQAnalysis.c
-00003010: 6c69 2e67 656e 3278 797a 948f 9428 6867  li.gen2xyz...(hg
-00003020: 908c 1d50 5141 6e61 6c79 7369 732e 636c  ...PQAnalysis.cl
-00003030: 692e 636f 6e74 696e 7565 5f69 6e70 7574  i.continue_input
-00003040: 948f 9428 6867 908c 1c50 5141 6e61 6c79  ...(hg...PQAnaly
-00003050: 7369 732e 636c 692e 6164 645f 6d6f 6c65  sis.cli.add_mole
-00003060: 6375 6c65 7394 8f94 2868 6790 8c1d 5051  cules...(hg...PQ
-00003070: 416e 616c 7973 6973 2e63 6c69 2e62 7569  Analysis.cli.bui
-00003080: 6c64 5f6e 6570 5f74 7261 6a94 8f94 2868  ld_nep_traj...(h
-00003090: 6790 8c0b 6172 6763 6f6d 706c 6574 6594  g...argcomplete.
-000030a0: 8f94 2868 6990 8c0d 7269 6368 5f61 7267  ..(hi...rich_arg
-000030b0: 7061 7273 6594 8f94 2868 6990 8c23 5051  parse...(hi..#PQ
-000030c0: 416e 616c 7973 6973 2e70 6879 7369 6361  Analysis.physica
-000030d0: 6c5f 6461 7461 2e65 7863 6570 7469 6f6e  l_data.exception
-000030e0: 7394 8f94 288c 1850 5141 6e61 6c79 7369  s...(..PQAnalysi
-000030f0: 732e 7068 7973 6963 616c 5f64 6174 6194  s.physical_data.
-00003100: 686f 908c 1f50 5141 6e61 6c79 7369 732e  ho...PQAnalysis.
-00003110: 7068 7973 6963 616c 5f64 6174 612e 656e  physical_data.en
-00003120: 6572 6779 948f 9428 6aaa 0100 0090 8c23  ergy...(j......#
-00003130: 5051 416e 616c 7973 6973 2e61 746f 6d69  PQAnalysis.atomi
-00003140: 635f 7379 7374 656d 2e65 7863 6570 7469  c_system.excepti
-00003150: 6f6e 7394 8f94 286a 4701 0000 6875 8c18  ons...(jG...hu..
-00003160: 5051 416e 616c 7973 6973 2e61 746f 6d69  PQAnalysis.atomi
-00003170: 635f 7379 7374 656d 9468 7790 8c17 7363  c_system.hw...sc
-00003180: 6970 792e 7370 6174 6961 6c2e 7472 616e  ipy.spatial.tran
-00003190: 7366 6f72 6d94 8f94 2868 7790 8c17 5051  sform...(hw...PQ
-000031a0: 416e 616c 7973 6973 2e75 7469 6c73 2e72  Analysis.utils.r
-000031b0: 616e 646f 6d94 8f94 286a 1b01 0000 6877  andom...(j....hw
-000031c0: 908c 1550 5141 6e61 6c79 7369 732e 7574  ...PQAnalysis.ut
-000031d0: 696c 732e 6d61 7468 948f 9428 6899 6877  ils.math...(h.hw
-000031e0: 908c 2450 5141 6e61 6c79 7369 732e 6174  ..$PQAnalysis.at
-000031f0: 6f6d 6963 5f73 7973 7465 6d2e 5f70 726f  omic_system._pro
-00003200: 7065 7274 6965 7394 8f94 2868 7790 8c2d  perties...(hw..-
-00003210: 5051 416e 616c 7973 6973 2e61 746f 6d69  PQAnalysis.atomi
-00003220: 635f 7379 7374 656d 2e5f 7374 616e 6461  c_system._standa
-00003230: 7264 5f70 726f 7065 7274 6965 7394 8f94  rd_properties...
-00003240: 2868 7790 8c23 5051 416e 616c 7973 6973  (hw..#PQAnalysis
-00003250: 2e61 746f 6d69 635f 7379 7374 656d 2e5f  .atomic_system._
-00003260: 706f 7369 7469 6f6e 7394 8f94 2868 7790  positions...(hw.
-00003270: 8c26 5051 416e 616c 7973 6973 2e61 746f  .&PQAnalysis.ato
-00003280: 6d69 635f 7379 7374 656d 2e61 746f 6d69  mic_system.atomi
-00003290: 635f 7379 7374 656d 948f 9428 6aaf 0100  c_system...(j...
-000032a0: 0090 8c24 5051 416e 616c 7973 6973 2e61  ...$PQAnalysis.a
-000032b0: 746f 6d69 635f 7379 7374 656d 2e5f 6465  tomic_system._de
-000032c0: 636f 7261 746f 7273 948f 9428 6a47 0100  corators...(jG..
-000032d0: 006a 5701 0000 6a46 0100 0090 8c12 5051  .jW...jF......PQ
-000032e0: 416e 616c 7973 6973 2e66 6f72 6d61 7473  Analysis.formats
-000032f0: 948f 9428 68ff 6883 68b9 908c 1a50 5141  ...(h.h.h....PQA
-00003300: 6e61 6c79 7369 732e 7472 616a 2e65 7863  nalysis.traj.exc
-00003310: 6570 7469 6f6e 7394 8f94 2868 838c 0f50  eptions...(h...P
-00003320: 5141 6e61 6c79 7369 732e 7472 616a 9490  QAnalysis.traj..
-00003330: 8c17 5051 416e 616c 7973 6973 2e74 7261  ..PQAnalysis.tra
-00003340: 6a2e 666f 726d 6174 7394 8f94 286a c401  j.formats...(j..
-00003350: 0000 908c 1a50 5141 6e61 6c79 7369 732e  .....PQAnalysis.
-00003360: 7472 616a 2e74 7261 6a65 6374 6f72 7994  traj.trajectory.
-00003370: 8f94 286a c401 0000 9068 858f 9428 6ac4  ..(j.....h...(j.
-00003380: 0100 0090 8c14 5051 416e 616c 7973 6973  ......PQAnalysis
-00003390: 2e63 6f72 652e 6365 6c6c 948f 9428 688d  .core.cell...(h.
-000033a0: 8c0f 5051 416e 616c 7973 6973 2e63 6f72  ..PQAnalysis.cor
-000033b0: 6594 908c 1450 5141 6e61 6c79 7369 732e  e....PQAnalysis.
-000033c0: 636f 7265 2e61 746f 6d94 8f94 286a cc01  core.atom...(j..
-000033d0: 0000 688f 908c 1a50 5141 6e61 6c79 7369  ..h....PQAnalysi
-000033e0: 732e 636f 7265 2e65 7863 6570 7469 6f6e  s.core.exception
-000033f0: 7394 8f94 2868 9768 9568 a168 8f6a cc01  s...(h.h.h.h.j..
-00003400: 0000 908c 1750 5141 6e61 6c79 7369 732e  .....PQAnalysis.
-00003410: 636f 7265 2e72 6573 6964 7565 948f 9428  core.residue...(
-00003420: 6acc 0100 0090 8c13 5051 416e 616c 7973  j.......PQAnalys
-00003430: 6973 2e63 6f72 652e 6170 6994 8f94 286a  is.core.api...(j
-00003440: cc01 0000 908c 1c50 5141 6e61 6c79 7369  .......PQAnalysi
-00003450: 732e 636f 7265 2e61 746f 6d2e 656c 656d  s.core.atom.elem
-00003460: 656e 7494 8f94 2868 958c 1450 5141 6e61  ent...(h...PQAna
-00003470: 6c79 7369 732e 636f 7265 2e61 746f 6d94  lysis.core.atom.
-00003480: 908c 1950 5141 6e61 6c79 7369 732e 636f  ...PQAnalysis.co
-00003490: 7265 2e61 746f 6d2e 6174 6f6d 948f 9428  re.atom.atom...(
-000034a0: 6ad7 0100 0090 8c29 5051 416e 616c 7973  j......)PQAnalys
-000034b0: 6973 2e63 6f72 652e 6365 6c6c 2e5f 7374  is.core.cell._st
-000034c0: 616e 6461 7264 5f70 726f 7065 7274 6965  andard_propertie
-000034d0: 7394 8f94 2868 9990 8c19 5051 416e 616c  s...(h....PQAnal
-000034e0: 7973 6973 2e63 6f72 652e 6365 6c6c 2e63  ysis.core.cell.c
-000034f0: 656c 6c94 8f94 288c 1450 5141 6e61 6c79  ell...(..PQAnaly
-00003500: 7369 732e 636f 7265 2e63 656c 6c94 908c  sis.core.cell...
-00003510: 1e50 5141 6e61 6c79 7369 732e 746f 706f  .PQAnalysis.topo
-00003520: 6c6f 6779 2e65 7863 6570 7469 6f6e 7394  logy.exceptions.
-00003530: 8f94 288c 1350 5141 6e61 6c79 7369 732e  ..(..PQAnalysis.
-00003540: 746f 706f 6c6f 6779 9468 a190 8c33 5051  topology.h...3PQ
-00003550: 416e 616c 7973 6973 2e74 6f70 6f6c 6f67  Analysis.topolog
-00003560: 792e 626f 6e64 6564 5f74 6f70 6f6c 6f67  y.bonded_topolog
-00003570: 792e 626f 6e64 6564 5f74 6f70 6f6c 6f67  y.bonded_topolog
-00003580: 7994 8f94 286a e101 0000 68a1 908c 1d50  y...(j....h....P
-00003590: 5141 6e61 6c79 7369 732e 746f 706f 6c6f  QAnalysis.topolo
-000035a0: 6779 2e73 656c 6563 7469 6f6e 948f 9428  gy.selection...(
-000035b0: 68a3 6ae1 0100 0068 a990 8c22 5051 416e  h.j....h..."PQAn
-000035c0: 616c 7973 6973 2e74 6f70 6f6c 6f67 792e  alysis.topology.
-000035d0: 7368 616b 655f 746f 706f 6c6f 6779 948f  shake_topology..
-000035e0: 9428 68a3 908c 2850 5141 6e61 6c79 7369  .(h...(PQAnalysi
-000035f0: 732e 746f 706f 6c6f 6779 2e62 6f6e 6465  s.topology.bonde
-00003600: 645f 746f 706f 6c6f 6779 2e62 6f6e 6494  d_topology.bond.
-00003610: 8f94 286a e101 0000 68ad 68b3 908c 2950  ..(j....h.h...)P
-00003620: 5141 6e61 6c79 7369 732e 746f 706f 6c6f  QAnalysis.topolo
-00003630: 6779 2e62 6f6e 6465 645f 746f 706f 6c6f  gy.bonded_topolo
-00003640: 6779 2e61 6e67 6c65 948f 9428 6ae1 0100  gy.angle...(j...
-00003650: 0068 ad68 b390 8c2c 5051 416e 616c 7973  .h.h...,PQAnalys
-00003660: 6973 2e74 6f70 6f6c 6f67 792e 626f 6e64  is.topology.bond
-00003670: 6564 5f74 6f70 6f6c 6f67 792e 6469 6865  ed_topology.dihe
-00003680: 6472 616c 948f 9428 6ae1 0100 0068 ad68  dral...(j....h.h
-00003690: b390 8c1c 5051 416e 616c 7973 6973 2e74  ....PQAnalysis.t
-000036a0: 6f70 6f6c 6f67 792e 746f 706f 6c6f 6779  opology.topology
-000036b0: 948f 9428 68a7 6ae1 0100 0090 8c04 6c61  ...(h.j.......la
-000036c0: 726b 948f 9428 6a03 0100 0068 a790 8c38  rk...(j....h...8
-000036d0: 5051 416e 616c 7973 6973 2e74 6f70 6f6c  PQAnalysis.topol
-000036e0: 6f67 792e 626f 6e64 6564 5f74 6f70 6f6c  ogy.bonded_topol
-000036f0: 6f67 792e 5f74 6f70 6f6c 6f67 795f 7072  ogy._topology_pr
-00003700: 6f70 6572 7469 6573 948f 9428 68b3 908c  operties...(h...
-00003710: 1850 5141 6e61 6c79 7369 732e 696f 2e65  .PQAnalysis.io.e
-00003720: 7863 6570 7469 6f6e 7394 8f94 2868 cb68  xceptions...(h.h
-00003730: b96a 3e01 0000 68c9 908c 1f50 5141 6e61  .j>...h....PQAna
-00003740: 6c79 7369 732e 696f 2e69 6e70 7574 5f66  lysis.io.input_f
-00003750: 696c 655f 7265 6164 6572 948f 9428 6a87  ile_reader...(j.
-00003760: 0100 0068 bb90 8c27 5051 416e 616c 7973  ...h...'PQAnalys
-00003770: 6973 2e69 6f2e 696e 7075 745f 6669 6c65  is.io.input_file
-00003780: 5f72 6561 6465 722e 666f 726d 6174 7394  _reader.formats.
-00003790: 8f94 286a 3f01 0000 68bb 6a03 0100 008c  ..(j?...h.j.....
-000037a0: 1f50 5141 6e61 6c79 7369 732e 696f 2e69  .PQAnalysis.io.i
-000037b0: 6e70 7574 5f66 696c 655f 7265 6164 6572  nput_file_reader
-000037c0: 946a 1101 0000 908c 1850 5141 6e61 6c79  .j.......PQAnaly
-000037d0: 7369 732e 7068 7973 6963 616c 5f64 6174  sis.physical_dat
-000037e0: 6194 8f94 2868 bd90 8c12 5051 416e 616c  a...(h....PQAnal
-000037f0: 7973 6973 2e69 6f2e 6261 7365 948f 9428  ysis.io.base...(
-00003800: 68c3 68ed 68f1 68d7 68bd 6a03 0100 006a  h.h.h.h.h.j....j
-00003810: 3d01 0000 6a87 0100 0068 c968 cb68 cf68  =...j....h.h.h.h
-00003820: df6a 4001 0000 68f7 908c 1e50 5141 6e61  .j@...h....PQAna
-00003830: 6c79 7369 732e 696f 2e69 6e66 6f5f 6669  lysis.io.info_fi
-00003840: 6c65 5f72 6561 6465 7294 8f94 2868 bd6a  le_reader...(h.j
-00003850: 8701 0000 908c 1750 5141 6e61 6c79 7369  .......PQAnalysi
-00003860: 732e 696f 2e74 7261 6a5f 6669 6c65 948f  s.io.traj_file..
-00003870: 9428 68d1 68bf 908c 1850 5141 6e61 6c79  .(h.h....PQAnaly
-00003880: 7369 732e 696f 2e62 6f78 5f77 7269 7465  sis.io.box_write
-00003890: 7294 8f94 2868 bf68 c76a 8701 0000 908c  r...(h.h.j......
-000038a0: 1650 5141 6e61 6c79 7369 732e 696f 2e67  .PQAnalysis.io.g
-000038b0: 656e 5f66 696c 6594 8f94 2868 bf90 8c1e  en_file...(h....
-000038c0: 5051 416e 616c 7973 6973 2e69 6f2e 7265  PQAnalysis.io.re
-000038d0: 7374 6172 745f 6669 6c65 2e61 7069 948f  start_file.api..
-000038e0: 9428 68bf 6a87 0100 0090 8c1b 5051 416e  .(h.j.......PQAn
-000038f0: 616c 7973 6973 2e69 6f2e 7472 616a 5f66  alysis.io.traj_f
-00003900: 696c 652e 6170 6994 8f94 2868 bf68 c76a  ile.api...(h.h.j
-00003910: 8701 0000 908c 2250 5141 6e61 6c79 7369  ......"PQAnalysi
-00003920: 732e 696f 2e6d 6f6c 6465 7363 7269 7074  s.io.moldescript
-00003930: 6f72 5f72 6561 6465 7294 8f94 286a 3d01  or_reader...(j=.
-00003940: 0000 6a87 0100 0090 8c29 5051 416e 616c  ..j......)PQAnal
-00003950: 7973 6973 2e69 6f2e 7265 7374 6172 745f  ysis.io.restart_
-00003960: 6669 6c65 2e72 6573 7461 7274 5f77 7269  file.restart_wri
-00003970: 7465 7294 8f94 288c 1a50 5141 6e61 6c79  ter...(..PQAnaly
-00003980: 7369 732e 696f 2e72 6573 7461 7274 5f66  sis.io.restart_f
-00003990: 696c 6594 6a87 0100 0090 8c29 5051 416e  ile.j......)PQAn
-000039a0: 616c 7973 6973 2e69 6f2e 7265 7374 6172  alysis.io.restar
-000039b0: 745f 6669 6c65 2e72 6573 7461 7274 5f72  t_file.restart_r
-000039c0: 6561 6465 7294 8f94 286a 6c01 0000 6a0f  eader...(jl...j.
-000039d0: 0200 006a 8701 0000 908c 2950 5141 6e61  ...j......)PQAna
-000039e0: 6c79 7369 732e 696f 2e74 7261 6a5f 6669  lysis.io.traj_fi
-000039f0: 6c65 2e74 7261 6a65 6374 6f72 795f 7265  le.trajectory_re
-00003a00: 6164 6572 948f 9428 8c17 5051 416e 616c  ader...(..PQAnal
-00003a10: 7973 6973 2e69 6f2e 7472 616a 5f66 696c  ysis.io.traj_fil
-00003a20: 6594 6a87 0100 0090 8c29 5051 416e 616c  e.j......)PQAnal
-00003a30: 7973 6973 2e69 6f2e 7472 616a 5f66 696c  ysis.io.traj_fil
-00003a40: 652e 7472 616a 6563 746f 7279 5f77 7269  e.trajectory_wri
-00003a50: 7465 7294 8f94 286a 1402 0000 6a87 0100  ter...(j....j...
-00003a60: 0090 8c24 5051 416e 616c 7973 6973 2e69  ...$PQAnalysis.i
-00003a70: 6f2e 7472 616a 5f66 696c 652e 6672 616d  o.traj_file.fram
-00003a80: 655f 7265 6164 6572 948f 9428 6a14 0200  e_reader...(j...
-00003a90: 006a 8701 0000 68d7 908c 2650 5141 6e61  .j....h...&PQAna
-00003aa0: 6c79 7369 732e 696f 2e67 656e 5f66 696c  lysis.io.gen_fil
-00003ab0: 652e 6765 6e5f 6669 6c65 5f72 6561 6465  e.gen_file_reade
-00003ac0: 7294 8f94 288c 1650 5141 6e61 6c79 7369  r...(..PQAnalysi
-00003ad0: 732e 696f 2e67 656e 5f66 696c 6594 6a6d  s.io.gen_file.jm
-00003ae0: 0100 006a 8701 0000 908c 2650 5141 6e61  ...j......&PQAna
-00003af0: 6c79 7369 732e 696f 2e67 656e 5f66 696c  lysis.io.gen_fil
-00003b00: 652e 6765 6e5f 6669 6c65 5f77 7269 7465  e.gen_file_write
-00003b10: 7294 8f94 286a 1b02 0000 6a6d 0100 006a  r...(j....jm...j
-00003b20: 8701 0000 908c 1a50 5141 6e61 6c79 7369  .......PQAnalysi
-00003b30: 732e 696f 2e67 656e 5f66 696c 652e 6170  s.io.gen_file.ap
-00003b40: 6994 8f94 286a 1b02 0000 6a87 0100 0090  i...(j....j.....
-00003b50: 8c1b 5051 416e 616c 7973 6973 2e69 6f2e  ..PQAnalysis.io.
-00003b60: 746f 706f 6c6f 6779 5f66 696c 6594 8f94  topology_file...
-00003b70: 286a 8701 0000 908c 1f50 5141 6e61 6c79  (j.......PQAnaly
-00003b80: 7369 732e 696f 2e74 6f70 6f6c 6f67 795f  sis.io.topology_
-00003b90: 6669 6c65 2e61 7069 948f 9428 6a87 0100  file.api...(j...
-00003ba0: 0090 8c20 5051 416e 616c 7973 6973 2e69  ... PQAnalysis.i
-00003bb0: 6f2e 656e 6572 6779 5f66 696c 655f 7265  o.energy_file_re
-00003bc0: 6164 6572 948f 9428 6a87 0100 0090 8c11  ader...(j.......
-00003bd0: 5051 416e 616c 7973 6973 2e69 6f2e 6170  PQAnalysis.io.ap
-00003be0: 6994 8f94 286a 8701 0000 908c 1c50 5141  i...(j.......PQA
-00003bf0: 6e61 6c79 7369 732e 696f 2e63 6f6e 7665  nalysis.io.conve
-00003c00: 7273 696f 6e5f 6170 6994 8f94 286a 8701  rsion_api...(j..
-00003c10: 0000 908c 1750 5141 6e61 6c79 7369 732e  .....PQAnalysis.
-00003c20: 696f 2e77 7269 7465 5f61 7069 948f 9428  io.write_api...(
-00003c30: 6a87 0100 0090 8c22 5051 416e 616c 7973  j......"PQAnalys
-00003c40: 6973 2e69 6f2e 7472 616a 5f66 696c 652e  is.io.traj_file.
-00003c50: 6578 6365 7074 696f 6e73 948f 9428 68d7  exceptions...(h.
-00003c60: 68d5 908c 2150 5141 6e61 6c79 7369 732e  h...!PQAnalysis.
-00003c70: 696f 2e67 656e 5f66 696c 652e 6578 6365  io.gen_file.exce
-00003c80: 7074 696f 6e73 948f 9428 6a40 0100 0090  ptions...(j@....
-00003c90: 8c22 5051 416e 616c 7973 6973 2e69 6f2e  ."PQAnalysis.io.
-00003ca0: 7669 7269 616c 2e76 6972 6961 6c5f 7265  virial.virial_re
-00003cb0: 6164 6572 948f 9428 8c14 5051 416e 616c  ader...(..PQAnal
-00003cc0: 7973 6973 2e69 6f2e 7669 7269 616c 9468  ysis.io.virial.h
-00003cd0: e390 8c30 5051 416e 616c 7973 6973 2e69  ...0PQAnalysis.i
-00003ce0: 6f2e 746f 706f 6c6f 6779 5f66 696c 652e  o.topology_file.
-00003cf0: 746f 706f 6c6f 6779 5f66 696c 655f 7772  topology_file_wr
-00003d00: 6974 6572 948f 9428 8c1b 5051 416e 616c  iter...(..PQAnal
-00003d10: 7973 6973 2e69 6f2e 746f 706f 6c6f 6779  ysis.io.topology
-00003d20: 5f66 696c 6594 68eb 908c 3050 5141 6e61  _file.h...0PQAna
-00003d30: 6c79 7369 732e 696f 2e74 6f70 6f6c 6f67  lysis.io.topolog
-00003d40: 795f 6669 6c65 2e74 6f70 6f6c 6f67 795f  y_file.topology_
-00003d50: 6669 6c65 5f72 6561 6465 7294 8f94 286a  file_reader...(j
-00003d60: 3502 0000 68eb 908c 2650 5141 6e61 6c79  5...h...&PQAnaly
-00003d70: 7369 732e 696f 2e74 6f70 6f6c 6f67 795f  sis.io.topology_
-00003d80: 6669 6c65 2e65 7863 6570 7469 6f6e 7394  file.exceptions.
-00003d90: 8f94 2868 ed68 f190 8c25 5051 416e 616c  ..(h.h...%PQAnal
-00003da0: 7973 6973 2e69 6f2e 7265 7374 6172 745f  ysis.io.restart_
-00003db0: 6669 6c65 2e65 7863 6570 7469 6f6e 7394  file.exceptions.
-00003dc0: 8f94 286a 3d01 0000 68f7 908c 3150 5141  ..(j=...h...1PQA
-00003dd0: 6e61 6c79 7369 732e 696f 2e69 6e70 7574  nalysis.io.input
-00003de0: 5f66 696c 655f 7265 6164 6572 2e69 6e70  _file_reader.inp
-00003df0: 7574 5f66 696c 655f 7061 7273 6572 948f  ut_file_parser..
-00003e00: 9428 6afa 0100 006a 3f01 0000 6a11 0100  .(j....j?...j...
-00003e10: 006a 0501 0000 908c 2250 5141 6e61 6c79  .j......"PQAnaly
-00003e20: 7369 732e 696f 2e69 6e70 7574 5f66 696c  sis.io.input_fil
-00003e30: 655f 7265 6164 6572 2e70 7194 8f94 286a  e_reader.pq...(j
-00003e40: fa01 0000 908c 2b50 5141 6e61 6c79 7369  ......+PQAnalysi
-00003e50: 732e 696f 2e69 6e70 7574 5f66 696c 655f  s.io.input_file_
-00003e60: 7265 6164 6572 2e70 715f 616e 616c 7973  reader.pq_analys
-00003e70: 6973 948f 9428 6afa 0100 0090 8c48 5051  is...(j......HPQ
-00003e80: 416e 616c 7973 6973 2e69 6f2e 696e 7075  Analysis.io.inpu
-00003e90: 745f 6669 6c65 5f72 6561 6465 722e 7071  t_file_reader.pq
-00003ea0: 5f61 6e61 6c79 7369 732e 7071 616e 616c  _analysis.pqanal
-00003eb0: 7973 6973 5f69 6e70 7574 5f66 696c 655f  ysis_input_file_
-00003ec0: 7265 6164 6572 948f 9428 8c2b 5051 416e  reader...(.+PQAn
-00003ed0: 616c 7973 6973 2e69 6f2e 696e 7075 745f  alysis.io.input_
-00003ee0: 6669 6c65 5f72 6561 6465 722e 7071 5f61  file_reader.pq_a
-00003ef0: 6e61 6c79 7369 7394 908c 3750 5141 6e61  nalysis...7PQAna
-00003f00: 6c79 7369 732e 696f 2e69 6e70 7574 5f66  lysis.io.input_f
-00003f10: 696c 655f 7265 6164 6572 2e70 715f 616e  ile_reader.pq_an
-00003f20: 616c 7973 6973 2e5f 6669 6c65 5f6d 6978  alysis._file_mix
-00003f30: 696e 948f 9428 6a3f 0100 0090 8c3c 5051  in...(j?.....<PQ
-00003f40: 416e 616c 7973 6973 2e69 6f2e 696e 7075  Analysis.io.inpu
-00003f50: 745f 6669 6c65 5f72 6561 6465 722e 7071  t_file_reader.pq
-00003f60: 5f61 6e61 6c79 7369 732e 5f73 656c 6563  _analysis._selec
-00003f70: 7469 6f6e 5f6d 6978 696e 948f 9428 6a3f  tion_mixin...(j?
-00003f80: 0100 0090 8c3c 5051 416e 616c 7973 6973  .....<PQAnalysis
-00003f90: 2e69 6f2e 696e 7075 745f 6669 6c65 5f72  .io.input_file_r
-00003fa0: 6561 6465 722e 7071 5f61 6e61 6c79 7369  eader.pq_analysi
-00003fb0: 732e 5f70 6f73 6974 696f 6e73 5f6d 6978  s._positions_mix
-00003fc0: 696e 948f 9428 6a3f 0100 0090 8c32 5051  in...(j?.....2PQ
-00003fd0: 416e 616c 7973 6973 2e69 6f2e 696e 7075  Analysis.io.inpu
-00003fe0: 745f 6669 6c65 5f72 6561 6465 722e 7071  t_file_reader.pq
-00003ff0: 5f61 6e61 6c79 7369 732e 5f70 6172 7365  _analysis._parse
-00004000: 948f 9428 8c3c 5051 416e 616c 7973 6973  ...(.<PQAnalysis
-00004010: 2e69 6f2e 696e 7075 745f 6669 6c65 5f72  .io.input_file_r
-00004020: 6561 6465 722e 7071 5f61 6e61 6c79 7369  eader.pq_analysi
-00004030: 732e 5f73 656c 6563 7469 6f6e 5f6d 6978  s._selection_mix
-00004040: 696e 946a 5601 0000 6a45 0100 0090 8c2f  in.jV...jE...../
-00004050: 5051 416e 616c 7973 6973 2e69 6f2e 696e  PQAnalysis.io.in
-00004060: 7075 745f 6669 6c65 5f72 6561 6465 722e  put_file_reader.
-00004070: 7071 2e6f 7574 7075 745f 6669 6c65 7394  pq.output_files.
-00004080: 8f94 286a 1101 0000 908c 3750 5141 6e61  ..(j......7PQAna
-00004090: 6c79 7369 732e 696f 2e69 6e70 7574 5f66  lysis.io.input_f
-000040a0: 696c 655f 7265 6164 6572 2e70 712e 7071  ile_reader.pq.pq
-000040b0: 5f69 6e70 7574 5f66 696c 655f 7265 6164  _input_file_read
-000040c0: 6572 948f 9428 8c22 5051 416e 616c 7973  er...(."PQAnalys
-000040d0: 6973 2e69 6f2e 696e 7075 745f 6669 6c65  is.io.input_file
-000040e0: 5f72 6561 6465 722e 7071 9490 8c18 5051  _reader.pq....PQ
-000040f0: 416e 616c 7973 6973 2e69 6f2e 7669 7269  Analysis.io.viri
-00004100: 616c 2e61 7069 948f 9428 6a1b 0100 0090  al.api...(j.....
-00004110: 8c16 5051 416e 616c 7973 6973 2e75 7469  ..PQAnalysis.uti
-00004120: 6c73 2e75 6e69 7473 948f 9428 6a1b 0100  ls.units...(j...
-00004130: 0090 8c16 5051 416e 616c 7973 6973 2e75  ....PQAnalysis.u
-00004140: 7469 6c73 2e66 696c 6573 948f 9428 6a1b  tils.files...(j.
-00004150: 0100 0090 8c1c 5051 416e 616c 7973 6973  ......PQAnalysis
-00004160: 2e69 6f2e 6e65 702e 6578 6365 7074 696f  .io.nep.exceptio
-00004170: 6e73 948f 9428 6a1b 0100 0090 758c 1064  ns...(j.....u..d
-00004180: 7570 6c69 6361 7465 645f 6c69 6e65 7394  uplicated_lines.
-00004190: 7d94 288c 136e 625f 6475 706c 6963 6174  }.(..nb_duplicat
-000041a0: 6564 5f6c 696e 6573 944b 008c 1870 6572  ed_lines.K...per
-000041b0: 6365 6e74 5f64 7570 6c69 6361 7465 645f  cent_duplicated_
-000041c0: 6c69 6e65 7394 4700 0000 0000 0000 0075  lines.G........u
-000041d0: 8c0a 6e6f 6465 5f63 6f75 6e74 947d 9428  ..node_count.}.(
-000041e0: 680e 4b4c 6809 4b75 680f 4d12 0268 104b  h.KLh.Kuh.M..h.K
-000041f0: 7d75 8c0c 756e 646f 6375 6d65 6e74 6564  }u..undocumented
-00004200: 947d 9428 680e 4b00 6809 4b00 680f 4b00  .}.(h.K.h.K.h.K.
-00004210: 6810 4b00 7568 184b 0168 194b 1f68 1a4b  h.K.uh.K.h.K.h.K
-00004220: 0068 1b4b 0068 1c4b 3368 1d4d de11 681e  .h.K.h.K3h.M..h.
-00004230: 4b0a 8c0b 676c 6f62 616c 5f6e 6f74 6594  K...global_note.
-00004240: 4740 230d 18bc f320 936a 5d02 0000 4b1b  G@#.... .j]...K.
-00004250: 6a5e 0200 0047 3fc1 f1e2 2523 a31d 7562  j^...G?...%#..ub
-00004260: 2e                                       .
+00000100: 288c 312f 686f 6d65 2f72 756e 6e65 722f  (.1/home/runner/
+00000110: 776f 726b 2f50 5141 6e61 6c79 7369 732f  work/PQAnalysis/
+00000120: 5051 416e 616c 7973 6973 2f2e 7079 6c69  PQAnalysis/.pyli
+00000130: 6e74 7263 947d 9428 8c0a 636f 6e76 656e  ntrc.}.(..conven
+00000140: 7469 6f6e 944b 008c 0565 7272 6f72 944b  tion.K...error.K
+00000150: 008c 0566 6174 616c 944b 008c 0469 6e66  ...fatal.K...inf
+00000160: 6f94 4b00 8c08 7265 6661 6374 6f72 944b  o.K...refactor.K
+00000170: 008c 0973 7461 7465 6d65 6e74 944b 008c  ...statement.K..
+00000180: 0777 6172 6e69 6e67 944b 0075 8c0c 436f  .warning.K.u..Co
+00000190: 6d6d 616e 6420 6c69 6e65 947d 9428 6818  mmand line.}.(h.
+000001a0: 4b00 6819 4b00 681a 4b00 681b 4b00 681c  K.h.K.h.K.h.K.h.
+000001b0: 4b00 681d 4b00 681e 4b00 758c 2243 6f6d  K.h.K.h.K.u."Com
+000001c0: 6d61 6e64 206c 696e 6520 6f72 2063 6f6e  mand line or con
+000001d0: 6669 6775 7261 7469 6f6e 2066 696c 6594  figuration file.
+000001e0: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
+000001f0: 1b4b 0068 1c4b 0068 1d4b 0068 1e4b 0075  .K.h.K.h.K.h.K.u
+00000200: 8c0a 5051 416e 616c 7973 6973 947d 9428  ..PQAnalysis.}.(
+00000210: 6818 4b00 6819 4b01 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
+00000220: 681c 4b00 681d 4b1c 681e 4b01 758c 1250  h.K.h.K.h.K.u..P
+00000230: 5141 6e61 6c79 7369 732e 666f 726d 6174  QAnalysis.format
+00000240: 7394 7d94 2868 184b 0068 194b 0068 1a4b  s.}.(h.K.h.K.h.K
+00000250: 0068 1b4b 0068 1c4b 0068 1d4b 1468 1e4b  .h.K.h.K.h.K.h.K
+00000260: 0075 8c11 5051 416e 616c 7973 6973 2e63  .u..PQAnalysis.c
+00000270: 6f6e 6669 6794 7d94 2868 184b 0068 194b  onfig.}.(h.K.h.K
+00000280: 0068 1a4b 0068 1b4b 0068 1c4b 0068 1d4b  .h.K.h.K.h.K.h.K
+00000290: 0668 1e4b 0075 8c18 5051 416e 616c 7973  .h.K.u..PQAnalys
+000002a0: 6973 2e74 7970 655f 6368 6563 6b69 6e67  is.type_checking
+000002b0: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
+000002c0: 681b 4b00 681c 4b00 681d 4b37 681e 4b00  h.K.h.K.h.K7h.K.
+000002d0: 758c 1050 5141 6e61 6c79 7369 732e 7479  u..PQAnalysis.ty
+000002e0: 7065 7394 7d94 2868 184b 0068 194b 0068  pes.}.(h.K.h.K.h
+000002f0: 1a4b 0068 1b4b 0068 1c4b 0068 1d4b 0f68  .K.h.K.h.K.h.K.h
+00000300: 1e4b 0075 8c15 5051 416e 616c 7973 6973  .K.u..PQAnalysis
+00000310: 2e65 7863 6570 7469 6f6e 7394 7d94 2868  .exceptions.}.(h
+00000320: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
+00000330: 1c4b 0068 1d4b 1168 1e4b 0075 8c17 5051  .K.h.K.h.K.u..PQ
+00000340: 416e 616c 7973 6973 2e74 7261 6a2e 666f  Analysis.traj.fo
+00000350: 726d 6174 7394 7d94 2868 184b 0068 194b  rmats.}.(h.K.h.K
+00000360: 0068 1a4b 0068 1b4b 0068 1c4b 0168 1d4b  .h.K.h.K.h.K.h.K
+00000370: 2d68 1e4b 0075 8c18 5051 416e 616c 7973  -h.K.u..PQAnalys
+00000380: 6973 2e74 7261 6a2e 5f5f 696e 6974 5f5f  is.traj.__init__
+00000390: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
+000003a0: 681b 4b00 681c 4b00 681d 4b04 681e 4b00  h.K.h.K.h.K.h.K.
+000003b0: 758c 1350 5141 6e61 6c79 7369 732e 7472  u..PQAnalysis.tr
+000003c0: 616a 2e61 7069 947d 9428 6818 4b00 6819  aj.api.}.(h.K.h.
+000003d0: 4b00 681a 4b00 681b 4b00 681c 4b00 681d  K.h.K.h.K.h.K.h.
+000003e0: 4b08 681e 4b00 758c 1a50 5141 6e61 6c79  K.h.K.u..PQAnaly
+000003f0: 7369 732e 7472 616a 2e74 7261 6a65 6374  sis.traj.traject
+00000400: 6f72 7994 7d94 2868 184b 0068 194b 0068  ory.}.(h.K.h.K.h
+00000410: 1a4b 0068 1b4b 0068 1c4b 0068 1d4b 6668  .K.h.K.h.K.h.Kfh
+00000420: 1e4b 0075 8c1a 5051 416e 616c 7973 6973  .K.u..PQAnalysis
+00000430: 2e74 7261 6a2e 6578 6365 7074 696f 6e73  .traj.exceptions
+00000440: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
+00000450: 681b 4b00 681c 4b00 681d 4b07 681e 4b00  h.K.h.K.h.K.h.K.
+00000460: 758c 1950 5141 6e61 6c79 7369 732e 746f  u..PQAnalysis.to
+00000470: 6f6c 732e 5f5f 696e 6974 5f5f 947d 9428  ols.__init__.}.(
+00000480: 6818 4b00 6819 4b00 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
+00000490: 681c 4b00 681d 4b01 681e 4b00 758c 2150  h.K.h.K.h.K.u.!P
+000004a0: 5141 6e61 6c79 7369 732e 746f 6f6c 732e  QAnalysis.tools.
+000004b0: 7472 616a 5f74 6f5f 636f 6d5f 7472 616a  traj_to_com_traj
+000004c0: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
+000004d0: 681b 4b00 681c 4b00 681d 4b0c 681e 4b02  h.K.h.K.h.K.h.K.
+000004e0: 758c 1d50 5141 6e61 6c79 7369 732e 746f  u..PQAnalysis.to
+000004f0: 6f6c 732e 6164 645f 6d6f 6c65 6375 6c65  ols.add_molecule
+00000500: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
+00000510: 681b 4b00 681c 4b04 681d 4b52 681e 4b00  h.K.h.K.h.KRh.K.
+00000520: 758c 2150 5141 6e61 6c79 7369 732e 7068  u.!PQAnalysis.ph
+00000530: 7973 6963 616c 5f64 6174 612e 5f5f 696e  ysical_data.__in
+00000540: 6974 5f5f 947d 9428 6818 4b00 6819 4b00  it__.}.(h.K.h.K.
+00000550: 681a 4b00 681b 4b00 681c 4b00 681d 4b02  h.K.h.K.h.K.h.K.
+00000560: 681e 4b00 758c 1f50 5141 6e61 6c79 7369  h.K.u..PQAnalysi
+00000570: 732e 7068 7973 6963 616c 5f64 6174 612e  s.physical_data.
+00000580: 656e 6572 6779 947d 9428 6818 4b00 6819  energy.}.(h.K.h.
+00000590: 4b00 681a 4b00 681b 4b00 681c 4b00 681d  K.h.K.h.K.h.K.h.
+000005a0: 4b3e 681e 4b00 758c 2350 5141 6e61 6c79  K>h.K.u.#PQAnaly
+000005b0: 7369 732e 7068 7973 6963 616c 5f64 6174  sis.physical_dat
+000005c0: 612e 6578 6365 7074 696f 6e73 947d 9428  a.exceptions.}.(
+000005d0: 6818 4b00 6819 4b00 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
+000005e0: 681c 4b00 681d 4b05 681e 4b00 758c 1950  h.K.h.K.h.K.u..P
+000005f0: 5141 6e61 6c79 7369 732e 7574 696c 732e  QAnalysis.utils.
+00000600: 5f5f 696e 6974 5f5f 947d 9428 6818 4b00  __init__.}.(h.K.
+00000610: 6819 4b00 681a 4b00 681b 4b00 681c 4b00  h.K.h.K.h.K.h.K.
+00000620: 681d 4b02 681e 4b00 758c 1650 5141 6e61  h.K.h.K.u..PQAna
+00000630: 6c79 7369 732e 7574 696c 732e 756e 6974  lysis.utils.unit
+00000640: 7394 7d94 2868 184b 0068 194b 0068 1a4b  s.}.(h.K.h.K.h.K
+00000650: 0068 1b4b 0068 1c4b 0068 1d4b 0768 1e4b  .h.K.h.K.h.K.h.K
+00000660: 0075 8c15 5051 416e 616c 7973 6973 2e75  .u..PQAnalysis.u
+00000670: 7469 6c73 2e6d 6174 6894 7d94 2868 184b  tils.math.}.(h.K
+00000680: 0068 194b 0068 1a4b 0068 1b4b 0068 1c4b  .h.K.h.K.h.K.h.K
+00000690: 0068 1d4b 0768 1e4b 0075 8c16 5051 416e  .h.K.h.K.u..PQAn
+000006a0: 616c 7973 6973 2e75 7469 6c73 2e66 696c  alysis.utils.fil
+000006b0: 6573 947d 9428 6818 4b00 6819 4b00 681a  es.}.(h.K.h.K.h.
+000006c0: 4b00 681b 4b00 681c 4b00 681d 4b0a 681e  K.h.K.h.K.h.K.h.
+000006d0: 4b00 758c 1750 5141 6e61 6c79 7369 732e  K.u..PQAnalysis.
+000006e0: 7574 696c 732e 7261 6e64 6f6d 947d 9428  utils.random.}.(
+000006f0: 6818 4b00 6819 4b00 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
+00000700: 681c 4b00 681d 4b06 681e 4b00 758c 1b50  h.K.h.K.h.K.u..P
+00000710: 5141 6e61 6c79 7369 732e 7574 696c 732e  QAnalysis.utils.
+00000720: 6465 636f 7261 746f 7273 947d 9428 6818  decorators.}.(h.
+00000730: 4b00 6819 4b00 681a 4b00 681b 4b00 681c  K.h.K.h.K.h.K.h.
+00000740: 4b00 681d 4b20 681e 4b00 758c 1f50 5141  K.h.K h.K.u..PQA
+00000750: 6e61 6c79 7369 732e 7574 696c 732e 6375  nalysis.utils.cu
+00000760: 7374 6f6d 5f6c 6f67 6769 6e67 947d 9428  stom_logging.}.(
+00000770: 6818 4b00 6819 4b00 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
+00000780: 681c 4b00 681d 4b65 681e 4b00 758c 1750  h.K.h.Keh.K.u..P
+00000790: 5141 6e61 6c79 7369 732e 7574 696c 732e  QAnalysis.utils.
+000007a0: 636f 6d6d 6f6e 947d 9428 6818 4b00 6819  common.}.(h.K.h.
+000007b0: 4b00 681a 4b00 681b 4b00 681c 4b00 681d  K.h.K.h.K.h.K.h.
+000007c0: 4b09 681e 4b00 758c 1c50 5141 6e61 6c79  K.h.K.u..PQAnaly
+000007d0: 7369 732e 746f 706f 6c6f 6779 2e5f 5f69  sis.topology.__i
+000007e0: 6e69 745f 5f94 7d94 2868 184b 0068 194b  nit__.}.(h.K.h.K
+000007f0: 0068 1a4b 0068 1b4b 0068 1c4b 0068 1d4b  .h.K.h.K.h.K.h.K
+00000800: 0768 1e4b 0275 8c1d 5051 416e 616c 7973  .h.K.u..PQAnalys
+00000810: 6973 2e74 6f70 6f6c 6f67 792e 7365 6c65  is.topology.sele
+00000820: 6374 696f 6e94 7d94 2868 184b 0068 194b  ction.}.(h.K.h.K
+00000830: 0068 1a4b 0068 1b4b 0068 1c4b 0168 1d4b  .h.K.h.K.h.K.h.K
+00000840: 9268 1e4b 0075 8c22 5051 416e 616c 7973  .h.K.u."PQAnalys
+00000850: 6973 2e74 6f70 6f6c 6f67 792e 7368 616b  is.topology.shak
+00000860: 655f 746f 706f 6c6f 6779 947d 9428 6818  e_topology.}.(h.
+00000870: 4b00 6819 4b00 681a 4b00 681b 4b00 681c  K.h.K.h.K.h.K.h.
+00000880: 4b00 681d 4b48 681e 4b00 758c 1750 5141  K.h.KHh.K.u..PQA
+00000890: 6e61 6c79 7369 732e 746f 706f 6c6f 6779  nalysis.topology
+000008a0: 2e61 7069 947d 9428 6818 4b00 6819 4b00  .api.}.(h.K.h.K.
+000008b0: 681a 4b00 681b 4b00 681c 4b00 681d 4b11  h.K.h.K.h.K.h.K.
+000008c0: 681e 4b00 758c 1c50 5141 6e61 6c79 7369  h.K.u..PQAnalysi
+000008d0: 732e 746f 706f 6c6f 6779 2e74 6f70 6f6c  s.topology.topol
+000008e0: 6f67 7994 7d94 2868 184b 0068 194b 0068  ogy.}.(h.K.h.K.h
+000008f0: 1a4b 0068 1b4b 0068 1c4b 0268 1d4b a768  .K.h.K.h.K.h.K.h
+00000900: 1e4b 0075 8c1e 5051 416e 616c 7973 6973  .K.u..PQAnalysis
+00000910: 2e74 6f70 6f6c 6f67 792e 6578 6365 7074  .topology.except
+00000920: 696f 6e73 947d 9428 6818 4b00 6819 4b00  ions.}.(h.K.h.K.
+00000930: 681a 4b00 681b 4b00 681c 4b00 681d 4b05  h.K.h.K.h.K.h.K.
+00000940: 681e 4b00 758c 3850 5141 6e61 6c79 7369  h.K.u.8PQAnalysi
+00000950: 732e 746f 706f 6c6f 6779 2e62 6f6e 6465  s.topology.bonde
+00000960: 645f 746f 706f 6c6f 6779 2e5f 746f 706f  d_topology._topo
+00000970: 6c6f 6779 5f70 726f 7065 7274 6965 7394  logy_properties.
+00000980: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
+00000990: 1b4b 0068 1c4b 0068 1d4b 2e68 1e4b 0075  .K.h.K.h.K.h.K.u
+000009a0: 8c2c 5051 416e 616c 7973 6973 2e74 6f70  .,PQAnalysis.top
+000009b0: 6f6c 6f67 792e 626f 6e64 6564 5f74 6f70  ology.bonded_top
+000009c0: 6f6c 6f67 792e 5f5f 696e 6974 5f5f 947d  ology.__init__.}
+000009d0: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
+000009e0: 4b00 681c 4b00 681d 4b00 681e 4b00 758c  K.h.K.h.K.h.K.u.
+000009f0: 2c50 5141 6e61 6c79 7369 732e 746f 706f  ,PQAnalysis.topo
+00000a00: 6c6f 6779 2e62 6f6e 6465 645f 746f 706f  logy.bonded_topo
+00000a10: 6c6f 6779 2e64 6968 6564 7261 6c94 7d94  logy.dihedral.}.
+00000a20: 2868 184b 0068 194b 0068 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
+00000a30: 0068 1c4b 0268 1d4b 1268 1e4b 0075 8c29  .h.K.h.K.h.K.u.)
+00000a40: 5051 416e 616c 7973 6973 2e74 6f70 6f6c  PQAnalysis.topol
+00000a50: 6f67 792e 626f 6e64 6564 5f74 6f70 6f6c  ogy.bonded_topol
+00000a60: 6f67 792e 616e 676c 6594 7d94 2868 184b  ogy.angle.}.(h.K
+00000a70: 0068 194b 0068 1a4b 0068 1b4b 0068 1c4b  .h.K.h.K.h.K.h.K
+00000a80: 0168 1d4b 1068 1e4b 0075 8c33 5051 416e  .h.K.h.K.u.3PQAn
+00000a90: 616c 7973 6973 2e74 6f70 6f6c 6f67 792e  alysis.topology.
+00000aa0: 626f 6e64 6564 5f74 6f70 6f6c 6f67 792e  bonded_topology.
+00000ab0: 626f 6e64 6564 5f74 6f70 6f6c 6f67 7994  bonded_topology.
+00000ac0: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
+00000ad0: 1b4b 0068 1c4b 0168 1d4b 2468 1e4b 0075  .K.h.K.h.K$h.K.u
+00000ae0: 8c28 5051 416e 616c 7973 6973 2e74 6f70  .(PQAnalysis.top
+00000af0: 6f6c 6f67 792e 626f 6e64 6564 5f74 6f70  ology.bonded_top
+00000b00: 6f6c 6f67 792e 626f 6e64 947d 9428 6818  ology.bond.}.(h.
+00000b10: 4b00 6819 4b00 681a 4b00 681b 4b00 681c  K.h.K.h.K.h.K.h.
+00000b20: 4b01 681d 4b10 681e 4b00 758c 1550 5141  K.h.K.h.K.u..PQA
+00000b30: 6e61 6c79 7369 732e 696f 2e66 6f72 6d61  nalysis.io.forma
+00000b40: 7473 947d 9428 6818 4b00 6819 4b00 681a  ts.}.(h.K.h.K.h.
+00000b50: 4b00 681b 4b00 681c 4b01 681d 4b52 681e  K.h.K.h.K.h.KRh.
+00000b60: 4b00 758c 2250 5141 6e61 6c79 7369 732e  K.u."PQAnalysis.
+00000b70: 696f 2e6d 6f6c 6465 7363 7269 7074 6f72  io.moldescriptor
+00000b80: 5f72 6561 6465 7294 7d94 2868 184b 0068  _reader.}.(h.K.h
+00000b90: 194b 0068 1a4b 0068 1b4b 0068 1c4b 0068  .K.h.K.h.K.h.K.h
+00000ba0: 1d4b 3968 1e4b 0275 8c16 5051 416e 616c  .K9h.K.u..PQAnal
+00000bb0: 7973 6973 2e69 6f2e 5f5f 696e 6974 5f5f  ysis.io.__init__
+00000bc0: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
+00000bd0: 681b 4b00 681c 4b00 681d 4b1a 681e 4b00  h.K.h.K.h.K.h.K.
+00000be0: 758c 1e50 5141 6e61 6c79 7369 732e 696f  u..PQAnalysis.io
+00000bf0: 2e69 6e66 6f5f 6669 6c65 5f72 6561 6465  .info_file_reade
+00000c00: 7294 7d94 2868 184b 0068 194b 0068 1a4b  r.}.(h.K.h.K.h.K
+00000c10: 0068 1b4b 0068 1c4b 0168 1d4b 3768 1e4b  .h.K.h.K.h.K7h.K
+00000c20: 0075 8c20 5051 416e 616c 7973 6973 2e69  .u. PQAnalysis.i
+00000c30: 6f2e 656e 6572 6779 5f66 696c 655f 7265  o.energy_file_re
+00000c40: 6164 6572 947d 9428 6818 4b00 6819 4b00  ader.}.(h.K.h.K.
+00000c50: 681a 4b00 681b 4b00 681c 4b00 681d 4b2e  h.K.h.K.h.K.h.K.
+00000c60: 681e 4b00 758c 1150 5141 6e61 6c79 7369  h.K.u..PQAnalysi
+00000c70: 732e 696f 2e61 7069 947d 9428 6818 4b00  s.io.api.}.(h.K.
+00000c80: 6819 4b00 681a 4b00 681b 4b00 681c 4b00  h.K.h.K.h.K.h.K.
+00000c90: 681d 4b11 681e 4b00 758c 1c50 5141 6e61  h.K.h.K.u..PQAna
+00000ca0: 6c79 7369 732e 696f 2e63 6f6e 7665 7273  lysis.io.convers
+00000cb0: 696f 6e5f 6170 6994 7d94 2868 184b 0068  ion_api.}.(h.K.h
+00000cc0: 194b 0068 1a4b 0068 1b4b 0068 1c4b 0068  .K.h.K.h.K.h.K.h
+00000cd0: 1d4b 2768 1e4b 0075 8c18 5051 416e 616c  .K'h.K.u..PQAnal
+00000ce0: 7973 6973 2e69 6f2e 626f 785f 7772 6974  ysis.io.box_writ
+00000cf0: 6572 947d 9428 6818 4b00 6819 4b00 681a  er.}.(h.K.h.K.h.
+00000d00: 4b00 681b 4b00 681c 4b00 681d 4b2c 681e  K.h.K.h.K.h.K,h.
+00000d10: 4b00 758c 1250 5141 6e61 6c79 7369 732e  K.u..PQAnalysis.
+00000d20: 696f 2e62 6173 6594 7d94 2868 184b 0068  io.base.}.(h.K.h
+00000d30: 194b 0068 1a4b 0068 1b4b 0068 1c4b 0068  .K.h.K.h.K.h.K.h
+00000d40: 1d4b 3268 1e4b 0075 8c17 5051 416e 616c  .K2h.K.u..PQAnal
+00000d50: 7973 6973 2e69 6f2e 7772 6974 655f 6170  ysis.io.write_ap
+00000d60: 6994 7d94 2868 184b 0068 194b 0068 1a4b  i.}.(h.K.h.K.h.K
+00000d70: 0068 1b4b 0068 1c4b 0068 1d4b 1468 1e4b  .h.K.h.K.h.K.h.K
+00000d80: 0175 8c18 5051 416e 616c 7973 6973 2e69  .u..PQAnalysis.i
+00000d90: 6f2e 6578 6365 7074 696f 6e73 947d 9428  o.exceptions.}.(
+00000da0: 6818 4b00 6819 4b00 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
+00000db0: 681c 4b00 681d 4b06 681e 4b00 758c 2250  h.K.h.K.h.K.u."P
+00000dc0: 5141 6e61 6c79 7369 732e 696f 2e76 6972  QAnalysis.io.vir
+00000dd0: 6961 6c2e 7669 7269 616c 5f72 6561 6465  ial.virial_reade
+00000de0: 7294 7d94 2868 184b 0068 194b 0068 1a4b  r.}.(h.K.h.K.h.K
+00000df0: 0068 1b4b 0068 1c4b 0068 1d4b 1468 1e4b  .h.K.h.K.h.K.h.K
+00000e00: 0075 8c1d 5051 416e 616c 7973 6973 2e69  .u..PQAnalysis.i
+00000e10: 6f2e 7669 7269 616c 2e5f 5f69 6e69 745f  o.virial.__init_
+00000e20: 5f94 7d94 2868 184b 0068 194b 0068 1a4b  _.}.(h.K.h.K.h.K
+00000e30: 0068 1b4b 0068 1c4b 0068 1d4b 0168 1e4b  .h.K.h.K.h.K.h.K
+00000e40: 0075 8c18 5051 416e 616c 7973 6973 2e69  .u..PQAnalysis.i
+00000e50: 6f2e 7669 7269 616c 2e61 7069 947d 9428  o.virial.api.}.(
+00000e60: 6818 4b00 6819 4b00 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
+00000e70: 681c 4b00 681d 4b09 681e 4b00 758c 2050  h.K.h.K.h.K.u. P
+00000e80: 5141 6e61 6c79 7369 732e 696f 2e74 7261  QAnalysis.io.tra
+00000e90: 6a5f 6669 6c65 2e5f 5f69 6e69 745f 5f94  j_file.__init__.
+00000ea0: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
+00000eb0: 1b4b 0068 1c4b 0068 1d4b 0368 1e4b 0075  .K.h.K.h.K.h.K.u
+00000ec0: 8c29 5051 416e 616c 7973 6973 2e69 6f2e  .)PQAnalysis.io.
+00000ed0: 7472 616a 5f66 696c 652e 7472 616a 6563  traj_file.trajec
+00000ee0: 746f 7279 5f77 7269 7465 7294 7d94 2868  tory_writer.}.(h
+00000ef0: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
+00000f00: 1c4b 0068 1d4b 4f68 1e4b 0075 8c1b 5051  .K.h.KOh.K.u..PQ
+00000f10: 416e 616c 7973 6973 2e69 6f2e 7472 616a  Analysis.io.traj
+00000f20: 5f66 696c 652e 6170 6994 7d94 2868 184b  _file.api.}.(h.K
+00000f30: 0068 194b 0168 1a4b 0068 1b4b 0068 1c4b  .h.K.h.K.h.K.h.K
+00000f40: 0068 1d4b 1368 1e4b 0075 8c29 5051 416e  .h.K.h.K.u.)PQAn
+00000f50: 616c 7973 6973 2e69 6f2e 7472 616a 5f66  alysis.io.traj_f
+00000f60: 696c 652e 7472 616a 6563 746f 7279 5f72  ile.trajectory_r
+00000f70: 6561 6465 7294 7d94 2868 184b 0068 194b  eader.}.(h.K.h.K
+00000f80: 0068 1a4b 0068 1b4b 0068 1c4b 0568 1d4b  .h.K.h.K.h.K.h.K
+00000f90: a768 1e4b 0075 8c24 5051 416e 616c 7973  .h.K.u.$PQAnalys
+00000fa0: 6973 2e69 6f2e 7472 616a 5f66 696c 652e  is.io.traj_file.
+00000fb0: 6672 616d 655f 7265 6164 6572 947d 9428  frame_reader.}.(
+00000fc0: 6818 4b00 6819 4b02 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
+00000fd0: 681c 4b02 681d 4b6e 681e 4b00 758c 2250  h.K.h.Knh.K.u."P
+00000fe0: 5141 6e61 6c79 7369 732e 696f 2e74 7261  QAnalysis.io.tra
+00000ff0: 6a5f 6669 6c65 2e65 7863 6570 7469 6f6e  j_file.exception
+00001000: 7394 7d94 2868 184b 0068 194b 0068 1a4b  s.}.(h.K.h.K.h.K
+00001010: 0068 1b4b 0068 1c4b 0068 1d4b 0368 1e4b  .h.K.h.K.h.K.h.K
+00001020: 0075 8c1c 5051 416e 616c 7973 6973 2e69  .u..PQAnalysis.i
+00001030: 6f2e 6e65 702e 6e65 705f 7772 6974 6572  o.nep.nep_writer
+00001040: 947d 9428 6818 4b01 6819 4b04 681a 4b00  .}.(h.K.h.K.h.K.
+00001050: 681b 4b00 681c 4b08 681d 4d16 0168 1e4b  h.K.h.K.h.M..h.K
+00001060: 0075 8c1a 5051 416e 616c 7973 6973 2e69  .u..PQAnalysis.i
+00001070: 6f2e 6e65 702e 5f5f 696e 6974 5f5f 947d  o.nep.__init__.}
+00001080: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
+00001090: 4b00 681c 4b00 681d 4b00 681e 4b00 758c  K.h.K.h.K.h.K.u.
+000010a0: 1c50 5141 6e61 6c79 7369 732e 696f 2e6e  .PQAnalysis.io.n
+000010b0: 6570 2e65 7863 6570 7469 6f6e 7394 7d94  ep.exceptions.}.
+000010c0: 2868 184b 0068 194b 0068 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
+000010d0: 0068 1c4b 0068 1d4b 0268 1e4b 0075 8c23  .h.K.h.K.h.K.u.#
+000010e0: 5051 416e 616c 7973 6973 2e69 6f2e 7265  PQAnalysis.io.re
+000010f0: 7374 6172 745f 6669 6c65 2e5f 5f69 6e69  start_file.__ini
+00001100: 745f 5f94 7d94 2868 184b 0068 194b 0068  t__.}.(h.K.h.K.h
+00001110: 1a4b 0068 1b4b 0068 1c4b 0068 1d4b 0268  .K.h.K.h.K.h.K.h
+00001120: 1e4b 0075 8c29 5051 416e 616c 7973 6973  .K.u.)PQAnalysis
+00001130: 2e69 6f2e 7265 7374 6172 745f 6669 6c65  .io.restart_file
+00001140: 2e72 6573 7461 7274 5f77 7269 7465 7294  .restart_writer.
+00001150: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
+00001160: 1b4b 0068 1c4b 0068 1d4b 3d68 1e4b 0075  .K.h.K.h.K=h.K.u
+00001170: 8c29 5051 416e 616c 7973 6973 2e69 6f2e  .)PQAnalysis.io.
+00001180: 7265 7374 6172 745f 6669 6c65 2e72 6573  restart_file.res
+00001190: 7461 7274 5f72 6561 6465 7294 7d94 2868  tart_reader.}.(h
+000011a0: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
+000011b0: 1c4b 0168 1d4b 4968 1e4b 0075 8c1e 5051  .K.h.KIh.K.u..PQ
+000011c0: 416e 616c 7973 6973 2e69 6f2e 7265 7374  Analysis.io.rest
+000011d0: 6172 745f 6669 6c65 2e61 7069 947d 9428  art_file.api.}.(
+000011e0: 6818 4b00 6819 4b00 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
+000011f0: 681c 4b00 681d 4b08 681e 4b00 758c 2550  h.K.h.K.h.K.u.%P
+00001200: 5141 6e61 6c79 7369 732e 696f 2e72 6573  QAnalysis.io.res
+00001210: 7461 7274 5f66 696c 652e 6578 6365 7074  tart_file.except
+00001220: 696f 6e73 947d 9428 6818 4b00 6819 4b00  ions.}.(h.K.h.K.
+00001230: 681a 4b00 681b 4b00 681c 4b00 681d 4b03  h.K.h.K.h.K.h.K.
+00001240: 681e 4b00 758c 3050 5141 6e61 6c79 7369  h.K.u.0PQAnalysi
+00001250: 732e 696f 2e74 6f70 6f6c 6f67 795f 6669  s.io.topology_fi
+00001260: 6c65 2e74 6f70 6f6c 6f67 795f 6669 6c65  le.topology_file
+00001270: 5f72 6561 6465 7294 7d94 2868 184b 0068  _reader.}.(h.K.h
+00001280: 194b 1568 1a4b 0068 1b4b 0068 1c4b 0068  .K.h.K.h.K.h.K.h
+00001290: 1d4b 7168 1e4b 0075 8c24 5051 416e 616c  .Kqh.K.u.$PQAnal
+000012a0: 7973 6973 2e69 6f2e 746f 706f 6c6f 6779  ysis.io.topology
+000012b0: 5f66 696c 652e 5f5f 696e 6974 5f5f 947d  _file.__init__.}
+000012c0: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
+000012d0: 4b00 681c 4b00 681d 4b02 681e 4b00 758c  K.h.K.h.K.h.K.u.
+000012e0: 1f50 5141 6e61 6c79 7369 732e 696f 2e74  .PQAnalysis.io.t
+000012f0: 6f70 6f6c 6f67 795f 6669 6c65 2e61 7069  opology_file.api
+00001300: 947d 9428 6818 4b00 6819 4b00 681a 4b00  .}.(h.K.h.K.h.K.
+00001310: 681b 4b00 681c 4b00 681d 4b09 681e 4b00  h.K.h.K.h.K.h.K.
+00001320: 758c 3050 5141 6e61 6c79 7369 732e 696f  u.0PQAnalysis.io
+00001330: 2e74 6f70 6f6c 6f67 795f 6669 6c65 2e74  .topology_file.t
+00001340: 6f70 6f6c 6f67 795f 6669 6c65 5f77 7269  opology_file_wri
+00001350: 7465 7294 7d94 2868 184b 0068 194b 0068  ter.}.(h.K.h.K.h
+00001360: 1a4b 0068 1b4b 0068 1c4b 0068 1d4b 6b68  .K.h.K.h.K.h.Kkh
+00001370: 1e4b 0075 8c26 5051 416e 616c 7973 6973  .K.u.&PQAnalysis
+00001380: 2e69 6f2e 746f 706f 6c6f 6779 5f66 696c  .io.topology_fil
+00001390: 652e 6578 6365 7074 696f 6e73 947d 9428  e.exceptions.}.(
+000013a0: 6818 4b00 6819 4b00 681a 4b00 681b 4b00  h.K.h.K.h.K.h.K.
+000013b0: 681c 4b00 681d 4b02 681e 4b00 758c 2750  h.K.h.K.h.K.u.'P
+000013c0: 5141 6e61 6c79 7369 732e 696f 2e69 6e70  QAnalysis.io.inp
+000013d0: 7574 5f66 696c 655f 7265 6164 6572 2e66  ut_file_reader.f
+000013e0: 6f72 6d61 7473 947d 9428 6818 4b00 6819  ormats.}.(h.K.h.
+000013f0: 4b00 681a 4b00 681b 4b00 681c 4b00 681d  K.h.K.h.K.h.K.h.
+00001400: 4b0f 681e 4b00 758c 2850 5141 6e61 6c79  K.h.K.u.(PQAnaly
+00001410: 7369 732e 696f 2e69 6e70 7574 5f66 696c  sis.io.input_fil
+00001420: 655f 7265 6164 6572 2e5f 5f69 6e69 745f  e_reader.__init_
+00001430: 5f94 7d94 2868 184b 0068 194b 0068 1a4b  _.}.(h.K.h.K.h.K
+00001440: 0068 1b4b 0068 1c4b 0068 1d4b 0468 1e4b  .h.K.h.K.h.K.h.K
+00001450: 0075 8c31 5051 416e 616c 7973 6973 2e69  .u.1PQAnalysis.i
+00001460: 6f2e 696e 7075 745f 6669 6c65 5f72 6561  o.input_file_rea
+00001470: 6465 722e 696e 7075 745f 6669 6c65 5f70  der.input_file_p
+00001480: 6172 7365 7294 7d94 2868 184b 0068 194b  arser.}.(h.K.h.K
+00001490: 0168 1a4b 0068 1b4b 0068 1c4b 0168 1d4b  .h.K.h.K.h.K.h.K
+000014a0: 7f68 1e4b 0075 8c2a 5051 416e 616c 7973  .h.K.u.*PQAnalys
+000014b0: 6973 2e69 6f2e 696e 7075 745f 6669 6c65  is.io.input_file
+000014c0: 5f72 6561 6465 722e 6578 6365 7074 696f  _reader.exceptio
+000014d0: 6e73 947d 9428 6818 4b00 6819 4b00 681a  ns.}.(h.K.h.K.h.
+000014e0: 4b00 681b 4b00 681c 4b00 681d 4b0e 681e  K.h.K.h.K.h.K.h.
+000014f0: 4b00 758c 3c50 5141 6e61 6c79 7369 732e  K.u.<PQAnalysis.
+00001500: 696f 2e69 6e70 7574 5f66 696c 655f 7265  io.input_file_re
+00001510: 6164 6572 2e70 715f 616e 616c 7973 6973  ader.pq_analysis
+00001520: 2e5f 7365 6c65 6374 696f 6e5f 6d69 7869  ._selection_mixi
+00001530: 6e94 7d94 2868 184b 0068 194b 0068 1a4b  n.}.(h.K.h.K.h.K
+00001540: 0068 1b4b 0068 1c4b 0068 1d4b 0c68 1e4b  .h.K.h.K.h.K.h.K
+00001550: 0075 8c34 5051 416e 616c 7973 6973 2e69  .u.4PQAnalysis.i
+00001560: 6f2e 696e 7075 745f 6669 6c65 5f72 6561  o.input_file_rea
+00001570: 6465 722e 7071 5f61 6e61 6c79 7369 732e  der.pq_analysis.
+00001580: 5f5f 696e 6974 5f5f 947d 9428 6818 4b00  __init__.}.(h.K.
+00001590: 6819 4b00 681a 4b00 681b 4b00 681c 4b00  h.K.h.K.h.K.h.K.
+000015a0: 681d 4b01 681e 4b00 758c 3250 5141 6e61  h.K.h.K.u.2PQAna
+000015b0: 6c79 7369 732e 696f 2e69 6e70 7574 5f66  lysis.io.input_f
+000015c0: 696c 655f 7265 6164 6572 2e70 715f 616e  ile_reader.pq_an
+000015d0: 616c 7973 6973 2e5f 7061 7273 6594 7d94  alysis._parse.}.
+000015e0: 2868 184b 0068 194b 0068 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
+000015f0: 0068 1c4b 0168 1d4b 4468 1e4b 0075 8c37  .h.K.h.KDh.K.u.7
+00001600: 5051 416e 616c 7973 6973 2e69 6f2e 696e  PQAnalysis.io.in
+00001610: 7075 745f 6669 6c65 5f72 6561 6465 722e  put_file_reader.
+00001620: 7071 5f61 6e61 6c79 7369 732e 5f66 696c  pq_analysis._fil
+00001630: 655f 6d69 7869 6e94 7d94 2868 184b 0068  e_mixin.}.(h.K.h
+00001640: 194b 0068 1a4b 0068 1b4b 0068 1c4b 0068  .K.h.K.h.K.h.K.h
+00001650: 1d4b 0d68 1e4b 0075 8c3c 5051 416e 616c  .K.h.K.u.<PQAnal
+00001660: 7973 6973 2e69 6f2e 696e 7075 745f 6669  ysis.io.input_fi
+00001670: 6c65 5f72 6561 6465 722e 7071 5f61 6e61  le_reader.pq_ana
+00001680: 6c79 7369 732e 5f70 6f73 6974 696f 6e73  lysis._positions
+00001690: 5f6d 6978 696e 947d 9428 6818 4b00 6819  _mixin.}.(h.K.h.
+000016a0: 4b00 681a 4b00 681b 4b00 681c 4b00 681d  K.h.K.h.K.h.K.h.
+000016b0: 4b0b 681e 4b00 758c 4850 5141 6e61 6c79  K.h.K.u.HPQAnaly
+000016c0: 7369 732e 696f 2e69 6e70 7574 5f66 696c  sis.io.input_fil
+000016d0: 655f 7265 6164 6572 2e70 715f 616e 616c  e_reader.pq_anal
+000016e0: 7973 6973 2e70 7161 6e61 6c79 7369 735f  ysis.pqanalysis_
+000016f0: 696e 7075 745f 6669 6c65 5f72 6561 6465  input_file_reade
+00001700: 7294 7d94 2868 184b 0068 194b 0068 1a4b  r.}.(h.K.h.K.h.K
+00001710: 0068 1b4b 0068 1c4b 0068 1d4b 3b68 1e4b  .h.K.h.K.h.K;h.K
+00001720: 0075 8c2b 5051 416e 616c 7973 6973 2e69  .u.+PQAnalysis.i
+00001730: 6f2e 696e 7075 745f 6669 6c65 5f72 6561  o.input_file_rea
+00001740: 6465 722e 7071 2e5f 5f69 6e69 745f 5f94  der.pq.__init__.
+00001750: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
+00001760: 1b4b 0068 1c4b 0068 1d4b 0168 1e4b 0075  .K.h.K.h.K.h.K.u
+00001770: 8c37 5051 416e 616c 7973 6973 2e69 6f2e  .7PQAnalysis.io.
+00001780: 696e 7075 745f 6669 6c65 5f72 6561 6465  input_file_reade
+00001790: 722e 7071 2e70 715f 696e 7075 745f 6669  r.pq.pq_input_fi
+000017a0: 6c65 5f72 6561 6465 7294 7d94 2868 184b  le_reader.}.(h.K
+000017b0: 0068 194b 0068 1a4b 0068 1b4b 0068 1c4b  .h.K.h.K.h.K.h.K
+000017c0: 0168 1d4b 5868 1e4b 0075 8c2f 5051 416e  .h.KXh.K.u./PQAn
+000017d0: 616c 7973 6973 2e69 6f2e 696e 7075 745f  alysis.io.input_
+000017e0: 6669 6c65 5f72 6561 6465 722e 7071 2e6f  file_reader.pq.o
+000017f0: 7574 7075 745f 6669 6c65 7394 7d94 2868  utput_files.}.(h
+00001800: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
+00001810: 1c4b 0068 1d4b 3268 1e4b 0075 8c1f 5051  .K.h.K2h.K.u..PQ
+00001820: 416e 616c 7973 6973 2e69 6f2e 6765 6e5f  Analysis.io.gen_
+00001830: 6669 6c65 2e5f 5f69 6e69 745f 5f94 7d94  file.__init__.}.
+00001840: 2868 184b 0068 194b 0068 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
+00001850: 0068 1c4b 0068 1d4b 0368 1e4b 0075 8c26  .h.K.h.K.h.K.u.&
+00001860: 5051 416e 616c 7973 6973 2e69 6f2e 6765  PQAnalysis.io.ge
+00001870: 6e5f 6669 6c65 2e67 656e 5f66 696c 655f  n_file.gen_file_
+00001880: 7772 6974 6572 947d 9428 6818 4b00 6819  writer.}.(h.K.h.
+00001890: 4b00 681a 4b00 681b 4b00 681c 4b00 681d  K.h.K.h.K.h.K.h.
+000018a0: 4b2c 681e 4b00 758c 1a50 5141 6e61 6c79  K,h.K.u..PQAnaly
+000018b0: 7369 732e 696f 2e67 656e 5f66 696c 652e  sis.io.gen_file.
+000018c0: 6170 6994 7d94 2868 184b 0068 194b 0068  api.}.(h.K.h.K.h
+000018d0: 1a4b 0068 1b4b 0068 1c4b 0068 1d4b 0968  .K.h.K.h.K.h.K.h
+000018e0: 1e4b 0075 8c21 5051 416e 616c 7973 6973  .K.u.!PQAnalysis
+000018f0: 2e69 6f2e 6765 6e5f 6669 6c65 2e65 7863  .io.gen_file.exc
+00001900: 6570 7469 6f6e 7394 7d94 2868 184b 0068  eptions.}.(h.K.h
+00001910: 194b 0068 1a4b 0068 1b4b 0068 1c4b 0068  .K.h.K.h.K.h.K.h
+00001920: 1d4b 0268 1e4b 0075 8c26 5051 416e 616c  .K.h.K.u.&PQAnal
+00001930: 7973 6973 2e69 6f2e 6765 6e5f 6669 6c65  ysis.io.gen_file
+00001940: 2e67 656e 5f66 696c 655f 7265 6164 6572  .gen_file_reader
+00001950: 947d 9428 6818 4b00 6819 4b01 681a 4b00  .}.(h.K.h.K.h.K.
+00001960: 681b 4b00 681c 4b00 681d 4b2f 681e 4b00  h.K.h.K.h.K/h.K.
+00001970: 758c 1c50 5141 6e61 6c79 7369 732e 616e  u..PQAnalysis.an
+00001980: 616c 7973 6973 2e5f 5f69 6e69 745f 5f94  alysis.__init__.
+00001990: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
+000019a0: 1b4b 0068 1c4b 0068 1d4b 0168 1e4b 0075  .K.h.K.h.K.h.K.u
+000019b0: 8c20 5051 416e 616c 7973 6973 2e61 6e61  . PQAnalysis.ana
+000019c0: 6c79 7369 732e 7264 662e 5f5f 696e 6974  lysis.rdf.__init
+000019d0: 5f5f 947d 9428 6818 4b00 6819 4b00 681a  __.}.(h.K.h.K.h.
+000019e0: 4b00 681b 4b00 681c 4b00 681d 4b05 681e  K.h.K.h.K.h.K.h.
+000019f0: 4b00 758c 2e50 5141 6e61 6c79 7369 732e  K.u..PQAnalysis.
+00001a00: 616e 616c 7973 6973 2e72 6466 2e72 6466  analysis.rdf.rdf
+00001a10: 5f6f 7574 7075 745f 6669 6c65 5f77 7269  _output_file_wri
+00001a20: 7465 7294 7d94 2868 184b 0068 194b 0068  ter.}.(h.K.h.K.h
+00001a30: 1a4b 0068 1b4b 0068 1c4b 0068 1d4b 3368  .K.h.K.h.K.h.K3h
+00001a40: 1e4b 0075 8c1b 5051 416e 616c 7973 6973  .K.u..PQAnalysis
+00001a50: 2e61 6e61 6c79 7369 732e 7264 662e 7264  .analysis.rdf.rd
+00001a60: 6694 7d94 2868 184b 0068 194b 0068 1a4b  f.}.(h.K.h.K.h.K
+00001a70: 0068 1b4b 0068 1c4b 0368 1d4b 9a68 1e4b  .h.K.h.K.h.K.h.K
+00001a80: 0075 8c1b 5051 416e 616c 7973 6973 2e61  .u..PQAnalysis.a
+00001a90: 6e61 6c79 7369 732e 7264 662e 6170 6994  nalysis.rdf.api.
+00001aa0: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
+00001ab0: 1b4b 0068 1c4b 0068 1d4b 1e68 1e4b 0075  .K.h.K.h.K.h.K.u
+00001ac0: 8c2d 5051 416e 616c 7973 6973 2e61 6e61  .-PQAnalysis.ana
+00001ad0: 6c79 7369 732e 7264 662e 7264 665f 696e  lysis.rdf.rdf_in
+00001ae0: 7075 745f 6669 6c65 5f72 6561 6465 7294  put_file_reader.
+00001af0: 7d94 2868 184b 0068 194b 0068 1a4b 0068  }.(h.K.h.K.h.K.h
+00001b00: 1b4b 0068 1c4b 0068 1d4b 1868 1e4b 0075  .K.h.K.h.K.h.K.u
+00001b10: 8c22 5051 416e 616c 7973 6973 2e61 6e61  ."PQAnalysis.ana
+00001b20: 6c79 7369 732e 7264 662e 6578 6365 7074  lysis.rdf.except
+00001b30: 696f 6e73 947d 9428 6818 4b00 6819 4b00  ions.}.(h.K.h.K.
+00001b40: 681a 4b00 681b 4b00 681c 4b00 681d 4b09  h.K.h.K.h.K.h.K.
+00001b50: 681e 4b00 758c 1750 5141 6e61 6c79 7369  h.K.u..PQAnalysi
+00001b60: 732e 636c 692e 5f5f 696e 6974 5f5f 947d  s.cli.__init__.}
+00001b70: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
+00001b80: 4b00 681c 4b00 681d 4b02 681e 4b00 758c  K.h.K.h.K.h.K.u.
+00001b90: 1350 5141 6e61 6c79 7369 732e 636c 692e  .PQAnalysis.cli.
+00001ba0: 6d61 696e 947d 9428 6818 4b00 6819 4b00  main.}.(h.K.h.K.
+00001bb0: 681a 4b00 681b 4b00 681c 4b00 681d 4b1c  h.K.h.K.h.K.h.K.
+00001bc0: 681e 4b00 758c 1650 5141 6e61 6c79 7369  h.K.u..PQAnalysi
+00001bd0: 732e 636c 692e 7879 7a32 6765 6e94 7d94  s.cli.xyz2gen.}.
+00001be0: 2868 184b 0068 194b 0068 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
+00001bf0: 0068 1c4b 0068 1d4b 1b68 1e4b 0075 8c12  .h.K.h.K.h.K.u..
+00001c00: 5051 416e 616c 7973 6973 2e63 6c69 2e72  PQAnalysis.cli.r
+00001c10: 6466 947d 9428 6818 4b00 6819 4b00 681a  df.}.(h.K.h.K.h.
+00001c20: 4b00 681b 4b00 681c 4b00 681d 4b1f 681e  K.h.K.h.K.h.K.h.
+00001c30: 4b00 758c 1850 5141 6e61 6c79 7369 732e  K.u..PQAnalysis.
+00001c40: 636c 692e 5f63 6c69 5f62 6173 6594 7d94  cli._cli_base.}.
+00001c50: 2868 184b 0068 194b 0068 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
+00001c60: 0068 1c4b 0068 1d4b 0568 1e4b 0075 8c19  .h.K.h.K.h.K.u..
+00001c70: 5051 416e 616c 7973 6973 2e63 6c69 2e74  PQAnalysis.cli.t
+00001c80: 7261 6a32 716d 6366 6394 7d94 2868 184b  raj2qmcfc.}.(h.K
+00001c90: 0068 194b 0068 1a4b 0068 1b4b 0068 1c4b  .h.K.h.K.h.K.h.K
+00001ca0: 0068 1d4b 1968 1e4b 0075 8c1c 5051 416e  .h.K.h.K.u..PQAn
+00001cb0: 616c 7973 6973 2e63 6c69 2e61 6464 5f6d  alysis.cli.add_m
+00001cc0: 6f6c 6563 756c 6573 947d 9428 6818 4b00  olecules.}.(h.K.
+00001cd0: 6819 4b00 681a 4b00 681b 4b00 681c 4b00  h.K.h.K.h.K.h.K.
+00001ce0: 681d 4b28 681e 4b00 758c 1d50 5141 6e61  h.K(h.K.u..PQAna
+00001cf0: 6c79 7369 732e 636c 692e 6275 696c 645f  lysis.cli.build_
+00001d00: 6e65 705f 7472 616a 947d 9428 6818 4b00  nep_traj.}.(h.K.
+00001d10: 6819 4b00 681a 4b00 681b 4b00 681c 4b00  h.K.h.K.h.K.h.K.
+00001d20: 681d 4b1f 681e 4b00 758c 1f50 5141 6e61  h.K.h.K.u..PQAna
+00001d30: 6c79 7369 732e 636c 692e 5f61 7267 756d  lysis.cli._argum
+00001d40: 656e 745f 7061 7273 6572 947d 9428 6818  ent_parser.}.(h.
+00001d50: 4b00 6819 4b00 681a 4b00 681b 4b00 681c  K.h.K.h.K.h.K.h.
+00001d60: 4b00 681d 4b33 681e 4b00 758c 1750 5141  K.h.K3h.K.u..PQA
+00001d70: 6e61 6c79 7369 732e 636c 692e 7472 616a  nalysis.cli.traj
+00001d80: 3262 6f78 947d 9428 6818 4b00 6819 4b00  2box.}.(h.K.h.K.
+00001d90: 681a 4b00 681b 4b00 681c 4b00 681d 4b1a  h.K.h.K.h.K.h.K.
+00001da0: 681e 4b00 758c 1650 5141 6e61 6c79 7369  h.K.u..PQAnalysi
+00001db0: 732e 636c 692e 6765 6e32 7879 7a94 7d94  s.cli.gen2xyz.}.
+00001dc0: 2868 184b 0068 194b 0068 1a4b 0068 1b4b  (h.K.h.K.h.K.h.K
+00001dd0: 0068 1c4b 0068 1d4b 1b68 1e4b 0075 8c16  .h.K.h.K.h.K.u..
+00001de0: 5051 416e 616c 7973 6973 2e63 6c69 2e72  PQAnalysis.cli.r
+00001df0: 7374 3278 797a 947d 9428 6818 4b00 6819  st2xyz.}.(h.K.h.
+00001e00: 4b00 681a 4b00 681b 4b00 681c 4b00 681d  K.h.K.h.K.h.K.h.
+00001e10: 4b1b 681e 4b00 758c 1d50 5141 6e61 6c79  K.h.K.u..PQAnaly
+00001e20: 7369 732e 636c 692e 636f 6e74 696e 7565  sis.cli.continue
+00001e30: 5f69 6e70 7574 947d 9428 6818 4b00 6819  _input.}.(h.K.h.
+00001e40: 4b00 681a 4b00 681b 4b00 681c 4b00 681d  K.h.K.h.K.h.K.h.
+00001e50: 4b1a 681e 4b00 758c 1850 5141 6e61 6c79  K.h.K.u..PQAnaly
+00001e60: 7369 732e 636f 7265 2e5f 5f69 6e69 745f  sis.core.__init_
+00001e70: 5f94 7d94 2868 184b 0068 194b 0068 1a4b  _.}.(h.K.h.K.h.K
+00001e80: 0068 1b4b 0068 1c4b 0068 1d4b 0568 1e4b  .h.K.h.K.h.K.h.K
+00001e90: 0075 8c17 5051 416e 616c 7973 6973 2e63  .u..PQAnalysis.c
+00001ea0: 6f72 652e 7265 7369 6475 6594 7d94 2868  ore.residue.}.(h
+00001eb0: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
+00001ec0: 1c4b 0268 1d4b 5068 1e4b 0075 8c13 5051  .K.h.KPh.K.u..PQ
+00001ed0: 416e 616c 7973 6973 2e63 6f72 652e 6170  Analysis.core.ap
+00001ee0: 6994 7d94 2868 184b 0068 194b 0068 1a4b  i.}.(h.K.h.K.h.K
+00001ef0: 0068 1b4b 0068 1c4b 0068 1d4b 0968 1e4b  .h.K.h.K.h.K.h.K
+00001f00: 0175 8c1a 5051 416e 616c 7973 6973 2e63  .u..PQAnalysis.c
+00001f10: 6f72 652e 6578 6365 7074 696f 6e73 947d  ore.exceptions.}
+00001f20: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
+00001f30: 4b00 681c 4b00 681d 4b10 681e 4b00 758c  K.h.K.h.K.h.K.u.
+00001f40: 1d50 5141 6e61 6c79 7369 732e 636f 7265  .PQAnalysis.core
+00001f50: 2e63 656c 6c2e 5f5f 696e 6974 5f5f 947d  .cell.__init__.}
+00001f60: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
+00001f70: 4b00 681c 4b00 681d 4b01 681e 4b00 758c  K.h.K.h.K.h.K.u.
+00001f80: 2950 5141 6e61 6c79 7369 732e 636f 7265  )PQAnalysis.core
+00001f90: 2e63 656c 6c2e 5f73 7461 6e64 6172 645f  .cell._standard_
+00001fa0: 7072 6f70 6572 7469 6573 947d 9428 6818  properties.}.(h.
+00001fb0: 4b00 6819 4b00 681a 4b00 681b 4b00 681c  K.h.K.h.K.h.K.h.
+00001fc0: 4b00 681d 4b24 681e 4b00 758c 1950 5141  K.h.K$h.K.u..PQA
+00001fd0: 6e61 6c79 7369 732e 636f 7265 2e63 656c  nalysis.core.cel
+00001fe0: 6c2e 6365 6c6c 947d 9428 6818 4b00 6819  l.cell.}.(h.K.h.
+00001ff0: 4b00 681a 4b00 681b 4b00 681c 4b01 681d  K.h.K.h.K.h.K.h.
+00002000: 4b53 681e 4b00 758c 1d50 5141 6e61 6c79  KSh.K.u..PQAnaly
+00002010: 7369 732e 636f 7265 2e61 746f 6d2e 5f5f  sis.core.atom.__
+00002020: 696e 6974 5f5f 947d 9428 6818 4b00 6819  init__.}.(h.K.h.
+00002030: 4b00 681a 4b00 681b 4b00 681c 4b00 681d  K.h.K.h.K.h.K.h.
+00002040: 4b02 681e 4b00 758c 1950 5141 6e61 6c79  K.h.K.u..PQAnaly
+00002050: 7369 732e 636f 7265 2e61 746f 6d2e 6174  sis.core.atom.at
+00002060: 6f6d 947d 9428 6818 4b00 6819 4b00 681a  om.}.(h.K.h.K.h.
+00002070: 4b00 681b 4b00 681c 4b00 681d 4b39 681e  K.h.K.h.K.h.K9h.
+00002080: 4b00 758c 1c50 5141 6e61 6c79 7369 732e  K.u..PQAnalysis.
+00002090: 636f 7265 2e61 746f 6d2e 656c 656d 656e  core.atom.elemen
+000020a0: 7494 7d94 2868 184b 0068 194b 0068 1a4b  t.}.(h.K.h.K.h.K
+000020b0: 0068 1b4b 0068 1c4b 0068 1d4b 3468 1e4b  .h.K.h.K.h.K4h.K
+000020c0: 0075 8c21 5051 416e 616c 7973 6973 2e61  .u.!PQAnalysis.a
+000020d0: 746f 6d69 635f 7379 7374 656d 2e5f 5f69  tomic_system.__i
+000020e0: 6e69 745f 5f94 7d94 2868 184b 0068 194b  nit__.}.(h.K.h.K
+000020f0: 0068 1a4b 0068 1b4b 0068 1c4b 0068 1d4b  .h.K.h.K.h.K.h.K
+00002100: 0268 1e4b 0075 8c26 5051 416e 616c 7973  .h.K.u.&PQAnalys
+00002110: 6973 2e61 746f 6d69 635f 7379 7374 656d  is.atomic_system
+00002120: 2e61 746f 6d69 635f 7379 7374 656d 947d  .atomic_system.}
+00002130: 9428 6818 4b00 6819 4b00 681a 4b00 681b  .(h.K.h.K.h.K.h.
+00002140: 4b00 681c 4b06 681d 4ba5 681e 4b02 758c  K.h.K.h.K.h.K.u.
+00002150: 2450 5141 6e61 6c79 7369 732e 6174 6f6d  $PQAnalysis.atom
+00002160: 6963 5f73 7973 7465 6d2e 5f64 6563 6f72  ic_system._decor
+00002170: 6174 6f72 7394 7d94 2868 184b 0068 194b  ators.}.(h.K.h.K
+00002180: 0068 1a4b 0068 1b4b 0068 1c4b 0068 1d4b  .h.K.h.K.h.K.h.K
+00002190: 1868 1e4b 0075 8c2d 5051 416e 616c 7973  .h.K.u.-PQAnalys
+000021a0: 6973 2e61 746f 6d69 635f 7379 7374 656d  is.atomic_system
+000021b0: 2e5f 7374 616e 6461 7264 5f70 726f 7065  ._standard_prope
+000021c0: 7274 6965 7394 7d94 2868 184b 0068 194b  rties.}.(h.K.h.K
+000021d0: 0068 1a4b 0068 1b4b 0068 1c4b 0268 1d4b  .h.K.h.K.h.K.h.K
+000021e0: 4468 1e4b 0075 8c23 5051 416e 616c 7973  Dh.K.u.#PQAnalys
+000021f0: 6973 2e61 746f 6d69 635f 7379 7374 656d  is.atomic_system
+00002200: 2e5f 706f 7369 7469 6f6e 7394 7d94 2868  ._positions.}.(h
+00002210: 184b 0068 194b 0068 1a4b 0068 1b4b 0068  .K.h.K.h.K.h.K.h
+00002220: 1c4b 0068 1d4b 1968 1e4b 0075 8c23 5051  .K.h.K.h.K.u.#PQ
+00002230: 416e 616c 7973 6973 2e61 746f 6d69 635f  Analysis.atomic_
+00002240: 7379 7374 656d 2e65 7863 6570 7469 6f6e  system.exception
+00002250: 7394 7d94 2868 184b 0068 194b 0068 1a4b  s.}.(h.K.h.K.h.K
+00002260: 0068 1b4b 0068 1c4b 0068 1d4b 1268 1e4b  .h.K.h.K.h.K.h.K
+00002270: 0075 8c24 5051 416e 616c 7973 6973 2e61  .u.$PQAnalysis.a
+00002280: 746f 6d69 635f 7379 7374 656d 2e5f 7072  tomic_system._pr
+00002290: 6f70 6572 7469 6573 947d 9428 6818 4b00  operties.}.(h.K.
+000022a0: 6819 4b00 681a 4b00 681b 4b00 681c 4b03  h.K.h.K.h.K.h.K.
+000022b0: 681d 4b28 681e 4b00 7575 8c06 6279 5f6d  h.K(h.K.uu..by_m
+000022c0: 7367 947d 9428 8c05 6669 786d 6594 4b0a  sg.}.(..fixme.K.
+000022d0: 8c1f 706f 7373 6962 6c79 2d75 7365 642d  ..possibly-used-
+000022e0: 6265 666f 7265 2d61 7373 6967 6e6d 656e  before-assignmen
+000022f0: 7494 4b1e 8c1e 696e 636f 6e73 6973 7465  t.K...inconsiste
+00002300: 6e74 2d72 6574 7572 6e2d 7374 6174 656d  nt-return-statem
+00002310: 656e 7473 944b 098c 1274 6f6f 2d6d 616e  ents.K...too-man
+00002320: 792d 6172 6775 6d65 6e74 7394 4b12 8c0f  y-arguments.K...
+00002330: 746f 6f2d 6d61 6e79 2d6c 6f63 616c 7394  too-many-locals.
+00002340: 4b03 8c1c 746f 6f2d 6d61 6e79 2d69 6e73  K...too-many-ins
+00002350: 7461 6e63 652d 6174 7472 6962 7574 6573  tance-attributes
+00002360: 944b 0a8c 096e 6f2d 6d65 6d62 6572 944b  .K...no-member.K
+00002370: 018c 0b74 6f6f 2d63 6f6d 706c 6578 944b  ...too-complex.K
+00002380: 038c 1174 6f6f 2d6d 616e 792d 6272 616e  ...too-many-bran
+00002390: 6368 6573 944b 028c 0e74 6f6f 2d6d 616e  ches.K...too-man
+000023a0: 792d 6c69 6e65 7394 4b01 8c13 746f 6f2d  y-lines.K...too-
+000023b0: 6d61 6e79 2d73 7461 7465 6d65 6e74 7394  many-statements.
+000023c0: 4b01 8c0f 756e 7573 6564 2d61 7267 756d  K...unused-argum
+000023d0: 656e 7494 4b01 8c1a 746f 6f2d 6d61 6e79  ent.K...too-many
+000023e0: 2d72 6574 7572 6e2d 7374 6174 656d 656e  -return-statemen
+000023f0: 7473 944b 018c 1774 6f6f 2d6d 616e 792d  ts.K...too-many-
+00002400: 7075 626c 6963 2d6d 6574 686f 6473 944b  public-methods.K
+00002410: 018c 0e64 7570 6c69 6361 7465 2d63 6f64  ...duplicate-cod
+00002420: 6594 4b03 758c 0f63 6f64 655f 7479 7065  e.K.u..code_type
+00002430: 5f63 6f75 6e74 947d 9428 8c04 636f 6465  _count.}.(..code
+00002440: 944d 7e1e 8c07 636f 6d6d 656e 7494 4d0d  .M~...comment.M.
+00002450: 018c 0964 6f63 7374 7269 6e67 944d 9421  ...docstring.M.!
+00002460: 8c05 656d 7074 7994 4d37 0b8c 0574 6f74  ..empty.M7...tot
+00002470: 616c 944d 564c 758c 0c64 6570 656e 6465  al.MVLu..depende
+00002480: 6e63 6965 7394 7d94 288c 0d62 6561 7274  ncies.}.(..beart
+00002490: 7970 652e 636c 6177 948f 9428 6823 908c  ype.claw...(h#..
+000024a0: 1150 5141 6e61 6c79 7369 732e 636f 6e66  .PQAnalysis.conf
+000024b0: 6967 948f 9428 688f 68e5 68ed 6851 68eb  ig...(h.h.h.hQh.
+000024c0: 68ef 68f9 68f5 68f1 68e7 68d9 68f3 6895  h.h.h.h.h.h.h.h.
+000024d0: 6823 68e3 68f7 908c 1f50 5141 6e61 6c79  h#h.h....PQAnaly
+000024e0: 7369 732e 7574 696c 732e 6375 7374 6f6d  sis.utils.custom
+000024f0: 5f6c 6f67 6769 6e67 948f 9428 682f 683d  _logging...(h/h=
+00002500: 6859 6829 8c24 5051 416e 616c 7973 6973  hYh).$PQAnalysis
+00002510: 2e69 6f2e 7472 616a 5f66 696c 652e 6672  .io.traj_file.fr
+00002520: 616d 655f 7265 6164 6572 9468 9d68 3568  ame_reader.h.h5h
+00002530: c168 dd68 6968 6d8c 1250 5141 6e61 6c79  .h.hihm..PQAnaly
+00002540: 7369 732e 696f 2e62 6173 6594 68ab 687b  sis.io.base.h.h{
+00002550: 68bb 68b3 8c29 5051 416e 616c 7973 6973  h.h..)PQAnalysis
+00002560: 2e69 6f2e 7265 7374 6172 745f 6669 6c65  .io.restart_file
+00002570: 2e72 6573 7461 7274 5f72 6561 6465 7294  .restart_reader.
+00002580: 6875 6895 6873 6877 686f 6a0d 0100 0068  huh.hshwhoj....h
+00002590: c568 5768 5d8c 2650 5141 6e61 6c79 7369  .hWh].&PQAnalysi
+000025a0: 732e 696f 2e67 656e 5f66 696c 652e 6765  s.io.gen_file.ge
+000025b0: 6e5f 6669 6c65 5f72 6561 6465 7294 6a0b  n_file_reader.j.
+000025c0: 0100 0068 7f68 8f8c 2650 5141 6e61 6c79  ...h.h..&PQAnaly
+000025d0: 7369 732e 6174 6f6d 6963 5f73 7973 7465  sis.atomic_syste
+000025e0: 6d2e 6174 6f6d 6963 5f73 7973 7465 6d94  m.atomic_system.
+000025f0: 68fd 6841 68d9 68a5 68cb 6823 908c 0f62  h.hAh.h.h.h#...b
+00002600: 6561 7274 7970 652e 7479 7069 6e67 948f  eartype.typing..
+00002610: 9428 688b 682f 8c24 5051 416e 616c 7973  .(h.h/.$PQAnalys
+00002620: 6973 2e61 746f 6d69 635f 7379 7374 656d  is.atomic_system
+00002630: 2e5f 7072 6f70 6572 7469 6573 9468 8768  ._properties.h.h
+00002640: 3d68 4b8c 1a50 5141 6e61 6c79 7369 732e  =hK..PQAnalysis.
+00002650: 636f 7265 2e65 7863 6570 7469 6f6e 7394  core.exceptions.
+00002660: 6859 685b 684f 6829 6a3d 0100 0068 d78c  hYh[hOh)j=...h..
+00002670: 2450 5141 6e61 6c79 7369 732e 6174 6f6d  $PQAnalysis.atom
+00002680: 6963 5f73 7973 7465 6d2e 5f64 6563 6f72  ic_system._decor
+00002690: 6174 6f72 7394 689d 68bd 6835 68c1 6869  ators.h.h.h5h.hi
+000026a0: 8c23 5051 416e 616c 7973 6973 2e61 746f  .#PQAnalysis.ato
+000026b0: 6d69 635f 7379 7374 656d 2e5f 706f 7369  mic_system._posi
+000026c0: 7469 6f6e 7394 686d 6879 6a3e 0100 0068  tions.hmhyj>...h
+000026d0: ab68 bb68 256a 3f01 0000 68b3 68f1 6895  .h.h%j?...h.h.h.
+000026e0: 6873 68af 6851 686f 6a0d 0100 0068 5768  hsh.hQhoj....hWh
+000026f0: 5d68 2b6a 4001 0000 6a0b 0100 0068 7f68  ]h+j@...j....h.h
+00002700: 8f6a 0701 0000 6a41 0100 0068 6168 fd68  .j....jA...hah.h
+00002710: 4168 d968 a568 8d90 8c09 6465 636f 7261  Ah.h.h....decora
+00002720: 746f 7294 8f94 286a 4601 0000 684f 6829  tor...(jF...hOh)
+00002730: 908c 0d62 6561 7274 7970 652e 646f 6f72  ...beartype.door
+00002740: 948f 9428 6829 908c 1550 5141 6e61 6c79  ...(h)...PQAnaly
+00002750: 7369 732e 6578 6365 7074 696f 6e73 948f  sis.exceptions..
+00002760: 9428 683d 6a45 0100 0068 5968 2968 378c  .(h=jE...hYh)h7.
+00002770: 2f50 5141 6e61 6c79 7369 732e 696f 2e69  /PQAnalysis.io.i
+00002780: 6e70 7574 5f66 696c 655f 7265 6164 6572  nput_file_reader
+00002790: 2e70 712e 6f75 7470 7574 5f66 696c 6573  .pq.output_files
+000027a0: 9468 3568 6968 816a 3e01 0000 68bb 68b3  .h5hih.j>...h.h.
+000027b0: 6875 6899 68b5 6877 6851 8c22 5051 416e  huh.h.hwhQ."PQAn
+000027c0: 616c 7973 6973 2e61 6e61 6c79 7369 732e  alysis.analysis.
+000027d0: 7264 662e 6578 6365 7074 696f 6e73 9468  rdf.exceptions.h
+000027e0: ad68 cf68 c568 5768 a36a 0b01 0000 8c23  .h.h.hWh.j.....#
+000027f0: 5051 416e 616c 7973 6973 2e61 746f 6d69  PQAnalysis.atomi
+00002800: 635f 7379 7374 656d 2e65 7863 6570 7469  c_system.excepti
+00002810: 6f6e 7394 687f 688f 6a41 0100 0068 9368  ons.h.h.jA...h.h
+00002820: 5f68 cb68 4390 8c10 5051 416e 616c 7973  _h.hC...PQAnalys
+00002830: 6973 2e74 7970 6573 948f 9428 688b 6849  is.types...(h.hI
+00002840: 6a44 0100 0068 6768 3d68 5968 5b68 2968  jD...hgh=hYh[h)h
+00002850: 656a 3d01 0000 68d7 689d 6835 6869 6a47  ej=...h.h.h5hijG
+00002860: 0100 0068 6b6a 0501 0000 68bb 68b3 68ff  ...hkj....h.h.h.
+00002870: 6895 6883 6877 68c5 6857 685d 6a40 0100  h.h.hwh.hWh]j@..
+00002880: 0068 bf6a 0701 0000 6a41 0100 008c 2d50  .h.j....jA....-P
+00002890: 5141 6e61 6c79 7369 732e 6174 6f6d 6963  QAnalysis.atomic
+000028a0: 5f73 7973 7465 6d2e 5f73 7461 6e64 6172  _system._standar
+000028b0: 645f 7072 6f70 6572 7469 6573 9468 6168  d_properties.hah
+000028c0: fd68 4168 d990 8c05 6e75 6d70 7994 8f94  .hAh....numpy...
+000028d0: 2868 496a 4401 0000 683d 684b 6859 6a3d  (hIjD...h=hKhYj=
+000028e0: 0100 006a 4601 0000 689d 6835 6a47 0100  ...jF...h.h5jG..
+000028f0: 006a 0501 0000 6a3f 0100 0068 ff68 7568  .j....j?...h.huh
+00002900: 9568 8368 6f68 5768 5d6a 4001 0000 682b  .h.hohWh]j@...h+
+00002910: 6a07 0100 006a 4101 0000 68fd 6841 68d9  j....jA...h.hAh.
+00002920: 68cb 908c 0d62 6561 7274 7970 652e 7661  h....beartype.va
+00002930: 6c65 948f 9428 682b 6a07 0100 006a 0d01  le...(h+j....j..
+00002940: 0000 908c 0b6d 756c 7469 6d65 7468 6f64  .....multimethod
+00002950: 948f 9428 682d 908c 1250 5141 6e61 6c79  ...(h-...PQAnaly
+00002960: 7369 732e 666f 726d 6174 7394 8f94 2868  sis.formats...(h
+00002970: af68 2f68 6d90 8c0a 5051 416e 616c 7973  .h/hm...PQAnalys
+00002980: 6973 948f 9428 682f 683d 6859 6a3d 0100  is...(h/h=hYj=..
+00002990: 0068 9d68 3568 c168 dd68 6968 6d6a 3e01  .h.h5h.h.hihmj>.
+000029a0: 0000 68ab 687b 68bb 68b3 6a3f 0100 0068  ..h.h{h.h.j?...h
+000029b0: 7568 9568 7368 7768 6f6a 0d01 0000 68c5  uh.hshwhoj....h.
+000029c0: 6857 685d 6a40 0100 006a 0b01 0000 687f  hWh]j@...j....h.
+000029d0: 688f 6a41 0100 0068 fd68 4168 d968 a568  h.jA...h.hAh.h.h
+000029e0: cb90 8c1a 5051 416e 616c 7973 6973 2e74  ....PQAnalysis.t
+000029f0: 7261 6a2e 6578 6365 7074 696f 6e73 948f  raj.exceptions..
+00002a00: 9428 682f 8c0f 5051 416e 616c 7973 6973  .(h/..PQAnalysis
+00002a10: 2e74 7261 6a94 908c 1750 5141 6e61 6c79  .traj....PQAnaly
+00002a20: 7369 732e 7472 616a 2e66 6f72 6d61 7473  sis.traj.formats
+00002a30: 948f 9428 6a60 0100 0090 8c1a 5051 416e  ...(j`......PQAn
+00002a40: 616c 7973 6973 2e74 7261 6a2e 7472 616a  alysis.traj.traj
+00002a50: 6563 746f 7279 948f 9428 6a60 0100 0090  ectory...(j`....
+00002a60: 8c13 5051 416e 616c 7973 6973 2e74 7261  ..PQAnalysis.tra
+00002a70: 6a2e 6170 6994 8f94 286a 6001 0000 908c  j.api...(j`.....
+00002a80: 0f50 5141 6e61 6c79 7369 732e 636f 7265  .PQAnalysis.core
+00002a90: 948f 9428 6a40 0100 0068 8b68 8f6a 4101  ...(j@...h.h.jA.
+00002aa0: 0000 6a53 0100 006a 4701 0000 6a44 0100  ..jS...jG...jD..
+00002ab0: 0068 7968 6f6a 6501 0000 6a3f 0100 0068  .hyhoje...j?...h
+00002ac0: 5768 d96a 3d01 0000 685d 8c1e 5051 416e  Wh.j=...h]..PQAn
+00002ad0: 616c 7973 6973 2e69 6f2e 7265 7374 6172  alysis.io.restar
+00002ae0: 745f 6669 6c65 2e61 7069 9468 9d68 3590  t_file.api.h.h5.
+00002af0: 8c18 5051 416e 616c 7973 6973 2e74 7970  ..PQAnalysis.typ
+00002b00: 655f 6368 6563 6b69 6e67 948f 9428 688b  e_checking...(h.
+00002b10: 6887 6867 683d 6859 685b 6865 68d7 689d  h.hgh=hYh[heh.h.
+00002b20: 6835 68dd 6869 6a47 0100 0068 7968 6b68  h5h.hijG...hyhkh
+00002b30: ab6a 0501 0000 687b 6a3f 0100 0068 ff68  .j....h{j?...h.h
+00002b40: 756a 6901 0000 6895 6873 6883 68db 6877  uji...h.hsh.h.hw
+00002b50: 686f 6a0d 0100 0068 5768 5d6a 4001 0000  hoj....hWh]j@...
+00002b60: 6a0b 0100 0068 7f68 8f6a 0701 0000 6a41  j....h.h.j....jA
+00002b70: 0100 006a 5301 0000 68fd 6841 68a9 6a65  ...jS...h.hAh.je
+00002b80: 0100 0068 3b68 d968 a568 cb68 8d8c 1a50  ...h;h.h.h.h...P
+00002b90: 5141 6e61 6c79 7369 732e 696f 2e67 656e  QAnalysis.io.gen
+00002ba0: 5f66 696c 652e 6170 6994 908c 1350 5141  _file.api....PQA
+00002bb0: 6e61 6c79 7369 732e 746f 706f 6c6f 6779  nalysis.topology
+00002bc0: 948f 9428 688f 6a41 0100 0068 db6a 5301  ...(h.jA...h.jS.
+00002bd0: 0000 6a47 0100 0068 ab68 a96a 3f01 0000  ..jG...h.h.j?...
+00002be0: 68a5 68d9 6a3d 0100 0068 8d68 3590 8c18  h.h.j=...h.h5...
+00002bf0: 5051 416e 616c 7973 6973 2e61 746f 6d69  PQAnalysis.atomi
+00002c00: 635f 7379 7374 656d 948f 9428 6a40 0100  c_system...(j@..
+00002c10: 0068 8b68 8f68 cb68 3d68 9d6a 3f01 0000  .h.h.h.h=h.j?...
+00002c20: 6a3d 0100 006a 6901 0000 688d 6895 6a6c  j=...ji...h.h.jl
+00002c30: 0100 0068 3568 7f90 8c21 5051 416e 616c  ...h5h...!PQAnal
+00002c40: 7973 6973 2e74 6f6f 6c73 2e74 7261 6a5f  ysis.tools.traj_
+00002c50: 746f 5f63 6f6d 5f74 7261 6a94 8f94 288c  to_com_traj...(.
+00002c60: 1050 5141 6e61 6c79 7369 732e 746f 6f6c  .PQAnalysis.tool
+00002c70: 7394 908c 0f50 5141 6e61 6c79 7369 732e  s....PQAnalysis.
+00002c80: 7472 616a 948f 9428 688b 683d 685b 6859  traj...(h.h=h[hY
+00002c90: 6a3d 0100 0068 9d68 7968 7b68 f16a 3f01  j=...h.hyh{h.j?.
+00002ca0: 0000 6875 6a69 0100 0068 9568 7368 db68  ..huji...h.hsh.h
+00002cb0: 7f68 8f68 3b68 d968 8d90 8c15 5051 416e  .h.h;h.h....PQAn
+00002cc0: 616c 7973 6973 2e69 6f2e 666f 726d 6174  alysis.io.format
+00002cd0: 7394 8f94 2868 8b68 ed68 7968 cb6a 3e01  s...(h.h.hyh.j>.
+00002ce0: 0000 683d 68a9 68ab 687b 68f1 8c0d 5051  ..h=h.h.h{h...PQ
+00002cf0: 416e 616c 7973 6973 2e69 6f94 688d 689d  Analysis.io.h.h.
+00002d00: 6a6c 0100 0068 7f90 8c0d 5051 416e 616c  jl...h....PQAnal
+00002d10: 7973 6973 2e69 6f94 8f94 2868 dd68 e568  ysis.io...(h.h.h
+00002d20: db68 eb68 3d68 f968 5b68 5968 f368 d968  .h.h=h.h[hYh.h.h
+00002d30: f568 d768 9568 8368 f790 8c23 5051 416e  .h.h.h.h...#PQAn
+00002d40: 616c 7973 6973 2e70 6879 7369 6361 6c5f  alysis.physical_
+00002d50: 6461 7461 2e65 7863 6570 7469 6f6e 7394  data.exceptions.
+00002d60: 8f94 2868 418c 1850 5141 6e61 6c79 7369  ..(hA..PQAnalysi
+00002d70: 732e 7068 7973 6963 616c 5f64 6174 6194  s.physical_data.
+00002d80: 908c 1f50 5141 6e61 6c79 7369 732e 7068  ...PQAnalysis.ph
+00002d90: 7973 6963 616c 5f64 6174 612e 656e 6572  ysical_data.ener
+00002da0: 6779 948f 9428 6a7d 0100 0090 8c17 5051  gy...(j}......PQ
+00002db0: 416e 616c 7973 6973 2e75 7469 6c73 2e63  Analysis.utils.c
+00002dc0: 6f6d 6d6f 6e94 8f94 288c 1050 5141 6e61  ommon...(..PQAna
+00002dd0: 6c79 7369 732e 7574 696c 7394 68f1 908c  lysis.utils.h...
+00002de0: 1b50 5141 6e61 6c79 7369 732e 7574 696c  .PQAnalysis.util
+00002df0: 732e 6465 636f 7261 746f 7273 948f 9428  s.decorators...(
+00002e00: 6a82 0100 0090 8c10 5051 416e 616c 7973  j.......PQAnalys
+00002e10: 6973 2e75 7469 6c73 948f 9428 6851 687b  is.utils...(hQh{
+00002e20: 68d9 68d7 8c0e 5051 416e 616c 7973 6973  h.h...PQAnalysis
+00002e30: 2e63 6c69 9490 8c13 5051 416e 616c 7973  .cli....PQAnalys
+00002e40: 6973 2e5f 7665 7273 696f 6e94 8f94 2868  is._version...(h
+00002e50: f168 5390 8c1e 5051 416e 616c 7973 6973  .hS...PQAnalysis
+00002e60: 2e74 6f70 6f6c 6f67 792e 6578 6365 7074  .topology.except
+00002e70: 696f 6e73 948f 9428 8c13 5051 416e 616c  ions...(..PQAnal
+00002e80: 7973 6973 2e74 6f70 6f6c 6f67 7994 685d  ysis.topology.h]
+00002e90: 908c 2850 5141 6e61 6c79 7369 732e 746f  ..(PQAnalysis.to
+00002ea0: 706f 6c6f 6779 2e62 6f6e 6465 645f 746f  pology.bonded_to
+00002eb0: 706f 6c6f 6779 2e62 6f6e 6494 8f94 286a  pology.bond...(j
+00002ec0: 8c01 0000 6869 6861 908c 2950 5141 6e61  ....hiha..)PQAna
+00002ed0: 6c79 7369 732e 746f 706f 6c6f 6779 2e62  lysis.topology.b
+00002ee0: 6f6e 6465 645f 746f 706f 6c6f 6779 2e61  onded_topology.a
+00002ef0: 6e67 6c65 948f 9428 6a8c 0100 0068 6968  ngle...(j....hih
+00002f00: 6190 8c2c 5051 416e 616c 7973 6973 2e74  a..,PQAnalysis.t
+00002f10: 6f70 6f6c 6f67 792e 626f 6e64 6564 5f74  opology.bonded_t
+00002f20: 6f70 6f6c 6f67 792e 6469 6865 6472 616c  opology.dihedral
+00002f30: 948f 9428 6a8c 0100 0068 6968 6190 8c33  ...(j....hiha..3
+00002f40: 5051 416e 616c 7973 6973 2e74 6f70 6f6c  PQAnalysis.topol
+00002f50: 6f67 792e 626f 6e64 6564 5f74 6f70 6f6c  ogy.bonded_topol
+00002f60: 6f67 792e 626f 6e64 6564 5f74 6f70 6f6c  ogy.bonded_topol
+00002f70: 6f67 7994 8f94 286a 8c01 0000 685d 908c  ogy...(j....h]..
+00002f80: 1d50 5141 6e61 6c79 7369 732e 746f 706f  .PQAnalysis.topo
+00002f90: 6c6f 6779 2e73 656c 6563 7469 6f6e 948f  logy.selection..
+00002fa0: 9428 6a8c 0100 0068 5b68 5990 8c1c 5051  .(j....h[hY...PQ
+00002fb0: 416e 616c 7973 6973 2e74 6f70 6f6c 6f67  Analysis.topolog
+00002fc0: 792e 746f 706f 6c6f 6779 948f 9428 6a8c  y.topology...(j.
+00002fd0: 0100 0068 5790 8c04 6c61 726b 948f 9428  ...hW...lark...(
+00002fe0: 68b3 6857 908c 2250 5141 6e61 6c79 7369  h.hW.."PQAnalysi
+00002ff0: 732e 746f 706f 6c6f 6779 2e73 6861 6b65  s.topology.shake
+00003000: 5f74 6f70 6f6c 6f67 7994 8f94 2868 5b90  _topology...(h[.
+00003010: 8c1a 5051 416e 616c 7973 6973 2e63 6f72  ..PQAnalysis.cor
+00003020: 652e 6578 6365 7074 696f 6e73 948f 9428  e.exceptions...(
+00003030: 68fd 6a0d 0100 0068 5d6a 0b01 0000 8c0f  h.j....h]j......
+00003040: 5051 416e 616c 7973 6973 2e63 6f72 6594  PQAnalysis.core.
+00003050: 908c 3850 5141 6e61 6c79 7369 732e 746f  ..8PQAnalysis.to
+00003060: 706f 6c6f 6779 2e62 6f6e 6465 645f 746f  pology.bonded_to
+00003070: 706f 6c6f 6779 2e5f 746f 706f 6c6f 6779  pology._topology
+00003080: 5f70 726f 7065 7274 6965 7394 8f94 2868  _properties...(h
+00003090: 6990 8c18 5051 416e 616c 7973 6973 2e69  i...PQAnalysis.i
+000030a0: 6f2e 6578 6365 7074 696f 6e73 948f 9428  o.exceptions...(
+000030b0: 6a3e 0100 0068 6f68 6d68 7b90 8c12 5051  j>...hohmh{...PQ
+000030c0: 416e 616c 7973 6973 2e69 6f2e 6261 7365  Analysis.io.base
+000030d0: 948f 9428 6a40 0100 0068 8b68 8f68 cb68  ...(j@...h.h.h.h
+000030e0: 6f68 ab68 7b68 b36a 3f01 0000 68a5 6875  oh.h{h.j?...h.hu
+000030f0: 6a78 0100 0068 9d68 7390 8c22 5051 416e  jx...h.hs.."PQAn
+00003100: 616c 7973 6973 2e69 6f2e 6d6f 6c64 6573  alysis.io.moldes
+00003110: 6372 6970 746f 725f 7265 6164 6572 948f  criptor_reader..
+00003120: 9428 6a3f 0100 006a 7801 0000 908c 2950  .(j?...jx.....)P
+00003130: 5141 6e61 6c79 7369 732e 696f 2e72 6573  QAnalysis.io.res
+00003140: 7461 7274 5f66 696c 652e 7265 7374 6172  tart_file.restar
+00003150: 745f 7772 6974 6572 948f 9428 8c1a 5051  t_writer...(..PQ
+00003160: 416e 616c 7973 6973 2e69 6f2e 7265 7374  Analysis.io.rest
+00003170: 6172 745f 6669 6c65 946a 7801 0000 908c  art_file.jx.....
+00003180: 2950 5141 6e61 6c79 7369 732e 696f 2e72  )PQAnalysis.io.r
+00003190: 6573 7461 7274 5f66 696c 652e 7265 7374  estart_file.rest
+000031a0: 6172 745f 7265 6164 6572 948f 9428 6a69  art_reader...(ji
+000031b0: 0100 006a aa01 0000 6a78 0100 0090 8c1e  ...j....jx......
+000031c0: 5051 416e 616c 7973 6973 2e69 6f2e 7265  PQAnalysis.io.re
+000031d0: 7374 6172 745f 6669 6c65 2e61 7069 948f  start_file.api..
+000031e0: 9428 6879 6a78 0100 0090 8c29 5051 416e  .(hyjx.....)PQAn
+000031f0: 616c 7973 6973 2e69 6f2e 7472 616a 5f66  alysis.io.traj_f
+00003200: 696c 652e 7472 616a 6563 746f 7279 5f72  ile.trajectory_r
+00003210: 6561 6465 7294 8f94 288c 1750 5141 6e61  eader...(..PQAna
+00003220: 6c79 7369 732e 696f 2e74 7261 6a5f 6669  lysis.io.traj_fi
+00003230: 6c65 946a 7801 0000 908c 2950 5141 6e61  le.jx.....)PQAna
+00003240: 6c79 7369 732e 696f 2e74 7261 6a5f 6669  lysis.io.traj_fi
+00003250: 6c65 2e74 7261 6a65 6374 6f72 795f 7772  le.trajectory_wr
+00003260: 6974 6572 948f 9428 6ab1 0100 006a 7801  iter...(j....jx.
+00003270: 0000 908c 2450 5141 6e61 6c79 7369 732e  ....$PQAnalysis.
+00003280: 696f 2e74 7261 6a5f 6669 6c65 2e66 7261  io.traj_file.fra
+00003290: 6d65 5f72 6561 6465 7294 8f94 2868 8f6a  me_reader...(h.j
+000032a0: b101 0000 6a78 0100 0090 8c1b 5051 416e  ....jx......PQAn
+000032b0: 616c 7973 6973 2e69 6f2e 7472 616a 5f66  alysis.io.traj_f
+000032c0: 696c 652e 6170 6994 8f94 2868 7968 7f6a  ile.api...(hyh.j
+000032d0: 7801 0000 908c 2650 5141 6e61 6c79 7369  x.....&PQAnalysi
+000032e0: 732e 696f 2e67 656e 5f66 696c 652e 6765  s.io.gen_file.ge
+000032f0: 6e5f 6669 6c65 5f72 6561 6465 7294 8f94  n_file_reader...
+00003300: 288c 1650 5141 6e61 6c79 7369 732e 696f  (..PQAnalysis.io
+00003310: 2e67 656e 5f66 696c 6594 6a6c 0100 006a  .gen_file.jl...j
+00003320: 7801 0000 908c 2650 5141 6e61 6c79 7369  x.....&PQAnalysi
+00003330: 732e 696f 2e67 656e 5f66 696c 652e 6765  s.io.gen_file.ge
+00003340: 6e5f 6669 6c65 5f77 7269 7465 7294 8f94  n_file_writer...
+00003350: 286a ba01 0000 6a6c 0100 006a 7801 0000  (j....jl...jx...
+00003360: 908c 1a50 5141 6e61 6c79 7369 732e 696f  ...PQAnalysis.io
+00003370: 2e67 656e 5f66 696c 652e 6170 6994 8f94  .gen_file.api...
+00003380: 286a ba01 0000 6a78 0100 0090 8c1b 5051  (j....jx......PQ
+00003390: 416e 616c 7973 6973 2e69 6f2e 746f 706f  Analysis.io.topo
+000033a0: 6c6f 6779 5f66 696c 6594 8f94 286a 7801  logy_file...(jx.
+000033b0: 0000 908c 1f50 5141 6e61 6c79 7369 732e  .....PQAnalysis.
+000033c0: 696f 2e74 6f70 6f6c 6f67 795f 6669 6c65  io.topology_file
+000033d0: 2e61 7069 948f 9428 6a78 0100 0090 8c1e  .api...(jx......
+000033e0: 5051 416e 616c 7973 6973 2e69 6f2e 696e  PQAnalysis.io.in
+000033f0: 666f 5f66 696c 655f 7265 6164 6572 948f  fo_file_reader..
+00003400: 9428 6875 6a78 0100 0090 8c20 5051 416e  .(hujx..... PQAn
+00003410: 616c 7973 6973 2e69 6f2e 656e 6572 6779  alysis.io.energy
+00003420: 5f66 696c 655f 7265 6164 6572 948f 9428  _file_reader...(
+00003430: 6a78 0100 0090 8c18 5051 416e 616c 7973  jx......PQAnalys
+00003440: 6973 2e69 6f2e 626f 785f 7772 6974 6572  is.io.box_writer
+00003450: 948f 9428 6879 687f 6a78 0100 0090 8c1f  ...(hyh.jx......
+00003460: 5051 416e 616c 7973 6973 2e69 6f2e 696e  PQAnalysis.io.in
+00003470: 7075 745f 6669 6c65 5f72 6561 6465 7294  put_file_reader.
+00003480: 8f94 2868 776a 7801 0000 908c 1150 5141  ..(hwjx......PQA
+00003490: 6e61 6c79 7369 732e 696f 2e61 7069 948f  nalysis.io.api..
+000034a0: 9428 6a78 0100 0090 8c1c 5051 416e 616c  .(jx......PQAnal
+000034b0: 7973 6973 2e69 6f2e 636f 6e76 6572 7369  ysis.io.conversi
+000034c0: 6f6e 5f61 7069 948f 9428 6a78 0100 0090  on_api...(jx....
+000034d0: 8c17 5051 416e 616c 7973 6973 2e69 6f2e  ..PQAnalysis.io.
+000034e0: 7772 6974 655f 6170 6994 8f94 286a 7801  write_api...(jx.
+000034f0: 0000 908c 1850 5141 6e61 6c79 7369 732e  .....PQAnalysis.
+00003500: 7068 7973 6963 616c 5f64 6174 6194 8f94  physical_data...
+00003510: 2868 7590 8c27 5051 416e 616c 7973 6973  (hu..'PQAnalysis
+00003520: 2e69 6f2e 696e 7075 745f 6669 6c65 5f72  .io.input_file_r
+00003530: 6561 6465 722e 666f 726d 6174 7394 8f94  eader.formats...
+00003540: 2868 c168 778c 1f50 5141 6e61 6c79 7369  (h.hw..PQAnalysi
+00003550: 732e 696f 2e69 6e70 7574 5f66 696c 655f  s.io.input_file_
+00003560: 7265 6164 6572 9468 c568 b390 8c17 5051  reader.h.h....PQ
+00003570: 416e 616c 7973 6973 2e69 6f2e 7472 616a  Analysis.io.traj
+00003580: 5f66 696c 6594 8f94 2868 8d68 7990 8c16  _file...(h.hy...
+00003590: 5051 416e 616c 7973 6973 2e69 6f2e 6765  PQAnalysis.io.ge
+000035a0: 6e5f 6669 6c65 948f 9428 6879 908c 2250  n_file...(hy.."P
+000035b0: 5141 6e61 6c79 7369 732e 696f 2e76 6972  QAnalysis.io.vir
+000035c0: 6961 6c2e 7669 7269 616c 5f72 6561 6465  ial.virial_reade
+000035d0: 7294 8f94 288c 1450 5141 6e61 6c79 7369  r...(..PQAnalysi
+000035e0: 732e 696f 2e76 6972 6961 6c94 6887 908c  s.io.virial.h...
+000035f0: 0974 7164 6d2e 6175 746f 948f 9428 688f  .tqdm.auto...(h.
+00003600: 68d9 908c 2250 5141 6e61 6c79 7369 732e  h..."PQAnalysis.
+00003610: 696f 2e74 7261 6a5f 6669 6c65 2e65 7863  io.traj_file.exc
+00003620: 6570 7469 6f6e 7394 8f94 2868 8f6a 3d01  eptions...(h.j=.
+00003630: 0000 908c 1850 5141 6e61 6c79 7369 732e  .....PQAnalysis.
+00003640: 696f 2e76 6972 6961 6c2e 6170 6994 8f94  io.virial.api...
+00003650: 2868 9590 8c16 5051 416e 616c 7973 6973  (h....PQAnalysis
+00003660: 2e75 7469 6c73 2e75 6e69 7473 948f 9428  .utils.units...(
+00003670: 6895 908c 1650 5141 6e61 6c79 7369 732e  h....PQAnalysis.
+00003680: 7574 696c 732e 6669 6c65 7394 8f94 2868  utils.files...(h
+00003690: 9590 8c17 5051 416e 616c 7973 6973 2e75  ....PQAnalysis.u
+000036a0: 7469 6c73 2e72 616e 646f 6d94 8f94 2868  tils.random...(h
+000036b0: 956a 4101 0000 908c 1c50 5141 6e61 6c79  .jA......PQAnaly
+000036c0: 7369 732e 696f 2e6e 6570 2e65 7863 6570  sis.io.nep.excep
+000036d0: 7469 6f6e 7394 8f94 2868 9590 8c25 5051  tions...(h...%PQ
+000036e0: 416e 616c 7973 6973 2e69 6f2e 7265 7374  Analysis.io.rest
+000036f0: 6172 745f 6669 6c65 2e65 7863 6570 7469  art_file.excepti
+00003700: 6f6e 7394 8f94 2868 9d6a 3f01 0000 908c  ons...(h.j?.....
+00003710: 2650 5141 6e61 6c79 7369 732e 696f 2e74  &PQAnalysis.io.t
+00003720: 6f70 6f6c 6f67 795f 6669 6c65 2e65 7863  opology_file.exc
+00003730: 6570 7469 6f6e 7394 8f94 2868 a568 ab90  eptions...(h.h..
+00003740: 8c30 5051 416e 616c 7973 6973 2e69 6f2e  .0PQAnalysis.io.
+00003750: 746f 706f 6c6f 6779 5f66 696c 652e 746f  topology_file.to
+00003760: 706f 6c6f 6779 5f66 696c 655f 7265 6164  pology_file_read
+00003770: 6572 948f 9428 68a9 8c1b 5051 416e 616c  er...(h...PQAnal
+00003780: 7973 6973 2e69 6f2e 746f 706f 6c6f 6779  ysis.io.topology
+00003790: 5f66 696c 6594 908c 3050 5141 6e61 6c79  _file...0PQAnaly
+000037a0: 7369 732e 696f 2e74 6f70 6f6c 6f67 795f  sis.io.topology_
+000037b0: 6669 6c65 2e74 6f70 6f6c 6f67 795f 6669  file.topology_fi
+000037c0: 6c65 5f77 7269 7465 7294 8f94 2868 a96a  le_writer...(h.j
+000037d0: f101 0000 908c 2a50 5141 6e61 6c79 7369  ......*PQAnalysi
+000037e0: 732e 696f 2e69 6e70 7574 5f66 696c 655f  s.io.input_file_
+000037f0: 7265 6164 6572 2e65 7863 6570 7469 6f6e  reader.exception
+00003800: 7394 8f94 2868 bb68 c168 af68 dd90 8c31  s...(h.h.h.h...1
+00003810: 5051 416e 616c 7973 6973 2e69 6f2e 696e  PQAnalysis.io.in
+00003820: 7075 745f 6669 6c65 5f72 6561 6465 722e  put_file_reader.
+00003830: 696e 7075 745f 6669 6c65 5f70 6172 7365  input_file_parse
+00003840: 7294 8f94 2868 bb68 c16a d501 0000 68c5  r...(h.h.j....h.
+00003850: 908c 2250 5141 6e61 6c79 7369 732e 696f  .."PQAnalysis.io
+00003860: 2e69 6e70 7574 5f66 696c 655f 7265 6164  .input_file_read
+00003870: 6572 2e70 7194 8f94 286a d501 0000 908c  er.pq...(j......
+00003880: 2b50 5141 6e61 6c79 7369 732e 696f 2e69  +PQAnalysis.io.i
+00003890: 6e70 7574 5f66 696c 655f 7265 6164 6572  nput_file_reader
+000038a0: 2e70 715f 616e 616c 7973 6973 948f 9428  .pq_analysis...(
+000038b0: 6ad5 0100 0090 8c32 5051 416e 616c 7973  j......2PQAnalys
+000038c0: 6973 2e69 6f2e 696e 7075 745f 6669 6c65  is.io.input_file
+000038d0: 5f72 6561 6465 722e 7071 5f61 6e61 6c79  _reader.pq_analy
+000038e0: 7369 732e 5f70 6172 7365 948f 9428 68bd  sis._parse...(h.
+000038f0: 68b7 68bf 908c 4850 5141 6e61 6c79 7369  h.h...HPQAnalysi
+00003900: 732e 696f 2e69 6e70 7574 5f66 696c 655f  s.io.input_file_
+00003910: 7265 6164 6572 2e70 715f 616e 616c 7973  reader.pq_analys
+00003920: 6973 2e70 7161 6e61 6c79 7369 735f 696e  is.pqanalysis_in
+00003930: 7075 745f 6669 6c65 5f72 6561 6465 7294  put_file_reader.
+00003940: 8f94 288c 2b50 5141 6e61 6c79 7369 732e  ..(.+PQAnalysis.
+00003950: 696f 2e69 6e70 7574 5f66 696c 655f 7265  io.input_file_re
+00003960: 6164 6572 2e70 715f 616e 616c 7973 6973  ader.pq_analysis
+00003970: 9490 8c37 5051 416e 616c 7973 6973 2e69  ...7PQAnalysis.i
+00003980: 6f2e 696e 7075 745f 6669 6c65 5f72 6561  o.input_file_rea
+00003990: 6465 722e 7071 5f61 6e61 6c79 7369 732e  der.pq_analysis.
+000039a0: 5f66 696c 655f 6d69 7869 6e94 8f94 2868  _file_mixin...(h
+000039b0: c190 8c3c 5051 416e 616c 7973 6973 2e69  ...<PQAnalysis.i
+000039c0: 6f2e 696e 7075 745f 6669 6c65 5f72 6561  o.input_file_rea
+000039d0: 6465 722e 7071 5f61 6e61 6c79 7369 732e  der.pq_analysis.
+000039e0: 5f73 656c 6563 7469 6f6e 5f6d 6978 696e  _selection_mixin
+000039f0: 948f 9428 68c1 908c 3c50 5141 6e61 6c79  ...(h...<PQAnaly
+00003a00: 7369 732e 696f 2e69 6e70 7574 5f66 696c  sis.io.input_fil
+00003a10: 655f 7265 6164 6572 2e70 715f 616e 616c  e_reader.pq_anal
+00003a20: 7973 6973 2e5f 706f 7369 7469 6f6e 735f  ysis._positions_
+00003a30: 6d69 7869 6e94 8f94 2868 c190 8c37 5051  mixin...(h...7PQ
+00003a40: 416e 616c 7973 6973 2e69 6f2e 696e 7075  Analysis.io.inpu
+00003a50: 745f 6669 6c65 5f72 6561 6465 722e 7071  t_file_reader.pq
+00003a60: 2e70 715f 696e 7075 745f 6669 6c65 5f72  .pq_input_file_r
+00003a70: 6561 6465 7294 8f94 288c 2250 5141 6e61  eader...(."PQAna
+00003a80: 6c79 7369 732e 696f 2e69 6e70 7574 5f66  lysis.io.input_f
+00003a90: 696c 655f 7265 6164 6572 2e70 7194 908c  ile_reader.pq...
+00003aa0: 2f50 5141 6e61 6c79 7369 732e 696f 2e69  /PQAnalysis.io.i
+00003ab0: 6e70 7574 5f66 696c 655f 7265 6164 6572  nput_file_reader
+00003ac0: 2e70 712e 6f75 7470 7574 5f66 696c 6573  .pq.output_files
+00003ad0: 948f 9428 68c5 908c 2150 5141 6e61 6c79  ...(h...!PQAnaly
+00003ae0: 7369 732e 696f 2e67 656e 5f66 696c 652e  sis.io.gen_file.
+00003af0: 6578 6365 7074 696f 6e73 948f 9428 6a40  exceptions...(j@
+00003b00: 0100 0090 8c17 5051 416e 616c 7973 6973  ......PQAnalysis
+00003b10: 2e61 6e61 6c79 7369 732e 7264 6694 8f94  .analysis.rdf...
+00003b20: 288c 1350 5141 6e61 6c79 7369 732e 616e  (..PQAnalysis.an
+00003b30: 616c 7973 6973 9490 8c1b 5051 416e 616c  alysis....PQAnal
+00003b40: 7973 6973 2e61 6e61 6c79 7369 732e 7264  ysis.analysis.rd
+00003b50: 662e 7264 6694 8f94 2868 db6a 1002 0000  f.rdf...(h.j....
+00003b60: 68e7 68d7 8c17 5051 416e 616c 7973 6973  h.h...PQAnalysis
+00003b70: 2e61 6e61 6c79 7369 732e 7264 6694 908c  .analysis.rdf...
+00003b80: 1b50 5141 6e61 6c79 7369 732e 616e 616c  .PQAnalysis.anal
+00003b90: 7973 6973 2e72 6466 2e61 7069 948f 9428  ysis.rdf.api...(
+00003ba0: 6a13 0200 0090 8c2d 5051 416e 616c 7973  j......-PQAnalys
+00003bb0: 6973 2e61 6e61 6c79 7369 732e 7264 662e  is.analysis.rdf.
+00003bc0: 7264 665f 696e 7075 745f 6669 6c65 5f72  rdf_input_file_r
+00003bd0: 6561 6465 7294 8f94 286a 1302 0000 68db  eader...(j....h.
+00003be0: 68e7 908c 2e50 5141 6e61 6c79 7369 732e  h....PQAnalysis.
+00003bf0: 616e 616c 7973 6973 2e72 6466 2e72 6466  analysis.rdf.rdf
+00003c00: 5f6f 7574 7075 745f 6669 6c65 5f77 7269  _output_file_wri
+00003c10: 7465 7294 8f94 286a 1302 0000 68db 906a  ter...(j....h..j
+00003c20: 4f01 0000 8f94 286a 1302 0000 68d9 908c  O.....(j....h...
+00003c30: 1650 5141 6e61 6c79 7369 732e 636c 692e  .PQAnalysis.cli.
+00003c40: 7879 7a32 6765 6e94 8f94 2868 e390 8c19  xyz2gen...(h....
+00003c50: 5051 416e 616c 7973 6973 2e63 6c69 2e74  PQAnalysis.cli.t
+00003c60: 7261 6a32 716d 6366 6394 8f94 2868 e390  raj2qmcfc...(h..
+00003c70: 8c17 5051 416e 616c 7973 6973 2e63 6c69  ..PQAnalysis.cli
+00003c80: 2e74 7261 6a32 626f 7894 8f94 2868 e390  .traj2box...(h..
+00003c90: 8c16 5051 416e 616c 7973 6973 2e63 6c69  ..PQAnalysis.cli
+00003ca0: 2e72 7374 3278 797a 948f 9428 68e3 908c  .rst2xyz...(h...
+00003cb0: 1250 5141 6e61 6c79 7369 732e 636c 692e  .PQAnalysis.cli.
+00003cc0: 7264 6694 8f94 2868 e390 8c16 5051 416e  rdf...(h....PQAn
+00003cd0: 616c 7973 6973 2e63 6c69 2e67 656e 3278  alysis.cli.gen2x
+00003ce0: 797a 948f 9428 68e3 908c 1d50 5141 6e61  yz...(h....PQAna
+00003cf0: 6c79 7369 732e 636c 692e 636f 6e74 696e  lysis.cli.contin
+00003d00: 7565 5f69 6e70 7574 948f 9428 68e3 908c  ue_input...(h...
+00003d10: 1c50 5141 6e61 6c79 7369 732e 636c 692e  .PQAnalysis.cli.
+00003d20: 6164 645f 6d6f 6c65 6375 6c65 7394 8f94  add_molecules...
+00003d30: 2868 e390 8c1d 5051 416e 616c 7973 6973  (h....PQAnalysis
+00003d40: 2e63 6c69 2e62 7569 6c64 5f6e 6570 5f74  .cli.build_nep_t
+00003d50: 7261 6a94 8f94 2868 e390 8c1f 5051 416e  raj...(h....PQAn
+00003d60: 616c 7973 6973 2e63 6c69 2e5f 6172 6775  alysis.cli._argu
+00003d70: 6d65 6e74 5f70 6172 7365 7294 8f94 2868  ment_parser...(h
+00003d80: e568 ed68 eb68 ef68 f968 f568 e768 f368  .h.h.h.h.h.h.h.h
+00003d90: e368 f790 8c18 5051 416e 616c 7973 6973  .h....PQAnalysis
+00003da0: 2e63 6c69 2e5f 636c 695f 6261 7365 948f  .cli._cli_base..
+00003db0: 9428 68e5 68ed 68eb 68ef 68f9 68f5 68e7  .(h.h.h.h.h.h.h.
+00003dc0: 68f3 68f7 908c 1d50 5141 6e61 6c79 7369  h.h....PQAnalysi
+00003dd0: 732e 746f 6f6c 732e 6164 645f 6d6f 6c65  s.tools.add_mole
+00003de0: 6375 6c65 948f 9428 68ed 908c 1c50 5141  cule...(h....PQA
+00003df0: 6e61 6c79 7369 732e 696f 2e6e 6570 2e6e  nalysis.io.nep.n
+00003e00: 6570 5f77 7269 7465 7294 8f94 2868 ef90  ep_writer...(h..
+00003e10: 8c0b 6172 6763 6f6d 706c 6574 6594 8f94  ..argcomplete...
+00003e20: 2868 f190 8c0d 7269 6368 5f61 7267 7061  (h....rich_argpa
+00003e30: 7273 6594 8f94 2868 f190 8c14 5051 416e  rse...(h....PQAn
+00003e40: 616c 7973 6973 2e63 6f72 652e 6365 6c6c  alysis.core.cell
+00003e50: 948f 9428 68ff 6a9f 0100 0090 8c14 5051  ...(h.j.......PQ
+00003e60: 416e 616c 7973 6973 2e63 6f72 652e 6174  Analysis.core.at
+00003e70: 6f6d 948f 9428 6a9f 0100 0068 fd90 8c17  om...(j....h....
+00003e80: 5051 416e 616c 7973 6973 2e63 6f72 652e  PQAnalysis.core.
+00003e90: 7265 7369 6475 6594 8f94 286a 9f01 0000  residue...(j....
+00003ea0: 908c 1350 5141 6e61 6c79 7369 732e 636f  ...PQAnalysis.co
+00003eb0: 7265 2e61 7069 948f 9428 6a9f 0100 0090  re.api...(j.....
+00003ec0: 8c19 5051 416e 616c 7973 6973 2e63 6f72  ..PQAnalysis.cor
+00003ed0: 652e 6365 6c6c 2e63 656c 6c94 8f94 288c  e.cell.cell...(.
+00003ee0: 1450 5141 6e61 6c79 7369 732e 636f 7265  .PQAnalysis.core
+00003ef0: 2e63 656c 6c94 908c 1550 5141 6e61 6c79  .cell....PQAnaly
+00003f00: 7369 732e 7574 696c 732e 6d61 7468 948f  sis.utils.math..
+00003f10: 9428 6a07 0100 006a 4101 0000 908c 2950  .(j....jA.....)P
+00003f20: 5141 6e61 6c79 7369 732e 636f 7265 2e63  QAnalysis.core.c
+00003f30: 656c 6c2e 5f73 7461 6e64 6172 645f 7072  ell._standard_pr
+00003f40: 6f70 6572 7469 6573 948f 9428 6a07 0100  operties...(j...
+00003f50: 0090 8c1c 5051 416e 616c 7973 6973 2e63  ....PQAnalysis.c
+00003f60: 6f72 652e 6174 6f6d 2e65 6c65 6d65 6e74  ore.atom.element
+00003f70: 948f 9428 6a0b 0100 008c 1450 5141 6e61  ...(j......PQAna
+00003f80: 6c79 7369 732e 636f 7265 2e61 746f 6d94  lysis.core.atom.
+00003f90: 908c 1950 5141 6e61 6c79 7369 732e 636f  ...PQAnalysis.co
+00003fa0: 7265 2e61 746f 6d2e 6174 6f6d 948f 9428  re.atom.atom...(
+00003fb0: 6a4a 0200 0090 8c26 5051 416e 616c 7973  jJ.....&PQAnalys
+00003fc0: 6973 2e61 746f 6d69 635f 7379 7374 656d  is.atomic_system
+00003fd0: 2e61 746f 6d69 635f 7379 7374 656d 948f  .atomic_system..
+00003fe0: 9428 8c18 5051 416e 616c 7973 6973 2e61  .(..PQAnalysis.a
+00003ff0: 746f 6d69 635f 7379 7374 656d 9490 6a50  tomic_system..jP
+00004000: 0100 008f 9428 6a46 0100 006a 4101 0000  .....(jF...jA...
+00004010: 6a44 0100 006a 4f02 0000 908c 1773 6369  jD...jO......sci
+00004020: 7079 2e73 7061 7469 616c 2e74 7261 6e73  py.spatial.trans
+00004030: 666f 726d 948f 9428 6a41 0100 0090 8c24  form...(jA.....$
+00004040: 5051 416e 616c 7973 6973 2e61 746f 6d69  PQAnalysis.atomi
+00004050: 635f 7379 7374 656d 2e5f 7072 6f70 6572  c_system._proper
+00004060: 7469 6573 948f 9428 6a41 0100 0090 8c2d  ties...(jA.....-
+00004070: 5051 416e 616c 7973 6973 2e61 746f 6d69  PQAnalysis.atomi
+00004080: 635f 7379 7374 656d 2e5f 7374 616e 6461  c_system._standa
+00004090: 7264 5f70 726f 7065 7274 6965 7394 8f94  rd_properties...
+000040a0: 286a 4101 0000 908c 2350 5141 6e61 6c79  (jA.....#PQAnaly
+000040b0: 7369 732e 6174 6f6d 6963 5f73 7973 7465  sis.atomic_syste
+000040c0: 6d2e 5f70 6f73 6974 696f 6e73 948f 9428  m._positions...(
+000040d0: 6a41 0100 0090 8c24 5051 416e 616c 7973  jA.....$PQAnalys
+000040e0: 6973 2e61 746f 6d69 635f 7379 7374 656d  is.atomic_system
+000040f0: 2e5f 6465 636f 7261 746f 7273 948f 9428  ._decorators...(
+00004100: 6a53 0100 006a 4401 0000 6a47 0100 0090  jS...jD...jG....
+00004110: 758c 1064 7570 6c69 6361 7465 645f 6c69  u..duplicated_li
+00004120: 6e65 7394 7d94 288c 136e 625f 6475 706c  nes.}.(..nb_dupl
+00004130: 6963 6174 6564 5f6c 696e 6573 944b 008c  icated_lines.K..
+00004140: 1870 6572 6365 6e74 5f64 7570 6c69 6361  .percent_duplica
+00004150: 7465 645f 6c69 6e65 7394 4700 0000 0000  ted_lines.G.....
+00004160: 0000 0075 8c0a 6e6f 6465 5f63 6f75 6e74  ...u..node_count
+00004170: 947d 9428 680e 4b4c 6809 4b75 680f 4d12  .}.(h.KLh.Kuh.M.
+00004180: 0268 104b 7d75 8c0c 756e 646f 6375 6d65  .h.K}u..undocume
+00004190: 6e74 6564 947d 9428 680e 4b00 6809 4b00  nted.}.(h.K.h.K.
+000041a0: 680f 4b00 6810 4b00 7568 184b 0168 194b  h.K.h.K.uh.K.h.K
+000041b0: 1f68 1a4b 0068 1b4b 0068 1c4b 3368 1d4d  .h.K.h.K.h.K3h.M
+000041c0: df11 681e 4b0b 8c0b 676c 6f62 616c 5f6e  ..h.K...global_n
+000041d0: 6f74 6594 4740 230c 07d5 7925 366a 5d02  ote.G@#...y%6j].
+000041e0: 0000 4b1b 6a5e 0200 0047 3fc1 f1e2 2523  ..K.j^...G?...%#
+000041f0: a31d 7562 2e                             ..ub.
```

### Comparing `pqanalysis-1.0.7/.github/ISSUE_TEMPLATE/feature_request.md` & `pqanalysis-1.0.8.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/.github/scripts/parse_pylint.py` & `pqanalysis-1.0.8.1/.github/scripts/parse_pylint.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/.github/workflows/ci.yml` & `pqanalysis-1.0.8.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/.github/workflows/docs.yml` & `pqanalysis-1.0.8.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/.github/workflows/pylint.yml` & `pqanalysis-1.0.8.1/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/.github/workflows/release.yml` & `pqanalysis-1.0.8.1/.github/workflows/release.yml`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     - name: Create GitHub Release
       env:
         GITHUB_TOKEN: ${{ github.token }}
       run: >-
         gh release create
         '${{ github.ref_name }}'
         --repo '${{ github.repository }}'
-        --notes '${{ steps.changelog.outputs.changes }}''
+        --notes '${{ steps.changelog.outputs.changes }}'
 
   pypi-release-update:
     name: >-
       Sign the Python distribution with Sigstore
       and upload them to GitHub Release
     needs:
     - publish-to-pypi
```

### Comparing `pqanalysis-1.0.7/.pylintrc` & `pqanalysis-1.0.8.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/CODE_OF_CONDUCT.md` & `pqanalysis-1.0.8.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/LICENSE` & `pqanalysis-1.0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PKG-INFO` & `pqanalysis-1.0.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PQAnalysis
-Version: 1.0.7
+Version: 1.0.8.1
 Summary: PQAnalysis is a python package for the analysis of PQ simulations.
 Author-email: Jakob Gamper <97gamjak@gmail.com>, "Josef M. Gallmetzer" <gallmetzer.josef@gmail.com>, "Clarissa A. Seidler" <clarissa.seidler@gmail.com>
 Project-URL: Homepage, https://github.com/MolarVerse/PQAnalysis
 Project-URL: PQ, https://github.com/MolarVerse/PQ
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -33,14 +33,16 @@
 Requires-Dist: sphinx-sitemap; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Requires-Dist: better-apidoc; extra == "docs"
 Requires-Dist: six; extra == "docs"
 Requires-Dist: docstr-coverage; extra == "docs"
 
+<img src="docs/source/logo/PQAnalysis.png" width="250">
+
 # PQAnalysis
 
 [![CI](https://github.com/MolarVerse/PQAnalysis/actions/workflows/ci.yml/badge.svg)](https://github.com/MolarVerse/PQAnalysis/actions/workflows/ci.yml)
 [![Docs](https://github.com/MolarVerse/PQAnalysis/actions/workflows/docs.yml/badge.svg)](https://MolarVerse.github.io/PQAnalysis/)
 [![codecov](https://codecov.io/gh/MolarVerse/PQAnalysis/graph/badge.svg?token=IDFK8L6IIQ)](https://codecov.io/gh/MolarVerse/PQAnalysis)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

### Comparing `pqanalysis-1.0.7/PQAnalysis/__init__.py` & `pqanalysis-1.0.8.1/PQAnalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/analysis/rdf/__init__.py` & `pqanalysis-1.0.8.1/PQAnalysis/analysis/rdf/__init__.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/analysis/rdf/api.py` & `pqanalysis-1.0.8.1/PQAnalysis/analysis/rdf/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/analysis/rdf/exceptions.py` & `pqanalysis-1.0.8.1/PQAnalysis/analysis/rdf/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/analysis/rdf/rdf.py` & `pqanalysis-1.0.8.1/PQAnalysis/analysis/rdf/rdf.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/analysis/rdf/rdf_input_file_reader.py` & `pqanalysis-1.0.8.1/PQAnalysis/analysis/rdf/rdf_input_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/analysis/rdf/rdf_output_file_writer.py` & `pqanalysis-1.0.8.1/PQAnalysis/analysis/rdf/rdf_output_file_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/atomic_system/_decorators.py` & `pqanalysis-1.0.8.1/PQAnalysis/atomic_system/_decorators.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,17 +20,15 @@
 import sys
 import numpy as np
 
 from beartype.typing import Any
 from decorator import decorator
 
 from .exceptions import (
-    AtomicSystemPositionsError,
-    AtomicSystemMassError,
-    AtomicSystemError
+    AtomicSystemPositionsError, AtomicSystemMassError, AtomicSystemError
 )
 
 
 
 @decorator
 def check_atom_number_setters(func, self, arg_to_set: Any) -> None:
     """
@@ -50,25 +48,20 @@
         The result of the function.
 
     Raises
     ------
     AtomicSystemError
         If the number of atoms is not equal the number of positions.
     """
-    print("test")
-    print(func.__name__, file=sys.stderr)
-    print(self.logger)
-    print(arg_to_set)
     if self.n_atoms != np.shape(arg_to_set)[0]:
-        print("test")
         self.logger.error(
             (
-            "The number of atoms in the AtomicSystem object have "
-            "to be equal to the number of atoms in the new array "
-            "in order to set the property."
+                "The number of atoms in the AtomicSystem object have "
+                "to be equal to the number of atoms in the new array "
+                "in order to set the property."
             ),
             exception=AtomicSystemError
         )
 
     return func(self, arg_to_set)
 
 
@@ -125,12 +118,11 @@
         If any atom does not have mass information.
     """
 
     self = args[0]
 
     if not all(atom.mass is not None for atom in self.atoms):
         self.logger.error(
-            AtomicSystemMassError.message,
-            exception=AtomicSystemMassError
+            AtomicSystemMassError.message, exception=AtomicSystemMassError
         )
 
     return func(*args, **kwargs)
```

### Comparing `pqanalysis-1.0.7/PQAnalysis/atomic_system/_positions.py` & `pqanalysis-1.0.8.1/PQAnalysis/atomic_system/_positions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/atomic_system/_properties.py` & `pqanalysis-1.0.8.1/PQAnalysis/atomic_system/_properties.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/atomic_system/_standard_properties.py` & `pqanalysis-1.0.8.1/PQAnalysis/atomic_system/_standard_properties.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/atomic_system/atomic_system.py` & `pqanalysis-1.0.8.1/PQAnalysis/atomic_system/atomic_system.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,18 @@
         self._forces = np.zeros((0, 3)) if forces is None else forces
         self._charges = np.zeros(0) if charges is None else charges
         self._energy = energy
         self._virial = virial
         self._stress = stress
         self._cell = cell
 
-    @runtime_type_checking
+    #TODO: check why dynamic formatting does
+    #      not work here for "AtomicSystem"
+    #
+    # @runtime_type_checking
     def fit_atomic_system(
         self,
         system: "AtomicSystem",
         number_of_additions: PositiveInt = 1,
         max_iterations: PositiveInt = 100,
         distance_cutoff: PositiveReal = 1.0,
         max_displacement: PositiveReal | Np1DNumberArray = 0.1,
```

### Comparing `pqanalysis-1.0.7/PQAnalysis/atomic_system/exceptions.py` & `pqanalysis-1.0.8.1/PQAnalysis/atomic_system/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/cli/_argument_parser.py` & `pqanalysis-1.0.8.1/PQAnalysis/cli/_argument_parser.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/cli/_cli_base.py` & `pqanalysis-1.0.8.1/PQAnalysis/cli/_cli_base.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/cli/add_molecules.py` & `pqanalysis-1.0.8.1/PQAnalysis/cli/add_molecules.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/cli/build_nep_traj.py` & `pqanalysis-1.0.8.1/PQAnalysis/cli/build_nep_traj.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/cli/continue_input.py` & `pqanalysis-1.0.8.1/PQAnalysis/cli/continue_input.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/cli/gen2xyz.py` & `pqanalysis-1.0.8.1/PQAnalysis/cli/gen2xyz.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/cli/main.py` & `pqanalysis-1.0.8.1/PQAnalysis/cli/main.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/cli/rdf.py` & `pqanalysis-1.0.8.1/PQAnalysis/cli/rdf.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/cli/rst2xyz.py` & `pqanalysis-1.0.8.1/PQAnalysis/cli/rst2xyz.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/cli/traj2box.py` & `pqanalysis-1.0.8.1/PQAnalysis/cli/traj2box.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/cli/traj2qmcfc.py` & `pqanalysis-1.0.8.1/PQAnalysis/cli/traj2qmcfc.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/cli/xyz2gen.py` & `pqanalysis-1.0.8.1/PQAnalysis/cli/xyz2gen.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/core/__init__.py` & `pqanalysis-1.0.8.1/PQAnalysis/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/core/api.py` & `pqanalysis-1.0.8.1/PQAnalysis/core/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/core/atom/atom.py` & `pqanalysis-1.0.8.1/PQAnalysis/core/atom/atom.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/core/atom/element.py` & `pqanalysis-1.0.8.1/PQAnalysis/core/atom/element.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/core/cell/_standard_properties.py` & `pqanalysis-1.0.8.1/PQAnalysis/core/cell/_standard_properties.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/core/cell/cell.py` & `pqanalysis-1.0.8.1/PQAnalysis/core/cell/cell.py`

 * *Files 4% similar despite different names*

```diff
@@ -273,17 +273,14 @@
         alpha = np.arccos(
             (
                 box_matrix[0][1] * box_matrix[0][2] +
                 box_matrix[1][1] * box_matrix[1][2]
             ) / (y * z)
         )
 
-        print(alpha, beta, gamma)
-        print(np.rad2deg(alpha), np.rad2deg(beta), np.rad2deg(gamma))
-
         return cls(
             x, y, z, np.rad2deg(alpha), np.rad2deg(beta), np.rad2deg(gamma)
         )
 
 
 
 #: A type hint for a list of cells
```

### Comparing `pqanalysis-1.0.7/PQAnalysis/core/exceptions.py` & `pqanalysis-1.0.8.1/PQAnalysis/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/core/residue.py` & `pqanalysis-1.0.8.1/PQAnalysis/core/residue.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/exceptions.py` & `pqanalysis-1.0.8.1/PQAnalysis/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/formats.py` & `pqanalysis-1.0.8.1/PQAnalysis/formats.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/grammar/inputGrammar.lark` & `pqanalysis-1.0.8.1/PQAnalysis/grammar/inputGrammar.lark`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/grammar/rules.lark` & `pqanalysis-1.0.8.1/PQAnalysis/grammar/rules.lark`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/grammar/selection.lark` & `pqanalysis-1.0.8.1/PQAnalysis/grammar/selection.lark`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/__init__.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/api.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/base.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/base.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/box_writer.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/box_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/conversion_api.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/conversion_api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/energy_file_reader.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/energy_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/exceptions.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/formats.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/formats.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 from beartype.typing import Any, List
 
 from PQAnalysis.formats import BaseEnumFormat
 from PQAnalysis.utils.custom_logging import setup_logger
 from PQAnalysis import __package_name__
 
 from .exceptions import (
-    BoxFileFormatError,
-    FileWritingModeError,
-    OutputFileFormatError
+    BoxFileFormatError, FileWritingModeError, OutputFileFormatError
 )
 
 logger = logging.getLogger(__package_name__).getChild("OutputFileFormat")
 logger = setup_logger(logger)
 
 
 
@@ -83,16 +81,16 @@
             filename = None
 
         output_file_format = super()._missing_(value, OutputFileFormatError)
 
         if output_file_format == cls.AUTO and filename is None:
             logger.error(
                 (
-                "The file format could not be inferred from "
-                "the file extension because no filename was given."
+                    "The file format could not be inferred from "
+                    "the file extension because no filename was given."
                 ),
                 exception=OutputFileFormatError
             )
 
         if output_file_format == cls.AUTO:
             return cls.infer_format_from_extension(filename)
 
@@ -115,17 +113,15 @@
         file_extensions[cls.CHARGE.value] = [".charge", ".chrg", ".charges"]
         file_extensions[cls.RESTART.value] = [".rst", ".restart"]
         file_extensions[cls.ENERGY.value] = [".en", ".energy", ".energies"]
         file_extensions[cls.STRESS.value] = [".stress", ".stresses"]
         file_extensions[cls.VIRIAL.value] = [".virial", ".virials", ".vir"]
         file_extensions[cls.INFO.value] = [".info", ".information"]
         file_extensions[cls.INSTANTANEOUS_ENERGY.value] = [
-            ".instant_en",
-            ".instant_energies",
-            ".inst_energy"
+            ".instant_en", ".instant_energies", ".inst_energy"
         ]
 
         return file_extensions
 
     @classmethod
     def infer_format_from_extension(cls, file_path: str) -> "OutputFileFormat":
         """
@@ -138,44 +134,43 @@
 
         Returns
         -------
         OutputFileFormat
             The inferred file format.
         """
 
-        file_extension = file_path.split(".")[-1]
+        file_extension = "." + file_path.split(".")[-1]
 
-        if file_extension in cls.file_extensions()[cls.XYZ]:
+        if file_extension in cls.file_extensions()[cls.XYZ.value]:
             return cls.XYZ
 
-        if file_extension in cls.file_extensions()[cls.VEL]:
+        if file_extension in cls.file_extensions()[cls.VEL.value]:
             return cls.VEL
 
-        if file_extension in cls.file_extensions()[cls.FORCE]:
+        if file_extension in cls.file_extensions()[cls.FORCE.value]:
             return cls.FORCE
 
-        if file_extension in cls.file_extensions()[cls.CHARGE]:
+        if file_extension in cls.file_extensions()[cls.CHARGE.value]:
             return cls.CHARGE
 
-        if file_extension in cls.file_extensions()[cls.RESTART]:
+        if file_extension in cls.file_extensions()[cls.RESTART.value]:
             return cls.RESTART
 
         logger.error(
             (
-            "Could not infer the file format from the file extension of "
-            f"\"{file_path}\". Possible file formats are: "
-            f"{cls.__members__.values()}"
+                "Could not infer the file format from the file extension of "
+                f"\"{file_path}\". Possible file formats are: "
+                f"{cls.__members__.values()}"
             ),
             exception=OutputFileFormatError
         )
 
     @classmethod
     def get_file_extensions(
-        cls,
-        file_format: "OutputFileFormat | str"
+        cls, file_format: "OutputFileFormat | str"
     ) -> List[str]:
         """
         Get the file extensions of the given file format.
 
         Parameters
         ----------
         file_format : OutputFileFormat
```

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/gen_file/api.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/gen_file/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/gen_file/gen_file_reader.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/gen_file/gen_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/gen_file/gen_file_writer.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/gen_file/gen_file_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/info_file_reader.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/info_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/input_file_reader/exceptions.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/input_file_reader/formats.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/formats.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/input_file_reader/input_file_parser.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/input_file_parser.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/input_file_reader/pq/output_files.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq/output_files.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/input_file_reader/pq/pq_input_file_reader.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq/pq_input_file_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -128,41 +128,36 @@
             new_raw_input_file = self.raw_input_file
 
             # replace digit strings in start files
             for key in self.output_file_keys:
                 if key in self.dictionary.keys():
 
                     new_filename = self.dictionary[key][0].replace(
-                        self.actual_n,
-                        new_actual_n
+                        self.actual_n, new_actual_n
                     )
 
                     new_raw_input_file = new_raw_input_file.replace(
-                        self.dictionary[key][0],
-                        new_filename
+                        self.dictionary[key][0], new_filename
                     )
 
             # replace digit strings in output files
             for key in self.start_file_keys:
                 if key in self.dictionary.keys():
 
                     new_filename = self.dictionary[key][0].replace(
-                        self.start_n,
-                        new_start_n
+                        self.start_n, new_start_n
                     )
 
                     new_raw_input_file = new_raw_input_file.replace(
-                        self.dictionary[key][0],
-                        new_filename
+                        self.dictionary[key][0], new_filename
                     )
 
             # create new input file and write new_raw_input_file to it
             new_filename = self.filename.replace(
-                self.input_file_n,
-                new_input_file_n
+                self.input_file_n, new_input_file_n
             )
 
             with open(new_filename, "w", encoding="utf-8") as file:
                 file.write(new_raw_input_file)
                 file.close()
 
             old_input_file_n = new_input_file_n
@@ -187,16 +182,18 @@
         PQValueError
             if the n from the start file and the rpmd_start_file do not match
         """
         n = _get_digit_string_from_filename(self.start_file)
 
         if self.is_rpmd_start_file_defined:
             # add "." to match also files without extension
-            if (_n := _get_digit_string_from_filename(self.rpmd_start_file +
-                '.')) != n:
+            if (
+                _n :=
+                _get_digit_string_from_filename(self.rpmd_start_file + '.')
+            ) != n:
                 self.logger.error(
                     f"N from start_file ({n}) and rpmd_start_file ({_n}) do not match.",
                     exception=PQValueError
                 )
 
         return n
 
@@ -222,15 +219,14 @@
             if key in self.dictionary.keys():
                 # add "." to match also files without extension
                 _n = _get_digit_string_from_filename(
                     self.dictionary[key][0] + "."
                 )
 
                 if _n != n and n is not None:
-                    print(_n, n, key)
                     self.logger.error(
                         "Actual n in output files is not consistent.",
                         exception=PQValueError
                     )
 
                 n = _n
 
@@ -320,14 +316,14 @@
     PQValueError
         if filename does not contain a number to be parsed
     """
 
     if (regex := re.search(r"\d+.", filename)) is None:
         PQInputFileReader.logger.error(
             (
-            f"Filename {filename} does not contain a number to be "
-            "continued from. It has to be of the form \"...<number>.<extension>\"."
+                f"Filename {filename} does not contain a number to be "
+                "continued from. It has to be of the form \"...<number>.<extension>\"."
             ),
             exception=PQValueError
         )
 
     return regex.group(0)[:-1]
```

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/input_file_reader/pq_analysis/_file_mixin.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq_analysis/_file_mixin.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/input_file_reader/pq_analysis/_parse.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq_analysis/_parse.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/input_file_reader/pq_analysis/_positions_mixin.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq_analysis/_positions_mixin.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/input_file_reader/pq_analysis/_selection_mixin.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq_analysis/_selection_mixin.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/input_file_reader/pq_analysis/pqanalysis_input_file_reader.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/input_file_reader/pq_analysis/pqanalysis_input_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/moldescriptor_reader.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/moldescriptor_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/nep/nep_writer.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/nep/nep_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/restart_file/api.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/restart_file/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/restart_file/restart_reader.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/restart_file/restart_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,16 +79,16 @@
             The format of the restart file, by default MDEngineFormat.PQ
         """
         super().__init__(filename)
 
         if moldescriptor_filename is not None and reference_residues is not None:
             self.logger.error(
                 (
-                "Both moldescriptor_filename and reference_residues "
-                "are given. They are mutually exclusive."
+                    "Both moldescriptor_filename and reference_residues "
+                    "are given. They are mutually exclusive."
                 ),
                 exception=RestartFileReaderError
             )
 
         self.moldescriptor_filename = moldescriptor_filename
         self.reference_residues = reference_residues
 
@@ -269,15 +269,15 @@
 
             if len(line) != 12 and len(line) != 21:
                 cls.logger.error(
                     f"Invalid number of arguments for atom: {len(line)}",
                     exception=RestartFileReaderError
                 )
 
-            atoms.append(Atom(line[0], use_guess_element=False))
+            atoms.append(Atom(line[0]))
             residues.append(int(line[2]))
             positions.append(np.array([float(l) for l in line[3:6]]))
             velocities.append(np.array([float(l) for l in line[6:9]]))
             forces.append(np.array([float(l) for l in line[9:12]]))
 
         if not atoms:
             cls.logger.error(
```

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/restart_file/restart_writer.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/restart_file/restart_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/topology_file/api.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/topology_file/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/topology_file/topology_file_reader.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/topology_file/topology_file_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/topology_file/topology_file_writer.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/topology_file/topology_file_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/traj_file/api.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/traj_file/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/traj_file/frame_reader.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/traj_file/frame_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/traj_file/trajectory_reader.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/traj_file/trajectory_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/traj_file/trajectory_writer.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/traj_file/trajectory_writer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/virial/api.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/virial/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/virial/virial_reader.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/virial/virial_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/io/write_api.py` & `pqanalysis-1.0.8.1/PQAnalysis/io/write_api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/physical_data/energy.py` & `pqanalysis-1.0.8.1/PQAnalysis/physical_data/energy.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/tools/add_molecule.py` & `pqanalysis-1.0.8.1/PQAnalysis/tools/add_molecule.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,17 +106,15 @@
     Raises
     ------
     PQValueError
         If the molecule file type is not RESTART and a moldescriptor file is specified.
     """
 
     _check_topology_args(
-        topology_file,
-        topology_file_to_add,
-        topology_file_output
+        topology_file, topology_file_to_add, topology_file_output
     )
 
     _add_molecule = AddMolecule(
         restart_file=restart_file,
         molecule_file=molecule_file,
         output_file=output_file,
         mode=mode,
@@ -175,16 +173,16 @@
         If the output topology file is None.
     """
 
     if topology_file is None and topology_file_to_add is None:
         if topology_file_output is not None:
             AddMolecule.logger.warning(
                 (
-                "The output topology file is specified, but no topology "
-                "files are given to add. The output topology file will be ignored."
+                    "The output topology file is specified, but no topology "
+                    "files are given to add. The output topology file will be ignored."
                 )
             )
 
         return
 
     if topology_file is None and topology_file_to_add is not None:
         AddMolecule.logger.error(
@@ -197,17 +195,17 @@
             "The topology file to add must be specified if a topology file is given.",
             exception=PQValueError
         )
 
     if topology_file_output is None:
         AddMolecule.logger.error(
             (
-            "The output topology file must be specified if topology files are "
-            "given to add. This is a special case where None cannot be treated "
-            "as stdout as it is already used for the restart file."
+                "The output topology file must be specified if topology files are "
+                "given to add. This is a special case where None cannot be treated "
+                "as stdout as it is already used for the restart file."
             ),
             exception=PQValueError
         )
 
 
 
 class AddMolecule:
@@ -305,27 +303,29 @@
         self.rotation_angle_step = rotation_angle_step
 
         # Initialize the variables, just to make sure they are defined
         self.molecule = None
         self.restart_system = None
 
         self.molecule_file_type = OutputFileFormat(
-            (molecule_file_type,
-            self.molecule_file)
+            (molecule_file_type, self.molecule_file)
         )
 
-        if (self.molecule_file_type != OutputFileFormat.RESTART and
-                self.molecule_moldescriptor_file is not None):
+        if (
+            self.molecule_file_type != OutputFileFormat.RESTART and
+            self.molecule_moldescriptor_file is not None
+        ):
             self.logger.error(
                 "A moldescriptor file can only be specified for restart files.",
                 exception=PQValueError
             )
 
-        if self.molecule_file_type not in [OutputFileFormat.RESTART,
-            OutputFileFormat.XYZ]:
+        if self.molecule_file_type not in [
+            OutputFileFormat.RESTART, OutputFileFormat.XYZ
+        ]:
             self.logger.error(
                 "The molecule file type must be either RESTART or XYZ.",
                 exception=PQValueError
             )
 
     @runtime_type_checking
     def write_restart_file(self) -> None:
@@ -371,28 +371,28 @@
         ------
         PQValueError
             If the restart system or the molecule is not read before extending the topology file.
         """
 
         self.logger.warning(
             (
-            "Extension of the topology file is only implemented for shake bonds. "
-            "The extension of general bonded topologies is not implemented yet."
+                "Extension of the topology file is only implemented for shake bonds. "
+                "The extension of general bonded topologies is not implemented yet."
             )
         )
 
         original_topology = read_topology_file(original_shake_file)
         new_topology = read_topology_file(extension_shake_file)
 
         if self.restart_system is None or self.molecule is None:
             self.logger.error(
                 (
-                "The restart frame and the molecule must be read "
-                "before extending the topology file. Either call "
-                "the read_files method or the add_molecules method first."
+                    "The restart frame and the molecule must be read "
+                    "before extending the topology file. Either call "
+                    "the read_files method or the add_molecules method first."
                 ),
                 exception=PQValueError
             )
 
         original_topology.extend_shake_bonds(
             new_topology.shake_bonds,
             n_atoms=self.restart_system.n_atoms,
```

### Comparing `pqanalysis-1.0.7/PQAnalysis/tools/traj_to_com_traj.py` & `pqanalysis-1.0.8.1/PQAnalysis/tools/traj_to_com_traj.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/topology/__init__.py` & `pqanalysis-1.0.8.1/PQAnalysis/topology/__init__.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/topology/api.py` & `pqanalysis-1.0.8.1/PQAnalysis/topology/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/topology/bonded_topology/_topology_properties.py` & `pqanalysis-1.0.8.1/PQAnalysis/topology/bonded_topology/_topology_properties.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/topology/bonded_topology/angle.py` & `pqanalysis-1.0.8.1/PQAnalysis/topology/bonded_topology/angle.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/topology/bonded_topology/bond.py` & `pqanalysis-1.0.8.1/PQAnalysis/topology/bonded_topology/bond.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/topology/bonded_topology/bonded_topology.py` & `pqanalysis-1.0.8.1/PQAnalysis/topology/bonded_topology/bonded_topology.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/topology/bonded_topology/dihedral.py` & `pqanalysis-1.0.8.1/PQAnalysis/topology/bonded_topology/dihedral.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/topology/selection.py` & `pqanalysis-1.0.8.1/PQAnalysis/topology/selection.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/topology/shake_topology.py` & `pqanalysis-1.0.8.1/PQAnalysis/topology/shake_topology.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/topology/topology.py` & `pqanalysis-1.0.8.1/PQAnalysis/topology/topology.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/traj/api.py` & `pqanalysis-1.0.8.1/PQAnalysis/traj/api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/traj/exceptions.py` & `pqanalysis-1.0.8.1/PQAnalysis/traj/exceptions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/traj/formats.py` & `pqanalysis-1.0.8.1/PQAnalysis/traj/formats.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/traj/trajectory.py` & `pqanalysis-1.0.8.1/PQAnalysis/traj/trajectory.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/type_checking.py` & `pqanalysis-1.0.8.1/PQAnalysis/type_checking.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/types.py` & `pqanalysis-1.0.8.1/PQAnalysis/types.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/utils/common.py` & `pqanalysis-1.0.8.1/PQAnalysis/utils/common.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/utils/custom_logging.py` & `pqanalysis-1.0.8.1/PQAnalysis/utils/custom_logging.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/utils/decorators.py` & `pqanalysis-1.0.8.1/PQAnalysis/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/utils/files.py` & `pqanalysis-1.0.8.1/PQAnalysis/utils/files.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/utils/math.py` & `pqanalysis-1.0.8.1/PQAnalysis/utils/math.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis/utils/random.py` & `pqanalysis-1.0.8.1/PQAnalysis/utils/random.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/PQAnalysis.egg-info/PKG-INFO` & `pqanalysis-1.0.8.1/PQAnalysis.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PQAnalysis
-Version: 1.0.7
+Version: 1.0.8.1
 Summary: PQAnalysis is a python package for the analysis of PQ simulations.
 Author-email: Jakob Gamper <97gamjak@gmail.com>, "Josef M. Gallmetzer" <gallmetzer.josef@gmail.com>, "Clarissa A. Seidler" <clarissa.seidler@gmail.com>
 Project-URL: Homepage, https://github.com/MolarVerse/PQAnalysis
 Project-URL: PQ, https://github.com/MolarVerse/PQ
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -33,14 +33,16 @@
 Requires-Dist: sphinx-sitemap; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Requires-Dist: better-apidoc; extra == "docs"
 Requires-Dist: six; extra == "docs"
 Requires-Dist: docstr-coverage; extra == "docs"
 
+<img src="docs/source/logo/PQAnalysis.png" width="250">
+
 # PQAnalysis
 
 [![CI](https://github.com/MolarVerse/PQAnalysis/actions/workflows/ci.yml/badge.svg)](https://github.com/MolarVerse/PQAnalysis/actions/workflows/ci.yml)
 [![Docs](https://github.com/MolarVerse/PQAnalysis/actions/workflows/docs.yml/badge.svg)](https://MolarVerse.github.io/PQAnalysis/)
 [![codecov](https://codecov.io/gh/MolarVerse/PQAnalysis/graph/badge.svg?token=IDFK8L6IIQ)](https://codecov.io/gh/MolarVerse/PQAnalysis)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

### Comparing `pqanalysis-1.0.7/PQAnalysis.egg-info/SOURCES.txt` & `pqanalysis-1.0.8.1/PQAnalysis.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -277,14 +277,17 @@
 docs/source/code/PQAnalysis.utils.rst
 docs/source/code/PQAnalysis.utils.units.rst
 docs/source/code/modules.rst
 docs/source/developerGuide/developerGuide.rst
 docs/source/logo/PQAnalysis.png
 docs/source/userGuide/inputFile.rst
 docs/source/userGuide/userGuide.rst
+examples/add_molecules/mil68ga-md-01.rst
+examples/add_molecules/perylene-md-05.rst
+examples/add_molecules/perylene-md-05.xyz
 examples/traj2box/.gitignore
 examples/traj2box/acof_triclinic.xyz
 examples/traj2box/acof_triclinic_2.xyz
 examples/traj2comtraj/umcm-9-md-01.xyz
 tests/__init__.py
 tests/conftest.py
 tests/test_formats.py
```

### Comparing `pqanalysis-1.0.7/README.md` & `pqanalysis-1.0.8.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+<img src="docs/source/logo/PQAnalysis.png" width="250">
+
 # PQAnalysis
 
 [![CI](https://github.com/MolarVerse/PQAnalysis/actions/workflows/ci.yml/badge.svg)](https://github.com/MolarVerse/PQAnalysis/actions/workflows/ci.yml)
 [![Docs](https://github.com/MolarVerse/PQAnalysis/actions/workflows/docs.yml/badge.svg)](https://MolarVerse.github.io/PQAnalysis/)
 [![codecov](https://codecov.io/gh/MolarVerse/PQAnalysis/graph/badge.svg?token=IDFK8L6IIQ)](https://codecov.io/gh/MolarVerse/PQAnalysis)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

### Comparing `pqanalysis-1.0.7/benchmarks/core/benchmark_traj_reader.py` & `pqanalysis-1.0.8.1/benchmarks/core/benchmark_traj_reader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/docs/Makefile` & `pqanalysis-1.0.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/docs/make.bat` & `pqanalysis-1.0.8.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/docs/source/_templates/module.rst` & `pqanalysis-1.0.8.1/docs/source/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/docs/source/_templates/package.rst` & `pqanalysis-1.0.8.1/docs/source/_templates/package.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/docs/source/code/PQAnalysis.atomic_system.exceptions.rst` & `pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.atomic_system.exceptions.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.exceptions.rst` & `pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.exceptions.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.input_file_reader.exceptions.rst` & `pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.input_file_reader.exceptions.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.input_file_reader.input_file_parser.rst` & `pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.input_file_reader.input_file_parser.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.pqanalysis_input_file_reader.rst` & `pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.input_file_reader.pq_analysis.pqanalysis_input_file_reader.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.input_file_reader.rst` & `pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.input_file_reader.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.rst` & `pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.topology_file.topology_file_writer.rst` & `pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.topology_file.topology_file_writer.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/docs/source/code/PQAnalysis.io.traj_file.api.rst` & `pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.io.traj_file.api.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/docs/source/code/PQAnalysis.rst` & `pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/docs/source/code/PQAnalysis.tools.add_molecule.rst` & `pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.tools.add_molecule.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/docs/source/code/PQAnalysis.topology.api.rst` & `pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.topology.api.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/docs/source/code/PQAnalysis.utils.custom_logging.rst` & `pqanalysis-1.0.8.1/docs/source/code/PQAnalysis.utils.custom_logging.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/docs/source/conf.py` & `pqanalysis-1.0.8.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/docs/source/developerGuide/developerGuide.rst` & `pqanalysis-1.0.8.1/docs/source/developerGuide/developerGuide.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/docs/source/logo/PQAnalysis.png` & `pqanalysis-1.0.8.1/docs/source/logo/PQAnalysis.png`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/docs/source/userGuide/inputFile.rst` & `pqanalysis-1.0.8.1/docs/source/userGuide/inputFile.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/docs/source/userGuide/userGuide.rst` & `pqanalysis-1.0.8.1/docs/source/userGuide/userGuide.rst`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/examples/traj2box/acof_triclinic.xyz` & `pqanalysis-1.0.8.1/examples/traj2box/acof_triclinic.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/examples/traj2box/acof_triclinic_2.xyz` & `pqanalysis-1.0.8.1/examples/traj2box/acof_triclinic_2.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/examples/traj2comtraj/umcm-9-md-01.xyz` & `pqanalysis-1.0.8.1/examples/traj2comtraj/umcm-9-md-01.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/pyproject.toml` & `pqanalysis-1.0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/analysis/rdf/test_api.py` & `pqanalysis-1.0.8.1/tests/analysis/rdf/test_api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/analysis/rdf/test_rdf.py` & `pqanalysis-1.0.8.1/tests/analysis/rdf/test_rdf.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/analysis/rdf/test_rdfInputFileReader.py` & `pqanalysis-1.0.8.1/tests/analysis/rdf/test_rdfInputFileReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/analysis/rdf/test_rdfOutputFileReader.py` & `pqanalysis-1.0.8.1/tests/analysis/rdf/test_rdfOutputFileReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/atomicSystem/test_atomic_system.py` & `pqanalysis-1.0.8.1/tests/atomicSystem/test_atomic_system.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/atomicSystem/test_decorators.py` & `pqanalysis-1.0.8.1/tests/atomicSystem/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/atomicSystem/test_positions.py` & `pqanalysis-1.0.8.1/tests/atomicSystem/test_positions.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/cli/test_continue_input.py` & `pqanalysis-1.0.8.1/tests/cli/test_continue_input.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/cli/test_rst2xyz.py` & `pqanalysis-1.0.8.1/tests/cli/test_rst2xyz.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/cli/test_traj2box.py` & `pqanalysis-1.0.8.1/tests/cli/test_traj2box.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/cli/test_traj2qmcfc.py` & `pqanalysis-1.0.8.1/tests/cli/test_traj2qmcfc.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/conftest.py` & `pqanalysis-1.0.8.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/core/atom/test_atom.py` & `pqanalysis-1.0.8.1/tests/core/atom/test_atom.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/core/atom/test_element.py` & `pqanalysis-1.0.8.1/tests/core/atom/test_element.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/core/test_cell.py` & `pqanalysis-1.0.8.1/tests/core/test_cell.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/core/test_residue.py` & `pqanalysis-1.0.8.1/tests/core/test_residue.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/data/inputFileReader/PQ_input/n_not_matching.in` & `pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/n_not_matching.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/data/inputFileReader/PQ_input/n_not_matching_input_file_n-08.in` & `pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/n_not_matching_input_file_n-08.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/data/inputFileReader/PQ_input/no_output_files.in` & `pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/no_output_files.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/data/inputFileReader/PQ_input/no_start_file.in` & `pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/no_start_file.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/data/inputFileReader/PQ_input/old_n_not_less_one_than_actual_n-09.in` & `pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/old_n_not_less_one_than_actual_n-09.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/data/inputFileReader/PQ_input/run-08.in` & `pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/run-08.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/data/inputFileReader/PQ_input/run-08.rpmd.in` & `pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/run-08.rpmd.in`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/data/inputFileReader/PQ_input/run-09.in.ref` & `pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/run-09.in.ref`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/data/inputFileReader/PQ_input/run-09.rpmd.in.ref` & `pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/run-09.rpmd.in.ref`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/data/inputFileReader/PQ_input/run-10.in.ref` & `pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/run-10.in.ref`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/data/inputFileReader/PQ_input/run-10.rpmd.in.ref` & `pqanalysis-1.0.8.1/tests/data/inputFileReader/PQ_input/run-10.rpmd.in.ref`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/data/readEnergyFile/md-01.info` & `pqanalysis-1.0.8.1/tests/data/readEnergyFile/md-01.info`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/data/readInfoFile/md-01.info` & `pqanalysis-1.0.8.1/tests/data/readInfoFile/md-01.info`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/data/readInfoFile/md-01.qmcfc.info` & `pqanalysis-1.0.8.1/tests/data/readInfoFile/md-01.qmcfc.info`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/data/traj2qmcfc/acof_triclinic.xyz` & `pqanalysis-1.0.8.1/tests/data/traj2qmcfc/acof_triclinic.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/data/traj2qmcfc/acof_triclinic_2.xyz` & `pqanalysis-1.0.8.1/tests/data/traj2qmcfc/acof_triclinic_2.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/data/traj2qmcfc/traj.qmcfc.xyz` & `pqanalysis-1.0.8.1/tests/data/traj2qmcfc/traj.qmcfc.xyz`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/io/inputFileReader/PQ/test_PQ_inputFileReader.py` & `pqanalysis-1.0.8.1/tests/io/inputFileReader/PQ/test_PQ_inputFileReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/io/inputFileReader/PQAnalysis/test_parse.py` & `pqanalysis-1.0.8.1/tests/io/inputFileReader/PQAnalysis/test_parse.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/io/inputFileReader/test_inputDictionary.py` & `pqanalysis-1.0.8.1/tests/io/inputFileReader/test_inputDictionary.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/io/inputFileReader/test_inputFileParser.py` & `pqanalysis-1.0.8.1/tests/io/inputFileReader/test_inputFileParser.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/io/inputFileReader/test_transformers.py` & `pqanalysis-1.0.8.1/tests/io/inputFileReader/test_transformers.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/io/inputFileReader/test_visitors.py` & `pqanalysis-1.0.8.1/tests/io/inputFileReader/test_visitors.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/io/test_base.py` & `pqanalysis-1.0.8.1/tests/io/test_base.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/io/test_boxWriter.py` & `pqanalysis-1.0.8.1/tests/io/test_boxWriter.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/io/test_energyFileReader.py` & `pqanalysis-1.0.8.1/tests/io/test_energyFileReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/io/test_frameReader.py` & `pqanalysis-1.0.8.1/tests/io/test_frameReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/io/test_infoFileReader.py` & `pqanalysis-1.0.8.1/tests/io/test_infoFileReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/io/test_moldescriptorReader.py` & `pqanalysis-1.0.8.1/tests/io/test_moldescriptorReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/io/test_restartReader.py` & `pqanalysis-1.0.8.1/tests/io/test_restartReader.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 from PQAnalysis.exceptions import PQFileNotFoundError
 
 
 
 class Test_RestartFileReader:
 
     @pytest.mark.parametrize(
-        "example_dir",
-        ["readRestartFile"],
-        indirect=False
+        "example_dir", ["readRestartFile"], indirect=False
     )
     def test__init__(self, test_with_data_dir):
         with pytest.raises(PQFileNotFoundError) as exception:
             RestartFileReader("tmp")
         assert str(exception.value) == "File tmp not found."
 
         filename = "md-01.rst"
@@ -39,17 +37,15 @@
         assert reader.filename == filename
         assert reader.md_engine_format == MDEngineFormat.QMCFC
         assert reader.moldescriptor_filename == "moldescriptor.dat"
         assert reader.reference_residues == None
 
         residue = Residue("H2O", 1, 0, Element("Ar"), 1, 0)
         reader = RestartFileReader(
-            filename,
-            md_engine_format="qmcfc",
-            reference_residues=[residue]
+            filename, md_engine_format="qmcfc", reference_residues=[residue]
         )
         assert reader.filename == filename
         assert reader.md_engine_format == MDEngineFormat.QMCFC
         assert reader.moldescriptor_filename == None
         assert reader.reference_residues == [residue]
 
         with pytest.raises(RestartFileReaderError) as exception:
@@ -68,20 +64,15 @@
         assert RestartFileReader._parse_box(line) == Cell()
 
         line = ["box", "1.0", "2.0", "3.0"]
         assert RestartFileReader._parse_box(line) == Cell(1.0, 2.0, 3.0)
 
         line = ["box", "1.0", "2.0", "3.0", "90.0", "90.0", "120.0"]
         assert RestartFileReader._parse_box(line) == Cell(
-            1.0,
-            2.0,
-            3.0,
-            90.0,
-            90.0,
-            120.0
+            1.0, 2.0, 3.0, 90.0, 90.0, 120.0
         )
 
         with pytest.raises(RestartFileReaderError) as exception:
             line = ["box", "1.0", "2.0"]
             RestartFileReader._parse_box(line)
         assert str(exception.value) == "Invalid number of arguments for box: 3"
 
@@ -102,138 +93,72 @@
             "C 0 1 1.0 1.0 1.0 1.1 1.2 1.3 1.4 1.5 1.6",
             "H 0 2 2.0 2.0 2.0 2.1 2.2 2.3 2.4 2.5 2.6"
         ]
         frame = RestartFileReader._parse_atoms(lines, Cell())
         system = frame
         residue_ids = frame.topology.residue_ids
         assert system.n_atoms == 2
-        assert system.atoms == [
-            Atom(name,
-            use_guess_element=False) for name in ["C",
-            "H"]
-        ]
+        assert system.atoms == [Atom(name) for name in ["C", "H"]]
         assert system.pos.shape == (2, 3)
         assert np.allclose(
-            system.pos,
-            np.array([[1.0,
-            1.0,
-            1.0],
-            [2.0,
-            2.0,
-            2.0]])
+            system.pos, np.array([[1.0, 1.0, 1.0], [2.0, 2.0, 2.0]])
         )
         assert system.vel.shape == (2, 3)
         assert np.allclose(
-            system.vel,
-            np.array([[1.1,
-            1.2,
-            1.3],
-            [2.1,
-            2.2,
-            2.3]])
+            system.vel, np.array([[1.1, 1.2, 1.3], [2.1, 2.2, 2.3]])
         )
         assert system.forces.shape == (2, 3)
         assert np.allclose(
-            system.forces,
-            np.array([[1.4,
-            1.5,
-            1.6],
-            [2.4,
-            2.5,
-            2.6]])
+            system.forces, np.array([[1.4, 1.5, 1.6], [2.4, 2.5, 2.6]])
         )
         assert np.allclose(residue_ids, np.array([1, 2]))
         assert system.cell == Cell()
 
     @pytest.mark.parametrize(
-        "example_dir",
-        ["readRestartFile"],
-        indirect=False
+        "example_dir", ["readRestartFile"], indirect=False
     )
     def test_read(self, test_with_data_dir):
         frame = RestartFileReader(
-            "md-01.rst",
-            moldescriptor_filename="moldescriptor.dat"
+            "md-01.rst", moldescriptor_filename="moldescriptor.dat"
         ).read()
         system = frame
         residue_ids = frame.topology.residue_ids
 
         assert np.allclose(residue_ids, np.array([1, 1, 2, 2]))
         assert system.n_atoms == 4
-        assert system.atoms == [
-            Atom(name,
-            use_guess_element=False) for name in ["C",
-            "H",
-            "N",
-            "N"]
-        ]
+        assert system.atoms == [Atom(name) for name in ["C", "H", "N", "N"]]
 
         assert system.pos.shape == (4, 3)
         assert np.allclose(
             system.pos,
             np.array(
-            [
-            [1.0,
-            1.1,
-            1.2],
-            [2.0,
-            2.1,
-            2.2],
-            [3.0,
-            3.1,
-            3.2],
-            [4.0,
-            4.1,
-            4.2]
-            ]
+                [
+                    [1.0, 1.1, 1.2], [2.0, 2.1, 2.2], [3.0, 3.1, 3.2],
+                    [4.0, 4.1, 4.2]
+                ]
             )
         )
         assert system.vel.shape == (4, 3)
         assert np.allclose(
             system.vel,
             np.array(
-            [
-            [1.3,
-            1.4,
-            1.5],
-            [2.3,
-            2.4,
-            2.5],
-            [3.3,
-            3.4,
-            3.5],
-            [4.3,
-            4.4,
-            4.5]
-            ]
+                [
+                    [1.3, 1.4, 1.5], [2.3, 2.4, 2.5], [3.3, 3.4, 3.5],
+                    [4.3, 4.4, 4.5]
+                ]
             )
         )
         assert system.forces.shape == (4, 3)
         assert np.allclose(
             system.forces,
             np.array(
-            [
-            [1.6,
-            1.7,
-            1.8],
-            [2.6,
-            2.7,
-            2.8],
-            [3.6,
-            3.7,
-            3.8],
-            [4.6,
-            4.7,
-            4.8]
-            ]
+                [
+                    [1.6, 1.7, 1.8], [2.6, 2.7, 2.8], [3.6, 3.7, 3.8],
+                    [4.6, 4.7, 4.8]
+                ]
             )
         )
         assert system.cell == Cell(
-            15.0623,
-            15.0964,
-            20.0232,
-            89.9232,
-            90.2261,
-            120.324
+            15.0623, 15.0964, 20.0232, 89.9232, 90.2261, 120.324
         )
         assert np.allclose(system.topology.residue_ids, np.array([1, 1, 2, 2]))
         assert len(system.topology.reference_residues) == 2
```

### Comparing `pqanalysis-1.0.7/tests/io/test_restartWriter.py` & `pqanalysis-1.0.8.1/tests/io/test_restartWriter.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/io/test_trajectoryReader.py` & `pqanalysis-1.0.8.1/tests/io/test_trajectoryReader.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/io/test_trajectoryWriter.py` & `pqanalysis-1.0.8.1/tests/io/test_trajectoryWriter.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/io/test_write_api.py` & `pqanalysis-1.0.8.1/tests/io/test_write_api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/physicalData/test_energy.py` & `pqanalysis-1.0.8.1/tests/physicalData/test_energy.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/tools/test_traj_to_com_traj.py` & `pqanalysis-1.0.8.1/tests/tools/test_traj_to_com_traj.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/topology/bonded_topology/test_angle.py` & `pqanalysis-1.0.8.1/tests/topology/bonded_topology/test_angle.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/topology/bonded_topology/test_bond.py` & `pqanalysis-1.0.8.1/tests/topology/bonded_topology/test_bond.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/topology/bonded_topology/test_bondedTopology.py` & `pqanalysis-1.0.8.1/tests/topology/bonded_topology/test_bondedTopology.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/topology/bonded_topology/test_dihedral.py` & `pqanalysis-1.0.8.1/tests/topology/bonded_topology/test_dihedral.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/topology/test_selection.py` & `pqanalysis-1.0.8.1/tests/topology/test_selection.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/topology/test_selectionTransformer.py` & `pqanalysis-1.0.8.1/tests/topology/test_selectionTransformer.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/topology/test_shakeTopology.py` & `pqanalysis-1.0.8.1/tests/topology/test_shakeTopology.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/topology/test_topology.py` & `pqanalysis-1.0.8.1/tests/topology/test_topology.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/traj/test_api.py` & `pqanalysis-1.0.8.1/tests/traj/test_api.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/traj/test_trajectory.py` & `pqanalysis-1.0.8.1/tests/traj/test_trajectory.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/utils/test_common.py` & `pqanalysis-1.0.8.1/tests/utils/test_common.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/utils/test_decorators.py` & `pqanalysis-1.0.8.1/tests/utils/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pqanalysis-1.0.7/tests/utils/test_math.py` & `pqanalysis-1.0.8.1/tests/utils/test_math.py`

 * *Files identical despite different names*

