# Comparing `tmp/pyelq_sdk-1.0.5.tar.gz` & `tmp/pyelq_sdk-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyelq_sdk-1.0.5.tar", max compression
+gzip compressed data, was "pyelq_sdk-1.0.6.tar", max compression
```

## Comparing `pyelq_sdk-1.0.5.tar` & `pyelq_sdk-1.0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    11358 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/LICENSE.md
-drwxr-xr-x   0        0        0        0 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/LICENSES/
--rw-r--r--   0        0        0    10280 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/LICENSES/Apache-2.0.txt
--rw-r--r--   0        0        0     7491 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/README.md
--rw-r--r--   0        0        0     1838 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      414 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/src/pyelq/__init__.py
--rw-r--r--   0        0        0      245 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/src/pyelq/component/__init__.py
--rw-r--r--   0        0        0    18705 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/src/pyelq/component/background.py
--rw-r--r--   0        0        0     2360 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/src/pyelq/component/component.py
--rw-r--r--   0        0        0    16261 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/src/pyelq/component/error_model.py
--rw-r--r--   0        0        0     7718 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/src/pyelq/component/offset.py
--rw-r--r--   0        0        0    37479 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/src/pyelq/component/source_model.py
--rw-r--r--   0        0        0    22281 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/src/pyelq/coordinate_system.py
--rw-r--r--   0        0        0      186 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/src/pyelq/data_access/__init__.py
--rw-r--r--   0        0        0     3973 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/src/pyelq/data_access/data_access.py
--rw-r--r--   0        0        0      194 2024-05-27 13:28:42.300979 pyelq_sdk-1.0.5/src/pyelq/dispersion_model/__init__.py
--rw-r--r--   0        0        0    31586 2024-05-27 13:28:42.304979 pyelq_sdk-1.0.5/src/pyelq/dispersion_model/gaussian_plume.py
--rw-r--r--   0        0        0    25293 2024-05-27 13:28:42.304979 pyelq_sdk-1.0.5/src/pyelq/dlm.py
--rw-r--r--   0        0        0     6504 2024-05-27 13:28:42.304979 pyelq_sdk-1.0.5/src/pyelq/gas_species.py
--rw-r--r--   0        0        0    13207 2024-05-27 13:28:42.304979 pyelq_sdk-1.0.5/src/pyelq/meteorology.py
--rw-r--r--   0        0        0     9173 2024-05-27 13:28:42.304979 pyelq_sdk-1.0.5/src/pyelq/model.py
--rw-r--r--   0        0        0      176 2024-05-27 13:28:42.304979 pyelq_sdk-1.0.5/src/pyelq/plotting/__init__.py
--rw-r--r--   0        0        0    58335 2024-05-27 13:28:42.304979 pyelq_sdk-1.0.5/src/pyelq/plotting/plot.py
--rw-r--r--   0        0        0    12658 2024-05-27 13:28:42.304979 pyelq_sdk-1.0.5/src/pyelq/preprocessing.py
--rw-r--r--   0        0        0      197 2024-05-27 13:28:42.304979 pyelq_sdk-1.0.5/src/pyelq/sensor/__init__.py
--rw-r--r--   0        0        0     1806 2024-05-27 13:28:42.304979 pyelq_sdk-1.0.5/src/pyelq/sensor/beam.py
--rw-r--r--   0        0        0     2316 2024-05-27 13:28:42.304979 pyelq_sdk-1.0.5/src/pyelq/sensor/satellite.py
--rw-r--r--   0        0        0     9190 2024-05-27 13:28:42.304979 pyelq_sdk-1.0.5/src/pyelq/sensor/sensor.py
--rw-r--r--   0        0        0     5741 2024-05-27 13:28:42.304979 pyelq_sdk-1.0.5/src/pyelq/source_map.py
--rw-r--r--   0        0        0      210 2024-05-27 13:28:42.304979 pyelq_sdk-1.0.5/src/pyelq/support_functions/__init__.py
--rw-r--r--   0        0        0    10609 2024-05-27 13:28:42.304979 pyelq_sdk-1.0.5/src/pyelq/support_functions/spatio_temporal_interpolation.py
--rw-r--r--   0        0        0     8437 1970-01-01 00:00:00.000000 pyelq_sdk-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/LICENSE.md
+drwxr-xr-x   0        0        0        0 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/LICENSES/
+-rw-r--r--   0        0        0    10280 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/LICENSES/Apache-2.0.txt
+-rw-r--r--   0        0        0     7491 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/README.md
+-rw-r--r--   0        0        0     1838 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      414 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/src/pyelq/__init__.py
+-rw-r--r--   0        0        0      245 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/src/pyelq/component/__init__.py
+-rw-r--r--   0        0        0    18705 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/src/pyelq/component/background.py
+-rw-r--r--   0        0        0     2360 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/src/pyelq/component/component.py
+-rw-r--r--   0        0        0    16261 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/src/pyelq/component/error_model.py
+-rw-r--r--   0        0        0     7718 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/src/pyelq/component/offset.py
+-rw-r--r--   0        0        0    37479 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/src/pyelq/component/source_model.py
+-rw-r--r--   0        0        0    22281 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/src/pyelq/coordinate_system.py
+-rw-r--r--   0        0        0      186 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/src/pyelq/data_access/__init__.py
+-rw-r--r--   0        0        0     3973 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/src/pyelq/data_access/data_access.py
+-rw-r--r--   0        0        0      194 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/src/pyelq/dispersion_model/__init__.py
+-rw-r--r--   0        0        0    31586 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/src/pyelq/dispersion_model/gaussian_plume.py
+-rw-r--r--   0        0        0    25293 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/src/pyelq/dlm.py
+-rw-r--r--   0        0        0     6504 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/src/pyelq/gas_species.py
+-rw-r--r--   0        0        0    16959 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/src/pyelq/meteorology.py
+-rw-r--r--   0        0        0     9173 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/src/pyelq/model.py
+-rw-r--r--   0        0        0      176 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/src/pyelq/plotting/__init__.py
+-rw-r--r--   0        0        0    58335 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/src/pyelq/plotting/plot.py
+-rw-r--r--   0        0        0    12658 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/src/pyelq/preprocessing.py
+-rw-r--r--   0        0        0      197 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/src/pyelq/sensor/__init__.py
+-rw-r--r--   0        0        0     1806 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/src/pyelq/sensor/beam.py
+-rw-r--r--   0        0        0     2316 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/src/pyelq/sensor/satellite.py
+-rw-r--r--   0        0        0     9190 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/src/pyelq/sensor/sensor.py
+-rw-r--r--   0        0        0     5741 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/src/pyelq/source_map.py
+-rw-r--r--   0        0        0      210 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/src/pyelq/support_functions/__init__.py
+-rw-r--r--   0        0        0    10609 2024-05-31 12:58:47.948449 pyelq_sdk-1.0.6/src/pyelq/support_functions/spatio_temporal_interpolation.py
+-rw-r--r--   0        0        0     8437 1970-01-01 00:00:00.000000 pyelq_sdk-1.0.6/PKG-INFO
```

### Comparing `pyelq_sdk-1.0.5/LICENSE.md` & `pyelq_sdk-1.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.5/LICENSES/Apache-2.0.txt` & `pyelq_sdk-1.0.6/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.5/README.md` & `pyelq_sdk-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.5/pyproject.toml` & `pyelq_sdk-1.0.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pyelq-sdk"
-version = "1.0.5"
+version = "1.0.6"
 description = "Package for detection, localization and quantification code."
 authors = ["Bas van de Kerkhof", "Matthew Jones", "David Randell"]
 homepage = "https://sede-open.github.io/pyELQ/"
 repository = "https://github.com/sede-open/pyELQ"
 documentation = "https://sede-open.github.io/pyELQ/"
 readme = "README.md"
 license = "Apache-2.0"
