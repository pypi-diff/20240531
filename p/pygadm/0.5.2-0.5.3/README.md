# Comparing `tmp/pygadm-0.5.2.tar.gz` & `tmp/pygadm-0.5.3.tar.gz`

## Comparing `pygadm-0.5.2.tar` & `pygadm-0.5.3.tar`

### file list

```diff
@@ -1,60 +1,64 @@
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 pygadm-0.5.2/.copier-answers.yml
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pygadm-0.5.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 pygadm-0.5.2/.readthedocs.yaml
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 pygadm-0.5.2/CITATION.cff
--rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 pygadm-0.5.2/CODE_OF_CONDUCT.rst
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 pygadm-0.5.2/CONTRIBUTING.rst
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 pygadm-0.5.2/noxfile.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 pygadm-0.5.2/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 pygadm-0.5.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 pygadm-0.5.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 pygadm-0.5.2/.github/ISSUE_TEMPLATE/PULL_REQUEST_TEMPLATE/pr_template.md
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 pygadm-0.5.2/.github/workflows/pypackage_check.yaml
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pygadm-0.5.2/.github/workflows/release.yaml
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 pygadm-0.5.2/.github/workflows/unit.yaml
--rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 pygadm-0.5.2/docs/conf.py
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 pygadm-0.5.2/docs/index.rst
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pygadm-0.5.2/docs/setup.rst
--rw-r--r--   0        0        0     8782 2020-02-02 00:00:00.000000 pygadm-0.5.2/docs/usage.rst
--rw-r--r--   0        0        0     8382 2020-02-02 00:00:00.000000 pygadm-0.5.2/docs/_static/android-chrome-96x96.png
--rw-r--r--   0        0        0    15135 2020-02-02 00:00:00.000000 pygadm-0.5.2/docs/_static/apple-touch-icon.png
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 pygadm-0.5.2/docs/_static/browserconfig.xml
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 pygadm-0.5.2/docs/_static/custom.css
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 pygadm-0.5.2/docs/_static/favicon-16x16.png
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 pygadm-0.5.2/docs/_static/favicon-32x32.png
--rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 pygadm-0.5.2/docs/_static/favicon.ico
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 pygadm-0.5.2/docs/_static/logo.png
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 pygadm-0.5.2/docs/_static/mstile-150x150.png
--rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 pygadm-0.5.2/docs/_static/safari-pinned-tab.svg
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 pygadm-0.5.2/docs/_static/site.webmanifest
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 pygadm-0.5.2/docs/_template/pypackage-credit.html
--rw-r--r--   0        0        0    12786 2020-02-02 00:00:00.000000 pygadm-0.5.2/pygadm/__init__.py
--rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 pygadm-0.5.2/pygadm/bin/refresh_database.py
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 pygadm-0.5.2/pygadm/data/gadm_continent.json
--rw-r--r--   0        0        0  8715783 2020-02-02 00:00:00.000000 pygadm-0.5.2/pygadm/data/gadm_database.parquet
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pygadm-0.5.2/tests/__init__.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 pygadm-0.5.2/tests/check_warnings.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 pygadm-0.5.2/tests/test_continent.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 pygadm-0.5.2/tests/test_items.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 pygadm-0.5.2/tests/test_names.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygadm-0.5.2/tests/data/warning_list.txt
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 pygadm-0.5.2/tests/test_continent/test_continent.csv
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 pygadm-0.5.2/tests/test_items/test_area.csv
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 pygadm-0.5.2/tests/test_items/test_camelCase_names.yml
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pygadm-0.5.2/tests/test_items/test_duplication.yml
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 pygadm-0.5.2/tests/test_items/test_multiple_input.csv
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pygadm-0.5.2/tests/test_items/test_sub_content.csv
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 pygadm-0.5.2/tests/test_items/test_too_high.yml
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 pygadm-0.5.2/tests/test_items/test_too_low.yml
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pygadm-0.5.2/tests/test_names/test_area.csv
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 pygadm-0.5.2/tests/test_names/test_complete_content.csv
--rw-r--r--   0        0        0     4876 2020-02-02 00:00:00.000000 pygadm-0.5.2/tests/test_names/test_empty.csv
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 pygadm-0.5.2/tests/test_names/test_sub_content.csv
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pygadm-0.5.2/tests/test_names/test_too_high.csv
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pygadm-0.5.2/tests/test_names/test_too_low.csv
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 pygadm-0.5.2/.gitignore
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 pygadm-0.5.2/AUTHORS.rst
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pygadm-0.5.2/LICENSE
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 pygadm-0.5.2/README.rst
--rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 pygadm-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 pygadm-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 pygadm-0.5.3/.copier-answers.yml
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pygadm-0.5.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 pygadm-0.5.3/.readthedocs.yaml
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 pygadm-0.5.3/CITATION.cff
+-rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 pygadm-0.5.3/CODE_OF_CONDUCT.rst
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 pygadm-0.5.3/CONTRIBUTING.rst
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 pygadm-0.5.3/codecov.yml
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 pygadm-0.5.3/noxfile.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 pygadm-0.5.3/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 pygadm-0.5.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 pygadm-0.5.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 pygadm-0.5.3/.github/ISSUE_TEMPLATE/PULL_REQUEST_TEMPLATE/pr_template.md
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 pygadm-0.5.3/.github/workflows/pypackage_check.yaml
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 pygadm-0.5.3/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 pygadm-0.5.3/.github/workflows/unit.yaml
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 pygadm-0.5.3/docs/conf.py
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 pygadm-0.5.3/docs/index.rst
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pygadm-0.5.3/docs/setup.rst
+-rw-r--r--   0        0        0     8784 2020-02-02 00:00:00.000000 pygadm-0.5.3/docs/usage.rst
+-rw-r--r--   0        0        0     8382 2020-02-02 00:00:00.000000 pygadm-0.5.3/docs/_static/android-chrome-96x96.png
+-rw-r--r--   0        0        0    15135 2020-02-02 00:00:00.000000 pygadm-0.5.3/docs/_static/apple-touch-icon.png
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 pygadm-0.5.3/docs/_static/browserconfig.xml
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 pygadm-0.5.3/docs/_static/custom.css
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 pygadm-0.5.3/docs/_static/favicon-16x16.png
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 pygadm-0.5.3/docs/_static/favicon-32x32.png
+-rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 pygadm-0.5.3/docs/_static/favicon.ico
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 pygadm-0.5.3/docs/_static/logo.png
+-rw-r--r--   0        0        0    10960 2020-02-02 00:00:00.000000 pygadm-0.5.3/docs/_static/logo.svg
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 pygadm-0.5.3/docs/_static/mstile-150x150.png
+-rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 pygadm-0.5.3/docs/_static/safari-pinned-tab.svg
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 pygadm-0.5.3/docs/_static/site.webmanifest
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pygadm-0.5.3/docs/_template/pypackage-credit.html
+-rw-r--r--   0        0        0    12709 2020-02-02 00:00:00.000000 pygadm-0.5.3/pygadm/__init__.py
+-rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 pygadm-0.5.3/pygadm/bin/refresh_database.py
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 pygadm-0.5.3/pygadm/data/gadm_continent.json
+-rw-r--r--   0        0        0  8715783 2020-02-02 00:00:00.000000 pygadm-0.5.3/pygadm/data/gadm_database.parquet
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pygadm-0.5.3/tests/__init__.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 pygadm-0.5.3/tests/check_warnings.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 pygadm-0.5.3/tests/test_continent.py
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 pygadm-0.5.3/tests/test_items.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 pygadm-0.5.3/tests/test_names.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygadm-0.5.3/tests/data/warning_list.txt
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 pygadm-0.5.3/tests/test_continent/test_continent.csv
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 pygadm-0.5.3/tests/test_items/test_area.csv
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 pygadm-0.5.3/tests/test_items/test_camelCase_names.yml
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pygadm-0.5.3/tests/test_items/test_duplication.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 pygadm-0.5.3/tests/test_items/test_multi_word_name.csv
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 pygadm-0.5.3/tests/test_items/test_multiple_input.csv
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pygadm-0.5.3/tests/test_items/test_sub_admin.csv
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pygadm-0.5.3/tests/test_items/test_sub_content.csv
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 pygadm-0.5.3/tests/test_items/test_too_high.yml
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 pygadm-0.5.3/tests/test_items/test_too_low.yml
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pygadm-0.5.3/tests/test_names/test_area.csv
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 pygadm-0.5.3/tests/test_names/test_complete_content.csv
+-rw-r--r--   0        0        0     4876 2020-02-02 00:00:00.000000 pygadm-0.5.3/tests/test_names/test_empty.csv
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 pygadm-0.5.3/tests/test_names/test_sub_content.csv
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pygadm-0.5.3/tests/test_names/test_too_high.csv
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pygadm-0.5.3/tests/test_names/test_too_low.csv
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 pygadm-0.5.3/.gitignore
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 pygadm-0.5.3/AUTHORS.rst
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pygadm-0.5.3/LICENSE
+-rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 pygadm-0.5.3/README.rst
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 pygadm-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 pygadm-0.5.3/PKG-INFO
```

