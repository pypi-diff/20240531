# Comparing `tmp/pytroll_db-0.2.0.tar.gz` & `tmp/pytroll_db-0.3.0.tar.gz`

## Comparing `pytroll_db-0.2.0.tar` & `pytroll_db-0.3.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/.readthedocs.yaml
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/.github/workflows/deploy-sdist.yaml
--rwxr-xr-x   0        0        0      303 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/docs/Makefile
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/docs/requirements.txt
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/docs/source/conf.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/docs/source/index.rst
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/__init__.py
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/cli.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/template_config.yaml
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/version.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/api/__init__.py
--rw-r--r--   0        0        0     6619 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/api/api.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/api/routes/__init__.py
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/api/routes/common.py
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/api/routes/databases.py
--rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/api/routes/datetime_.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/api/routes/platforms.py
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/api/routes/queries.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/api/routes/root.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/api/routes/router.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/api/routes/sensors.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/config/__init__.py
--rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/config/config.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/database/__init__.py
--rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/database/errors.py
--rw-r--r--   0        0        0    12907 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/database/mongodb.py
--rw-r--r--   0        0        0     6305 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/database/piplines.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/errors/__init__.py
--rw-r--r--   0        0        0    11216 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/errors/errors.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/test_utils/__init__.py
--rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/test_utils/common.py
--rw-r--r--   0        0        0     7736 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/test_utils/mongodb_database.py
--rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/test_utils/mongodb_instance.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/tests/conftest.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/tests/pytest.ini
--rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/tests/test_recorder.py
--rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/tests/tests_api/test_api.py
--rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/tests/tests_database/test_mongodb.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/trolldb/tests/tests_database/test_pipelines.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/.gitignore
--rw-r--r--   0        0        0    35121 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/LICENSE
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/README.rst
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    42462 2020-02-02 00:00:00.000000 pytroll_db-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/.github/workflows/deploy-sdist.yaml
+-rwxr-xr-x   0        0        0      303 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/docs/Makefile
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/docs/requirements.txt
+-rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/docs/source/conf.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/docs/source/index.rst
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/__init__.py
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/cli.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/template_config.yaml
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/version.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/api/__init__.py
+-rw-r--r--   0        0        0     6731 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/api/api.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/api/routes/__init__.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/api/routes/common.py
+-rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/api/routes/databases.py
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/api/routes/datetime_.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/api/routes/platforms.py
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/api/routes/queries.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/api/routes/root.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/api/routes/router.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/api/routes/sensors.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/config/__init__.py
+-rw-r--r--   0        0        0     4625 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/config/config.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/database/__init__.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/database/errors.py
+-rw-r--r--   0        0        0    13117 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/database/mongodb.py
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/database/pipelines.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/errors/__init__.py
+-rw-r--r--   0        0        0    11467 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/errors/errors.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/test_utils/__init__.py
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/test_utils/common.py
+-rw-r--r--   0        0        0    12910 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/test_utils/mongodb_database.py
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/test_utils/mongodb_instance.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/tests/conftest.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/tests/pytest.ini
+-rw-r--r--   0        0        0     5936 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/tests/test_recorder.py
+-rw-r--r--   0        0        0     7388 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/tests/tests_api/test_api.py
+-rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/tests/tests_database/test_mongodb.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/trolldb/tests/tests_database/test_pipelines.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/.gitignore
+-rw-r--r--   0        0        0    35121 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/README.rst
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    42462 2020-02-02 00:00:00.000000 pytroll_db-0.3.0/PKG-INFO
```

### Comparing `pytroll_db-0.2.0/.readthedocs.yaml` & `pytroll_db-0.3.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pytroll_db-0.2.0/.github/workflows/ci.yml` & `pytroll_db-0.3.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pytroll_db-0.2.0/.github/workflows/deploy-sdist.yaml` & `pytroll_db-0.3.0/.github/workflows/deploy-sdist.yaml`

 * *Files identical despite different names*

### Comparing `pytroll_db-0.2.0/trolldb/template_config.yaml` & `pytroll_db-0.3.0/trolldb/template_config.yaml`

 * *Files identical despite different names*

### Comparing `pytroll_db-0.2.0/trolldb/api/api.py` & `pytroll_db-0.3.0/trolldb/api/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,100 +10,101 @@
     Assuming that the API server is running on `<http://localhost:8000>`_ (example) the auto-generated documentation can
     be accessed via either `<http://localhost:8000/redoc>`_ or  `<http://localhost:8000/docs>`_.
 
     Read more at `FastAPI automatics docs <https://fastapi.tiangolo.com/features/#automatic-docs>`_.
 """
 
 import asyncio
+import sys
 import time
 from contextlib import contextmanager
 from multiprocessing import Process
-from typing import Union
+from typing import Any, Generator, NoReturn
 
 import uvicorn
 from fastapi import FastAPI, status
 from fastapi.responses import PlainTextResponse
 from loguru import logger
-from pydantic import FilePath, validate_call
+from pydantic import ValidationError
 
 from trolldb.api.routes import api_router
-from trolldb.config.config import AppConfig, Timeout, parse_config_yaml_file
+from trolldb.config.config import AppConfig, Timeout
 from trolldb.database.mongodb import mongodb_context
 from trolldb.errors.errors import ResponseError
 
 API_INFO = dict(
     title="pytroll-db",
     summary="The database API of Pytroll",
     description=
-    "The API allows   you to perform CRUD operations as well as querying the database"
+    "The API allows you to perform CRUD operations as well as querying the database"
     "At the moment only MongoDB is supported. It is based on the following Python packages"
     "\n * **PyMongo** (https://github.com/mongodb/mongo-python-driver)"
     "\n * **motor** (https://github.com/mongodb/motor)",
     license_info=dict(
         name="The GNU General Public License v3.0",
         url="https://www.gnu.org/licenses/gpl-3.0.en.html"
     )
 )
-"""These will appear int the auto-generated documentation and are passed to the ``FastAPI`` class as keyword args."""
+"""These will appear in the auto-generated documentation and are passed to the ``FastAPI`` class as keyword args."""
 
 
-@validate_call
-def run_server(config: Union[AppConfig, FilePath], **kwargs) -> None:
+@logger.catch(onerror=lambda _: sys.exit(1))
+def run_server(config: AppConfig, **kwargs) -> None:
     """Runs the API server with all the routes and connection to the database.
 
     It first creates a FastAPI application and runs it using `uvicorn <https://www.uvicorn.org/>`_ which is
     ASGI (Asynchronous Server Gateway Interface) compliant. This function runs the event loop using
     `asyncio <https://docs.python.org/3/library/asyncio.html>`_ and does not yield!
 
     Args:
         config:
-            The configuration of the application which includes both the server and database configurations. Its type
-            should be a :class:`FilePath`, which is a valid path to an existing config file which will parsed as a
-            ``.YAML`` file.
+            The configuration of the application which includes both the server and database configurations.
 
         **kwargs:
             The keyword arguments are the same as those accepted by the
             `FastAPI class <https://fastapi.tiangolo.com/reference/fastapi/#fastapi.FastAPI>`_ and are directly passed
             to it. These keyword arguments will be first concatenated with the configurations of the API server which
             are read from the ``config`` argument. The keyword arguments which are passed explicitly to the function