```

### Comparing `pyelq_sdk-1.0.5/src/pyelq/component/background.py` & `pyelq_sdk-1.0.6/src/pyelq/component/background.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.5/src/pyelq/component/component.py` & `pyelq_sdk-1.0.6/src/pyelq/component/component.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.5/src/pyelq/component/error_model.py` & `pyelq_sdk-1.0.6/src/pyelq/component/error_model.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.5/src/pyelq/component/offset.py` & `pyelq_sdk-1.0.6/src/pyelq/component/offset.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.5/src/pyelq/component/source_model.py` & `pyelq_sdk-1.0.6/src/pyelq/component/source_model.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.5/src/pyelq/coordinate_system.py` & `pyelq_sdk-1.0.6/src/pyelq/coordinate_system.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.5/src/pyelq/data_access/data_access.py` & `pyelq_sdk-1.0.6/src/pyelq/data_access/data_access.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.5/src/pyelq/dispersion_model/gaussian_plume.py` & `pyelq_sdk-1.0.6/src/pyelq/dispersion_model/gaussian_plume.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.5/src/pyelq/dlm.py` & `pyelq_sdk-1.0.6/src/pyelq/dlm.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.5/src/pyelq/gas_species.py` & `pyelq_sdk-1.0.6/src/pyelq/gas_species.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.5/src/pyelq/meteorology.py` & `pyelq_sdk-1.0.6/src/pyelq/meteorology.py`

 * *Files 14% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 
     def plot_polar_hist(self, nof_sectors: int = 16, nof_divisions: int = 5, template: object = None) -> go.Figure():
         """Plots a histogram of wind speed and wind direction in polar Coordinates.
 
         Args:
             nof_sectors (int, optional): The number of wind direction sectors into which the data is binned.
             nof_divisions (int, optional): The number of wind speed divisions into which the data is binned.
-            template (go.update_layout): A layout template which can be applied to the plot. Defaults to None.
+            template (object): A layout template which can be applied to the plot. Defaults to None.
 
         Returns:
             fig (go.Figure): A plotly go figure containing the trace of the rose plot.
 
         """
         sector_half_width = 0.5 * (360 / nof_sectors)
         wind_direction_bin_edges = np.linspace(-sector_half_width, 360 - sector_half_width, nof_sectors + 1)
@@ -191,21 +191,27 @@
 
         fig.update_layout(polar=polar_dict)
         fig.update_layout(template=template)
         fig.update_layout(title="Distribution of Wind Speeds and Directions")
 
         return fig
 
-    def plot_polar_scatter(self, fig, sensor_object: SensorGroup, template: object = None) -> go.Figure():
+    def plot_polar_scatter(self, fig: go.Figure, sensor_object: SensorGroup, template: object = None) -> go.Figure():
         """Plots a scatter plot of concentration with respect to wind direction in polar Coordinates.
 
+        This function implements the polar scatter functionality for a (single) Meteorology object. Assuming the all
+        Sensors in the SensorGroup are consistent with the Meteorology object.
+
+        Note we do plot the sensors which do not contain any values when present in the SensorGroup to keep consistency
+        in plot colors.
+
         Args:
             fig (go.Figure): A plotly figure onto which traces can be drawn.
             sensor_object (SensorGroup): SensorGroup object which contains the concentration information
-            template (go.update_layout): A layout template which can be applied to the plot. Defaults to None.
+            template (object): A layout template which can be applied to the plot. Defaults to None.
 
         Returns:
             fig (go.Figure): A plotly go figure containing the trace of the rose plot.
 
         """
         max_concentration = 0
 
@@ -214,61 +220,29 @@
                 warnings.warn(
                     f"Concentration values for sensor {sensor_key} are of shape "
                     + f"{sensor.concentration.shape}, but self.wind_direction has shape "
                     + f"{self.wind_direction.shape}. It will not be plotted on the polar scatter plot."
                 )
             else:
                 theta = self.wind_direction
+                color_idx = i % len(sensor_object.color_map)
 
                 fig.add_trace(
                     go.Scatterpolar(
                         r=sensor.concentration,
                         theta=theta,
                         mode="markers",
                         name=sensor_key,
-                        marker={"color": sensor_object.color_map[i]},
+                        marker={"color": sensor_object.color_map[color_idx]},
                     )
                 )
+                if sensor.concentration.size > 0:
+                    max_concentration = np.maximum(np.nanmax(sensor.concentration), max_concentration)
 
-                max_concentration = np.maximum(np.nanmax(sensor.concentration), max_concentration)
-
-        ticktext = ["N", "NE", "E", "SE", "S", "SW", "W", "NW"]
-        polar_dict = {
-            "radialaxis": {"tickangle": 0, "range": [0.0, 1.01 * max_concentration]},
-            "radialaxis_angle": 0,
-            "angularaxis": {
-                "tickmode": "array",
-                "ticktext": ticktext,
-                "direction": "clockwise",
-                "rotation": 90,
-                "tickvals": list(np.linspace(0, 360 - (360 / 8), 8)),
-            },
-        }
-
-        fig.add_annotation(
-            x=1,
-            y=1,
-            yref="paper",
-            xref="paper",
-            xanchor="right",
-            yanchor="top",
-            align="left",
-            font={"size": 18, "color": "#000000"},
-            showarrow=False,
-            borderwidth=2,
-            borderpad=10,
-            bgcolor="#ffffff",
-            bordercolor="#000000",
-            opacity=0.8,
-            text="<b>Radial Axis:</b> Wind<br>speed in m/s.",
-        )
-
-        fig.update_layout(polar=polar_dict)
-        fig.update_layout(template=template)
-        fig.update_layout(title="Measured Concentration against Wind Direction.")
+        fig = set_plot_polar_scatter_layout(max_concentration=max_concentration, fig=fig, template=template)
 
         return fig
 
 
 @dataclass
 class MeteorologyGroup(dict):
     """A dictionary containing multiple Meteorology objects.
@@ -297,7 +271,113 @@
         for met in self.values():
             met.calculate_wind_direction_from_uv()
 
     def calculate_wind_speed_from_uv(self):
         """Calculate wind speed from the u and v components for each member of the group."""
         for met in self.values():
             met.calculate_wind_speed_from_uv()
+
+    def plot_polar_scatter(self, fig: go.Figure, sensor_object: SensorGroup, template: object = None) -> go.Figure():
+        """Plots a scatter plot of concentration with respect to wind direction in polar coordinates.
+
+        This function implements the polar scatter functionality for a MeteorologyGroup object. It assumes each object
+        in the SensorGroup has an associated Meteorology object in the MeteorologyGroup.
+
+        Note we do plot the sensors which do not contain any values when present in the SensorGroup to keep consistency
+        in plot colors.
+
+        Args:
+            fig (go.Figure): A plotly figure onto which traces can be drawn.
+            sensor_object (SensorGroup): SensorGroup object which contains the concentration information
+            template (object): A layout template which can be applied to the plot. Defaults to None.
+
+        Returns:
+            fig (go.Figure): A plotly go figure containing the trace of the rose plot.
+
+        Raises
+            ValueError: When there is a sensor key which is not present in the MeteorologyGroup.
+
+        """
+        max_concentration = 0
+
+        for i, (sensor_key, sensor) in enumerate(sensor_object.items()):
+            if sensor_key not in self.keys():
+                raise ValueError(f"Key {sensor_key} not found in MeteorologyGroup.")
+            temp_met_object = self[sensor_key]
+            if sensor.concentration.shape != temp_met_object.wind_direction.shape:
+                warnings.warn(
+                    f"Concentration values for sensor {sensor_key} are of shape "
+                    + f"{sensor.concentration.shape}, but wind_direction values for meteorology object {sensor_key} "
+                    f"has shape {temp_met_object.wind_direction.shape}. It will not be plotted on the polar scatter "
+                    f"plot."
+                )
+            else:
+                theta = temp_met_object.wind_direction
+                color_idx = i % len(sensor_object.color_map)
+
+                fig.add_trace(
+                    go.Scatterpolar(
+                        r=sensor.concentration,
+                        theta=theta,
+                        mode="markers",
+                        name=sensor_key,
+                        marker={"color": sensor_object.color_map[color_idx]},
+                    )
+                )
+
+                if sensor.concentration.size > 0:
+                    max_concentration = np.maximum(np.nanmax(sensor.concentration), max_concentration)
+
+        fig = set_plot_polar_scatter_layout(max_concentration=max_concentration, fig=fig, template=template)
+
+        return fig
+
+
+def set_plot_polar_scatter_layout(max_concentration: float, fig: go.Figure(), template: object) -> go.Figure:
+    """Helper function to set the layout of the polar scatter plot.
+
+    Helps avoid code duplication.
+
+    Args:
+        max_concentration (float): The maximum concentration value used to update radial axis range.
+        fig (go.Figure): A plotly figure onto which traces can be drawn.
+        template (object): A layout template which can be applied to the plot.
+
+    Returns:
+        fig (go.Figure): A plotly go figure containing the trace of the rose plot.
+
+    """
+    ticktext = ["N", "NE", "E", "SE", "S", "SW", "W", "NW"]
+    polar_dict = {
+        "radialaxis": {"tickangle": 0, "range": [0.0, 1.01 * max_concentration]},
+        "radialaxis_angle": 0,
+        "angularaxis": {
+            "tickmode": "array",
+            "ticktext": ticktext,
+            "direction": "clockwise",
+            "rotation": 90,
+            "tickvals": list(np.linspace(0, 360 - (360 / 8), 8)),
+        },
+    }
+
+    fig.add_annotation(
+        x=1,
+        y=1,
+        yref="paper",
+        xref="paper",
+        xanchor="right",
+        yanchor="top",
+        align="left",
+        font={"size": 18, "color": "#000000"},
+        showarrow=False,
+        borderwidth=2,
+        borderpad=10,
+        bgcolor="#ffffff",
+        bordercolor="#000000",
+        opacity=0.8,
+        text="<b>Radial Axis:</b> Wind<br>speed in m/s.",
+    )
+
+    fig.update_layout(polar=polar_dict)
+    fig.update_layout(template=template)
+    fig.update_layout(title="Measured Concentration against Wind Direction.")
+    return fig
```