### Comparing `pygadm-0.5.2/.pre-commit-config.yaml` & `pygadm-0.5.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pygadm-0.5.2/CODE_OF_CONDUCT.rst` & `pygadm-0.5.3/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `pygadm-0.5.2/CONTRIBUTING.rst` & `pygadm-0.5.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pygadm-0.5.2/noxfile.py` & `pygadm-0.5.3/noxfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,26 @@
     """Apply the pre-commits."""
     session.install("pre-commit")
     session.run("pre-commit", "run", "--all-files", *session.posargs)
 
 
 @nox.session(reuse_venv=True)
 def test(session):
-    """Run all the test using the environment variable of the running machine."""
+    """Run the selected tests and report coverage in html."""
     session.install(".[test]")
     test_files = session.posargs or ["tests"]
-    session.run("pytest", "--color=yes", "--cov", "--cov-report=xml", *test_files)
+    session.run("pytest", "--color=yes", "--cov", "--cov-report=html", *test_files)
+
+
+@nox.session(reuse_venv=True, name="ci-test")
+def ci_test(session):
+    """Run all the test and report coverage in xml."""
+    session.install(".[test]")
+    session.posargs[0] if session.posargs else "default"
+    session.run("pytest", "--color=yes", "--cov", "--cov-report=xml")
 
 
 @nox.session(reuse_venv=True, name="dead-fixtures")
 def dead_fixtures(session):
     """Check for dead fixtures within the tests."""
     session.install(".[test]")
     session.run("pytest", "--dead-fixtures")
