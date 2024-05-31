# Comparing `tmp/impactlab_tools-0.5.0.tar.gz` & `tmp/impactlab_tools-0.6.0.tar.gz`

## Comparing `impactlab_tools-0.5.0.tar` & `impactlab_tools-0.6.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/.readthedocs.yaml
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/CONTRIBUTING.rst
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/requirements.txt
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/whatsnew.rst
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/.github/dependabot.yml
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/.github/workflows/python-publish.yaml
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/.github/workflows/pythonpackage.yaml
--rw-r--r--   0        0        0     6765 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/docs/Makefile
--rw-r--r--   0        0        0     9577 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/docs/conf.py
--rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/docs/configuration.rst
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/docs/contributing.rst
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/docs/impactlab_tools.acp.rst
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/docs/impactlab_tools.gcp.rst
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/docs/impactlab_tools.rst
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/docs/impactlab_tools.utils.rst
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/docs/index.rst
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/docs/make.bat
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/docs/readme.rst
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/docs/whatsnew.rst
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/src/impactlab_tools/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/src/impactlab_tools/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/src/impactlab_tools/acp/__init__.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/src/impactlab_tools/acp/aggregate.py
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/src/impactlab_tools/acp/dist.py
--rw-r--r--   0        0        0   312203 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/src/impactlab_tools/assets/ACP_county_census_pop.nc
--rw-r--r--   0        0        0  1055639 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/src/impactlab_tools/assets/GCP_impact_regions.nc
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/src/impactlab_tools/assets/__init__.py
--rwxr-xr-x   0        0        0  4412579 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/src/impactlab_tools/assets/hierid_regions.dbf
--rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/src/impactlab_tools/assets/hierid_regions.prj
--rwxr-xr-x   0        0        0 12901012 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/src/impactlab_tools/assets/hierid_regions.shp
--rwxr-xr-x   0        0        0   195124 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/src/impactlab_tools/assets/hierid_regions.shx
--rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/src/impactlab_tools/assets/weights_acp.csv
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/src/impactlab_tools/assets/weights_gcp.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/src/impactlab_tools/gcp/__init__.py
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/src/impactlab_tools/gcp/dist.py
--rw-r--r--   0        0        0     4998 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/src/impactlab_tools/gcp/reindex.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/src/impactlab_tools/utils/__init__.py
--rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/src/impactlab_tools/utils/binning.py
--rw-r--r--   0        0        0     9396 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/src/impactlab_tools/utils/configdict.py
--rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/src/impactlab_tools/utils/files.py
--rw-r--r--   0        0        0     7760 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/src/impactlab_tools/utils/paralog.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/src/impactlab_tools/utils/spatial.py
--rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/src/impactlab_tools/utils/versions.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/src/impactlab_tools/utils/visualize.py
--rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/src/impactlab_tools/utils/weighting.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/tests/test_deployment.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/tests/gcp/test_gcp_dist.py
--rw-r--r--   0        0        0     4745 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/tests/utils/test_configdict.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/tests/utils/test_files.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/tests/utils/test_paralog.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/tests/utils/test_weighting.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/LICENSE
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/README.rst
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 impactlab_tools-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/requirements.txt
+-rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/whatsnew.rst
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/.github/workflows/python-publish.yaml
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/.github/workflows/pythonpackage.yaml
+-rw-r--r--   0        0        0     6765 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/docs/Makefile
+-rw-r--r--   0        0        0     9577 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/docs/conf.py
+-rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/docs/configuration.rst
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/docs/contributing.rst
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/docs/impactlab_tools.acp.rst
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/docs/impactlab_tools.gcp.rst
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/docs/impactlab_tools.rst
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/docs/impactlab_tools.utils.rst
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/docs/index.rst
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/docs/make.bat
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/docs/readme.rst
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/docs/whatsnew.rst
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/src/impactlab_tools/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/src/impactlab_tools/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/src/impactlab_tools/acp/__init__.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/src/impactlab_tools/acp/aggregate.py
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/src/impactlab_tools/acp/dist.py
+-rw-r--r--   0        0        0   312203 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/src/impactlab_tools/assets/ACP_county_census_pop.nc
+-rw-r--r--   0        0        0  1055639 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/src/impactlab_tools/assets/GCP_impact_regions.nc
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/src/impactlab_tools/assets/__init__.py
+-rwxr-xr-x   0        0        0  4412579 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/src/impactlab_tools/assets/hierid_regions.dbf
+-rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/src/impactlab_tools/assets/hierid_regions.prj
+-rwxr-xr-x   0        0        0 12901012 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/src/impactlab_tools/assets/hierid_regions.shp
+-rwxr-xr-x   0        0        0   195124 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/src/impactlab_tools/assets/hierid_regions.shx
+-rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/src/impactlab_tools/assets/weights_acp.csv
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/src/impactlab_tools/assets/weights_gcp.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/src/impactlab_tools/gcp/__init__.py
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/src/impactlab_tools/gcp/dist.py
+-rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/src/impactlab_tools/gcp/reindex.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/src/impactlab_tools/utils/__init__.py
+-rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/src/impactlab_tools/utils/binning.py
+-rw-r--r--   0        0        0     9396 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/src/impactlab_tools/utils/configdict.py
+-rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/src/impactlab_tools/utils/files.py
+-rw-r--r--   0        0        0     7754 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/src/impactlab_tools/utils/paralog.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/src/impactlab_tools/utils/spatial.py
+-rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/src/impactlab_tools/utils/versions.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/src/impactlab_tools/utils/visualize.py
+-rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/src/impactlab_tools/utils/weighting.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/tests/test_deployment.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/tests/gcp/test_gcp_dist.py
+-rw-r--r--   0        0        0     4745 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/tests/utils/test_configdict.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/tests/utils/test_files.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/tests/utils/test_paralog.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/tests/utils/test_weighting.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/README.rst
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 impactlab_tools-0.6.0/PKG-INFO
```

### Comparing `impactlab_tools-0.5.0/.readthedocs.yaml` & `impactlab_tools-0.6.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/CONTRIBUTING.rst` & `impactlab_tools-0.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/whatsnew.rst` & `impactlab_tools-0.6.0/whatsnew.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,29 @@
 What's New
 ==========
 
 These are new features and improvements of note in each release.
 
