# Comparing `tmp/prefect_sqlalchemy-0.4.3.tar.gz` & `tmp/prefect_sqlalchemy-0.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_sqlalchemy-0.4.3.tar", last modified: Thu May 16 20:56:02 2024, max compression
+gzip compressed data, was "prefect_sqlalchemy-0.5.0rc1.tar", last modified: Fri May 31 20:49:46 2024, max compression
```

## Comparing `prefect_sqlalchemy-0.4.3.tar` & `prefect_sqlalchemy-0.5.0rc1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:56:02.599934 prefect_sqlalchemy-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-16 20:55:50.000000 prefect_sqlalchemy-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 20:55:50.000000 prefect_sqlalchemy-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10600 2024-05-16 20:56:02.599934 prefect_sqlalchemy-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8826 2024-05-16 20:55:50.000000 prefect_sqlalchemy-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:56:02.595934 prefect_sqlalchemy-0.4.3/prefect_sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-16 20:55:50.000000 prefect_sqlalchemy-0.4.3/prefect_sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 20:56:02.000000 prefect_sqlalchemy-0.4.3/prefect_sqlalchemy/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    15377 2024-05-16 20:55:50.000000 prefect_sqlalchemy-0.4.3/prefect_sqlalchemy/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    35914 2024-05-16 20:55:50.000000 prefect_sqlalchemy-0.4.3/prefect_sqlalchemy/database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:56:02.595934 prefect_sqlalchemy-0.4.3/prefect_sqlalchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10600 2024-05-16 20:56:02.000000 prefect_sqlalchemy-0.4.3/prefect_sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-16 20:56:02.000000 prefect_sqlalchemy-0.4.3/prefect_sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:56:02.000000 prefect_sqlalchemy-0.4.3/prefect_sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-16 20:56:02.000000 prefect_sqlalchemy-0.4.3/prefect_sqlalchemy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-16 20:56:02.000000 prefect_sqlalchemy-0.4.3/prefect_sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-16 20:56:02.000000 prefect_sqlalchemy-0.4.3/prefect_sqlalchemy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-16 20:55:50.000000 prefect_sqlalchemy-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:56:02.599934 prefect_sqlalchemy-0.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:56:02.595934 prefect_sqlalchemy-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-16 20:55:50.000000 prefect_sqlalchemy-0.4.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-16 20:55:50.000000 prefect_sqlalchemy-0.4.3/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-05-16 20:55:50.000000 prefect_sqlalchemy-0.4.3/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    23372 2024-05-16 20:55:50.000000 prefect_sqlalchemy-0.4.3/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-16 20:55:50.000000 prefect_sqlalchemy-0.4.3/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:46.989595 prefect_sqlalchemy-0.5.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-31 20:49:35.000000 prefect_sqlalchemy-0.5.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-31 20:49:35.000000 prefect_sqlalchemy-0.5.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10485 2024-05-31 20:49:46.989595 prefect_sqlalchemy-0.5.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8826 2024-05-31 20:49:35.000000 prefect_sqlalchemy-0.5.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:46.985595 prefect_sqlalchemy-0.5.0rc1/prefect_sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-31 20:49:35.000000 prefect_sqlalchemy-0.5.0rc1/prefect_sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-31 20:49:46.000000 prefect_sqlalchemy-0.5.0rc1/prefect_sqlalchemy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15214 2024-05-31 20:49:35.000000 prefect_sqlalchemy-0.5.0rc1/prefect_sqlalchemy/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29716 2024-05-31 20:49:35.000000 prefect_sqlalchemy-0.5.0rc1/prefect_sqlalchemy/database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:46.985595 prefect_sqlalchemy-0.5.0rc1/prefect_sqlalchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10485 2024-05-31 20:49:46.000000 prefect_sqlalchemy-0.5.0rc1/prefect_sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-31 20:49:46.000000 prefect_sqlalchemy-0.5.0rc1/prefect_sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:49:46.000000 prefect_sqlalchemy-0.5.0rc1/prefect_sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-31 20:49:46.000000 prefect_sqlalchemy-0.5.0rc1/prefect_sqlalchemy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-31 20:49:46.000000 prefect_sqlalchemy-0.5.0rc1/prefect_sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-31 20:49:46.000000 prefect_sqlalchemy-0.5.0rc1/prefect_sqlalchemy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-31 20:49:35.000000 prefect_sqlalchemy-0.5.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 20:49:46.989595 prefect_sqlalchemy-0.5.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:49:46.985595 prefect_sqlalchemy-0.5.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-31 20:49:35.000000 prefect_sqlalchemy-0.5.0rc1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-31 20:49:35.000000 prefect_sqlalchemy-0.5.0rc1/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-31 20:49:35.000000 prefect_sqlalchemy-0.5.0rc1/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18674 2024-05-31 20:49:35.000000 prefect_sqlalchemy-0.5.0rc1/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-31 20:49:35.000000 prefect_sqlalchemy-0.5.0rc1/tests/test_version.py
```

### Comparing `prefect_sqlalchemy-0.4.3/LICENSE` & `prefect_sqlalchemy-0.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect_sqlalchemy-0.4.3/PKG-INFO` & `prefect_sqlalchemy-0.5.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 Metadata-Version: 2.1
 Name: prefect-sqlalchemy
