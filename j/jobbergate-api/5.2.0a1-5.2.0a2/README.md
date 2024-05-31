# Comparing `tmp/jobbergate_api-5.2.0a1.tar.gz` & `tmp/jobbergate_api-5.2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobbergate_api-5.2.0a1.tar", max compression
+gzip compressed data, was "jobbergate_api-5.2.0a2.tar", max compression
```

## Comparing `jobbergate_api-5.2.0a1.tar` & `jobbergate_api-5.2.0a2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1082 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/LICENSE
--rw-r--r--   0        0        0      683 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/README.md
--rw-r--r--   0        0        0      169 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/__init__.py
--rw-r--r--   0        0        0       30 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/__init__.py
--rw-r--r--   0        0        0       54 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/clusters/__init__.py
--rw-r--r--   0        0        0      944 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/clusters/models.py
--rw-r--r--   0        0        0     2114 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/clusters/routers.py
--rw-r--r--   0        0        0     1582 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/clusters/schemas.py
--rw-r--r--   0        0        0      177 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/constants.py
--rw-r--r--   0        0        0     5251 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/dependencies.py
--rw-r--r--   0        0        0     3620 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/file_validation.py
--rw-r--r--   0        0        0     1955 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/garbage_collector.py
--rw-r--r--   0        0        0       43 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_script_templates/__init__.py
--rw-r--r--   0        0        0      100 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_script_templates/constants.py
--rw-r--r--   0        0        0     4098 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_script_templates/models.py
--rw-r--r--   0        0        0    16611 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_script_templates/routers.py
--rw-r--r--   0        0        0     7060 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_script_templates/schemas.py
--rw-r--r--   0        0        0     3749 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_script_templates/services.py
--rw-r--r--   0        0        0       40 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_scripts/__init__.py
--rw-r--r--   0        0        0     2984 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_scripts/models.py
--rw-r--r--   0        0        0    14649 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_scripts/routers.py
--rw-r--r--   0        0        0     4759 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_scripts/schemas.py
--rw-r--r--   0        0        0     6483 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_scripts/services.py
--rw-r--r--   0        0        0     1295 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_scripts/tools.py
--rw-r--r--   0        0        0       44 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_submissions/__init__.py
--rw-r--r--   0        0        0     6561 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_submissions/constants.py
--rw-r--r--   0        0        0     3575 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_submissions/models.py
--rw-r--r--   0        0        0    14577 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_submissions/routers.py
--rw-r--r--   0        0        0     8208 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_submissions/schemas.py
--rw-r--r--   0        0        0     1285 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/job_submissions/services.py
--rw-r--r--   0        0        0     5986 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/models.py
--rw-r--r--   0        0        0     1065 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/permissions.py
--rw-r--r--   0        0        0     2254 2024-05-24 13:00:31.443983 jobbergate_api-5.2.0a1/jobbergate_api/apps/schemas.py
--rw-r--r--   0        0        0    25232 2024-05-24 13:00:31.447983 jobbergate_api-5.2.0a1/jobbergate_api/apps/services.py
--rw-r--r--   0        0        0     4589 2024-05-24 13:00:31.447983 jobbergate_api-5.2.0a1/jobbergate_api/config.py
--rw-r--r--   0        0        0     2467 2024-05-24 13:00:31.447983 jobbergate_api-5.2.0a1/jobbergate_api/email_notification.py
--rw-r--r--   0        0        0     1627 2024-05-24 13:00:31.447983 jobbergate_api-5.2.0a1/jobbergate_api/logging.py
--rw-r--r--   0        0        0     3622 2024-05-24 13:00:31.447983 jobbergate_api-5.2.0a1/jobbergate_api/main.py
--rw-r--r--   0        0        0     3436 2024-05-24 13:00:31.447983 jobbergate_api-5.2.0a1/jobbergate_api/meta_mapper.py
--rw-r--r--   0        0        0     2781 2024-05-24 13:00:31.447983 jobbergate_api-5.2.0a1/jobbergate_api/rabbitmq_notification.py
--rw-r--r--   0        0        0     1082 2024-05-24 13:00:31.447983 jobbergate_api-5.2.0a1/jobbergate_api/safe_types.py
--rw-r--r--   0        0        0     4598 2024-05-24 13:00:31.447983 jobbergate_api-5.2.0a1/jobbergate_api/security.py
--rw-r--r--   0        0        0    10874 2024-05-24 13:00:31.447983 jobbergate_api-5.2.0a1/jobbergate_api/storage.py
--rw-r--r--   0        0        0     1146 2024-05-24 13:00:31.447983 jobbergate_api-5.2.0a1/jobbergate_api/version.py
--rw-r--r--   0        0        0     4007 2024-05-24 13:00:31.447983 jobbergate_api-5.2.0a1/pyproject.toml
--rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 jobbergate_api-5.2.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/LICENSE
+-rw-r--r--   0        0        0      683 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/README.md
+-rw-r--r--   0        0        0      169 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/__init__.py
+-rw-r--r--   0        0        0       54 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/clusters/__init__.py
+-rw-r--r--   0        0        0      944 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/clusters/models.py
+-rw-r--r--   0        0        0     2114 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/clusters/routers.py
+-rw-r--r--   0        0        0     1582 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/clusters/schemas.py
+-rw-r--r--   0        0        0      177 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/constants.py
+-rw-r--r--   0        0        0     5251 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/dependencies.py
+-rw-r--r--   0        0        0     3620 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/file_validation.py
+-rw-r--r--   0        0        0     2177 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/garbage_collector.py
+-rw-r--r--   0        0        0       43 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/job_script_templates/__init__.py
+-rw-r--r--   0        0        0      100 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/job_script_templates/constants.py
+-rw-r--r--   0        0        0     4098 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/job_script_templates/models.py
+-rw-r--r--   0        0        0    16611 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/job_script_templates/routers.py
+-rw-r--r--   0        0        0     7060 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/job_script_templates/schemas.py
+-rw-r--r--   0        0        0     3749 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/job_script_templates/services.py
+-rw-r--r--   0        0        0       40 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/job_scripts/__init__.py
+-rw-r--r--   0        0        0     2984 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/job_scripts/models.py
+-rw-r--r--   0        0        0    14649 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/job_scripts/routers.py
+-rw-r--r--   0        0        0     4759 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/job_scripts/schemas.py
+-rw-r--r--   0        0        0     6988 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/job_scripts/services.py
+-rw-r--r--   0        0        0     1295 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/job_scripts/tools.py
+-rw-r--r--   0        0        0       44 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/job_submissions/__init__.py
+-rw-r--r--   0        0        0     6561 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/job_submissions/constants.py
+-rw-r--r--   0        0        0     3575 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/job_submissions/models.py
+-rw-r--r--   0        0        0    14577 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/job_submissions/routers.py
+-rw-r--r--   0        0        0     8208 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/job_submissions/schemas.py
+-rw-r--r--   0        0        0     1285 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/job_submissions/services.py
+-rw-r--r--   0        0        0     5986 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/models.py
+-rw-r--r--   0        0        0     1065 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/permissions.py
+-rw-r--r--   0        0        0     2254 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/schemas.py
+-rw-r--r--   0        0        0    25232 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/apps/services.py
+-rw-r--r--   0        0        0     4589 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/config.py
+-rw-r--r--   0        0        0     2467 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/email_notification.py
+-rw-r--r--   0        0        0     1627 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/logging.py
+-rw-r--r--   0        0        0     3622 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/main.py
+-rw-r--r--   0        0        0     3436 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/meta_mapper.py
+-rw-r--r--   0        0        0     2781 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/rabbitmq_notification.py
+-rw-r--r--   0        0        0     1082 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/safe_types.py
+-rw-r--r--   0        0        0     4598 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/security.py
+-rw-r--r--   0        0        0    10874 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/storage.py
+-rw-r--r--   0        0        0     1146 2024-05-31 17:18:22.423034 jobbergate_api-5.2.0a2/jobbergate_api/version.py
+-rw-r--r--   0        0        0     4007 2024-05-31 17:18:22.427034 jobbergate_api-5.2.0a2/pyproject.toml
+-rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 jobbergate_api-5.2.0a2/PKG-INFO
```

### Comparing `jobbergate_api-5.2.0a1/LICENSE` & `jobbergate_api-5.2.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/README.md` & `jobbergate_api-5.2.0a2/README.md`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/apps/clusters/models.py` & `jobbergate_api-5.2.0a2/jobbergate_api/apps/clusters/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/apps/clusters/routers.py` & `jobbergate_api-5.2.0a2/jobbergate_api/apps/clusters/routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/apps/clusters/schemas.py` & `jobbergate_api-5.2.0a2/jobbergate_api/apps/clusters/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/apps/dependencies.py` & `jobbergate_api-5.2.0a2/jobbergate_api/apps/dependencies.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/apps/file_validation.py` & `jobbergate_api-5.2.0a2/jobbergate_api/apps/file_validation.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/apps/garbage_collector.py` & `jobbergate_api-5.2.0a2/jobbergate_api/apps/garbage_collector.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Delete unused files from jobbergate's file storage."""
 
+import asyncio
+
 from fastapi import BackgroundTasks
 from loguru import logger
 from sqlalchemy import select
 
 
 async def get_set_of_files_from_database(session, table) -> set[str]:
     """Get a set of files from the database."""
@@ -28,18 +30,25 @@
     result = files_in_bucket - files_in_database
     logger.debug(f"Total of files to be garbage collected: {len(result)}")
     return result
 
 
 async def delete_files_from_bucket(bucket, files_to_delete: set[str]) -> None:
     """Delete files from the bucket."""
-    for file_to_delete in files_to_delete:
-        file = await bucket.Object(file_to_delete)
-        await file.delete()
-        logger.debug(f"Deleted file {file_to_delete} from bucket {bucket.name}")
+    MAX_CONCURRENT_REQUESTS = 25
+    semaphore = asyncio.Semaphore(MAX_CONCURRENT_REQUESTS)
+
+    async def delete_file(file: str) -> None:
+        async with semaphore:
+            obj = await bucket.Object(file)
+            await obj.delete()
+        logger.debug(f"Deleted file {file} from bucket {bucket.name}")
+
+    tasks = [delete_file(file) for file in files_to_delete]
+    await asyncio.gather(*tasks)
 
 
 async def garbage_collect(session, bucket, list_of_tables, background_tasks: BackgroundTasks) -> None:
     """Delete unused files from jobbergate's file storage."""
     for table in list_of_tables:
         files_to_delete = await get_files_to_delete(session, table, bucket)
         if files_to_delete:
```

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/apps/job_script_templates/models.py` & `jobbergate_api-5.2.0a2/jobbergate_api/apps/job_script_templates/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/apps/job_script_templates/routers.py` & `jobbergate_api-5.2.0a2/jobbergate_api/apps/job_script_templates/routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/apps/job_script_templates/schemas.py` & `jobbergate_api-5.2.0a2/jobbergate_api/apps/job_script_templates/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/apps/job_script_templates/services.py` & `jobbergate_api-5.2.0a2/jobbergate_api/apps/job_script_templates/services.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/apps/job_scripts/models.py` & `jobbergate_api-5.2.0a2/jobbergate_api/apps/job_scripts/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/apps/job_scripts/routers.py` & `jobbergate_api-5.2.0a2/jobbergate_api/apps/job_scripts/routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/apps/job_scripts/schemas.py` & `jobbergate_api-5.2.0a2/jobbergate_api/apps/job_scripts/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/apps/job_scripts/services.py` & `jobbergate_api-5.2.0a2/jobbergate_api/apps/job_scripts/services.py`

 * *Files 15% similar despite different names*

```diff
@@ -60,57 +60,62 @@
         Automatically clean unused job scripts depending on a threshold.
 
         Based on the last time each job script was updated or used to create a job submission,
         this will archived job scripts that were unarchived and delete jos script that were archived.
         """
         result = AutoCleanResponse(archived=set(), deleted=set())
 
-        subquery = (
-            select(
-                JobSubmission.job_script_id,
-                func.max(JobSubmission.created_at).label("last_used"),
-            )  # type: ignore
-            .group_by(JobSubmission.job_script_id)
-            .subquery()
-        )
-        joined_query = (
-            select(self.model_type, subquery)  # type: ignore
-            .join(subquery, subquery.c.job_script_id == self.model_type.id, isouter=True)
-            .subquery()
-        )
-
         if days_to_delete := settings.AUTO_CLEAN_JOB_SCRIPTS_DAYS_TO_DELETE:
-            query = (
+            threshold = PendulumDateTime.utcnow().subtract(days=days_to_delete).naive()
+            subquery_unused_job_script = select(self.model_type.id).where(
+                self.model_type.is_archived.is_(True), self.model_type.updated_at < threshold
+            )
+            subquery_recent_child = (
+                select(JobSubmission.job_script_id)
+                .where(JobSubmission.job_script_id.in_(subquery_unused_job_script))
+                .group_by(JobSubmission.job_script_id)
+                .having(func.max(JobSubmission.created_at) >= threshold)
+            )
+
+            delete_query = (
                 delete(self.model_type)  # type: ignore
-                .where(self.model_type.is_archived.is_(True))
                 .where(
-                    func.greatest(joined_query.c.updated_at, joined_query.c.last_used)
-                    < PendulumDateTime.utcnow().subtract(days=days_to_delete).naive()
+                    self.model_type.id.in_(subquery_unused_job_script),
+                    ~self.model_type.id.in_(subquery_recent_child),
                 )
                 .returning(self.model_type.id)
             )
-            deleted = await self.session.execute(query)
+            deleted = await self.session.execute(delete_query)
             result.deleted.update(row[0] for row in deleted.all())
+        logger.debug(f"Job scripts deleted: {result.deleted}")
 
         if days_to_archive := settings.AUTO_CLEAN_JOB_SCRIPTS_DAYS_TO_ARCHIVE:
+            threshold = PendulumDateTime.utcnow().subtract(days=days_to_archive).naive()
+            subquery_unused_job_script = select(self.model_type.id).where(
+                self.model_type.is_archived.is_(False), self.model_type.updated_at < threshold
+            )
+            subquery_recent_child = (
+                select(JobSubmission.job_script_id)
+                .where(JobSubmission.job_script_id.in_(subquery_unused_job_script))
+                .group_by(JobSubmission.job_script_id)
+                .having(func.max(JobSubmission.created_at) >= threshold)
+            )
+
             update_query = (
                 update(self.model_type)  # type: ignore
-                .where(self.model_type.is_archived.is_(False))
                 .where(
-                    func.greatest(joined_query.c.updated_at, joined_query.c.last_used)
-                    < PendulumDateTime.utcnow().subtract(days=days_to_archive).naive()
+                    self.model_type.id.in_(subquery_unused_job_script),
+                    ~self.model_type.id.in_(subquery_recent_child),
                 )
                 .values(is_archived=True)
                 .returning(self.model_type.id)
             )
             archived = await self.session.execute(update_query)
             result.archived.update(row[0] for row in archived.all())
-
         logger.debug(f"Job scripts marked as archived: {result.archived}")
-        logger.debug(f"Job scripts marked as deleted: {result.deleted}")
 
         return result
 
 
 class JobScriptFileService(FileService):
     """
     Provide an empty derived class of FileService.