+v0.6.0 (May 31, 2024)
+---------------------
+
+ - Drop unused ``h5netcdf`` dependency. Make ``matplotlib``, ``geopandas`` optional dependencies.
+
+ - Add new extras for optional dependencies: ``impactlab-tools[viz]``, ``impactlab-tools[complete]``.
+
+ - Minor code cleanup, style update.
+
+ - Update ruff lint section format in pyproject.toml
+
+ - Minor update to docstr examples to match xarray > 2023.12.0.
+
 v0.5.0 (August 23, 2023)
 ------------------------
 
- - Drop Python 2 support. Requires Python >= v3.7.
+ - Drop Python 2 support. Require Python >= v3.7.
 
  - General documentation build update. Update to readthedocs v2 configuration.
 
  - Update package dependencies. Require previously unlisted dependencies: ``h5netcdf``, ``geopandas``, ``matplotlib``, ``numpy``, ``pandas``, ``scipy``, ``xarray``.
 
  - Fix error from bad coordinate assignment in ``impactlab_tools.gcp.reindex.hierid_to_shapenum()``.
```

### Comparing `impactlab_tools-0.5.0/.github/dependabot.yml` & `impactlab_tools-0.6.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/.github/workflows/python-publish.yaml` & `impactlab_tools-0.6.0/.github/workflows/python-publish.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.x"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install build
       - name: Build package
         run: python -m build
       - name: Publish package
-        uses: pypa/gh-action-pypi-publish@v1.8.8
+        uses: pypa/gh-action-pypi-publish@v1.8.14
```

### Comparing `impactlab_tools-0.5.0/.github/workflows/pythonpackage.yaml` & `impactlab_tools-0.6.0/.github/workflows/pythonpackage.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -18,17 +18,17 @@
     strategy:
       matrix:
         python-version: ["3.x"]
     defaults:
       run:
         shell: bash
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
           cache: 'pip'
           cache-dependency-path: 'requirements.txt'
       - name: Install dependencies
         run: |
           pip install -r requirements.txt