```

### Comparing `pygadm-0.5.2/.github/ISSUE_TEMPLATE/feature_request.md` & `pygadm-0.5.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pygadm-0.5.2/.github/workflows/pypackage_check.yaml` & `pygadm-0.5.3/.github/workflows/pypackage_check.yaml`

 * *Files identical despite different names*

### Comparing `pygadm-0.5.2/.github/workflows/unit.yaml` & `pygadm-0.5.3/.github/workflows/unit.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 name: Unit tests
 
 on:
+  workflow_call:
   push:
     branches:
       - main
   pull_request:
 
-env:
-  EARTHENGINE_TOKEN: ${{ secrets.EARTHENGINE_TOKEN }}
-
 jobs:
   lint:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
@@ -62,28 +60,32 @@
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install nox
         run: pip install nox
       - name: test with pytest
-        run: nox -s test
+        run: nox -s ci-test
+      - name: assess dead fixtures
+        if: ${{ matrix.python-version == '3.10' }}
+        shell: bash
+        run: nox -s dead-fixtures
+      - uses: actions/upload-artifact@v4
+        if: ${{ matrix.python-version == '3.10' }}
+        with:
+          name: coverage
+          path: coverage.xml
 
   coverage:
     needs: [build]
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/download-artifact@v4
         with:
-          python-version: "3.10"
-      - name: Install deps
-        run: pip install nox
-      - name: test with pytest
-        run: nox -s test
-      - name: assess dead fixtures
-        run: nox -s dead-fixtures
+          name: coverage
+          path: coverage.xml
       - name: codecov
         uses: codecov/codecov-action@v3
         with:
+          file: ./coverage.xml
           token: ${{ secrets.CODECOV_TOKEN }}
           verbose: true
```

### Comparing `pygadm-0.5.2/docs/index.rst` & `pygadm-0.5.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pygadm-0.5.2/docs/setup.rst` & `pygadm-0.5.3/docs/setup.rst`

 * *Files identical despite different names*

### Comparing `pygadm-0.5.2/docs/usage.rst` & `pygadm-0.5.3/docs/usage.rst`

 * *Files 2% similar despite different names*

```diff
@@ -184,15 +184,15 @@
 
 .. code-block:: console
 
     EEException: Request payload size exceeds the limit: 10485760 bytes.
 
 Use the :code:`simplify` method from GeoPandas (more information `here <https://geopandas.org/en/stable/docs/reference/api/geopandas.GeoSeries.simplify.html>`__) to downscale the resolution of the geometries. The following example is needed if you want to work with France:
 
-.. jupyter-execute::
+.. code-block:: python
 
     import pygadm
     import geemap
     import ee
     from ipyleaflet import ZoomControl
 
     ee.Initialize()
