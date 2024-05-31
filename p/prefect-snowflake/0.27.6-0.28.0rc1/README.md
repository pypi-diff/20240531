# Comparing `tmp/prefect_snowflake-0.27.6.tar.gz` & `tmp/prefect_snowflake-0.28.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_snowflake-0.27.6.tar", last modified: Thu May 16 20:58:43 2024, max compression
+gzip compressed data, was "prefect_snowflake-0.28.0rc1.tar", last modified: Fri May 31 20:49:46 2024, max compression
```

## Comparing `prefect_snowflake-0.27.6.tar` & `prefect_snowflake-0.28.0rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:43.862519 prefect_snowflake-0.27.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-16 20:58:32.000000 prefect_snowflake-0.27.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 20:58:32.000000 prefect_snowflake-0.27.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11238 2024-05-16 20:58:43.858519 prefect_snowflake-0.27.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9569 2024-05-16 20:58:32.000000 prefect_snowflake-0.27.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:43.854519 prefect_snowflake-0.27.6/prefect_snowflake/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-16 20:58:32.000000 prefect_snowflake-0.27.6/prefect_snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-16 20:58:43.000000 prefect_snowflake-0.27.6/prefect_snowflake/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12965 2024-05-16 20:58:32.000000 prefect_snowflake-0.27.6/prefect_snowflake/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    30138 2024-05-16 20:58:32.000000 prefect_snowflake-0.27.6/prefect_snowflake/database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:43.858519 prefect_snowflake-0.27.6/prefect_snowflake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11238 2024-05-16 20:58:43.000000 prefect_snowflake-0.27.6/prefect_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-16 20:58:43.000000 prefect_snowflake-0.27.6/prefect_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:58:43.000000 prefect_snowflake-0.27.6/prefect_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-16 20:58:43.000000 prefect_snowflake-0.27.6/prefect_snowflake.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-16 20:58:43.000000 prefect_snowflake-0.27.6/prefect_snowflake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 20:58:43.000000 prefect_snowflake-0.27.6/prefect_snowflake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-16 20:58:32.000000 prefect_snowflake-0.27.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:58:43.862519 prefect_snowflake-0.27.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:43.858519 prefect_snowflake-0.27.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-05-16 20:58:32.000000 prefect_snowflake-0.27.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-16 20:58:32.000000 prefect_snowflake-0.27.6/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)    16774 2024-05-16 20:58:32.000000 prefect_snowflake-0.27.6/tests/test_credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:43.858519 prefect_snowflake-0.27.6/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-16 20:58:32.000000 prefect_snowflake-0.27.6/tests/test_data/test_cert.p8
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-16 20:58:32.000000 prefect_snowflake-0.27.6/tests/test_data/test_cert_malformed_format.p8
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-16 20:58:32.000000 prefect_snowflake-0.27.6/tests/test_data/test_cert_no_pass.p8
--rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-05-16 20:58:32.000000 prefect_snowflake-0.27.6/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-16 20:58:32.000000 prefect_snowflake-0.27.6/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:46.253561 prefect_snowflake-0.28.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-31 20:49:35.000000 prefect_snowflake-0.28.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-31 20:49:35.000000 prefect_snowflake-0.28.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11123 2024-05-31 20:49:46.253561 prefect_snowflake-0.28.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9569 2024-05-31 20:49:35.000000 prefect_snowflake-0.28.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:46.245561 prefect_snowflake-0.28.0rc1/prefect_snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-31 20:49:35.000000 prefect_snowflake-0.28.0rc1/prefect_snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-31 20:49:45.000000 prefect_snowflake-0.28.0rc1/prefect_snowflake/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12825 2024-05-31 20:49:35.000000 prefect_snowflake-0.28.0rc1/prefect_snowflake/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46074 2024-05-31 20:49:35.000000 prefect_snowflake-0.28.0rc1/prefect_snowflake/database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:46.249561 prefect_snowflake-0.28.0rc1/prefect_snowflake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11123 2024-05-31 20:49:45.000000 prefect_snowflake-0.28.0rc1/prefect_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-31 20:49:46.000000 prefect_snowflake-0.28.0rc1/prefect_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:49:45.000000 prefect_snowflake-0.28.0rc1/prefect_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-31 20:49:45.000000 prefect_snowflake-0.28.0rc1/prefect_snowflake.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-31 20:49:45.000000 prefect_snowflake-0.28.0rc1/prefect_snowflake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-31 20:49:45.000000 prefect_snowflake-0.28.0rc1/prefect_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-31 20:49:35.000000 prefect_snowflake-0.28.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 20:49:46.253561 prefect_snowflake-0.28.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:46.249561 prefect_snowflake-0.28.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-31 20:49:35.000000 prefect_snowflake-0.28.0rc1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-31 20:49:35.000000 prefect_snowflake-0.28.0rc1/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16642 2024-05-31 20:49:35.000000 prefect_snowflake-0.28.0rc1/tests/test_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:46.249561 prefect_snowflake-0.28.0rc1/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-31 20:49:35.000000 prefect_snowflake-0.28.0rc1/tests/test_data/test_cert.p8
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-31 20:49:35.000000 prefect_snowflake-0.28.0rc1/tests/test_data/test_cert_malformed_format.p8
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-31 20:49:35.000000 prefect_snowflake-0.28.0rc1/tests/test_data/test_cert_no_pass.p8
+-rw-r--r--   0 runner    (1001) docker     (127)    13120 2024-05-31 20:49:35.000000 prefect_snowflake-0.28.0rc1/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-31 20:49:35.000000 prefect_snowflake-0.28.0rc1/tests/test_version.py
```

### Comparing `prefect_snowflake-0.27.6/LICENSE` & `prefect_snowflake-0.28.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect_snowflake-0.27.6/PKG-INFO` & `prefect_snowflake-0.28.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 Metadata-Version: 2.1
 Name: prefect-snowflake