@@ -41,26 +41,27 @@
     strategy:
       matrix:
         python-version: ["3.x"]
     defaults:
       run:
         shell: bash
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
           cache: 'pip'
           cache-dependency-path: 'requirements.txt'
       - name: Install dependencies
         run: |
           pip install -r requirements.txt
       - name: Install package
         run: |
           pip install . --no-deps
       - name: Test with pytest
         run: |
           pytest -v --cov-report term-missing --cov-report xml
       - name: Upload coverage to Codecov
-        uses: codecov/codecov-action@v3
-        
+        uses: codecov/codecov-action@v4
+        env:
+          CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `impactlab_tools-0.5.0/docs/Makefile` & `impactlab_tools-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/docs/conf.py` & `impactlab_tools-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/docs/configuration.rst` & `impactlab_tools-0.6.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/docs/impactlab_tools.acp.rst` & `impactlab_tools-0.6.0/docs/impactlab_tools.acp.rst`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/docs/impactlab_tools.gcp.rst` & `impactlab_tools-0.6.0/docs/impactlab_tools.gcp.rst`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/docs/impactlab_tools.utils.rst` & `impactlab_tools-0.6.0/docs/impactlab_tools.utils.rst`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/docs/index.rst` & `impactlab_tools-0.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/docs/make.bat` & `impactlab_tools-0.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/src/impactlab_tools/acp/aggregate.py` & `impactlab_tools-0.6.0/src/impactlab_tools/acp/aggregate.py`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/src/impactlab_tools/acp/dist.py` & `impactlab_tools-0.6.0/src/impactlab_tools/acp/dist.py`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/src/impactlab_tools/assets/ACP_county_census_pop.nc` & `impactlab_tools-0.6.0/src/impactlab_tools/assets/ACP_county_census_pop.nc`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/src/impactlab_tools/assets/GCP_impact_regions.nc` & `impactlab_tools-0.6.0/src/impactlab_tools/assets/GCP_impact_regions.nc`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/src/impactlab_tools/assets/hierid_regions.dbf` & `impactlab_tools-0.6.0/src/impactlab_tools/assets/hierid_regions.dbf`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/src/impactlab_tools/assets/hierid_regions.shp` & `impactlab_tools-0.6.0/src/impactlab_tools/assets/hierid_regions.shp`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/src/impactlab_tools/assets/hierid_regions.shx` & `impactlab_tools-0.6.0/src/impactlab_tools/assets/hierid_regions.shx`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/src/impactlab_tools/assets/weights_acp.csv` & `impactlab_tools-0.6.0/src/impactlab_tools/assets/weights_acp.csv`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/src/impactlab_tools/assets/weights_gcp.csv` & `impactlab_tools-0.6.0/src/impactlab_tools/assets/weights_gcp.csv`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/src/impactlab_tools/gcp/dist.py` & `impactlab_tools-0.6.0/src/impactlab_tools/gcp/dist.py`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/src/impactlab_tools/gcp/reindex.py` & `impactlab_tools-0.6.0/src/impactlab_tools/gcp/reindex.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,20 +66,20 @@
         >>> ds = xr.Dataset({'var1': xr.DataArray(
         ...     np.random.random((24378,)),
         ...     dims=('SHAPENUM',),
         ...     coords={'SHAPENUM': np.arange(1,24379)})})
         ...
         >>> reshaped = shapenum_to_hierid(ds)
         >>> reshaped # doctest: +ELLIPSIS
-        <xarray.Dataset>
+        <xarray.Dataset> Size: 4MB
         Dimensions:  (hierid: 24378)
         Coordinates:
-          * hierid   (hierid) ...
+          * hierid   (hierid) <U35 3MB 'CAN.1.2.28' 'CAN.1.17.403' ... 'BWA.4.13'
         Data variables:
-            var1     (hierid) float64 0.417 0.7203 0.0001144 ...
+            var1     (hierid) float64 195kB 0.417 0.7203 0.0001144 ... 0.1359 0.9259
 
         >>> (reshaped.var1.values == ds.var1.values).all()
         True
 
     '''
     mapping = _get_impactregion_mapping()
 
@@ -147,20 +147,20 @@
         ...          'AFG.1.R91a8634efe8e02a7', 'AFG.1.Ra6a2bba0a271cb4a',
         ...          'AFG.1.Rcf29900a4c191e96', 'AFG.1.Rd0d6327d56611fba',
         ...          'AFG.10.103', 'AFG.10.106', 'AFG.10.109']})})
         ...
         ...
         >>> reshaped = hierid_to_shapenum(ds)
         >>> reshaped
-        <xarray.Dataset>
+        <xarray.Dataset> Size: 160B
         Dimensions:   (SHAPENUM: 10)
         Coordinates:
-          * SHAPENUM  (SHAPENUM) float64 1.369e+03 5.747e+03 ...
+          * SHAPENUM  (SHAPENUM) float64 80B 1.369e+03 5.747e+03 ... 5.812e+03 5.832e+03
         Data variables:
-            var2      (SHAPENUM) float64 0.417 0.7203 0.0001144 ...
+            var2      (SHAPENUM) float64 80B 0.417 0.7203 0.0001144 ... 0.3968 0.5388
 
         >>> (reshaped.var2.values == ds.var2.values).all()
         True
 
     '''
     mapping = _get_impactregion_mapping()
     mapping["hierid"] = mapping["hierid"].astype(unicode)
```

### Comparing `impactlab_tools-0.5.0/src/impactlab_tools/utils/binning.py` & `impactlab_tools-0.6.0/src/impactlab_tools/utils/binning.py`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/src/impactlab_tools/utils/configdict.py` & `impactlab_tools-0.6.0/src/impactlab_tools/utils/configdict.py`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/src/impactlab_tools/utils/files.py` & `impactlab_tools-0.6.0/src/impactlab_tools/utils/files.py`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/src/impactlab_tools/utils/paralog.py` & `impactlab_tools-0.6.0/src/impactlab_tools/utils/paralog.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,30 +117,30 @@
         """Provide additional status information."""
         status_path = StatusManager.claiming_filepath(dirpath, self.jobname)
         try:
             with open(status_path, 'a') as fp:
                 fp.write(status + '\n')
         except Exception:
             print("CAUGHT A WILD EXCEPTION BUT IGNORING IT WITHOUT LOGGING IT!")
-            print("Warning: Could write status update %s" % status)
+            print(f"Warning: Could write status update {status}")
 
     def release(self, dirpath, status):
         """Release the claim on this directory."""
         try:
             os.remove(StatusManager.claiming_filepath(dirpath, self.jobname))
         except Exception:
             print("CAUGHT A WILD EXCEPTION BUT IGNORING IT WITHOUT LOGGING IT!")
             print("Warning: Could not release directory.")
 
         try:
             with open(StatusManager.globalstatus_filepath(dirpath), 'a') as fp:
                 fp.write(f"{time.asctime()} {self.jobtitle}: {status}\n")
         except Exception:
             print("CAUGHT A WILD EXCEPTION BUT IGNORING IT WITHOUT LOGGING IT!")
-            print("Warning: Could write release status %s" % status)
+            print(f"Warning: Could write release status {status}")
 
     def is_claimed(self, dirname):
         """Check if a directory has claims from any of our jobs."""
         if not os.path.exists(dirname):
             return False
 
         for jobname in [self.jobname] + self.exclusive_jobnames:
@@ -168,15 +168,15 @@
     def globalstatus_filepath(dirpath):
         """The path to the global status for the directory."""
         return StatusManager.claiming_filepath(dirpath, 'global')
 
     @staticmethod
     def claiming_filepath(dirpath, jobname):
         """Return the path to the status file used for claiming a directory."""
-        return os.path.join(dirpath, "status-%s.txt" % jobname)
+        return os.path.join(dirpath, f"status-{jobname}.txt")
 
     @staticmethod
     def kill_active(dirpath, jobname):
         """Kill any job claiming this directory."""
         filepath = StatusManager.claiming_filepath(dirpath, jobname)
 
         if not os.path.exists(filepath):
```