### Comparing `pyelq_sdk-1.0.5/src/pyelq/model.py` & `pyelq_sdk-1.0.6/src/pyelq/model.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.5/src/pyelq/plotting/plot.py` & `pyelq_sdk-1.0.6/src/pyelq/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.5/src/pyelq/preprocessing.py` & `pyelq_sdk-1.0.6/src/pyelq/preprocessing.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.5/src/pyelq/sensor/beam.py` & `pyelq_sdk-1.0.6/src/pyelq/sensor/beam.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.5/src/pyelq/sensor/satellite.py` & `pyelq_sdk-1.0.6/src/pyelq/sensor/satellite.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.5/src/pyelq/sensor/sensor.py` & `pyelq_sdk-1.0.6/src/pyelq/sensor/sensor.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.5/src/pyelq/source_map.py` & `pyelq_sdk-1.0.6/src/pyelq/source_map.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.5/src/pyelq/support_functions/spatio_temporal_interpolation.py` & `pyelq_sdk-1.0.6/src/pyelq/support_functions/spatio_temporal_interpolation.py`

 * *Files identical despite different names*

### Comparing `pyelq_sdk-1.0.5/PKG-INFO` & `pyelq_sdk-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyelq-sdk
-Version: 1.0.5
+Version: 1.0.6
 Summary: Package for detection, localization and quantification code.
 Home-page: https://sede-open.github.io/pyELQ/
 License: Apache-2.0
 Keywords: gas dispersion,emission,detection,localization,quantification
 Author: Bas van de Kerkhof
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
```

