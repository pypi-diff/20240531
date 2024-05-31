# Comparing `tmp/hf_hydrodata-1.1.7.tar.gz` & `tmp/hf_hydrodata-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hf_hydrodata-1.1.7.tar", max compression
+gzip compressed data, was "hf_hydrodata-1.1.9.tar", max compression
```

## Comparing `hf_hydrodata-1.1.7.tar` & `hf_hydrodata-1.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1241 2024-03-27 19:21:02.445266 hf_hydrodata-1.1.7/LICENSE
--rw-r--r--   0        0        0     5347 2024-03-27 19:21:02.445266 hf_hydrodata-1.1.7/README.md
--rw-r--r--   0        0        0      924 2024-03-28 14:52:06.357246 hf_hydrodata-1.1.7/pyproject.toml
--rw-r--r--   0        0        0      847 2024-01-10 13:07:50.859229 hf_hydrodata-1.1.7/src/hf_hydrodata/__init__.py
--rw-r--r--   0        0        0    25580 2024-03-22 19:17:19.697150 hf_hydrodata-1.1.7/src/hf_hydrodata/data_catalog.py
--rw-r--r--   0        0        0    13568 2024-02-16 17:29:21.918229 hf_hydrodata-1.1.7/src/hf_hydrodata/data_model_access.py
--rw-r--r--   0        0        0     5828 2024-02-16 17:29:21.918229 hf_hydrodata-1.1.7/src/hf_hydrodata/generate_hydrodata_catalog_yaml.py
--rw-r--r--   0        0        0     9478 2024-01-10 13:07:50.859229 hf_hydrodata-1.1.7/src/hf_hydrodata/grid.py
--rw-r--r--   0        0        0   112256 2024-03-28 14:52:06.358246 hf_hydrodata-1.1.7/src/hf_hydrodata/gridded.py
--rw-r--r--   0        0        0      462 2023-11-29 18:16:33.996626 hf_hydrodata-1.1.7/src/hf_hydrodata/model/aggregation.csv
--rw-r--r--   0        0        0    68493 2024-03-27 19:21:02.446266 hf_hydrodata-1.1.7/src/hf_hydrodata/model/data_catalog_entry.csv
--rw-r--r--   0        0        0     2223 2024-03-22 19:17:19.698150 hf_hydrodata-1.1.7/src/hf_hydrodata/model/dataset.csv
--rw-r--r--   0        0        0      243 2023-12-05 18:33:56.257124 hf_hydrodata-1.1.7/src/hf_hydrodata/model/dataset_type.csv
--rw-r--r--   0        0        0      251 2024-03-22 19:17:19.698150 hf_hydrodata-1.1.7/src/hf_hydrodata/model/datasource.csv
--rw-r--r--   0        0        0     1067 2024-03-27 19:21:02.446266 hf_hydrodata-1.1.7/src/hf_hydrodata/model/file_type.csv
--rw-r--r--   0        0        0     1681 2024-01-16 13:26:11.587371 hf_hydrodata-1.1.7/src/hf_hydrodata/model/grid.csv
--rw-r--r--   0        0        0      269 2023-12-05 18:33:56.257124 hf_hydrodata-1.1.7/src/hf_hydrodata/model/security_level.csv
--rw-r--r--   0        0        0       90 2023-11-09 13:40:32.111421 hf_hydrodata-1.1.7/src/hf_hydrodata/model/site_type.csv
--rw-r--r--   0        0        0       63 2023-11-09 13:40:32.111421 hf_hydrodata-1.1.7/src/hf_hydrodata/model/structure_type.csv
--rw-r--r--   0        0        0      832 2024-02-03 02:01:34.098598 hf_hydrodata-1.1.7/src/hf_hydrodata/model/substitution_keys.csv
--rw-r--r--   0        0        0      540 2024-03-27 19:21:02.446266 hf_hydrodata-1.1.7/src/hf_hydrodata/model/temporal_resolution.csv
--rw-r--r--   0        0        0      111 2023-11-09 13:40:32.111421 hf_hydrodata-1.1.7/src/hf_hydrodata/model/unit_type.csv
--rw-r--r--   0        0        0      824 2023-12-05 18:33:56.257124 hf_hydrodata-1.1.7/src/hf_hydrodata/model/units.csv
--rw-r--r--   0        0        0     5378 2024-02-03 02:01:34.098598 hf_hydrodata-1.1.7/src/hf_hydrodata/model/variable.csv
--rw-r--r--   0        0        0      679 2023-12-05 18:33:56.257124 hf_hydrodata-1.1.7/src/hf_hydrodata/model/variable_type.csv
--rw-r--r--   0        0        0    79164 2024-03-28 14:52:06.358246 hf_hydrodata-1.1.7/src/hf_hydrodata/point.py
--rw-r--r--   0        0        0     6784 2024-01-16 13:26:11.587371 hf_hydrodata-1.1.7/src/hf_hydrodata/projection.py
--rw-r--r--   0        0        0     1152 2024-01-17 18:05:31.038756 hf_hydrodata-1.1.7/src/hf_hydrodata/publish_model.py
--rw-r--r--   0        0        0     6228 1970-01-01 00:00:00.000000 hf_hydrodata-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1241 2024-03-27 19:21:02.445266 hf_hydrodata-1.1.9/LICENSE
+-rw-r--r--   0        0        0     5347 2024-03-27 19:21:02.445266 hf_hydrodata-1.1.9/README.md
+-rw-r--r--   0        0        0      924 2024-04-19 20:55:51.365056 hf_hydrodata-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0      847 2024-01-10 13:07:50.859229 hf_hydrodata-1.1.9/src/hf_hydrodata/__init__.py
+-rw-r--r--   0        0        0    25580 2024-03-22 19:17:19.697150 hf_hydrodata-1.1.9/src/hf_hydrodata/data_catalog.py
+-rw-r--r--   0        0        0    13568 2024-02-16 17:29:21.918229 hf_hydrodata-1.1.9/src/hf_hydrodata/data_model_access.py
+-rw-r--r--   0        0        0     5828 2024-02-16 17:29:21.918229 hf_hydrodata-1.1.9/src/hf_hydrodata/generate_hydrodata_catalog_yaml.py
+-rw-r--r--   0        0        0     9478 2024-01-10 13:07:50.859229 hf_hydrodata-1.1.9/src/hf_hydrodata/grid.py
+-rw-r--r--   0        0        0   112674 2024-04-19 20:55:51.365056 hf_hydrodata-1.1.9/src/hf_hydrodata/gridded.py
+-rw-r--r--   0        0        0      478 2024-04-19 20:55:51.366056 hf_hydrodata-1.1.9/src/hf_hydrodata/model/aggregation.csv
+-rw-r--r--   0        0        0    68954 2024-04-19 20:55:51.366056 hf_hydrodata-1.1.9/src/hf_hydrodata/model/data_catalog_entry.csv
+-rw-r--r--   0        0        0     2429 2024-04-19 20:55:51.366056 hf_hydrodata-1.1.9/src/hf_hydrodata/model/dataset.csv
+-rw-r--r--   0        0        0      243 2023-12-05 18:33:56.257124 hf_hydrodata-1.1.9/src/hf_hydrodata/model/dataset_type.csv
+-rw-r--r--   0        0        0      285 2024-04-19 20:55:51.366056 hf_hydrodata-1.1.9/src/hf_hydrodata/model/datasource.csv
+-rw-r--r--   0        0        0     1067 2024-03-27 19:21:02.446266 hf_hydrodata-1.1.9/src/hf_hydrodata/model/file_type.csv
+-rw-r--r--   0        0        0     1681 2024-01-16 13:26:11.587371 hf_hydrodata-1.1.9/src/hf_hydrodata/model/grid.csv
+-rw-r--r--   0        0        0      269 2023-12-05 18:33:56.257124 hf_hydrodata-1.1.9/src/hf_hydrodata/model/security_level.csv
+-rw-r--r--   0        0        0       90 2023-11-09 13:40:32.111421 hf_hydrodata-1.1.9/src/hf_hydrodata/model/site_type.csv
+-rw-r--r--   0        0        0       63 2023-11-09 13:40:32.111421 hf_hydrodata-1.1.9/src/hf_hydrodata/model/structure_type.csv
+-rw-r--r--   0        0        0      832 2024-02-03 02:01:34.098598 hf_hydrodata-1.1.9/src/hf_hydrodata/model/substitution_keys.csv
+-rw-r--r--   0        0        0      592 2024-04-19 20:55:51.366056 hf_hydrodata-1.1.9/src/hf_hydrodata/model/temporal_resolution.csv
+-rw-r--r--   0        0        0      111 2023-11-09 13:40:32.111421 hf_hydrodata-1.1.9/src/hf_hydrodata/model/unit_type.csv
+-rw-r--r--   0        0        0      824 2023-12-05 18:33:56.257124 hf_hydrodata-1.1.9/src/hf_hydrodata/model/units.csv
+-rw-r--r--   0        0        0     5378 2024-02-03 02:01:34.098598 hf_hydrodata-1.1.9/src/hf_hydrodata/model/variable.csv
+-rw-r--r--   0        0        0      679 2023-12-05 18:33:56.257124 hf_hydrodata-1.1.9/src/hf_hydrodata/model/variable_type.csv
+-rw-r--r--   0        0        0    81199 2024-04-19 20:55:51.366056 hf_hydrodata-1.1.9/src/hf_hydrodata/point.py
+-rw-r--r--   0        0        0     6784 2024-01-16 13:26:11.587371 hf_hydrodata-1.1.9/src/hf_hydrodata/projection.py
+-rw-r--r--   0        0        0     1152 2024-01-17 18:05:31.038756 hf_hydrodata-1.1.9/src/hf_hydrodata/publish_model.py
+-rw-r--r--   0        0        0     6228 1970-01-01 00:00:00.000000 hf_hydrodata-1.1.9/PKG-INFO
```

### Comparing `hf_hydrodata-1.1.7/LICENSE` & `hf_hydrodata-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hf_hydrodata-1.1.7/README.md` & `hf_hydrodata-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `hf_hydrodata-1.1.7/pyproject.toml` & `hf_hydrodata-1.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hf_hydrodata"
-version = "1.1.7"
+version = "1.1.9"
 description = "hydroframe tools and utilities"
 authors = ["William M. Hasling", "Laura Condon", "Reed Maxwell",  "George Artavanis", "Amy M. Johnson", "Amy C. Defnet"]
 license = "MIT"
 readme = "README.md"
 
 [package]
 include = ["src/hf_hydrodata/model/*.csv"]
```

