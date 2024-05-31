# Comparing `tmp/jobbergate_agent-5.2.0a1.tar.gz` & `tmp/jobbergate_agent-5.2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobbergate_agent-5.2.0a1.tar", max compression
+gzip compressed data, was "jobbergate_agent-5.2.0a2.tar", max compression
```

## Comparing `jobbergate_agent-5.2.0a1.tar` & `jobbergate_agent-5.2.0a2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1077 2024-05-24 13:00:30.018884 jobbergate_agent-5.2.0a1/LICENSE
--rw-r--r--   0        0        0     1346 2024-05-24 13:00:30.018884 jobbergate_agent-5.2.0a1/README.md
--rw-r--r--   0        0        0        0 2024-05-24 13:00:30.018884 jobbergate_agent-5.2.0a1/jobbergate_agent/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 13:00:30.018884 jobbergate_agent-5.2.0a1/jobbergate_agent/clients/__init__.py
--rw-r--r--   0        0        0     3597 2024-05-24 13:00:30.018884 jobbergate_agent-5.2.0a1/jobbergate_agent/clients/cluster_api.py
--rw-r--r--   0        0        0        0 2024-05-24 13:00:30.018884 jobbergate_agent-5.2.0a1/jobbergate_agent/internals/__init__.py
--rw-r--r--   0        0        0     4284 2024-05-24 13:00:30.018884 jobbergate_agent-5.2.0a1/jobbergate_agent/internals/update.py
--rw-r--r--   0        0        0        0 2024-05-24 13:00:30.018884 jobbergate_agent-5.2.0a1/jobbergate_agent/jobbergate/__init__.py
--rw-r--r--   0        0        0      150 2024-05-24 13:00:30.018884 jobbergate_agent-5.2.0a1/jobbergate_agent/jobbergate/constants.py
--rw-r--r--   0        0        0      636 2024-05-24 13:00:30.018884 jobbergate_agent-5.2.0a1/jobbergate_agent/jobbergate/report_health.py
--rw-r--r--   0        0        0     2805 2024-05-24 13:00:30.018884 jobbergate_agent-5.2.0a1/jobbergate_agent/jobbergate/schemas.py
--rw-r--r--   0        0        0    11828 2024-05-24 13:00:30.018884 jobbergate_agent-5.2.0a1/jobbergate_agent/jobbergate/submit.py
--rw-r--r--   0        0        0     3676 2024-05-24 13:00:30.018884 jobbergate_agent-5.2.0a1/jobbergate_agent/jobbergate/update.py
--rw-r--r--   0        0        0      491 2024-05-24 13:00:30.018884 jobbergate_agent-5.2.0a1/jobbergate_agent/main.py
--rw-r--r--   0        0        0     2759 2024-05-24 13:00:30.018884 jobbergate_agent-5.2.0a1/jobbergate_agent/settings.py
--rw-r--r--   0        0        0     3035 2024-05-24 13:00:30.018884 jobbergate_agent-5.2.0a1/jobbergate_agent/tasks.py
--rw-r--r--   0        0        0        0 2024-05-24 13:00:30.018884 jobbergate_agent-5.2.0a1/jobbergate_agent/utils/__init__.py
--rw-r--r--   0        0        0     4663 2024-05-24 13:00:30.018884 jobbergate_agent-5.2.0a1/jobbergate_agent/utils/exception.py
--rw-r--r--   0        0        0     1440 2024-05-24 13:00:30.018884 jobbergate_agent-5.2.0a1/jobbergate_agent/utils/logging.py
--rw-r--r--   0        0        0     1414 2024-05-24 13:00:30.018884 jobbergate_agent-5.2.0a1/jobbergate_agent/utils/plugin.py
--rw-r--r--   0        0        0     2153 2024-05-24 13:00:30.018884 jobbergate_agent-5.2.0a1/jobbergate_agent/utils/scheduler.py
--rw-r--r--   0        0        0      730 2024-05-24 13:00:30.018884 jobbergate_agent-5.2.0a1/jobbergate_agent/utils/sentry.py
--rw-r--r--   0        0        0     2500 2024-05-24 13:00:30.018884 jobbergate_agent-5.2.0a1/jobbergate_agent/utils/user_mapper.py
--rw-r--r--   0        0        0     3320 2024-05-24 13:00:30.022884 jobbergate_agent-5.2.0a1/pyproject.toml
--rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 jobbergate_agent-5.2.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-31 17:18:21.108158 jobbergate_agent-5.2.0a2/LICENSE
+-rw-r--r--   0        0        0     1346 2024-05-31 17:18:21.108158 jobbergate_agent-5.2.0a2/README.md
+-rw-r--r--   0        0        0        0 2024-05-31 17:18:21.108158 jobbergate_agent-5.2.0a2/jobbergate_agent/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 17:18:21.108158 jobbergate_agent-5.2.0a2/jobbergate_agent/clients/__init__.py
+-rw-r--r--   0        0        0     3597 2024-05-31 17:18:21.108158 jobbergate_agent-5.2.0a2/jobbergate_agent/clients/cluster_api.py
+-rw-r--r--   0        0        0        0 2024-05-31 17:18:21.108158 jobbergate_agent-5.2.0a2/jobbergate_agent/internals/__init__.py
+-rw-r--r--   0        0        0     4284 2024-05-31 17:18:21.108158 jobbergate_agent-5.2.0a2/jobbergate_agent/internals/update.py
+-rw-r--r--   0        0        0        0 2024-05-31 17:18:21.108158 jobbergate_agent-5.2.0a2/jobbergate_agent/jobbergate/__init__.py
+-rw-r--r--   0        0        0      150 2024-05-31 17:18:21.108158 jobbergate_agent-5.2.0a2/jobbergate_agent/jobbergate/constants.py
+-rw-r--r--   0        0        0      636 2024-05-31 17:18:21.108158 jobbergate_agent-5.2.0a2/jobbergate_agent/jobbergate/report_health.py
+-rw-r--r--   0        0        0     2266 2024-05-31 17:18:21.108158 jobbergate_agent-5.2.0a2/jobbergate_agent/jobbergate/schemas.py
+-rw-r--r--   0        0        0    11828 2024-05-31 17:18:21.108158 jobbergate_agent-5.2.0a2/jobbergate_agent/jobbergate/submit.py
+-rw-r--r--   0        0        0     3676 2024-05-31 17:18:21.108158 jobbergate_agent-5.2.0a2/jobbergate_agent/jobbergate/update.py
+-rw-r--r--   0        0        0      491 2024-05-31 17:18:21.108158 jobbergate_agent-5.2.0a2/jobbergate_agent/main.py
+-rw-r--r--   0        0        0     2759 2024-05-31 17:18:21.108158 jobbergate_agent-5.2.0a2/jobbergate_agent/settings.py
+-rw-r--r--   0        0        0     3035 2024-05-31 17:18:21.108158 jobbergate_agent-5.2.0a2/jobbergate_agent/tasks.py
+-rw-r--r--   0        0        0        0 2024-05-31 17:18:21.108158 jobbergate_agent-5.2.0a2/jobbergate_agent/utils/__init__.py
+-rw-r--r--   0        0        0     4663 2024-05-31 17:18:21.108158 jobbergate_agent-5.2.0a2/jobbergate_agent/utils/exception.py
+-rw-r--r--   0        0        0     1440 2024-05-31 17:18:21.108158 jobbergate_agent-5.2.0a2/jobbergate_agent/utils/logging.py
+-rw-r--r--   0        0        0     1414 2024-05-31 17:18:21.108158 jobbergate_agent-5.2.0a2/jobbergate_agent/utils/plugin.py
+-rw-r--r--   0        0        0     2153 2024-05-31 17:18:21.108158 jobbergate_agent-5.2.0a2/jobbergate_agent/utils/scheduler.py
+-rw-r--r--   0        0        0      730 2024-05-31 17:18:21.108158 jobbergate_agent-5.2.0a2/jobbergate_agent/utils/sentry.py
+-rw-r--r--   0        0        0     2500 2024-05-31 17:18:21.108158 jobbergate_agent-5.2.0a2/jobbergate_agent/utils/user_mapper.py
+-rw-r--r--   0        0        0     3320 2024-05-31 17:18:21.108158 jobbergate_agent-5.2.0a2/pyproject.toml
+-rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 jobbergate_agent-5.2.0a2/PKG-INFO
```

### Comparing `jobbergate_agent-5.2.0a1/LICENSE` & `jobbergate_agent-5.2.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.2.0a1/README.md` & `jobbergate_agent-5.2.0a2/README.md`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.2.0a1/jobbergate_agent/clients/cluster_api.py` & `jobbergate_agent-5.2.0a2/jobbergate_agent/clients/cluster_api.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.2.0a1/jobbergate_agent/internals/update.py` & `jobbergate_agent-5.2.0a2/jobbergate_agent/internals/update.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.2.0a1/jobbergate_agent/jobbergate/report_health.py` & `jobbergate_agent-5.2.0a2/jobbergate_agent/jobbergate/report_health.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.2.0a1/jobbergate_agent/jobbergate/schemas.py` & `jobbergate_agent-5.2.0a2/jobbergate_agent/jobbergate/schemas.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,38 +43,14 @@
     Specialized model for the cluster-agent to pull an active job_submission.
     """
 
     id: int
     slurm_job_id: int
 
 
-class SlurmJobParams(pydantic.BaseModel):
-    """
-    Specialized model for describing job submission parameters for Slurm REST API.
-    """
-
-    name: str
-    get_user_environment: int = 1
-    standard_error: Optional[Path]
-    standard_output: Optional[Path]
-    current_working_directory: Optional[Path]
-
-    class Config:
-        extra = "allow"
-
-
-class SlurmJobSubmission(pydantic.BaseModel):
-    """
-    Specialized model for describing a request to submit a job to Slurm REST API.
-    """
-
-    script: str
-    job: SlurmJobParams
-
-
 class SlurmSubmitError(pydantic.BaseModel):
     """
     Specialized model for error content in a SlurmSubmitResponse.
     """
 
     error: Optional[str]
     error_code: Optional[int] = pydantic.Field(alias="errno")
```

