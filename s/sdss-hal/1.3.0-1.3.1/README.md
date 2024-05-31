# Comparing `tmp/sdss_hal-1.3.0.tar.gz` & `tmp/sdss_hal-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_hal-1.3.0.tar", max compression
+gzip compressed data, was "sdss_hal-1.3.1.tar", max compression
```

## Comparing `sdss_hal-1.3.0.tar` & `sdss_hal-1.3.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1504 2024-05-29 23:42:56.001789 sdss_hal-1.3.0/LICENSE.md
--rw-r--r--   0        0        0      816 2024-05-29 23:42:56.001789 sdss_hal-1.3.0/README.md
--rw-r--r--   0        0        0     2708 2024-05-29 23:42:56.005790 sdss_hal-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      483 2024-05-29 23:42:56.005790 sdss_hal-1.3.0/src/hal/__init__.py
--rw-r--r--   0        0        0     1761 2024-05-29 23:42:56.005790 sdss_hal-1.3.0/src/hal/__main__.py
--rw-r--r--   0        0        0      356 2024-05-29 23:42:56.005790 sdss_hal-1.3.0/src/hal/actor/__init__.py
--rw-r--r--   0        0        0     3024 2024-05-29 23:42:56.005790 sdss_hal-1.3.0/src/hal/actor/actor.py
--rw-r--r--   0        0        0     3357 2024-05-29 23:42:56.005790 sdss_hal-1.3.0/src/hal/actor/commands/__init__.py
--rw-r--r--   0        0        0     2014 2024-05-29 23:42:56.005790 sdss_hal-1.3.0/src/hal/actor/commands/abort_exposures.py
--rw-r--r--   0        0        0     3940 2024-05-29 23:42:56.005790 sdss_hal-1.3.0/src/hal/actor/commands/auto_pilot.py
--rw-r--r--   0        0        0     1593 2024-05-29 23:42:56.005790 sdss_hal-1.3.0/src/hal/actor/commands/bypass.py
--rw-r--r--   0        0        0      844 2024-05-29 23:42:56.005790 sdss_hal-1.3.0/src/hal/actor/commands/calibrations.py
--rw-r--r--   0        0        0     8082 2024-05-29 23:42:56.005790 sdss_hal-1.3.0/src/hal/actor/commands/expose.py
--rw-r--r--   0        0        0     1669 2024-05-29 23:42:56.005790 sdss_hal-1.3.0/src/hal/actor/commands/goto.py
--rw-r--r--   0        0        0     3498 2024-05-29 23:42:56.005790 sdss_hal-1.3.0/src/hal/actor/commands/goto_field.py
--rw-r--r--   0        0        0     2537 2024-05-29 23:42:56.005790 sdss_hal-1.3.0/src/hal/actor/commands/script.py
--rw-r--r--   0        0        0     1419 2024-05-29 23:42:56.005790 sdss_hal-1.3.0/src/hal/actor/commands/status.py
--rw-r--r--   0        0        0      687 2024-05-29 23:42:56.005790 sdss_hal-1.3.0/src/hal/actor/commands/test.py
--rw-r--r--   0        0        0     3362 2024-05-29 23:42:56.005790 sdss_hal-1.3.0/src/hal/etc/hal.yml
--rw-r--r--   0        0        0     2190 2024-05-29 23:42:56.005790 sdss_hal-1.3.0/src/hal/etc/schema.json
--rw-r--r--   0        0        0      346 2024-05-29 23:42:56.005790 sdss_hal-1.3.0/src/hal/etc/scripts/apo/cartchange.inp
--rw-r--r--   0        0        0     1161 2024-05-29 23:42:56.005790 sdss_hal-1.3.0/src/hal/etc/scripts/apo/eveningcals.inp
--rw-r--r--   0        0        0      161 2024-05-29 23:42:56.005790 sdss_hal-1.3.0/src/hal/etc/scripts/apo/example.inp
--rw-r--r--   0        0        0     1616 2024-05-29 23:42:56.005790 sdss_hal-1.3.0/src/hal/etc/scripts/apo/morningcals.inp
--rw-r--r--   0        0        0       35 2024-05-29 23:42:56.005790 sdss_hal-1.3.0/src/hal/etc/scripts/apo/test.inp
--rw-r--r--   0        0        0      346 2024-05-29 23:42:56.005790 sdss_hal-1.3.0/src/hal/etc/scripts/lco/cartchange.inp
--rw-r--r--   0        0        0     1056 2024-05-29 23:42:56.009790 sdss_hal-1.3.0/src/hal/etc/scripts/lco/eveningcals.inp
--rw-r--r--   0        0        0     1450 2024-05-29 23:42:56.009790 sdss_hal-1.3.0/src/hal/etc/scripts/lco/morningcals.inp
--rw-r--r--   0        0        0     1180 2024-05-29 23:42:56.009790 sdss_hal-1.3.0/src/hal/exceptions.py
--rw-r--r--   0        0        0     3502 2024-05-29 23:42:56.009790 sdss_hal-1.3.0/src/hal/helpers/__init__.py
--rw-r--r--   0        0        0    10870 2024-05-29 23:42:56.009790 sdss_hal-1.3.0/src/hal/helpers/apogee.py
--rw-r--r--   0        0        0     7773 2024-05-29 23:42:56.009790 sdss_hal-1.3.0/src/hal/helpers/boss.py
--rw-r--r--   0        0        0     6514 2024-05-29 23:42:56.009790 sdss_hal-1.3.0/src/hal/helpers/cherno.py
--rw-r--r--   0        0        0     1769 2024-05-29 23:42:56.009790 sdss_hal-1.3.0/src/hal/helpers/ffs.py
--rw-r--r--   0        0        0     8270 2024-05-29 23:42:56.009790 sdss_hal-1.3.0/src/hal/helpers/jaeger.py
--rw-r--r--   0        0        0    10429 2024-05-29 23:42:56.009790 sdss_hal-1.3.0/src/hal/helpers/lamps.py
--rw-r--r--   0        0        0     4732 2024-05-29 23:42:56.009790 sdss_hal-1.3.0/src/hal/helpers/overhead.py
--rw-r--r--   0        0        0     4671 2024-05-29 23:42:56.009790 sdss_hal-1.3.0/src/hal/helpers/scripts.py
--rw-r--r--   0        0        0    13441 2024-05-29 23:42:56.009790 sdss_hal-1.3.0/src/hal/helpers/tcc.py
--rw-r--r--   0        0        0     1399 2024-05-29 23:42:56.009790 sdss_hal-1.3.0/src/hal/macros/__init__.py
--rw-r--r--   0        0        0     3844 2024-05-29 23:42:56.009790 sdss_hal-1.3.0/src/hal/macros/apogee_dome_flat.py
--rw-r--r--   0        0        0    12441 2024-05-29 23:42:56.009790 sdss_hal-1.3.0/src/hal/macros/auto_pilot.py
--rw-r--r--   0        0        0    21726 2024-05-29 23:42:56.009790 sdss_hal-1.3.0/src/hal/macros/expose.py
--rw-r--r--   0        0        0    23929 2024-05-29 23:42:56.009790 sdss_hal-1.3.0/src/hal/macros/goto_field.py
--rw-r--r--   0        0        0    18881 2024-05-29 23:42:56.009790 sdss_hal-1.3.0/src/hal/macros/macro.py
--rw-r--r--   0        0        0     1263 2024-05-29 23:42:56.009790 sdss_hal-1.3.0/src/hal/macros/test_macro.py
--rw-r--r--   0        0        0     2219 1970-01-01 00:00:00.000000 sdss_hal-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2024-05-31 00:14:27.909060 sdss_hal-1.3.1/LICENSE.md
+-rw-r--r--   0        0        0      816 2024-05-31 00:14:27.909060 sdss_hal-1.3.1/README.md
+-rw-r--r--   0        0        0     2708 2024-05-31 00:14:27.913060 sdss_hal-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      483 2024-05-31 00:14:27.913060 sdss_hal-1.3.1/src/hal/__init__.py
+-rw-r--r--   0        0        0     1761 2024-05-31 00:14:27.913060 sdss_hal-1.3.1/src/hal/__main__.py
+-rw-r--r--   0        0        0      356 2024-05-31 00:14:27.913060 sdss_hal-1.3.1/src/hal/actor/__init__.py
+-rw-r--r--   0        0        0     3024 2024-05-31 00:14:27.913060 sdss_hal-1.3.1/src/hal/actor/actor.py
+-rw-r--r--   0        0        0     3357 2024-05-31 00:14:27.913060 sdss_hal-1.3.1/src/hal/actor/commands/__init__.py
+-rw-r--r--   0        0        0     2014 2024-05-31 00:14:27.913060 sdss_hal-1.3.1/src/hal/actor/commands/abort_exposures.py
+-rw-r--r--   0        0        0     4811 2024-05-31 00:14:27.913060 sdss_hal-1.3.1/src/hal/actor/commands/auto_pilot.py
+-rw-r--r--   0        0        0     1593 2024-05-31 00:14:27.913060 sdss_hal-1.3.1/src/hal/actor/commands/bypass.py
+-rw-r--r--   0        0        0      844 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/actor/commands/calibrations.py
+-rw-r--r--   0        0        0     8082 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/actor/commands/expose.py
+-rw-r--r--   0        0        0     1669 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/actor/commands/goto.py
+-rw-r--r--   0        0        0     3498 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/actor/commands/goto_field.py
+-rw-r--r--   0        0        0     2537 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/actor/commands/script.py
+-rw-r--r--   0        0        0     1419 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/actor/commands/status.py
+-rw-r--r--   0        0        0      687 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/actor/commands/test.py
+-rw-r--r--   0        0        0     3362 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/etc/hal.yml
+-rw-r--r--   0        0        0     2240 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/etc/schema.json
+-rw-r--r--   0        0        0      346 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/etc/scripts/apo/cartchange.inp
+-rw-r--r--   0        0        0     1161 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/etc/scripts/apo/eveningcals.inp
+-rw-r--r--   0        0        0      161 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/etc/scripts/apo/example.inp
+-rw-r--r--   0        0        0     1616 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/etc/scripts/apo/morningcals.inp
+-rw-r--r--   0        0        0       35 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/etc/scripts/apo/test.inp
+-rw-r--r--   0        0        0      346 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/etc/scripts/lco/cartchange.inp
+-rw-r--r--   0        0        0     1056 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/etc/scripts/lco/eveningcals.inp
+-rw-r--r--   0        0        0     1450 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/etc/scripts/lco/morningcals.inp
+-rw-r--r--   0        0        0     1180 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/exceptions.py
+-rw-r--r--   0        0        0     3502 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/helpers/__init__.py
+-rw-r--r--   0        0        0    10870 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/helpers/apogee.py
+-rw-r--r--   0        0        0     7773 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/helpers/boss.py
+-rw-r--r--   0        0        0     6514 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/helpers/cherno.py
+-rw-r--r--   0        0        0     1769 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/helpers/ffs.py
+-rw-r--r--   0        0        0     8276 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/helpers/jaeger.py
+-rw-r--r--   0        0        0    10429 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/helpers/lamps.py
+-rw-r--r--   0        0        0     4732 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/helpers/overhead.py
+-rw-r--r--   0        0        0     4671 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/helpers/scripts.py
+-rw-r--r--   0        0        0    13441 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/helpers/tcc.py
+-rw-r--r--   0        0        0     1399 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/macros/__init__.py
+-rw-r--r--   0        0        0     3844 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/macros/apogee_dome_flat.py
+-rw-r--r--   0        0        0    13042 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/macros/auto_pilot.py
+-rw-r--r--   0        0        0    21726 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/macros/expose.py
+-rw-r--r--   0        0        0    23929 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/macros/goto_field.py
+-rw-r--r--   0        0        0    18881 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/macros/macro.py
+-rw-r--r--   0        0        0     1263 2024-05-31 00:14:27.917060 sdss_hal-1.3.1/src/hal/macros/test_macro.py
+-rw-r--r--   0        0        0     2219 1970-01-01 00:00:00.000000 sdss_hal-1.3.1/PKG-INFO
```

### Comparing `sdss_hal-1.3.0/LICENSE.md` & `sdss_hal-1.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/README.md` & `sdss_hal-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/pyproject.toml` & `sdss_hal-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-hal"
-version = "1.3.0"
+version = "1.3.1"
 description = "High-level observing tool for SDSS-V (replaces SOP)"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/hal"
 repository = "https://github.com/sdss/hal"
 documentation = "https://sdss-hal.readthedocs.org"