### Comparing `impactlab_tools-0.5.0/src/impactlab_tools/utils/spatial.py` & `impactlab_tools-0.6.0/src/impactlab_tools/utils/spatial.py`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/src/impactlab_tools/utils/versions.py` & `impactlab_tools-0.6.0/src/impactlab_tools/utils/versions.py`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/src/impactlab_tools/utils/visualize.py` & `impactlab_tools-0.6.0/src/impactlab_tools/utils/visualize.py`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/src/impactlab_tools/utils/weighting.py` & `impactlab_tools-0.6.0/src/impactlab_tools/utils/weighting.py`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/tests/gcp/test_gcp_dist.py` & `impactlab_tools-0.6.0/tests/gcp/test_gcp_dist.py`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/tests/utils/test_configdict.py` & `impactlab_tools-0.6.0/tests/utils/test_configdict.py`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/tests/utils/test_files.py` & `impactlab_tools-0.6.0/tests/utils/test_files.py`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/tests/utils/test_paralog.py` & `impactlab_tools-0.6.0/tests/utils/test_paralog.py`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/tests/utils/test_weighting.py` & `impactlab_tools-0.6.0/tests/utils/test_weighting.py`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/.gitignore` & `impactlab_tools-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/LICENSE` & `impactlab_tools-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/README.rst` & `impactlab_tools-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `impactlab_tools-0.5.0/pyproject.toml` & `impactlab_tools-0.6.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -14,38 +14,40 @@
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
-    "geopandas",
-    "h5netcdf",
-    "matplotlib",
     "numpy>=1.7",
     "pandas>=0.15",
     "pyyaml",
     "scipy",
     "xarray>=0.8",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ClimateImpactLab/impactlab-tools"
 "Bug Tracker" = "https://github.com/ClimateImpactLab/impactlab-tools/issues"
 
 [project.optional-dependencies]
+complete = ["impactlab-tools[viz,docs,test]"]
 docs = [
     "Sphinx",
     "sphinx-rtd-theme",
 ]
 test = [
     "ruff",
     "pytest>=3.0",
     "pytest-cov>=2.0",
 ]
+viz = [
+    "geopandas",
+    "matplotlib",
+]
 
 [tool.pytest.ini_options]
 testpaths = [
     "src",
     "tests",
 ]
 addopts = "--cov=impactlab_tools --doctest-modules"
@@ -58,14 +60,16 @@
 version-file = "src/impactlab_tools/_version.py"
 
 [tool.ruff]
 exclude = [
     ".eggs",
     "docs",
 ]
+
+[tool.ruff.lint]
 # E402: module level import not at top of file
 ignore = [
     "E402",
 ]
 select = [
     # Pyflakes
     "F",
```

### Comparing `impactlab_tools-0.5.0/PKG-INFO` & `impactlab_tools-0.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,43 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: impactlab-tools
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python tools for Climate Impact Lab developers
 Project-URL: Homepage, https://github.com/ClimateImpactLab/impactlab-tools
 Project-URL: Bug Tracker, https://github.com/ClimateImpactLab/impactlab-tools/issues
 Author-email: Climate Impact Lab <mdelgado@rhg.com>
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Requires-Dist: geopandas
-Requires-Dist: h5netcdf
-Requires-Dist: matplotlib
 Requires-Dist: numpy>=1.7
 Requires-Dist: pandas>=0.15
 Requires-Dist: pyyaml
 Requires-Dist: scipy
 Requires-Dist: xarray>=0.8
+Provides-Extra: complete
+Requires-Dist: geopandas; extra == 'complete'
+Requires-Dist: matplotlib; extra == 'complete'
+Requires-Dist: pytest-cov>=2.0; extra == 'complete'
+Requires-Dist: pytest>=3.0; extra == 'complete'
+Requires-Dist: ruff; extra == 'complete'
+Requires-Dist: sphinx; extra == 'complete'
+Requires-Dist: sphinx-rtd-theme; extra == 'complete'
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == 'docs'
 Requires-Dist: sphinx-rtd-theme; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: pytest-cov>=2.0; extra == 'test'
 Requires-Dist: pytest>=3.0; extra == 'test'
 Requires-Dist: ruff; extra == 'test'
+Provides-Extra: viz
+Requires-Dist: geopandas; extra == 'viz'
+Requires-Dist: matplotlib; extra == 'viz'
 Description-Content-Type: text/x-rst
 
 =========================================
 Climate Impact Lab development toolkit
 =========================================
 
 .. image:: https://img.shields.io/pypi/v/impactlab-tools.svg
```

