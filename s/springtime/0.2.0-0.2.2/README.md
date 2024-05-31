# Comparing `tmp/springtime-0.2.0.tar.gz` & `tmp/springtime-0.2.2.tar.gz`

## Comparing `springtime-0.2.0.tar` & `springtime-0.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 springtime-0.2.0/src/springtime/__init__.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 springtime-0.2.0/src/springtime/config.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 springtime-0.2.0/src/springtime/dummy.py
--rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 springtime-0.2.0/src/springtime/main.py
--rw-r--r--   0        0        0    13499 2020-02-02 00:00:00.000000 springtime-0.2.0/src/springtime/utils.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 springtime-0.2.0/src/springtime/datasets/__init__.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 springtime-0.2.0/src/springtime/datasets/abstract.py
--rw-r--r--   0        0        0    23261 2020-02-02 00:00:00.000000 springtime-0.2.0/src/springtime/datasets/appeears.py
--rw-r--r--   0        0        0    15309 2020-02-02 00:00:00.000000 springtime-0.2.0/src/springtime/datasets/daymet.py
--rw-r--r--   0        0        0    14553 2020-02-02 00:00:00.000000 springtime-0.2.0/src/springtime/datasets/eobs.py
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 springtime-0.2.0/src/springtime/datasets/pep725.py
--rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 springtime-0.2.0/src/springtime/datasets/phenocam.py
--rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 springtime-0.2.0/src/springtime/datasets/ppo.py
--rw-r--r--   0        0        0    10161 2020-02-02 00:00:00.000000 springtime-0.2.0/src/springtime/datasets/rnpn.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 springtime-0.2.0/src/springtime/models/__init__.py
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 springtime-0.2.0/src/springtime/models/basinhopper.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 springtime-0.2.0/src/springtime/models/loss_functions.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 springtime-0.2.0/src/springtime/models/phenology_models/__init__.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 springtime-0.2.0/src/springtime/models/phenology_models/phenology_model.py
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 springtime-0.2.0/src/springtime/models/phenology_models/thermaltime.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 springtime-0.2.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 springtime-0.2.0/LICENSE
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 springtime-0.2.0/README.md
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 springtime-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 springtime-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 springtime-0.2.2/src/springtime/__init__.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 springtime-0.2.2/src/springtime/config.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 springtime-0.2.2/src/springtime/dummy.py
+-rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 springtime-0.2.2/src/springtime/main.py
+-rw-r--r--   0        0        0    13499 2020-02-02 00:00:00.000000 springtime-0.2.2/src/springtime/utils.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 springtime-0.2.2/src/springtime/datasets/__init__.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 springtime-0.2.2/src/springtime/datasets/abstract.py
+-rw-r--r--   0        0        0    23261 2020-02-02 00:00:00.000000 springtime-0.2.2/src/springtime/datasets/appeears.py
+-rw-r--r--   0        0        0    15364 2020-02-02 00:00:00.000000 springtime-0.2.2/src/springtime/datasets/daymet.py
+-rw-r--r--   0        0        0    14553 2020-02-02 00:00:00.000000 springtime-0.2.2/src/springtime/datasets/eobs.py
+-rw-r--r--   0        0        0     4608 2020-02-02 00:00:00.000000 springtime-0.2.2/src/springtime/datasets/pep725.py
+-rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 springtime-0.2.2/src/springtime/datasets/phenocam.py
+-rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 springtime-0.2.2/src/springtime/datasets/ppo.py
+-rw-r--r--   0        0        0    10161 2020-02-02 00:00:00.000000 springtime-0.2.2/src/springtime/datasets/rnpn.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 springtime-0.2.2/src/springtime/models/__init__.py
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 springtime-0.2.2/src/springtime/models/basinhopper.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 springtime-0.2.2/src/springtime/models/loss_functions.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 springtime-0.2.2/src/springtime/models/phenology_models/__init__.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 springtime-0.2.2/src/springtime/models/phenology_models/phenology_model.py
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 springtime-0.2.2/src/springtime/models/phenology_models/thermaltime.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 springtime-0.2.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 springtime-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 springtime-0.2.2/README.md
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 springtime-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 springtime-0.2.2/PKG-INFO
```

### Comparing `springtime-0.2.0/src/springtime/config.py` & `springtime-0.2.2/src/springtime/config.py`

 * *Files identical despite different names*

### Comparing `springtime-0.2.0/src/springtime/dummy.py` & `springtime-0.2.2/src/springtime/dummy.py`

 * *Files identical despite different names*

### Comparing `springtime-0.2.0/src/springtime/main.py` & `springtime-0.2.2/src/springtime/main.py`

 * *Files identical despite different names*

### Comparing `springtime-0.2.0/src/springtime/utils.py` & `springtime-0.2.2/src/springtime/utils.py`

 * *Files identical despite different names*

### Comparing `springtime-0.2.0/src/springtime/datasets/__init__.py` & `springtime-0.2.2/src/springtime/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `springtime-0.2.0/src/springtime/datasets/abstract.py` & `springtime-0.2.2/src/springtime/datasets/abstract.py`

 * *Files identical despite different names*

### Comparing `springtime-0.2.0/src/springtime/datasets/appeears.py` & `springtime-0.2.2/src/springtime/datasets/appeears.py`

 * *Files identical despite different names*