```

### Comparing `sdss_hal-1.3.0/src/hal/__main__.py` & `sdss_hal-1.3.1/src/hal/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/actor/actor.py` & `sdss_hal-1.3.1/src/hal/actor/actor.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/actor/commands/__init__.py` & `sdss_hal-1.3.1/src/hal/actor/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/actor/commands/abort_exposures.py` & `sdss_hal-1.3.1/src/hal/actor/commands/abort_exposures.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/actor/commands/auto_pilot.py` & `sdss_hal-1.3.1/src/hal/actor/commands/auto_pilot.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import asyncio
 
 from typing import TYPE_CHECKING
 
 import click
 
+from hal.macros.auto_pilot import AutoPilotMacro
 from hal.macros.expose import ExposeMacro
 
 from . import hal_command_parser
 
 
 if TYPE_CHECKING:
     from .. import HALCommandType
@@ -61,38 +62,60 @@
 )
 @click.option(
     "--preload-ahead",
     type=float,
     default=None,
     help="Preload the next design this many seconds before the exposure completes.",
 )
+@click.option(
+    "--add-hartmann",
+    is_flag=True,
+    default=False,
+    help="Take a Hartmann during the next goto-field (will not repeat Hartmanns).",
+)
+@click.option(
+    "--remove-hartmann",
+    is_flag=True,
+    default=False,
+    help="Removes a previously scheduled Hartmann.",
+)
 async def auto_pilot(
     command: HALCommandType,
     stop: bool = False,
     now: bool = False,
     modify: bool = False,
     pause: bool = False,
     resume: bool = False,
     count: int = 1,
     preload_ahead: float | None = None,
+    add_hartmann: bool = False,
+    remove_hartmann: bool = False,
 ):
     """Starts the auto-pilot mode."""
 
     assert command.actor
 
     expose_macro = command.actor.helpers.macros["expose"]
     assert isinstance(expose_macro, ExposeMacro)
 
     macro = command.actor.helpers.macros["auto_pilot"]