-            take precedence over ``config``. Finally, ``API_INFO``, which are hard-coded information for the API server,
-            will be concatenated and takes precedence over all.
-
-    Raises:
-        ValidationError:
-            If the function is not called with arguments of valid type.
+            take precedence over ``config``. Finally, :obj:`API_INFO`, which are hard-coded information for the API
+            server, will be concatenated and takes precedence over all.
 
     Example:
         .. code-block:: python
 
-            from api.api import run_server
+            from trolldb.api.api import run_server
+            from trolldb.config.config import parse_config
+
             if __name__ == "__main__":
-                run_server("config.yaml")
+                run_server(parse_config("config.yaml"))
     """
     logger.info("Attempt to run the API server ...")
-    if not isinstance(config, AppConfig):
-        config = parse_config_yaml_file(config)
 
     # Concatenate the keyword arguments for the API server in the order of precedence (lower to higher).
     app = FastAPI(**(config.api_server._asdict() | kwargs | API_INFO))
 
     app.include_router(api_router)
 
     @app.exception_handler(ResponseError)
-    async def auto_exception_handler(_, exc: ResponseError):
+    async def auto_handler_response_errors(_, exc: ResponseError) -> PlainTextResponse:
         """Catches all the exceptions raised as a ResponseError, e.g. accessing non-existing databases/collections."""
         status_code, message = exc.get_error_details()
         info = dict(
             status_code=status_code if status_code else status.HTTP_500_INTERNAL_SERVER_ERROR,
             content=message if message else "Generic Error [This is not okay, check why we have the generic error!]",
         )
         logger.error(f"Response error caught by the API auto exception handler: {info}")
         return PlainTextResponse(**info)
 
-    async def _serve():
+    @app.exception_handler(ValidationError)
+    async def auto_handler_pydantic_validation_errors(_, exc: ValidationError) -> PlainTextResponse:
+        """Catches all the exceptions raised as a Pydantic ValidationError."""
+        logger.error(f"Response error caught by the API auto exception handler: {exc}")
+        return PlainTextResponse(str(exc), status_code=status.HTTP_500_INTERNAL_SERVER_ERROR)
+
+    async def _serve() -> NoReturn:
         """An auxiliary coroutine to be used in the asynchronous execution of the FastAPI application."""
         async with mongodb_context(config.database):
             logger.info("Attempt to start the uvicorn server ...")
             await uvicorn.Server(
                 config=uvicorn.Config(
                     host=config.api_server.url.host,
                     port=config.api_server.url.port,
@@ -112,15 +113,15 @@
             ).serve()
 
     logger.info("Attempt to run the asyncio loop for the API server ...")
     asyncio.run(_serve())
 
 
 @contextmanager
-def api_server_process_context(config: Union[AppConfig, FilePath], startup_time: Timeout = 2):
+def api_server_process_context(config: AppConfig, startup_time: Timeout = 2) -> Generator[Process, Any, None]:
     """A synchronous context manager to run the API server in a separate process (non-blocking).
 
     It uses the `multiprocessing <https://docs.python.org/3/library/multiprocessing.html>`_ package. The main use case
     is envisaged to be in `TESTING` environments.
 
     Args:
         config:
@@ -128,17 +129,14 @@
 
         startup_time:
             The overall time in seconds that is expected for the server and the database connections to be established
             before actual requests can be sent to the server. For testing purposes ensure that this is sufficiently
             large so that the tests will not time out.
     """
     logger.info("Attempt to run the API server process in a context manager ...")
-    if not isinstance(config, AppConfig):
-        config = parse_config_yaml_file(config)
-
     process = Process(target=run_server, args=(config,))
     try:
         process.start()
         time.sleep(startup_time)
         yield process
     finally:
         logger.info("Attempt to terminate the API server process in the context manager ...")
```

### Comparing `pytroll_db-0.2.0/trolldb/api/routes/common.py` & `pytroll_db-0.3.0/trolldb/api/routes/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,16 @@
 """The module with common functions to be used in handling requests related to `databases` and `collections`."""
 
 from typing import Annotated, Union
 
-from fastapi import Depends, Query, Response
+from fastapi import Depends, Response
 from motor.motor_asyncio import AsyncIOMotorCollection, AsyncIOMotorDatabase
 
 from trolldb.database.mongodb import MongoDB
 
-exclude_defaults_query = Query(
-    True,
-    title="Query string",
-    description=
-    "A boolean to exclude default databases from a MongoDB instance. Refer to "
-    "`trolldb.database.mongodb.MongoDB.default_database_names` for more information."
-)
-
 
 async def check_database(database_name: str | None = None) -> AsyncIOMotorDatabase:
     """A dependency for route handlers to check for the existence of a database given its name.
 
     Args:
         database_name (Optional, default ``None``):
             The name of the database to check. In case of ``None``, the main database will be picked.
```

### Comparing `pytroll_db-0.2.0/trolldb/api/routes/databases.py` & `pytroll_db-0.3.0/trolldb/api/routes/databases.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """The module which handles all requests related to getting the list of `databases` and `collections`.
 
 Note:
     For more information on the API server, see the automatically generated documentation by FastAPI.
 """
 
-from fastapi import APIRouter
+from typing import Annotated
+
+from fastapi import APIRouter, Query
 from pymongo.collection import _DocumentType
 
-from trolldb.api.routes.common import CheckCollectionDependency, CheckDataBaseDependency, exclude_defaults_query
+from trolldb.api.routes.common import CheckCollectionDependency, CheckDataBaseDependency
 from trolldb.config.config import MongoObjectId
 from trolldb.database.errors import (
     Databases,
     Documents,
     database_collection_document_error_descriptor,
     database_collection_error_descriptor,
 )
@@ -19,15 +21,20 @@
 
 router = APIRouter()
 
 
 @router.get("/",
             response_model=list[str],
             summary="Gets the list of all database names")
-async def database_names(exclude_defaults: bool = exclude_defaults_query) -> list[str]:
+async def database_names(
+        exclude_defaults: Annotated[bool, Query(
+            title="Query parameter",
+            description="A boolean to exclude default databases from a MongoDB instance. Refer to "
+                        "`trolldb.database.mongodb.MongoDB.default_database_names` for more information."
+        )] = True) -> list[str]:
     """Please consult the auto-generated documentation by FastAPI."""
     db_names = await MongoDB.list_database_names()
 
     if not exclude_defaults:
         return db_names
 
     return [db for db in db_names if db not in MongoDB.default_database_names]
```

### Comparing `pytroll_db-0.2.0/trolldb/api/routes/datetime_.py` & `pytroll_db-0.3.0/trolldb/api/routes/datetime_.py`

 * *Files identical despite different names*

### Comparing `pytroll_db-0.2.0/trolldb/api/routes/platforms.py` & `pytroll_db-0.3.0/trolldb/api/routes/platforms.py`

 * *Files identical despite different names*

### Comparing `pytroll_db-0.2.0/trolldb/api/routes/queries.py` & `pytroll_db-0.3.0/trolldb/api/routes/queries.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,46 @@
 """The module which handles all requests to the queries route.
 
 Note:
     For more information on the API server, see the automatically generated documentation by FastAPI.
 """
 
 import datetime
+from typing import Annotated
 
 from fastapi import APIRouter, Query
 
 from trolldb.api.routes.common import CheckCollectionDependency
 from trolldb.database.errors import database_collection_error_descriptor
 from trolldb.database.mongodb import get_ids