-Version: 0.27.6
+Version: 0.28.0rc1
 Summary: Prefect integrations for interacting with Snowflake
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-snowflake
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: snowflake-connector-python>=2.7.6
-Requires-Dist: prefect<3.0.0,>=2.13.5
+Requires-Dist: prefect>=3.0.0rc1
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
-Requires-Dist: mock; python_version < "3.8" and extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pillow; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 
@@ -195,15 +193,15 @@
 
 ```bash
 pip install prefect-snowflake
 ```
 
 A list of available blocks in `prefect-snowflake` and their setup instructions can be found [here](https://PrefectHQ.github.io/prefect-snowflake/blocks_catalog).
 
-Requires an installation of Python 3.8+.
+Requires an installation of Python 3.9+.
 
 We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
 
 These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Saving credentials to block
```

### Comparing `prefect_snowflake-0.27.6/README.md` & `prefect_snowflake-0.28.0rc1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
 
 ```bash
 pip install prefect-snowflake
 ```
 
 A list of available blocks in `prefect-snowflake` and their setup instructions can be found [here](https://PrefectHQ.github.io/prefect-snowflake/blocks_catalog).
 
-Requires an installation of Python 3.8+.
+Requires an installation of Python 3.9+.
 
 We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
 
 These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Saving credentials to block
```

### Comparing `prefect_snowflake-0.27.6/prefect_snowflake/credentials.py` & `prefect_snowflake-0.28.0rc1/prefect_snowflake/credentials.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,23 +15,18 @@
 
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
 import snowflake.connector
-from pydantic import VERSION as PYDANTIC_VERSION
+from pydantic import Field, SecretBytes, SecretStr, model_validator
 
 from prefect.blocks.abstract import CredentialsBlock
 
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import Field, SecretBytes, SecretField, SecretStr, root_validator
-else:
-    from pydantic import Field, SecretBytes, SecretField, SecretStr, root_validator
-
 # PEM certificates have the pattern:
 #   -----BEGIN PRIVATE KEY-----
 #   <- multiple lines of encoded data->
 #   -----END PRIVATE KEY-----
 #
 # The regex captures the header and footer into groups 1 and 3, the body into group 2
 # group 1: "header" captures series of hyphens followed by anything that is
@@ -76,15 +71,17 @@
     """  # noqa E501
 
     _block_type_name = "Snowflake Credentials"
     _logo_url = "https://cdn.sanity.io/images/3ugk85nk/production/bd359de0b4be76c2254bd329fe3a267a1a3879c2-250x250.png"  # noqa
     _documentation_url = "https://prefecthq.github.io/prefect-snowflake/credentials/#prefect_snowflake.credentials.SnowflakeCredentials"  # noqa
 
     account: str = Field(
-        ..., description="The snowflake account name.", example="nh12345.us-east-2.aws"
+        ...,
+        description="The snowflake account name.",
+        examples=["nh12345.us-east-2.aws"],
     )
     user: str = Field(..., description="The user name used to authenticate.")
     password: Optional[SecretStr] = Field(
         default=None, description="The password used to authenticate."
     )
     private_key: Optional[SecretBytes] = Field(
         default=None, description="The PEM used to authenticate."
@@ -121,15 +118,15 @@
     role: Optional[str] = Field(
         default=None, description="The name of the default role to use."
     )
     autocommit: Optional[bool] = Field(
         default=None, description="Whether to automatically commit."
     )
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
     def _validate_auth_kwargs(cls, values):
         """
         Ensure an authorization value has been provided by the user.
         """
         auth_params = (
             "password",
             "private_key",
@@ -149,28 +146,28 @@
         elif values.get("password") and values.get("private_key_passphrase"):
             raise ValueError(
                 "Do not provide both password and private_key_passphrase; "
                 "specify private_key_passphrase only instead."
             )
         return values
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
     def _validate_token_kwargs(cls, values):
         """
         Ensure an authorization value has been provided by the user.
         """
         authenticator = values.get("authenticator")
         token = values.get("token")
         if authenticator == "oauth" and not token:
             raise ValueError(
                 "If authenticator is set to `oauth`, `token` must be provided"
             )
         return values
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
     def _validate_okta_kwargs(cls, values):
         """
         Ensure an authorization value has been provided by the user.
         """
         authenticator = values.get("authenticator")
 
         # did not want to make a breaking change so we will allow both
@@ -246,15 +243,15 @@
         Args:
             secret: The value to decode.
 
         Returns:
             The decoded secret as bytes.
 
         """
-        if isinstance(secret, (SecretBytes, SecretStr)):
+        if isinstance(secret, (SecretStr, SecretBytes)):
             secret = secret.get_secret_value()
 
         if not isinstance(secret, (bytes, str)) or len(secret) == 0 or secret.isspace():
             return None
 
         return secret if isinstance(secret, bytes) else secret.encode()
 
@@ -319,20 +316,20 @@
 
             connection = snowflake_credentials_block.get_client(database="my_database")
             ```
         """  # noqa
         connect_params = {
             # required to track task's usage in the Snowflake Partner Network Portal
             "application": "Prefect_Snowflake_Collection",
-            **self.dict(exclude_unset=True, exclude={"block_type_slug"}),
+            **self.model_dump(exclude_unset=True, exclude={"block_type_slug"}),
             **connect_kwargs,
         }
 
         for key, value in connect_params.items():
-            if isinstance(value, SecretField):
+            if isinstance(value, (SecretStr, SecretBytes)):
                 connect_params[key] = connect_params[key].get_secret_value()
 
         # set authenticator to the actual okta_endpoint
         if connect_params.get("authenticator") == "okta_endpoint":
             endpoint = connect_params.pop("endpoint", None) or connect_params.pop(
                 "okta_endpoint", None
             )  # okta_endpoint is deprecated
```

### Comparing `prefect_snowflake-0.27.6/prefect_snowflake/database.py` & `prefect_snowflake-0.28.0rc1/prefect_snowflake/database.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 """Module for querying against Snowflake databases."""
 
 import asyncio
-from typing import Any, Dict, List, Optional, Tuple, Type, Union
+from time import sleep
+from typing import Any, Dict, List, Optional, Sequence, Tuple, Type, Union
 
-from pydantic import VERSION as PYDANTIC_VERSION
+from pydantic import Field
+from snowflake.connector.connection import SnowflakeConnection
+from snowflake.connector.cursor import SnowflakeCursor
 
 from prefect import task
 from prefect.blocks.abstract import DatabaseBlock
-from prefect.utilities.asyncutils import run_sync_in_worker_thread, sync_compatible
+from prefect.utilities.asyncutils import run_coro_as_sync, run_sync_in_worker_thread
 from prefect.utilities.hashing import hash_objects
-
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import Field
-else:
-    from pydantic import Field
-
-from snowflake.connector.connection import SnowflakeConnection
-from snowflake.connector.cursor import SnowflakeCursor
-
 from prefect_snowflake import SnowflakeCredentials
 
 BEGIN_TRANSACTION_STATEMENT = "BEGIN TRANSACTION"
 END_TRANSACTION_STATEMENT = "COMMIT"
 
 
 class SnowflakeConnector(DatabaseBlock):
@@ -184,15 +178,15 @@
             Whether a cursor is new and a Snowflake cursor.
         """
         self._start_connection()
 
         input_hash = hash_objects(inputs)
         if input_hash is None:
             raise RuntimeError(
-                "We were not able to hash your inputs, "
+                f"We were not able to hash your inputs, {inputs!r}, "
                 "which resulted in an unexpected data return; "
                 "please open an issue with a reproducible example."
             )
         if input_hash not in self._unique_cursors.keys():
             new_cursor = self._connection.cursor(cursor_type)
             self._unique_cursors[input_hash] = new_cursor
             return True, new_cursor
@@ -254,16 +248,15 @@
                 cursor.close()
             except Exception as exc:
                 self.logger.warning(
                     f"Failed to close cursor for input hash {input_hash!r}: {exc}"
                 )
         self.logger.info("Successfully reset the cursors.")
 
-    @sync_compatible
-    async def fetch_one(
+    def fetch_one(
         self,
         operation: str,
         parameters: Optional[Dict[str, Any]] = None,
         cursor_type: Type[SnowflakeCursor] = SnowflakeCursor,
         **execute_kwargs: Any,
     ) -> Tuple[Any]:
         """
@@ -310,24 +303,84 @@
         inputs = dict(
             command=operation,
             params=parameters,
             **execute_kwargs,
         )
         new, cursor = self._get_cursor(inputs, cursor_type=cursor_type)
         if new:
+            self.execute(
+                operation, parameters, cursor_type=cursor_type, **execute_kwargs
+            )
+        self.logger.debug("Preparing to fetch a row.")
+        return cursor.fetchone()
+
+    async def fetch_one_async(
+        self,
+        operation: str,
+        parameters: Optional[Dict[str, Any]] = None,
+        cursor_type: Type[SnowflakeCursor] = SnowflakeCursor,
+        **execute_kwargs: Any,
+    ) -> Tuple[Any]:
+        """
+        Fetch a single result from the database asynchronously.
+        Repeated calls using the same inputs to *any* of the fetch methods of this
+        block will skip executing the operation again, and instead,
+        return the next set of results from the previous execution,
+        until the reset_cursors method is called.
+
+        Args:
+            operation: The SQL query or other operation to be executed.
+            parameters: The parameters for the operation.
+            cursor_type: The class of the cursor to use when creating a Snowflake cursor.
+            **execute_kwargs: Additional options to pass to `cursor.execute_async`.
+
+        Returns:
+            A tuple containing the data returned by the database,
+                where each row is a tuple and each column is a value in the tuple.
+
+        Examples:
+            Fetch one row from the database where address is Space.
+            ```python
+            from prefect_snowflake.database import SnowflakeConnector
+
+            with SnowflakeConnector.load("BLOCK_NAME") as conn:
+                conn.execute(
+                    "CREATE TABLE IF NOT EXISTS customers (name varchar, address varchar);"
+                )
+                conn.execute_many(
+                    "INSERT INTO customers (name, address) VALUES (%(name)s, %(address)s);",
+                    seq_of_parameters=[
+                        {"name": "Ford", "address": "Highway 42"},
+                        {"name": "Unknown", "address": "Space"},
+                        {"name": "Me", "address": "Myway 88"},
+                    ],
+                )
+                result = await conn.fetch_one_async(
+                    "SELECT * FROM customers WHERE address = %(address)s",
+                    parameters={"address": "Space"}
+                )
+                print(result)
+            ```
+        """  # noqa
+        inputs = dict(
+            command=operation,
+            params=parameters,
+            **execute_kwargs,
+        )
+        new, cursor = self._get_cursor(inputs, cursor_type=cursor_type)
+        if new:
             await self._execute_async(cursor, inputs)
         self.logger.debug("Preparing to fetch a row.")
         result = await run_sync_in_worker_thread(cursor.fetchone)
         return result
 
-    @sync_compatible
-    async def fetch_many(
+    def fetch_many(
         self,
         operation: str,
-        parameters: Optional[Dict[str, Any]] = None,
+        parameters: Optional[Sequence[Dict[str, Any]]] = None,
         size: Optional[int] = None,
         cursor_type: Type[SnowflakeCursor] = SnowflakeCursor,
         **execute_kwargs: Any,
     ) -> List[Tuple[Any]]:
         """
         Fetch a limited number of results from the database.
         Repeated calls using the same inputs to *any* of the fetch methods of this
@@ -382,22 +435,130 @@
         inputs = dict(
             command=operation,
             params=parameters,
             **execute_kwargs,
         )
         new, cursor = self._get_cursor(inputs, cursor_type)
         if new:
+            self.execute(cursor, inputs)
+        size = size or self.fetch_size
+        self.logger.debug(f"Preparing to fetch {size} rows.")
+        return cursor.fetchmany(size=size)
+
+    async def fetch_many_async(
+        self,
+        operation: str,
+        parameters: Optional[Sequence[Dict[str, Any]]] = None,
+        size: Optional[int] = None,
+        cursor_type: Type[SnowflakeCursor] = SnowflakeCursor,
+        **execute_kwargs: Any,
+    ) -> List[Tuple[Any]]:
+        """
+        Fetch a limited number of results from the database asynchronously.
+        Repeated calls using the same inputs to *any* of the fetch methods of this
+        block will skip executing the operation again, and instead,
+        return the next set of results from the previous execution,
+        until the reset_cursors method is called.
+
+        Args:
+            operation: The SQL query or other operation to be executed.
+            parameters: The parameters for the operation.
+            size: The number of results to return; if None or 0, uses the value of
+                `fetch_size` configured on the block.
+            cursor_type: The class of the cursor to use when creating a Snowflake cursor.
+            **execute_kwargs: Additional options to pass to `cursor.execute_async`.
+
+        Returns:
+            A list of tuples containing the data returned by the database,
+                where each row is a tuple and each column is a value in the tuple.
+
+        Examples:
+            Repeatedly fetch two rows from the database where address is Highway 42.
+            ```python
+            from prefect_snowflake.database import SnowflakeConnector
+
+            with SnowflakeConnector.load("BLOCK_NAME") as conn:
+                conn.execute(
+                    "CREATE TABLE IF NOT EXISTS customers (name varchar, address varchar);"
+                )
+                conn.execute_many(
+                    "INSERT INTO customers (name, address) VALUES (%(name)s, %(address)s);",
+                    seq_of_parameters=[
+                        {"name": "Marvin", "address": "Highway 42"},
+                        {"name": "Ford", "address": "Highway 42"},
+                        {"name": "Unknown", "address": "Highway 42"},
+                        {"name": "Me", "address": "Highway 42"},
+                    ],
+                )
+                result = conn.fetch_many(
+                    "SELECT * FROM customers WHERE address = %(address)s",
+                    parameters={"address": "Highway 42"},
+                    size=2
+                )
+                print(result)  # Marvin, Ford
+                result = conn.fetch_many(
+                    "SELECT * FROM customers WHERE address = %(address)s",
+                    parameters={"address": "Highway 42"},
+                    size=2
+                )
+                print(result)  # Unknown, Me
+            ```
+        """  # noqa
+        inputs = dict(
+            command=operation,
+            params=parameters,
+            **execute_kwargs,
+        )
+        new, cursor = self._get_cursor(inputs, cursor_type)
+        if new:
             await self._execute_async(cursor, inputs)
         size = size or self.fetch_size
         self.logger.debug(f"Preparing to fetch {size} rows.")
         result = await run_sync_in_worker_thread(cursor.fetchmany, size=size)
         return result
 
-    @sync_compatible
-    async def fetch_all(
+    def fetch_all(
+        self,
+        operation: str,
+        parameters: Optional[Dict[str, Any]] = None,
+        cursor_type: Type[SnowflakeCursor] = SnowflakeCursor,
+        **execute_kwargs: Any,
+    ) -> List[Tuple[Any]]:
+        """
+        Fetch all results from the database.
+        Repeated calls using the same inputs to *any* of the fetch methods of this
+        block will skip executing the operation again, and instead,
+        return the next set of results from the previous execution,
+        until the reset_cursors method is called.
+
+        Args:
+            operation: The SQL query or other operation to be executed.
+            parameters: The parameters for the operation.
+            cursor_type: The class of the cursor to use when creating a Snowflake cursor.
+            **execute_kwargs: Additional options to pass to `cursor.execute_async`.
+
+        Returns:
+            A list of tuples containing the data returned by the database,
+                where each row is a tuple and each column is a value in the tuple.
+
+        """  # noqa
+        inputs = dict(
+            command=operation,
+            params=parameters,
+            **execute_kwargs,
+        )
+        new, cursor = self._get_cursor(inputs, cursor_type)
+        if new:
+            self.execute(
+                operation, parameters, cursor_type=cursor_type, **execute_kwargs
+            )
+        self.logger.debug("Preparing to fetch all rows.")
+        return cursor.fetchall()
+
+    async def fetch_all_async(
         self,
         operation: str,
         parameters: Optional[Dict[str, Any]] = None,
         cursor_type: Type[SnowflakeCursor] = SnowflakeCursor,
         **execute_kwargs: Any,
     ) -> List[Tuple[Any]]:
         """
@@ -419,27 +580,27 @@
 
         Examples:
             Fetch all rows from the database where address is Highway 42.
             ```python
             from prefect_snowflake.database import SnowflakeConnector
 
             with SnowflakeConnector.load("BLOCK_NAME") as conn:
-                conn.execute(
+                await conn.execute_async(
                     "CREATE TABLE IF NOT EXISTS customers (name varchar, address varchar);"
                 )
-                conn.execute_many(
+                await conn.execute_many_async(
                     "INSERT INTO customers (name, address) VALUES (%(name)s, %(address)s);",
                     seq_of_parameters=[
                         {"name": "Marvin", "address": "Highway 42"},
                         {"name": "Ford", "address": "Highway 42"},
                         {"name": "Unknown", "address": "Highway 42"},
                         {"name": "Me", "address": "Myway 88"},
                     ],
                 )
-                result = conn.fetch_all(
+                result = await conn.fetch_all_async(
                     "SELECT * FROM customers WHERE address = %(address)s",
                     parameters={"address": "Highway 42"},
                 )
                 print(result)  # Marvin, Ford, Unknown
             ```
         """  # noqa
         inputs = dict(
@@ -450,16 +611,56 @@
         new, cursor = self._get_cursor(inputs, cursor_type)
         if new:
             await self._execute_async(cursor, inputs)
         self.logger.debug("Preparing to fetch all rows.")
         result = await run_sync_in_worker_thread(cursor.fetchall)
         return result
 
-    @sync_compatible
-    async def execute(
+    def execute(
+        self,
+        operation: str,
+        parameters: Optional[Dict[str, Any]] = None,
+        cursor_type: Type[SnowflakeCursor] = SnowflakeCursor,
+        **execute_kwargs: Any,
+    ) -> None:
+        """
+        Executes an operation on the database. This method is intended to be used
+        for operations that do not return data, such as INSERT, UPDATE, or DELETE.
+        Unlike the fetch methods, this method will always execute the operation
+        upon calling.
+
+        Args:
+            operation: The SQL query or other operation to be executed.
+            parameters: The parameters for the operation.
+            cursor_type: The class of the cursor to use when creating a Snowflake cursor.
+            **execute_kwargs: Additional options to pass to `cursor.execute_async`.
+
+        Examples:
+            Create table named customers with two columns, name and address.
+            ```python
+            from prefect_snowflake.database import SnowflakeConnector
+
+            with SnowflakeConnector.load("BLOCK_NAME") as conn:
+                conn.execute(
+                    "CREATE TABLE IF NOT EXISTS customers (name varchar, address varchar);"
+                )
+            ```
+        """  # noqa
+        self._start_connection()
+
+        inputs = dict(
+            command=operation,
+            params=parameters,
+            **execute_kwargs,
+        )
+        with self._connection.cursor(cursor_type) as cursor:
+            run_coro_as_sync(self._execute_async(cursor, inputs))
+        self.logger.info(f"Executed the operation, {operation!r}.")
+
+    async def execute_async(
         self,
         operation: str,
         parameters: Optional[Dict[str, Any]] = None,
         cursor_type: Type[SnowflakeCursor] = SnowflakeCursor,
         **execute_kwargs: Any,
     ) -> None:
         """
@@ -492,16 +693,61 @@
             params=parameters,
             **execute_kwargs,
         )
         with self._connection.cursor(cursor_type) as cursor:
             await run_sync_in_worker_thread(cursor.execute, **inputs)
         self.logger.info(f"Executed the operation, {operation!r}.")
 
-    @sync_compatible
-    async def execute_many(
+    def execute_many(
+        self,
+        operation: str,
+        seq_of_parameters: List[Dict[str, Any]],
+    ) -> None:
+        """
+        Executes many operations on the database. This method is intended to be used
+        for operations that do not return data, such as INSERT, UPDATE, or DELETE.
+        Unlike the fetch methods, this method will always execute the operations
+        upon calling.
+
+        Args:
+            operation: The SQL query or other operation to be executed.
+            seq_of_parameters: The sequence of parameters for the operation.
+
+        Examples:
+            Create table and insert three rows into it.
+            ```python
+            from prefect_snowflake.database import SnowflakeConnector
+
+            with SnowflakeConnector.load("BLOCK_NAME") as conn:
+                conn.execute(
+                    "CREATE TABLE IF NOT EXISTS customers (name varchar, address varchar);"
+                )
+                conn.execute_many(
+                    "INSERT INTO customers (name, address) VALUES (%(name)s, %(address)s);",
+                    seq_of_parameters=[
+                        {"name": "Marvin", "address": "Highway 42"},
+                        {"name": "Ford", "address": "Highway 42"},
+                        {"name": "Unknown", "address": "Space"},
+                    ],
+                )
+            ```
+        """  # noqa
+        self._start_connection()
+
+        inputs = dict(
+            command=operation,
+            seqparams=seq_of_parameters,
+        )
+        with self._connection.cursor() as cursor:
+            cursor.executemany(**inputs)
+        self.logger.info(
+            f"Executed {len(seq_of_parameters)} operations off {operation!r}."
+        )
+
+    async def execute_many_async(
         self,
         operation: str,
         seq_of_parameters: List[Dict[str, Any]],
     ) -> None:
         """
         Executes many operations on the database. This method is intended to be used
         for operations that do not return data, such as INSERT, UPDATE, or DELETE.
@@ -578,15 +824,82 @@
     def __setstate__(self, data: dict):
         """Reset connection and cursors upon loading."""
         self.__dict__.update(data)
         self._start_connection()
 
 
 @task
-async def snowflake_query(
+def snowflake_query(
+    query: str,
+    snowflake_connector: SnowflakeConnector,
+    params: Union[Tuple[Any], Dict[str, Any]] = None,
+    cursor_type: Type[SnowflakeCursor] = SnowflakeCursor,
+    poll_frequency_seconds: int = 1,
+) -> List[Tuple[Any]]:
+    """
+    Executes a query against a Snowflake database.
+
+    Args:
+        query: The query to execute against the database.
+        params: The params to replace the placeholders in the query.
+        snowflake_connector: The credentials to use to authenticate.
+        cursor_type: The type of database cursor to use for the query.
+        poll_frequency_seconds: Number of seconds to wait in between checks for
+            run completion.
+
+    Returns:
+        The output of `response.fetchall()`.
+
+    Examples:
+        Query Snowflake table with the ID value parameterized.
+        ```python
+        from prefect import flow
+        from prefect_snowflake.credentials import SnowflakeCredentials
+        from prefect_snowflake.database import SnowflakeConnector, snowflake_query
+
+
+        @flow
+        def snowflake_query_flow():
+            snowflake_credentials = SnowflakeCredentials(
+                account="account",
+                user="user",
+                password="password",
+            )
+            snowflake_connector = SnowflakeConnector(
+                database="database",
+                warehouse="warehouse",
+                schema="schema",
+                credentials=snowflake_credentials
+            )
+            result = snowflake_query(
+                "SELECT * FROM table WHERE id=%{id_param}s LIMIT 8;",
+                snowflake_connector,
+                params={"id_param": 1}
+            )
+            return result
+
+        snowflake_query_flow()
+        ```
+    """
+    # context manager automatically rolls back failed transactions and closes
+    with snowflake_connector.get_connection() as connection:
+        with connection.cursor(cursor_type) as cursor:
+            response = cursor.execute_async(query, params=params)
+            query_id = response["queryId"]
+            while connection.is_still_running(
+                connection.get_query_status_throw_if_error(query_id)
+            ):
+                sleep(poll_frequency_seconds)
+            cursor.get_results_from_sfqid(query_id)
+            result = cursor.fetchall()
+    return result
+
+
+@task
+async def snowflake_query_async(
     query: str,
     snowflake_connector: SnowflakeConnector,
     params: Union[Tuple[Any], Dict[str, Any]] = None,
     cursor_type: Type[SnowflakeCursor] = SnowflakeCursor,
     poll_frequency_seconds: int = 1,
 ) -> List[Tuple[Any]]:
     """
@@ -645,15 +958,100 @@
                 await asyncio.sleep(poll_frequency_seconds)
             cursor.get_results_from_sfqid(query_id)
             result = cursor.fetchall()
     return result
 
 
 @task
-async def snowflake_multiquery(
+def snowflake_multiquery(
+    queries: List[str],
+    snowflake_connector: SnowflakeConnector,
+    params: Union[Tuple[Any], Dict[str, Any]] = None,
+    cursor_type: Type[SnowflakeCursor] = SnowflakeCursor,
+    as_transaction: bool = False,
+    return_transaction_control_results: bool = False,
+    poll_frequency_seconds: int = 1,
+) -> List[List[Tuple[Any]]]:
+    """
+    Executes multiple queries against a Snowflake database in a shared session.
+    Allows execution in a transaction.
+
+    Args:
+        queries: The list of queries to execute against the database.
+        params: The params to replace the placeholders in the query.
+        snowflake_connector: The credentials to use to authenticate.
+        cursor_type: The type of database cursor to use for the query.
+        as_transaction: If True, queries are executed in a transaction.
+        return_transaction_control_results: Determines if the results of queries
+            controlling the transaction (BEGIN/COMMIT) should be returned.
+        poll_frequency_seconds: Number of seconds to wait in between checks for
+            run completion.
+
+    Returns:
+        List of the outputs of `response.fetchall()` for each query.
+
+    Examples:
+        Query Snowflake table with the ID value parameterized.
+        ```python
+        from prefect import flow
+        from prefect_snowflake.credentials import SnowflakeCredentials
+        from prefect_snowflake.database import SnowflakeConnector, snowflake_multiquery
+
+
+        @flow
+        def snowflake_multiquery_flow():
+            snowflake_credentials = SnowflakeCredentials(
+                account="account",
+                user="user",
+                password="password",
+            )
+            snowflake_connector = SnowflakeConnector(
+                database="database",
+                warehouse="warehouse",
+                schema="schema",
+                credentials=snowflake_credentials
+            )
+            result = snowflake_multiquery(
+                ["SELECT * FROM table WHERE id=%{id_param}s LIMIT 8;", "SELECT 1,2"],
+                snowflake_connector,
+                params={"id_param": 1},
+                as_transaction=True
+            )
+            return result
+
+        snowflake_multiquery_flow()
+        ```
+    """
+    with snowflake_connector.get_connection() as connection:
+        if as_transaction:
+            queries.insert(0, BEGIN_TRANSACTION_STATEMENT)
+            queries.append(END_TRANSACTION_STATEMENT)
+
+        with connection.cursor(cursor_type) as cursor:
+            results = []
+            for query in queries:
+                response = cursor.execute_async(query, params=params)
+                query_id = response["queryId"]
+                while connection.is_still_running(
+                    connection.get_query_status_throw_if_error(query_id)
+                ):
+                    sleep(poll_frequency_seconds)
+                cursor.get_results_from_sfqid(query_id)
+                result = cursor.fetchall()
+                results.append(result)
+
+    # cut off results from BEGIN/COMMIT queries
+    if as_transaction and not return_transaction_control_results:
+        return results[1:-1]
+    else:
+        return results
+
+
+@task
+async def snowflake_multiquery_async(
     queries: List[str],
     snowflake_connector: SnowflakeConnector,
     params: Union[Tuple[Any], Dict[str, Any]] = None,
     cursor_type: Type[SnowflakeCursor] = SnowflakeCursor,
     as_transaction: bool = False,
     return_transaction_control_results: bool = False,
     poll_frequency_seconds: int = 1,
@@ -730,15 +1128,15 @@
     if as_transaction and not return_transaction_control_results:
         return results[1:-1]
     else:
         return results
 
 
 @task
-async def snowflake_query_sync(
+def snowflake_query_sync(
     query: str,
     snowflake_connector: SnowflakeConnector,
     params: Union[Tuple[Any], Dict[str, Any]] = None,
     cursor_type: Type[SnowflakeCursor] = SnowflakeCursor,
 ) -> List[Tuple[Any]]:
     """
     Executes a query in sync mode against a Snowflake database.
```

### Comparing `prefect_snowflake-0.27.6/prefect_snowflake.egg-info/PKG-INFO` & `prefect_snowflake-0.28.0rc1/prefect_snowflake.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 Metadata-Version: 2.1
 Name: prefect-snowflake
-Version: 0.27.6
+Version: 0.28.0rc1
 Summary: Prefect integrations for interacting with Snowflake
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-snowflake
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: snowflake-connector-python>=2.7.6
-Requires-Dist: prefect<3.0.0,>=2.13.5
+Requires-Dist: prefect>=3.0.0rc1
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
-Requires-Dist: mock; python_version < "3.8" and extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pillow; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 
@@ -195,15 +193,15 @@
 
 ```bash
 pip install prefect-snowflake
 ```
 
 A list of available blocks in `prefect-snowflake` and their setup instructions can be found [here](https://PrefectHQ.github.io/prefect-snowflake/blocks_catalog).
 
-Requires an installation of Python 3.8+.
+Requires an installation of Python 3.9+.
 
 We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
 
 These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Saving credentials to block
```

### Comparing `prefect_snowflake-0.27.6/prefect_snowflake.egg-info/SOURCES.txt` & `prefect_snowflake-0.28.0rc1/prefect_snowflake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect_snowflake-0.27.6/pyproject.toml` & `prefect_snowflake-0.28.0rc1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 [build-system]
 requires = ["setuptools>=45", "wheel", "setuptools_scm>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prefect-snowflake"
-dependencies = ["snowflake-connector-python>=2.7.6", "prefect>=2.13.5, < 3.0.0"]
+dependencies = [
+  "snowflake-connector-python>=2.7.6",
+  "prefect>=3.0.0rc1",
+]
 dynamic = ["version"]
 description = "Prefect integrations for interacting with Snowflake"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = { text = "Apache License 2.0" }
 keywords = ["prefect"]
 authors = [{ name = "Prefect Technologies, Inc.", email = "help@prefect.io" }]
 classifiers = [
   "Natural Language :: English",
   "Intended Audience :: Developers",
   "Intended Audience :: System Administrators",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Software Development :: Libraries",
 ]
 
@@ -30,15 +32,14 @@
 dev = [
   "coverage",
   "interrogate",
   "mkdocs-gen-files",
   "mkdocs-material",
   "mkdocs",
   "mkdocstrings[python]",
-  "mock; python_version < '3.8'",
   "mypy",
   "pillow",
   "pre-commit",
   "pytest-asyncio",
   "pytest",
   "pytest-xdist",
 ]
@@ -48,15 +49,15 @@
 
 [project.entry-points."prefect.collections"]
 prefect_snowflake = "prefect_snowflake"
 
 [tool.setuptools_scm]
 version_file = "prefect_snowflake/_version.py"
 root = "../../.."
-tag_regex = "^prefect-snowflake-(?P<version>\\d+\\.\\d+\\.\\d+)$"
+tag_regex = "^prefect-snowflake-(?P<version>\\d+\\.\\d+\\.\\d+(?:[a-zA-Z0-9]+(?:\\.[a-zA-Z0-9]+)*)?)$"
 fallback_version = "0.0.0"
 git_describe_command = 'git describe --dirty --tags --long --match "prefect-snowflake-*[0-9]*"'
 
 [tool.interrogate]
 ignore-init-module = true
 ignore_init_method = true
 exclude = ["prefect_snowflake/_version.py", "tests"]
```

### Comparing `prefect_snowflake-0.27.6/tests/conftest.py` & `prefect_snowflake-0.28.0rc1/tests/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,16 +21,22 @@
 
 
 @pytest.fixture(scope="session", autouse=True)
 def prefect_db():
     """
     Sets up test harness for temporary DB during test runs.
     """
-    with prefect_test_harness():
-        yield
+    try:
+        with prefect_test_harness():
+            yield
+    except OSError as e:
+        if "Directory not empty" in str(e):
+            pass
+        else:
+            raise e
 
 
 @pytest.fixture(autouse=True)
 def reset_object_registry():
     """
     Ensures each test has a clean object registry.
     """
@@ -46,26 +52,14 @@
         "account": "account",
         "user": "user",
         "password": "password",
     }
 
 
 @pytest.fixture()
-def connector_params(credentials_params):
-    snowflake_credentials = SnowflakeCredentials(**credentials_params)
-    _connector_params = {
-        "schema": "schema_input",
-        "database": "database",
-        "warehouse": "warehouse",
-        "credentials": snowflake_credentials,
-    }
-    return _connector_params
-
-
-@pytest.fixture()
 def private_credentials_params():
     return {
         "account": "account",
         "user": "user",
         "password": "letmein",
         "private_key": _read_test_file("test_cert.p8"),
     }
@@ -78,26 +72,14 @@
         "user": "user",
         "private_key_path": "path/to/private/key",
         "private_key_passphrase": "letmein",
     }
 
 
 @pytest.fixture()
-def private_connector_params(private_credentials_params):
-    snowflake_credentials = SnowflakeCredentials(**private_credentials_params)
-    _connector_params = {
-        "schema": "schema_input",
-        "database": "database",
-        "warehouse": "warehouse",
-        "credentials": snowflake_credentials,
-    }
-    return _connector_params
-
-
-@pytest.fixture()
 def private_no_pass_credentials_params():
     return {
         "account": "account",
         "user": "user",
         "password": "letmein",
         "private_key": _read_test_file("test_cert_no_pass.p8"),
     }
```

### Comparing `prefect_snowflake-0.27.6/tests/test_block_standards.py` & `prefect_snowflake-0.28.0rc1/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect_snowflake-0.27.6/tests/test_credentials.py` & `prefect_snowflake-0.28.0rc1/tests/test_credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 import sys
 from pathlib import Path
 from unittest.mock import MagicMock
 
 import pytest
-from pydantic import VERSION as PYDANTIC_VERSION
+from prefect_snowflake.credentials import InvalidPemFormat, SnowflakeCredentials
+from prefect_snowflake.database import SnowflakeConnector
+from pydantic import SecretBytes, SecretStr
 
 from prefect import flow
 from prefect.utilities.filesystem import relative_path_to_current_platform
 
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import SecretBytes, SecretStr
-else:
-    from pydantic import SecretBytes, SecretStr
-
-from prefect_snowflake.credentials import InvalidPemFormat, SnowflakeCredentials
-from prefect_snowflake.database import SnowflakeConnector
-
 
 def test_snowflake_credentials_init(credentials_params):
     snowflake_credentials = SnowflakeCredentials(**credentials_params)
-    actual_credentials_params = snowflake_credentials.dict()
+    actual_credentials_params = snowflake_credentials.model_dump()
     for param in credentials_params:
         actual = actual_credentials_params[param]
         expected = credentials_params[param]
         if isinstance(actual, SecretStr):
             actual = actual.get_secret_value()
         assert actual == expected
 
@@ -94,15 +88,15 @@
     credentials_params_missing["endpoint"] = "new.com"
     snowflake_credentials = SnowflakeCredentials(**credentials_params_missing)
     assert snowflake_credentials.endpoint == "new.com"
 
 
 def test_snowflake_private_credentials_init(private_credentials_params):
     snowflake_credentials = SnowflakeCredentials(**private_credentials_params)
-    actual_credentials_params = snowflake_credentials.dict()
+    actual_credentials_params = snowflake_credentials.model_dump()
     for param in private_credentials_params:
         actual = actual_credentials_params[param]
         expected = private_credentials_params[param]
         if isinstance(actual, (SecretStr, SecretBytes)):
             actual = actual.get_secret_value()
         if sys.platform != "win32":
             assert actual == expected
@@ -229,15 +223,15 @@
         assert credentials.resolve_private_key() is not None
 
 
 def test_snowflake_credentials_validate_private_key_path_init(
     private_key_path_credentials_params,
 ):
     snowflake_credentials = SnowflakeCredentials(**private_key_path_credentials_params)
-    actual_credentials_params = snowflake_credentials.dict()
+    actual_credentials_params = snowflake_credentials.model_dump()
     for param in private_key_path_credentials_params:
         actual = actual_credentials_params[param]
         expected = private_key_path_credentials_params[param]
         if isinstance(actual, (SecretStr, SecretBytes)):
             actual = actual.get_secret_value()
         elif isinstance(actual, Path):
             actual = relative_path_to_current_platform(actual)
```

### Comparing `prefect_snowflake-0.27.6/tests/test_data/test_cert.p8` & `prefect_snowflake-0.28.0rc1/tests/test_data/test_cert.p8`

 * *Files identical despite different names*

### Comparing `prefect_snowflake-0.27.6/tests/test_data/test_cert_malformed_format.p8` & `prefect_snowflake-0.28.0rc1/tests/test_data/test_cert_malformed_format.p8`

 * *Files identical despite different names*

### Comparing `prefect_snowflake-0.27.6/tests/test_data/test_cert_no_pass.p8` & `prefect_snowflake-0.28.0rc1/tests/test_data/test_cert_no_pass.p8`

 * *Files identical despite different names*