```

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/apps/job_scripts/tools.py` & `jobbergate_api-5.2.0a2/jobbergate_api/apps/job_scripts/tools.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/apps/job_submissions/constants.py` & `jobbergate_api-5.2.0a2/jobbergate_api/apps/job_submissions/constants.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/apps/job_submissions/models.py` & `jobbergate_api-5.2.0a2/jobbergate_api/apps/job_submissions/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/apps/job_submissions/routers.py` & `jobbergate_api-5.2.0a2/jobbergate_api/apps/job_submissions/routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/apps/job_submissions/schemas.py` & `jobbergate_api-5.2.0a2/jobbergate_api/apps/job_submissions/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/apps/job_submissions/services.py` & `jobbergate_api-5.2.0a2/jobbergate_api/apps/job_submissions/services.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/apps/models.py` & `jobbergate_api-5.2.0a2/jobbergate_api/apps/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/apps/permissions.py` & `jobbergate_api-5.2.0a2/jobbergate_api/apps/permissions.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/apps/schemas.py` & `jobbergate_api-5.2.0a2/jobbergate_api/apps/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/apps/services.py` & `jobbergate_api-5.2.0a2/jobbergate_api/apps/services.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/config.py` & `jobbergate_api-5.2.0a2/jobbergate_api/config.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/email_notification.py` & `jobbergate_api-5.2.0a2/jobbergate_api/email_notification.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/logging.py` & `jobbergate_api-5.2.0a2/jobbergate_api/logging.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/main.py` & `jobbergate_api-5.2.0a2/jobbergate_api/main.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/meta_mapper.py` & `jobbergate_api-5.2.0a2/jobbergate_api/meta_mapper.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/rabbitmq_notification.py` & `jobbergate_api-5.2.0a2/jobbergate_api/rabbitmq_notification.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/safe_types.py` & `jobbergate_api-5.2.0a2/jobbergate_api/safe_types.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/security.py` & `jobbergate_api-5.2.0a2/jobbergate_api/security.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/storage.py` & `jobbergate_api-5.2.0a2/jobbergate_api/storage.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/jobbergate_api/version.py` & `jobbergate_api-5.2.0a2/jobbergate_api/version.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-5.2.0a1/pyproject.toml` & `jobbergate_api-5.2.0a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jobbergate-api"
-version = "5.2.0a1"
+version = "5.2.0a2"
 description = "Jobbergate API"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/omnivector-solutions/jobbergate"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `jobbergate_api-5.2.0a1/PKG-INFO` & `jobbergate_api-5.2.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobbergate-api
-Version: 5.2.0a1
+Version: 5.2.0a2
 Summary: Jobbergate API
 Home-page: https://github.com/omnivector-solutions/jobbergate
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