### Comparing `hf_hydrodata-1.1.7/src/hf_hydrodata/__init__.py` & `hf_hydrodata-1.1.9/src/hf_hydrodata/__init__.py`

 * *Files identical despite different names*

### Comparing `hf_hydrodata-1.1.7/src/hf_hydrodata/data_catalog.py` & `hf_hydrodata-1.1.9/src/hf_hydrodata/data_catalog.py`

 * *Files identical despite different names*

### Comparing `hf_hydrodata-1.1.7/src/hf_hydrodata/data_model_access.py` & `hf_hydrodata-1.1.9/src/hf_hydrodata/data_model_access.py`

 * *Files identical despite different names*

### Comparing `hf_hydrodata-1.1.7/src/hf_hydrodata/generate_hydrodata_catalog_yaml.py` & `hf_hydrodata-1.1.9/src/hf_hydrodata/generate_hydrodata_catalog_yaml.py`

 * *Files identical despite different names*

### Comparing `hf_hydrodata-1.1.7/src/hf_hydrodata/grid.py` & `hf_hydrodata-1.1.9/src/hf_hydrodata/grid.py`

 * *Files identical despite different names*

### Comparing `hf_hydrodata-1.1.7/src/hf_hydrodata/gridded.py` & `hf_hydrodata-1.1.9/src/hf_hydrodata/gridded.py`

 * *Files 1% similar despite different names*