-from trolldb.database.piplines import PipelineAttribute, Pipelines
+from trolldb.database.pipelines import PipelineAttribute, Pipelines
 
 router = APIRouter()
 
 
 @router.get("",
             response_model=list[str],
             responses=database_collection_error_descriptor,
             summary="Gets the database UUIDs of the documents that match specifications determined by the query string")
 async def queries(
         collection: CheckCollectionDependency,
-        # We suppress ruff for the following four lines with `Query(default=None)`.
-        # Reason: This is the FastAPI way of defining optional queries and ruff is not happy about it!
-        platform: list[str] = Query(default=None),  # noqa: B008
-        sensor: list[str] = Query(default=None),  # noqa: B008
-        time_min: datetime.datetime = Query(default=None),  # noqa: B008
-        time_max: datetime.datetime = Query(default=None)) -> list[str]:  # noqa: B008
+        platform: Annotated[list[str] | None, Query()] = None,
+        sensor: Annotated[list[str] | None, Query()] = None,
+        time_min: Annotated[datetime.datetime, Query()] = None,
+        time_max: Annotated[datetime.datetime, Query()] = None) -> list[str]:
     """Please consult the auto-generated documentation by FastAPI."""
-    # We
     pipelines = Pipelines()
 
     if platform:
         pipelines += PipelineAttribute("platform_name") == platform
 
     if sensor:
         pipelines += PipelineAttribute("sensor") == sensor
 
     if [time_min, time_max] != [None, None]:
         start_time = PipelineAttribute("start_time")
         end_time = PipelineAttribute("end_time")
         pipelines += (
-                (start_time >= time_min) |
-                (start_time <= time_max) |
-                (end_time >= time_min) |
-                (end_time <= time_max)
+                ((start_time >= time_min) & (start_time <= time_max)) |
+                ((end_time >= time_min) & (end_time <= time_max))
         )
-
     return await get_ids(collection.aggregate(pipelines))
```

### Comparing `pytroll_db-0.2.0/trolldb/api/routes/root.py` & `pytroll_db-0.3.0/trolldb/api/routes/root.py`

 * *Files identical despite different names*

### Comparing `pytroll_db-0.2.0/trolldb/api/routes/router.py` & `pytroll_db-0.3.0/trolldb/api/routes/router.py`

 * *Files identical despite different names*

### Comparing `pytroll_db-0.2.0/trolldb/api/routes/sensors.py` & `pytroll_db-0.3.0/trolldb/api/routes/sensors.py`

 * *Files identical despite different names*

### Comparing `pytroll_db-0.2.0/trolldb/config/config.py` & `pytroll_db-0.3.0/trolldb/config/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,74 @@
 """The module which handles parsing and validating the config (YAML) file.
 
 The validation is performed using `Pydantic <https://docs.pydantic.dev/latest/>`_.
 
 Note:
-    Functions in this module are decorated with
-    `pydantic.validate_call <https://docs.pydantic.dev/latest/api/validate_call/#pydantic.validate_call_decorator.validate_call>`_
-    so that their arguments can be validated using the corresponding type hints, when calling the function at runtime.
+    Some functions/methods in this module are decorated with the Pydantic
+    `@validate_call <https://docs.pydantic.dev/latest/api/validate_call/>`_ which checks the arguments during the
+    function calls.
 """
 
 import errno
 import sys
 from typing import Any, NamedTuple
 
 from bson import ObjectId
 from bson.errors import InvalidId
 from loguru import logger
-from pydantic import AnyUrl, BaseModel, Field, FilePath, MongoDsn, ValidationError
+from pydantic import AnyUrl, BaseModel, MongoDsn, PositiveFloat, ValidationError, validate_call
 from pydantic.functional_validators import AfterValidator
 from typing_extensions import Annotated
 from yaml import safe_load
 
-Timeout = Annotated[float, Field(ge=0)]
+Timeout = PositiveFloat
 """A type hint for the timeout in seconds (non-negative float)."""
 
 
+@validate_call
 def id_must_be_valid(id_like_string: str) -> ObjectId:
     """Checks that the given string can be converted to a valid MongoDB ObjectId.
 
     Args:
         id_like_string:
             The string to be converted to an ObjectId.
 
     Returns:
-       The ObjectId object if successfully.
+       The ObjectId object if successful.
 
     Raises:
+        ValidationError:
+            If the given argument is not of type ``str``.
+
         ValueError:
             If the given string cannot be converted to a valid ObjectId. This will ultimately turn into a pydantic
             validation error.
     """
     try:
         return ObjectId(id_like_string)
     except InvalidId as e:
         raise ValueError from e
 
 
 MongoObjectId = Annotated[str, AfterValidator(id_must_be_valid)]
-"""Type hint validator for object IDs."""
+"""The type hint validator for object IDs."""
 
 
 class MongoDocument(BaseModel):
     """Pydantic model for a MongoDB document."""
     _id: MongoObjectId
 
 
 class APIServerConfig(NamedTuple):
     """A named tuple to hold all the configurations of the API server (excluding the database).
 
     Note:
         The attributes herein are a subset of the keyword arguments accepted by
         `FastAPI class <https://fastapi.tiangolo.com/reference/fastapi/#fastapi.FastAPI>`_ and are directly passed
-        to the FastAPI class.
+        to the FastAPI class. Consult :func:`trolldb.api.api.run_server` on how these configurations are treated.
     """
 
     url: AnyUrl
     """The URL of the API server including the port, e.g. ``mongodb://localhost:8000``."""
 
 
 class DatabaseConfig(NamedTuple):
@@ -75,15 +79,15 @@
 
     main_collection_name: str
     """The name of the main collection which resides inside the ``main_database`` and includes the actual data for the
     files, e.g. ``"files"``
     """
 
     url: MongoDsn
-    """The URL of the MongoDB server excluding the port part, e.g. ``"mongodb://localhost:27017"``"""
+    """The URL of the MongoDB server including the port part, e.g. ``"mongodb://localhost:27017"``"""
 
     timeout: Timeout
     """The timeout in seconds (non-negative float), after which an exception is raised if a connection with the
     MongoDB instance is not established successfully, e.g. ``1.5``.
     """
 
 
@@ -91,49 +95,43 @@
 """A dictionary to hold all the configurations of the subscriber.
 
 TODO: This has to be moved to the `posttroll` package.
 """
 
 
 class AppConfig(BaseModel):
-    """A model to hold all the configurations of the application including both the API server and the database.
+    """A model to hold all the configurations of the application, i.e. the API server, the database, and the subscriber.
 
     This will be used by Pydantic to validate the parsed YAML file.
     """
     api_server: APIServerConfig
     database: DatabaseConfig
     subscriber: SubscriberConfig
 
 
-def parse_config_yaml_file(filename: FilePath) -> AppConfig:
-    """Parses and validates the configurations from a YAML file.
+@logger.catch(onerror=lambda _: sys.exit(1))
+def parse_config(file) -> AppConfig:
+    """Parses and validates the configurations from a YAML file (descriptor).
 
     Args:
-        filename:
-            The filename of a valid YAML file which holds the configurations.
+        file:
+            A `path-like object <https://docs.python.org/3/glossary.html#term-path-like-object>`_ or an integer file
+            descriptor. This will be directly passed to the ``open()`` function. For example, it can be the filename
+            (absolute or relative) of a valid YAML file which holds the configurations.
 
     Returns:
         An instance of :class:`AppConfig`.
-
-    Raises:
-        ParserError:
-            If the file cannot be properly parsed
-
-        ValidationError:
-            If the successfully parsed file fails the validation, i.e. its schema or the content does not conform to
-            :class:`AppConfig`.
-
-        ValidationError:
-            If the function is not called with arguments of valid type.
     """
     logger.info("Attempt to parse the YAML file ...")