+    assert isinstance(macro, AutoPilotMacro)
 
     if (stop or modify or pause or resume) and not macro.running:
         return command.fail(
             "I'm afraid I cannot do that Dave. The auto pilot mode is not running."
         )
 
+    if macro.running and (add_hartmann or remove_hartmann):
+        macro.hartmann = False if remove_hartmann else True
+        if macro.hartmann:
+            return command.finish("Scheduled a Hartmann for the next goto-field.")
+        else:
+            return command.finish("Removed any previously scheduled Hartmanns.")
+
     if pause and resume:
         return command.fail("--pause and --resume are incompatible Dave.")
 
     if pause:
         await expose_macro._pause()
         return command.finish()
 
@@ -127,14 +150,18 @@
     # From this point on this is a new macro, so it should not be already running.
     if macro.running:
         return command.fail(
             "I'm afraid I cannot do that Dave. The auto mode is already running."
         )
 
     macro.reset(command, count=count, preload_ahead_time=preload_ahead)
+    if add_hartmann:
+        macro.hartmann = True
+    else:
+        macro.hartmann = False
 
     result: bool = True
     while True:
         # Reset the macro (stages and such) but keep the current config.
         macro.reset(command, reset_config=False)
 
         # Run the auto loop until the command is cancelled.
```

### Comparing `sdss_hal-1.3.0/src/hal/actor/commands/bypass.py` & `sdss_hal-1.3.1/src/hal/actor/commands/bypass.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/actor/commands/calibrations.py` & `sdss_hal-1.3.1/src/hal/actor/commands/calibrations.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/actor/commands/expose.py` & `sdss_hal-1.3.1/src/hal/actor/commands/expose.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/actor/commands/goto.py` & `sdss_hal-1.3.1/src/hal/actor/commands/goto.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/actor/commands/goto_field.py` & `sdss_hal-1.3.1/src/hal/actor/commands/goto_field.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/actor/commands/script.py` & `sdss_hal-1.3.1/src/hal/actor/commands/script.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/actor/commands/status.py` & `sdss_hal-1.3.1/src/hal/actor/commands/status.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/actor/commands/test.py` & `sdss_hal-1.3.1/src/hal/actor/commands/test.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/etc/hal.yml` & `sdss_hal-1.3.1/src/hal/etc/hal.yml`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/etc/schema.json` & `sdss_hal-1.3.1/src/hal/etc/schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9895833333333334%*

 * *Differences: {"'properties'": "{'auto_pilot_hartmann': OrderedDict([('type', 'boolean')])}"}*

```diff
@@ -5,14 +5,17 @@
         "all_stages": {
             "items": {
                 "type": "string"
             },
             "minLength": 2,
             "type": "array"
         },