```

### Comparing `pygadm-0.5.2/docs/_static/android-chrome-96x96.png` & `pygadm-0.5.3/docs/_static/android-chrome-96x96.png`

 * *Files identical despite different names*

### Comparing `pygadm-0.5.2/docs/_static/apple-touch-icon.png` & `pygadm-0.5.3/docs/_static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `pygadm-0.5.2/docs/_static/favicon-16x16.png` & `pygadm-0.5.3/docs/_static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `pygadm-0.5.2/docs/_static/favicon-32x32.png` & `pygadm-0.5.3/docs/_static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `pygadm-0.5.2/docs/_static/favicon.ico` & `pygadm-0.5.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `pygadm-0.5.2/docs/_static/logo.png` & `pygadm-0.5.3/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `pygadm-0.5.2/docs/_static/mstile-150x150.png` & `pygadm-0.5.3/docs/_static/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `pygadm-0.5.2/docs/_static/safari-pinned-tab.svg` & `pygadm-0.5.3/docs/_static/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `pygadm-0.5.2/pygadm/__init__.py` & `pygadm-0.5.3/pygadm/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import numpy as np
 import pandas as pd
 from deprecated.sphinx import deprecated, versionadded
 from requests_cache import CachedSession
 
 session = CachedSession("pygadm", use_temp=True)
 
-__version__ = "0.5.2"
+__version__ = "0.5.3"
 __author__ = "Pierrick Rambaud"
 __email__ = "pierrick.rambaud49@gmail.com"
 
 __gadm_version__ = "410"  # 4.1
 __gadm_url__ = "https://geodata.ucdavis.edu/gadm/gadm4.1/json/gadm41_{}_{}.json"
 __gadm_data__ = Path(__file__).parent / "data" / "gadm_database.parquet"
 __gadm_continent__ = json.loads(
@@ -78,17 +78,15 @@
                 df.filter([column.format(i) for i in range(6)])
                 .apply(lambda col: col.str.lower())
                 .isin([id.lower()])
             )
 
             if not is_in.any().any():
                 # find the 5 closest names/id
-                columns = [
-                    df[column.format(i)].dropna().str.lower().values for i in range(6)
-                ]
+                columns = [df[column.format(i)].dropna().str.lower().values for i in range(6)]
                 ids = np.unique(np.concatenate(columns))
                 close_ids = get_close_matches(id.lower(), ids, n=5)
                 if is_name is True:
                     close_ids = [i.capitalize() for i in close_ids]
                 else:
                     close_ids = [i.upper() for i in close_ids]
                 raise ValueError(
@@ -98,17 +96,15 @@
 
             # Get the iso_3 of the associated country of the identifed area and the associated level
             line = is_in[~((~is_in).all(axis=1))].idxmax(1)
             level = line.iloc[0][5 if is_name else 4]  # GID_ or NAME_
 
             # load the max_level available in the requested area
             sub_df = df[df[column.format(level)].str.fullmatch(id, case=False)]
-            max_level = next(
-                i for i in reversed(range(6)) if (sub_df[f"GID_{i}"] != "").any()
-            )
+            max_level = next(i for i in reversed(range(6)) if (sub_df[f"GID_{i}"] != "").any())
 
             # get the request level from user
             content_level, level = int(content_level), int(level)
             if content_level == -1:
                 content_level = level
             elif content_level < level:
                 warnings.warn(
@@ -181,17 +177,15 @@
         gdf_list = [self._items(n, a, content_level) for a, n in product(admins, names)]
 
         # avoid concat if not needed for speed boost
         gdf = gdf_list[0] if len(gdf_list) == 1 else pd.concat(gdf_list)
 
         super().__init__(gdf)
 
-    def _items(
-        self, name: str = "", admin: str = "", content_level: int = -1
-    ) -> gpd.GeoDataFrame:
+    def _items(self, name: str = "", admin: str = "", content_level: int = -1) -> gpd.GeoDataFrame:
         """
         Return the requested administrative boundaries from the single name or administrative code.
 
         Args:
             name: The name of an administrative area. Cannot be set along with :code:`admin`.
             admin: The id of an administrative area in the GADM nomenclature. Cannot be set along with :code:`name`.
             content_level: The level to use in the final dataset. Default to -1 (use level from the area).
@@ -232,24 +226,25 @@
                 f"Try to manually open the following link: {url}. "
                 "If it doesn't work, the error is coming from GADM servers. "
                 "If it works please open an issue on our repository: https://github.com/12rambau/pygadm/issues."
             )
 
         level_gdf = gpd.GeoDataFrame.from_features(data)
         level_gdf.rename(columns={"COUNTRY": "NAME_0"}, inplace=True)
-        gdf = level_gdf[level_gdf[column.format(level)].str.fullmatch(id, case=False)]
 
         # workaround for the wrong naming convention in the geojson files
         # https://gis.stackexchange.com/questions/467848/how-to-get-back-spaces-in-administrative-names-in-gadm-4-1
         # it should disappear in the next version of GADM
         # we are forced to retrieve all the names from the df (sourced from.gpkg) to replace the one from
         # the geojson that are all in camelCase
-        complete_df = Names(name, admin, content_level=content_level, complete=True)
+        complete_df = Names(admin=iso_3, content_level=content_level, complete=True)
         for i in range(int(content_level) + 1):
-            gdf.loc[:, (f"NAME_{i}")] = complete_df[f"NAME_{i}"].values
+            level_gdf.loc[:, f"NAME_{i}"] = complete_df[f"NAME_{i}"].values
+
+        gdf = level_gdf[level_gdf[column.format(level)].str.fullmatch(id, case=False)]
 
         return gdf
 
 
 @deprecated(version="0.5.2", reason="Use the Names class instead.")
 class AdmNames(Names):
     pass
```

### Comparing `pygadm-0.5.2/pygadm/bin/refresh_database.py` & `pygadm-0.5.3/pygadm/bin/refresh_database.py`

 * *Files identical despite different names*

### Comparing `pygadm-0.5.2/pygadm/data/gadm_continent.json` & `pygadm-0.5.3/pygadm/data/gadm_continent.json`

 * *Files identical despite different names*

### Comparing `pygadm-0.5.2/pygadm/data/gadm_database.parquet` & `pygadm-0.5.3/pygadm/data/gadm_database.parquet`

 * *Files identical despite different names*

### Comparing `pygadm-0.5.2/tests/check_warnings.py` & `pygadm-0.5.3/tests/check_warnings.py`

 * *Files identical despite different names*