-    with open(filename, "r") as file:
-        config = safe_load(file)
+    with open(file, "r") as f:
+        config = safe_load(f)
     logger.info("Parsing YAML file is successful.")
+
     try:
         logger.info("Attempt to validate the parsed YAML file ...")
         config = AppConfig(**config)
-        logger.info("Validation of the parsed YAML file is successful.")
-        return config
     except ValidationError as e:
         logger.error(e)
         sys.exit(errno.EIO)
+
+    logger.info("Validation of the parsed YAML file is successful.")
+    return config
```

### Comparing `pytroll_db-0.2.0/trolldb/database/errors.py` & `pytroll_db-0.3.0/trolldb/database/errors.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,78 +2,80 @@
 
 Note:
     The error responses are grouped into classes, with each class representing the major
     category (context) in which the errors occur. As such, the attributes of the top classes
     are (expected to be) self-explanatory and require no additional documentation.
 """
 
+from typing import ClassVar
+
 from fastapi import status
 
 from trolldb.errors.errors import ResponseError, ResponsesErrorGroup
 
 
 class Client(ResponsesErrorGroup):
-    """Client error responses, e.g. if something goes wrong with initialization or closing the client."""
-    CloseNotAllowedError = ResponseError({
+    """Database client error responses, e.g. if something goes wrong with initialization or closing the client."""
+    CloseNotAllowedError: ClassVar[ResponseError] = ResponseError({
         status.HTTP_405_METHOD_NOT_ALLOWED:
             "Calling `close()` on a client which has not been initialized is not allowed!"
     })
 
-    ReinitializeConfigError = ResponseError({
+    ReinitializeConfigError: ClassVar[ResponseError] = ResponseError({
         status.HTTP_405_METHOD_NOT_ALLOWED:
             "The client is already initialized with a different database configuration!"
     })
 
-    AlreadyOpenError = ResponseError({
+    AlreadyOpenError: ClassVar[ResponseError] = ResponseError({
         status.HTTP_100_CONTINUE:
             "The client has been already initialized with the same configuration."
     })
 
-    InconsistencyError = ResponseError({
+    InconsistencyError: ClassVar[ResponseError] = ResponseError({
         status.HTTP_405_METHOD_NOT_ALLOWED:
             "Something must have been wrong as we are in an inconsistent state. "
             "The internal database configuration is not empty and is the same as what we just "
             "received but the client is `None` or has been already closed!"
     })
 
-    ConnectionError = ResponseError({
+    ConnectionError: ClassVar[ResponseError] = ResponseError({
         status.HTTP_400_BAD_REQUEST:
-            "Could not connect to the database with URL."
+            "Could not connect to the database with the given URL."
     })
 
 
 class Collections(ResponsesErrorGroup):
-    """Collections error responses, e.g. if a requested collection cannot be found."""
-    NotFoundError = ResponseError({
+    """Collections error responses, e.g. if the requested collection cannot be found."""
+    NotFoundError: ClassVar[ResponseError] = ResponseError({
         status.HTTP_404_NOT_FOUND:
             "Could not find the given collection name inside the specified database."
     })
 
-    WrongTypeError = ResponseError({
+    WrongTypeError: ClassVar[ResponseError] = ResponseError({
         status.HTTP_422_UNPROCESSABLE_ENTITY:
-            "Both the Database and collection name must be `None` if one of them is `None`."
+            "Both the database and collection name must be `None` if either one is `None`."
     })
 
 
 class Databases(ResponsesErrorGroup):
-    """Databases error responses, e.g. if a requested database cannot be found."""
-    NotFoundError = ResponseError({
+    """Databases error responses, e.g. if the requested database cannot be found."""
+    NotFoundError: ClassVar[ResponseError] = ResponseError({
         status.HTTP_404_NOT_FOUND:
             "Could not find the given database name."
     })
 
-    WrongTypeError = ResponseError({
+    WrongTypeError: ClassVar[ResponseError] = ResponseError({
         status.HTTP_422_UNPROCESSABLE_ENTITY:
             "Database name must be either of type `str` or `None.`"
     })
 
 
 class Documents(ResponsesErrorGroup):
-    """Documents error responses, e.g. if a requested document cannot be found."""
-    NotFound = ResponseError({
+    """Documents error responses, e.g. if the requested document cannot be found."""
+    NotFound: ClassVar[ResponseError] = ResponseError({
         status.HTTP_404_NOT_FOUND:
             "Could not find any document with the given object id."
     })
 
 
 database_collection_error_descriptor = (
         Databases.union() | Collections.union()
```

### Comparing `pytroll_db-0.2.0/trolldb/database/mongodb.py` & `pytroll_db-0.3.0/trolldb/database/mongodb.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,61 +1,55 @@
 """The module which handles database CRUD operations for MongoDB.
 
 It is based on the following libraries:
   - `PyMongo <https://github.com/mongodb/mongo-python-driver>`_
   - `motor <https://github.com/mongodb/motor>`_.
+
+Note:
+    Some functions/methods in this module are decorated with the Pydantic
+    `@validate_call <https://docs.pydantic.dev/latest/api/validate_call/>`_ which checks the arguments during the
+    function calls.
 """
 
 import errno
 from contextlib import asynccontextmanager
-from typing import Any, AsyncGenerator, Coroutine, Optional, TypeVar, Union
+from typing import Any, AsyncGenerator, ClassVar, Coroutine, Optional, TypeVar, Union
 
 from loguru import logger
 from motor.motor_asyncio import (
     AsyncIOMotorClient,
     AsyncIOMotorCollection,
     AsyncIOMotorCommandCursor,
     AsyncIOMotorCursor,
     AsyncIOMotorDatabase,
 )
-from pydantic import BaseModel
+from pydantic import validate_call
 from pymongo.collection import _DocumentType
 from pymongo.errors import ConnectionFailure, ServerSelectionTimeoutError
 
 from trolldb.config.config import DatabaseConfig
 from trolldb.database.errors import Client, Collections, Databases
-from trolldb.errors.errors import ResponseError
 
 T = TypeVar("T")
 CoroutineLike = Coroutine[Any, Any, T]
 """A simple type hint for a coroutine of any type."""
 
 CoroutineDocument = CoroutineLike[_DocumentType | None]
 """Coroutine type hint for document like objects."""
 
 CoroutineStrList = CoroutineLike[list[str]]
 """Coroutine type hint for a list of strings."""
 
 
-class DatabaseName(BaseModel):
-    """Pydantic model for a database name."""
-    name: str | None
-
-
-class CollectionName(BaseModel):
-    """Pydantic model for a collection name."""
-    name: str | None
-
-
 async def get_id(doc: CoroutineDocument) -> str:
     """Retrieves the ID of a document as a simple flat string.
 
     Note:
         The rationale behind this method is as follows. In MongoDB, each document has a unique ID which is of type
