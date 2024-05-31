# Comparing `tmp/sdss_cherno-0.6.9.tar.gz` & `tmp/sdss_cherno-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_cherno-0.6.9.tar", max compression
+gzip compressed data, was "sdss_cherno-1.0.0.tar", max compression
```

## Comparing `sdss_cherno-0.6.9.tar` & `sdss_cherno-1.0.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1504 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/LICENSE.md
--rw-r--r--   0        0        0     2723 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/README.md
--rw-r--r--   0        0        0     1251 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/__init__.py
--rw-r--r--   0        0        0     2188 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/__main__.py
--rw-r--r--   0        0        0      747 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/actor/__init__.py
--rw-r--r--   0        0        0     4729 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/actor/actor.py
--rw-r--r--   0        0        0        0 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/actor/commands/__init__.py
--rw-r--r--   0        0        0     1746 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/actor/commands/acquire.py
--rw-r--r--   0        0        0     4938 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/actor/commands/config.py
--rw-r--r--   0        0        0    10565 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/actor/commands/guide.py
--rw-r--r--   0        0        0     1273 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/actor/commands/offset.py
--rw-r--r--   0        0        0     1008 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/actor/commands/reprocess.py
--rw-r--r--   0        0        0     2298 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/actor/commands/scale.py
--rw-r--r--   0        0        0     3511 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/actor/commands/set.py
--rw-r--r--   0        0        0     1049 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/actor/commands/show.py
--rw-r--r--   0        0        0     1964 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/actor/commands/status.py
--rw-r--r--   0        0        0      778 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/actor/commands/stop.py
--rw-r--r--   0        0        0     1148 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/actor/commands/version.py
--rw-r--r--   0        0        0    10858 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/actor/exposer.py
--rw-r--r--   0        0        0       73 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/etc/astrometrynet_APO.cfg
--rw-r--r--   0        0        0       73 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/etc/astrometrynet_LCO.cfg
--rw-r--r--   0        0        0     2210 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/etc/cherno_APO.yml
--rw-r--r--   0        0        0     2145 2024-04-18 16:20:09.393807 sdss_cherno-0.6.9/cherno/etc/cherno_LCO.yml
--rw-r--r--   0        0        0     5688 2024-04-18 16:20:09.397807 sdss_cherno-0.6.9/cherno/etc/schema.json
--rw-r--r--   0        0        0     1233 2024-04-18 16:20:09.397807 sdss_cherno-0.6.9/cherno/exceptions.py
--rw-r--r--   0        0        0    14028 2024-04-18 16:20:09.397807 sdss_cherno-0.6.9/cherno/extraction.py
--rw-r--r--   0        0        0    42948 2024-04-18 16:20:09.397807 sdss_cherno-0.6.9/cherno/guider.py
--rw-r--r--   0        0        0     4175 2024-04-18 16:20:09.397807 sdss_cherno-0.6.9/cherno/lcotcc.py
--rw-r--r--   0        0        0     1394 2024-04-18 16:20:09.397807 sdss_cherno-0.6.9/cherno/maskbits.py
--rw-r--r--   0        0        0     4738 2024-04-18 16:20:09.397807 sdss_cherno-0.6.9/cherno/tcc.py
--rw-r--r--   0        0        0     6237 2024-04-18 16:20:09.397807 sdss_cherno-0.6.9/cherno/utils.py
--rw-r--r--   0        0        0     2476 2024-04-18 16:20:09.397807 sdss_cherno-0.6.9/pyproject.toml
--rw-r--r--   0        0        0     4133 1970-01-01 00:00:00.000000 sdss_cherno-0.6.9/PKG-INFO
+-rw-r--r--   0        0        0     1504 2020-01-30 05:13:05.000000 sdss_cherno-1.0.0/LICENSE.md
+-rw-r--r--   0        0        0     2723 2023-04-27 15:46:07.696857 sdss_cherno-1.0.0/README.md
+-rw-r--r--   0        0        0     1251 2024-05-13 20:11:32.490515 sdss_cherno-1.0.0/cherno/__init__.py
+-rw-r--r--   0        0        0     2188 2024-05-13 20:11:30.623722 sdss_cherno-1.0.0/cherno/__main__.py
+-rw-r--r--   0        0        0      747 2024-05-13 20:11:39.315311 sdss_cherno-1.0.0/cherno/actor/__init__.py
+-rw-r--r--   0        0        0     5592 2024-05-20 21:36:42.086547 sdss_cherno-1.0.0/cherno/actor/actor.py
+-rw-r--r--   0        0        0        0 2022-12-31 00:58:46.900178 sdss_cherno-1.0.0/cherno/actor/commands/__init__.py
+-rw-r--r--   0        0        0     1746 2024-05-13 20:12:01.073516 sdss_cherno-1.0.0/cherno/actor/commands/acquire.py
+-rw-r--r--   0        0        0     4938 2024-05-13 20:11:57.614412 sdss_cherno-1.0.0/cherno/actor/commands/config.py
+-rw-r--r--   0        0        0    10565 2024-05-20 21:36:42.087002 sdss_cherno-1.0.0/cherno/actor/commands/guide.py
+-rw-r--r--   0        0        0     1273 2024-05-13 20:11:53.466267 sdss_cherno-1.0.0/cherno/actor/commands/offset.py
+-rw-r--r--   0        0        0     1008 2024-05-13 20:11:51.642344 sdss_cherno-1.0.0/cherno/actor/commands/reprocess.py
+-rw-r--r--   0        0        0     2298 2024-05-13 20:11:49.942973 sdss_cherno-1.0.0/cherno/actor/commands/scale.py
+-rw-r--r--   0        0        0     3511 2024-05-13 20:11:48.326220 sdss_cherno-1.0.0/cherno/actor/commands/set.py
+-rw-r--r--   0        0        0     1049 2024-05-13 20:11:46.500780 sdss_cherno-1.0.0/cherno/actor/commands/show.py
+-rw-r--r--   0        0        0     1964 2024-05-13 20:11:44.140651 sdss_cherno-1.0.0/cherno/actor/commands/status.py
+-rw-r--r--   0        0        0      778 2024-05-13 20:11:42.500523 sdss_cherno-1.0.0/cherno/actor/commands/stop.py
+-rw-r--r--   0        0        0     1148 2024-05-13 20:11:41.052204 sdss_cherno-1.0.0/cherno/actor/commands/version.py
+-rw-r--r--   0        0        0    10858 2024-05-13 20:11:35.221400 sdss_cherno-1.0.0/cherno/actor/exposer.py
+-rw-r--r--   0        0        0       73 2022-09-11 21:16:25.900130 sdss_cherno-1.0.0/cherno/etc/astrometrynet_APO.cfg
+-rw-r--r--   0        0        0       73 2022-11-07 20:29:49.539178 sdss_cherno-1.0.0/cherno/etc/astrometrynet_LCO.cfg
+-rw-r--r--   0        0        0     3619 2024-05-20 21:36:42.088845 sdss_cherno-1.0.0/cherno/etc/cherno_APO.yml
+-rw-r--r--   0        0        0     3554 2024-05-20 21:36:42.090304 sdss_cherno-1.0.0/cherno/etc/cherno_LCO.yml
+-rw-r--r--   0        0        0     5688 2023-04-25 16:01:12.321758 sdss_cherno-1.0.0/cherno/etc/schema.json
+-rw-r--r--   0        0        0     1233 2024-05-13 20:11:28.810687 sdss_cherno-1.0.0/cherno/exceptions.py
+-rw-r--r--   0        0        0    14928 2024-05-20 21:36:42.093199 sdss_cherno-1.0.0/cherno/extraction.py
+-rw-r--r--   0        0        0    55107 2024-05-31 00:20:18.297612 sdss_cherno-1.0.0/cherno/guider.py
+-rw-r--r--   0        0        0     4175 2023-04-25 16:01:12.324097 sdss_cherno-1.0.0/cherno/lcotcc.py
+-rw-r--r--   0        0        0     1394 2022-12-28 21:44:43.126066 sdss_cherno-1.0.0/cherno/maskbits.py
+-rw-r--r--   0        0        0     4738 2024-05-13 20:11:23.893914 sdss_cherno-1.0.0/cherno/tcc.py
+-rw-r--r--   0        0        0     6237 2024-05-13 20:11:26.235150 sdss_cherno-1.0.0/cherno/utils.py
+-rw-r--r--   0        0        0     2477 2024-05-31 00:42:06.714318 sdss_cherno-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4134 1970-01-01 00:00:00.000000 sdss_cherno-1.0.0/PKG-INFO
```

### Comparing `sdss_cherno-0.6.9/LICENSE.md` & `sdss_cherno-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.9/README.md` & `sdss_cherno-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.9/cherno/__init__.py` & `sdss_cherno-1.0.0/cherno/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.9/cherno/__main__.py` & `sdss_cherno-1.0.0/cherno/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.9/cherno/actor/__init__.py` & `sdss_cherno-1.0.0/cherno/actor/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.9/cherno/actor/actor.py` & `sdss_cherno-1.0.0/cherno/actor/actor.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,15 +29,21 @@
 
 class ChernoActor(clu.LegacyActor):
     """The Cherno SDSS-style actor."""
 
     def __init__(self, *args, **kwargs):
         self.observatory: str = config["observatory"].upper()
 
