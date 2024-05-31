# Comparing `tmp/df_file_interchange-0.0.15a0.tar.gz` & `tmp/df_file_interchange-0.0.16a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "df_file_interchange-0.0.15a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "df_file_interchange-0.0.16a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `df_file_interchange-0.0.15a0.tar` & `df_file_interchange-0.0.16a0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     4265 2024-05-29 09:48:09.357860 df_file_interchange-0.0.15a0/.github/workflows/do_tests.yaml
--rw-r--r--   0        0        0     3213 2024-05-29 09:24:12.023876 df_file_interchange-0.0.15a0/.gitignore
--rw-r--r--   0        0        0     1541 2024-05-14 13:52:19.431269 df_file_interchange-0.0.15a0/LICENSE
--rw-r--r--   0        0        0     6379 2024-05-28 10:20:33.308490 df_file_interchange-0.0.15a0/README.md
--rw-r--r--   0        0        0      927 2024-05-28 10:20:33.312490 df_file_interchange-0.0.15a0/df_file_interchange/__init__.py
--rw-r--r--   0        0        0       52 2024-05-14 13:52:19.431269 df_file_interchange-0.0.15a0/df_file_interchange/ci/__init__.py
--rw-r--r--   0        0        0     1211 2024-05-14 13:52:19.431269 df_file_interchange-0.0.15a0/df_file_interchange/ci/base.py
--rw-r--r--   0        0        0     1299 2024-05-14 13:52:19.431269 df_file_interchange-0.0.15a0/df_file_interchange/ci/examples.py
--rw-r--r--   0        0        0       44 2024-05-14 13:52:19.431269 df_file_interchange-0.0.15a0/df_file_interchange/ci/extra/__init__.py
--rw-r--r--   0        0        0      938 2024-05-14 13:52:19.431269 df_file_interchange-0.0.15a0/df_file_interchange/ci/extra/base.py
--rw-r--r--   0        0        0      555 2024-05-14 13:52:19.431269 df_file_interchange-0.0.15a0/df_file_interchange/ci/extra/std_extra.py
--rw-r--r--   0        0        0     7250 2024-05-28 10:20:33.312490 df_file_interchange-0.0.15a0/df_file_interchange/ci/structured.py
--rw-r--r--   0        0        0       55 2024-05-14 13:52:19.435269 df_file_interchange-0.0.15a0/df_file_interchange/ci/unit/__init__.py
--rw-r--r--   0        0        0     1321 2024-05-14 13:52:19.435269 df_file_interchange-0.0.15a0/df_file_interchange/ci/unit/base.py
--rw-r--r--   0        0        0     5697 2024-05-28 10:20:33.312490 df_file_interchange-0.0.15a0/df_file_interchange/ci/unit/currency.py
--rw-r--r--   0        0        0      818 2024-05-28 10:20:33.312490 df_file_interchange-0.0.15a0/df_file_interchange/ci/unit/population.py
--rw-r--r--   0        0        0       41 2024-05-14 13:52:19.435269 df_file_interchange-0.0.15a0/df_file_interchange/file/__init__.py
--rw-r--r--   0        0        0    11494 2024-05-28 10:20:33.312490 df_file_interchange-0.0.15a0/df_file_interchange/file/examples.py
--rw-r--r--   0        0        0    80247 2024-05-29 09:48:09.361860 df_file_interchange-0.0.15a0/df_file_interchange/file/rw.py
--rw-r--r--   0        0        0       35 2024-05-28 10:20:33.316490 df_file_interchange-0.0.15a0/df_file_interchange/util/__init__.py
--rw-r--r--   0        0        0     1577 2024-05-29 09:48:09.361860 df_file_interchange-0.0.15a0/df_file_interchange/util/common.py
--rw-r--r--   0        0        0       28 2024-05-29 09:48:09.361860 df_file_interchange-0.0.15a0/df_file_interchange/version.py
--rw-r--r--   0        0        0        0 2024-05-14 10:53:44.460601 df_file_interchange-0.0.15a0/docs/.nojekyll
--rw-r--r--   0        0        0     1479 2024-05-14 13:52:19.443268 df_file_interchange-0.0.15a0/docs/background.md
--rw-r--r--   0        0        0      689 2024-05-14 13:52:19.443268 df_file_interchange-0.0.15a0/docs/code_reference__ci.md
--rw-r--r--   0        0        0      364 2024-05-14 13:52:19.443268 df_file_interchange-0.0.15a0/docs/code_reference__ci_extra.md
--rw-r--r--   0        0        0      475 2024-05-14 13:52:19.443268 df_file_interchange-0.0.15a0/docs/code_reference__ci_unit.md
--rw-r--r--   0        0        0     1739 2024-05-14 13:52:19.443268 df_file_interchange-0.0.15a0/docs/code_reference__file.md
--rw-r--r--   0        0        0     7434 2024-05-28 10:20:33.316490 df_file_interchange-0.0.15a0/docs/custom_info.md
--rw-r--r--   0        0        0     2903 2024-05-28 10:20:33.316490 df_file_interchange-0.0.15a0/docs/getting_started.md
--rw-r--r--   0        0        0     1555 2024-05-14 13:52:19.443268 df_file_interchange-0.0.15a0/docs/index.md
--rw-r--r--   0        0        0      290 2024-05-28 09:01:37.511964 df_file_interchange-0.0.15a0/docs/notebooks/data/tutorial_tring_out_a_save_new_sep.csv
--rw-r--r--   0        0        0     1188 2024-05-28 10:20:33.316490 df_file_interchange-0.0.15a0/docs/notebooks/data/tutorial_tring_out_a_save_new_sep.yaml
--rw-r--r--   0        0        0      290 2024-05-28 09:01:37.495965 df_file_interchange-0.0.15a0/docs/notebooks/data/tutorial_trying_out_a_save.csv
--rw-r--r--   0        0        0     3070 2024-05-28 10:20:33.316490 df_file_interchange-0.0.15a0/docs/notebooks/data/tutorial_trying_out_a_save.parq
--rw-r--r--   0        0        0     1188 2024-05-28 10:20:33.316490 df_file_interchange-0.0.15a0/docs/notebooks/data/tutorial_trying_out_a_save.yaml
--rw-r--r--   0        0        0     1183 2024-05-28 10:20:33.316490 df_file_interchange-0.0.15a0/docs/notebooks/data/tutorial_trying_out_a_save_diff_metafile.yaml
--rw-r--r--   0        0        0     7105 2024-05-28 10:20:33.316490 df_file_interchange-0.0.15a0/docs/notebooks/tutorial_simple_structured_custom_info.ipynb
--rw-r--r--   0        0        0    14318 2024-05-28 10:20:33.316490 df_file_interchange-0.0.15a0/docs/notebooks/tutorial_simple_write_read.ipynb
--rw-r--r--   0        0        0     3607 2024-05-14 13:52:19.451268 df_file_interchange-0.0.15a0/docs/yaml_fields.md
--rw-r--r--   0        0        0      478 2024-05-28 10:31:36.850631 df_file_interchange-0.0.15a0/environment.yaml
--rw-r--r--   0        0        0     1320 2024-05-28 10:20:33.320490 df_file_interchange-0.0.15a0/mkdocs.yml
--rw-r--r--   0        0        0     1516 2024-05-29 09:48:09.361860 df_file_interchange-0.0.15a0/pyproject.toml
--rw-r--r--   0        0        0      887 2024-05-14 13:52:19.455268 df_file_interchange-0.0.15a0/scratch/currency_abbreviations.txt
--rw-r--r--   0        0        0     1064 2024-05-14 13:52:19.455268 df_file_interchange-0.0.15a0/scratch/currency_abbreviations_processed.txt
--rw-r--r--   0        0        0      483 2024-05-29 09:48:09.361860 df_file_interchange-0.0.15a0/scratch/envs_for_older_python/environment_3_10.yaml
--rw-r--r--   0        0        0      481 2024-05-29 09:48:09.361860 df_file_interchange-0.0.15a0/scratch/envs_for_older_python/environment_3_9.yaml
--rw-r--r--   0        0        0     7549 2024-05-14 13:52:19.451268 df_file_interchange-0.0.15a0/scratch/pandas_github_issues/bad_dtype_for_csv_read.ipynb
--rw-r--r--   0        0        0       96 2024-05-14 13:52:19.451268 df_file_interchange-0.0.15a0/scratch/pandas_github_issues/data/test_csv
--rw-r--r--   0        0        0       96 2024-05-28 10:20:33.320490 df_file_interchange-0.0.15a0/scratch/pandas_github_issues/data/test_csv.csv
--rw-r--r--   0        0        0      316 2024-05-28 10:20:33.324490 df_file_interchange-0.0.15a0/scratch/pandas_github_issues/data/test_range_index.csv
--rw-r--r--   0        0        0     5454 2024-05-14 13:52:19.455268 df_file_interchange-0.0.15a0/scratch/pandas_github_issues/datetime_issue_github.ipynb
--rw-r--r--   0        0        0    20732 2024-05-28 10:20:33.324490 df_file_interchange-0.0.15a0/scratch/pandas_github_issues/rangeindex_list_out_of_range.ipynb
--rw-r--r--   0        0        0        0 2024-05-14 13:52:19.471268 df_file_interchange-0.0.15a0/test/__init__.py
--rw-r--r--   0        0        0     2940 2024-05-14 13:52:19.531265 df_file_interchange-0.0.15a0/test/test_custom_info_extend_ci.py
--rw-r--r--   0        0        0     2602 2024-05-14 13:52:19.531265 df_file_interchange-0.0.15a0/test/test_custom_info_structured.py
--rw-r--r--   0        0        0      963 2024-05-28 10:20:33.324490 df_file_interchange-0.0.15a0/test/test_custom_info_units.py
--rw-r--r--   0        0        0     2257 2024-05-14 13:52:19.531265 df_file_interchange-0.0.15a0/test/test_deserialize_check_types.py
--rw-r--r--   0        0        0     1754 2024-05-14 13:52:19.531265 df_file_interchange-0.0.15a0/test/test_indexing_dtypes.py
--rw-r--r--   0        0        0     3108 2024-05-14 13:52:19.531265 df_file_interchange-0.0.15a0/test/test_write_read_examples.py
--rw-r--r--   0        0        0     7635 1970-01-01 00:00:00.000000 df_file_interchange-0.0.15a0/PKG-INFO
+-rw-r--r--   0        0        0     4265 2024-05-29 09:48:09.357860 df_file_interchange-0.0.16a0/.github/workflows/do_tests.yaml
+-rw-r--r--   0        0        0     3213 2024-05-29 09:24:12.023876 df_file_interchange-0.0.16a0/.gitignore
+-rw-r--r--   0        0        0     1541 2024-05-14 13:52:19.431269 df_file_interchange-0.0.16a0/LICENSE
+-rw-r--r--   0        0        0     6379 2024-05-28 10:20:33.308490 df_file_interchange-0.0.16a0/README.md
+-rw-r--r--   0        0        0      927 2024-05-28 10:20:33.312490 df_file_interchange-0.0.16a0/df_file_interchange/__init__.py
+-rw-r--r--   0        0        0       52 2024-05-14 13:52:19.431269 df_file_interchange-0.0.16a0/df_file_interchange/ci/__init__.py
+-rw-r--r--   0        0        0     1211 2024-05-14 13:52:19.431269 df_file_interchange-0.0.16a0/df_file_interchange/ci/base.py
+-rw-r--r--   0        0        0     1299 2024-05-14 13:52:19.431269 df_file_interchange-0.0.16a0/df_file_interchange/ci/examples.py
+-rw-r--r--   0        0        0       44 2024-05-14 13:52:19.431269 df_file_interchange-0.0.16a0/df_file_interchange/ci/extra/__init__.py
+-rw-r--r--   0        0        0      938 2024-05-14 13:52:19.431269 df_file_interchange-0.0.16a0/df_file_interchange/ci/extra/base.py
+-rw-r--r--   0        0        0      555 2024-05-14 13:52:19.431269 df_file_interchange-0.0.16a0/df_file_interchange/ci/extra/std_extra.py
+-rw-r--r--   0        0        0     7250 2024-05-28 10:20:33.312490 df_file_interchange-0.0.16a0/df_file_interchange/ci/structured.py
+-rw-r--r--   0        0        0       55 2024-05-14 13:52:19.435269 df_file_interchange-0.0.16a0/df_file_interchange/ci/unit/__init__.py
+-rw-r--r--   0        0        0     1321 2024-05-14 13:52:19.435269 df_file_interchange-0.0.16a0/df_file_interchange/ci/unit/base.py
+-rw-r--r--   0        0        0     5697 2024-05-28 10:20:33.312490 df_file_interchange-0.0.16a0/df_file_interchange/ci/unit/currency.py
+-rw-r--r--   0        0        0      818 2024-05-28 10:20:33.312490 df_file_interchange-0.0.16a0/df_file_interchange/ci/unit/population.py
+-rw-r--r--   0        0        0       41 2024-05-14 13:52:19.435269 df_file_interchange-0.0.16a0/df_file_interchange/file/__init__.py
+-rw-r--r--   0        0        0    11494 2024-05-28 10:20:33.312490 df_file_interchange-0.0.16a0/df_file_interchange/file/examples.py
+-rw-r--r--   0        0        0    80247 2024-05-29 09:48:09.361860 df_file_interchange-0.0.16a0/df_file_interchange/file/rw.py
+-rw-r--r--   0        0        0       35 2024-05-28 10:20:33.316490 df_file_interchange-0.0.16a0/df_file_interchange/util/__init__.py
+-rw-r--r--   0        0        0     1577 2024-05-29 09:48:09.361860 df_file_interchange-0.0.16a0/df_file_interchange/util/common.py
+-rw-r--r--   0        0        0       28 2024-05-31 14:16:09.130070 df_file_interchange-0.0.16a0/df_file_interchange/version.py
+-rw-r--r--   0        0        0        0 2024-05-14 10:53:44.460601 df_file_interchange-0.0.16a0/docs/.nojekyll
+-rw-r--r--   0        0        0     1479 2024-05-14 13:52:19.443268 df_file_interchange-0.0.16a0/docs/background.md
+-rw-r--r--   0        0        0      689 2024-05-14 13:52:19.443268 df_file_interchange-0.0.16a0/docs/code_reference__ci.md
+-rw-r--r--   0        0        0      364 2024-05-14 13:52:19.443268 df_file_interchange-0.0.16a0/docs/code_reference__ci_extra.md
+-rw-r--r--   0        0        0      475 2024-05-14 13:52:19.443268 df_file_interchange-0.0.16a0/docs/code_reference__ci_unit.md
+-rw-r--r--   0        0        0     1739 2024-05-14 13:52:19.443268 df_file_interchange-0.0.16a0/docs/code_reference__file.md
+-rw-r--r--   0        0        0     7434 2024-05-28 10:20:33.316490 df_file_interchange-0.0.16a0/docs/custom_info.md
+-rw-r--r--   0        0        0     2903 2024-05-28 10:20:33.316490 df_file_interchange-0.0.16a0/docs/getting_started.md
+-rw-r--r--   0        0        0     1555 2024-05-14 13:52:19.443268 df_file_interchange-0.0.16a0/docs/index.md
+-rw-r--r--   0        0        0      290 2024-05-28 09:01:37.511964 df_file_interchange-0.0.16a0/docs/notebooks/data/tutorial_tring_out_a_save_new_sep.csv
+-rw-r--r--   0        0        0     1188 2024-05-28 10:20:33.316490 df_file_interchange-0.0.16a0/docs/notebooks/data/tutorial_tring_out_a_save_new_sep.yaml
+-rw-r--r--   0        0        0      290 2024-05-28 09:01:37.495965 df_file_interchange-0.0.16a0/docs/notebooks/data/tutorial_trying_out_a_save.csv
+-rw-r--r--   0        0        0     3070 2024-05-28 10:20:33.316490 df_file_interchange-0.0.16a0/docs/notebooks/data/tutorial_trying_out_a_save.parq
+-rw-r--r--   0        0        0     1188 2024-05-28 10:20:33.316490 df_file_interchange-0.0.16a0/docs/notebooks/data/tutorial_trying_out_a_save.yaml
+-rw-r--r--   0        0        0     1183 2024-05-28 10:20:33.316490 df_file_interchange-0.0.16a0/docs/notebooks/data/tutorial_trying_out_a_save_diff_metafile.yaml
+-rw-r--r--   0        0        0     7105 2024-05-28 10:20:33.316490 df_file_interchange-0.0.16a0/docs/notebooks/tutorial_simple_structured_custom_info.ipynb
+-rw-r--r--   0        0        0    14318 2024-05-28 10:20:33.316490 df_file_interchange-0.0.16a0/docs/notebooks/tutorial_simple_write_read.ipynb
+-rw-r--r--   0        0        0     3607 2024-05-14 13:52:19.451268 df_file_interchange-0.0.16a0/docs/yaml_fields.md
+-rw-r--r--   0        0        0      478 2024-05-28 10:31:36.850631 df_file_interchange-0.0.16a0/environment.yaml
+-rw-r--r--   0        0        0     1320 2024-05-28 10:20:33.320490 df_file_interchange-0.0.16a0/mkdocs.yml
+-rw-r--r--   0        0        0     1516 2024-05-31 14:15:35.566868 df_file_interchange-0.0.16a0/pyproject.toml
+-rw-r--r--   0        0        0      887 2024-05-14 13:52:19.455268 df_file_interchange-0.0.16a0/scratch/currency_abbreviations.txt
+-rw-r--r--   0        0        0     1064 2024-05-14 13:52:19.455268 df_file_interchange-0.0.16a0/scratch/currency_abbreviations_processed.txt
+-rw-r--r--   0        0        0      483 2024-05-29 09:48:09.361860 df_file_interchange-0.0.16a0/scratch/envs_for_older_python/environment_3_10.yaml
+-rw-r--r--   0        0        0      481 2024-05-29 09:48:09.361860 df_file_interchange-0.0.16a0/scratch/envs_for_older_python/environment_3_9.yaml
+-rw-r--r--   0        0        0     7549 2024-05-14 13:52:19.451268 df_file_interchange-0.0.16a0/scratch/pandas_github_issues/bad_dtype_for_csv_read.ipynb
+-rw-r--r--   0        0        0       96 2024-05-14 13:52:19.451268 df_file_interchange-0.0.16a0/scratch/pandas_github_issues/data/test_csv
+-rw-r--r--   0        0        0       96 2024-05-28 10:20:33.320490 df_file_interchange-0.0.16a0/scratch/pandas_github_issues/data/test_csv.csv
+-rw-r--r--   0        0        0      316 2024-05-28 10:20:33.324490 df_file_interchange-0.0.16a0/scratch/pandas_github_issues/data/test_range_index.csv
+-rw-r--r--   0        0        0     5454 2024-05-14 13:52:19.455268 df_file_interchange-0.0.16a0/scratch/pandas_github_issues/datetime_issue_github.ipynb
+-rw-r--r--   0        0        0    20732 2024-05-28 10:20:33.324490 df_file_interchange-0.0.16a0/scratch/pandas_github_issues/rangeindex_list_out_of_range.ipynb
+-rw-r--r--   0        0        0        0 2024-05-14 13:52:19.471268 df_file_interchange-0.0.16a0/test/__init__.py
+-rw-r--r--   0        0        0     2940 2024-05-14 13:52:19.531265 df_file_interchange-0.0.16a0/test/test_custom_info_extend_ci.py
+-rw-r--r--   0        0        0     2602 2024-05-14 13:52:19.531265 df_file_interchange-0.0.16a0/test/test_custom_info_structured.py
+-rw-r--r--   0        0        0      963 2024-05-28 10:20:33.324490 df_file_interchange-0.0.16a0/test/test_custom_info_units.py
+-rw-r--r--   0        0        0     2257 2024-05-14 13:52:19.531265 df_file_interchange-0.0.16a0/test/test_deserialize_check_types.py
+-rw-r--r--   0        0        0     1754 2024-05-14 13:52:19.531265 df_file_interchange-0.0.16a0/test/test_indexing_dtypes.py
+-rw-r--r--   0        0        0     3108 2024-05-14 13:52:19.531265 df_file_interchange-0.0.16a0/test/test_write_read_examples.py
+-rw-r--r--   0        0        0     7635 1970-01-01 00:00:00.000000 df_file_interchange-0.0.16a0/PKG-INFO
```

### Comparing `df_file_interchange-0.0.15a0/.github/workflows/do_tests.yaml` & `df_file_interchange-0.0.16a0/.github/workflows/do_tests.yaml`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/.gitignore` & `df_file_interchange-0.0.16a0/.gitignore`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/LICENSE` & `df_file_interchange-0.0.16a0/LICENSE`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/README.md` & `df_file_interchange-0.0.16a0/README.md`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/df_file_interchange/__init__.py` & `df_file_interchange-0.0.16a0/df_file_interchange/__init__.py`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/df_file_interchange/ci/base.py` & `df_file_interchange-0.0.16a0/df_file_interchange/ci/base.py`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/df_file_interchange/ci/examples.py` & `df_file_interchange-0.0.16a0/df_file_interchange/ci/examples.py`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/df_file_interchange/ci/extra/base.py` & `df_file_interchange-0.0.16a0/df_file_interchange/ci/extra/base.py`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/df_file_interchange/ci/extra/std_extra.py` & `df_file_interchange-0.0.16a0/df_file_interchange/ci/extra/std_extra.py`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/df_file_interchange/ci/structured.py` & `df_file_interchange-0.0.16a0/df_file_interchange/ci/structured.py`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/df_file_interchange/ci/unit/base.py` & `df_file_interchange-0.0.16a0/df_file_interchange/ci/unit/base.py`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/df_file_interchange/ci/unit/currency.py` & `df_file_interchange-0.0.16a0/df_file_interchange/ci/unit/currency.py`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/df_file_interchange/ci/unit/population.py` & `df_file_interchange-0.0.16a0/df_file_interchange/ci/unit/population.py`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/df_file_interchange/file/examples.py` & `df_file_interchange-0.0.16a0/df_file_interchange/file/examples.py`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/df_file_interchange/file/rw.py` & `df_file_interchange-0.0.16a0/df_file_interchange/file/rw.py`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/df_file_interchange/util/common.py` & `df_file_interchange-0.0.16a0/df_file_interchange/util/common.py`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/docs/background.md` & `df_file_interchange-0.0.16a0/docs/background.md`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/docs/code_reference__ci.md` & `df_file_interchange-0.0.16a0/docs/code_reference__ci.md`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/docs/code_reference__file.md` & `df_file_interchange-0.0.16a0/docs/code_reference__file.md`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/docs/custom_info.md` & `df_file_interchange-0.0.16a0/docs/custom_info.md`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/docs/getting_started.md` & `df_file_interchange-0.0.16a0/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/docs/index.md` & `df_file_interchange-0.0.16a0/docs/index.md`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/docs/notebooks/data/tutorial_tring_out_a_save_new_sep.yaml` & `df_file_interchange-0.0.16a0/docs/notebooks/data/tutorial_tring_out_a_save_new_sep.yaml`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/docs/notebooks/data/tutorial_trying_out_a_save.parq` & `df_file_interchange-0.0.16a0/docs/notebooks/data/tutorial_trying_out_a_save.parq`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/docs/notebooks/data/tutorial_trying_out_a_save.yaml` & `df_file_interchange-0.0.16a0/docs/notebooks/data/tutorial_trying_out_a_save.yaml`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/docs/notebooks/data/tutorial_trying_out_a_save_diff_metafile.yaml` & `df_file_interchange-0.0.16a0/docs/notebooks/data/tutorial_trying_out_a_save_diff_metafile.yaml`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/docs/notebooks/tutorial_simple_structured_custom_info.ipynb` & `df_file_interchange-0.0.16a0/docs/notebooks/tutorial_simple_structured_custom_info.ipynb`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/docs/notebooks/tutorial_simple_write_read.ipynb` & `df_file_interchange-0.0.16a0/docs/notebooks/tutorial_simple_write_read.ipynb`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/docs/yaml_fields.md` & `df_file_interchange-0.0.16a0/docs/yaml_fields.md`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/mkdocs.yml` & `df_file_interchange-0.0.16a0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/pyproject.toml` & `df_file_interchange-0.0.16a0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 dynamic = ["version"]
 requires-python = ">= 3.10"
 dependencies = [
     "pydantic >= 2.7, < 3",
     "pydantic-settings",
     "numpy >= 1.26.4, < 2",
     "pandas >= 2.2.2, < 3",
-    "pyarrow >= 15.0.2, < 16",
+    "pyarrow >= 16.1.0, < 17",
     "loguru >= 0.7.2, < 1",
     "pyyaml >= 6.0.1, < 7",
 ]
 classifiers = [
   # How mature is this project? Common values are
   #   3 - Alpha
   #   4 - Beta
```

### Comparing `df_file_interchange-0.0.15a0/scratch/currency_abbreviations.txt` & `df_file_interchange-0.0.16a0/scratch/currency_abbreviations.txt`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/scratch/currency_abbreviations_processed.txt` & `df_file_interchange-0.0.16a0/scratch/currency_abbreviations_processed.txt`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/scratch/pandas_github_issues/bad_dtype_for_csv_read.ipynb` & `df_file_interchange-0.0.16a0/scratch/pandas_github_issues/bad_dtype_for_csv_read.ipynb`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/scratch/pandas_github_issues/datetime_issue_github.ipynb` & `df_file_interchange-0.0.16a0/scratch/pandas_github_issues/datetime_issue_github.ipynb`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/scratch/pandas_github_issues/rangeindex_list_out_of_range.ipynb` & `df_file_interchange-0.0.16a0/scratch/pandas_github_issues/rangeindex_list_out_of_range.ipynb`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/test/test_custom_info_extend_ci.py` & `df_file_interchange-0.0.16a0/test/test_custom_info_extend_ci.py`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/test/test_custom_info_structured.py` & `df_file_interchange-0.0.16a0/test/test_custom_info_structured.py`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/test/test_custom_info_units.py` & `df_file_interchange-0.0.16a0/test/test_custom_info_units.py`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/test/test_deserialize_check_types.py` & `df_file_interchange-0.0.16a0/test/test_deserialize_check_types.py`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/test/test_indexing_dtypes.py` & `df_file_interchange-0.0.16a0/test/test_indexing_dtypes.py`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/test/test_write_read_examples.py` & `df_file_interchange-0.0.16a0/test/test_write_read_examples.py`

 * *Files identical despite different names*

### Comparing `df_file_interchange-0.0.15a0/PKG-INFO` & `df_file_interchange-0.0.16a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: df_file_interchange
-Version: 0.0.15a0
+Version: 0.0.16a0
 Summary: Ensures exact round-trip saves with Pandas (CSV/Parquet) and storage of validatable metadata
 Author-email: Esmé Maxwell <osdev@allicient.co.uk>
 Requires-Python: >= 3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: File Formats
 Requires-Dist: pydantic >= 2.7, < 3
 Requires-Dist: pydantic-settings
 Requires-Dist: numpy >= 1.26.4, < 2
 Requires-Dist: pandas >= 2.2.2, < 3
-Requires-Dist: pyarrow >= 15.0.2, < 16
+Requires-Dist: pyarrow >= 16.1.0, < 17
 Requires-Dist: loguru >= 0.7.2, < 1
 Requires-Dist: pyyaml >= 6.0.1, < 7
 Requires-Dist: pytest >= 8.2.0 ; extra == "test"
 Project-URL: Documentation, https://ntnu-indecol.github.io/df_file_interchange/
 Project-URL: Home, https://github.com/EXIOBASE/df_file_interchange
 Project-URL: Issues, https://github.com/EXIOBASE/df_file_interchange/issues
 Provides-Extra: test
```