-        :class:`~bson.objectid.ObjectId`. This is not suitable for purposes when a simple string is needed, hence
+        :class:`bson.objectid.ObjectId`. This is not suitable for purposes when a simple string is needed, hence
         the need for this method.
 
     Args:
         doc:
             A MongoDB document in the coroutine form. This could be e.g. the result of applying the standard
             ``find_one`` method from MongoDB on a collection given a ``filter``.
 
@@ -80,15 +74,15 @@
     """
     return [str(doc["_id"]) async for doc in docs]
 
 
 class MongoDB:
     """A wrapper class around the `motor async driver <https://www.mongodb.com/docs/drivers/motor/>`_ for Mongo DB.
 
-    It includes convenience methods tailored to our specific needs. As such, the :func:`~MongoDB.initialize()`` method
+    It includes convenience methods tailored to our specific needs. As such, the :func:`~MongoDB.initialize()` method
     returns a coroutine which needs to be awaited.
 
     Note:
         This class is not meant to be instantiated! That's why all the methods in this class are decorated with
         ``@classmethods``. This choice has been made to guarantee optimal performance, i.e. for each running process
         there must be only a single motor client to handle all database operations. Having different clients which are
         constantly opened/closed degrades the performance. The expected usage is that we open a client in the beginning
@@ -99,47 +93,51 @@
         The main difference between this wrapper class and the original motor driver class is that we attempt to access
         the database and collections during the initialization to see if we succeed or fail. This is contrary to the
         behaviour of the motor driver which simply creates a client object and does not attempt to access the database
         until some time later when an actual operation is performed on the database. This behaviour is not desired for
         us, we would like to fail early!
     """
 
-    __client: Optional[AsyncIOMotorClient] = None
-    __database_config: Optional[DatabaseConfig] = None
-    __main_collection: AsyncIOMotorCollection = None
-    __main_database: AsyncIOMotorDatabase = None
+    __client: ClassVar[Optional[AsyncIOMotorClient]] = None
+    __database_config: ClassVar[Optional[DatabaseConfig]] = None
+    __main_collection: ClassVar[Optional[AsyncIOMotorCollection]] = None
+    __main_database: ClassVar[Optional[AsyncIOMotorDatabase]] = None
 
-    default_database_names = ["admin", "config", "local"]
+    default_database_names: ClassVar[list[str]] = ["admin", "config", "local"]
     """MongoDB creates these databases by default for self usage."""
 
     @classmethod
     async def initialize(cls, database_config: DatabaseConfig):
         """Initializes the motor client. Note that this method has to be awaited!
 
         Args:
             database_config:
-                 A named tuple which includes the database configurations.
+                 An object of type :class:`~trolldb.config.config.DatabaseConfig` which includes the database
+                 configurations.
+
+        Warning:
+            The timeout is given in seconds in the configurations, while the MongoDB uses milliseconds.
 
         Returns:
             On success ``None``.
 
         Raises:
             SystemExit(errno.EIO):
-                If connection is not established (``ConnectionFailure``)
+                If connection is not established, i.e. ``ConnectionFailure``.
             SystemExit(errno.EIO):
-                If the attempt times out (``ServerSelectionTimeoutError``)
+                If the attempt times out, i.e. ``ServerSelectionTimeoutError``.
             SystemExit(errno.EIO):
                 If one attempts reinitializing the class with new (different) database configurations without calling
                 :func:`~close()` first.
             SystemExit(errno.EIO):
                 If the state is not consistent, i.e. the client is closed or ``None`` but the internal database
                 configurations still exist and are different from the new ones which have been just provided.
-
             SystemExit(errno.ENODATA):
-                If either ``database_config.main_database`` or ``database_config.main_collection`` does not exist.
+                If either ``database_config.main_database_name`` or ``database_config.main_collection_name`` does not
+                exist.
         """
         logger.info("Attempt to initialize the MongoDB client ...")
         logger.info("Checking the database configs ...")
         if cls.__database_config:
             if database_config == cls.__database_config:
                 if cls.__client:
                     return Client.AlreadyOpenError.log_as_warning()
@@ -216,76 +214,76 @@
             The main database which includes the main collection, which in turn includes the desired documents.
 
             This is equivalent to ``MongoDB.client()[<main_database_name>]``.
         """
         return cls.__main_database
 
     @classmethod
+    @validate_call
     async def get_collection(
             cls,
-            database_name: str,
-            collection_name: str) -> Union[AsyncIOMotorCollection, ResponseError]:
+            database_name: str | None,
+            collection_name: str | None) -> AsyncIOMotorCollection:
         """Gets the collection object given its name and the database name in which it resides.
 
         Args:
             database_name:
                 The name of the parent database which includes the collection.
             collection_name:
                 The name of the collection which resides inside the parent database labelled by ``database_name``.
 
         Returns:
             The database object. In case of ``None`` for both the database name and collection name, the main collection
             will be returned.
 
         Raises:
             ValidationError:
-                If input args are invalid according to the pydantic.
+                If the method is not called with arguments of valid type.
 
             KeyError:
                 If the database name exists, but it does not include any collection with the given name.
 
             TypeError:
                 If only one of the database or collection names are ``None``.
 
             ...:
                 This method relies on :func:`get_database` to check for the existence of the database which can raise
                 exceptions. Check its documentation for more information.
         """
-        database_name = DatabaseName(name=database_name).name
-        collection_name = CollectionName(name=collection_name).name
-
         match database_name, collection_name:
             case None, None:
                 return cls.main_collection()
 
             case str(), str():
                 db = await cls.get_database(database_name)
                 if collection_name in await db.list_collection_names():
                     return db[collection_name]
                 raise Collections.NotFoundError
             case _:
                 raise Collections.WrongTypeError
 
     @classmethod
-    async def get_database(cls, database_name: str) -> Union[AsyncIOMotorDatabase, ResponseError]:
+    @validate_call
+    async def get_database(cls, database_name: str | None) -> AsyncIOMotorDatabase:
         """Gets the database object given its name.
 
         Args:
             database_name:
                 The name of the database to retrieve.
 
         Returns:
             The database object.
 
         Raises:
-             KeyError:
+            ValidationError:
+                If the method is not called with arguments of valid type.
+
+            KeyError:
                 If the database name does not exist in the list of database names.
         """
-        database_name = DatabaseName(name=database_name).name
-
         match database_name:
             case None:
                 return cls.main_database()
             case _ if database_name in await cls.list_database_names():
                 return cls.__client[database_name]
             case _:
                 raise Databases.NotFoundError
```

### Comparing `pytroll_db-0.2.0/trolldb/database/piplines.py` & `pytroll_db-0.3.0/trolldb/database/pipelines.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,19 +26,19 @@
 
             pd_or = pd1 | pd2
             pd_or_literal = PipelineBooleanDict({"$or": [{"number": 2}, {"kind": 1}]})
             # The following evaluates to True
             pd_or == pd_or_literal
     """
 
-    def __or__(self, other: Self):
+    def __or__(self, other: Self) -> Self:
         """Implements the bitwise or operator, i.e. ``|``."""
         return PipelineBooleanDict({"$or": [self, other]})
 
-    def __and__(self, other: Self):
+    def __and__(self, other: Self) -> Self:
         """Implements the bitwise and operator, i.e. ``&``."""
         return PipelineBooleanDict({"$and": [self, other]})
 
 
 class PipelineAttribute:
     """A class which defines a single pipeline attribute on which boolean operations will be performed.
 
