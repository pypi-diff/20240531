# Comparing `tmp/fancy_dataclass-0.4.4.tar.gz` & `tmp/fancy_dataclass-0.4.5.tar.gz`

## Comparing `fancy_dataclass-0.4.4.tar` & `fancy_dataclass-0.4.5.tar`

### file list

```diff
@@ -1,80 +1,81 @@
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/.readthedocs.yaml
--rw-r--r--   0        0        0    10102 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass.json
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/mkdocs.yml
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/ruff.toml
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/vermin.ini
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/website_config.toml
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/.github/workflows/workflow.yml
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/docs/.changelog-version-regex.txt
--rw-r--r--   0        0        0     5414 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/docs/LICENSE.txt
--rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/docs/cli.md
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/docs/config.md
--rw-r--r--   0        0        0     3869 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/docs/func.md
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/docs/gen_ref_pages.py
--rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/docs/json.md
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/docs/sql.md
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/docs/subprocess.md
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/docs/toml.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/docs/stylesheets/extra.css
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/__init__.py
--rw-r--r--   0        0        0    24098 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/cli.py
--rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/config.py
--rw-r--r--   0        0        0    16860 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/dict.py
--rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/func.py
--rw-r--r--   0        0        0     6605 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/json.py
--rw-r--r--   0        0        0    12488 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/mixin.py
--rw-r--r--   0        0        0    10866 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/serialize.py
--rw-r--r--   0        0        0     5924 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/sql.py
--rw-r--r--   0        0        0     8167 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/subprocess.py
--rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/toml.py
--rw-r--r--   0        0        0    21398 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/utils.py
--rw-r--r--   0        0        0    16849 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/404.html
--rw-r--r--   0        0        0    29210 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/CHANGELOG.html
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/LICENSE.txt
--rw-r--r--   0        0        0    36316 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/cli.html
--rw-r--r--   0        0        0    37532 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/config.html
--rw-r--r--   0        0        0    35567 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/func.html
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/gen_ref_pages.py
--rw-r--r--   0        0        0    29932 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/index.html
--rw-r--r--   0        0        0    37493 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/json.html
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/objects.inv
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/sitemap.xml
--rw-r--r--   0        0        0    32366 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/sql.html
--rw-r--r--   0        0        0    31503 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/subprocess.html
--rw-r--r--   0        0        0    29136 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/toml.html
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/assets/_mkdocstrings.css
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/assets/images/favicon.png
--rw-r--r--   0        0        0   128974 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/assets/stylesheets/main.bcfcd587.min.css
--rw-r--r--   0        0        0    44820 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/assets/stylesheets/main.bcfcd587.min.css.map
--rw-r--r--   0        0        0    12522 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/assets/stylesheets/palette.06af60db.min.css
--rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/assets/stylesheets/palette.06af60db.min.css.map
--rw-r--r--   0        0        0    17276 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/reference/SUMMARY.html
--rw-r--r--   0        0        0   300109 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/reference/cli.html
--rw-r--r--   0        0        0    77699 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/reference/config.html
--rw-r--r--   0        0        0   164574 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/reference/dict.html
--rw-r--r--   0        0        0    28633 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/reference/func.html
--rw-r--r--   0        0        0    91901 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/reference/json.html
--rw-r--r--   0        0        0   117935 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/reference/mixin.html
--rw-r--r--   0        0        0   137170 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/reference/serialize.html
--rw-r--r--   0        0        0    77797 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/reference/sql.html
--rw-r--r--   0        0        0   120438 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/reference/subprocess.html
--rw-r--r--   0        0        0    63719 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/reference/toml.html
--rw-r--r--   0        0        0   198769 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/reference/utils.html
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/fancy_dataclass/docs/stylesheets/extra.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/tests/__init__.py
--rw-r--r--   0        0        0    30195 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/tests/test_cli.py
--rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/tests/test_config.py
--rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/tests/test_dict.py
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/tests/test_func.py
--rw-r--r--   0        0        0     8598 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/tests/test_inheritance.py
--rw-r--r--   0        0        0    11292 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/tests/test_mixin.py
--rw-r--r--   0        0        0    25727 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/tests/test_serializable.py
--rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/tests/test_sql.py
--rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/tests/test_subprocess.py
--rw-r--r--   0        0        0    13855 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/tests/test_utils.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/.gitignore
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/docs/README.md
--rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/.readthedocs.yaml
+-rw-r--r--   0        0        0    10102 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass.json
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/mkdocs.yml
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/ruff.toml
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/vermin.ini
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/website_config.toml
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/.github/workflows/workflow.yml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/docs/.changelog-version-regex.txt
+-rw-r--r--   0        0        0     5784 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/docs/LICENSE.txt
+-rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/docs/cli.md
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/docs/config.md
+-rw-r--r--   0        0        0     3869 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/docs/func.md
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/docs/gen_ref_pages.py
+-rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/docs/json.md
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/docs/sql.md
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/docs/subprocess.md
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/docs/toml.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/__init__.py
+-rw-r--r--   0        0        0    24127 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/cli.py
+-rw-r--r--   0        0        0     5130 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/config.py
+-rw-r--r--   0        0        0    17279 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/dict.py
+-rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/func.py
+-rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/json.py
+-rw-r--r--   0        0        0    12487 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/py.typed
+-rw-r--r--   0        0        0    11383 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/serialize.py
+-rw-r--r--   0        0        0     5900 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/sql.py
+-rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/subprocess.py
+-rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/toml.py
+-rw-r--r--   0        0        0    21918 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/utils.py
+-rw-r--r--   0        0        0    16849 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/404.html
+-rw-r--r--   0        0        0    29210 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/CHANGELOG.html
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/LICENSE.txt
+-rw-r--r--   0        0        0    36316 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/cli.html
+-rw-r--r--   0        0        0    37532 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/config.html
+-rw-r--r--   0        0        0    35567 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/func.html
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/gen_ref_pages.py
+-rw-r--r--   0        0        0    29932 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/index.html
+-rw-r--r--   0        0        0    37493 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/json.html
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/objects.inv
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/sitemap.xml
+-rw-r--r--   0        0        0    32366 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/sql.html
+-rw-r--r--   0        0        0    31503 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/subprocess.html
+-rw-r--r--   0        0        0    29136 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/toml.html
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/assets/_mkdocstrings.css
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/assets/images/favicon.png
+-rw-r--r--   0        0        0   128974 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/assets/stylesheets/main.bcfcd587.min.css
+-rw-r--r--   0        0        0    44820 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/assets/stylesheets/main.bcfcd587.min.css.map
+-rw-r--r--   0        0        0    12522 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/assets/stylesheets/palette.06af60db.min.css
+-rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/assets/stylesheets/palette.06af60db.min.css.map
+-rw-r--r--   0        0        0    17276 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/reference/SUMMARY.html
+-rw-r--r--   0        0        0   300109 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/reference/cli.html
+-rw-r--r--   0        0        0    77699 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/reference/config.html
+-rw-r--r--   0        0        0   164574 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/reference/dict.html
+-rw-r--r--   0        0        0    28633 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/reference/func.html
+-rw-r--r--   0        0        0    91901 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/reference/json.html
+-rw-r--r--   0        0        0   117935 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/reference/mixin.html
+-rw-r--r--   0        0        0   137170 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/reference/serialize.html
+-rw-r--r--   0        0        0    77797 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/reference/sql.html
+-rw-r--r--   0        0        0   120438 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/reference/subprocess.html
+-rw-r--r--   0        0        0    63719 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/reference/toml.html
+-rw-r--r--   0        0        0   198769 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/reference/utils.html
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/fancy_dataclass/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/tests/__init__.py
+-rw-r--r--   0        0        0    31361 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/tests/test_cli.py
+-rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/tests/test_config.py
+-rw-r--r--   0        0        0     6881 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/tests/test_dict.py
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/tests/test_func.py
+-rw-r--r--   0        0        0     8598 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/tests/test_inheritance.py
+-rw-r--r--   0        0        0    11292 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/tests/test_mixin.py
+-rw-r--r--   0        0        0    26416 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/tests/test_serializable.py
+-rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/tests/test_sql.py
+-rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/tests/test_subprocess.py
+-rw-r--r--   0        0        0    13855 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/tests/test_utils.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/.gitignore
+-rw-r--r--   0        0        0     4885 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/docs/README.md
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.5/PKG-INFO
```