-Version: 0.4.3
+Version: 0.5.0rc1
 Summary: Prefect integrations for working with databases
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-sqlalchemy
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
 Requires-Dist: sqlalchemy<3,>=1.4.31
-Requires-Dist: prefect<3.0.0,>=2.13.5
+Requires-Dist: prefect>=3.0.0rc1
 Provides-Extra: dev
 Requires-Dist: aiosqlite; extra == "dev"
 Requires-Dist: asyncpg; extra == "dev"
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
 Requires-Dist: psycopg2; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
@@ -186,15 +184,15 @@
 
 Install `prefect-sqlalchemy` with `pip`:
 
 ```bash
 pip install prefect-sqlalchemy
 ```
 
-Requires an installation of Python 3.8 or higher.
+Requires an installation of Python 3.9 or higher.
 
 We recommend using a Python virtual environment manager such as pipenv, conda, or virtualenv.
 
 The tasks in this library are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Saving credentials to a block
```

#### html2text {}

```diff
@@ -1,32 +1,30 @@
-Metadata-Version: 2.1 Name: prefect-sqlalchemy Version: 0.4.3 Summary: Prefect
-integrations for working with databases Author-email: "Prefect Technologies,
-Inc."
+Metadata-Version: 2.1 Name: prefect-sqlalchemy Version: 0.5.0rc1 Summary:
+Prefect integrations for working with databases Author-email: "Prefect
+Technologies, Inc."
 prefect.io> License: Apache License 2.0 Project-URL: Homepage, https://
 github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-sqlalchemy
 Keywords: prefect Classifier: Natural Language :: English Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