+        "auto_pilot_hartmann": {
+            "type": "boolean"
+        },
         "auto_pilot_message": {
             "type": "string"
         },
         "available_scripts": {
             "items": {
                 "type": "string"
             },
```

### Comparing `sdss_hal-1.3.0/src/hal/etc/scripts/apo/eveningcals.inp` & `sdss_hal-1.3.1/src/hal/etc/scripts/apo/eveningcals.inp`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/etc/scripts/apo/morningcals.inp` & `sdss_hal-1.3.1/src/hal/etc/scripts/apo/morningcals.inp`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/etc/scripts/lco/eveningcals.inp` & `sdss_hal-1.3.1/src/hal/etc/scripts/lco/eveningcals.inp`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/etc/scripts/lco/morningcals.inp` & `sdss_hal-1.3.1/src/hal/etc/scripts/lco/morningcals.inp`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/exceptions.py` & `sdss_hal-1.3.1/src/hal/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/helpers/__init__.py` & `sdss_hal-1.3.1/src/hal/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/helpers/apogee.py` & `sdss_hal-1.3.1/src/hal/helpers/apogee.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/helpers/boss.py` & `sdss_hal-1.3.1/src/hal/helpers/boss.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/helpers/cherno.py` & `sdss_hal-1.3.1/src/hal/helpers/cherno.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/helpers/ffs.py` & `sdss_hal-1.3.1/src/hal/helpers/ffs.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/helpers/jaeger.py` & `sdss_hal-1.3.1/src/hal/helpers/jaeger.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         elif self.new_field is False:
             stages = goto_auto_mode_stages["repeat_field_stages"][observatory]
         elif self.is_rm_field is True:
             stages = goto_auto_mode_stages["rm_field_stages"][observatory]
         else:
             stages = goto_auto_mode_stages["new_field_stages"][observatory]
 
-        return stages
+        return list(stages)
 
 
 class JaegerHelper(HALHelper):
     """Helper to interact with jaeger."""
 
     name = "jaeger"
```

### Comparing `sdss_hal-1.3.0/src/hal/helpers/lamps.py` & `sdss_hal-1.3.1/src/hal/helpers/lamps.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/helpers/overhead.py` & `sdss_hal-1.3.1/src/hal/helpers/overhead.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/helpers/scripts.py` & `sdss_hal-1.3.1/src/hal/helpers/scripts.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/helpers/tcc.py` & `sdss_hal-1.3.1/src/hal/helpers/tcc.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/macros/__init__.py` & `sdss_hal-1.3.1/src/hal/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/macros/apogee_dome_flat.py` & `sdss_hal-1.3.1/src/hal/macros/apogee_dome_flat.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/macros/auto_pilot.py` & `sdss_hal-1.3.1/src/hal/macros/auto_pilot.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,16 +88,32 @@
     __CLEANUP__ = ["cleanup"]
 
     def __init__(self):
         super().__init__()
 
         self.system_state = SystemState(self)
 
+        self._hartmann: bool = False
         self._preload_task: asyncio.Task | None = None
 
+    @property
+    def hartmann(self):
+        """Returns whether a Hartmann is scheduled."""
+
+        return self._hartmann
+
+    @hartmann.setter
+    def hartmann(self, value: bool):
+        """Sets whether a Hartmann is to be scheduled."""
+
+        self._hartmann = value
+
+        if self.command:
+            self.command.debug(auto_pilot_hartmann=value)
+
     async def prepare(self):
         """Prepares the auto pilot."""
 
         # Update spectrograph states.
         self.system_state.update_exposure_state()
         self.system_state.update_time_remaining()
 
@@ -180,17 +196,26 @@
 
         stages = configuration.get_goto_field_stages()
 
         if len(stages) == 0:  # For cloned designs.
             self._auto_pilot_message("Skipping goto-field")
             return
 
+        if self.hartmann and "hartmann" not in stages:
+            stages.append("hartmann")
+
         self._auto_pilot_message("Running goto-field")
         self.helpers.macros["goto_field"].reset(self.command, stages)
-        if not await self.helpers.macros["goto_field"].run():
+
+        result = await self.helpers.macros["goto_field"].run()
+
+        if self.hartmann and "hartmann" in stages:
+            self.hartmann = False
+
+        if not result:
             raise MacroError("Goto-field failed during auto pilot mode.")
 
     async def expose(self):
         """Exposes the cameras."""
 
         expose_macro = self.helpers.macros["expose"]
         if expose_macro.running:
```

### Comparing `sdss_hal-1.3.0/src/hal/macros/expose.py` & `sdss_hal-1.3.1/src/hal/macros/expose.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/macros/goto_field.py` & `sdss_hal-1.3.1/src/hal/macros/goto_field.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/macros/macro.py` & `sdss_hal-1.3.1/src/hal/macros/macro.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/src/hal/macros/test_macro.py` & `sdss_hal-1.3.1/src/hal/macros/test_macro.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.0/PKG-INFO` & `sdss_hal-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-hal
-Version: 1.3.0
+Version: 1.3.1
 Summary: High-level observing tool for SDSS-V (replaces SOP)
 Home-page: https://github.com/sdss/hal
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.10,<4.0
```