```diff
@@ -519,16 +519,22 @@
         # The files will contain projection information suitable to view with GIS.
 
     For long downloads if the function execution is aborted before completion it can be restarted and will continue where it left off by skipping
     files that already exist. To re-download data, remember to delete previously created files first.
     """
     verbose_start_time = time.time()
     temporal_resolution = options.get("temporal_resolution")
-    temporal_resolution = _get_temporal_resolution_from_catalog(options) if temporal_resolution is None else temporal_resolution
-    temporal_resolution = "static" if temporal_resolution == "-" else temporal_resolution
+    temporal_resolution = (
+        _get_temporal_resolution_from_catalog(options)
+        if temporal_resolution is None
+        else temporal_resolution
+    )
+    temporal_resolution = (
+        "static" if temporal_resolution == "-" else temporal_resolution
+    )
     if temporal_resolution not in ["daily", "hourly", "monthly", "static"]:
         raise ValueError(
             "The temporal_resolution must be hourly, daily, monthly, or static."
         )
 
     if not filename_template:
         if temporal_resolution == "hourly":
@@ -655,21 +661,24 @@
     entries = dc.get_catalog_entries(options)
     if len(entries) == 0:
         raise ValueError("Unable to determine temporal resolution")
     result = entries[0]["temporal_resolution"]
     result = "static" if result == "-" else result
     for entry in entries:
         temporal_resolution = entry["temporal_resolution"]
-        temporal_resolution = "static" if temporal_resolution == "-" else temporal_resolution
-        if temporal_resolution is not None and not temporal_resolution == result:
+        temporal_resolution = (
+            "static" if temporal_resolution == "-" else temporal_resolution
+        )
+        if temporal_resolution != result:
             raise ValueError("Temporal resolution is not specified and is ambiguous.")
     if result is None:
         raise ValueError("Unable to determine temporal resolution.")
     return result
 
+
 def _get_aggregation_entries(options):
     """
     Get the list of different aggregation entries for the filter options.
     Returns:
         A list of entries that satisfy the options filter.
     Raises:
         ValueError: if two entries for the filter different by other than aggregation value.
@@ -1289,15 +1298,15 @@
             data = _read_and_filter_netcdf_files(entry, options, time_values)
         elif file_type == "tiff":
             data = _read_and_filter_tiff_files(entry, options)
         else:
             raise ValueError(f"File type '{file_type}' is not supported yet.")
         if structure_type == "gridded":
             data = _adjust_dimensions(data, entry)
-            if options.get("mask") and options.get("mask").lower() in ["true", "yes"]:
+            if not options.get("nomask") == "true":
                 data = _apply_mask(data, entry, options)
         options = _convert_json_to_strings(options)
 
     return data
 
 
 def _apply_mask(data, entry, options):
@@ -1307,48 +1316,53 @@
         The data with NaN values used for masked point.
     If the options contain a huc_id option then mask using the HUC boundaries of the grid of the entry.
     Else if the options contain a grid_bounds (or lat/lon bounds) mask using the HUC bounds subset for that grid.
     The second option masks only against ocean and outer HUC bounds. The first option masks with internal HUC boundaries.
     """
 
     if options.get("dataset") == "huc_mapping":
+        # Do not mask the mask
         return data
     grid = entry["grid"]
     if grid not in ["conus1", "conus2"]:
         return data
     if not isinstance(data, np.ndarray):
+        # All results should be numpy arrays, but if it is not then do not do anything since it would not work
         return data
     grid_bounds = _get_grid_bounds(grid, options)
     huc_id = options.get("huc_id")
     if huc_id:
+        # Only mask using HUC masks if the query gives us list of huc_id
         huc_ids = huc_id.split(",")
         bbox = get_huc_bbox(grid, huc_ids)
         level = len(huc_ids[0])
         mask = get_gridded_data(
             {
                 "dataset": "huc_mapping",
                 "variable": "huc_map",
                 "grid": grid,
                 "grid_bounds": bbox,
                 "level": level,
             }
         )
+        # Apply the HUC mask to the data, mask with all huc_ids
         for h_id in huc_ids:
             data = np.where(mask == float(h_id), data, np.nan)
     elif grid_bounds:
+        # If subsetting with a grid using level 2 HUC mask to mask coastline
         mask = get_gridded_data(
             {
                 "dataset": "huc_mapping",
                 "variable": "huc_map",
                 "grid": grid,
                 "grid_bounds": grid_bounds,
                 "level": 2,
             }
         )
-        data = np.where(mask, np.nan, data)
+        data = np.where(mask > 0, data, np.nan)
     return data
 
 
 def get_huc_from_latlon(grid: str, level: int, lat: float, lon: float) -> str:
     """
     Get a HUC id at a lat/lon point for a given grid and level.
 
@@ -2140,17 +2154,21 @@
     ):
         raise ValueError(
             f"grid_bounds {grid_bounds[0]},{grid_bounds[1]} is outside the grid shape {grid_shape[2]}, {grid_shape[1]}."
         )
 
     if grid_bounds:
         if len(da.shape) == 3:
-            result = da[:, grid_bounds[1] : grid_bounds[3], grid_bounds[0] : grid_bounds[2]]
+            result = da[
+                :, grid_bounds[1] : grid_bounds[3], grid_bounds[0] : grid_bounds[2]
+            ]
         elif len(da.shape) == 2:
-            result = da[grid_bounds[1] : grid_bounds[3], grid_bounds[0] : grid_bounds[2]]
+            result = da[
+                grid_bounds[1] : grid_bounds[3], grid_bounds[0] : grid_bounds[2]
+            ]
         else:
             raise ValueError(f"Unsupported shape size {len(da.shape)}")
     else:
         result = da
     return result
```

### Comparing `hf_hydrodata-1.1.7/src/hf_hydrodata/model/data_catalog_entry.csv` & `hf_hydrodata-1.1.9/src/hf_hydrodata/model/data_catalog_entry.csv`

 * *Files 1% similar despite different names*