-Topic :: Software Development :: Libraries Requires-Python: >=3.8 Description-
-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-sqlalchemy<3,>=1.4.31 Requires-Dist: prefect<3.0.0,>=2.13.5 Provides-Extra: dev
-Requires-Dist: aiosqlite; extra == "dev" Requires-Dist: asyncpg; extra == "dev"
-Requires-Dist: coverage; extra == "dev" Requires-Dist: interrogate; extra ==
-"dev" Requires-Dist: mkdocs-gen-files; extra == "dev" Requires-Dist: mkdocs-
-material; extra == "dev" Requires-Dist: mkdocs; extra == "dev" Requires-Dist:
-mkdocstrings[python]; extra == "dev" Requires-Dist: mock; python_version <
-"3.8" and extra == "dev" Requires-Dist: mypy; extra == "dev" Requires-Dist:
-pillow; extra == "dev" Requires-Dist: pre-commit; extra == "dev" Requires-Dist:
-psycopg2; extra == "dev" Requires-Dist: pytest-asyncio; extra == "dev"
-Requires-Dist: pytest-xdist; extra == "dev" Requires-Dist: pytest; extra ==
-"dev" # prefect-sqlalchemy
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Topic :: Software Development :: Libraries Requires-
+Python: >=3.9 Description-Content-Type: text/markdown License-File: LICENSE
+Requires-Dist: sqlalchemy<3,>=1.4.31 Requires-Dist: prefect>=3.0.0rc1 Provides-
+Extra: dev Requires-Dist: aiosqlite; extra == "dev" Requires-Dist: asyncpg;
+extra == "dev" Requires-Dist: coverage; extra == "dev" Requires-Dist:
+interrogate; extra == "dev" Requires-Dist: mkdocs-gen-files; extra == "dev"
+Requires-Dist: mkdocs-material; extra == "dev" Requires-Dist: mkdocs; extra ==
+"dev" Requires-Dist: mkdocstrings[python]; extra == "dev" Requires-Dist: mypy;
+extra == "dev" Requires-Dist: pillow; extra == "dev" Requires-Dist: pre-commit;
+extra == "dev" Requires-Dist: psycopg2; extra == "dev" Requires-Dist: pytest-
+asyncio; extra == "dev" Requires-Dist: pytest-xdist; extra == "dev" Requires-
+Dist: pytest; extra == "dev" # prefect-sqlalchemy
                 _[_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_p_r_e_f_e_c_t_-
                   _s_q_l_a_l_c_h_e_m_y_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]
 Visit the full docs [here](https://PrefectHQ.github.io/prefect-sqlalchemy) to
 see additional examples and the API reference. The prefect-sqlalchemy
 collection makes it easy to connect to a database in your Prefect flows. Check
 out the examples below to get started! ## Getting started ### Integrate with
 Prefect flows Prefect and SQLAlchemy are a data powerhouse duo. With Prefect,
@@ -78,15 +76,15 @@
 break all_rows.append(new_rows) return all_rows @flow async def sqlalchemy_flow
 (block_name: str) -> list: await setup_table(block_name) all_rows = await
 fetch_data(block_name) return all_rows asyncio.run(sqlalchemy_flow("BLOCK-NAME-
 PLACEHOLDER")) ``` ## Resources For more tips on how to use tasks and flows
 provided in a Prefect integration library, check out the [Prefect docs on using
 integrations](https://docs.prefect.io/integrations/usage/). ### Installation
 Install `prefect-sqlalchemy` with `pip`: ```bash pip install prefect-sqlalchemy
-``` Requires an installation of Python 3.8 or higher. We recommend using a
+``` Requires an installation of Python 3.9 or higher. We recommend using a
 Python virtual environment manager such as pipenv, conda, or virtualenv. The
 tasks in this library are designed to work with Prefect 2. For more information
 about how to use Prefect, please refer to the [Prefect documentation](https://
 docs.prefect.io/). ### Saving credentials to a block To use the `load` method
 on Blocks, you must have a block document [saved through code](https://
 docs.prefect.io/concepts/blocks/#saving-blocks) or saved through the UI. Below
 is a walkthrough on saving block documents through code; simply create a short
```

### Comparing `prefect_sqlalchemy-0.4.3/README.md` & `prefect_sqlalchemy-0.5.0rc1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 
 Install `prefect-sqlalchemy` with `pip`:
 
 ```bash
 pip install prefect-sqlalchemy
 ```
 
-Requires an installation of Python 3.8 or higher.
+Requires an installation of Python 3.9 or higher.
 
 We recommend using a Python virtual environment manager such as pipenv, conda, or virtualenv.
 
 The tasks in this library are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Saving credentials to a block
```

#### html2text {}

```diff
@@ -54,15 +54,15 @@
 break all_rows.append(new_rows) return all_rows @flow async def sqlalchemy_flow
 (block_name: str) -> list: await setup_table(block_name) all_rows = await
 fetch_data(block_name) return all_rows asyncio.run(sqlalchemy_flow("BLOCK-NAME-
 PLACEHOLDER")) ``` ## Resources For more tips on how to use tasks and flows
 provided in a Prefect integration library, check out the [Prefect docs on using
 integrations](https://docs.prefect.io/integrations/usage/). ### Installation
 Install `prefect-sqlalchemy` with `pip`: ```bash pip install prefect-sqlalchemy
-``` Requires an installation of Python 3.8 or higher. We recommend using a
+``` Requires an installation of Python 3.9 or higher. We recommend using a
 Python virtual environment manager such as pipenv, conda, or virtualenv. The
 tasks in this library are designed to work with Prefect 2. For more information
 about how to use Prefect, please refer to the [Prefect documentation](https://
 docs.prefect.io/). ### Saving credentials to a block To use the `load` method
 on Blocks, you must have a block document [saved through code](https://
 docs.prefect.io/concepts/blocks/#saving-blocks) or saved through the UI. Below
 is a walkthrough on saving block documents through code; simply create a short
```

### Comparing `prefect_sqlalchemy-0.4.3/prefect_sqlalchemy/credentials.py` & `prefect_sqlalchemy-0.5.0rc1/prefect_sqlalchemy/credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 """Credential classes used to perform authenticated interactions with SQLAlchemy"""
 
 import warnings
 from enum import Enum
 from typing import Any, Dict, Optional, Union
 
-from pydantic import VERSION as PYDANTIC_VERSION
-
-from prefect.blocks.core import Block
-
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import AnyUrl, BaseModel, Field, SecretStr
-else:
-    from pydantic import AnyUrl, BaseModel, Field, SecretStr
-
+from pydantic import AnyUrl, BaseModel, Field, SecretStr
 from sqlalchemy.engine import Connection, create_engine
 from sqlalchemy.engine.url import URL, make_url
 from sqlalchemy.ext.asyncio import AsyncConnection, create_async_engine
 from sqlalchemy.pool import NullPool
 
+from prefect.blocks.core import Block
+
 
 class AsyncDriver(Enum):
     """
     Known dialects with their corresponding async drivers.
 
     Attributes:
         POSTGRESQL_ASYNCPG (Enum): [postgresql+asyncpg](https://docs.sqlalchemy.org/en/14/dialects/postgresql.html#module-sqlalchemy.dialects.postgresql.asyncpg)
@@ -115,15 +109,15 @@
     )
     password: Optional[SecretStr] = Field(
         default=None, description="The password used to authenticate."
     )
     host: Optional[str] = Field(
         default=None, description="The host address of the database."
     )
-    port: Optional[str] = Field(
+    port: Optional[int] = Field(
         default=None, description="The port to connect to the database."
     )
     query: Optional[Dict[str, str]] = Field(
         default=None,
         description=(
             "A dictionary of string keys to string values to be passed to the dialect "
             "and/or the DBAPI upon connect. To specify non-string parameters to a "
```

### Comparing `prefect_sqlalchemy-0.4.3/prefect_sqlalchemy/database.py` & `prefect_sqlalchemy-0.5.0rc1/prefect_sqlalchemy/database.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,196 +1,30 @@
 """Tasks for querying a database with SQLAlchemy"""
 
-import contextlib
-import warnings
 from contextlib import AsyncExitStack, ExitStack, asynccontextmanager
 from typing import Any, Dict, List, Optional, Tuple, Union
 
-from pydantic import VERSION as PYDANTIC_VERSION
-
-from prefect import task
-from prefect.blocks.abstract import CredentialsBlock, DatabaseBlock
-from prefect.utilities.asyncutils import sync_compatible
-from prefect.utilities.hashing import hash_objects
-
-if PYDANTIC_VERSION.startswith("2."):
-    from pydantic.v1 import AnyUrl, Field, SecretStr
-else:
-    from pydantic import AnyUrl, Field, SecretStr
-
+from pydantic import AnyUrl, ConfigDict, Field
 from sqlalchemy import __version__ as SQLALCHEMY_VERSION
 from sqlalchemy.engine import Connection, Engine, create_engine
 from sqlalchemy.engine.cursor import CursorResult
-from sqlalchemy.engine.url import URL, make_url
+from sqlalchemy.engine.url import make_url
 from sqlalchemy.ext.asyncio import AsyncConnection, AsyncEngine, create_async_engine
 from sqlalchemy.sql import text
 from typing_extensions import Literal
 
+from prefect.blocks.abstract import CredentialsBlock, DatabaseBlock
+from prefect.utilities.asyncutils import sync_compatible
+from prefect.utilities.hashing import hash_objects
 from prefect_sqlalchemy.credentials import (
     AsyncDriver,
     ConnectionComponents,
-    DatabaseCredentials,
 )
 
 
-@contextlib.asynccontextmanager
-async def _connect(
-    engine: Union["AsyncEngine", "Engine"],
-    async_supported: bool,
-) -> Union["AsyncConnection", "Connection"]:
-    """
-    Helper method to create a connection to the database, either
-    synchronously or asynchronously.
-    """
-    try:
-        # a context manager nested within a context manager!
-        if async_supported:
-            async with engine.connect() as connection:
-                yield connection
-        else:
-            with engine.connect() as connection:
-                yield connection
-    finally:
-        dispose = engine.dispose()
-        if async_supported:
-            await dispose
-
-
-async def _execute(
-    connection: Union["AsyncConnection", "Connection"],
-    query: str,
-    params: Optional[Union[Tuple[Any], Dict[str, Any]]],
-    async_supported: bool,
-) -> "CursorResult":
-    """
-    Helper method to execute database queries or statements, either
-    synchronously or asynchronously.
-    """
-    result = connection.execute(text(query), params)
-    if async_supported:
-        result = await result
-        await connection.commit()
-    elif SQLALCHEMY_VERSION.startswith("2."):
-        connection.commit()
-    return result
-
-
-@task
-async def sqlalchemy_execute(
-    statement: str,
-    sqlalchemy_credentials: "DatabaseCredentials",
-    params: Optional[Union[Tuple[Any], Dict[str, Any]]] = None,
-):
-    """
-    Executes a SQL DDL or DML statement; useful for creating tables and inserting rows
-    since this task does not return any objects.
-
-    Args:
-        statement: The statement to execute against the database.
-        sqlalchemy_credentials: The credentials to use to authenticate.
-        params: The params to replace the placeholders in the query.
-
-    Examples:
-        Create table named customers and insert values.
-        ```python
-        from prefect_sqlalchemy import DatabaseCredentials, AsyncDriver
-        from prefect_sqlalchemy.database import sqlalchemy_execute
-        from prefect import flow
-
-        @flow
-        def sqlalchemy_execute_flow():
-            sqlalchemy_credentials = DatabaseCredentials(
-                driver=AsyncDriver.SQLITE_AIOSQLITE,
-                database="prefect.db",
-            )
-            sqlalchemy_execute(
-                "CREATE TABLE IF NOT EXISTS customers (name varchar, address varchar);",
-                sqlalchemy_credentials,
-            )
-            sqlalchemy_execute(
-                "INSERT INTO customers (name, address) VALUES (:name, :address);",
-                sqlalchemy_credentials,
-                params={"name": "Marvin", "address": "Highway 42"}
-            )
-
-        sqlalchemy_execute_flow()
-        ```
-    """
-    warnings.warn(
-        "sqlalchemy_query is now deprecated and will be removed March 2023; "
-        "please use SqlAlchemyConnector execute_* methods instead.",
-        DeprecationWarning,
-    )
-    # do not return anything or else results in the error:
-    # This result object does not return rows. It has been closed automatically
-    engine = sqlalchemy_credentials.get_engine()
-    async_supported = sqlalchemy_credentials._driver_is_async
-    async with _connect(engine, async_supported) as connection:
-        await _execute(connection, statement, params, async_supported)
-
-
-@task
-async def sqlalchemy_query(
-    query: str,
-    sqlalchemy_credentials: "DatabaseCredentials",
-    params: Optional[Union[Tuple[Any], Dict[str, Any]]] = None,
-    limit: Optional[int] = None,
-) -> List[Tuple[Any]]:
-    """
-    Executes a SQL query; useful for querying data from existing tables.
-
-    Args:
-        query: The query to execute against the database.
-        sqlalchemy_credentials: The credentials to use to authenticate.
-        params: The params to replace the placeholders in the query.
-        limit: The number of rows to fetch. Note, this parameter is
-            executed on the client side, i.e. passed to `fetchmany`.
-            To limit on the server side, add the `LIMIT` clause, or
-            the dialect's equivalent clause, like `TOP`, to the query.
-
-    Returns:
-        The fetched results.
-
-    Examples:
-        Query postgres table with the ID value parameterized.
-        ```python
-        from prefect_sqlalchemy import DatabaseCredentials, AsyncDriver
-        from prefect_sqlalchemy.database import sqlalchemy_query
-        from prefect import flow
-
-        @flow
-        def sqlalchemy_query_flow():
-            sqlalchemy_credentials = DatabaseCredentials(
-                driver=AsyncDriver.SQLITE_AIOSQLITE,
-                database="prefect.db",
-            )
-            result = sqlalchemy_query(
-                "SELECT * FROM customers WHERE name = :name;",
-                sqlalchemy_credentials,
-                params={"name": "Marvin"},
-            )
-            return result
-
-        sqlalchemy_query_flow()
-        ```
-    """
-    warnings.warn(
-        "sqlalchemy_query is now deprecated and will be removed March 2023; "
-        "please use SqlAlchemyConnector fetch_* methods instead.",
-        DeprecationWarning,
-    )
-    engine = sqlalchemy_credentials.get_engine()
-    async_supported = sqlalchemy_credentials._driver_is_async
-    async with _connect(engine, async_supported) as connection:
-        result = await _execute(connection, query, params, async_supported)
-        # some databases, like sqlite, require a connection still open to fetch!
-        rows = result.fetchall() if limit is None else result.fetchmany(limit)
-    return rows
-
-
 class SqlAlchemyConnector(CredentialsBlock, DatabaseBlock):
     """
     Block used to manage authentication with a database.
 
     Upon instantiating, an engine is created and maintained for the life of
     the object until the close method is called.
 
@@ -244,16 +78,17 @@
                 size=10
             )
         print(results)
         ```
     """
 
     _block_type_name = "SQLAlchemy Connector"
-    _logo_url = "https://cdn.sanity.io/images/3ugk85nk/production/3c7dff04f70aaf4528e184a3b028f9e40b98d68c-250x250.png"  # noqa
-    _documentation_url = "https://prefecthq.github.io/prefect-sqlalchemy/database/#prefect_sqlalchemy.database.SqlAlchemyConnector"  # noqa
+    _logo_url = "https://cdn.sanity.io/images/3ugk85nk/production/3c7dff04f70aaf4528e184a3b028f9e40b98d68c-250x250.png"  # type: ignore
+    _documentation_url = "https://prefecthq.github.io/prefect-sqlalchemy/database/#prefect_sqlalchemy.database.SqlAlchemyConnector"  # type: ignore
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
     connection_info: Union[ConnectionComponents, AnyUrl] = Field(
         default=...,
         description=(
             "SQLAlchemy URL to create the engine; either create from components "
             "or create from a string."
         ),
@@ -267,34 +102,16 @@
         ),
     )
     fetch_size: int = Field(
         default=1, description="The number of rows to fetch at a time."
     )
 
     _engine: Optional[Union[AsyncEngine, Engine]] = None
-    _exit_stack: Union[ExitStack, AsyncExitStack] = None
-    _unique_results: Dict[str, CursorResult] = None
-
-    class Config:
-        """Configuration of pydantic."""
-
-        # Support serialization of the 'URL' type
-        arbitrary_types_allowed = True
-        json_encoders = {URL: lambda u: u.render_as_string()}
-
-    def dict(self, *args, **kwargs) -> Dict:
-        """
-        Convert to a dictionary.
-        """
-        # Support serialization of the 'URL' type
-        d = super().dict(*args, **kwargs)
-        d["_rendered_url"] = SecretStr(
-            self._rendered_url.render_as_string(hide_password=False)
-        )
-        return d
+    _exit_stack: Optional[Union[ExitStack, AsyncExitStack]] = None
+    _unique_results: Optional[Dict[str, CursorResult]] = None
 
     def block_initialization(self):
         """
         Initializes the engine.
         """
         super().block_initialization()
```

### Comparing `prefect_sqlalchemy-0.4.3/prefect_sqlalchemy.egg-info/PKG-INFO` & `prefect_sqlalchemy-0.5.0rc1/prefect_sqlalchemy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 Metadata-Version: 2.1
 Name: prefect-sqlalchemy
-Version: 0.4.3
+Version: 0.5.0rc1
 Summary: Prefect integrations for working with databases
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-sqlalchemy
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
 Requires-Dist: sqlalchemy<3,>=1.4.31
-Requires-Dist: prefect<3.0.0,>=2.13.5
+Requires-Dist: prefect>=3.0.0rc1
 Provides-Extra: dev
 Requires-Dist: aiosqlite; extra == "dev"
 Requires-Dist: asyncpg; extra == "dev"
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
 Requires-Dist: psycopg2; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
@@ -186,15 +184,15 @@
 
 Install `prefect-sqlalchemy` with `pip`:
 
 ```bash
 pip install prefect-sqlalchemy
 ```
 
-Requires an installation of Python 3.8 or higher.
+Requires an installation of Python 3.9 or higher.
 
 We recommend using a Python virtual environment manager such as pipenv, conda, or virtualenv.
 
 The tasks in this library are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
 
 ### Saving credentials to a block
```

#### html2text {}

```diff
@@ -1,32 +1,30 @@
-Metadata-Version: 2.1 Name: prefect-sqlalchemy Version: 0.4.3 Summary: Prefect
-integrations for working with databases Author-email: "Prefect Technologies,
-Inc."
+Metadata-Version: 2.1 Name: prefect-sqlalchemy Version: 0.5.0rc1 Summary:
+Prefect integrations for working with databases Author-email: "Prefect
+Technologies, Inc."
 prefect.io> License: Apache License 2.0 Project-URL: Homepage, https://
 github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-sqlalchemy
 Keywords: prefect Classifier: Natural Language :: English Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
-Topic :: Software Development :: Libraries Requires-Python: >=3.8 Description-
-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-sqlalchemy<3,>=1.4.31 Requires-Dist: prefect<3.0.0,>=2.13.5 Provides-Extra: dev
-Requires-Dist: aiosqlite; extra == "dev" Requires-Dist: asyncpg; extra == "dev"
-Requires-Dist: coverage; extra == "dev" Requires-Dist: interrogate; extra ==
-"dev" Requires-Dist: mkdocs-gen-files; extra == "dev" Requires-Dist: mkdocs-
-material; extra == "dev" Requires-Dist: mkdocs; extra == "dev" Requires-Dist:
-mkdocstrings[python]; extra == "dev" Requires-Dist: mock; python_version <
-"3.8" and extra == "dev" Requires-Dist: mypy; extra == "dev" Requires-Dist:
-pillow; extra == "dev" Requires-Dist: pre-commit; extra == "dev" Requires-Dist:
-psycopg2; extra == "dev" Requires-Dist: pytest-asyncio; extra == "dev"
-Requires-Dist: pytest-xdist; extra == "dev" Requires-Dist: pytest; extra ==
-"dev" # prefect-sqlalchemy
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Topic :: Software Development :: Libraries Requires-
+Python: >=3.9 Description-Content-Type: text/markdown License-File: LICENSE
+Requires-Dist: sqlalchemy<3,>=1.4.31 Requires-Dist: prefect>=3.0.0rc1 Provides-
+Extra: dev Requires-Dist: aiosqlite; extra == "dev" Requires-Dist: asyncpg;
+extra == "dev" Requires-Dist: coverage; extra == "dev" Requires-Dist:
+interrogate; extra == "dev" Requires-Dist: mkdocs-gen-files; extra == "dev"
+Requires-Dist: mkdocs-material; extra == "dev" Requires-Dist: mkdocs; extra ==
+"dev" Requires-Dist: mkdocstrings[python]; extra == "dev" Requires-Dist: mypy;
+extra == "dev" Requires-Dist: pillow; extra == "dev" Requires-Dist: pre-commit;
+extra == "dev" Requires-Dist: psycopg2; extra == "dev" Requires-Dist: pytest-
+asyncio; extra == "dev" Requires-Dist: pytest-xdist; extra == "dev" Requires-
+Dist: pytest; extra == "dev" # prefect-sqlalchemy
                 _[_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_p_r_e_f_e_c_t_-
                   _s_q_l_a_l_c_h_e_m_y_?_c_o_l_o_r_=_0_0_5_2_F_F_&_l_a_b_e_l_C_o_l_o_r_=_0_9_0_4_2_2_]
 Visit the full docs [here](https://PrefectHQ.github.io/prefect-sqlalchemy) to
 see additional examples and the API reference. The prefect-sqlalchemy
 collection makes it easy to connect to a database in your Prefect flows. Check
 out the examples below to get started! ## Getting started ### Integrate with
 Prefect flows Prefect and SQLAlchemy are a data powerhouse duo. With Prefect,
@@ -78,15 +76,15 @@
 break all_rows.append(new_rows) return all_rows @flow async def sqlalchemy_flow
 (block_name: str) -> list: await setup_table(block_name) all_rows = await
 fetch_data(block_name) return all_rows asyncio.run(sqlalchemy_flow("BLOCK-NAME-
 PLACEHOLDER")) ``` ## Resources For more tips on how to use tasks and flows
 provided in a Prefect integration library, check out the [Prefect docs on using
 integrations](https://docs.prefect.io/integrations/usage/). ### Installation
 Install `prefect-sqlalchemy` with `pip`: ```bash pip install prefect-sqlalchemy
-``` Requires an installation of Python 3.8 or higher. We recommend using a
+``` Requires an installation of Python 3.9 or higher. We recommend using a
 Python virtual environment manager such as pipenv, conda, or virtualenv. The
 tasks in this library are designed to work with Prefect 2. For more information
 about how to use Prefect, please refer to the [Prefect documentation](https://
 docs.prefect.io/). ### Saving credentials to a block To use the `load` method
 on Blocks, you must have a block document [saved through code](https://
 docs.prefect.io/concepts/blocks/#saving-blocks) or saved through the UI. Below
 is a walkthrough on saving block documents through code; simply create a short
```

### Comparing `prefect_sqlalchemy-0.4.3/prefect_sqlalchemy.egg-info/SOURCES.txt` & `prefect_sqlalchemy-0.5.0rc1/prefect_sqlalchemy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect_sqlalchemy-0.4.3/pyproject.toml` & `prefect_sqlalchemy-0.5.0rc1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 [build-system]
 requires = ["setuptools>=45", "wheel", "setuptools_scm>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prefect-sqlalchemy"
-dependencies = ["sqlalchemy>=1.4.31,<3", "prefect>=2.13.5, < 3.0.0"]
+dependencies = [
+  "sqlalchemy>=1.4.31,<3",
+  "prefect>=3.0.0rc1",
+]
 dynamic = ["version"]
 description = "Prefect integrations for working with databases"
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
 
@@ -32,15 +34,14 @@
   "asyncpg",
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
   "psycopg2",
   "pytest-asyncio",
   "pytest-xdist",
   "pytest",
@@ -51,15 +52,15 @@
 
 [project.entry-points."prefect.collections"]
 prefect_sqlalchemy = "prefect_sqlalchemy"
 
 [tool.setuptools_scm]
 version_file = "prefect_sqlalchemy/_version.py"
 root = "../../.."
-tag_regex = "^prefect-sqlalchemy-(?P<version>\\d+\\.\\d+\\.\\d+)$"
+tag_regex = "^prefect-sqlalchemy-(?P<version>\\d+\\.\\d+\\.\\d+(?:[a-zA-Z0-9]+(?:\\.[a-zA-Z0-9]+)*)?)$"
 fallback_version = "0.0.0"
 git_describe_command = 'git describe --dirty --tags --long --match "prefect-sqlalchemy-*[0-9]*"'
 
 [tool.interrogate]
 ignore-init-module = true
 ignore_init_method = true
 exclude = ["prefect_sqlalchemy/_version.py", "tests"]
```

### Comparing `prefect_sqlalchemy-0.4.3/tests/conftest.py` & `prefect_sqlalchemy-0.5.0rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prefect_sqlalchemy-0.4.3/tests/test_block_standards.py` & `prefect_sqlalchemy-0.5.0rc1/tests/test_block_standards.py`

 * *Files identical despite different names*

