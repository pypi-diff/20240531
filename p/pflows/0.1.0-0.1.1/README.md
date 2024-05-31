# Comparing `tmp/pflows-0.1.0.tar.gz` & `tmp/pflows-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pflows-0.1.0.tar", last modified: Mon May 27 19:22:00 2024, max compression
+gzip compressed data, was "pflows-0.1.1.tar", last modified: Fri May 31 15:25:44 2024, max compression
```

## Comparing `pflows-0.1.0.tar` & `pflows-0.1.1.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 dperezrada   (501) staff       (20)        0 2024-05-27 19:22:00.258331 pflows-0.1.0/
--rw-r--r--   0 dperezrada   (501) staff       (20)     1077 2024-05-12 16:29:53.000000 pflows-0.1.0/LICENSE
--rw-r--r--   0 dperezrada   (501) staff       (20)     3950 2024-05-27 19:22:00.258143 pflows-0.1.0/PKG-INFO
--rw-r--r--   0 dperezrada   (501) staff       (20)     2643 2024-05-27 19:17:33.000000 pflows-0.1.0/README.md
--rw-r--r--   0 dperezrada   (501) staff       (20)     1482 2024-05-27 19:17:33.000000 pflows-0.1.0/pyproject.toml
--rw-r--r--   0 dperezrada   (501) staff       (20)      254 2024-05-24 22:10:01.000000 pflows-0.1.0/requirements.txt
--rw-r--r--   0 dperezrada   (501) staff       (20)      102 2024-05-15 15:25:27.000000 pflows-0.1.0/requirements_dev.txt
--rw-r--r--   0 dperezrada   (501) staff       (20)       38 2024-05-27 19:22:00.258378 pflows-0.1.0/setup.cfg
-drwxr-xr-x   0 dperezrada   (501) staff       (20)        0 2024-05-27 19:22:00.253035 pflows-0.1.0/src/
--rw-r--r--   0 dperezrada   (501) staff       (20)        0 2024-05-12 17:27:48.000000 pflows-0.1.0/src/__init__.py
--rw-r--r--   0 dperezrada   (501) staff       (20)     6938 2024-05-27 19:17:33.000000 pflows-0.1.0/src/modal_server.py
-drwxr-xr-x   0 dperezrada   (501) staff       (20)        0 2024-05-27 19:22:00.254396 pflows-0.1.0/src/pflows/
--rw-r--r--   0 dperezrada   (501) staff       (20)        0 2024-05-12 21:27:45.000000 pflows-0.1.0/src/pflows/__init__.py
--rw-r--r--   0 dperezrada   (501) staff       (20)     1474 2024-05-27 19:17:33.000000 pflows-0.1.0/src/pflows/cli.py
--rw-r--r--   0 dperezrada   (501) staff       (20)      635 2024-05-27 19:17:33.000000 pflows-0.1.0/src/pflows/model.py
--rw-r--r--   0 dperezrada   (501) staff       (20)     2879 2024-05-27 19:17:33.000000 pflows-0.1.0/src/pflows/polygons.py
-drwxr-xr-x   0 dperezrada   (501) staff       (20)        0 2024-05-27 19:22:00.256833 pflows-0.1.0/src/pflows/tools/
--rw-r--r--   0 dperezrada   (501) staff       (20)        0 2024-05-12 15:44:18.000000 pflows-0.1.0/src/pflows/tools/__init__.py
--rw-r--r--   0 dperezrada   (501) staff       (20)      224 2024-05-27 19:17:33.000000 pflows-0.1.0/src/pflows/tools/annotations.py
--rw-r--r--   0 dperezrada   (501) staff       (20)     8681 2024-05-27 19:17:33.000000 pflows-0.1.0/src/pflows/tools/augmentations.py
--rw-r--r--   0 dperezrada   (501) staff       (20)     3709 2024-05-27 19:17:33.000000 pflows-0.1.0/src/pflows/tools/base.py
--rw-r--r--   0 dperezrada   (501) staff       (20)     7599 2024-05-27 19:17:33.000000 pflows-0.1.0/src/pflows/tools/categories.py
--rw-r--r--   0 dperezrada   (501) staff       (20)     3374 2024-05-27 19:17:33.000000 pflows-0.1.0/src/pflows/tools/dataset.py
--rw-r--r--   0 dperezrada   (501) staff       (20)     1702 2024-05-27 19:17:33.000000 pflows-0.1.0/src/pflows/tools/filter_images.py
--rw-r--r--   0 dperezrada   (501) staff       (20)     1027 2024-05-15 15:16:32.000000 pflows-0.1.0/src/pflows/tools/roboflow_tools.py
--rw-r--r--   0 dperezrada   (501) staff       (20)    16567 2024-05-27 19:17:33.000000 pflows-0.1.0/src/pflows/tools/yolo_v8.py
--rw-r--r--   0 dperezrada   (501) staff       (20)     1000 2024-05-26 21:00:48.000000 pflows-0.1.0/src/pflows/typedef.py
--rw-r--r--   0 dperezrada   (501) staff       (20)     8198 2024-05-27 19:17:33.000000 pflows-0.1.0/src/pflows/workflow.py
-drwxr-xr-x   0 dperezrada   (501) staff       (20)        0 2024-05-27 19:22:00.257593 pflows-0.1.0/src/pflows.egg-info/
--rw-r--r--   0 dperezrada   (501) staff       (20)     3950 2024-05-27 19:22:00.000000 pflows-0.1.0/src/pflows.egg-info/PKG-INFO
--rw-r--r--   0 dperezrada   (501) staff       (20)      740 2024-05-27 19:22:00.000000 pflows-0.1.0/src/pflows.egg-info/SOURCES.txt
--rw-r--r--   0 dperezrada   (501) staff       (20)        1 2024-05-27 19:22:00.000000 pflows-0.1.0/src/pflows.egg-info/dependency_links.txt
--rw-r--r--   0 dperezrada   (501) staff       (20)       43 2024-05-27 19:22:00.000000 pflows-0.1.0/src/pflows.egg-info/entry_points.txt
--rw-r--r--   0 dperezrada   (501) staff       (20)      364 2024-05-27 19:22:00.000000 pflows-0.1.0/src/pflows.egg-info/requires.txt
--rw-r--r--   0 dperezrada   (501) staff       (20)       29 2024-05-27 19:22:00.000000 pflows-0.1.0/src/pflows.egg-info/top_level.txt
-drwxr-xr-x   0 dperezrada   (501) staff       (20)        0 2024-05-27 19:22:00.257269 pflows-0.1.0/tests/
--rw-r--r--   0 dperezrada   (501) staff       (20)     1424 2024-05-27 19:17:33.000000 pflows-0.1.0/tests/test_workflow.py
+drwxr-xr-x   0 dperezrada   (501) staff       (20)        0 2024-05-31 15:25:44.611008 pflows-0.1.1/
+-rw-r--r--   0 dperezrada   (501) staff       (20)     1077 2024-05-12 16:29:53.000000 pflows-0.1.1/LICENSE
+-rw-r--r--   0 dperezrada   (501) staff       (20)     4022 2024-05-31 15:25:44.610793 pflows-0.1.1/PKG-INFO
+-rw-r--r--   0 dperezrada   (501) staff       (20)     2643 2024-05-31 14:56:45.000000 pflows-0.1.1/README.md
+-rw-r--r--   0 dperezrada   (501) staff       (20)     1482 2024-05-31 15:25:27.000000 pflows-0.1.1/pyproject.toml
+-rw-r--r--   0 dperezrada   (501) staff       (20)      296 2024-05-31 14:56:45.000000 pflows-0.1.1/requirements.txt
+-rw-r--r--   0 dperezrada   (501) staff       (20)      102 2024-05-15 15:25:27.000000 pflows-0.1.1/requirements_dev.txt
+-rw-r--r--   0 dperezrada   (501) staff       (20)       38 2024-05-31 15:25:44.611054 pflows-0.1.1/setup.cfg
+drwxr-xr-x   0 dperezrada   (501) staff       (20)        0 2024-05-31 15:25:44.604267 pflows-0.1.1/src/
+-rw-r--r--   0 dperezrada   (501) staff       (20)        0 2024-05-12 17:27:48.000000 pflows-0.1.1/src/__init__.py
+-rw-r--r--   0 dperezrada   (501) staff       (20)     9880 2024-05-31 14:56:45.000000 pflows-0.1.1/src/modal_server.py
+drwxr-xr-x   0 dperezrada   (501) staff       (20)        0 2024-05-31 15:25:44.605015 pflows-0.1.1/src/pflows/
+-rw-r--r--   0 dperezrada   (501) staff       (20)        0 2024-05-31 14:56:45.000000 pflows-0.1.1/src/pflows/__init__.py
+-rw-r--r--   0 dperezrada   (501) staff       (20)     1474 2024-05-31 14:56:45.000000 pflows-0.1.1/src/pflows/cli.py
+-rw-r--r--   0 dperezrada   (501) staff       (20)      635 2024-05-31 14:56:45.000000 pflows-0.1.1/src/pflows/model.py
+-rw-r--r--   0 dperezrada   (501) staff       (20)     2879 2024-05-31 14:56:45.000000 pflows-0.1.1/src/pflows/polygons.py
+drwxr-xr-x   0 dperezrada   (501) staff       (20)        0 2024-05-31 15:25:44.609578 pflows-0.1.1/src/pflows/tools/
+-rw-r--r--   0 dperezrada   (501) staff       (20)        0 2024-05-31 14:56:45.000000 pflows-0.1.1/src/pflows/tools/__init__.py
+-rw-r--r--   0 dperezrada   (501) staff       (20)      224 2024-05-31 14:56:45.000000 pflows-0.1.1/src/pflows/tools/annotations.py
+-rw-r--r--   0 dperezrada   (501) staff       (20)     8681 2024-05-31 14:56:45.000000 pflows-0.1.1/src/pflows/tools/augmentations.py
+-rw-r--r--   0 dperezrada   (501) staff       (20)     4501 2024-05-31 14:56:45.000000 pflows-0.1.1/src/pflows/tools/base.py
+-rw-r--r--   0 dperezrada   (501) staff       (20)     7599 2024-05-31 14:56:45.000000 pflows-0.1.1/src/pflows/tools/categories.py
+-rw-r--r--   0 dperezrada   (501) staff       (20)     3830 2024-05-31 14:56:45.000000 pflows-0.1.1/src/pflows/tools/dataset.py
+-rw-r--r--   0 dperezrada   (501) staff       (20)     1931 2024-05-31 14:56:45.000000 pflows-0.1.1/src/pflows/tools/filter_images.py
+-rw-r--r--   0 dperezrada   (501) staff       (20)     4470 2024-05-31 14:56:45.000000 pflows-0.1.1/src/pflows/tools/pflows_remote.py
+-rw-r--r--   0 dperezrada   (501) staff       (20)     1027 2024-05-31 14:56:45.000000 pflows-0.1.1/src/pflows/tools/roboflow_tools.py
+-rw-r--r--   0 dperezrada   (501) staff       (20)    16567 2024-05-31 14:56:45.000000 pflows-0.1.1/src/pflows/tools/yolo_v8.py
+-rw-r--r--   0 dperezrada   (501) staff       (20)     1000 2024-05-31 14:56:45.000000 pflows-0.1.1/src/pflows/typedef.py
+-rw-r--r--   0 dperezrada   (501) staff       (20)     8230 2024-05-31 14:56:45.000000 pflows-0.1.1/src/pflows/workflow.py
+drwxr-xr-x   0 dperezrada   (501) staff       (20)        0 2024-05-31 15:25:44.610192 pflows-0.1.1/src/pflows.egg-info/
+-rw-r--r--   0 dperezrada   (501) staff       (20)     4022 2024-05-31 15:25:44.000000 pflows-0.1.1/src/pflows.egg-info/PKG-INFO
+-rw-r--r--   0 dperezrada   (501) staff       (20)      774 2024-05-31 15:25:44.000000 pflows-0.1.1/src/pflows.egg-info/SOURCES.txt
+-rw-r--r--   0 dperezrada   (501) staff       (20)        1 2024-05-31 15:25:44.000000 pflows-0.1.1/src/pflows.egg-info/dependency_links.txt
+-rw-r--r--   0 dperezrada   (501) staff       (20)       43 2024-05-31 15:25:44.000000 pflows-0.1.1/src/pflows.egg-info/entry_points.txt
+-rw-r--r--   0 dperezrada   (501) staff       (20)      406 2024-05-31 15:25:44.000000 pflows-0.1.1/src/pflows.egg-info/requires.txt
+-rw-r--r--   0 dperezrada   (501) staff       (20)       35 2024-05-31 15:25:44.000000 pflows-0.1.1/src/pflows.egg-info/top_level.txt
+drwxr-xr-x   0 dperezrada   (501) staff       (20)        0 2024-05-31 15:25:44.609736 pflows-0.1.1/tests/
+-rw-r--r--   0 dperezrada   (501) staff       (20)     1163 2024-05-31 14:56:45.000000 pflows-0.1.1/tests/test_workflow.py
```

### Comparing `pflows-0.1.0/LICENSE` & `pflows-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pflows-0.1.0/PKG-INFO` & `pflows-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pflows
-Version: 0.1.0
+Version: 0.1.1
 Summary: Several tools for dealing with image annotations to train YOLO or similar models
 Author-email: Daniel Pérez Rada <dperezrada@gmail.com>
 Maintainer-email: Daniel Pérez Rada <dperezrada@gmail.com>
 License: MIT license
 Project-URL: bugs, https://github.com/dperezrada/pflows/issues
 Project-URL: changelog, https://github.com/dperezrada/pflows/blob/master/changelog.md
 Project-URL: homepage, https://github.com/dperezrada/pflows