### Comparing `fancy_dataclass-0.4.4/.pre-commit-config.yaml` & `fancy_dataclass-0.4.5/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -36,11 +36,11 @@
       pass_filenames: false
       verbose: true
     - id: loc-summarize
       args: ['fancy_dataclass/*.py']
       pass_filenames: false
       verbose: true
     - id: check-version
-      args: []
+      args: ['--dist-dir', 'dist', '--changelog', 'docs/CHANGELOG.md']
       pass_filenames: false
       verbose: true
       stages: [commit]
```

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass.json` & `fancy_dataclass-0.4.5/fancy_dataclass.json`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/mkdocs.yml` & `fancy_dataclass-0.4.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/ruff.toml` & `fancy_dataclass-0.4.5/ruff.toml`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     "D415",  # first line ending with punctuation
     "E501",  # line length
     "E731",  # assign lambda expression
     "PT001",  # use of pytest.fixture (with no parens)
     "PT013",  # use simple import of pytest
     "PTH123",  # Path.open instead of regular open
     "RET501",  # return None
-    "RET505",  # unnecessary 'else' after 'return'
     "UP006",  # deprecated collection types in annotations
     "UP007",  # | instead of Union
     "UP035"  # import replacements (collections.abc)
 ]
 # ignore = ["B019", "E203", "E251", "E301", "E302", "E305", "E306", "E501", "E722", "E731", "E741", "W292", "W391"]
 
 # paths to exclude
@@ -69,14 +68,15 @@
 
 line-length = 10000
 
 [lint.per-file-ignores]
 "__init__.py" = ["D104", "F401"]
 "tests/*" = ["ANN", "D"]
 
+
 [lint.flake8-pytest-style]
 parametrize-names-type = "list"
 
 [lint.isort]
 # don't separate straight-style and 'from' imports for the same module
 force-sort-within-sections = true
 # force imports to the top of their section
```

### Comparing `fancy_dataclass-0.4.4/.github/workflows/workflow.yml` & `fancy_dataclass-0.4.5/.github/workflows/workflow.yml`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/docs/CHANGELOG.md` & `fancy_dataclass-0.4.5/docs/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,31 @@
     - Removed
     - Fixed
     - Security
 -->
 
 ## [Unreleased]
 