-        models = list(set(kwargs.pop("models", []) + ["fliswarm"]))
+        _models = ["fliswarm"]
+        if self.observatory == "APO":
+            _models.append("boss")
+        elif self.observatory == "LCO":
+            _models.append("yao")
+
+        models = list(set(kwargs.pop("models", []) + _models))
 
         schema = kwargs.pop("schema", None)
         if schema is not None and os.path.isabs(schema) is False:
             schema = os.path.join(os.path.dirname(cherno.__file__), schema)
 
         super().__init__(
             *args,
@@ -66,14 +72,32 @@
             temperature = float(key.value[16])
             if camera_name not in camera_state:
                 camera_state[camera_name] = CameraState(camera_name)
             camera_state[camera_name].temperature = temperature
         else:
             pass
 
+    def _process_boss_status(self):
+        exposing = False
+        expNum = -999
+
+        if self.observatory == "APO":
+            values = self.models["boss"]["exposureState"].value
+            if len(values) > 0 and values[0] == "INTEGRATING":
+                exposing = True
+                # Get the current exposure number
+                expNum = int(self.models["boss"]["exposureId"].value[0]) + 1
+        else:
+            values = self.models["yao"]["sp2_status_names"].value
+            if len(values) > 0 and "EXPOSING" in values:
+                exposing = True
+                expNum = int(self.models["yao"]["next_exposure_no"].value[0])
+
+        return exposing, expNum
+
 
 @dataclass
 class ChernoState:
     """Stores the state of the guider."""
 
     actor: ChernoActor
     status: GuiderStatus = GuiderStatus.IDLE
```

### Comparing `sdss_cherno-0.6.9/cherno/actor/commands/acquire.py` & `sdss_cherno-1.0.0/cherno/actor/commands/acquire.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.9/cherno/actor/commands/config.py` & `sdss_cherno-1.0.0/cherno/actor/commands/config.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.9/cherno/actor/commands/guide.py` & `sdss_cherno-1.0.0/cherno/actor/commands/guide.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,15 +239,15 @@
             if current_exposure_time >= max_exposure_time:
                 # This should only happen if the observer manually set the
                 # exposure time, in which case we accept it.
                 new_exposure_time = current_exposure_time
             elif not ast_solution.valid_solution:
                 new_exposure_time = min(current_exposure_time * 2, max_exposure_time)
             elif ast_solution.n_solved < 4:
-                new_exposure_time = max(current_exposure_time * 1.5, max_exposure_time)
+                new_exposure_time = min(current_exposure_time * 1.5, max_exposure_time)
             else:
                 new_exposure_time = current_exposure_time
 
             if new_exposure_time != round(current_exposure_time, 1):
                 command.actor.state.exposure_time = new_exposure_time
                 command.info(f"Exposure time updated to {new_exposure_time:.1f} s.")
```

### Comparing `sdss_cherno-0.6.9/cherno/actor/commands/offset.py` & `sdss_cherno-1.0.0/cherno/actor/commands/offset.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.9/cherno/actor/commands/reprocess.py` & `sdss_cherno-1.0.0/cherno/actor/commands/reprocess.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.9/cherno/actor/commands/scale.py` & `sdss_cherno-1.0.0/cherno/actor/commands/scale.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.9/cherno/actor/commands/set.py` & `sdss_cherno-1.0.0/cherno/actor/commands/set.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.9/cherno/actor/commands/show.py` & `sdss_cherno-1.0.0/cherno/actor/commands/show.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.9/cherno/actor/commands/status.py` & `sdss_cherno-1.0.0/cherno/actor/commands/status.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.9/cherno/actor/commands/stop.py` & `sdss_cherno-1.0.0/cherno/actor/commands/stop.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.9/cherno/actor/commands/version.py` & `sdss_cherno-1.0.0/cherno/actor/commands/version.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.9/cherno/actor/exposer.py` & `sdss_cherno-1.0.0/cherno/actor/exposer.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.9/cherno/etc/schema.json` & `sdss_cherno-1.0.0/cherno/etc/schema.json`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.9/cherno/exceptions.py` & `sdss_cherno-1.0.0/cherno/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.9/cherno/extraction.py` & `sdss_cherno-1.0.0/cherno/extraction.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,27 @@
 
 seaborn.set_theme(style="white")
 
 
 PathLike = TypeVar("PathLike", pathlib.Path, str)
 
 
+def apply_calibs(data, bias_path, dark_path, flat_path, gain, exptime):
+    with fits.open(bias_path) as ff:
+        bias = ff[0].data
+    with fits.open(dark_path) as ff:
+        dark = ff[0].data / gain
+    with fits.open(flat_path) as ff:
+        flat = ff[0].data
+    data = data - bias
+    data = data - dark * exptime
+    data = data / flat
+    return data
+
+
 @dataclass
 class ExtractionData:
     """Data from extraction."""
 
     image: str
     path: pathlib.Path
     camera: str
@@ -57,14 +70,16 @@
     field_pa: float
     algorithm: str
     regions: pandas.DataFrame = field(default_factory=pandas.DataFrame)
     nregions: int = 0
     nvalid: int = 0
     fwhm_median: float = -999.0
     focus_offset: float = 0.0
+    gain: float = 1
+    exptime: float = 15
 
 
 class Extraction:
     """Extract centroids and PSF information from an image."""
 
     __VALID_METHODS = ["sextractor", "marginal"]
 
@@ -89,15 +104,14 @@
         if self.method not in self.__VALID_METHODS:
             raise ValueError(
                 f"Invalid star finder. Valid values are {self.__VALID_METHODS}."
             )
 
     def process(self, image: PathLike, plot: bool | None = None) -> ExtractionData:
         """Process an image."""
-
         hdu = fits.open(image)
         data = hdu[1].data
         header = hdu[1].header
 
         camera = header["CAMNAME"][0:-1]  # Remove the n/s at the end of the camera name
         observatory = header["OBSERVAT"]
 
@@ -112,14 +126,23 @@
         if match := re.match(r".*gimg\-gfa(\d)[ns]\-(\d+)\.fits", path.parts[-1]):
             cam_no = int(match.group(1))
             exp_no = int(match.group(2))
         else:
             cam_no = 0
             exp_no = 0
 
+        data = apply_calibs(
+            data,
+            config["calib"][camera]["bias"],
+            config["calib"][camera]["dark"],
+            config["calib"][camera]["flat"],
+            header["GAIN"],
+            header["EXPTIMEN"],
+        )
+
         if plot is None:
             plot = config["extraction"]["plot"]
 
         if self.method == "sextractor":
             regions = self._process_sextractor(data, path, plot=plot)[0]
         elif self.method == "marginal":
             regions = self._process_marginal(data, path, plot=plot)
@@ -162,21 +185,22 @@
             field_pa=header["FIELDPA"],
             algorithm=self.method,
             regions=regions,
             nregions=len(regions),
             nvalid=sum(regions.valid == 1),
             fwhm_median=fwhm_median_round,
             focus_offset=config["cameras"]["focus_offset"][camera],
+            gain=header["GAIN"],
+            exptime=header["EXPTIMEN"],
         )
 
         output_file = self._get_output_path(path).with_suffix(".csv")
         output_file.unlink(missing_ok=True)
 
         regions.to_csv(str(output_file))
-
         return extraction_data
 
     def multiprocess(
         self,
         images: list[PathLike],
         n_cpus: int | None = None,
     ) -> list[ExtractionData]:
@@ -290,21 +314,25 @@
         plot_path = str(output_root) + "-marginal.pdf" if plot else None
 
         # Build an empty DF with the expected  columns to return in case
         # extract_marginal fails.
         default_columns = ["x1", "y1", "flux", "fwhm", "valid"]
         mock_regions = pandas.DataFrame([], columns=default_columns)
 
+        # Calculate a 5 arcsecond radius in pixels for aperture photometry
+        aper_radius = 5.0 / config["pixel_scale"]
+
         try:
             regions = extract_marginal(
                 data,
                 marginal_params["background_sigma"],
                 sextractor_quick_options={"minarea": marginal_params["minarea"]},
                 max_detections=marginal_params.get("max_detections", None),
                 plot=plot_path,
+                aper_radius=aper_radius,
             )
         except Exception as err:
             warnings.warn(f"extract_marginal failed with error: {err}", UserWarning)
             return mock_regions
 
         if len(regions) == 0:
             return mock_regions
```

### Comparing `sdss_cherno-0.6.9/cherno/guider.py` & `sdss_cherno-1.0.0/cherno/guider.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,22 +5,25 @@
 # @Date: 2022-02-07
 # @Filename: guider.py
 # @License: BSD 3-clause (http://www.opensource.org/licenses/BSD-3-Clause)
 
 from __future__ import annotations
 
 import asyncio
+import multiprocessing as mp
+import os
 import pathlib
 import re
 import time
 import warnings
+from concurrent.futures import ProcessPoolExecutor
 from dataclasses import dataclass, field
 from functools import partial
 
-from typing import TYPE_CHECKING, Any, Coroutine
+from typing import TYPE_CHECKING, Any, Coroutine, Literal
 
 import numpy
 import pandas
 from astropy.io import fits
 from astropy.stats.sigma_clipping import SigmaClip
 from astropy.table import Table
 from astropy.wcs import WCS, FITSFixedWarning
@@ -28,36 +31,41 @@
 
 from clu.command import FakeCommand
 from coordio import calibration, defaults
 from coordio.astrometry import AstrometryNet
 from coordio.guide import (
     GuiderFit,
     GuiderFitter,
+    SolvePointing,
     cross_match,
     gfa_to_radec,
     radec_to_gfa,
 )
 
 from cherno import config, log
 from cherno.exceptions import ChernoError
-from cherno.extraction import Extraction, ExtractionData, PathLike
+from cherno.extraction import Extraction, ExtractionData, PathLike, apply_calibs
 from cherno.lcotcc import apply_correction_lco
 from cherno.maskbits import GuiderStatus
 from cherno.tcc import apply_axes_correction, apply_focus_correction
 from cherno.utils import focus_fit, run_in_executor
 
 
 if TYPE_CHECKING:
     from cherno.actor import ChernoActor, ChernoCommandType
     from cherno.actor.actor import ChernoState
 
 warnings.filterwarnings("ignore", message="pandas only supports SQLAlchemy")
 warnings.filterwarnings("ignore", module="astropy.wcs.wcs")
 warnings.filterwarnings("ignore", category=FITSFixedWarning)
-
+warnings.filterwarnings(
+    "ignore",
+    message="Card is too long, comment will be truncated.",
+)
+warnings.filterwarnings("ignore", category=RuntimeWarning)
 
 __all__ = ["Guider", "GuideData", "AstrometricSolution", "AxesPID"]
 
 
 @dataclass
 class GuideData:
     """Data from the acquisition process."""
@@ -188,188 +196,160 @@
 
         self.observatory = observatory.upper()
         self.fitter = GuiderFitter(self.observatory)
         self.command = command or FakeCommand(log)
         self.target_rms = target_rms
         self.pids = AxesPID(command.actor if command is not None else None)
 
+        # reference to solve pointing instance, initialize to None
+        self.solve_pointing: SolvePointing | None = None
+
         # To cache Gaia sources.
         self._gaia_sources: dict = {}
 
         # Clear RMS history.
         if self.command.actor:
             self.command.actor.state.rms_history.clear()
 
+        # setup task queue for writing proc-*.fits files
+        self.write_background_tasks = set()
+        self.write_executor = ProcessPoolExecutor(
+            max_workers=3,
+            mp_context=mp.get_context("spawn"),
+        )
+
         self._database_lock = asyncio.Lock()
 
     def set_command(self, command: ChernoCommandType):
         """Sets the command."""
 
         self.command = command
 
-    async def process(
+    def check_convergence(
         self,
-        command: ChernoCommandType | None,
-        images: list[PathLike],
-        write_proc: bool = True,
-        overwrite: bool = False,
-        correct: bool = True,
-        full_correction: bool = False,
-        offset: list[float] | None = None,
-        scale_rms: bool = True,
-        wait_for_correction: bool = True,
-        only_radec: bool = False,
-        auto_radec_min: int = 2,
-        use_astrometry_net: bool | None = None,
-        use_gaia: bool = True,
-        gaia_phot_g_mean_mag_max: float | None = None,
-        gaia_cross_correlation_blur: float | None = None,
-        fit_all_detections: bool = True,
-        fit_focus: bool = True,
-        plot: bool | None = None,
-        stop_at_target_rms: bool = False,
+        ex_data: list[ExtractionData],
+        offset: list[float] | None,
     ):
-        """Performs extraction and astrometry."""
+        """Determine whether the guider has converged."""
 
-        if command is not None:
-            self.set_command(command)
+        if self.solve_pointing is None:
+            return False
 
-        self.command.info("Extracting sources.")
+        nSources = numpy.sum([len(ex.regions) for ex in ex_data])
+        if nSources < 6:
+            return False
 
-        ext_data = await asyncio.gather(
-            *[
-                run_in_executor(
-                    self.extractor.process,
-                    im,
-                    plot=plot,
-                    executor="process",
-                )
-                for im in images
-            ]
-        )
+        ex = ex_data[0]
 
-        for d in ext_data:
-            if d.nvalid == 0:
-                self.command.warning(f"Camera {d.camera}: not enough sources.")
-            else:
-                self.command.info(
-                    fwhm_camera=[
-                        d.camera,
-                        d.exposure_no,
-                        d.fwhm_median,
-                        d.nregions,
-                        d.nvalid,
-                    ]
-                )
+        assert self.solve_pointing and self.solve_pointing.imgNum is not None
 
-        guide_data: list[GuideData]
+        if ex.exposure_no != self.solve_pointing.imgNum + 1:
+            return False
 
-        use_astrometry_net = (
-            use_astrometry_net
-            if use_astrometry_net is not None
-            else config["guider"].get("use_astrometry_net", True)
-        )
+        if self.solve_pointing.guide_rms_sky > 1:
+            return False
 
-        if use_astrometry_net:
-            self.command.info("Running astrometry.net.")
-            guide_data = await asyncio.gather(
-                *[self._astrometry_one(d) for d in ext_data]
-            )
-        else:
-            guide_data = [GuideData(ed.camera, ed) for ed in ext_data]
+        if self.solve_pointing._raCen != ex.field_ra:
+            return False
 
-        # Use Gaia cross-match for the cameras that did not solve with astrometry.net.
-        not_solved = [ad for ad in guide_data if ad.solved is False]
-        if use_gaia and len(not_solved) > 0:
-            self.command.info("Running Gaia cross-match.")
-            res = await asyncio.gather(
-                *[
-                    self._gaia_cross_match_one(
-                        ad,
-                        gaia_phot_g_mean_mag_max=gaia_phot_g_mean_mag_max,
-                        gaia_cross_correlation_blur=gaia_cross_correlation_blur,
-                    )
-                    for ad in not_solved
-                ],
-                return_exceptions=True,
-            )
-            for ii, rr in enumerate(res):
-                if isinstance(rr, Exception):
-                    cam = not_solved[ii].camera
-                    self.command.warning(f"{cam}: Gaia cross-match failed: {str(rr)}")
+        if self.solve_pointing._decCen != ex.field_dec:
+            return False
 
-        # Output all the camera_solution keywords at once.
-        for ad in guide_data:
-            self.output_camera_solution(ad)
+        if self.solve_pointing._paCen != ex.field_pa:
+            return False
 
-        self.command.debug("Saving proc- file.")
-        if write_proc:
-            await asyncio.gather(
-                *[self.write_proc_image(d, overwrite=overwrite) for d in guide_data]
-            )
+        full_offset = self.get_full_offset(offset)
 
-        ast_solution = await self.fit(
-            list(guide_data),
-            offset=offset,
-            scale_rms=scale_rms,
-            only_radec=only_radec,
-            auto_radec_min=auto_radec_min,
-            fit_all_detections=fit_all_detections,
-            fit_focus=fit_focus,
-        )
+        if self.solve_pointing.offset_ra != full_offset[0]:
+            return False
 
-        if (
-            self.target_rms is not None
-            and ast_solution.valid_solution
-            and ast_solution.rms > 0
-            and ast_solution.rms <= self.target_rms
-            and stop_at_target_rms
-        ):
-            self.command.warning("RMS has been reached. Not applying correction.")
-            correct = False
+        if self.solve_pointing.offset_dec != full_offset[1]:
+            return False
 
-        if correct and ast_solution.valid_solution is True:
-            await self.correct(
-                ast_solution,
-                full=full_correction,
-                wait_for_correction=wait_for_correction,
-                apply_focus=fit_focus,
-            )
-        else:
-            self.command.info(
-                acquisition_valid=ast_solution.valid_solution,
-                did_correct=any(ast_solution.correction_applied),
-                correction_applied=ast_solution.correction_applied,
-            )
+        if self.solve_pointing.offset_pa != full_offset[2]:
+            return False
 
-        if self.command.actor:
-            update_proc_headers(ast_solution, self.command.actor.state)
+        return True
 
-        return ast_solution
+    def check_wcs(self, guide_data: list[GuideData]):
+        """Returns WCS objects for cameras that solved."""
 
-    async def fit(
+        guide_cameras = self.command.actor.state.guide_cameras
+        wcs_solved = [
+            ad.camera
+            for ad in guide_data
+            if ad.solved is True and ad.camera in guide_cameras
+        ]
+        if len(wcs_solved) > 1:
+            # if 2 or more cameras have wcs solutions, use "coordio"
+            for gd in guide_data:
+                gd.solved = True
+                gd.solve_method = "coordio"
+
+        return wcs_solved
+
+    def try_rapid_solve(
         self,
-        data: list[GuideData],
-        offset: list[float] | None = None,
-        scale_rms: bool = False,
-        fit_focus: bool = True,
-        only_radec: bool = False,
-        auto_radec_min: int = 2,
-        fit_all_detections: bool = True,
+        guide_data: list[GuideData],
+        ext_data: list[ExtractionData],
+        offset: list[float] | None,
     ):
-        """Calculate the astrometric solution."""
+        sp_guider_fit = None
+        converged = self.check_convergence(ext_data, offset)
+
+        if converged:
+            dfList = []
+            for ex in ext_data:
+                regions = ex.regions.copy().reset_index(drop=True)
+                if len(regions) == 0:
+                    continue
+                gfaNum = int(ex.camera.strip("gfa"))
+                regions["gfaNum"] = gfaNum
+                gain = ex.gain
+                regions["gain"] = gain
+                dfList.append(regions)
+
+            df = pandas.concat(dfList).reset_index(drop=True)
+
+            # assert self.solve_pointing
+            sp_guider_fit = self.solve_pointing.reSolve(
+                ex.exposure_no,
+                ex.obstime,
+                ex.exptime,
+                df,
+            )
+
+            # assert self.solve_pointing
+            if self.solve_pointing.guide_rms_sky > 1:
+                # guider probably jumped safer to revert to slow solve
+                sp_guider_fit = None
+                self.solve_pointing = None
+            else:
+                for gd in guide_data:
+                    gfaNum = int(gd.camera.strip("gfa"))
+                    gd.solved = True
+                    wcs = self.solve_pointing.fitWCS(gfaNum)
+                    gd.wcs = wcs
+                    gd.solve_method = "coordio-fast"
+
+        return sp_guider_fit
+
+    def validate_astrometry(self, data: list[GuideData], offset: list[float] | None):
+        """Checks if the astrometry.net solution is valid."""
+
+        isOK = False
 
         ast_solution = AstrometricSolution(False, data)
 
         solved = sorted([d for d in data if d.solved is True], key=lambda x: x.camera)
         weights = [s.extraction_data.nvalid for s in solved]
 
         if len(solved) == 0:
             self.command.error(acquisition_valid=False, did_correct=False)
-            return ast_solution
+            return ast_solution, isOK
 
         fwhm = [d.e_data.fwhm_median for d in data if d.e_data.fwhm_median > 0]
         fwhm_weights = [
             1 / numpy.abs(d.e_data.focus_offset or 1.0)
             for d in data
             if d.e_data.fwhm_median > 0
         ]
@@ -379,113 +359,74 @@
 
         ast_solution.fwhm_median = numpy.round(float(fwhm), 3)
         ast_solution.camera_rotation = numpy.round(float(camera_rotation), 2)
 
         if solved[0].field_ra == "NaN" or isinstance(solved[0].field_ra, str):
             self.command.error(acquisition_valid=False, did_correct=False)
             self.command.error("Field not defined. Cannot run astrometric fit.")
-            return ast_solution
+            return ast_solution, isOK
+
+        isOK = True
 
         if offset is None:
             if self.command.actor:
                 offset = list(self.command.actor.state.offset)
             else:
                 offset = list(config.get("offset", [0.0, 0.0, 0.0]))
 
         if not numpy.allclose(offset, [0.0, 0.0, 0.0]):
             self.command.warning("Using non-zero offsets for astrometric fit.")
 
-        self.fitter.reset()
-        for d in solved:
-            if fit_all_detections:
-                regions = d.extraction_data.regions
-                pixels = regions.loc[:, ["x", "y"]].copy().values
-            else:
-                pixels = None
-            self.fitter.add_wcs(d.camera, d.wcs, d.obstime.jd, pixels=pixels)
+        return ast_solution, isOK
 
-        field_ra = solved[0].field_ra
-        field_dec = solved[0].field_dec
-        field_pa = solved[0].field_pa
+    def get_full_offset(self, offset: list[float] | None):
+        """Outputs and returns the full offset (absolute plus user-commanded)."""
+
+        if offset is None:
+            if self.command.actor:
+                offset = list(self.command.actor.state.offset)
+            else:
+                offset = list(config.get("offset", [0.0, 0.0, 0.0]))
 
         default_offset = config.get("default_offset", (0.0, 0.0, 0.0))
         full_offset = numpy.array(offset) + numpy.array(default_offset)
 
         self.command.debug(default_offset=default_offset)
         if any(offset):
             self.command.warning(offset=offset)
         else:
             self.command.debug(offset=offset)
 
-        if only_radec is True:
-            self.command.warning(
-                "Only fitting RA/Dec. The rotation and scale offsets "
-                "are informational-only and not corrected."
-            )
-        elif auto_radec_min >= 0 and len(solved) <= auto_radec_min:
-            only_radec = True
-            self.command.warning(
-                f"Only {len(solved)} cameras solved. Only fitting RA/Dec. "
-                "The rotation and scale offsets are informational-only "
-                "and not corrected."
-            )
-
-        guide_cameras = self.command.actor.state.guide_cameras
-        fit_cameras = [d.camera_id for d in solved if d.camera in guide_cameras]
-        fit_rms_sigma = config["guider"].get("fit_rms_sigma", 3)
-        guider_fit = False
-        while True:
-            tmp_guider_fit = self.fitter.fit(
-                field_ra,
-                field_dec,
-                field_pa,
-                offset=full_offset,
-                scale_rms=scale_rms,
-                only_radec=only_radec,
-                cameras=fit_cameras,
-            )
-
-            # If we already had a solution and this fit failed or the fit RMS is bad,
-            # just use the previous fit.
-            if guider_fit is not False and (fit_rms_sigma <= 0 or not tmp_guider_fit):
-                break
-
-            # Update the fit with the previous one.
-            guider_fit = tmp_guider_fit
-
-            # If the fit failed, exit.
-            if guider_fit is False:
-                break
-
-            # If only 3 cameras remain we exit. We don't want to reject any more.
-            if len(fit_cameras) <= 3:
-                break
-
-            sc = SigmaClip(fit_rms_sigma)
-            rms_clip = sc(guider_fit.fit_rms.loc[fit_cameras, "rms"])
-
-            # All the camera fit RMS are within X sigma. Exit.
-            if rms_clip.mask.sum() == 0:
-                break
+        return full_offset
 
-            # Find the camera with the largest fit RMS and remove it. Redo the fit.
-            cam_max_rms = int(guider_fit.fit_rms.loc[fit_cameras, "rms"].idxmax())
+    def update_ast_solution(
+        self,
+        ast_solution: AstrometricSolution,
+        data: list[GuideData],
+        guider_fit: GuiderFit | Literal[False],
+        fit_focus: bool,
+    ):
 
-            self.command.warning(
-                "Fit RMS found outlier detections. "
-                f"Refitting without camera {cam_max_rms}."
-            )
-            fit_cameras.remove(cam_max_rms)
+        guide_cameras = self.command.actor.state.guide_cameras
+        solved = sorted([d for d in data if d.solved is True], key=lambda x: x.camera)
+        # fit_cameras1 = [d.camera_id for d in solved if d.camera in guide_cameras]
+        fit_cameras = []
+        for d in solved:
+            if d.camera not in guide_cameras:
+                continue
+            if d.wcs is None:
+                continue
+            fit_cameras.append(d.camera_id)
 
         plate_scale = defaults.PLATE_SCALE[self.observatory]
         mm_to_arcsec = 1 / plate_scale * 3600
 
         exp_no = solved[0].exposure_no  # Should be the same for all.
 
-        if guider_fit:
+        if guider_fit is not False:
             # If we have a guider_fit != False, the fit produced a good astrometric
             # solution.
             ast_solution.valid_solution = True
 
             # Now unpack fit information. We do this even if we reject the
             # fit below because we want the fit data in the headers, but
             # won't apply the correction.
@@ -581,17 +522,17 @@
 
         self.command.info(
             astrometry_fit=[
                 exp_no,
                 len(solved),
                 -999.0,
                 -999.0,
-                numpy.round(fwhm, 2),
+                numpy.round(ast_solution.fwhm_median, 2),
                 -999,
-                numpy.round(camera_rotation, 3),
+                numpy.round(ast_solution.camera_rotation, 3),
                 delta_ra,
                 delta_dec,
                 delta_rot,
                 delta_scale,
             ]
         )
 
@@ -619,15 +560,15 @@
                     ast_solution.delta_focus,
                 ]
             )
 
         if (
             delta_scale > 0
             and self.command.actor
-            and fwhm < 2.5
+            and ast_solution.fwhm_median < 2.5
             and rms > 0
             and rms <= 1
             and guider_fit
             and not guider_fit.only_radec
         ):
             # If we measured the scale, add it to the actor state. This is later
             # used to compute the average scale over a period. We also add the time
@@ -639,16 +580,387 @@
             path = e_data_test.path.parent
             mjd = e_data_test.mjd
             seq = e_data_test.exposure_no
             outpath = path / "fit" / f"fit_rms-{mjd}-{seq}.pdf"
             outpath.parent.mkdir(exist_ok=True)
             self.fitter.plot_fit(outpath)
 
+    async def process(
+        self,
+        command: ChernoCommandType | None,
+        images: list[PathLike],
+        write_proc: bool = True,
+        overwrite: bool = False,
+        correct: bool = True,
+        full_correction: bool = False,
+        offset: list[float] | None = None,
+        scale_rms: bool = True,
+        wait_for_correction: bool = True,
+        only_radec: bool = False,
+        auto_radec_min: int = 2,
+        use_astrometry_net: bool | None = None,
+        use_gaia: bool = True,
+        gaia_phot_g_mean_mag_max: float | None = None,
+        gaia_cross_correlation_blur: float | None = None,
+        fit_all_detections: bool = True,
+        fit_focus: bool = True,
+        plot: bool | None = None,
+        stop_at_target_rms: bool = False,
+    ):
+        """Performs extraction and astrometry."""
+        if command is not None:
+            self.set_command(command)
+
+        # Get the state of the boss spectrograph up front
+        bossExposing = False
+        bossExpNum = -999
+
+        if self.command.actor is not None:
+            if hasattr(self.command.actor, "_process_boss_status"):
+                bossExposing, bossExpNum = self.command.actor._process_boss_status()
+
+        self.command.info("Extracting sources.")
+        ext_data = await asyncio.gather(
+            *[
+                run_in_executor(
+                    self.extractor.process,
+                    im,
+                    plot=plot,
+                    executor="process",
+                )
+                for im in images
+            ]
+        )
+
+        for d in ext_data:
+            if d.nvalid == 0:
+                self.command.warning(f"Camera {d.camera}: not enough sources.")
+            else:
+                self.command.info(
+                    fwhm_camera=[
+                        d.camera,
+                        d.exposure_no,
+                        d.fwhm_median,
+                        d.nregions,
+                        d.nvalid,
+                    ]
+                )
+
+        guide_data = [GuideData(ed.camera, ed) for ed in ext_data]
+
+        _wcs_solved = []
+
+        sp_guider_fit = self.try_rapid_solve(guide_data, ext_data, offset)
+
+        # try:
+        #     sp_guider_fit = self.try_rapid_solve(guide_data, ext_data, offset)
+        # except Exception as err:
+        #     self.command.warning(f"Rapid solve failed: {err}")
+        #     self.command.warning("Reverting to non-converged mode.")
+        #     sp_guider_fit = None
+
+        if sp_guider_fit is None:
+            # Rapid solve didn't work
+            use_astrometry_net = (
+                use_astrometry_net
+                if use_astrometry_net is not None
+                else config["guider"].get("use_astrometry_net", True)
+            )
+
+            if use_astrometry_net:
+                self.command.info("Running astrometry.net.")
+                guide_data = await asyncio.gather(
+                    *[self._astrometry_one(d) for d in ext_data]
+                )
+
+            # check for astrometry.net solutions for cameras actively used
+            # for guide corrections
+            # will modify solved attr on guide_data(s)
+            # if more than 1 wcs exists
+
+            _wcs_solved = self.check_wcs(guide_data)
+
+            # Use Gaia cross-match for the cameras that did not solve with
+            # astrometry.net.
+            not_solved = [ad for ad in guide_data if ad.solved is False]
+            if use_gaia and len(not_solved) > 0:
+                self.command.info("Running Gaia cross-match.")
+                res = await asyncio.gather(
+                    *[
+                        self._gaia_cross_match_one(
+                            ad,
+                            gaia_phot_g_mean_mag_max=gaia_phot_g_mean_mag_max,
+                            gaia_cross_correlation_blur=gaia_cross_correlation_blur,
+                            gaia_table_name=config["guider"]["gaia_connection_table"],
+                            gaia_connection_string=config["guider"][
+                                "gaia_connection_string"
+                            ],
+                        )
+                        for ad in not_solved
+                    ],
+                    return_exceptions=True,
+                )
+
+                for ii, rr in enumerate(res):
+                    if isinstance(rr, Exception):
+                        cam = not_solved[ii].camera
+                        self.command.warning(
+                            f"{cam}: Gaia cross-match failed: {str(rr)}"
+                        )
+
+                # check for xmatch solutions for cameras actively used
+                # for guide corrections
+                # will modify solved attr on guide_data(s)
+                # if more than 1 wcs exists
+
+                _wcs_solved = self.check_wcs(guide_data)
+
+        # Output all the camera_solution keywords at once.
+        for ad in guide_data:
+            self.output_camera_solution(ad)
+
+        ast_solution, isOK = self.validate_astrometry(guide_data, offset)
+
+        if isOK:
+            # continue with guide fitting
+            full_offset: list[float] = self.get_full_offset(offset).tolist()
+
+            if only_radec is True:
+                self.command.warning(
+                    "Only fitting RA/Dec. The rotation and scale offsets "
+                    "are informational-only and not corrected."
+                )
+
+            if sp_guider_fit:
+                # field was already solved in fast mode
+                guider_fit = sp_guider_fit
+
+            elif len(_wcs_solved) > 1:
+                guider_fit = await self.fit_SP(
+                    list(guide_data),
+                    wcs_solved=_wcs_solved,
+                    full_offset=full_offset,
+                )
+
+            else:
+                guider_fit = await self.fit(
+                    list(guide_data),
+                    full_offset=full_offset,
+                    scale_rms=scale_rms,
+                    only_radec=only_radec,
+                    auto_radec_min=auto_radec_min,
+                    fit_all_detections=fit_all_detections,
+                )
+
+            self.update_ast_solution(
+                ast_solution,
+                list(guide_data),
+                guider_fit,
+                fit_focus,
+            )
+
+            if (
+                self.target_rms is not None
+                and ast_solution.valid_solution
+                and ast_solution.rms > 0
+                and ast_solution.rms <= self.target_rms
+                and stop_at_target_rms
+            ):
+                self.command.warning("RMS has been reached. Not applying correction.")
+                correct = False
+
+        if correct and ast_solution.valid_solution is True:
+            await self.correct(
+                ast_solution,
+                full=full_correction,
+                wait_for_correction=wait_for_correction,
+                apply_focus=fit_focus,
+            )
+        else:
+            self.command.info(
+                acquisition_valid=ast_solution.valid_solution,
+                did_correct=any(ast_solution.correction_applied),
+                correction_applied=ast_solution.correction_applied,
+            )
+
+        # write files in the background and move on
+
+        if write_proc and self.command.actor:
+            self.command.debug("Saving proc- files.")
+
+            for d in guide_data:
+                header_updates = get_proc_headers(
+                    ast_solution, self.command.actor.state, d
+                )
+                gaia_matches = None
+                if self.solve_pointing is not None:
+                    header_updates += self.solve_pointing.getMetadata()
+                    zp = self.solve_pointing.median_zeropoint(d.camera_id)
+                    if numpy.isnan(zp):
+                        zp = -999
+                    zptTuple = (
+                        "R_ZPT",
+                        zp,
+                        "median measured zeropoint of gaia sources",
+                    )
+                    header_updates.append(zptTuple)
+                    gaia_matches = self.solve_pointing.matchedSources.copy()
+
+                func = partial(
+                    write_proc_image,
+                    d,
+                    overwrite=overwrite,
+                    bossExposing=bossExposing,
+                    bossExpNum=bossExpNum,
+                    header_updates=header_updates,
+                    gaia_matches=gaia_matches,
+                )
+
+                task = self.write_executor.submit(func)
+
+                # Fire and forget (eg no checking that the fits was actually written ok)
+                self.write_background_tasks.add(task)
+                task.add_done_callback(self.write_background_tasks.discard)
+
         return ast_solution
 
+    async def fit(
+        self,
+        data: list[GuideData],
+        full_offset: list[float],
+        scale_rms: bool = False,
+        only_radec: bool = False,
+        auto_radec_min: int = 2,
+        fit_all_detections: bool = True,
+    ):
+        """Calculate the astrometric solution."""
+
+        solved = sorted([d for d in data if d.solved is True], key=lambda x: x.camera)
+
+        if auto_radec_min >= 0 and len(solved) <= auto_radec_min:
+            only_radec = True
+            self.command.warning(
+                f"Only {len(solved)} cameras solved. Only fitting RA/Dec. "
+                "The rotation and scale offsets are informational-only "
+                "and not corrected."
+            )
+
+        self.fitter.reset()
+        for d in solved:
+            if fit_all_detections:
+                regions = d.extraction_data.regions
+                pixels = regions.loc[:, ["x", "y"]].copy().values
+            else:
+                pixels = None
+            self.fitter.add_wcs(d.camera, d.wcs, d.obstime.jd, pixels=pixels)
+
+        field_ra = solved[0].field_ra
+        field_dec = solved[0].field_dec
+        field_pa = solved[0].field_pa
+
+        guide_cameras = self.command.actor.state.guide_cameras
+        fit_cameras = [d.camera_id for d in solved if d.camera in guide_cameras]
+        fit_rms_sigma = config["guider"].get("fit_rms_sigma", 3)
+        guider_fit = False
+        while True:
+            tmp_guider_fit = self.fitter.fit(
+                field_ra,
+                field_dec,
+                field_pa,
+                offset=numpy.array(full_offset),
+                scale_rms=scale_rms,
+                only_radec=only_radec,
+                cameras=fit_cameras,
+            )
+
+            # If we already had a solution and this fit failed or the fit RMS is bad,
+            # just use the previous fit.
+            if guider_fit is not False and (fit_rms_sigma <= 0 or not tmp_guider_fit):
+                break
+
+            # Update the fit with the previous one.
+            guider_fit = tmp_guider_fit
+
+            # If the fit failed, exit.
+            if guider_fit is False:
+                break
+
+            # If only 3 cameras remain we exit. We don't want to reject any more.
+            if len(fit_cameras) <= 3:
+                break
+
+            sc = SigmaClip(fit_rms_sigma)
+            rms_clip = sc(guider_fit.fit_rms.loc[fit_cameras, "rms"])
+
+            # All the camera fit RMS are within X sigma. Exit.
+            if rms_clip.mask.sum() == 0:
+                break
+
+            # Find the camera with the largest fit RMS and remove it. Redo the fit.
+            cam_max_rms = int(guider_fit.fit_rms.loc[fit_cameras, "rms"].idxmax())
+
+            self.command.warning(
+                "Fit RMS found outlier detections. "
+                f"Refitting without camera {cam_max_rms}."
+            )
+            fit_cameras.remove(cam_max_rms)
+
+        return guider_fit
+
+    async def fit_SP(
+        self,
+        data: list[GuideData],
+        wcs_solved: list[str],
+        full_offset: list[float],
+    ):
+        """Calculate the astrometric solution."""
+
+        solved = sorted([d for d in data if d.solved is True], key=lambda x: x.camera)
+
+        field_ra = solved[0].field_ra
+        field_dec = solved[0].field_dec
+        field_pa = solved[0].field_pa
+
+        guide_cameras = self.command.actor.state.guide_cameras
+
+        self.solve_pointing = SolvePointing(
+            raCen=field_ra,
+            decCen=field_dec,
+            paCen=field_pa,
+            offset_ra=full_offset[0],
+            offset_dec=full_offset[1],
+            offset_pa=full_offset[2],
+            db_conn_st=config["guider"]["gaia_connection_string"],
+            db_tab_name=config["guider"]["gaia_connection_table"],
+        )
+        for d in data:
+            if d.camera not in guide_cameras:
+                continue
+            if d.extraction_data.nregions == 0:
+                continue
+            wcs = None
+            if d.camera in wcs_solved:
+                wcs = d.wcs
+
+            self.solve_pointing.add_gimg(
+                d.path,
+                d.extraction_data.regions.copy(),
+                wcs,
+                d.extraction_data.gain,
+            )
+
+        guider_fit = self.solve_pointing.solve()
+
+        for gd in data:
+            gfaNum = int(gd.camera.strip("gfa"))
+            wcs = self.solve_pointing.fitWCS(gfaNum)
+            gd.wcs = wcs
+
+        return guider_fit
+
     async def correct(
         self,
         data: AstrometricSolution,
         full: bool = False,
         wait_for_correction: bool = True,
         apply_focus: bool = True,
     ):
@@ -681,14 +993,16 @@
 
     async def _correct_apo(
         self,
         data: AstrometricSolution,
         full: bool = False,
         apply_focus: bool = True,
     ):
+        """Apply corrections at APO."""
+
         actor_state = self.command.actor.state
 
         min_isolated = actor_state.guide_loop["rot"]["min_isolated_correction"]
         if abs(data.delta_rot) >= min_isolated:
             self.command.debug("Applying only large rotator correction.")
             coro = apply_axes_correction(
                 self.command,
@@ -742,14 +1056,16 @@
     async def _correct_lco(
         self,
         data: AstrometricSolution,
         full: bool = False,
         wait_for_correction: bool = True,
         apply_focus: bool = True,
     ):
+        """Apply corrections at LCO"""
+
         do_focus: bool = False
 
         enabled_axes = self.command.actor.state.enabled_axes
 
         # Ignore focus correction when the r2 correlation is bad or when we got
         # an inverted parabola.
         if (
@@ -839,14 +1155,15 @@
         proc = await self.astrometry.run_async(
             [gfa_xyls_path],
             stdout=outfile_root.with_suffix(".stdout"),
             stderr=outfile_root.with_suffix(".stderr"),
             ra=radec_centre[0],
             dec=radec_centre[1],
             odds_to_solve=odds_to_solve,
+            radius=1,
         )
 
         guide_data = GuideData(ext_data.camera, ext_data, solve_time=proc.elapsed)
 
         if wcs_output.exists():
             guide_data.solved = True
             wcs = WCS(open(wcs_output).read())
@@ -856,15 +1173,15 @@
         return guide_data
 
     def output_camera_solution(self, guide_data: GuideData):
         """Calculates and outputs the camera_solution keyword."""
 
         wcs = guide_data.wcs
 
-        if wcs and guide_data.solved:
+        if wcs and hasattr(wcs.wcs, "cd") and guide_data.solved:
             racen, deccen = wcs.pixel_to_world_values([[1024, 1024]])[0]
             guide_data.camera_racen = float(numpy.round(racen, 6))
             guide_data.camera_deccen = float(numpy.round(deccen, 6))
 
             # TODO: consider parallactic angle here.
             cd: numpy.ndarray = wcs.wcs.cd
             rot_rad = numpy.arctan2(
@@ -900,14 +1217,16 @@
         )
 
     async def _gaia_cross_match_one(
         self,
         guide_data: GuideData,
         gaia_phot_g_mean_mag_max: float | None = None,
         gaia_cross_correlation_blur: float | None = None,
+        gaia_table_name: str = "catalogdb.gaia_dr2_source_g19",
+        gaia_connection_string: str = config["guider"]["gaia_connection_string"],
     ):
         """Solves a field cross-matching to Gaia."""
 
         cam = guide_data.camera
 
         regions = guide_data.extraction_data.regions.copy()
         regions = regions.loc[regions.valid == 1]
@@ -958,19 +1277,19 @@
 
         fid = guide_data.extraction_data.field_id
         if fid != -999 and (fid, cam_id) in self._gaia_sources:
             gaia_stars = self._gaia_sources[(fid, cam_id)]
 
         else:
             gaia_stars = pandas.read_sql(
-                "SELECT * FROM catalogdb.gaia_dr2_source_g19 "
+                f"SELECT * FROM {gaia_table_name} "
                 "WHERE q3c_radial_query(ra, dec, "
                 f"{ccd_centre[0]}, {ccd_centre[1]}, {gaia_search_radius}) AND "
                 f"phot_g_mean_mag < {g_mag}",
-                config["guider"]["gaia_connection_string"],
+                gaia_connection_string,
             )
             self._gaia_sources[(fid, cam_id)] = gaia_stars
 
         gaia_x, gaia_y = radec_to_gfa(
             self.observatory,
             numpy.array(gaia_stars["ra"].values),
             numpy.array(gaia_stars["dec"].values),
@@ -1018,85 +1337,26 @@
         elif shift and error < min_error:
             self.command.warning(f"{cam}: cross-matching error {error}. Cannot solve.")
         else:
             guide_data.solved = True
             guide_data.solve_method = "gaia"
             guide_data.wcs = wcs
 
-    async def write_proc_image(
-        self,
-        guide_data: GuideData,
-        outpath: PathLike | None = None,
-        overwrite: bool = False,
-    ):
-        """Writes the proc-gimg image."""
 
-        ext_data = guide_data.extraction_data
-
-        proc_hdu = fits.open(str(guide_data.path)).copy()
-
-        rec = Table.from_pandas(guide_data.extraction_data.regions).as_array()
-        proc_hdu.append(fits.BinTableHDU(rec, name="CENTROIDS"))
-
-        gfa_coords = calibration.gfaCoords.reset_index()
-        gfa_coords_rec = Table.from_pandas(gfa_coords).as_array()
-        proc_hdu.append(fits.BinTableHDU(gfa_coords_rec, name="GFACOORD"))
-
-        proc_hdu[1].header["SOLVED"] = guide_data.solved
-        proc_hdu[1].header["SOLVMODE"] = (
-            guide_data.solve_method,
-            "Method used to solve the field",
-        )
-        proc_hdu[1].header["SOLVTIME"] = (
-            guide_data.solve_time,
-            "Time to solve the field or fail",
-        )
-
-        if self.command.actor is not None:
-            offsets = self.command.actor.state.offset
-        else:
-            offsets = [-999.0] * 3
-
-        proc_hdu[1].header["OFFRA"] = (offsets[0], "Relative offset in RA [arcsec]")
-        proc_hdu[1].header["OFFDEC"] = (offsets[1], "Relative offset in Dec [arcsec]")
-        proc_hdu[1].header["OFFPA"] = (offsets[2], "Relative offset in PA [arcsec]")
-
-        default_offset = config.get("default_offset", (0.0, 0.0, 0.0))
-        aoffset = (
-            default_offset[0] + offsets[0],
-            default_offset[1] + offsets[1],
-            default_offset[2] + offsets[2],
-        )
-        proc_hdu[1].header["AOFFRA"] = (aoffset[0], "Absolute offset in RA [arcsec]")
-        proc_hdu[1].header["AOFFDEC"] = (aoffset[1], "Absolute offset in Dec [arcsec]")
-        proc_hdu[1].header["AOFFPA"] = (aoffset[2], "Absolute offset in PA [arcsec]")
-
-        proc_hdu[1].header.update(guide_data.wcs.to_header())
-
-        proc_path: pathlib.Path
-        if outpath is not None:
-            proc_path = pathlib.Path(outpath)
-            if proc_path.is_dir():
-                proc_path = proc_path / ("proc-" + ext_data.path.name)
-        else:
-            proc_path = ext_data.path.parent / ("proc-" + ext_data.path.name)
-
-        loop = asyncio.get_running_loop()
-        func = partial(
-            proc_hdu.writeto,
-            proc_path,
-            overwrite=overwrite,
-            output_verify="silentfix",
-        )
-        await loop.run_in_executor(None, func)
-
-        guide_data.proc_image = proc_path
-
-
-def update_proc_headers(data: AstrometricSolution, guider_state: ChernoState):
+def get_proc_headers(
+    data: AstrometricSolution,
+    guider_state: ChernoState,
+    guide_data: GuideData,
+):
+    """Builds the header object for the ``proc-gimg`` files."""
+
+    # Largely modified from update_proc_headers
+    # returns a list of headers to be updated in a separate
+    # process (guider_state can't be offloaded to ProcessPool)
+    # but a list can.
     guide_loop = guider_state.guide_loop
 
     enabled_axes = guider_state.enabled_axes
     enabled_ra = "ra" in enabled_axes
     enabled_dec = "dec" in enabled_axes
     enabled_rot = "rot" in enabled_axes
     enabled_focus = "focus" in enabled_axes
@@ -1131,60 +1391,175 @@
     rms = data.rms
     delta_ra = data.delta_ra
     delta_dec = data.delta_dec
     delta_rot = data.delta_rot
     delta_scale = data.delta_scale
     delta_focus = data.delta_focus
 
-    # Update headers of proc images with deltas.
-    for a_data in data.guide_data:
-        if a_data.proc_image is not None:
-            hdus = fits.open(str(a_data.proc_image), mode="update")
-            header = hdus[1].header
-
-            header["EXTMETH"] = (a_data.e_data.algorithm, "Algorithm for star finding")
-
-            header["RAK"] = (ra_pid_k, "PID K term for RA")
-            header["RATD"] = (ra_pid_td, "PID Td term for RA")
-            header["RATI"] = (ra_pid_ti, "PID Ti term for RA")
-
-            header["DECK"] = (dec_pid_k, "PID K term for Dec")
-            header["DECTD"] = (dec_pid_td, "PID Td term for Dec")
-            header["DECTI"] = (dec_pid_ti, "PID Ti term for Dec")
-
-            header["ROTK"] = (rot_pid_k, "PID K term for Rot.")
-            header["ROTTD"] = (rot_pid_td, "PID Td term for Rot.")
-            header["ROTTI"] = (rot_pid_ti, "PID Ti term for Rot.")
-
-            header["SCLK"] = (scale_pid_k, "PID K term for Scale")
-            header["SCLTD"] = (scale_pid_td, "PID Td term for Scale")
-            header["SCLTI"] = (scale_pid_ti, "PID Ti term for Scale")
-
-            header["FOCUSK"] = (focus_pid_k, "PID K term for Focus")
-            header["FOCUSTD"] = (focus_pid_td, "PID Td term for Focus")
-            header["FOCUSTI"] = (focus_pid_ti, "PID Ti term for Focus")
-
-            header["FWHM"] = (a_data.e_data.fwhm_median, "Mesured FWHM [arcsec]")
-            header["FWHMFIT"] = (data.fwhm_fit, "Fitted FWHM [arcsec]")
-
-            header["RMS"] = (rms, "Guide RMS [arcsec]")
-            header["FITMODE"] = (data.fit_mode, "Fit mode (full or RA/Dec)")
-
-            header["E_RA"] = (enabled_ra, "RA corrections enabled?")
-            header["E_DEC"] = (enabled_dec, "Dec corrections enabled?")
-            header["E_ROT"] = (enabled_rot, "Rotator corrections enabled?")
-            header["E_FOCUS"] = (enabled_focus, "Focus corrections enabled?")
-            header["E_SCL"] = (False, "Scale corrections enabled?")
-
-            header["DELTARA"] = (delta_ra, "RA measured delta [arcsec]")
-            header["DELTADEC"] = (delta_dec, "Dec measured delta [arcsec]")
-            header["DELTAROT"] = (delta_rot, "Rotator measured delta [arcsec]")
-            header["DELTASCL"] = (delta_scale, "Scale measured factor")
-            header["DELTAFOC"] = (delta_focus, "Focus delta [microns]")
-
-            header["CORR_RA"] = (cra, "RA applied correction [arcsec]")
-            header["CORR_DEC"] = (cdec, "Dec applied correction [arcsec]")
-            header["CORR_ROT"] = (crot, "Rotator applied correction [arcsec]")
-            header["CORR_SCL"] = (cscl, "Scale applied correction")
-            header["CORR_FOC"] = (cfoc, "Focus applied correction [microns]")
+    cra, cdec, crot, cscl, cfoc = data.correction_applied
+
+    # generate header list
+    header = []
+
+    header.append(("SOLVED", guide_data.solved, "field was solved"))
+    header.append(
+        (
+            "SOLVMODE",
+            guide_data.solve_method,
+            "Method used to solve the field",
+        )
+    )
+    header.append(
+        (
+            "SOLVTIME",
+            guide_data.solve_time,
+            "Time to solve the field or fail",
+        )
+    )
+
+    offsets = guider_state.offset
+    header.append(("OFFRA", offsets[0], "Relative offset in RA [arcsec]"))
+    header.append(("OFFDEC", offsets[1], "Relative offset in Dec [arcsec]"))
+    header.append(("OFFPA", offsets[2], "Relative offset in PA [arcsec]"))
+
+    default_offset = config.get("default_offset", (0.0, 0.0, 0.0))
+    aoffset = (
+        default_offset[0] + offsets[0],
+        default_offset[1] + offsets[1],
+        default_offset[2] + offsets[2],
+    )
+    header.append(("AOFFRA", aoffset[0], "Absolute offset in RA [arcsec]"))
+    header.append(("AOFFDEC", aoffset[1], "Absolute offset in Dec [arcsec]"))
+    header.append(("AOFFPA", aoffset[2], "Absolute offset in PA [arcsec]"))
+
+    header.append(
+        (
+            "EXTMETH",
+            guide_data.e_data.algorithm,
+            "Algorithm for star finding",
+        )
+    )
+
+    header.append(("RAK", ra_pid_k, "PID K term for RA"))
+    header.append(("RATD", ra_pid_td, "PID Td term for RA"))
+    header.append(("RATI", ra_pid_ti, "PID Ti term for RA"))
+
+    header.append(("DECK", dec_pid_k, "PID K term for Dec"))
+    header.append(("DECTD", dec_pid_td, "PID Td term for Dec"))
+    header.append(("DECTI", dec_pid_ti, "PID Ti term for Dec"))
+
+    header.append(("ROTK", rot_pid_k, "PID K term for Rot."))
+    header.append(("ROTTD", rot_pid_td, "PID Td term for Rot."))
+    header.append(("ROTTI", rot_pid_ti, "PID Ti term for Rot."))
+
+    header.append(("SCLK", scale_pid_k, "PID K term for Scale"))
+    header.append(("SCLTD", scale_pid_td, "PID Td term for Scale"))
+    header.append(("SCLTI", scale_pid_ti, "PID Ti term for Scale"))
+
+    header.append(("FOCUSK", focus_pid_k, "PID K term for Focus"))
+    header.append(("FOCUSTD", focus_pid_td, "PID Td term for Focus"))
+    header.append(("FOCUSTI", focus_pid_ti, "PID Ti term for Focus"))
+
+    header.append(("FWHM", guide_data.e_data.fwhm_median, "Mesured FWHM [arcsec]"))
+    header.append(("FWHMFIT", data.fwhm_fit, "Fitted FWHM [arcsec]"))
+
+    header.append(("RMS", rms, "Guide RMS [arcsec]"))
+    header.append(("FITMODE", data.fit_mode, "Fit mode (full or RA/Dec)"))
+
+    header.append(("E_RA", enabled_ra, "RA corrections enabled?"))
+    header.append(("E_DEC", enabled_dec, "Dec corrections enabled?"))
+    header.append(("E_ROT", enabled_rot, "Rotator corrections enabled?"))
+    header.append(("E_FOCUS", enabled_focus, "Focus corrections enabled?"))
+    header.append(("E_SCL", False, "Scale corrections enabled?"))
+
+    header.append(("DELTARA", delta_ra, "RA measured delta [arcsec]"))
+    header.append(("DELTADEC", delta_dec, "Dec measured delta [arcsec]"))
+    header.append(("DELTAROT", delta_rot, "Rotator measured delta [arcsec]"))
+    header.append(("DELTASCL", delta_scale, "Scale measured factor"))
+    header.append(("DELTAFOC", delta_focus, "Focus delta [microns]"))
+
+    header.append(("CORR_RA", cra, "RA applied correction [arcsec]"))
+    header.append(("CORR_DEC", cdec, "Dec applied correction [arcsec]"))
+    header.append(("CORR_ROT", crot, "Rotator applied correction [arcsec]"))
+    header.append(("CORR_SCL", cscl, "Scale applied correction"))
+    header.append(("CORR_FOC", cfoc, "Focus applied correction [microns]"))
+
+    return header
+
+
+def write_proc_image(
+    guide_data: GuideData,
+    overwrite: bool = False,
+    bossExposing: bool = False,
+    bossExpNum: int = -999,
+    header_updates: list | None = None,
+    gaia_matches: pandas.DataFrame | None = None,
+):
+    """Writes the processed image to disk."""
+
+    niceness = os.nice(0)
+    dnice = 5 - niceness
+    if dnice != 0:
+        niceness = os.nice(dnice)
+
+    # Mostly coppied from write_proc_image method on guider
+    ext_data = guide_data.extraction_data
+
+    proc_hdu = fits.open(str(guide_data.path)).copy()
+    header = proc_hdu[1].header
+
+    calibs = config["calib"][guide_data.camera]
+
+    # apply calibs again for writing the processed image data (done in extraction
+    # phase too, but data not saved)
+    bias_path = calibs["bias"]
+    dark_path = calibs["dark"]
+    flat_path = calibs["flat"]
+
+    # flat/bias/dark adjust the raw image
+    _calib_data = apply_calibs(
+        data=proc_hdu[1].data,
+        bias_path=bias_path,
+        dark_path=dark_path,
+        flat_path=flat_path,
+        gain=proc_hdu[1].header["GAIN"],
+        exptime=proc_hdu[1].header["EXPTIMEN"],
+    )
+    proc_hdu[1].data = _calib_data
+    header["BKG_ADU"] = (
+        numpy.median(_calib_data),
+        "background (median) counts in calibrated frame",
+    )
+
+    header["BIASFILE"] = bias_path
+    header["FLATFILE"] = flat_path
+    header["DARKFILE"] = dark_path
+
+    rec = Table.from_pandas(guide_data.extraction_data.regions).as_array()
+    proc_hdu.append(fits.BinTableHDU(rec, name="CENTROIDS"))
+
+    gfa_coords = calibration.gfaCoords.reset_index()
+    gfa_coords_rec = Table.from_pandas(gfa_coords).as_array()
+    proc_hdu.append(fits.BinTableHDU(gfa_coords_rec, name="GFACOORD"))
+
+    if guide_data.wcs is not None:
+        header.update(guide_data.wcs.to_header())
+
+    proc_path: pathlib.Path
+
+    proc_path = ext_data.path.parent / ("proc-" + ext_data.path.name)
+
+    if header_updates is not None:
+        for kw, val, comment in header_updates:
+            header[kw] = (val, comment)
+    if gaia_matches is not None:
+        rec = Table.from_pandas(gaia_matches).as_array()
+        proc_hdu.append(fits.BinTableHDU(rec, name="GAIAMATCH"))
+
+    header["SPEXPNG"] = (bossExposing, "BOSS spectrograph exposing")
+    header["SPIMGNO"] = (bossExpNum, "BOSS spectrograph current exposure number")
+
+    proc_hdu.writeto(proc_path, overwrite=overwrite, output_verify="silentfix")
+    proc_hdu.close()
 
-            hdus.close()
+    # probably not necessary to add this to the guide_data anymore
+    guide_data.proc_image = proc_path
```

### Comparing `sdss_cherno-0.6.9/cherno/lcotcc.py` & `sdss_cherno-1.0.0/cherno/lcotcc.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.9/cherno/maskbits.py` & `sdss_cherno-1.0.0/cherno/maskbits.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.9/cherno/tcc.py` & `sdss_cherno-1.0.0/cherno/tcc.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.9/cherno/utils.py` & `sdss_cherno-1.0.0/cherno/utils.py`

 * *Files identical despite different names*

### Comparing `sdss_cherno-0.6.9/pyproject.toml` & `sdss_cherno-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-cherno"
-version = "0.6.9"
+version = "1.0.0"
 description = "SDSS guider actor"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/cherno"
 repository = "https://github.com/sdss/cherno"
 documentation = "https://sdss-cherno.readthedocs.org"
@@ -28,15 +28,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.10,<3.13"
 sdsstools = "^1.5.5"
 sdss-clu = "^1.8.0"
 astropy = "^6.0.0"
 click-default-group = "^1.2.2"
-sdss-coordio = "^1.9.2"
+sdss-coordio = "^1.11.2"
 pandas = "^2.0.0"
 tables = ">=3.6.1"
 simple-pid = "^1.0.1"
 sqlalchemy = "^2.0.0"
 psycopg2-binary = "^2.9.5"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `sdss_cherno-0.6.9/PKG-INFO` & `sdss_cherno-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-cherno
-Version: 0.6.9
+Version: 1.0.0
 Summary: SDSS guider actor
 Home-page: https://github.com/sdss/cherno
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.10,<3.13
@@ -20,15 +20,15 @@
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: astropy (>=6.0.0,<7.0.0)
 Requires-Dist: click-default-group (>=1.2.2,<2.0.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
 Requires-Dist: sdss-clu (>=1.8.0,<2.0.0)
-Requires-Dist: sdss-coordio (>=1.9.2,<2.0.0)
+Requires-Dist: sdss-coordio (>=1.11.2,<2.0.0)
 Requires-Dist: sdsstools (>=1.5.5,<2.0.0)
 Requires-Dist: simple-pid (>=1.0.1,<2.0.0)
 Requires-Dist: sqlalchemy (>=2.0.0,<3.0.0)
 Requires-Dist: tables (>=3.6.1)
 Project-URL: Documentation, https://sdss-cherno.readthedocs.org
 Project-URL: Repository, https://github.com/sdss/cherno
 Description-Content-Type: text/markdown
```