@@ -108,15 +108,15 @@
 
 class Pipelines(list):
     """A class which defines a list of pipelines.
 
     Each item in the list is a dictionary with its key being the literal string ``"$match"`` and its corresponding value
     being of type :class:`PipelineBooleanDict`. The ``"$match"`` key is what actually triggers the matching operation in
     the MongoDB aggregation pipeline. The condition against which the matching will be performed is given by the value
-    which is a simply a boolean pipeline dictionary which has a hierarchical structure.
+    which is a simply a boolean pipeline dictionary and has a hierarchical structure.
 
     Example:
         .. code-block:: python
 
             pipelines = Pipelines()
             pipelines += PipelineAttribute("platform_name") == "P"
             pipelines += PipelineAttribute("sensor") == ["SA", "SB"]
```

### Comparing `pytroll_db-0.2.0/trolldb/errors/errors.py` & `pytroll_db-0.3.0/trolldb/errors/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 This module only includes the generic utilities using which each module should define its own error responses
 specifically. See :obj:`trolldb.database.errors` as an example on how to achieve this.
 """
 
 from collections import OrderedDict
 from sys import exit
-from typing import Self
+from typing import ClassVar, NoReturn, Self
 
 from fastapi import Response
 from fastapi.responses import PlainTextResponse
 from loguru import logger
 
 StatusCode = int
 """An alias for the built-in ``int`` type, which is used for HTTP status codes."""
@@ -27,17 +27,17 @@
           If the input is itself a list of strings the same list is returned as-is, otherwise, the given input
           string is enclosed in ``[]`` and returned.
 
     Example:
         .. code-block:: python
 
             # The following evaluate to True
-            __listify("test") == ["test"]
-            __listify(["a", "b"]) = ["a", "b"]
-            __listify([]) == []
+            _listify("test") == ["test"]
+            _listify(["a", "b"]) = ["a", "b"]
+            _listify([]) == []
     """
     return item if isinstance(item, list) else [item]
 
 
 def _stringify(item: str | list[str], delimiter: str) -> str:
     """Makes a single string out of the item(s) by delimiting them with ``delimiter``.
 
@@ -60,32 +60,31 @@
 
     Attributes:
         __dict (``OrderedDict[StatusCode, str]``):
             An ordered dictionary in which the keys are (HTTP) status codes and the values are the corresponding
             messages.
     """
 
-    descriptor_delimiter: str = " |OR| "
+    descriptor_delimiter: ClassVar[str] = " |OR| "
     """A delimiter to divide the message part of several error responses which have been combined into a single one.
 
     This will be shown in textual format for the response descriptors of the Fast API routes.
 
     Example:
         .. code-block:: python
 
             error_a = ResponseError({400: "Bad Request"})
             error_b = ResponseError({404: "Not Found"})
             errors = error_a | error_b
 
-            # When used in a FastAPI response descriptor,
-            # the following string will be generated for errors
+            # When used in a FastAPI response descriptor, the following string is generated
             "Bad Request |OR| Not Found"
     """
 
-    DefaultResponseClass: Response = PlainTextResponse
+    DefaultResponseClass: ClassVar[Response] = PlainTextResponse
     """The default type of the response which will be returned when an error occurs.
 
     This must be a valid member (class) of ``fastapi.responses``.
     """
 
     def __init__(self, args_dict: OrderedDict[StatusCode, str | list[str]] | dict) -> None:
         """Initializes the error object given a dictionary of error (HTTP) codes (keys) and messages (values).
@@ -97,20 +96,20 @@
             .. code-block:: python
 
                 # The following are all valid error objects
                 error_a = ResponseError({400: "Bad Request"})
                 error_b = ResponseError({404: "Not Found"})
                 errors = error_a | error_b
                 errors_a_or_b = ResponseError({400: "Bad Request", 404: "Not Found"})
-                errors_list = ResponseError({404: ["Not Found", "Still Not Found"]})
+                errors_list = ResponseError({404: ["Not Found", "Yet Not Found"]})
         """
         self.__dict: OrderedDict = OrderedDict(args_dict)
         self.extra_information: dict | None = None
 
-    def __or__(self, other: Self):
+    def __or__(self, other: Self) -> Self:
         """Implements the bitwise `or` ``|`` which combines the error objects into a single error response.
 
         Args:
             other:
                 Another error response of the same base type to combine with.
 
         Returns:
@@ -138,15 +137,15 @@
             self_msg = buff.get(key, None)
             buff[key] = _listify(self_msg) if self_msg else []
             buff[key].extend(_listify(msg))
         return ResponseError(buff)
 
     def __retrieve_one_from_some(
             self,
-            status_code: StatusCode | None = None) -> (StatusCode, str):
+            status_code: StatusCode | None = None) -> tuple[StatusCode, str]:
         """Retrieves a tuple ``(<status-code>, <message>)`` from the internal dictionary :obj:`ResponseError.__dict`.
 
         Args:
             status_code (Optional, default ``None``):
                 The status code to retrieve from the internal dictionary. In case of ``None``, the internal dictionary
                 must include only a single entry which will be returned.
 
@@ -179,44 +178,44 @@
             # The internal dictionary is empty and the status code is None.
             case _:
                 return 500, "Generic Response Error"
 
     def get_error_details(
             self,
             extra_information: dict | None = None,
-            status_code: int | None = None) -> (StatusCode, str):
+            status_code: int | None = None) -> tuple[StatusCode, str]:
         """Gets the details of the error response.
 
         Args:
             extra_information (Optional, default ``None``):
-                More information (if any) that wants to be added to the message string.
+                More information (if any) that needs to be added to the message string.
             status_code (Optional, default ``None``):
                 The status code to retrieve. This is useful when there are several error items in the internal
                 dictionary. In case of ``None``, the internal dictionary must include a single entry, otherwise an error
                 is raised.
 
         Returns:
             A tuple, in which the first element is the status code and the second element is a single string message.
         """
         status_code, msg = self.__retrieve_one_from_some(status_code)
         return status_code, msg + (f" :=> {extra_information}" if extra_information else "")
 
     def log_as_warning(
             self,
             extra_information: dict | None = None,
-            status_code: int | None = None):
+            status_code: int | None = None) -> None:
         """Same as :func:`~ResponseError.get_error_details` but logs the error as a warning and returns ``None``."""
         msg, _ = self.get_error_details(extra_information, status_code)
         logger.warning(msg)
 
     def sys_exit_log(
             self,
             exit_code: int = -1,
             extra_information: dict | None = None,
-            status_code: int | None = None) -> None:
+            status_code: int | None = None) -> NoReturn:
         """Same as :func:`~ResponseError.get_error_details` but logs the error and calls the ``sys.exit``.
 
         The arguments are the same as :func:`~ResponseError.get_error_details` with the addition of ``exit_code``
         which is optional and is set to ``-1`` by default.
 
         Warning:
             This is supposed to be done in case of non-recoverable errors, e.g. database issues. For other cases, we try