@@ -19,14 +19,16 @@
 Requires-Dist: opencv-python-headless==4.8.0.74
 Requires-Dist: shapely==2.0.4
 Requires-Dist: albumentations==1.3.1
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: fastapi==0.111.0
 Requires-Dist: fastapi-cli==0.0.4
 Requires-Dist: modal==0.62.181
+Requires-Dist: requests==2.31.0
+Requires-Dist: requests-toolbelt==1.0.0
 Provides-Extra: dev
 Requires-Dist: pytest==6.2.4; extra == "dev"
 Requires-Dist: pylint==3.1.1; extra == "dev"
 Requires-Dist: mypy==1.10.0; extra == "dev"
 Requires-Dist: types-PyYAML==6.0.12.20240311; extra == "dev"
 Requires-Dist: black==24.4.2; extra == "dev"
 Requires-Dist: pytest-cov==5.0.0; extra == "dev"
```

### Comparing `pflows-0.1.0/README.md` & `pflows-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pflows-0.1.0/pyproject.toml` & `pflows-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pflows"
-version = "0.1.0"
+version = "0.1.1"
 description = "Several tools for dealing with image annotations to train YOLO or similar models"
 readme = "README.md"
 authors = [
   {name = "Daniel Pérez Rada", email = "dperezrada@gmail.com"}
 ]
 maintainers = [
   {name = "Daniel Pérez Rada", email = "dperezrada@gmail.com"}
```

### Comparing `pflows-0.1.0/src/modal_server.py` & `pflows-0.1.1/src/modal_server.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 from functools import wraps
 from typing import Any, Dict, Tuple, Sequence, cast
 
 import fastapi
 from fastapi.encoders import jsonable_encoder
 from fastapi.responses import JSONResponse
 from fastapi.exceptions import HTTPException
-import fastapi.security
+
 from modal import App, asgi_app, Function, Image, gpu, Volume, Dict as ModalDict, Secret
 from modal.functions import FunctionCall
 
 
 from pflows.workflow import run_workflow
 
 jobs_volume = Volume.from_name("pflows_jobs", create_if_missing=True)
+uploads_volume = Volume.from_name("pflows_upload", create_if_missing=True)
 
 persisted_jobs_dict: Dict[str, Any] = cast(
     Dict[str, Any], ModalDict.from_name("pflows_jobs_dict", create_if_missing=True)
 )
 
 GPU_TYPE = gpu.A100(size="40GB", count=1)
 
@@ -40,49 +41,62 @@
 app = App("pflows")
 
 web_app = fastapi.FastAPI()
 
 
 @app.function(
     image=image,
-    volumes={"/root/jobs_data": jobs_volume},
+    volumes={"/root/jobs_data": jobs_volume, "/root/uploads_data": uploads_volume},
     secrets=[Secret.from_name("PFLOW_AUTH_TOKEN")],
 )
 @asgi_app()
 def fastapi_app() -> Any:
     return web_app
 
 
 def set_env(env_variables: Dict[str, Any], job_id: str) -> None:
     for key, value in env_variables.items():
         os.environ[key] = value
     if os.environ.get("BASE_FOLDER") is None:
         with tempfile.TemporaryDirectory() as tmp:
             os.environ["BASE_FOLDER"] = tmp
+            os.environ["REMOTE_BASE_FOLDER"] = os.environ["BASE_FOLDER"]
             print(f"Setting BASE_FOLDER to {tmp}")
+    os.environ["JOB_ID"] = job_id
+
     os.environ["PERSISTED_FOLDER"] = f"/root/jobs_data/{job_id}"
+    os.environ["REMOTE_PERSISTED_FOLDER"] = os.environ["PERSISTED_FOLDER"]
     if not os.path.exists(os.environ["PERSISTED_FOLDER"]):
         os.makedirs(os.environ["PERSISTED_FOLDER"], exist_ok=True)
+    os.environ["TEMP_FOLDER"] = tempfile.gettempdir()
+    os.environ["REMOTE_TEMP_FOLDER"] = os.environ["TEMP_FOLDER"]
 
 
-@app.function(image=image, timeout=5_400, volumes={"/root/jobs_data": jobs_volume})
+@app.function(
+    image=image,
+    timeout=5_400,
+    volumes={"/root/jobs_data": jobs_volume, "/root/uploads_data": uploads_volume},
+)
 def endpoint_run_workflow_cpu(
     workflow: Sequence[Dict[str, Any]], env: Dict[str, Any], job_id: str
 ) -> Dict[str, Any]:
     print("Running workflow")
     set_env(env, job_id)
     results = run_workflow(
         raw_workflow=workflow, store_dict=persisted_jobs_dict, store_dict_key=job_id
     )
     persisted_jobs_dict[job_id] = {**results, "status": "completed"}
     return cast(Dict[str, Any], persisted_jobs_dict[job_id])
 
 
 @app.function(
-    image=image_gpu, gpu=GPU_TYPE, timeout=5_400, volumes={"/root/jobs_data": jobs_volume}
+    image=image_gpu,
+    gpu=GPU_TYPE,
+    timeout=5_400,
+    volumes={"/root/jobs_data": jobs_volume, "/root/uploads_data": uploads_volume},
 )
 def endpoint_run_workflow_gpu(
     workflow: Sequence[Dict[str, Any]], env: Dict[str, Any], job_id: str
 ) -> Dict[str, Any]:
     print("Running workflow")
     set_env(env, job_id)
     results = run_workflow(
@@ -114,19 +128,22 @@
 
 
 def auth_required(endpoint_func: Any) -> Any:
     @wraps(endpoint_func)
     async def wrapper(*args: Any, **kwargs: Any) -> Any:
         equal_tokens = False
         try:
-            request: fastapi.Request | None = kwargs.get("request") or kwargs.get("_request") or None
+            request: fastapi.Request | None = (
+                kwargs.get("request") or kwargs.get("_request") or None
+            )
             if request is None:
                 raise ValueError("Request not found")
             token = (request.headers.get("authorization") or "").split(" ")[1]
             equal_tokens = os.environ.get("PFLOW_AUTH_TOKEN") == token
+        # pylint: disable=broad-exception-caught
         except Exception:
             pass
 
         if not equal_tokens:
             raise HTTPException(
                 status_code=fastapi.status.HTTP_401_UNAUTHORIZED,
                 detail="Incorrect bearer token",
@@ -152,15 +169,18 @@
     print("workflow_cpu")
     return start_job(request_json, endpoint_run_workflow_cpu)
 
 
 @web_app.get("/result/{job_id}")
 @auth_required
 async def poll_results(_request: fastapi.Request, job_id: str) -> Any:
-    job_info = persisted_jobs_dict[job_id]
+    try:
+        job_info = persisted_jobs_dict[job_id]
+    except KeyError:
+        return {"error": "Job not found."}
     if job_info.get("status") == "completed":
         return JSONResponse(content=jsonable_encoder(persisted_jobs_dict[job_id]))
     function_call = FunctionCall.from_id(job_info["call_id"])
     try:
         json_result = function_call.get(timeout=0)
         persisted_jobs_dict[job_id] = {
             **json_result,
@@ -202,7 +222,80 @@
 
     # Read the file content
     with open(abs_path, "rb") as file:
         file_content = file.read()
 
     # Return the file content with the guessed content type
     return fastapi.Response(content=file_content, media_type=content_type)
+
+
+@web_app.post("/uploads/download/{upload_id}")
+@auth_required
+async def download_upload_file(request: fastapi.Request, upload_id: str) -> Any:
+    request_path = (await request.json()).get("path")
+    print("request_path", request_path)
+    if request_path is None:
+        return {"error": "The path is required."}
+    request_path = request_path.lstrip("/")
+
+    sanitized_path = os.path.normpath(request_path)
+
+    if ".." in sanitized_path:
+        return {"error": "Invalid path."}
+
+    abs_path = f"/root/uploads_data/{upload_id}/{request_path}"
+
+    if not os.path.exists(abs_path):
+        return {"error": "File not found."}
+
+    content_type, _ = mimetypes.guess_type(abs_path)
+    if content_type is None:
+        content_type = "application/octet-stream"
+
+    # Read the file content
+    with open(abs_path, "rb") as file:
+        file_content = file.read()
+
+    # Return the file content with the guessed content type
+    return fastapi.Response(content=file_content, media_type=content_type)
+
+
+@web_app.post("/uploads")
+@auth_required
+async def upload_file(request: fastapi.Request) -> Any:
+    data = await request.form()
+    file = data["file"]
+    path = data["path"]
+    upload_id = uuid.uuid4().hex
+    abs_path = f"/root/uploads_data/{upload_id}/{path}"
+    os.makedirs(os.path.dirname(abs_path), exist_ok=True)
+    if isinstance(file, str):
+        with open(abs_path, "w", encoding="utf-8") as f:
+            f.write(file)
+    else:
+        with open(abs_path, "wb") as f:
+            f.write(await file.read())
+    return {"status": "uploaded", "path": path, "upload_id": upload_id}
+
+
+@web_app.post("/uploads/delete/{upload_id}")
+@auth_required
+async def delete_upload_file(request: fastapi.Request, upload_id: str) -> Any:
+    request_path = (await request.json()).get("path") or ""
+    if request_path is None:
+        return {"error": "The path is required."}
+
+    request_path = request_path.split("/")[-1]
+
+    sanitized_path = os.path.normpath(request_path)
+
+    if ".." in sanitized_path:
+        return {"error": "Invalid path."}
+
+    abs_path = f"/root/uploads_data/{upload_id}/{request_path}"
+
+    print(abs_path)
+    if not os.path.exists(abs_path):
+        return {"error": "File not found."}
+
+    os.remove(abs_path)
+    return {"status": "deleted"}
```

### Comparing `pflows-0.1.0/src/pflows/cli.py` & `pflows-0.1.1/src/pflows/cli.py`

 * *Files identical despite different names*

### Comparing `pflows-0.1.0/src/pflows/model.py` & `pflows-0.1.1/src/pflows/model.py`

 * *Files identical despite different names*

### Comparing `pflows-0.1.0/src/pflows/polygons.py` & `pflows-0.1.1/src/pflows/polygons.py`

 * *Files identical despite different names*

### Comparing `pflows-0.1.0/src/pflows/tools/augmentations.py` & `pflows-0.1.1/src/pflows/tools/augmentations.py`

 * *Files identical despite different names*

### Comparing `pflows-0.1.0/src/pflows/tools/categories.py` & `pflows-0.1.1/src/pflows/tools/categories.py`

 * *Files identical despite different names*

### Comparing `pflows-0.1.0/src/pflows/tools/dataset.py` & `pflows-0.1.1/src/pflows/tools/dataset.py`

 * *Files 26% similar despite different names*

```diff
@@ -87,7 +87,23 @@
         image.group = "train"
         images.append(image)
     for group_name, images_start, images_end in groups_info:
         for image in images_to_resplit[images_start:images_end]:
             image.group = group_name
             images.append(image)
     return images
+
+
+def show_dataset(dataset: Dataset) -> Dict[str, Any]:
+    to_return = []
+    for image in dataset.images:
+        to_return.append(
+            {
+                **image.__dict__,
+                "annotations": [annotation.__dict__ for annotation in image.annotations],
+            }
+        )
+    return {
+        "images": to_return,
+        "categories": [category.__dict__ for category in dataset.categories],
+        "groups": dataset.groups,
+    }
```

### Comparing `pflows-0.1.0/src/pflows/tools/filter_images.py` & `pflows-0.1.1/src/pflows/tools/filter_images.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,7 +42,15 @@
     for name, group_images in name_groups.items():
         if len(group_images) > 1:
             # We need to exclude all the other paths
             exclude_images += [image.path for index, image in enumerate(group_images) if index != 0]
     print(f"found {len(exclude_images)} duplicate images")
     dataset.images = [image for image in dataset.images if image.path not in exclude_images]
     return dataset
+
+
+def by_group(dataset: Dataset, group: str) -> Dataset:
+    return Dataset(
+        images=[image for image in dataset.images if group == image.group],
+        categories=dataset.categories,
+        groups=dataset.groups,
+    )
```

### Comparing `pflows-0.1.0/src/pflows/tools/roboflow_tools.py` & `pflows-0.1.1/src/pflows/tools/roboflow_tools.py`

 * *Files identical despite different names*

### Comparing `pflows-0.1.0/src/pflows/tools/yolo_v8.py` & `pflows-0.1.1/src/pflows/tools/yolo_v8.py`

 * *Files identical despite different names*

### Comparing `pflows-0.1.0/src/pflows/typedef.py` & `pflows-0.1.1/src/pflows/typedef.py`

 * *Files identical despite different names*

### Comparing `pflows-0.1.0/src/pflows/workflow.py` & `pflows-0.1.1/src/pflows/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,16 @@
             if match == "CURRENT_DIR" and current_dir is not None:
                 value = current_dir
             else:
                 found_base_folder = os.getenv("BASE_FOLDER")
                 if match == "PERSISTED_FOLDER" and found_base_folder is not None:
                     value = found_base_folder
                 else:
-                    raise ValueError(f"The variable '{match}' is not defined.")
+                    print(f"Variable {match} not found in environment variables.")
+                    continue
         text = text.replace(f"{{{{{match}}}}}", value)
     return text
 
 
 def prepare_workflow(
     raw_workflow: Sequence[Dict[str, Any]], workflow_dir: str | None
 ) -> Sequence[Dict[str, Any]]:
```

### Comparing `pflows-0.1.0/src/pflows.egg-info/PKG-INFO` & `pflows-0.1.1/src/pflows.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pflows
-Version: 0.1.0
+Version: 0.1.1
 Summary: Several tools for dealing with image annotations to train YOLO or similar models
 Author-email: Daniel Pérez Rada <dperezrada@gmail.com>
 Maintainer-email: Daniel Pérez Rada <dperezrada@gmail.com>
 License: MIT license
 Project-URL: bugs, https://github.com/dperezrada/pflows/issues
 Project-URL: changelog, https://github.com/dperezrada/pflows/blob/master/changelog.md
 Project-URL: homepage, https://github.com/dperezrada/pflows
@@ -19,14 +19,16 @@
 Requires-Dist: opencv-python-headless==4.8.0.74
 Requires-Dist: shapely==2.0.4
 Requires-Dist: albumentations==1.3.1
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: fastapi==0.111.0
 Requires-Dist: fastapi-cli==0.0.4
 Requires-Dist: modal==0.62.181
+Requires-Dist: requests==2.31.0
+Requires-Dist: requests-toolbelt==1.0.0
 Provides-Extra: dev
 Requires-Dist: pytest==6.2.4; extra == "dev"
 Requires-Dist: pylint==3.1.1; extra == "dev"
 Requires-Dist: mypy==1.10.0; extra == "dev"
 Requires-Dist: types-PyYAML==6.0.12.20240311; extra == "dev"
 Requires-Dist: black==24.4.2; extra == "dev"
 Requires-Dist: pytest-cov==5.0.0; extra == "dev"
```

### Comparing `pflows-0.1.0/src/pflows.egg-info/SOURCES.txt` & `pflows-0.1.1/src/pflows.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -20,10 +20,11 @@
 src/pflows/tools/__init__.py
 src/pflows/tools/annotations.py
 src/pflows/tools/augmentations.py
 src/pflows/tools/base.py
 src/pflows/tools/categories.py
 src/pflows/tools/dataset.py
 src/pflows/tools/filter_images.py
+src/pflows/tools/pflows_remote.py
 src/pflows/tools/roboflow_tools.py
 src/pflows/tools/yolo_v8.py
 tests/test_workflow.py
```

### Comparing `pflows-0.1.0/tests/test_workflow.py` & `pflows-0.1.1/tests/test_workflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,16 +32,7 @@
 def test_read_w_variable_raw_workflow():
     with tempfile.TemporaryDirectory() as tmp:
         os.environ['BASE_FOLDER'] = tmp
         workflow, workflow_data = read_workflow(raw_workflow=workflow_w_variable)
         assert len(workflow) == 1
         first_task = workflow[0]
         assert first_task.params['folder_path'] == f"{tmp}/datasets/downloaded/group3"
-
-def test_read_w_missing_variable():
-    os.environ['BASE_FOLDER'] = ''
-    # we expect an error here
-    try:
-        workflow, workflow_data = read_workflow(raw_workflow=workflow_w_variable)
-        assert False
-    except ValueError as e:
-        assert True
```