```diff
@@ -204,52 +204,52 @@
 208,conus2_current_conditions,tiff,water_table_depth,band_data,,,,m,mean,conus2_wtd,,3,/hydrodata/temp/high_resolution_data/WTD_estimates/30m/remapped_data/wtd_mean_estimate_RF_additional_inputs_dummy_drop0LP_1000m_CONUS2_m_1s_remapped.tif,,
 209,conus2_current_conditions,tiff,water_table_depth,band_data,,,,m,mean,conus2_wtd.100,,3,/hydrodata/temp/high_resolution_data/WTD_estimates/30m/remapped_data/wtd_mean_estimate_RF_additional_inputs_dummy_drop0LP_100m_CONUS2_m_1s_remapped.tif,,
 210,conus2_current_conditions,tiff,water_table_depth,band_data,,,,m,mean,conus2_wtd.30,,3,/hydrodata/temp/high_resolution_data/WTD_estimates/30m/compressed_data/wtd_mean_estimate_RF_additional_inputs_dummy_drop0LP_1s_CONUS2_m_remapped_unflip_compressed.tif,,
 211,nasa_smap,netcdf,latitude,Latitude,,,static,degrees,mean,smapgrid,wy,3,/hydrodata/national_obs/smap/data/Oct1_{wy_minus1}_Sept30_{wy}.nc,,
 212,nasa_smap,netcdf,longitude,Longitude,,,static,degrees,mean,smapgrid,wy,3,/hydrodata/national_obs/smap/data/Oct1_{wy_minus1}_Sept30_{wy}.nc,,
 213,conus2_current_conditions,pfb,soil_moisture,soil_moisture,8/1/23,,daily,cm3/cm3,mean,conus2,mdy,1,/hydrodata/HydroGEN/current_conditions/CONUS2/WY{wy}/{dataset_var}.{mdy}.pfb,,
 214,conus2_domain,pfb,veg_type_IGBP,vegetation_type,,,static,-,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/model_inputs/1km_CONUS2_landcover_IGBP_723.pfb,,
-215,conus2_domain,tiff,veg_type_IGBP,vegetation_type,,,static,-,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/model_inputs/1km_CONUS2_landcover_IGBP_723.tif,,
+215,conus2_domain,tiff,veg_type_IGBP,band_data,,,static,-,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/model_inputs/1km_CONUS2_landcover_IGBP_723.tif,,
 216,conus2_domain,pfb,veg_type_IGBP,vegetation_type,,,static,-,-,conus2.250,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/model_inputs/250m_CONUS2_landcover_IGBP_723.pfb,,
-217,conus2_domain,tiff,veg_type_IGBP,vegetation_type,,,static,-,-,conus2.250,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/model_inputs/250m_CONUS2_landcover_IGBP_723.tif,,
+217,conus2_domain,tiff,veg_type_IGBP,band_data,,,static,-,-,conus2.250,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/model_inputs/250m_CONUS2_landcover_IGBP_723.tif,,
 218,conus2_domain,pfb,slope_x,slope_x,,,static,-,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/model_inputs/CONUS2.0.Final1km.slopex.pfb,,
 219,conus2_domain,pfb,slope_y,slope_y,,,static,-,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/model_inputs/CONUS2.0.Final1km.slopey.pfb,,
 220,conus2_domain,drv_clm,clm_run,clm_run,,,static,-,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/model_inputs/drv_clmin.dat,,
 221,conus2_domain,vegm,clm_run,clm_run,,,static,-,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/model_inputs/drv_vegm.CONUS2_fixed.2.dat,,
 222,conus2_domain,vegp,clm_run,clm_run,,,static,-,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/model_inputs/drv_vegp.dat,,
 223,conus2_domain,pfb,pme,pme,,,static,m/h,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/model_inputs/1km_CONUS2_PME.pfb,pme that was used for steady state CONUS2 spinup,
 224,conus2_domain,pfsol,pf_solid,pf_solid,,,static,-,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/model_inputs/CONUS2.0_fix115.pfsol,,
 225,conus2_domain,pfb,mannings,mannings,,,static,-,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/model_inputs/CONUS2.0.Final1km_mannings_rv50_original_values_Lake_Sink.pfb,,
 226,conus2_domain,pfb,pf_indicator,pf_indicator,,,static,-,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/model_inputs/CONUS2.0.Final1km.Subsurface.pfb,,
 227,conus2_domain,pfb,pf_flowbarrier,pf_flowbarrier,,,static,-,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/model_inputs/CONUS2.0.Shangguan_200m_FBZ.pfb,,
 228,conus2_domain,pfb,ss_pressure_head,pressure,,,static,-,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/steady_state_runs/2003_run/spinup.wy2003.out.press.08760.pfb,steady state pressure used to initialize transient runs,
 229,conus2_domain,pfb,distance_stream_lin,distance_stream_lin,,,static,km,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/1km/CONUS2.0.Final1km.DisToStream.pfb,Map of distance for each cell to the stream (CONUS2.0.Final1km.RiverMask) using the function StreamDist in PriorityFlow.,
-230,conus2_domain,tiff,distance_stream_lin,distance_stream_lin,,,static,km,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/1km/CONUS2.0.Final1km.DisToStream.tif,Map of distance for each cell to the stream (CONUS2.0.Final1km.RiverMask) using the function StreamDist in PriorityFlow.,
+230,conus2_domain,tiff,distance_stream_lin,band_data,,,static,km,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/1km/CONUS2.0.Final1km.DisToStream.tif,Map of distance for each cell to the stream (CONUS2.0.Final1km.RiverMask) using the function StreamDist in PriorityFlow.,
 231,conus2_domain,pfb,drainage_area,drainage_area,,,static,km2,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/1km/CONUS2.0.Final1km.DrainageArea.pfb,Drainage area in km2 calculated based on the flow directions,
-232,conus2_domain,tiff,drainage_area,drainage_area,,,static,km2,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/1km/CONUS2.0.Final1km.DrainageArea.tif,Drainage area in km2 calculated based on the flow directions,
+232,conus2_domain,tiff,drainage_area,band_data,,,static,km2,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/1km/CONUS2.0.Final1km.DrainageArea.tif,Drainage area in km2 calculated based on the flow directions,
 233,conus2_domain,pfb,flow_direction,flow_direction,,,static,-,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/1km/CONUS2.0.Final1km.FlowDirection.pfb,"Primary flow direction for every grid cell (1=down, 2=left, 3=up, 4=right)",
-234,conus2_domain,tiff,flow_direction,flow_direction,,,static,-,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/1km/CONUS2.0.Final1km.FlowDirection.tif,"Primary flow direction for every grid cell (1=down, 2=left, 3=up, 4=right)",
+234,conus2_domain,tiff,flow_direction,band_data,,,static,-,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/1km/CONUS2.0.Final1km.FlowDirection.tif,"Primary flow direction for every grid cell (1=down, 2=left, 3=up, 4=right)",
 235,conus2_domain,pfb,elevation,elevation,,,static,m,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/1km/CONUS2.0.Final1km.ProcessedDEM.pfb,"Final DEM after, smoothing, applying PriroirtyFlow algorithm to ensure complete drainage and additional smoothing to create constant slopes along river segments.",
-236,conus2_domain,tiff,elevation,elevation,,,static,m,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/1km/CONUS2.0.Final1km.ProcessedDEM.tif,"Final DEM after, smoothing, applying PriroirtyFlow algorithm to ensure complete drainage and additional smoothing to create constant slopes along river segments.",
+236,conus2_domain,tiff,elevation,band_data,,,static,m,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/1km/CONUS2.0.Final1km.ProcessedDEM.tif,"Final DEM after, smoothing, applying PriroirtyFlow algorithm to ensure complete drainage and additional smoothing to create constant slopes along river segments.",
 247,conus2_domain,pfb,stream_order,stream_order,,,static,-,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/1km/CONUS2.0.Final1km.StreamOrder.pfb,Strahler stream order calculated from the 100km area threshold river mask using the function CalcStreamOrder in PriorityFlow,
-248,conus2_domain,tiff,stream_order,stream_order,,,static,-,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/1km/CONUS2.0.Final1km.StreamOrder.tif,Strahler stream order calculated from the 100km area threshold river mask using the function CalcStreamOrder in PriorityFlow,
+248,conus2_domain,tiff,stream_order,band_data,,,static,-,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/1km/CONUS2.0.Final1km.StreamOrder.tif,Strahler stream order calculated from the 100km area threshold river mask using the function CalcStreamOrder in PriorityFlow,
 249,conus2_domain,pfb,stream_segments,stream_segments,,,static,-,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/1km/CONUS2.0.Final1km.StreamSegments.pfb,Mask of stream segments with their segment IDs.,
-250,conus2_domain,tiff,stream_segments,stream_segments,,,static,-,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/1km/CONUS2.0.Final1km.StreamSegments.tif,Mask of stream segments with their segment IDs.,
+250,conus2_domain,tiff,stream_segments,band_data,,,static,-,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/1km/CONUS2.0.Final1km.StreamSegments.tif,Mask of stream segments with their segment IDs.,
 251,conus2_domain,pfb,subbasins,subbasins,,,static,-,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/1km/CONUS2.0.Final1km.Subbasins.pfb,Map of the subbasins drainage area for each stream segment.,
-252,conus2_domain,tiff,subbasins,subbasins,,,static,-,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/1km/CONUS2.0.Final1km.Subbasins.tif,Map of the subbasins drainage area for each stream segment.,
+252,conus2_domain,tiff,subbasins,band_data,,,static,-,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/1km/CONUS2.0.Final1km.Subbasins.tif,Map of the subbasins drainage area for each stream segment.,
 253,conus2_domain,pfb,distance_stream_lin,distance_stream_lin,,,static,km,-,conus2.250,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/250m/CONUS2.0.Final250m.DisToStream.pfb,Map of distance for each cell to the stream (CONUS2.0.Final1km.RiverMask) using the function StreamDist in PriorityFlow.,
-254,conus2_domain,tiff,distance_stream_lin,distance_stream_lin,,,static,km,-,conus2.250,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/250m/CONUS2.0.Final250m.DisToStream.tif,Map of distance for each cell to the stream (CONUS2.0.Final1km.RiverMask) using the function StreamDist in PriorityFlow.,
-256,conus2_domain,tiff,drainage_area,drainage_area,,,static,km2,-,conus2.250,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/250m/CONUS2.0.Final250m.DrainageArea.tif,Drainage area in km2 calculated based on the flow directions,
-258,conus2_domain,tiff,flow_direction,flow_direction,,,static,-,-,conus2.250,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/250m/CONUS2.0.Final250m.FlowDirection.tif,"Primary flow direction for every grid cell (1=down, 2=left, 3=up, 4=right)",
-260,conus2_domain,tiff,elevation,elevation,,,static,m,-,conus2.250,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/250m/CONUS2.0.Final250m.ProcessedDEM.tif,"Final DEM after, smoothing, applying PriroirtyFlow algorithm to ensure complete drainage and additional smoothing to create constant slopes along river segments.",
-262,conus2_domain,tiff,stream_order,stream_order,,,static,-,-,conus2.250,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/250m/CONUS2.0.Final250m.StreamOrder.tif,Strahler stream order calculated from the 100km area threshold river mask using the function CalcStreamOrder in PriorityFlow,
-264,conus2_domain,tiff,stream_segments,stream_segments,,,static,-,-,conus2.250,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/250m/CONUS2.0.Final250m.StreamSegments.tif,Mask of stream segments with their segment IDs.,
-266,conus2_domain,tiff,subbasins,subbasins,,,static,-,-,conus2.250,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/250m/CONUS2.0.Final250m.Subbasins.tif,Map of the subbasins drainage area for each stream segment.,
+254,conus2_domain,tiff,distance_stream_lin,band_data,,,static,km,-,conus2.250,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/250m/CONUS2.0.Final250m.DisToStream.tif,Map of distance for each cell to the stream (CONUS2.0.Final1km.RiverMask) using the function StreamDist in PriorityFlow.,
+256,conus2_domain,tiff,drainage_area,band_data,,,static,km2,-,conus2.250,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/250m/CONUS2.0.Final250m.DrainageArea.tif,Drainage area in km2 calculated based on the flow directions,
+258,conus2_domain,tiff,flow_direction,band_data,,,static,-,-,conus2.250,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/250m/CONUS2.0.Final250m.FlowDirection.tif,"Primary flow direction for every grid cell (1=down, 2=left, 3=up, 4=right)",
+260,conus2_domain,tiff,elevation,band_data,,,static,m,-,conus2.250,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/250m/CONUS2.0.Final250m.ProcessedDEM.tif,"Final DEM after, smoothing, applying PriroirtyFlow algorithm to ensure complete drainage and additional smoothing to create constant slopes along river segments.",
+262,conus2_domain,tiff,stream_order,band_data,,,static,-,-,conus2.250,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/250m/CONUS2.0.Final250m.StreamOrder.tif,Strahler stream order calculated from the 100km area threshold river mask using the function CalcStreamOrder in PriorityFlow,
+264,conus2_domain,tiff,stream_segments,band_data,,,static,-,-,conus2.250,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/250m/CONUS2.0.Final250m.StreamSegments.tif,Mask of stream segments with their segment IDs.,
+266,conus2_domain,tiff,subbasins,band_data,,,static,-,-,conus2.250,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/topography_files/250m/CONUS2.0.Final250m.Subbasins.tif,Map of the subbasins drainage area for each stream segment.,
 267,conus2_domain,sa,lat_lon,lat_lon,,,static,-,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/domain_files/CONUS2.0.Final.LatLong.sa,,
-268,conus2_domain,tiff,mask,mask,,,static,-,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/domain_files/CONUS2.0.Final1km.Mask.tif,,
+268,conus2_domain,tiff,mask,band_data,,,static,-,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/domain_files/CONUS2.0.Final1km.Mask.tif,,
 271,observations,netcdf,streamflow,streamflow,,,daily,m3/s,mean,,site_id,0,/hydrodata/national_obs/streamflow/data/daily/{site_id}.nc,,streamflow
 272,observations,netcdf,anomaly,anomaly_daily_single_date,,,daily,-,mean,,site_id,0,/hydrodata/national_obs/streamflow/data/daily/{site_id}.nc,,streamflow
 273,observations,netcdf,anomaly_daily_week_of_values,anomaly_daily_week_of_values,,,daily,-,mean,,site_id,0,/hydrodata/national_obs/streamflow/data/daily/{site_id}.nc,,streamflow
 274,observations,netcdf,site_id,site,,,daily,-,mean,,site_id,0,/hydrodata/national_obs/streamflow/data/daily/{site_id}.nc,,streamflow
 275,observations,netcdf,streamflow,streamflow,,,weekly,mm,sum,,site_id,0,/hydrodata/national_obs/streamflow/data/weekly/{site_id}.nc,,streamflow
 276,observations,netcdf,anomaly,anomaly_weekly,,,weekly,-,sum,,site_id,0,/hydrodata/national_obs/streamflow/data/weekly/{site_id}.nc,,streamflow
 277,observations,netcdf,site_id,site,,,weekly,-,sum,,site_id,0,/hydrodata/national_obs/streamflow/data/weekly/{site_id}.nc,,streamflow
@@ -392,8 +392,11 @@
 515,conus1_baseline_mod,pfb,clm_run,clm_run,,,static,-,-,conus1,,1,/hydrodata/PFCLM/CONUS1_baseline/inputs/drv_vegm.fixed.pfb,,
 516,conus2_domain,pfb,clm_run,clm_run,,,static,-,-,conus2,,1,/hydrodata/PFCLM/CONUS2_baseline/inputs/model_inputs/drv_vegm.CONUS2_fixed.2.pfb,,
 517,noaa,pfb,precipitation,APCP,,,daily,mm,sum,conus1,wy,1,/hydrodata/national_obs/gridded_meteorology/NOAA_precipitation/CONUS1/WY{wy}/QPE.APCP.daily.regrid.{wy}.{wy_daynum:03d}.pfb,,
 518,noaa,pfb,air_temp,Temp_min,,,daily,K,min,conus1,wy_daynum,1,/hydrodata/national_obs/gridded_meteorology/NOAA_temperature/CONUS1/WY{wy}/HRRR.Temp_min.daily.regrid.{wy}.{wy_daynum:03d}.pfb,,
 519,noaa,pfb,air_temp,Temp_max,,,daily,K,max,conus1,wy_daynum,1,/hydrodata/national_obs/gridded_meteorology/NOAA_temperature/CONUS1/WY{wy}/HRRR.Temp_max.daily.regrid.{wy}.{wy_daynum:03d}.pfb,,
 520,noaa,pfb,air_temp,Temp_mean,,,daily,K,mean,conus1,wy_daynum,1,/hydrodata/national_obs/gridded_meteorology/NOAA_temperature/CONUS1/WY{wy}/HRRR.Temp_mean.daily.regrid.{wy}.{wy_daynum:03d}.pfb,,
 521,conus1_domain,pfb,topographic_index,topographic_index,,,static,-,-,conus1,,1,/hydrodata/PFCLM/CONUS1_baseline/simulations/static/CONUS1_topographic_index.pfb,,
-522,usgs_nwis,sql,water_table_depth,wtd,01/01/1801,,instantaneous,m,-,,,1,,,groundwater
+522,usgs_nwis,sql,water_table_depth,wtd,01/01/1801,,instantaneous,m,-,,,1,,,groundwater
+523,conus1_domain,tiff,flow_direction,band_data,,,static,-,-,conus1,,1,/hydrodata/PFCLM/CONUS1_baseline/other_domain_files/flow_direction.tif,"The flow directions for every grid cell (1=down, 2=left, 3=up, 4=right)",
+524,conus1_domain,pfb,flow_direction,band_data,,,static,-,-,conus1,,1,/hydrodata/PFCLM/CONUS1_baseline/other_domain_files/flow_direction.pfb,"The flow directions for every grid cell (1=down, 2=left, 3=up, 4=right)",
+525,jasechko_2024,sql,water_table_depth,wtd,1801,2022,yearly,m,median,,,1,,,groundwater
```