@@ -229,14 +228,19 @@
         logger.error(msg)
         exit(exit_code)
 
     @property
     def fastapi_descriptor(self) -> dict[StatusCode, dict[str, str]]:
         """Gets the FastAPI descriptor (dictionary) of the error items stored in :obj:`ResponseError.__dict`.
 
+        Note:
+            Consult the FastAPI documentation for
+            `additional responses <https://fastapi.tiangolo.com/advanced/additional-responses/>`_ to see why and how
+            descriptors are used.
+
         Example:
              .. code-block:: python
 
             error_a = ResponseError({400: "Bad Request"})
             error_b = ResponseError({404: "Not Found"})
             error_c = ResponseError({400: "Still Bad Request"})
```

### Comparing `pytroll_db-0.2.0/trolldb/test_utils/common.py` & `pytroll_db-0.3.0/trolldb/test_utils/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,32 +6,32 @@
 import yaml
 from pydantic import AnyUrl, FilePath
 from urllib3 import BaseHTTPResponse, request
 
 from trolldb.config.config import AppConfig
 
 
-def make_test_app_config(subscriber_address: Optional[FilePath] = None) -> dict:
+def make_test_app_config(subscriber_address: Optional[FilePath] = None) -> dict[str, dict]:
     """Makes the app configuration when used in testing.
 
     Args:
         subscriber_address:
             The address of the subscriber if it is of type ``FilePath``. Otherwise, if it is ``None`` the ``subscriber``
             config will be an empty dictionary.
 
     Returns:
-        A dictionary which resembles an object of type :obj:`AppConfig`.
+        A dictionary which resembles an object of type :obj:`~trolldb.config.config.AppConfig`.
     """
     app_config = dict(
         api_server=dict(
             url="http://localhost:8080"
         ),
         database=dict(
-            main_database_name="mock_database",
-            main_collection_name="mock_collection",
+            main_database_name="test_database",
+            main_collection_name="test_collection",
             url="mongodb://localhost:28017",
             timeout=1
         ),
         subscriber=dict(
             nameserver=False,
             addresses=[f"ipc://{subscriber_address}/in.ipc"] if subscriber_address is not None else [""],
             port=3000
```

### Comparing `pytroll_db-0.2.0/trolldb/test_utils/mongodb_instance.py` & `pytroll_db-0.3.0/trolldb/test_utils/mongodb_instance.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,66 +3,69 @@
 import subprocess
 import sys
 import tempfile
 import time
 from contextlib import contextmanager
 from os import mkdir, path
 from shutil import rmtree
+from typing import Any, AnyStr, ClassVar, Generator, Optional
 
 from loguru import logger
 
 from trolldb.config.config import DatabaseConfig, Timeout
 from trolldb.test_utils.common import test_app_config
 from trolldb.test_utils.mongodb_database import TestDatabase
 
 
 class TestMongoInstance:
     """A static class to enclose functionalities for running a MongoDB instance."""
 
-    log_dir: str = tempfile.mkdtemp("__pytroll_db_temp_test_log")
+    log_dir: ClassVar[str] = tempfile.mkdtemp("__pytroll_db_temp_test_log")
     """Temp directory for logging messages by the MongoDB instance.
 
     Warning:
-        The value of this attribute as shown above is just an example and will change in an unpredictable (secure) way!
+        The value of this attribute as shown above is just an example and will change in an unpredictable (secure) way
+        every time!
     """
 
-    storage_dir: str = tempfile.mkdtemp("__pytroll_db_temp_test_storage")
+    storage_dir: ClassVar[str] = tempfile.mkdtemp("__pytroll_db_temp_test_storage")
     """Temp directory for storing database files by the MongoDB instance.
 
     Warning:
-        The value of this attribute as shown above is just an example and will change in an unpredictable (secure) way!
+        The value of this attribute as shown above is just an example and will change in an unpredictable (secure) way
+        every time!
     """
 
-    port: int = 28017
+    port: ClassVar[int] = 28017
     """The port on which the instance will run.
 
     Warning:
         This must be always hard-coded.
     """
 
-    process: subprocess.Popen | None = None
+    process: ClassVar[Optional[subprocess.Popen]] = None
     """The process which is used to run the MongoDB instance."""
 
     @classmethod
-    def __prepare_dir(cls, directory: str):
+    def __prepare_dir(cls, directory: str) -> None:
         """An auxiliary function to prepare a single directory.
 
         It creates a directory if it does not exist, or removes it first if it exists and then recreates it.
         """
         cls.__remove_dir(directory)
         mkdir(directory)
 
     @classmethod
-    def __remove_dir(cls, directory: str):
+    def __remove_dir(cls, directory: str) -> None:
         """An auxiliary function to remove a directory and all its content recursively."""
         if path.exists(directory) and path.isdir(directory):
             rmtree(directory)
 
     @classmethod
-    def run_subprocess(cls, args: list[str], wait=True):
+    def run_subprocess(cls, args: list[str], wait=True) -> tuple[AnyStr, AnyStr] | None:
         """Runs the subprocess in shell given its arguments."""
         # We suppress ruff (S603) here as we are not receiving any args from outside, e.g. port is hard-coded.
         # Therefore, sanitization of arguments is not required.
         cls.process = subprocess.Popen(args, stdout=subprocess.PIPE, stderr=subprocess.PIPE)  # noqa: S603
         if wait:
             outs, errs = cls.process.communicate()
             return outs, errs
@@ -79,33 +82,33 @@
     @classmethod
     def prepare_dirs(cls) -> None:
         """Prepares the temp directories."""
         for d in [cls.log_dir, cls.storage_dir]:
             cls.__prepare_dir(d)
 
     @classmethod
-    def run_instance(cls):
+    def run_instance(cls) -> None:
         """Runs the MongoDB instance and does not wait for it, i.e. the process runs in the background."""
         cls.run_subprocess(
             ["mongod", "--dbpath", cls.storage_dir, "--logpath", f"{cls.log_dir}/mongod.log", "--port", f"{cls.port}"]
             , wait=False)
 
     @classmethod
-    def shutdown_instance(cls):
+    def shutdown_instance(cls) -> None:
         """Shuts down the MongoDB instance by terminating its process."""
         cls.process.terminate()
         cls.process.wait()
         for d in [cls.log_dir, cls.storage_dir]:
             cls.__remove_dir(d)
 
 
 @contextmanager
 def mongodb_instance_server_process_context(
         database_config: DatabaseConfig = test_app_config.database,
-        startup_time: Timeout = 2):
+        startup_time: Timeout = 2) -> Generator[Any, Any, None]:
     """A synchronous context manager to run the MongoDB instance in a separate process (non-blocking).
 
      It uses the `subprocess <https://docs.python.org/3/library/subprocess.html>`_ package. The main use case is
      envisaged to be in testing environments.
 
     Args:
         database_config:
@@ -127,12 +130,12 @@
         time.sleep(startup_time)
         yield
     finally:
         TestMongoInstance.shutdown_instance()
 
 
 @contextmanager
-def running_prepared_database_context():
+def running_prepared_database_context() -> Generator[Any, Any, None]:
     """A synchronous context manager to start and prepare a database instance for tests."""
     with mongodb_instance_server_process_context():
         TestDatabase.prepare()
         yield
```

### Comparing `pytroll_db-0.2.0/trolldb/tests/conftest.py` & `pytroll_db-0.3.0/trolldb/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytroll_db-0.2.0/trolldb/tests/test_recorder.py` & `pytroll_db-0.3.0/trolldb/tests/test_recorder.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 """Tests for the message recording into database."""
 
 import pytest
 from posttroll.message import Message
 from posttroll.testing import patched_subscriber_recv
 from pytest_lazy_fixtures import lf
 