### Comparing `pygadm-0.5.2/tests/test_continent.py` & `pygadm-0.5.3/tests/test_continent.py`

 * *Files identical despite different names*

### Comparing `pygadm-0.5.2/tests/test_items.py` & `pygadm-0.5.3/tests/test_items.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,14 +44,20 @@
 def test_too_high(data_regression):
     """Request a sublevel higher than available in the area."""
     with pytest.warns(UserWarning):
         gdf = pygadm.Items(admin="SGP.1_1", content_level=0)
         data_regression.check(gdf.GID_1.tolist())
 
 
+def test_multi_word_name(dataframe_regression):
+    """Request a multi-word area."""
+    gdf = pygadm.Items(name="United States")
+    dataframe_regression.check(gdf[["NAME_0", "GID_0"]])
+
+
 def test_too_low(data_regression):
     """Request a sublevel lower than available in the area."""
     # request a level too low
     with pytest.warns(UserWarning):
         gdf = pygadm.Items(admin="SGP.1_1", content_level=3)
         data_regression.check(gdf.GID_1.tolist())
 
@@ -105,7 +111,13 @@
 def test_adm_items():
     """Test the AdmItems class."""
     gdf1 = pygadm.Items(name="Singapore")
 
     with pytest.warns(DeprecationWarning):
         gdf2 = pygadm.AdmItems(name="Singapore")
         assert gdf1.equals(gdf2)
+
+
+def test_sub_admin(dataframe_regression):
+    """Request a sublevel."""
+    gdf = pygadm.Items(admin="SGP.1_1")
+    dataframe_regression.check(gdf[["GID_1", "NAME_1", "GID_0", "NAME_0"]])
```

### Comparing `pygadm-0.5.2/tests/test_names.py` & `pygadm-0.5.3/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `pygadm-0.5.2/tests/test_items/test_camelCase_names.yml` & `pygadm-0.5.3/tests/test_items/test_camelCase_names.yml`

 * *Files identical despite different names*

### Comparing `pygadm-0.5.2/tests/test_names/test_empty.csv` & `pygadm-0.5.3/tests/test_names/test_empty.csv`

 * *Files identical despite different names*

### Comparing `pygadm-0.5.2/.gitignore` & `pygadm-0.5.3/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -130,8 +130,11 @@
 # Pyre type checker
 .pyre/
 
 # system IDE
 .vscode/
 
 # image tmp file
-*Zone.Identifier
+*Zone.Identifier
+
+# debugging notebooks
+test.ipynb
```

### Comparing `pygadm-0.5.2/AUTHORS.rst` & `pygadm-0.5.3/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pygadm-0.5.2/LICENSE` & `pygadm-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pygadm-0.5.2/README.rst` & `pygadm-0.5.3/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,38 @@
-
-pyGADM
+PyGADM
 ======
 
-.. image:: https://img.shields.io/badge/License-MIT-yellow.svg?logo=opensourceinitiative&logoColor=white
+.. image:: https://img.shields.io/badge/License-MIT-yellow?logo=opensourceinitiative&logoColor=white
     :target: LICENSE
     :alt: License: MIT
 
-.. image:: https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg?logo=git&logoColor=white
+.. image:: https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow?logo=git&logoColor=white
    :target: https://conventionalcommits.org
    :alt: conventional commit
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+.. image:: https://img.shields.io/badge/code%20style-black-000000?logo=ford&logoColor=white
    :target: https://github.com/psf/black
    :alt: Black badge
 
-.. image:: https://img.shields.io/badge/code_style-prettier-ff69b4.svg?logo=prettier&logoColor=white
+.. image:: https://img.shields.io/badge/code_style-prettier-ff69b4?logo=prettier&logoColor=white
    :target: https://github.com/prettier/prettier
    :alt: prettier badge
 
 .. image:: https://img.shields.io/badge/pre--commit-active-yellow?logo=pre-commit&logoColor=white
     :target: https://pre-commit.com/
     :alt: pre-commit
 