### Comparing `hf_hydrodata-1.1.7/src/hf_hydrodata/model/dataset.csv` & `hf_hydrodata-1.1.9/src/hf_hydrodata/model/dataset.csv`

 * *Files 6% similar despite different names*

```diff
@@ -13,7 +13,8 @@
 observations,point_observations,Observation Points (deprecated),,,,,,point,UTC-00:00,,
 obs_anomalies,point_observations,Observation Anomolies (deprecated),,,,,,point,UTC-00:00,,
 usgs_nwis,point_observations,National Water Information Service,usgs,,,,,point,UTC-00:00,,
 snotel,point_observations,Snow Telemetry,usda,,,,,point,UTC-00:00,,
 scan,point_observations,Soil Climate Analysis Network,usda,,,,,point,UTC-00:00,,
 ameriflux,point_observations,Ameriflux,ameriflux,,,,,point,UTC-00:00,,
 noaa,forcing,NOAA Climate Data,noaa,,https://www.climate.gov/maps-data/dataset/daily-temperature-and-precipitation-reports-data-tables,6/1/22,,gridded,UTC-00:00,,
+jasechko_2024,point_observations,"Jasechko et al. 2024 water table depth dataset, subset to the CONUS2 domain",jasechko_2024,10.1038/s41586-023-06879-8,https://zenodo.org/records/10003697,1801,2022,point,,,
```