+## [0.4.5]
+
+2024-05-30
+
+### Changed
+
+- `ArgparseDataclass` `subcommand` property to `subcommand_name`
+
+### Fixed
+
+- `ArgparseDataclass`
+    - Preserve snake case for positional arguments instead of replacing `_` with `-`
+
+- `DictDataclass`
+    - Support `numpy` scalars and arrays
+    - Handle string type annotations (see [PEP 563](https://peps.python.org/pep-0563/))
+
 ## [0.4.4]
 
 2024-05-06
 
 ### Added
 
 - Groups, mutually exclusive groups, and subparsers for `ArgparseDataclass`
```

### Comparing `fancy_dataclass-0.4.4/docs/LICENSE.txt` & `fancy_dataclass-0.4.5/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/docs/cli.md` & `fancy_dataclass-0.4.5/docs/cli.md`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/docs/config.md` & `fancy_dataclass-0.4.5/docs/config.md`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/docs/func.md` & `fancy_dataclass-0.4.5/docs/func.md`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/docs/gen_ref_pages.py` & `fancy_dataclass-0.4.5/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/docs/json.md` & `fancy_dataclass-0.4.5/docs/json.md`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/docs/sql.md` & `fancy_dataclass-0.4.5/docs/sql.md`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/docs/subprocess.md` & `fancy_dataclass-0.4.5/docs/subprocess.md`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/docs/toml.md` & `fancy_dataclass-0.4.5/docs/toml.md`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/docs/stylesheets/extra.css` & `fancy_dataclass-0.4.5/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/__init__.py` & `fancy_dataclass-0.4.5/fancy_dataclass/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .json import JSONBaseDataclass, JSONDataclass, JSONSerializable
 from .mixin import DataclassMixin
 from .sql import SQLDataclass
 from .subprocess import SubprocessDataclass
 from .toml import TOMLDataclass
 
 
-__version__ = '0.4.4'
+__version__ = '0.4.5'
 
 __all__ = [
     'ArgparseDataclass',
     'CLIDataclass',
     'Config',
     'ConfigDataclass',
     'DataclassMixin',
```

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/cli.py` & `fancy_dataclass-0.4.5/fancy_dataclass/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,54 +7,54 @@
 from typing_extensions import Self, TypeGuard
 
 from fancy_dataclass.mixin import DataclassMixin, DataclassMixinSettings, FieldSettings
 from fancy_dataclass.utils import camel_case_to_kebab_case, check_dataclass, issubclass_safe, type_is_optional
 
 
 T = TypeVar('T')
+ArgParser = Union[ArgumentParser, _ArgumentGroup]
 
 
 ####################
 # HELPER FUNCTIONS #
 ####################
 
 def _get_parser_group_name(settings: 'ArgparseDataclassFieldSettings', name: str) -> Optional[Tuple[str, bool]]:
     if settings.group:
         if settings.exclusive_group:
             raise ValueError(f'{name!r} specifies both group and exclusive_group: must choose only one')
         return (settings.group, False)
-    else:
-        if settings.exclusive_group:
-            return (settings.exclusive_group, True)
-        return None
+    if settings.exclusive_group:
+        return (settings.exclusive_group, True)
+    return None
 
-def _get_parser_group(parser: ArgumentParser, name: str) -> Optional[_ArgumentGroup]:
+def _get_parser_group(parser: ArgParser, name: str) -> Optional[_ArgumentGroup]:
     for group in getattr(parser, '_action_groups', []):
         if getattr(group, 'title', None) == name:
             assert isinstance(group, _ArgumentGroup)
             return group
     return None
 
-def _get_parser_exclusive_group(parser: ArgumentParser, name: str) -> Optional[_MutuallyExclusiveGroup]:
+def _get_parser_exclusive_group(parser: ArgParser, name: str) -> Optional[_MutuallyExclusiveGroup]:
     for group in getattr(parser, '_mutually_exclusive_groups', []):
         if getattr(group, 'title', None) == name:
             assert isinstance(group, _MutuallyExclusiveGroup)
             return group
     return None
 
-def _add_exclusive_group(parser: ArgumentParser, group_name: str, required: bool) -> _MutuallyExclusiveGroup:
+def _add_exclusive_group(parser: ArgParser, group_name: str, required: bool) -> _MutuallyExclusiveGroup:
     if isinstance(parser, _MutuallyExclusiveGroup):
         raise ValueError('nested exclusive groups are not allowed')
     group = parser.add_mutually_exclusive_group()
     # set the title attribute so the group can be retrieved later
     group.title = group_name
     group.required = required
     return group
 
-def _add_group(parser: ArgumentParser, group_name: str, **group_kwargs: Any) -> _ArgumentGroup:
+def _add_group(parser: ArgParser, group_name: str, **group_kwargs: Any) -> _ArgumentGroup:
     if isinstance(parser, _ArgumentGroup):
         raise ValueError('nested argument groups are not allowed')
     return parser.add_argument_group(group_name, **group_kwargs)
 
 
 ##########
 # MIXINS #
@@ -160,15 +160,15 @@
                     continue
                 raise err
             raise TypeError(f'multiple fields ({subcommand} and {fld.name}) are registered as subcommands, at most one is allowed')
         # store the name of the subcommand field as a private class attribute
         cls._subcommand_field_name = subcommand
 
     @property
-    def subcommand(self) -> Optional[str]:
+    def subcommand_name(self) -> Optional[str]:
         """Gets the name of the chosen subcommand associated with the type of the object's subcommand field.
 
         Returns:
             Name of the subcommand, if a subcommand field exists, and `None` otherwise"""
         if self._subcommand_field_name is not None:
             tp: Type[ArgparseDataclass] = type(getattr(self, self._subcommand_field_name))
             return tp.__settings__.command_name
@@ -194,15 +194,15 @@
 
     @classmethod
     def parser_kwargs(cls) -> Dict[str, Any]:
         """Gets keyword arguments that will be passed to the top-level argument parser.
 
         Returns:
             Keyword arguments passed upon construction of the `ArgumentParser`"""
-        return {'description' : cls.parser_description()}
+        return {'description': cls.parser_description()}
 
     @classmethod
     def parser_argument_kwarg_names(cls) -> List[str]:
         """Gets keyword argument names that will be passed when adding arguments to the argument parser.
 
         Returns:
             Keyword argument names passed when adding arguments to the parser"""
@@ -213,15 +213,15 @@
         """Constructs a new top-level argument parser..
 
         Returns:
             New top-level parser derived from the class's fields"""
         return cls.parser_class()(**cls.parser_kwargs())
 
     @classmethod
-    def configure_argument(cls, parser: ArgumentParser, name: str) -> None:
+    def configure_argument(cls, parser: ArgParser, name: str) -> None:
         """Given an argument parser and a field name, configures the parser with an argument of that name.
 
         Attempts to provide reasonable default behavior based on the dataclass field name, type, default, and metadata.
 
         Subclasses may override this method to implement custom behavior.
 
         Args:
@@ -279,21 +279,21 @@
                 args = [args]
             # argument is positional if it is explicitly given without a leading dash
             positional = not args[0].startswith('-')
             if (not positional) and ('default' not in kwargs):
                 # no default available, so make the field a required option
                 kwargs['required'] = True
         else:
-            argname = fld.name.replace('_', '-')
             positional = (tp is not bool) and ('default' not in kwargs)
             if positional:
-                args = [argname]
+                args = [fld.name]
             else:
                 # use a single dash for 1-letter names
                 prefix = '-' if (len(fld.name) == 1) else '--'
+                argname = fld.name.replace('_', '-')
                 args = [prefix + argname]
         if args and (not positional):
             # store the argument based on the name of the field, and not whatever flag name was provided
             kwargs['dest'] = fld.name
         if fld.type is bool:  # use boolean flag instead of an argument
             action = settings.action or 'store_true'
             kwargs['action'] = action
@@ -321,39 +321,40 @@
             if not group:  # group not found, so create it
                 if is_exclusive:
                     group = _add_exclusive_group(parser, group_name, kwargs.get('required', False))
                 else:
                     # get kwargs from nested ArgparseDataclass
                     group_kwargs: Dict[str, Any] = tp.parser_kwargs() if is_nested(tp) else {}
                     group = _add_group(parser, group_name, **group_kwargs)
-            parser = group  # type: ignore[assignment]
+            parser = group
         if settings.subcommand:
             # create subparsers for each variant
+            assert isinstance(parser, ArgumentParser)
             subparsers = parser.add_subparsers(dest='_subcommand', required=True, help=settings.help, metavar='subcommand')
             tp_args = (tp,) if (origin_type is None) else tp_args
             for arg in tp_args:
                 assert issubclass_safe(arg, ArgparseDataclass)
                 subparser = subparsers.add_parser(arg.__settings__.command_name, help=arg.parser_description())
                 arg.configure_parser(subparser)
             return
         if is_nested(tp):  # recursively configure a nested ArgparseDataclass field
             tp.configure_parser(parser)
         else:
             # prevent duplicate positional args
             if not hasattr(parser, '_pos_args'):
-                parser._pos_args = set()  # type: ignore[attr-defined]
+                parser._pos_args = set()  # type: ignore[union-attr]
             if positional:
-                pos_args = parser._pos_args  # type: ignore[attr-defined]
+                pos_args = parser._pos_args
                 if args[0] in pos_args:
                     raise ValueError(f'duplicate positional argument {args[0]!r}')
                 pos_args.add(args[0])
             parser.add_argument(*args, **kwargs)
 
     @classmethod
-    def configure_parser(cls, parser: ArgumentParser) -> None:
+    def configure_parser(cls, parser: Union[ArgumentParser, _ArgumentGroup]) -> None:
         """Configures an argument parser by adding the appropriate arguments.
 
         By default, this will simply call [`configure_argument`][fancy_dataclass.cli.ArgparseDataclass.configure_argument] for each dataclass field.
 
         Args:
             parser: `ArgumentParser` to configure"""
         check_dataclass(cls)
```

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/config.py` & `fancy_dataclass-0.4.5/fancy_dataclass/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,19 +95,18 @@
         p = Path(path)
         if not p.suffix:
             raise ValueError(f'filename {p} has no extension')
         ext_lower = p.suffix.lower()
         if ext_lower == '.json':
             from fancy_dataclass.json import JSONDataclass
             return JSONDataclass
-        elif ext_lower == '.toml':
+        if ext_lower == '.toml':
             from fancy_dataclass.toml import TOMLDataclass
             return TOMLDataclass
-        else:
-            raise ValueError(f'unknown config file extension {p.suffix!r}')
+        raise ValueError(f'unknown config file extension {p.suffix!r}')
 
     @classmethod
     def load_config(cls, path: AnyPath) -> Self:  # noqa: D102
         tp = cls._get_dataclass_type_for_path(path)
         new_cls: Type[FileSerializable] = ConfigDataclass._wrap_config_dataclass(tp, cls)  # type: ignore
         with open(path) as fp:
             cfg: Self = coerce_to_dataclass(cls, new_cls._from_file(fp))
```

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/dict.py` & `fancy_dataclass-0.4.5/fancy_dataclass/dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from abc import ABC, abstractmethod
 from copy import copy
 import dataclasses
 from dataclasses import Field, dataclass
 from functools import partial
-from typing import TYPE_CHECKING, Any, ClassVar, Dict, Iterable, Literal, Optional, Type, TypeVar, Union, _TypedDictMeta, get_args, get_origin  # type: ignore[attr-defined]
+from typing import TYPE_CHECKING, Any, ClassVar, Dict, Iterable, Literal, Optional, Type, TypeVar, Union, _TypedDictMeta, get_args, get_origin, get_type_hints  # type: ignore[attr-defined]
 
 from typing_extensions import Self, _AnnotatedAlias
 
 from fancy_dataclass.mixin import DataclassMixin, DataclassMixinSettings, FieldSettings
-from fancy_dataclass.utils import TypeConversionError, _flatten_dataclass, check_dataclass, fully_qualified_class_name, issubclass_safe, obj_class_name, safe_dict_insert
+from fancy_dataclass.utils import TypeConversionError, _flatten_dataclass, check_dataclass, fully_qualified_class_name, get_object_from_fully_qualified_name, issubclass_safe, obj_class_name, safe_dict_insert
 
 
 if TYPE_CHECKING:
     from _typeshed import DataclassInstance
 
 T = TypeVar('T', bound=DataclassMixin)
 D = TypeVar('D', bound='DataclassInstance')
@@ -101,17 +101,17 @@
                 if fld.name == 'type':
                     raise TypeError(f"'type' is a reserved dict field for {cls.__name__}, cannot be used as dataclass field")
 
     def _dict_init(self) -> AnyDict:
         """Gets the basic skeleton for a dict generated by this type.
         If `store_type` or `qualified_type` is set to `True`, will include a `type` field to store the type."""
         if self.__settings__.store_type:
-            return {'type' : obj_class_name(self)}
+            return {'type': obj_class_name(self)}
         if self.__settings__.qualified_type:
-            return {'type' : fully_qualified_class_name(self.__class__)}
+            return {'type': fully_qualified_class_name(self.__class__)}
         return {}
 
     @classmethod
     def _to_dict_value_basic(cls, val: Any) -> Any:
         """Converts a value with a basic type to a form appropriate for dict values.
 
         By default this will return the original value. Subclasses may override the behavior, e.g. to perform custom type coercion."""
@@ -120,20 +120,20 @@
     @classmethod
     def _to_dict_value(cls, val: Any, full: bool) -> Any:
         """Converts an arbitrary value to a form appropriate for dict values.
 
         This will recursively process values within containers (lists, dicts, etc.)."""
         if isinstance(val, DictDataclass):
             return val.to_dict(full=full)
-        elif isinstance(val, list):
+        if isinstance(val, list):
             return [cls._to_dict_value(elt, full) for elt in val]
-        elif isinstance(val, tuple):
+        if isinstance(val, tuple):
             return tuple(cls._to_dict_value(elt, full) for elt in val)
-        elif isinstance(val, dict):
-            return {k : cls._to_dict_value(v, full) for (k, v) in val.items()}
+        if isinstance(val, dict):
+            return {k: cls._to_dict_value(v, full) for (k, v) in val.items()}
         return cls._to_dict_value_basic(val)
 
     def _to_dict(self, full: bool) -> AnyDict:
         if self.__settings__.flattened:
             cls = type(self)
             flat_obj = _flatten_dataclass(cls)[1].forward(self)
             return flat_obj._to_dict(full)  # type: ignore
@@ -229,54 +229,54 @@
             if issubclass(tp, dict):
                 if ttp is _TypedDictMeta:  # validate TypedDict fields
                     anns = tp.__annotations__
                     if cls.__settings__.validate and ((not isinstance(val, dict)) or (set(anns) != set(val))):
                         raise err()
                     return {key: convert_val(valtype, val[key]) for (key, valtype) in anns.items()}
                 return tp(val)
-            else:  # basic data type
-                return cls._from_dict_value_basic(tp, val)
-        else:  # compound data type
-            args = get_args(tp)
-            if origin_type == list:
-                subtype = args[0]
-                return [convert_val(subtype, elt) for elt in val]
-            elif origin_type == dict:
-                (keytype, valtype) = args
-                return {convert_val(keytype, k) : convert_val(valtype, v) for (k, v) in val.items()}
-            elif origin_type == tuple:
-                subtypes = args
-                if subtypes[-1] == Ellipsis:  # treat it like a list
-                    subtype = subtypes[0]
-                    return tuple(convert_val(subtype, elt) for elt in val)
-                return tuple(convert_val(subtype, elt) for (subtype, elt) in zip(args, val))
-            elif origin_type == Union:
-                for subtype in args:
-                    try:
-                        # NB: will resolve to the first valid type in the Union
-                        return convert_val(subtype, val)
-                    except Exception:
-                        continue
-            elif origin_type == Literal:
-                if any((val == arg) for arg in args):
-                    # one of the Literal options is matched
-                    return val
-            elif hasattr(origin_type, 'from_dict'):
-                return cls._from_dict_value_convertible(origin_type, val, strict)
-            elif issubclass_safe(origin_type, Iterable):  # arbitrary iterable
-                subtype = args[0]
-                return type(val)(convert_val(subtype, elt) for elt in val)
+            # basic data type
+            return cls._from_dict_value_basic(tp, val)
+        # compound data type
+        args = get_args(tp)
+        if origin_type == list:
+            subtype = args[0]
+            return [convert_val(subtype, elt) for elt in val]
+        if origin_type == dict:
+            (keytype, valtype) = args
+            return {convert_val(keytype, k): convert_val(valtype, v) for (k, v) in val.items()}
+        if origin_type == tuple:
+            subtypes = args
+            if subtypes[-1] == Ellipsis:  # treat it like a list
+                subtype = subtypes[0]
+                return tuple(convert_val(subtype, elt) for elt in val)
+            return tuple(convert_val(subtype, elt) for (subtype, elt) in zip(args, val))
+        if origin_type == Union:
+            for subtype in args:
+                try:
+                    # NB: will resolve to the first valid type in the Union
+                    return convert_val(subtype, val)
+                except Exception:
+                    continue
+        elif origin_type == Literal:
+            if any((val == arg) for arg in args):
+                # one of the Literal options is matched
+                return val
+        elif hasattr(origin_type, 'from_dict'):
+            return cls._from_dict_value_convertible(origin_type, val, strict)
+        elif issubclass_safe(origin_type, Iterable):  # arbitrary iterable
+            subtype = args[0]
+            return type(val)(convert_val(subtype, elt) for elt in val)
         raise err()
 
     @classmethod
     def _get_missing_value(cls, fld: Field) -> Any:  # type: ignore[type-arg]
         raise ValueError(f'{fld.name!r} field is required')
 
     @classmethod
-    def _dataclass_args_from_dict(cls, d: AnyDict, strict: bool = False) -> AnyDict:
+    def dataclass_args_from_dict(cls, d: AnyDict, strict: bool = False) -> AnyDict:
         """Given a dict of arguments, performs type conversion and/or validity checking, then returns a new dict that can be passed to the class's constructor."""
         check_dataclass(cls)
         kwargs = {}
         bases = cls.mro()
         fields = dataclasses.fields(cls)  # type: ignore[arg-type]
         if strict:  # check there are no extraneous fields
             field_names = {field.name for field in fields}
@@ -287,14 +287,19 @@
             if not fld.init:  # suppress fields where init=False
                 continue
             if fld.name in d:
                 # field may be defined in the dataclass itself or one of its ancestor dataclasses
                 for base in bases:
                     try:
                         field_type = base.__annotations__[fld.name]
+                        if isinstance(field_type, str):  # resolve string annotation to a type (see PEP 563)
+                            if '.' in field_type:  # fully qualified: import module and retrieve the type
+                                field_type = get_object_from_fully_qualified_name(field_type)
+                            else:  # builtin or locally defined type
+                                field_type = get_type_hints(base, globalns=globals(), localns=locals())[fld.name]  # type: ignore[arg-type]
                         kwargs[fld.name] = cls._from_dict_value(field_type, d[fld.name], strict=strict)
                         break
                     except (AttributeError, KeyError):
                         pass
                 else:
                     raise ValueError(f'could not locate field {fld.name!r}')
             elif fld.default == dataclasses.MISSING:
@@ -330,19 +335,19 @@
                 # tp must be a subclass of cls
                 # the name must be in scope to be found, allowing two alternatives for retrieval:
                 # option 1: all subclasses of this DictDataclass are defined in the same module as the base class
                 # option 2: the name is fully qualified, so the name can be loaded into scope
                 # call from_dict on the subclass in case it has its own custom implementation
                 # (remove the type name before passing to the constructor)
                 d2 = {key: val for (key, val) in d.items() if (key != 'type')}
-                return cls._get_subclass_with_name(typename).from_dict(d2, **kwargs)
+                return cls.get_subclass_with_name(typename).from_dict(d2, **kwargs)
         conv = None
         if cls.__settings__.flattened:
             # produce equivalent subfield-flattened type
             settings = copy(tp.__settings__)
             settings.flattened = True
             conv = _flatten_dataclass(tp, cls.__bases__)[1]
             tp = conv.to_type  # type: ignore[assignment]
             tp.__settings__ = settings
         strict = kwargs.get('strict', False)
-        result: Self = tp(**tp._dataclass_args_from_dict(d, strict=strict))
+        result: Self = tp(**tp.dataclass_args_from_dict(d, strict=strict))
         return conv.backward(result) if cls.__settings__.flattened else result  # type: ignore
```

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/func.py` & `fancy_dataclass-0.4.5/fancy_dataclass/func.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/json.py` & `fancy_dataclass-0.4.5/fancy_dataclass/json.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
                     valtype = getattr(tp, '__annotations__', {}).get(key)
                     vals.append(val[key] if (valtype is None) else cls._from_dict_value(valtype, val[key], strict=strict))
                 return tp(*vals)
             except KeyError as e:
                 raise TypeConversionError(tp, val) from e
         if origin_type == dict:  # decode keys to be valid JSON
             (keytype, valtype) = get_args(tp)
-            return {cls._json_key_decoder(cls._from_dict_value(keytype, k)) : cls._from_dict_value(valtype, v, strict=strict) for (k, v) in val.items()}
+            return {cls._json_key_decoder(cls._from_dict_value(keytype, k)): cls._from_dict_value(valtype, v, strict=strict) for (k, v) in val.items()}
         return super()._from_dict_value(tp, val)
 
 
 class JSONBaseDataclass(JSONDataclass, qualified_type=True):
     """This class should be used in place of [`JSONDataclass`][fancy_dataclass.json.JSONDataclass] when you intend to inherit from the class.
 
     When converting a subclass to a dict with [`to_dict`][fancy_dataclass.dict.DictDataclass.to_dict], it will store the subclass's type in the `type` field. It will also resolve this type when calling [`from_dict`][fancy_dataclass.dict.DictDataclass.from_dict]."""
```

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/mixin.py` & `fancy_dataclass-0.4.5/fancy_dataclass/mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,15 +228,15 @@
             if key in d:
                 d[key] = val
             else:
                 raise TypeError(f'{key!r} is not a valid field for {obj_class_name(self)}')
         return self.__class__(**d)
 
     @classmethod
-    def _get_subclass_with_name(cls, typename: str) -> Type[Self]:
+    def get_subclass_with_name(cls, typename: str) -> Type[Self]:
         """Gets the subclass of this class with the given name.
 
         Args:
             typename: Name of subclass
 
         Returns:
             Subclass with the given name
```

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/serialize.py` & `fancy_dataclass-0.4.5/fancy_dataclass/serialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from abc import ABC, abstractmethod
 from enum import Enum
 from io import BytesIO, StringIO, TextIOBase
+from numbers import Integral
 from pathlib import Path
 from typing import IO, Any, BinaryIO, Union, cast
 
 from typing_extensions import Self
 
 from fancy_dataclass.dict import AnyDict, DictDataclass
 from fancy_dataclass.utils import AnyIO, AnyPath, TypeConversionError
@@ -16,41 +17,53 @@
     Args:
         val: Value with basic data type
 
     Returns:
         A version of that value suitable for serialization"""
     if isinstance(val, Enum):
         return val.value
-    elif isinstance(val, range):  # store the range bounds
+    if isinstance(val, range):  # store the range bounds
         bounds = [val.start, val.stop]
         if val.step != 1:
             bounds.append(val.step)
         return bounds
-    elif hasattr(val, 'dtype'):  # assume it's a numpy array of numbers
-        return [float(elt) for elt in val]
+    if hasattr(val, 'dtype'):
+        if hasattr(val, '__len__'):  # assume it's a numpy array of numbers
+            return [float(elt) for elt in val]
+        # numpy scalars have trouble serializing
+        if isinstance(val, Integral):
+            return int(val)
+        if isinstance(val, float):
+            return float(val)
     return val
 
 def from_dict_value_basic(tp: type, val: Any) -> Any:
     """Converts a deserialized value to the given type.
 
     Args:
         tp: Target type to convert to
         val: Deserialized value
 
     Returns:
         Converted value"""
     if issubclass(tp, float):
         return tp(val)
+    if issubclass(tp, Integral) and isinstance(val, Integral):
+        # also handles numpy integer types
+        return tp(val)  # type: ignore[call-arg]
     if issubclass(tp, range):
         return tp(*val)
     if issubclass(tp, Enum):
         try:
             return tp(val)
         except ValueError as e:
             raise TypeConversionError(tp, val) from e
+    if getattr(tp, '__name__', None) == 'ndarray':  # numpy array
+        import numpy as np
+        return np.array(val)
     return val
 
 
 class FileSerializable:
     """Mixin class enabling serialization of an object to/from a file (either text or binary)."""
 
     @classmethod
@@ -319,12 +332,12 @@
             kwargs: Keyword arguments
 
         Returns:
             A dict representation of the file"""
 
     @classmethod
     def _from_text_file(cls, fp: IO[str], **kwargs: Any) -> Self:
-         # pop off known DictDataclass.from_dict kwargs
-         default_dict_kwargs = {'strict': False}
-         load_kwargs = {key: val for (key, val) in kwargs.items() if (key not in default_dict_kwargs)}
-         from_dict_kwargs = {key: kwargs.get(key, default_dict_kwargs[key]) for key in default_dict_kwargs}
-         return cls.from_dict(cls._text_file_to_dict(fp, **load_kwargs), **from_dict_kwargs)
+        # pop off known DictDataclass.from_dict kwargs
+        default_dict_kwargs = {'strict': False}
+        load_kwargs = {key: val for (key, val) in kwargs.items() if (key not in default_dict_kwargs)}
+        from_dict_kwargs = {key: kwargs.get(key, default_dict_kwargs[key]) for key in default_dict_kwargs}
+        return cls.from_dict(cls._text_file_to_dict(fp, **load_kwargs), **from_dict_kwargs)
```

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/sql.py` & `fancy_dataclass-0.4.5/fancy_dataclass/sql.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,26 +23,25 @@
     Args:
         tp: A Python type
 
     Returns:
         Corresponding sqlalchemy column type"""
     if issubclass(tp, str):
         return String
-    elif issubclass(tp, bool):
+    if issubclass(tp, bool):
         return Boolean
-    elif issubclass(tp, int):
+    if issubclass(tp, int):
         return Integer
-    elif issubclass(tp, float):
+    if issubclass(tp, float):
         return Numeric
-    elif issubclass(tp, bytes):
+    if issubclass(tp, bytes):
         return LargeBinary
-    elif issubclass(tp, datetime):
+    if issubclass(tp, datetime):
         return DateTime
-    else:
-        return PickleType
+    return PickleType
 
 
 @dataclass
 class SQLDataclassFieldSettings(FieldSettings):
     """Settings for [`SQLDataclass`][fancy_dataclass.sql.SQLDataclass] fields.
 
     Each field may define a `metadata` dict containing any of the following entries:
```

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/subprocess.py` & `fancy_dataclass-0.4.5/fancy_dataclass/subprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
         Returns:
             List of command-line args corresponding to the dataclass fields"""
         executable = self.get_executable()
         if not executable:
             raise ValueError(f'no executable identified for use with {obj_class_name(self)} instance')
         args = [executable]
         for fld in fields(self):  # type: ignore[arg-type]
-            args += [arg for arg in self.get_arg(fld.name, suppress_defaults = suppress_defaults) if arg]
+            args += [arg for arg in self.get_arg(fld.name, suppress_defaults=suppress_defaults) if arg]
         return args
 
     def run_subprocess(self, **kwargs: Any) -> subprocess.CompletedProcess:  # type: ignore[type-arg]
         """Executes the full subprocess command corresponding to the dataclass parameters.
 
         Args:
             kwargs: Keyword arguments passed to `subprocess.run`
```

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/toml.py` & `fancy_dataclass-0.4.5/fancy_dataclass/toml.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/utils.py` & `fancy_dataclass-0.4.5/fancy_dataclass/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,21 +169,21 @@
     This attempts to be somewhat more robust than `isinstance` in that it will handle compound types like `List[...]`."""
     # TODO: make this more complete
     if tp is Any:
         return True
     origin = get_origin(tp)
     if origin is Union:
         return any(_is_instance(obj, arg) for arg in get_args(tp))
-    elif origin in [list, collections.abc.Sequence]:
+    if origin in [list, collections.abc.Sequence]:
         base_type = get_args(tp)[0]
         return isinstance(obj, origin) and all(_is_instance(val, base_type) for val in obj)
-    elif origin is dict:
+    if origin is dict:
         (key_type, val_type) = get_args(tp)
         return isinstance(obj, dict) and all(_is_instance(key, key_type) and _is_instance(val, val_type) for (key, val) in obj.items())
-    elif origin is collections.abc.Callable:
+    if origin is collections.abc.Callable:
         # TODO: try to check object's annotations
         return isinstance(obj, Callable)  # type: ignore[arg-type]
     return isinstance(obj, tp)
 
 def obj_class_name(obj: object) -> str:
     """Gets the name of the class of an object.
 
@@ -200,14 +200,32 @@
     Args:
         cls: A Python class
 
     Returns:
         Fully qualified name of the class"""
     return f'{cls.__module__}.{cls.__qualname__}'
 
+def get_object_from_fully_qualified_name(name: str) -> object:
+    """Given a fully-qualified name of some object, gets the object, importing the module as needed.
+
+    Args:
+        name: Fully qualified object name
+
+    Returns:
+        Object with the fully qualified name
+
+    Raises:
+        ValueError: If the name does not have a . character"""
+    if '.' not in name:
+        raise ValueError(f'{name!r} is not a fully qualified name')
+    toks = name.split('.')
+    mod_name, obj_name = '.'.join(toks[:-1]), toks[-1]
+    mod = importlib.import_module(mod_name)
+    return getattr(mod, obj_name)
+
 def get_subclass_with_name(cls: Type[T], name: str) -> Type[T]:
     """Gets the subclass of a class with the given name.
 
     Args:
         cls: A Python class
         name: Name of the subclass
 
@@ -217,17 +235,15 @@
     Raises:
         ValueError: If no subclass with the given name exists"""
     fully_qualified = '.' in name
     cls_name = fully_qualified_class_name(cls) if fully_qualified else cls.__name__
     if cls_name == name:
         return cls
     if fully_qualified:  # import the module
-        toks = name.split('.')
-        mod_name, cls_name = '.'.join(toks[:-1]), toks[-1]
-        importlib.import_module(mod_name)
+        _ = get_object_from_fully_qualified_name(name)
     for subcls in all_subclasses(cls):
         subcls_name = fully_qualified_class_name(subcls) if fully_qualified else subcls.__name__
         if subcls_name == name:
             return subcls
     else:
         raise ValueError(f'{name} is not a known subclass of {cls.__name__}')
 
@@ -256,15 +272,15 @@
 
     Returns:
         A dataclass type with the given fields and constructors"""
     def __init__(self: 'DataclassInstance', *args: Any) -> None:
         # take inputs and wrap them in the provided constructors
         for (fld, cons, arg) in zip(dataclasses.fields(self), constructors, args):
             setattr(self, fld.name, cons(arg))
-    tp = make_dataclass(cls_name, fields, init = False, **kwargs)
+    tp = make_dataclass(cls_name, fields, init=False, **kwargs)
     tp.__init__ = __init__  # type: ignore
     # store the field names in a tuple, to match the behavior of namedtuple
     tp._fields = tuple(fld.name for fld in dataclasses.fields(tp))  # type: ignore[attr-defined]
     return tp
 
 def get_dataclass_fields(obj: Union[type, object], include_classvars: bool = False) -> Tuple[Field, ...]:  # type: ignore[type-arg]
     """Variant of `dataclasses.fields` which can optionally include ClassVars.
```

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/404.html` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/404.html`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/CHANGELOG.html` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/CHANGELOG.html`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/LICENSE.txt` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/cli.html` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/cli.html`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/config.html` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/config.html`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/func.html` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/func.html`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/gen_ref_pages.py` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/gen_ref_pages.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,12 +26,12 @@
         # parts = parts[:-1]
         continue
     elif parts[-1] == '__main__':
         continue
     nav[parts] = doc_path.as_posix()
     with mkdocs_gen_files.open(full_doc_path, 'w') as f:
         identifier = '.'.join(parts)
-        print(f'::: {PKG_NAME}.{identifier}', file = f)
+        print(f'::: {PKG_NAME}.{identifier}', file=f)
     mkdocs_gen_files.set_edit_path(full_doc_path, path)
 
 with mkdocs_gen_files.open(REF_DIR / 'SUMMARY.md', 'w') as nav_file:
     nav_file.writelines(nav.build_literate_nav())
```

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/index.html` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/index.html`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/json.html` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/json.html`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/objects.inv` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/objects.inv`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/sql.html` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/sql.html`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/subprocess.html` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/subprocess.html`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/toml.html` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/toml.html`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/assets/_mkdocstrings.css` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/assets/_mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/assets/images/favicon.png` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/assets/stylesheets/main.bcfcd587.min.css` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/assets/stylesheets/main.bcfcd587.min.css`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/assets/stylesheets/main.bcfcd587.min.css.map` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/assets/stylesheets/main.bcfcd587.min.css.map`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/assets/stylesheets/palette.06af60db.min.css` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/assets/stylesheets/palette.06af60db.min.css`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/assets/stylesheets/palette.06af60db.min.css.map` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/assets/stylesheets/palette.06af60db.min.css.map`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/reference/SUMMARY.html` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/reference/SUMMARY.html`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/reference/cli.html` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/reference/cli.html`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/reference/config.html` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/reference/config.html`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/reference/dict.html` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/reference/dict.html`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/reference/func.html` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/reference/func.html`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/reference/json.html` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/reference/json.html`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/reference/mixin.html` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/reference/mixin.html`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/reference/serialize.html` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/reference/serialize.html`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/reference/sql.html` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/reference/sql.html`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/reference/subprocess.html` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/reference/subprocess.html`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/reference/toml.html` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/reference/toml.html`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/reference/utils.html` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/reference/utils.html`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/fancy_dataclass/docs/stylesheets/extra.css` & `fancy_dataclass-0.4.5/fancy_dataclass/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/tests/test_cli.py` & `fancy_dataclass-0.4.5/tests/test_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -267,19 +267,24 @@
     class DC24(ArgparseDataclass):
         vals: List[int] = field(metadata={'nargs': 2})
     assert DC24.from_cli_args(['1', '2']).vals == [1, 2]
     check_invalid_args(DC24, [], 'required: vals')
     check_invalid_args(DC24, ['1'], 'required: vals')
     check_invalid_args(DC24, ['1', 'a'], "invalid int value: 'a'")
     check_invalid_args(DC24, ['1', '2', '3'], 'unrecognized arguments: 3')
-    # custom type constructor
+
+def test_positional():
+    """Tests positional argument."""
     @dataclass
-    class DC25(ArgparseDataclass):
-        x: int = field(metadata={'type': lambda x: int(x) + 1})
-    assert DC25.from_cli_args(['1']).x == 2
+    class DCPos(ArgparseDataclass):
+        pos_arg: str
+    help_str = DCPos.make_parser().format_help()
+    assert 'pos_arg' in help_str
+    assert DCPos.from_cli_args(['a']) == DCPos('a')
+    check_invalid_args(DCPos, ['--pos-arg', 'a'], 'unrecognized arguments: --pos-arg')
 
 def test_groups():
     """Tests the behavior of groups and nested groups."""
     # basic group
     @dataclass
     class DCGroup1(ArgparseDataclass):
         """Docstring for DCGroup1."""
@@ -479,23 +484,23 @@
         """First subcommand"""
         x1: int
         y1: int
         def run(self) -> None:
             print(self.__class__.__name__)
     assert Sub1.__settings__.command_name == 'sub1'
     assert Sub1._subcommand_field_name is None
-    assert Sub1(1, 2).subcommand is None
+    assert Sub1(1, 2).subcommand_name is None
     @dataclass
     class Sub2(ArgparseDataclass, command_name='my-subcommand'):
         """Second subcommand"""
         x2: int
         y2: str = 'abc'
     assert Sub2.__settings__.command_name == 'my-subcommand'
     assert Sub2._subcommand_field_name is None
-    assert Sub2(1, 2).subcommand is None
+    assert Sub2(1, 2).subcommand_name is None
     # multiple subcommands not allowed
     with pytest.raises(TypeError, match='multiple fields .* registered as subcommands'):
         @dataclass
         class DCSub1(ArgparseDataclass):
             sub1: Sub1 = field(metadata={'subcommand': True})
             sub2: Sub2 = field(metadata={'subcommand': True})
     # subcommand must be ArgparseDataclass or union thereof
@@ -511,15 +516,15 @@
     @dataclass
     class DCSub4(ArgparseDataclass):
         sub1: Sub1 = field(metadata={'subcommand': True})
         x: int = field(metadata={'help': 'x value'})  # positional arg in addition to subparser is allowed, though it's weird
         y: int = 2
     assert DCSub4.__settings__.command_name == 'dc-sub4'
     assert DCSub4._subcommand_field_name == 'sub1'
-    assert DCSub4(Sub1(1, 2), 1).subcommand == 'sub1'
+    assert DCSub4(Sub1(1, 2), 1).subcommand_name == 'sub1'
     help_str = DCSub4.make_parser().format_help()
     assert re.search(r'positional arguments:.+sub1\s+First subcommand\s+x\s+x value\s+option.+-y Y', help_str, re.DOTALL)
     check_invalid_args(DCSub4, [], 'the following arguments are required: subcommand, x')
     check_invalid_args(DCSub4, ['5'], "invalid choice: '5'")
     for args in [['sub1'], ['sub1', '1']]:
         check_invalid_args(DCSub4, args, 'the following arguments are required: x1, y1')
     check_invalid_args(DCSub4, ['sub1', '1', '2'], 'the following arguments are required: y1')
@@ -528,16 +533,16 @@
     # union subcommand
     @dataclass
     class DCSub5(CLIDataclass):
         sub: Union[Sub1, Sub2] = field(metadata={'subcommand': True, 'help': 'choose a subcommand'})
         x: int = 1
     assert DCSub5.__settings__.command_name == 'dc-sub5'
     assert DCSub5._subcommand_field_name == 'sub'
-    assert DCSub5(Sub1(1, 2)).subcommand == 'sub1'
-    assert DCSub5(Sub2(1, 2)).subcommand == 'my-subcommand'
+    assert DCSub5(Sub1(1, 2)).subcommand_name == 'sub1'
+    assert DCSub5(Sub2(1, 2)).subcommand_name == 'my-subcommand'
     help_str = DCSub5.make_parser().format_help()
     assert re.search(r'positional arguments:.+choose a subcommand\s+sub1\s+First subcommand\s+my-subcommand\s+Second subcommand.+-x X', help_str, re.DOTALL)
     for args in [[], ['-x', '5']]:
         check_invalid_args(DCSub5, args, 'the following arguments are required: subcommand')
     check_invalid_args(DCSub5, ['sub1'], 'required: x1, y1')
     check_invalid_args(DCSub5, ['sub1', '1'], 'required: y1')
     check_invalid_args(DCSub5, ['sub1', '1', '2', '3'], 'unrecognized arguments: 3')
@@ -615,7 +620,30 @@
         _ = DCFlagDefaultFalseActionFalse.make_parser()
     # action must be 'store_true' or 'store_false'
     @dataclass
     class DCFlagActionStore(ArgparseDataclass):
         flag: bool = field(default=False, metadata={'action': 'store'})
     with pytest.raises(ValueError, match="invalid action 'store'"):
         _ = DCFlagActionStore.make_parser()
+
+def test_type_metadata():
+    """Tests the behavior of using the "type" entry in the field metadata."""
+    @dataclass
+    class DCTypeMismatch(ArgparseDataclass):
+        x: int = field(default=1, metadata={'type': str})
+    assert DCTypeMismatch.from_cli_args([]).x == 1
+    assert DCTypeMismatch.from_cli_args(['-x', '1']).x == '1'
+    @dataclass
+    class DCTypeCallable(ArgparseDataclass):
+        x: int = field(metadata={'type': lambda x: int(x) + 1})
+    assert DCTypeCallable.from_cli_args(['1']).x == 2
+    def positive_int(s):
+        x = int(s)
+        if x < 0:
+            raise ValueError('negative number')
+        return x
+    @dataclass
+    class DCTypeCallable(ArgparseDataclass):
+        x: int = field(metadata={'type': positive_int})
+    assert DCTypeCallable.from_cli_args(['0']).x == 0
+    check_invalid_args(DCTypeCallable, ['a'], "invalid positive_int value: 'a'")
+    check_invalid_args(DCTypeCallable, ['-1'], "invalid positive_int value: '-1'")
```

### Comparing `fancy_dataclass-0.4.4/tests/test_config.py` & `fancy_dataclass-0.4.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/tests/test_dict.py` & `fancy_dataclass-0.4.5/tests/test_dict.py`

 * *Files 14% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     @dataclass
     class DC2(DictDataclass, store_type=True):
         x: int
     assert DC2(1).to_dict() == {'type': 'DC2', 'x': 1}
     @dataclass
     class DC3(DictDataclass, qualified_type=True):
         x: int
-    obj = DC3(1)
+    obj: object = DC3(1)
     d = obj.to_dict()
     assert d == {'type': 'tests.test_dict.test_type_field.<locals>.DC3', 'x': 1}
     assert DC3.from_dict(d) == obj
     assert DC3.from_dict({'type': 'DC3', 'x': 1}) == obj
     with pytest.raises(ValueError, match='fake is not a known subclass of DC3'):
         _ = DC3.from_dict({'type': 'fake', 'x': 1})
     # 'type' dataclass field prohibited (this is caught at dataclass wrap time)
@@ -115,29 +115,64 @@
         @dataclass
         class DC4(DictDataclass, store_type=True):
             type: int
     with pytest.raises(TypeError, match="'type' is a reserved dict field"):
         @dataclass
         class DC5(DictDataclass, store_type=True):
             type: Optional[int] = None
+    # string-annotated dataclass fields
+    @dataclass
+    class DC6(DictDataclass):
+        x: 'int'
+    obj = DC6(1)
+    assert DC6.from_dict(obj.to_dict()) == obj
+    @dataclass
+    class DC7(DictDataclass):
+        x: 'numbers.Number'  # type: ignore[name-defined]  # noqa: F821
+    obj = DC7(1)
+    assert DC7.from_dict(obj.to_dict()) == obj
+    # globally-scoped class, as string
+    @dataclass
+    class DC8(DictDataclass):
+        a: 'NestedComponentA'
+    obj = DC8(NestedComponentA(1, 3.7))
+    d = obj.to_dict()
+    assert 'NestedComponentA' in globals()
+    # NOTE: inner function cannot access globals/locals of higher stack frame
+    with pytest.raises(NameError, match="name 'NestedComponentA' is not defined"):
+        _ = DC8.from_dict(obj.to_dict())
+    # fully qualified name OK
+    @dataclass
+    class DC9(DictDataclass):
+        a: 'tests.test_dict.NestedComponentA'  # type: ignore[name-defined]  # noqa: F821
+    obj = DC9(NestedComponentA(1, 3.7))
+    assert DC9.from_dict(obj.to_dict()) == obj
+    # locally-scoped class, as string (no way to fully qualify it)
+    @dataclass
+    class DC10(DictDataclass):
+        x: 'DC1'
+    obj = DC10(DC1(1))
+    d = obj.to_dict()
+    with pytest.raises(NameError, match="name 'DC1' is not defined"):
+        _ = DC10.from_dict(d)
 
 def test_flattened():
     """Tests the flattened=True option for DictDataclass."""
     @dataclass
     class DC3(DictDataclass):
         y3: int
     @dataclass
     class DC2(DictDataclass):
         x2: DC3
         y2: int
     @dataclass
     class DC1Nested(DictDataclass):
         x1: DC2
         y1: int
-    obj_nested = DC1Nested(DC2(DC3(3),2),1)
+    obj_nested = DC1Nested(DC2(DC3(3), 2),1)
     assert obj_nested.to_dict() == {'x1': {'x2': {'y3': 3}, 'y2': 2}, 'y1': 1}
     @dataclass
     class DC1Flat(DictDataclass, flattened=True):
         x1: DC2
         y1: int
     obj_flat = DC1Flat(DC2(DC3(3),2),1)
     assert obj_flat.to_dict() == {'y1': 1, 'y2': 2, 'y3': 3}
```

### Comparing `fancy_dataclass-0.4.4/tests/test_func.py` & `fancy_dataclass-0.4.5/tests/test_func.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/tests/test_inheritance.py` & `fancy_dataclass-0.4.5/tests/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/tests/test_mixin.py` & `fancy_dataclass-0.4.5/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/tests/test_serializable.py` & `fancy_dataclass-0.4.5/tests/test_serializable.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from datetime import datetime
 from enum import Enum, Flag, auto
 import math
 import re
 import sys
 from typing import Any, ClassVar, List, Literal, NamedTuple, Optional, TypedDict, Union
 
+import numpy as np
 import pytest
 from typing_extensions import Annotated, Doc
 
 from fancy_dataclass.dict import DictDataclass
 from fancy_dataclass.json import JSONBaseDataclass, JSONDataclass
 from fancy_dataclass.toml import TOMLDataclass
 from fancy_dataclass.utils import coerce_to_dataclass, dataclass_type_map, issubclass_safe
@@ -32,16 +33,18 @@
                 elif issubclass_safe(base, JSONDataclass):
                     base = _convert_json_dataclass(base, new_cls)
                 bases.append(base)
             return type(tp.__name__, tuple(bases), dict(tp.__dict__))
         return tp
     tp = _convert(dataclass_type_map(cls, _convert))
     tp.__eq__ = cls.__eq__
+    tp.__settings__ = cls.__settings__
     return tp
 
+
 ################
 # TEST CLASSES #
 ################
 
 @dataclass
 class DCEmpty(JSONDataclass):
     ...
@@ -202,14 +205,32 @@
     vals: List[DCAny]
 
 @dataclass
 class DCListOptional(JSONDataclass):
     vals: List[Optional[int]]
 
 
+@dataclass
+class DCNumpy(JSONDataclass, suppress_defaults=False):
+    num_int: np.int64 = np.int64(1)
+    num_float: np.float64 = np.float64(1)
+    arr_int: np.ndarray = field(default_factory=lambda: np.ones(3, dtype=np.int64))
+    arr_float: np.ndarray = field(default_factory=lambda: np.ones(3, dtype=np.float64))
+
+    def __eq__(self, other):
+        for name in self.__dataclass_fields__:
+            val1, val2 = getattr(self, name), getattr(other, name)
+            if isinstance(val1, np.ndarray):
+                if not np.array_equal(val1, val2):
+                    return False
+            elif val1 != val2:
+                return False
+        return True
+
+
 # DictDataclass versions
 DictDCDatetime = _convert_json_dataclass(DCDatetime, DictDataclass)
 DictDCEnum = _convert_json_dataclass(DCEnum, DictDataclass)
 DictDCRange = _convert_json_dataclass(DCRange, DictDataclass)
 
 
 TEST_JSON = [
@@ -240,14 +261,15 @@
     DCAny(3),
     DCAny('a'),
     DCAny({}),
     DCAny(None),
     DCSuppress(),
     DCSuppress2(),
     DCList([DCAny(None), DCAny(1), DCAny([1]), DCAny(None), DCAny({})]),
+    DCNumpy(),
 ]
 
 class TestDict:
     """Unit tests for DictDataclass."""
 
     base_cls = DictDataclass
     ext: str = None
@@ -273,21 +295,19 @@
         else:
             assert 'type' not in obj.to_dict()
         assert tp.from_dict(obj.to_dict()) == obj
 
     def _get_conversion_contexts(self, err):
         if err is None:
             return (True, nullcontext(), nullcontext())
-        else:
-            (fwd_ok, errtype, match) = err
-            err_ctx = pytest.raises(errtype, match=match)
-            if fwd_ok:  # error occurs when converting back
-                return (True, nullcontext(), err_ctx)
-            else:
-                return (False, err_ctx, nullcontext())
+        (fwd_ok, errtype, match) = err
+        err_ctx = pytest.raises(errtype, match=match)
+        if fwd_ok:  # error occurs when converting back
+            return (True, nullcontext(), err_ctx)
+        return (False, err_ctx, nullcontext())
 
     def _test_dict_convert(self, obj, d, err):
         """Tests that an object gets converted to the expected dict and back."""
         (fwd_ok, fwd_ctx, bwd_ctx) = self._get_conversion_contexts(err)
         with fwd_ctx:
             assert obj.to_dict() == d
         if fwd_ok:
```

### Comparing `fancy_dataclass-0.4.4/tests/test_sql.py` & `fancy_dataclass-0.4.5/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/tests/test_subprocess.py` & `fancy_dataclass-0.4.5/tests/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/tests/test_utils.py` & `fancy_dataclass-0.4.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/pyproject.toml` & `fancy_dataclass-0.4.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -58,29 +58,31 @@
   "cat docs/.changelog-version-regex.txt | xargs gadzooks check-version --check-tag --dist-dir dist --changelog docs/CHANGELOG.md --changelog-version-regex",
 ]
 
 [tool.hatch.envs.lint]
 dependencies = [
   "mypy>=1.0",
   "numpy",
-  "py-gadzooks>=0.2",
+  "py-gadzooks>=0.2.9",
   "pytest",
   "ruff>=0.3",
   "vermin>=1.5",
 ]
 
 [tool.hatch.envs.lint.scripts]
 # linting
 run-ruff = "ruff check"
 # ensure compatibility with Py3.8 and higher
 run-vermin = "vermin {args:.}"
 # type-checking
 run-mypy = "mypy --install-types --non-interactive {args:fancy_dataclass tests}"
 # print info about lines of code
 run-loc-summarize = "gadzooks loc-summarize fancy_dataclass"
+# print out formatter diffs
+run-format = "gadzooks check-format fancy_dataclass --formatter yapf --ignore-patterns '\\s*'"
 all = ["run-ruff", "run-vermin", "run-mypy", "run-loc-summarize"]
 
 [tool.hatch.envs.test]
 dependencies = [
     "numpy",
     "pytest",
     "pytest-cov",
@@ -158,7 +160,19 @@
 
 [[tool.mypy.overrides]]
 module = "tests.test_subprocess"
 disable_error_code = ["assignment", "misc"]
 
 [tool.pytest.ini_options]
 addopts = "--verbose --cov=fancy_dataclass"
+
+[tool.yapf]
+# NOTE: we'd like to disable vertical whitespace adjustment,
+# but there appears to be no way to do that
+based_on_style = "pep8"
+blank_lines_between_top_level_imports_and_variables = 2
+coalesce_brackets = true
+column_limit = 10000
+dedent_closing_brackets = true
+space_between_ending_comma_and_closing_bracket = false
+spaces_around_power_operator = true
+split_all_top_level_comma_separated_values = true
```

### Comparing `fancy_dataclass-0.4.4/docs/README.md` & `fancy_dataclass-0.4.5/docs/README.md`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.4/PKG-INFO` & `fancy_dataclass-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fancy-dataclass
-Version: 0.4.4
+Version: 0.4.5
 Summary: Spiff up your dataclasses with extra features.
 Project-URL: Documentation, https://fancy-dataclass.readthedocs.io
 Project-URL: Issues, https://github.com/jeremander/fancy-dataclass/issues
 Project-URL: Source, https://github.com/jeremander/fancy-dataclass
 Project-URL: Changelog, https://fancy-dataclass.readthedocs.io/en/stable/CHANGELOG
 Author-email: Jeremy Silver <jeremys@nessiness.com>
 License-Expression: MIT
```