### Comparing `springtime-0.2.0/src/springtime/datasets/daymet.py` & `springtime-0.2.2/src/springtime/datasets/daymet.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,14 +250,15 @@
             return [self.download_point(self.points)]
 
         return [self.download_point(point) for point in self.points]
 
     def download_point(self, point: Point):
         """Download data for a single point."""
         path = self._point_path(point)
+        path.parent.mkdir(exist_ok=True, parents=True)
 
         if path.exists() and not CONFIG.force_override:
             logger.info(f"Found {path}")
         else:
             logger.info(f"Downloading data to {self._point_path(point)}.")
             run_r_script(self._r_download_point(point))
             logger.info("Please notice the metadata at the top of the file.")
@@ -302,15 +303,15 @@
 
     def raw_load_point(self, point) -> gpd.GeoDataFrame:
         """Read csv file for a single daymet data point.
 
         Lat/lon is in csv headers. Add geometry column instead.
         """
         file = self._point_path(point)
-        df = pd.read_csv(file, skiprows=7)
+        df = pd.read_csv(file, skiprows=6)
 
         # Add geometry since we want to batch read dataframes with different coords
         geometry = gpd.points_from_xy([point.x] * len(df), [point.y] * len(df))
         gdf = gpd.GeoDataFrame(df).set_geometry(geometry)
 
         # type checker is iffy
         assert isinstance(gdf, gpd.GeoDataFrame), "Something unexpected happened"
```

### Comparing `springtime-0.2.0/src/springtime/datasets/eobs.py` & `springtime-0.2.2/src/springtime/datasets/eobs.py`

 * *Files identical despite different names*

### Comparing `springtime-0.2.0/src/springtime/datasets/pep725.py` & `springtime-0.2.2/src/springtime/datasets/pep725.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 Requires phenor R package. Install with
 
 ```R
 devtools::install_github("bluegreen-labs/phenor@v1.3.1")
 ```
 
-Requires `~/.config/pep725_credentials.txt` file with your PEP725 credentials.
-Email adress on first line, password on second line.
+Requires `~/.config/springtime/pep725_credentials.txt` file with your
+PEP725 credentials. Email adress on first line, password on second line.
 
 Example:
 
     ```python
     from springtime.datasets.pep725 import PEP725Phenor
     dataset = PEP725Phenor(species='Syringa vulgaris', years=[2000, 2000])
     dataset.download()
```

### Comparing `springtime-0.2.0/src/springtime/datasets/phenocam.py` & `springtime-0.2.2/src/springtime/datasets/phenocam.py`

 * *Files identical despite different names*

### Comparing `springtime-0.2.0/src/springtime/datasets/ppo.py` & `springtime-0.2.2/src/springtime/datasets/ppo.py`

 * *Files identical despite different names*

### Comparing `springtime-0.2.0/src/springtime/datasets/rnpn.py` & `springtime-0.2.2/src/springtime/datasets/rnpn.py`

 * *Files identical despite different names*

### Comparing `springtime-0.2.0/src/springtime/models/basinhopper.py` & `springtime-0.2.2/src/springtime/models/basinhopper.py`

 * *Files identical despite different names*

### Comparing `springtime-0.2.0/src/springtime/models/phenology_models/thermaltime.py` & `springtime-0.2.2/src/springtime/models/phenology_models/thermaltime.py`

 * *Files identical despite different names*

### Comparing `springtime-0.2.0/.gitignore` & `springtime-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `springtime-0.2.0/LICENSE` & `springtime-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `springtime-0.2.0/README.md` & `springtime-0.2.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 [![Documentation Status](https://readthedocs.org/projects/springtime/badge/?version=latest)](https://springtime.readthedocs.io/en/latest/?badge=latest)
 [![RSD](https://img.shields.io/badge/RSD-springtime-blue)](https://research-software-directory.org/software/springtime)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7835299.svg)](https://doi.org/10.5281/zenodo.7835299)
+[![PyPI version](https://badge.fury.io/py/springtime.svg)](https://badge.fury.io/py/springtime)
+
+
 
 For detailed information and instruction, please refer to the
 [documentation](https://springtime.readthedocs.io/)
 
 <!--intro-start-->
 # Springtime
```

### Comparing `springtime-0.2.0/pyproject.toml` & `springtime-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `springtime-0.2.0/PKG-INFO` & `springtime-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: springtime
-Version: 0.2.0
+Version: 0.2.2
 Summary: Spatiotemporal phenology research with interpretable models
 Project-URL: Documentation, https://springtime.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/phenology/springtime/issues
 Project-URL: Source, https://github.com/phenology/springtime
 Author-email: Peter Kalverla <peter.kalverla@gmx.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -56,14 +56,17 @@
 Requires-Dist: pycaret[models]; extra == 'extras'
 Requires-Dist: pyphenology; extra == 'extras'
 Description-Content-Type: text/markdown
 
 [![Documentation Status](https://readthedocs.org/projects/springtime/badge/?version=latest)](https://springtime.readthedocs.io/en/latest/?badge=latest)
 [![RSD](https://img.shields.io/badge/RSD-springtime-blue)](https://research-software-directory.org/software/springtime)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7835299.svg)](https://doi.org/10.5281/zenodo.7835299)
+[![PyPI version](https://badge.fury.io/py/springtime.svg)](https://badge.fury.io/py/springtime)
+
+
 
 For detailed information and instruction, please refer to the
 [documentation](https://springtime.readthedocs.io/)
 
 <!--intro-start-->
 # Springtime
```