### Comparing `hf_hydrodata-1.1.7/src/hf_hydrodata/model/file_type.csv` & `hf_hydrodata-1.1.9/src/hf_hydrodata/model/file_type.csv`

 * *Files identical despite different names*

### Comparing `hf_hydrodata-1.1.7/src/hf_hydrodata/model/grid.csv` & `hf_hydrodata-1.1.9/src/hf_hydrodata/model/grid.csv`

 * *Files identical despite different names*

### Comparing `hf_hydrodata-1.1.7/src/hf_hydrodata/model/substitution_keys.csv` & `hf_hydrodata-1.1.9/src/hf_hydrodata/model/substitution_keys.csv`

 * *Files identical despite different names*

### Comparing `hf_hydrodata-1.1.7/src/hf_hydrodata/model/temporal_resolution.csv` & `hf_hydrodata-1.1.9/src/hf_hydrodata/model/temporal_resolution.csv`

 * *Files 15% similar despite different names*

```diff
@@ -3,8 +3,9 @@
 hourly,Hourly,Data recorded for each hour
 monthly,Monthly,Data value stored per month
 weekly,Weekly,Data values stored per week
 static,static,Variables that do not change with time
 monthly_clim,Monthly Climatology,Long term monthly mean values
 annual_clim,Annual Climatology,Long term annual mean values
 daily_of_week,Daily Over Week,Daily values aggregated over week
-instantaneous,Instantaneous,Data values reported at a given point in time
+instantaneous,Instantaneous,Data values reported at a given point in time
+yearly,Yearly,Data values stored per calendar year
```

### Comparing `hf_hydrodata-1.1.7/src/hf_hydrodata/model/units.csv` & `hf_hydrodata-1.1.9/src/hf_hydrodata/model/units.csv`

 * *Files identical despite different names*

### Comparing `hf_hydrodata-1.1.7/src/hf_hydrodata/model/variable.csv` & `hf_hydrodata-1.1.9/src/hf_hydrodata/model/variable.csv`

 * *Files identical despite different names*

### Comparing `hf_hydrodata-1.1.7/src/hf_hydrodata/model/variable_type.csv` & `hf_hydrodata-1.1.9/src/hf_hydrodata/model/variable_type.csv`

 * *Files identical despite different names*

### Comparing `hf_hydrodata-1.1.7/src/hf_hydrodata/point.py` & `hf_hydrodata-1.1.9/src/hf_hydrodata/point.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
 # List of SQL tables in the database corresponding to site-type-specific attributes
 SITE_ATTRIBUTE_TABLES = [
     "streamgauge_attributes",
     "well_attributes",
     "snotel_station_attributes",
     "flux_tower_attributes",
+    "jasechko_attributes",
 ]
 
 
 def get_point_data(*args, **kwargs):
     """
     Collect point observations data into a Pandas DataFrame.
 
@@ -63,22 +64,22 @@
     date bounds, geography bounds, and/or the minimum number of per-site observations allowed.
     Please see the package documentation for the full set of supported combinations.
 
     Parameters
     ----------
     dataset : str, required
         Source from which requested data originated. Currently supported: 'usgs_nwis', 'snotel',
-        'scan', 'ameriflux'.
+        'scan', 'ameriflux', 'jasechko_2024'.
     variable : str, required
         Description of type of data requested. Currently supported: 'streamflow', 'water_table_depth', 'swe',
         'precipitation', 'air_temp', 'soil_moisture', 'latent_heat', 'sensible_heat',
         'downward_shortwave', 'downward_longwave', 'vapor_pressure_deficit', 'wind_speed'.
     temporal_resolution : str, required
-        Collection frequency of data requested. Currently supported: 'daily', 'hourly', and 'instantaneous'.
-        Please see the documentation for allowable combinations with `variable`.
+        Collection frequency of data requested. Currently supported: 'daily', 'hourly', 'instantaneous', and.
+        'yearly'. Please see the documentation for allowable combinations with `variable`.
     aggregation : str, required
         Additional information specifying the aggregation method for the variable to be returned.
         Options include descriptors such as 'mean' and 'sum'. Please see the documentation
         for allowable combinations with `variable`.
     depth_level : int, optional
         Depth level in inches at which the measurement is taken. Necessary for `variable` = 'soil_moisture'.
     date_start : str, optional
@@ -237,15 +238,15 @@
 
     # Get data
     site_list = list(sites_df["site_id"])
 
     if (var_id in (1, 2, 3, 4)) | (var_id in range(6, 25)):
         data_df = _get_data_nc(site_list, var_id, *args, **kwargs)
 
-    elif var_id == 5:
+    elif var_id in (5, 25):
         data_df = _get_data_sql(conn, site_list, var_id, *args, **kwargs)
 
     conn.close()
 
     return data_df.reset_index().drop("index", axis=1)
 
 
@@ -253,21 +254,22 @@
     """
     Return DataFrame with site metadata for the filtered sites.
 
     Parameters
     ----------
     dataset : str, required
         Source from which requested data originated. Currently supported: 'usgs_nwis', 'snotel',
-        'scan', 'ameriflux'.
+        'scan', 'ameriflux', 'jasechko_2024'.
     variable : str, required
         Description of type of data requested. Currently supported: 'streamflow', 'water_table_depth', 'swe',
         'precipitation', 'air_temp', 'soil_moisture', 'latent_heat', 'sensible_heat',
         'downward_shortwave', 'downward_longwave', 'vapor_pressure_deficit', 'wind_speed'.
     temporal_resolution : str, required
-        Collection frequency of data requested. Currently supported: 'daily', 'hourly', and 'instantaneous'.
+        Collection frequency of data requested. Currently supported: 'daily', 'hourly', 'instantaneous',
+        and 'yearly'.
         Please see the documentation for allowable combinations with `variable`.
     aggregation : str, required
         Additional information specifying the aggregation method for the variable to be returned.
         Options include descriptors such as 'mean' and 'sum'. Please see the documentation
         for allowable combinations with `variable`.
     depth_level : int, optional
         Depth level in inches at which the measurement is taken. Necessary for `variable` = 'soil_moisture'.