-.. image:: https://img.shields.io/pypi/v/pygadm?color=blue&logo=pypi&logoColor=white
+.. image:: https://img.shields.io/pypi/v/pygadm?color=blue&logo=python&logoColor=white
     :target: https://pypi.org/project/pygadm/
     :alt: PyPI version
 
+.. image:: https://img.shields.io/conda/vn/conda-forge/pygadm?color=blue&logo=anaconda&logoColor=white
+    :target: https://anaconda.org/conda-forge/pygadm
+    :alt: Conda Version
+
 .. image:: https://img.shields.io/github/actions/workflow/status/12rambau/pygadm/unit.yaml?logo=github&logoColor=white
     :target: https://github.com/12rambau/pygadm/actions/workflows/unit.yaml
     :alt: build
 
 .. image:: https://img.shields.io/codecov/c/github/12rambau/pygadm?logo=codecov&logoColor=white
     :target: https://codecov.io/gh/12rambau/pygadm
     :alt: Test Coverage
@@ -37,14 +40,18 @@
 .. image:: https://img.shields.io/readthedocs/pygadm?logo=readthedocs&logoColor=white
     :target: https://pygadm.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 Overview
 --------
 
+.. image:: docs/_static/logo.svg
+    :width: 20%
+    :align: right
+
 Easy access to administrative boundary defined by GADM from a Python scripts.
 
 This lib provides access to GADM datasets from a Python script without downloading the file from their server. We provide access to The current version (4.1.) which delimits 400,276 administrative areas.
 
 The data are freely available for academic use and other non-commercial use. Redistribution, or commercial use is not allowed without prior permission. See the `license <https://gadm.org/license.html>`__ of the GADM project for more details.
 
 .. note::
@@ -64,8 +71,8 @@
    import pygadm
 
    gdf = pygadm.AdmItems(name="Singapore", content_level=1)
 
 Credits
 -------
 
-This package was created with `Copier <https://copier.readthedocs.io/en/latest/>`__ and the `@12rambau/pypackage <https://github.com/12rambau/pypackage>`__ 0.1.5 project template .
+This package was created with `Copier <https://copier.readthedocs.io/en/latest/>`__ and the `@12rambau/pypackage <https://github.com/12rambau/pypackage>`__ 0.1.11 project template.
```

### Comparing `pygadm-0.5.2/pyproject.toml` & `pygadm-0.5.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pygadm"
-version = "0.5.2"
+version = "0.5.3"
 description = "Easy access to administrative boundary defined by GADM from Python scripts"
 keywords = [
   "Python"
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -24,15 +24,15 @@
   "geopandas",
   "pyarrow",
   "requests-cache"
 ]
 
 [[project.authors]]
 name = "Pierrick Rambaud"
-email = "pierrick.rambaud49@gmai.com"
+email = "pierrick.rambaud49@gmail.com"
 
 [project.license]
 text = "MIT"
 
 [project.readme]
 file = "README.rst"
 content-type = "text/x-rst"
@@ -73,24 +73,27 @@
   "nox"
 ]
 post-install-commands = ["pre-commit install"]
 
 [tool.commitizen]
 tag_format = "v$major.$minor.$patch$prerelease"
 update_changelog_on_bump = false
-version = "0.5.2"
+version = "0.5.3"
 version_files = [
     "pyproject.toml:version",
     "pygadm/__init__.py:__version__",
     "CITATION.cff:version"
 ]
 
 [tool.pytest.ini_options]
 testpaths = "tests"
 