### Comparing `jobbergate_agent-5.2.0a1/jobbergate_agent/jobbergate/submit.py` & `jobbergate_agent-5.2.0a2/jobbergate_agent/jobbergate/submit.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
 
 
 async def submit_job_script(
     pending_job_submission: PendingJobSubmission,
     user_mapper: SlurmUserMapper,
 ) -> int:
     """
-    Submit a Job Script to slurm via the Slurm REST API.
+    Submit a Job Script to slurm via the sbatch command.
 
     :param: pending_job_submission: A job_submission with fields needed to submit.
     :returns: The ``slurm_job_id`` for the submitted job
     """
     logger.debug(f"Submitting {pending_job_submission}")
 
     async def _reject_handler(params: DoExceptParams):
```

### Comparing `jobbergate_agent-5.2.0a1/jobbergate_agent/jobbergate/update.py` & `jobbergate_agent-5.2.0a2/jobbergate_agent/jobbergate/update.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.2.0a1/jobbergate_agent/settings.py` & `jobbergate_agent-5.2.0a2/jobbergate_agent/settings.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.2.0a1/jobbergate_agent/tasks.py` & `jobbergate_agent-5.2.0a2/jobbergate_agent/tasks.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.2.0a1/jobbergate_agent/utils/exception.py` & `jobbergate_agent-5.2.0a2/jobbergate_agent/utils/exception.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.2.0a1/jobbergate_agent/utils/logging.py` & `jobbergate_agent-5.2.0a2/jobbergate_agent/utils/logging.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.2.0a1/jobbergate_agent/utils/plugin.py` & `jobbergate_agent-5.2.0a2/jobbergate_agent/utils/plugin.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.2.0a1/jobbergate_agent/utils/scheduler.py` & `jobbergate_agent-5.2.0a2/jobbergate_agent/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.2.0a1/jobbergate_agent/utils/sentry.py` & `jobbergate_agent-5.2.0a2/jobbergate_agent/utils/sentry.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.2.0a1/jobbergate_agent/utils/user_mapper.py` & `jobbergate_agent-5.2.0a2/jobbergate_agent/utils/user_mapper.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.2.0a1/pyproject.toml` & `jobbergate_agent-5.2.0a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jobbergate-agent"
-version = "5.2.0a1"
+version = "5.2.0a2"
 description = "Jobbergate Agent"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/omnivector-solutions/jobbergate"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `jobbergate_agent-5.2.0a1/PKG-INFO` & `jobbergate_agent-5.2.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobbergate-agent
-Version: 5.2.0a1
+Version: 5.2.0a2
 Summary: Jobbergate Agent
 Home-page: https://github.com/omnivector-solutions/jobbergate
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: apscheduler (==3.10.3)
 Requires-Dist: auto-name-enum (>=2.0.0,<3.0.0)
 Requires-Dist: httpx (==0.24.1)
 Requires-Dist: importlib-metadata (>=6.8.0,<7.0.0) ; python_version < "3.10"
-Requires-Dist: jobbergate-core (==5.2.0a1)
+Requires-Dist: jobbergate-core (==5.2.0a2)
 Requires-Dist: loguru (==0.6.0)
 Requires-Dist: py-buzz (>=4.0.0,<5.0.0)
 Requires-Dist: pydantic (==1.10.13)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: python-jose (==3.3.0)
 Requires-Dist: sentry-sdk (>=1.1.0,<2.0.0)
```