@@ -400,15 +402,17 @@
                FROM streamgauge_attributes WHERE site_id IN (%s)"""
             % ",".join("?" * len(site_ids)),
             conn,
             params=site_ids,
         )
         metadata_df = pd.merge(metadata_df, attributes_df, how="left", on="site_id")
 
-    if "groundwater well" in metadata_df["site_type"].unique():
+    if ("groundwater well" in metadata_df["site_type"].unique()) and (
+        options["dataset"] == "usgs_nwis"
+    ):
         attributes_df = pd.read_sql_query(
             """SELECT site_id, conus1_i, conus1_j, conus2_i, conus2_j,
                       nat_aqfr_cd AS usgs_nat_aqfr_cd,
                       aqfr_cd AS usgs_aqfr_cd,
                       aqfr_type_cd AS usgs_aqfr_type_cd,
                       well_depth_va AS usgs_well_depth,
                       hole_depth_va AS usgs_hole_depth,
@@ -436,14 +440,26 @@
             metadata_df = pd.merge(
                 metadata_df,
                 pd.DataFrame(data=wtd_sites_with_data, columns=["site_id"]),
                 on="site_id",
                 how="inner",
             )
 
+    if ("groundwater well" in metadata_df["site_type"].unique()) and (
+        options["dataset"] == "jasechko_2024"
+    ):
+        attributes_df = pd.read_sql_query(
+            """SELECT site_id, conus1_i, conus1_j, conus2_i, conus2_j, usgs_site
+               FROM jasechko_attributes WHERE site_id IN (%s)"""
+            % ",".join("?" * len(site_ids)),
+            conn,
+            params=site_ids,
+        )
+        metadata_df = pd.merge(metadata_df, attributes_df, how="left", on="site_id")
+
     if ("SNOTEL station" in metadata_df["site_type"].unique()) or (
         "SCAN station" in metadata_df["site_type"].unique()
     ):
         attributes_df = pd.read_sql_query(
             """SELECT site_id, conus1_i, conus1_j, conus2_i, conus2_j,
                       elevation AS usda_elevation
                FROM snotel_station_attributes WHERE site_id IN (%s)"""
@@ -598,26 +614,35 @@
 
     # Initialize parameter list to SQL queries
     param_list = []
 
     # Data source
     if "dataset" in options and options["dataset"] is not None:
         try:
-            assert options["dataset"] in ["usgs_nwis", "snotel", "scan", "ameriflux"]
+            assert options["dataset"] in [
+                "usgs_nwis",
+                "snotel",
+                "scan",
+                "ameriflux",
+                "jasechko_2024",
+            ]
         except:
             raise ValueError(
                 f"dataset must be one of 'usgs_nwis', 'snotel', 'scan', 'ameriflux'. You provided {options['dataset']}"
             )
 
         if options["dataset"] == "usgs_nwis":
             dataset_query = """ AND agency == ?"""
             param_list.append("USGS")
         elif options["dataset"] == "ameriflux":
             dataset_query = """ AND agency == ?"""
             param_list.append("AmeriFlux")
+        elif options["dataset"] == "jasechko_2024":
+            dataset_query = """ AND agency == ?"""
+            param_list.append("Jasechko_et_al_2024")
         elif options["dataset"] == "snotel":
             dataset_query = """ AND site_type == ?"""
             param_list.append("SNOTEL station")
         elif options["dataset"] == "scan":
             dataset_query = """ AND site_type == ?"""
             param_list.append("SCAN station")
     else:
@@ -1045,26 +1070,26 @@
     """
     Return a dictionary with relevant citation information.
 
     Parameters
     ----------
     dataset : str
         Source from which requested data originated. Currently supported: 'usgs_nwis', 'snotel',
-        'scan', 'ameriflux'.
+        'scan', 'ameriflux', 'jasechko_2024'.
 
     Returns
     -------
     str
         String containing overall attribution instructions for the provided dataset.
     """
     try:
-        assert dataset in ["usgs_nwis", "snotel", "scan", "ameriflux"]
+        assert dataset in ["usgs_nwis", "snotel", "scan", "ameriflux", "jasechko_2024"]
     except:
         raise ValueError(
-            f"Unexpected value of dataset, {dataset}. Supported values include 'usgs_nwis', 'snotel', 'scan', and 'ameriflux'"
+            f"Unexpected value of dataset, {dataset}. Supported values include 'usgs_nwis', 'snotel', 'scan', 'ameriflux', and 'jasechko_2024"
         )
 
     if dataset == "usgs_nwis":
         c = (
             "Most U.S. Geological Survey (USGS) information resides in Public Domain and "
             "may be used without restriction, though they do ask that proper credit be given. "
             'An example credit statement would be: "(Product or data name) courtesy of the U.S. Geological Survey".\n'
@@ -1090,14 +1115,17 @@
             'Department of Energy Office of Science." '
             "Additionally, for each AmeriFlux site used, you must provide a citation to the site "
             "data product that includes the data product DOI. The DOI for each site is included in the "
             "DataFrame returned by the hf_hydrodata get_point_metadata method, in the doi column.\n"
             "Source: https://ameriflux.lbl.gov/data/data-policy/"
         )
 
+    elif dataset == "jasechko_2024":
+        c = "Dataset DOI: 10.1038/s41586-023-06879-8"
+
     return c
 
 
 def _validate_user():
     email, pin = _get_registered_api_pin()
     url_security = f"{HYDRODATA_URL}/api/api_pins?pin={pin}&email={email}"
     response = requests.get(url_security, headers=None, timeout=15)
@@ -1147,21 +1175,22 @@
     """
     Checks on inputs to get_observations function.
 
     Parameters
     ----------
     dataset : str
         Source from which requested data originated. Currently supported: 'usgs_nwis', 'snotel',
-        'scan', 'ameriflux'.
+        'scan', 'ameriflux', 'jasechko_2024'.
     variable : str, required
         Description of type of data requested. Currently supported: 'streamflow', 'water_table_depth', 'swe',
         'precipitation', 'air_temp', 'soil_moisture', 'latent_heat', 'sensible_heat',
         'downward_shortwave', 'downward_longwave', 'vapor_pressure_deficit', 'wind_speed'.
     temporal_resolution : str
-        Collection frequency of data requested. Currently supported: 'daily', 'hourly', and 'instantaneous'.
+        Collection frequency of data requested. Currently supported: 'daily', 'hourly', 'instantaneous',
+        and 'yearly'.
     aggregation : str
         Additional information specifying the aggregation method for the variable to be returned.
         Options include descriptors such as 'mean' and 'sum'. Please see the documentation
         for allowable combinations with `variable`.
     args :
         Optional positional parameters that must be a dict with filter options.
     kwargs :
@@ -1178,15 +1207,15 @@
     """
     if len(args) > 0 and isinstance(args[0], dict):
         options = args[0]
     else:
         options = kwargs
 
     try:
-        assert temporal_resolution in ["daily", "hourly", "instantaneous"]
+        assert temporal_resolution in ["daily", "hourly", "instantaneous", "yearly"]
     except:
         raise ValueError(
             f"Unexpected value for temporal_resolution, {temporal_resolution}. Please see the documentation for allowed values."
         )
 
     try:
         assert variable in [
@@ -1207,14 +1236,15 @@
         raise ValueError(
             f"Unexpected value for variable, {variable}. Please see the documentation for allowed values."
         )
 
     try:
         assert aggregation in [
             "mean",
+            "median",
             "instantaneous",
             "-",
             "sum",
             "sum_snow_adjusted",
             "sod",
             "accumulated",
             "min",
@@ -1222,15 +1252,15 @@
         ]
     except:
         raise ValueError(
             f"Unexpected value for aggregation, {aggregation}. Please see the documentation for allowed values."
         )
 
     try:
-        assert dataset in ["usgs_nwis", "snotel", "scan", "ameriflux"]
+        assert dataset in ["usgs_nwis", "snotel", "scan", "ameriflux", "jasechko_2024"]
     except:
         raise ValueError(
             f"Unexpected value for dataset, {dataset} Please see the documentation for allowed values."
         )
 
     if variable == "soil_moisture":
         try:
@@ -1250,21 +1280,22 @@
 
     Parameters
     ----------
     conn : Connection object
         The Connection object associated with the SQLite database to query from.
     dataset : str
         Source from which requested data originated. Currently supported: 'usgs_nwis', 'snotel',
-        'scan', 'ameriflux'.
+        'scan', 'ameriflux', 'jasechko_2024'.
     variable : str, required
         Description of type of data requested. Currently supported: 'streamflow', 'water_table_depth', 'swe',
         'precipitation', 'air_temp', 'soil_moisture', 'latent_heat', 'sensible_heat',
         'downward_shortwave', 'downward_longwave', 'vapor_pressure_deficit', 'wind_speed'.
     temporal_resolution : str
-        Collection frequency of data requested. Currently supported: 'daily', 'hourly', and 'instantaneous'.
+        Collection frequency of data requested. Currently supported: 'daily', 'hourly', 'instantaneous', and
+        'yearly'.
     aggregation : str
         Additional information specifying the aggregation method for the variable to be returned.
         Options include descriptors such as 'mean' and 'sum'. Please see the documentation
         for allowable combinations with `variable`.
     args :
         Optional positional parameters that must be a dict with filter options.
     kwargs :
@@ -1388,21 +1419,22 @@
     Parameters
     ----------
     conn : Connection object
         The Connection object associated with the SQLite database to
         query from.
     dataset : str
         Source from which requested data originated. Currently supported: 'usgs_nwis', 'snotel',
-        'scan', 'ameriflux'.
+        'scan', 'ameriflux', 'jasechko_2024'.
     variable : str, required
         Description of type of data requested. Currently supported: 'streamflow', 'water_table_depth', 'swe',
         'precipitation', 'air_temp', 'soil_moisture', 'latent_heat', 'sensible_heat',
         'downward_shortwave', 'downward_longwave', 'vapor_pressure_deficit', 'wind_speed'.
     temporal_resolution : str
-        Collection frequency of data requested. Currently supported: 'daily', 'hourly', and 'instantaneous'.
+        Collection frequency of data requested. Currently supported: 'daily', 'hourly', 'instantaneous',
+        and 'yearly'.
         Please see the documentation for allowable combinations with `variable`.
     aggregation : str
         Additional information specifying the aggregation method for the variable to be returned.
         Options include descriptors such as 'mean' and 'sum'. Please see the documentation
         for allowable combinations with `variable`.
     depth_level : int, optional
         Depth level in inches at which the measurement is taken. Necessary for `variable` = 'soil_moisture'.
@@ -1516,14 +1548,16 @@
                 tbl = "streamgauge_attributes"
             elif variable == "water_table_depth":
                 tbl = "well_attributes"
         elif dataset in ("snotel", "scan"):
             tbl = "snotel_station_attributes"
         elif dataset == "ameriflux":
             tbl = "flux_tower_attributes"
+        elif dataset == "jasechko_2024":
+            tbl = "jasechko_attributes"
 
         grid = options["grid"]
         grid_bounds = options["grid_bounds"]
 
         grid_bounds_query = f"""SELECT site_id, {grid}_i, {grid}_j
                             FROM {tbl}
                             WHERE {grid}_i >= {grid_bounds[0]}
@@ -2025,15 +2059,22 @@
 
     Returns
     -------
     DataFrame
         Stacked observations data for a single variable, filtered to only sites that
         have the minimum number of observations specified.
     """
-    assert var_id == 5
+    assert var_id in (5, 25)
+    if var_id == 5:
+        tbl_name = "wtd_discrete_data"
+        var_names = "w.wtd, w.pumping_status"
+
+    elif var_id == 25:
+        tbl_name = "jasechko_wtd_data"
+        var_names = "w.wtd"
 
     if len(args) > 0 and isinstance(args[0], dict):
         options = args[0]
     else:
         options = kwargs
 
     # Note:
@@ -2041,14 +2082,26 @@
     #   pumping_status == 'P' --> Pumping
     #   pumping_status == '' --> unknown (not reported)
     if "min_num_obs" not in options or options["min_num_obs"] is None:
         min_num_obs = 1
     else:
         min_num_obs = options["min_num_obs"]
 
+    # This is a yearly variable. For date filtering to work properly, only consider the
+    # year provided in the input arguments.
+    if var_id == 25:
+        if "date_start" in options and options["date_start"] is not None:
+            options["date_start"] = datetime.datetime.strptime(
+                options["date_start"], "%Y-%m-%d"
+            ).year
+        if "date_end" in options and options["date_end"] is not None:
+            options["date_end"] = datetime.datetime.strptime(
+                options["date_end"], "%Y-%m-%d"
+            ).year
+
     if ("date_start" not in options) and ("date_end" not in options):
         date_query = """"""
         param_list = [min_num_obs]
     elif ("date_start" not in options) and ("date_end" in options):
         date_query = """ WHERE w.date <= ?"""
         param_list = [options["date_end"], min_num_obs, options["date_end"]]
     elif ("date_start" in options) and ("date_end" not in options):
@@ -2067,19 +2120,19 @@
     # Add filter for only the site IDs in site_list
     site_query = """ AND w.site_id IN (%s)""" % ",".join("?" * len(site_list))
     for s in site_list:
         param_list.append(s)
 
     # Filter on all spatial observations for the desired time range (if any)
     query = (
-        """
-            SELECT w.site_id, w.date, w.wtd, w.pumping_status
-            FROM wtd_discrete_data AS w
+        f"""
+            SELECT w.site_id, w.date, {var_names}
+            FROM {tbl_name} AS w
             INNER JOIN (SELECT w.site_id, COUNT(*) AS num_obs
-                FROM wtd_discrete_data AS w
+                FROM {tbl_name} AS w
                 """
         + date_query
         + """
                 GROUP BY site_id
                 HAVING num_obs >= ?) AS c
             ON w.site_id = c.site_id
             """
```

### Comparing `hf_hydrodata-1.1.7/src/hf_hydrodata/projection.py` & `hf_hydrodata-1.1.9/src/hf_hydrodata/projection.py`

 * *Files identical despite different names*

### Comparing `hf_hydrodata-1.1.7/src/hf_hydrodata/publish_model.py` & `hf_hydrodata-1.1.9/src/hf_hydrodata/publish_model.py`

 * *Files identical despite different names*

### Comparing `hf_hydrodata-1.1.7/PKG-INFO` & `hf_hydrodata-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hf_hydrodata
-Version: 1.1.7
+Version: 1.1.9
 Summary: hydroframe tools and utilities
 License: MIT
 Author: William M. Hasling
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

