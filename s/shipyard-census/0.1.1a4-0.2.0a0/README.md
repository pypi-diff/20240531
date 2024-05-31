# Comparing `tmp/shipyard_census-0.1.1a4.tar.gz` & `tmp/shipyard_census-0.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_census-0.1.1a4.tar", max compression
+gzip compressed data, was "shipyard_census-0.2.0a0.tar", max compression
```

## Comparing `shipyard_census-0.1.1a4.tar` & `shipyard_census-0.2.0a0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      632 2023-07-28 02:55:46.151323 shipyard_census-0.1.1a4/pyproject.toml
--rw-r--r--   0        0        0       33 2023-05-12 18:48:21.825204 shipyard_census-0.1.1a4/shipyard_census/__init__.py
--rw-r--r--   0        0        0     5852 2023-07-28 02:46:43.842558 shipyard_census-0.1.1a4/shipyard_census/census.py
--rw-r--r--   0        0        0      186 2023-07-28 00:25:41.244623 shipyard_census-0.1.1a4/shipyard_census/cli/authtest.py
--rw-r--r--   0        0        0     2844 2023-07-28 02:48:25.059554 shipyard_census-0.1.1a4/shipyard_census/cli/trigger_sync_cli.py
--rw-r--r--   0        0        0       71 2023-07-03 14:05:58.556145 shipyard_census-0.1.1a4/shipyard_census/test/tests.py
--rw-r--r--   0        0        0      517 1970-01-01 00:00:00.000000 shipyard_census-0.1.1a4/PKG-INFO
+-rw-r--r--   0        0        0      580 2024-05-31 01:56:12.726350 shipyard_census-0.2.0a0/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-05-12 18:48:21.825204 shipyard_census-0.2.0a0/shipyard_census/__init__.py
+-rw-r--r--   0        0        0     5783 2024-05-31 01:15:56.800033 shipyard_census-0.2.0a0/shipyard_census/census.py
+-rw-r--r--   0        0        0        0 2024-02-05 20:53:35.432394 shipyard_census-0.2.0a0/shipyard_census/cli/__init__.py
+-rw-r--r--   0        0        0      182 2024-02-05 20:53:35.432711 shipyard_census-0.2.0a0/shipyard_census/cli/authtest.py
+-rw-r--r--   0        0        0     2454 2024-05-31 01:15:56.800384 shipyard_census-0.2.0a0/shipyard_census/cli/trigger_sync_cli.py
+-rw-r--r--   0        0        0      618 1970-01-01 00:00:00.000000 shipyard_census-0.2.0a0/PKG-INFO
```

### Comparing `shipyard_census-0.1.1a4/shipyard_census/cli/trigger_sync_cli.py` & `shipyard_census-0.2.0a0/shipyard_census/cli/trigger_sync_cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,18 @@
+import argparse
 import os
 import sys
-import argparse
 import time
-import shipyard_utils as shipyard
 
-from shipyard_census import CensusClient
-from shipyard_templates import ExitCodeException
+from shipyard_bp_utils.artifacts import Artifact
+from shipyard_templates import ExitCodeException, ShipyardLogger
 
+from shipyard_census import CensusClient
 
-def create_artifact(sync_run_id):
-    # create artifacts folder to save run id for legacy sync check
-    base_folder_name = shipyard.logs.determine_base_artifact_folder("census")
-    artifact_subfolder_paths = shipyard.logs.determine_artifact_subfolders(
-        base_folder_name
-    )
-    shipyard.logs.create_artifacts_folders(artifact_subfolder_paths)
-
-    # save sync run id as variable
-    shipyard.logs.create_pickle_file(
-        artifact_subfolder_paths, "sync_run_id", sync_run_id
-    )
+logger = ShipyardLogger.get_logger()
 
 
 def get_args():
     parser = argparse.ArgumentParser()
     parser.add_argument("--access-token", dest="access_token", required=True)
     parser.add_argument("--sync-id", dest="sync_id", required=True)
     parser.add_argument("--wait-for-completion", default="FALSE")
@@ -33,48 +22,49 @@
 
 def main():
     args = get_args()
     census = CensusClient(args.access_token)
     try:
         trigger_sync = census.trigger_sync(args.sync_id)
     except ExitCodeException as error:
-        census.logger.error(error)
+        logger.error(error)
         sys.exit(error.exit_code)
 
     sync_run_id = trigger_sync["data"]["sync_run_id"]
     wait = args.wait_for_completion.upper() == "TRUE"
     if wait:
         poke_interval = args.poke_interval
         if poke_interval == "" or poke_interval is None:
-            census.logger.error(
+            logger.error(
                 "Poke interval must be specified when waiting for sync completion"
             )
-            sys.exit(census.EXIT_CODE_INVALID_POKE_INTERVAL)
+            sys.exit(census.EXIT_CODE_SYNC_INVALID_POKE_INTERVAL)
 
         if 0 < int(poke_interval) <= 60:
-            census.logger.info(f"Setting poke interval to {poke_interval} minute(s)")
+            logger.info(f"Setting poke interval to {poke_interval} minute(s)")
             poke_interval = int(poke_interval)
         else:
-            census.logger.error("Poke interval must be between 1 and 60 minutes")
-            sys.exit(census.EXIT_CODE_INVALID_POKE_INTERVAL)
+            logger.error("Poke interval must be between 1 and 60 minutes")
+            sys.exit(census.EXIT_CODE_SYNC_INVALID_POKE_INTERVAL)
 
         status = None
         while status != "completed":
             try:
                 sync_run_data = census.get_sync_status(sync_run_id)
                 status = census.determine_sync_status(sync_run_data)
                 if status != "completed":
-                    census.logger.info(
+                    logger.info(
                         f"Waiting {poke_interval} minute(s) to check sync status..."
                     )
                     time.sleep(poke_interval * 60)
             except ExitCodeException as error:
-                census.logger.error(error)
+                logger.error(error)
                 sys.exit(error.exit_code)
 
     elif not wait and int(os.environ.get("SHIPYARD_FLEET_DOWNSTREAM_COUNT")) > 0:
+        artifact = Artifact("census")
         # Create the artifact for legacy blueprints to continue to work
-        create_artifact(sync_run_id)
+        artifact.variables.create_pickle("sync_run_id", sync_run_id)
 
 
 if __name__ == "__main__":
     main()
```