-from trolldb.cli import record_messages, record_messages_from_command_line, record_messages_from_config
+from trolldb.cli import (
+    delete_uri_from_collection,
+    record_messages,
+    record_messages_from_command_line,
+    record_messages_from_config,
+)
 from trolldb.database.mongodb import MongoDB, mongodb_context
 from trolldb.test_utils.common import AppConfig, create_config_file, make_test_app_config, test_app_config
 from trolldb.test_utils.mongodb_instance import running_prepared_database_context
 
 
 @pytest.fixture()
 def file_message(tmp_data_filename):
@@ -19,14 +24,25 @@
             '"start_time": "2019-11-03T15:39:36.543000", "end_time": "2019-11-03T15:40:40.821000", "orbit_number": '
             '18765, "random_string1": "0235EA", "random_string2": "747D", "uri": '
             f'"{str(tmp_data_filename)}", "uid": "20191103_153936-s1b-ew-hh.tiff", '
             '"polarization": "hh", "sensor": "sar-c", "format": "GeoTIFF", "pass_direction": "ASCENDING"}')
 
 
 @pytest.fixture()
+def dataset_message(tmp_data_filename):
+    """Create a string for a file message."""
+    return ('pytroll://segment/raster/L2/SAR dataset a001673@c20969.ad.smhi.se 2019-11-05T13:00:10.366023 v1.01 '
+            'application/json {"platform_name": "S1B", "scan_mode": "EW", "type": "GRDM", "data_source": "1SDH", '
+            '"start_time": "2019-11-03T15:39:36.543000", "end_time": "2019-11-03T15:40:40.821000", "orbit_number": '
+            '18765, "random_string1": "0235EA", "random_string2": "747D", "dataset": [{"uri": '
+            f'"{str(tmp_data_filename)}", "uid": "20191103_153936-s1b-ew-hh.tiff"}}], '
+            '"polarization": "hh", "sensor": "sar-c", "format": "GeoTIFF", "pass_direction": "ASCENDING"}')
+
+
+@pytest.fixture()
 def del_message(tmp_data_filename):
     """Create a string for a delete message."""
     return ('pytroll://deletion del a001673@c20969.ad.smhi.se 2019-11-05T13:00:10.366023 v1.01 '
             'application/json {"platform_name": "S1B", "scan_mode": "EW", "type": "GRDM", "data_source": "1SDH", '
             '"start_time": "2019-11-03T15:39:36.543000", "end_time": "2019-11-03T15:40:40.821000", "orbit_number": '
             '18765, "random_string1": "0235EA", "random_string2": "747D", "uri": '
             f'"{str(tmp_data_filename)}", "uid": "20191103_153936-s1b-ew-hh.tiff", '
@@ -42,37 +58,41 @@
 
 @pytest.fixture()
 def config_file(tmp_path):
     """A fixture to create a config file for the tests."""
     return create_config_file(tmp_path)
 
 
-async def message_in_database_and_delete_count_is_one(msg) -> bool:
-    """Checks if there is exactly one item in the database which matches the data of the message."""
-    async with mongodb_context(test_app_config.database):
-        collection = await MongoDB.get_collection("mock_database", "mock_collection")
-        result = await collection.find_one(dict(scan_mode="EW"))
-        result.pop("_id")
-        deletion_result = await collection.delete_many({"uri": msg.data["uri"]})
-        return result == msg.data and deletion_result.deleted_count == 1
-
-
 @pytest.mark.parametrize(("function", "args"), [
     (record_messages_from_config, lf("config_file")),
     (record_messages_from_command_line, [lf("config_file")])
 ])
 async def test_record_from_cli_and_config(tmp_path, file_message, tmp_data_filename, function, args):
     """Tests that message recording adds a message to the database either via configs from a file or the CLI."""
     msg = Message.decode(file_message)
     with running_prepared_database_context():
         with patched_subscriber_recv([file_message]):
             await function(args)
             assert await message_in_database_and_delete_count_is_one(msg)
 
 
+async def message_in_database_and_delete_count_is_one(msg: Message) -> bool:
+    """Checks if there is exactly one item in the database which matches the data of the message."""
+    async with mongodb_context(test_app_config.database):
+        collection = await MongoDB.get_collection("test_database", "test_collection")
+        result = await collection.find_one(dict(scan_mode="EW"))
+        result.pop("_id")
+        uri = msg.data.get("uri")
+        if not uri:
+            uri = msg.data["dataset"][0]["uri"]
+        deletion_count = await delete_uri_from_collection(collection, uri)
+
+        return result == msg.data and deletion_count == 1
+
+
 async def test_record_messages(config_file, tmp_path, file_message, tmp_data_filename):
     """Tests that message recording adds a message to the database."""
     config = AppConfig(**make_test_app_config(tmp_path))
     msg = Message.decode(file_message)
     with running_prepared_database_context():
         with patched_subscriber_recv([file_message]):
             await record_messages(config)
@@ -82,10 +102,20 @@
 async def test_record_deletes_message(tmp_path, file_message, del_message):
     """Tests that message recording can delete a record in the database."""
     config = AppConfig(**make_test_app_config(tmp_path))
     with running_prepared_database_context():
         with patched_subscriber_recv([file_message, del_message]):
             await record_messages(config)
             async with mongodb_context(config.database):
-                collection = await MongoDB.get_collection("mock_database", "mock_collection")
+                collection = await MongoDB.get_collection("test_database", "test_collection")
                 result = await collection.find_one(dict(scan_mode="EW"))
                 assert result is None
+
+
+async def test_record_dataset_messages(tmp_path, dataset_message):
+    """Tests recording a dataset message and deleting the file."""
+    config = AppConfig(**make_test_app_config(tmp_path))
+    msg = Message.decode(dataset_message)
+    with running_prepared_database_context():
+        with patched_subscriber_recv([dataset_message]):
+            await record_messages(config)
+            assert await message_in_database_and_delete_count_is_one(msg)
```

### Comparing `pytroll_db-0.2.0/trolldb/tests/tests_database/test_mongodb.py` & `pytroll_db-0.3.0/trolldb/tests/tests_database/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `pytroll_db-0.2.0/trolldb/tests/tests_database/test_pipelines.py` & `pytroll_db-0.3.0/trolldb/tests/tests_database/test_pipelines.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Tests for the pipelines and applying comparison operations on them."""
-from trolldb.database.piplines import PipelineAttribute, PipelineBooleanDict, Pipelines
+from trolldb.database.pipelines import PipelineAttribute, PipelineBooleanDict, Pipelines
 from trolldb.test_utils.common import compare_by_operator_name
 
 
 def test_pipeline_boolean_dict():
     """Checks the pipeline boolean dict for bitwise `and/or` operators."""
     pd1 = PipelineBooleanDict({"number": 2})
     pd2 = PipelineBooleanDict({"kind": 1})
```

### Comparing `pytroll_db-0.2.0/.gitignore` & `pytroll_db-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytroll_db-0.2.0/LICENSE` & `pytroll_db-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytroll_db-0.2.0/README.rst` & `pytroll_db-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `pytroll_db-0.2.0/pyproject.toml` & `pytroll_db-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytroll_db-0.2.0/PKG-INFO` & `pytroll_db-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pytroll-db
-Version: 0.2.0
+Version: 0.3.0
 Summary: The database API of Pytroll.
 Project-URL: Documentation, https://pytroll-db.readthedocs.io/en/latest/
 Author-email: Pouria Khalaj <pouria.khalaj@smhi.se>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