+[tool.black]
+line-length = 100
+
 [tool.ruff]
 ignore-init-module-imports = true
 fix = true
 select = ["E", "F", "W", "I", "D", "RUF"]
 ignore = [
   "E501",  # line too long | Black take care of it
     "W605",  # invalid escape sequence | we escape specific characters for sphinx
```

### Comparing `pygadm-0.5.2/PKG-INFO` & `pygadm-0.5.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pygadm
-Version: 0.5.2
+Version: 0.5.3
 Summary: Easy access to administrative boundary defined by GADM from Python scripts
 Project-URL: Homepage, https://github.com/12rambau/pygadm
-Author-email: Pierrick Rambaud <pierrick.rambaud49@gmai.com>
+Author-email: Pierrick Rambaud <pierrick.rambaud49@gmail.com>
 License: MIT
 License-File: AUTHORS.rst
 License-File: LICENSE
 Keywords: Python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -36,42 +36,45 @@
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest-deadfixtures; extra == 'test'
 Requires-Dist: pytest-regressions>=2.4.3; extra == 'test'
 Requires-Dist: pytest-sugar; extra == 'test'
 Description-Content-Type: text/x-rst
 
-
-pyGADM
+PyGADM
 ======
 
-.. image:: https://img.shields.io/badge/License-MIT-yellow.svg?logo=opensourceinitiative&logoColor=white
+.. image:: https://img.shields.io/badge/License-MIT-yellow?logo=opensourceinitiative&logoColor=white
     :target: LICENSE
     :alt: License: MIT
 
-.. image:: https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg?logo=git&logoColor=white
+.. image:: https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow?logo=git&logoColor=white
    :target: https://conventionalcommits.org
    :alt: conventional commit
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+.. image:: https://img.shields.io/badge/code%20style-black-000000?logo=ford&logoColor=white
    :target: https://github.com/psf/black
    :alt: Black badge
 
-.. image:: https://img.shields.io/badge/code_style-prettier-ff69b4.svg?logo=prettier&logoColor=white
+.. image:: https://img.shields.io/badge/code_style-prettier-ff69b4?logo=prettier&logoColor=white
    :target: https://github.com/prettier/prettier
    :alt: prettier badge
 
 .. image:: https://img.shields.io/badge/pre--commit-active-yellow?logo=pre-commit&logoColor=white
     :target: https://pre-commit.com/
     :alt: pre-commit
 
-.. image:: https://img.shields.io/pypi/v/pygadm?color=blue&logo=pypi&logoColor=white
+.. image:: https://img.shields.io/pypi/v/pygadm?color=blue&logo=python&logoColor=white
     :target: https://pypi.org/project/pygadm/
     :alt: PyPI version
 
+.. image:: https://img.shields.io/conda/vn/conda-forge/pygadm?color=blue&logo=anaconda&logoColor=white
+    :target: https://anaconda.org/conda-forge/pygadm
+    :alt: Conda Version
+
 .. image:: https://img.shields.io/github/actions/workflow/status/12rambau/pygadm/unit.yaml?logo=github&logoColor=white
     :target: https://github.com/12rambau/pygadm/actions/workflows/unit.yaml
     :alt: build
 
 .. image:: https://img.shields.io/codecov/c/github/12rambau/pygadm?logo=codecov&logoColor=white
     :target: https://codecov.io/gh/12rambau/pygadm
     :alt: Test Coverage
@@ -79,14 +82,18 @@
 .. image:: https://img.shields.io/readthedocs/pygadm?logo=readthedocs&logoColor=white
     :target: https://pygadm.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 Overview
 --------
 
+.. image:: docs/_static/logo.svg
+    :width: 20%
+    :align: right
+
 Easy access to administrative boundary defined by GADM from a Python scripts.
 
 This lib provides access to GADM datasets from a Python script without downloading the file from their server. We provide access to The current version (4.1.) which delimits 400,276 administrative areas.
 
 The data are freely available for academic use and other non-commercial use. Redistribution, or commercial use is not allowed without prior permission. See the `license <https://gadm.org/license.html>`__ of the GADM project for more details.
 
 .. note::
@@ -106,8 +113,8 @@
    import pygadm
 
    gdf = pygadm.AdmItems(name="Singapore", content_level=1)
 
 Credits
 -------
 
-This package was created with `Copier <https://copier.readthedocs.io/en/latest/>`__ and the `@12rambau/pypackage <https://github.com/12rambau/pypackage>`__ 0.1.5 project template .
+This package was created with `Copier <https://copier.readthedocs.io/en/latest/>`__ and the `@12rambau/pypackage <https://github.com/12rambau/pypackage>`__ 0.1.11 project template.
```

