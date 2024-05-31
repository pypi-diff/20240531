# Comparing `tmp/frequenz-client-microgrid-0.3.0.tar.gz` & `tmp/frequenz-client-microgrid-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-client-microgrid-0.3.0.tar", last modified: Thu Mar 28 17:19:48 2024, max compression
+gzip compressed data, was "frequenz-client-microgrid-0.4.0.tar", last modified: Fri May 31 15:50:47 2024, max compression
```

## Comparing `frequenz-client-microgrid-0.3.0.tar` & `frequenz-client-microgrid-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:19:48.427439 frequenz-client-microgrid-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-28 17:19:39.000000 frequenz-client-microgrid-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-28 17:19:39.000000 frequenz-client-microgrid-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-28 17:19:48.427439 frequenz-client-microgrid-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-28 17:19:39.000000 frequenz-client-microgrid-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-28 17:19:39.000000 frequenz-client-microgrid-0.3.0/RELEASE_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-03-28 17:19:39.000000 frequenz-client-microgrid-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 17:19:48.427439 frequenz-client-microgrid-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:19:48.427439 frequenz-client-microgrid-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:19:48.423439 frequenz-client-microgrid-0.3.0/src/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:19:48.427439 frequenz-client-microgrid-0.3.0/src/frequenz/client/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:19:48.427439 frequenz-client-microgrid-0.3.0/src/frequenz/client/microgrid/
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-28 17:19:39.000000 frequenz-client-microgrid-0.3.0/src/frequenz/client/microgrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18174 2024-03-28 17:19:39.000000 frequenz-client-microgrid-0.3.0/src/frequenz/client/microgrid/_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8283 2024-03-28 17:19:39.000000 frequenz-client-microgrid-0.3.0/src/frequenz/client/microgrid/_component.py
--rw-r--r--   0 runner    (1001) docker     (127)    21979 2024-03-28 17:19:39.000000 frequenz-client-microgrid-0.3.0/src/frequenz/client/microgrid/_component_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-03-28 17:19:39.000000 frequenz-client-microgrid-0.3.0/src/frequenz/client/microgrid/_component_states.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-03-28 17:19:39.000000 frequenz-client-microgrid-0.3.0/src/frequenz/client/microgrid/_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-28 17:19:39.000000 frequenz-client-microgrid-0.3.0/src/frequenz/client/microgrid/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-03-28 17:19:39.000000 frequenz-client-microgrid-0.3.0/src/frequenz/client/microgrid/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-28 17:19:39.000000 frequenz-client-microgrid-0.3.0/src/frequenz/client/microgrid/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:19:39.000000 frequenz-client-microgrid-0.3.0/src/frequenz/client/microgrid/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:19:48.427439 frequenz-client-microgrid-0.3.0/src/frequenz_client_microgrid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-28 17:19:48.000000 frequenz-client-microgrid-0.3.0/src/frequenz_client_microgrid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-03-28 17:19:48.000000 frequenz-client-microgrid-0.3.0/src/frequenz_client_microgrid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:19:48.000000 frequenz-client-microgrid-0.3.0/src/frequenz_client_microgrid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-03-28 17:19:48.000000 frequenz-client-microgrid-0.3.0/src/frequenz_client_microgrid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-28 17:19:48.000000 frequenz-client-microgrid-0.3.0/src/frequenz_client_microgrid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:50:47.473436 frequenz-client-microgrid-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-31 15:50:39.000000 frequenz-client-microgrid-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-31 15:50:39.000000 frequenz-client-microgrid-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-31 15:50:47.473436 frequenz-client-microgrid-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-31 15:50:39.000000 frequenz-client-microgrid-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-31 15:50:39.000000 frequenz-client-microgrid-0.4.0/RELEASE_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-05-31 15:50:39.000000 frequenz-client-microgrid-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:50:47.473436 frequenz-client-microgrid-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:50:47.469436 frequenz-client-microgrid-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:50:47.469436 frequenz-client-microgrid-0.4.0/src/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:50:47.469436 frequenz-client-microgrid-0.4.0/src/frequenz/client/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:50:47.473436 frequenz-client-microgrid-0.4.0/src/frequenz/client/microgrid/
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-31 15:50:39.000000 frequenz-client-microgrid-0.4.0/src/frequenz/client/microgrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16186 2024-05-31 15:50:39.000000 frequenz-client-microgrid-0.4.0/src/frequenz/client/microgrid/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8138 2024-05-31 15:50:39.000000 frequenz-client-microgrid-0.4.0/src/frequenz/client/microgrid/_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21562 2024-05-31 15:50:39.000000 frequenz-client-microgrid-0.4.0/src/frequenz/client/microgrid/_component_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-05-31 15:50:39.000000 frequenz-client-microgrid-0.4.0/src/frequenz/client/microgrid/_component_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-05-31 15:50:39.000000 frequenz-client-microgrid-0.4.0/src/frequenz/client/microgrid/_component_states.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-31 15:50:39.000000 frequenz-client-microgrid-0.4.0/src/frequenz/client/microgrid/_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-31 15:50:39.000000 frequenz-client-microgrid-0.4.0/src/frequenz/client/microgrid/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20390 2024-05-31 15:50:39.000000 frequenz-client-microgrid-0.4.0/src/frequenz/client/microgrid/_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-31 15:50:39.000000 frequenz-client-microgrid-0.4.0/src/frequenz/client/microgrid/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-31 15:50:39.000000 frequenz-client-microgrid-0.4.0/src/frequenz/client/microgrid/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:50:39.000000 frequenz-client-microgrid-0.4.0/src/frequenz/client/microgrid/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:50:47.473436 frequenz-client-microgrid-0.4.0/src/frequenz_client_microgrid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-31 15:50:47.000000 frequenz-client-microgrid-0.4.0/src/frequenz_client_microgrid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-31 15:50:47.000000 frequenz-client-microgrid-0.4.0/src/frequenz_client_microgrid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:50:47.000000 frequenz-client-microgrid-0.4.0/src/frequenz_client_microgrid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-31 15:50:47.000000 frequenz-client-microgrid-0.4.0/src/frequenz_client_microgrid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 15:50:47.000000 frequenz-client-microgrid-0.4.0/src/frequenz_client_microgrid.egg-info/top_level.txt
```

### Comparing `frequenz-client-microgrid-0.3.0/LICENSE` & `frequenz-client-microgrid-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-client-microgrid-0.3.0/PKG-INFO` & `frequenz-client-microgrid-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-client-microgrid
-Version: 0.3.0
+Version: 0.4.0
 Summary: Microgrid API client for Python
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Documentation, https://frequenz-floss.github.io/frequenz-client-microgrid-python/
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-client-microgrid-python/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-client-microgrid-python/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-client-microgrid-python
```

### Comparing `frequenz-client-microgrid-0.3.0/README.md` & `frequenz-client-microgrid-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `frequenz-client-microgrid-0.3.0/pyproject.toml` & `frequenz-client-microgrid-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 # License: MIT
 # Copyright © 2024 Frequenz Energy-as-a-Service GmbH
 
 [build-system]
-requires = [
-  "setuptools == 68.1.0",
-  "setuptools_scm[toml] == 7.1.0",
-  "frequenz-repo-config[lib] == 0.9.1",
-]
+requires = ["setuptools == 68.1.0", "setuptools_scm[toml] == 7.1.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frequenz-client-microgrid"
 description = "Microgrid API client for Python"
 readme = "README.md"
 license = { text = "MIT" }
@@ -32,19 +28,18 @@
   "Programming Language :: Python :: 3 :: Only",
   "Topic :: Internet",
   "Topic :: Software Development :: Libraries",
   "Typing :: Typed",
 ]
 requires-python = ">= 3.11, < 4"
 dependencies = [
-  "frequenz-api-microgrid >= 0.15.3, < 0.16.0",
+  "betterproto == 2.0.0b6",
   "frequenz-channels >= 1.0.0-rc1, < 2.0.0",
-  "frequenz-client-base >= 0.3.0, < 0.4.0",
-  "grpcio >= 1.54.2, < 2",
-  "protobuf >= 4.21.6, < 5",
+  "frequenz-client-base[grpclib] >= 0.4.0, < 0.5",
+  "frequenz-microgrid-betterproto >= 0.15.3.1, < 0.16",
   "timezonefinder >= 6.2.0, < 7",
   "typing-extensions >= 4.5.0, < 5",
 ]
 dynamic = ["version"]
 
 [[project.authors]]
 name = "Frequenz Energy-as-a-Service GmbH"
@@ -72,15 +67,15 @@
 ]
 dev-mypy = [
   "mypy == 1.8.0",
   "types-Markdown == 3.5.0.20240129",
   # For checking the noxfile, docs/ script, and tests
   "frequenz-client-microgrid[dev-mkdocs,dev-noxfile,dev-pytest]",
 ]
-dev-noxfile = ["nox == 2023.4.22", "frequenz-repo-config[lib] == 0.9.1"]
+dev-noxfile = ["nox == 2024.4.15", "frequenz-repo-config[lib] == 0.9.1"]
 dev-pylint = [
   "pylint == 3.1.0",
   # For checking the noxfile, docs/ script, and tests
   "frequenz-client-microgrid[dev-mkdocs,dev-noxfile,dev-pytest]",
 ]
 dev-pytest = [
   "pytest == 8.0.2",
```

### Comparing `frequenz-client-microgrid-0.3.0/src/frequenz/client/microgrid/_client.py` & `frequenz-client-microgrid-0.4.0/src/frequenz/client/microgrid/_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,27 @@
 # License: MIT
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 """Client for requests to the Microgrid API."""
 
 import asyncio
 import logging
-from collections.abc import Awaitable, Callable, Iterable
-from typing import Any, TypeVar, cast
+from collections.abc import Callable, Iterable, Set
+from typing import Any, TypeVar
 
-import grpc.aio
-
-# pylint: disable=no-name-in-module
-from frequenz.api.common.components_pb2 import ComponentCategory as PbComponentCategory
-from frequenz.api.common.metrics_pb2 import Bounds as PbBounds
-from frequenz.api.microgrid.microgrid_pb2 import ComponentData as PbComponentData
-from frequenz.api.microgrid.microgrid_pb2 import ComponentFilter as PbComponentFilter
-from frequenz.api.microgrid.microgrid_pb2 import ComponentIdParam as PbComponentIdParam
-from frequenz.api.microgrid.microgrid_pb2 import ComponentList as PbComponentList
-from frequenz.api.microgrid.microgrid_pb2 import ConnectionFilter as PbConnectionFilter
-from frequenz.api.microgrid.microgrid_pb2 import ConnectionList as PbConnectionList
-from frequenz.api.microgrid.microgrid_pb2 import (
-    MicrogridMetadata as PbMicrogridMetadata,
-)
-from frequenz.api.microgrid.microgrid_pb2 import SetBoundsParam as PbSetBoundsParam
-from frequenz.api.microgrid.microgrid_pb2 import (
-    SetPowerActiveParam as PbSetPowerActiveParam,
-)
-from frequenz.api.microgrid.microgrid_pb2_grpc import MicrogridStub
-
-# pylint: enable=no-name-in-module
+import grpclib
+import grpclib.client
+from betterproto.lib.google import protobuf as pb_google
 from frequenz.channels import Receiver
-from frequenz.client.base import retry, streaming
-from google.protobuf.empty_pb2 import Empty  # pylint: disable=no-name-in-module
+from frequenz.client.base import channel, retry, streaming
+from frequenz.microgrid.betterproto.frequenz.api import microgrid as pb_microgrid
+from frequenz.microgrid.betterproto.frequenz.api.common import (
+    components as pb_components,
+)
+from frequenz.microgrid.betterproto.frequenz.api.common import metrics as pb_metrics
 
 from ._component import (
     Component,
     ComponentCategory,
     component_category_from_protobuf,
     component_metadata_from_protobuf,
     component_type_from_protobuf,
@@ -45,91 +31,88 @@
     ComponentData,
     EVChargerData,
     InverterData,
     MeterData,
 )
 from ._connection import Connection
 from ._constants import RECEIVER_MAX_SIZE
+from ._exception import ClientError
 from ._metadata import Location, Metadata
 
 DEFAULT_GRPC_CALL_TIMEOUT = 60.0
 """The default timeout for gRPC calls made by this client (in seconds)."""
 
 _ComponentDataT = TypeVar("_ComponentDataT", bound=ComponentData)
 """Type variable resolving to any ComponentData sub-class."""
 
 _logger = logging.getLogger(__name__)
 
 
 class ApiClient:
-    """Microgrid API client implementation using gRPC as the underlying protocol."""
+    """A microgrid API client."""
 
     def __init__(
         self,
-        grpc_channel: grpc.aio.Channel,
-        target: str,
-        retry_strategy: retry.Strategy = retry.LinearBackoff(),
+        server_url: str,
+        *,
+        retry_strategy: retry.Strategy | None = None,
     ) -> None:
         """Initialize the class instance.
 
         Args:
-            grpc_channel: asyncio-supporting gRPC channel
-            target: server (host:port) to be used for asyncio-supporting gRPC
-                channel that the client should use to contact the API
+            server_url: The location of the microgrid API server in the form of a URL.
+                The following format is expected:
+                "grpc://hostname{:`port`}{?ssl=`ssl`}",
+                where the `port` should be an int between 0 and 65535 (defaulting to
+                9090) and `ssl` should be a boolean (defaulting to `false`).
+                For example: `grpc://localhost:1090?ssl=true`.
             retry_strategy: The retry strategy to use to reconnect when the connection
-                to the streaming method is lost.
+                to the streaming method is lost. By default a linear backoff strategy
+                is used.
         """
-        self.target = target
-        """The location (as "host:port") of the microgrid API gRPC server."""
+        self._server_url = server_url
+        """The location of the microgrid API server as a URL."""
 
-        self.api = MicrogridStub(grpc_channel)
+        self.api = pb_microgrid.MicrogridStub(channel.parse_grpc_uri(server_url))
         """The gRPC stub for the microgrid API."""
 
         self._broadcasters: dict[int, streaming.GrpcStreamBroadcaster[Any, Any]] = {}
         self._retry_strategy = retry_strategy
 
+    @property
+    def server_url(self) -> str:
+        """The server location in URL format."""
+        return self._server_url
+
     async def components(self) -> Iterable[Component]:
         """Fetch all the components present in the microgrid.
 
         Returns:
             Iterator whose elements are all the components in the microgrid.
 
         Raises:
-            AioRpcError: if connection to Microgrid API cannot be established or
-                when the api call exceeded timeout
+            ClientError: If the are any errors communicating with the Microgrid API,
+                most likely a subclass of
+                [GrpcError][frequenz.client.microgrid.GrpcError].
         """
         try:
-            # grpc.aio is missing types and mypy thinks this is not awaitable,
-            # but it is
-            component_list = await cast(
-                Awaitable[PbComponentList],
-                self.api.ListComponents(
-                    PbComponentFilter(),
-                    timeout=int(DEFAULT_GRPC_CALL_TIMEOUT),
-                ),
-            )
+            component_list = await self.api.list_components(
+                pb_microgrid.ComponentFilter(),
+                timeout=int(DEFAULT_GRPC_CALL_TIMEOUT),
+            )
+        except grpclib.GRPCError as grpc_error:
+            raise ClientError.from_grpc_error(
+                server_url=self._server_url,
+                operation="list_components",
+                grpc_error=grpc_error,
+            ) from grpc_error
 
-        except grpc.aio.AioRpcError as err:
-            msg = f"Failed to list components. Microgrid API: {self.target}. Err: {err.details()}"
-            raise grpc.aio.AioRpcError(
-                code=err.code(),
-                initial_metadata=err.initial_metadata(),
-                # We need to ignore these errors for some reason, otherwise we get this
-                # mypy error:
-                #   Argument "trailing_metadata" to "AioRpcError" has incompatible type
-                #   "tuple[_Metadatum, ...]"; expected "Metadata"
-                # According to grpc.aio documentation, both should have the type
-                # Metadata.
-                # https://grpc.github.io/grpc/python/grpc_asyncio.html#grpc.aio.AioRpcError
-                trailing_metadata=err.trailing_metadata(),  # type: ignore[arg-type]
-                details=msg,
-                debug_error_string=err.debug_error_string(),
-            )
         components_only = filter(
-            lambda c: c.category is not PbComponentCategory.COMPONENT_CATEGORY_SENSOR,
+            lambda c: c.category
+            is not pb_components.ComponentCategory.COMPONENT_CATEGORY_SENSOR,
             component_list.components,
         )
         result: Iterable[Component] = map(
             lambda c: Component(
                 c.id,
                 component_category_from_protobuf(c.category),
                 component_type_from_protobuf(c.category, c.inverter),
@@ -145,24 +128,21 @@
 
         If there is an error fetching the metadata, the microgrid ID and
         location will be set to None.
 
         Returns:
             the microgrid metadata.
         """
-        microgrid_metadata: PbMicrogridMetadata | None = None
+        microgrid_metadata: pb_microgrid.MicrogridMetadata | None = None
         try:
-            microgrid_metadata = await cast(
-                Awaitable[PbMicrogridMetadata],
-                self.api.GetMicrogridMetadata(
-                    Empty(),
-                    timeout=int(DEFAULT_GRPC_CALL_TIMEOUT),
-                ),
+            microgrid_metadata = await self.api.get_microgrid_metadata(
+                pb_google.Empty(),
+                timeout=int(DEFAULT_GRPC_CALL_TIMEOUT),
             )
-        except grpc.aio.AioRpcError:
+        except grpclib.GRPCError:
             _logger.exception("The microgrid metadata is not available.")
 
         if not microgrid_metadata:
             return Metadata()
 
         location: Location | None = None
         if microgrid_metadata.location:
@@ -171,56 +151,50 @@
                 longitude=microgrid_metadata.location.longitude,
             )
 
         return Metadata(microgrid_id=microgrid_metadata.microgrid_id, location=location)
 
     async def connections(
         self,
-        starts: set[int] | None = None,
-        ends: set[int] | None = None,
+        starts: Set[int] = frozenset(),
+        ends: Set[int] = frozenset(),
     ) -> Iterable[Connection]:
         """Fetch the connections between components in the microgrid.
 
         Args:
             starts: if set and non-empty, only include connections whose start
                 value matches one of the provided component IDs
             ends: if set and non-empty, only include connections whose end value
                 matches one of the provided component IDs
 
         Returns:
             Microgrid connections matching the provided start and end filters.
 
         Raises:
-            AioRpcError: if connection to Microgrid API cannot be established or
-                when the api call exceeded timeout
+            ClientError: If the are any errors communicating with the Microgrid API,
+                most likely a subclass of
+                [GrpcError][frequenz.client.microgrid.GrpcError].
         """
-        connection_filter = PbConnectionFilter(starts=starts, ends=ends)
+        connection_filter = pb_microgrid.ConnectionFilter(
+            starts=list(starts), ends=list(ends)
+        )
         try:
             valid_components, all_connections = await asyncio.gather(
                 self.components(),
-                # grpc.aio is missing types and mypy thinks this is not
-                # awaitable, but it is
-                cast(
-                    Awaitable[PbConnectionList],
-                    self.api.ListConnections(
-                        connection_filter,
-                        timeout=int(DEFAULT_GRPC_CALL_TIMEOUT),
-                    ),
+                self.api.list_connections(
+                    connection_filter,
+                    timeout=int(DEFAULT_GRPC_CALL_TIMEOUT),
                 ),
             )
-        except grpc.aio.AioRpcError as err:
-            msg = f"Failed to list connections. Microgrid API: {self.target}. Err: {err.details()}"
-            raise grpc.aio.AioRpcError(
-                code=err.code(),
-                initial_metadata=err.initial_metadata(),
-                # See the comment in def components() for why we need to ignore
-                trailing_metadata=err.trailing_metadata(),  # type: ignore[arg-type]
-                details=msg,
-                debug_error_string=err.debug_error_string(),
-            )
+        except grpclib.GRPCError as grpc_error:
+            raise ClientError.from_grpc_error(
+                server_url=self._server_url,
+                operation="list_connections",
+                grpc_error=grpc_error,
+            ) from grpc_error
         # Filter out the components filtered in `components` method.
         # id=0 is an exception indicating grid component.
         valid_ids = {c.component_id for c in valid_components}
         valid_ids.add(0)
 
         connections = filter(
             lambda c: (c.start in valid_ids and c.end in valid_ids),
@@ -234,15 +208,15 @@
         return result
 
     async def _new_component_data_receiver(
         self,
         *,
         component_id: int,
         expected_category: ComponentCategory,
-        transform: Callable[[PbComponentData], _ComponentDataT],
+        transform: Callable[[pb_microgrid.ComponentData], _ComponentDataT],
         maxsize: int,
     ) -> Receiver[_ComponentDataT]:
         """Return a new broadcaster receiver for a given `component_id`.
 
         If a broadcaster for the given `component_id` doesn't exist, it creates a new
         one.
 
@@ -257,28 +231,25 @@
             The new receiver for the given `component_id`.
         """
         await self._expect_category(
             component_id,
             expected_category,
         )
 
-        broadcaster = self._broadcasters.setdefault(
-            component_id,
-            streaming.GrpcStreamBroadcaster(
+        broadcaster = self._broadcasters.get(component_id)
+        if broadcaster is None:
+            broadcaster = streaming.GrpcStreamBroadcaster(
                 f"raw-component-data-{component_id}",
-                # We need to cast here because grpc says StreamComponentData is
-                # a grpc.CallIterator[PbComponentData], not a
-                # grpc.aio.UnaryStreamCall[..., PbComponentData].
-                lambda: cast(
-                    grpc.aio.UnaryStreamCall[Any, PbComponentData],
-                    self.api.StreamComponentData(PbComponentIdParam(id=component_id)),
+                lambda: self.api.stream_component_data(
+                    pb_microgrid.ComponentIdParam(id=component_id)
                 ),
                 transform,
-            ),
-        )
+                retry_strategy=self._retry_strategy,
+            )
+            self._broadcasters[component_id] = broadcaster
         return broadcaster.new_receiver(maxsize=maxsize)
 
     async def _expect_category(
         self,
         component_id: int,
         expected_category: ComponentCategory,
     ) -> None:
@@ -301,16 +272,16 @@
         except StopIteration as exc:
             raise ValueError(
                 f"Unable to find component with id {component_id}"
             ) from exc
 
         if comp.category != expected_category:
             raise ValueError(
-                f"Component id {component_id} is a {comp.category}"
-                f", not a {expected_category}."
+                f"Component id {component_id} is a {comp.category.name.lower()}"
+                f", not a {expected_category.name.lower()}."
             )
 
     async def meter_data(  # noqa: DOC502 (ValueError is raised indirectly by _expect_category)
         self,
         component_id: int,
         maxsize: int = RECEIVER_MAX_SIZE,
     ) -> Receiver[MeterData]:
@@ -414,72 +385,68 @@
 
 
         Args:
             component_id: id of the component to set power.
             power_w: power to set for the component.
 
         Raises:
-            AioRpcError: if connection to Microgrid API cannot be established or
-                when the api call exceeded timeout
+            ClientError: If the are any errors communicating with the Microgrid API,
+                most likely a subclass of
+                [GrpcError][frequenz.client.microgrid.GrpcError].
         """
         try:
-            await cast(
-                Awaitable[PbSetPowerActiveParam],
-                self.api.SetPowerActive(
-                    PbSetPowerActiveParam(component_id=component_id, power=power_w),
-                    timeout=int(DEFAULT_GRPC_CALL_TIMEOUT),
+            await self.api.set_power_active(
+                pb_microgrid.SetPowerActiveParam(
+                    component_id=component_id, power=power_w
                 ),
+                timeout=int(DEFAULT_GRPC_CALL_TIMEOUT),
             )
-        except grpc.aio.AioRpcError as err:
-            msg = f"Failed to set power. Microgrid API: {self.target}. Err: {err.details()}"
-            raise grpc.aio.AioRpcError(
-                code=err.code(),
-                initial_metadata=err.initial_metadata(),
-                # See the comment in def components() for why we need to ignore
-                trailing_metadata=err.trailing_metadata(),  # type: ignore[arg-type]
-                details=msg,
-                debug_error_string=err.debug_error_string(),
-            )
+        except grpclib.GRPCError as grpc_error:
+            raise ClientError.from_grpc_error(
+                server_url=self._server_url,
+                operation="set_power_active",
+                grpc_error=grpc_error,
+            ) from grpc_error
 
     async def set_bounds(
         self,
         component_id: int,
         lower: float,
         upper: float,
     ) -> None:
-        """Send `PbSetBoundsParam`s received from a channel to the Microgrid service.
+        """Send `SetBoundsParam`s received from a channel to the Microgrid service.
 
         Args:
             component_id: ID of the component to set bounds for.
             lower: Lower bound to be set for the component.
             upper: Upper bound to be set for the component.
 
         Raises:
             ValueError: when upper bound is less than 0, or when lower bound is
                 greater than 0.
-            grpc.aio.AioRpcError: if connection to Microgrid API cannot be established
-                or when the api call exceeded timeout
+            ClientError: If the are any errors communicating with the Microgrid API,
+                most likely a subclass of
+                [GrpcError][frequenz.client.microgrid.GrpcError].
         """
-        api_details = f"Microgrid API: {self.target}."
         if upper < 0:
             raise ValueError(f"Upper bound {upper} must be greater than or equal to 0.")
         if lower > 0:
-            raise ValueError(f"Lower bound {upper} must be less than or equal to 0.")
+            raise ValueError(f"Lower bound {lower} must be less than or equal to 0.")
 
-        target_metric = PbSetBoundsParam.TargetMetric.TARGET_METRIC_POWER_ACTIVE
+        target_metric = (
+            pb_microgrid.SetBoundsParamTargetMetric.TARGET_METRIC_POWER_ACTIVE
+        )
         try:
-            self.api.AddInclusionBounds(
-                PbSetBoundsParam(
+            await self.api.add_inclusion_bounds(
+                pb_microgrid.SetBoundsParam(
                     component_id=component_id,
                     target_metric=target_metric,
-                    bounds=PbBounds(lower=lower, upper=upper),
+                    bounds=pb_metrics.Bounds(lower=lower, upper=upper),
                 ),
+                timeout=int(DEFAULT_GRPC_CALL_TIMEOUT),
             )
-        except grpc.aio.AioRpcError as err:
-            _logger.error(
-                "set_bounds write failed: %s, for message: %s, api: %s. Err: %s",
-                err,
-                next,
-                api_details,
-                err.details(),
-            )
-            raise
+        except grpclib.GRPCError as grpc_error:
+            raise ClientError.from_grpc_error(
+                server_url=self._server_url,
+                operation="add_inclusion_bounds",
+                grpc_error=grpc_error,
+            ) from grpc_error
```

### Comparing `frequenz-client-microgrid-0.3.0/src/frequenz/client/microgrid/_component.py` & `frequenz-client-microgrid-0.4.0/src/frequenz/client/microgrid/_component.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,46 +2,41 @@
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 """Defines the components that can be used in a microgrid."""
 
 from dataclasses import dataclass
 from enum import Enum
 
-# pylint: disable=no-name-in-module
-from frequenz.api.common.components_pb2 import ComponentCategory as PbComponentCategory
-from frequenz.api.microgrid.grid_pb2 import Metadata as PbGridMetadata
-from frequenz.api.microgrid.inverter_pb2 import Metadata as PbInverterMetadata
-from frequenz.api.microgrid.inverter_pb2 import Type as PbInverterType
-
-# pylint: enable=no-name-in-module
+from frequenz.microgrid.betterproto.frequenz.api.common import components
+from frequenz.microgrid.betterproto.frequenz.api.microgrid import grid, inverter
 
 
 class ComponentType(Enum):
     """A base class from which individual component types are derived."""
 
 
 class InverterType(ComponentType):
     """Enum representing inverter types."""
 
-    NONE = PbInverterType.TYPE_UNSPECIFIED
+    NONE = inverter.Type.TYPE_UNSPECIFIED
     """Unspecified inverter type."""
 
-    BATTERY = PbInverterType.TYPE_BATTERY
+    BATTERY = inverter.Type.TYPE_BATTERY
     """Battery inverter."""
 
-    SOLAR = PbInverterType.TYPE_SOLAR
+    SOLAR = inverter.Type.TYPE_SOLAR
     """Solar inverter."""
 
-    HYBRID = PbInverterType.TYPE_HYBRID
+    HYBRID = inverter.Type.TYPE_HYBRID
     """Hybrid inverter."""
 
 
 def component_type_from_protobuf(
-    component_category: PbComponentCategory.ValueType,
-    component_metadata: PbInverterMetadata,
+    component_category: components.ComponentCategory,
+    component_metadata: inverter.Metadata,
 ) -> ComponentType | None:
     """Convert a protobuf InverterType message to Component enum.
 
     For internal-only use by the `microgrid` package.
 
     Args:
         component_category: category the type belongs to.
@@ -49,50 +44,50 @@
 
     Returns:
         Enum value corresponding to the protobuf message.
     """
     # ComponentType values in the protobuf definition are not unique across categories
     # as of v0.11.0, so we need to check the component category first, before doing any
     # component type checks.
-    if component_category == PbComponentCategory.COMPONENT_CATEGORY_INVERTER:
+    if component_category == components.ComponentCategory.COMPONENT_CATEGORY_INVERTER:
         if not any(int(t.value) == int(component_metadata.type) for t in InverterType):
             return None
 
         return InverterType(component_metadata.type)
 
     return None
 
 
 class ComponentCategory(Enum):
     """Possible types of microgrid component."""
 
-    NONE = PbComponentCategory.COMPONENT_CATEGORY_UNSPECIFIED
+    NONE = components.ComponentCategory.COMPONENT_CATEGORY_UNSPECIFIED
     """Unspecified component category."""
 
-    GRID = PbComponentCategory.COMPONENT_CATEGORY_GRID
+    GRID = components.ComponentCategory.COMPONENT_CATEGORY_GRID
     """Grid component."""
 
-    METER = PbComponentCategory.COMPONENT_CATEGORY_METER
+    METER = components.ComponentCategory.COMPONENT_CATEGORY_METER
     """Meter component."""
 
-    INVERTER = PbComponentCategory.COMPONENT_CATEGORY_INVERTER
+    INVERTER = components.ComponentCategory.COMPONENT_CATEGORY_INVERTER
     """Inverter component."""
 
-    BATTERY = PbComponentCategory.COMPONENT_CATEGORY_BATTERY
+    BATTERY = components.ComponentCategory.COMPONENT_CATEGORY_BATTERY
     """Battery component."""
 
-    EV_CHARGER = PbComponentCategory.COMPONENT_CATEGORY_EV_CHARGER
+    EV_CHARGER = components.ComponentCategory.COMPONENT_CATEGORY_EV_CHARGER
     """EV charger component."""
 
-    CHP = PbComponentCategory.COMPONENT_CATEGORY_CHP
+    CHP = components.ComponentCategory.COMPONENT_CATEGORY_CHP
     """CHP component."""
 
 
 def component_category_from_protobuf(
-    component_category: PbComponentCategory.ValueType,
+    component_category: components.ComponentCategory,
 ) -> ComponentCategory:
     """Convert a protobuf ComponentCategory message to ComponentCategory enum.
 
     For internal-only use by the `microgrid` package.
 
     Args:
         component_category: protobuf enum to convert
@@ -101,15 +96,15 @@
         Enum value corresponding to the protobuf message.
 
     Raises:
         ValueError: if `component_category` is a sensor (this is not considered
             a valid component category as it does not form part of the
             microgrid itself)
     """
-    if component_category == PbComponentCategory.COMPONENT_CATEGORY_SENSOR:
+    if component_category == components.ComponentCategory.COMPONENT_CATEGORY_SENSOR:
         raise ValueError("Cannot create a component from a sensor!")
 
     if not any(t.value == component_category for t in ComponentCategory):
         return ComponentCategory.NONE
 
     return ComponentCategory(component_category)
 
@@ -132,29 +127,29 @@
 
 @dataclass(frozen=True)
 class GridMetadata(ComponentMetadata):
     """Metadata for a grid connection point."""
 
 
 def component_metadata_from_protobuf(
-    component_category: PbComponentCategory.ValueType,
-    component_metadata: PbGridMetadata,
+    component_category: components.ComponentCategory,
+    component_metadata: grid.Metadata,
 ) -> GridMetadata | None:
     """Convert a protobuf GridMetadata message to GridMetadata class.
 
     For internal-only use by the `microgrid` package.
 
     Args:
         component_category: category the type belongs to.
         component_metadata: protobuf metadata to fetch type from.
 
     Returns:
         GridMetadata instance corresponding to the protobuf message.
     """
-    if component_category == PbComponentCategory.COMPONENT_CATEGORY_GRID:
+    if component_category == components.ComponentCategory.COMPONENT_CATEGORY_GRID:
         max_current = component_metadata.rated_fuse_current
         fuse = Fuse(max_current)
         return GridMetadata(fuse)
 
     return None
```

### Comparing `frequenz-client-microgrid-0.3.0/src/frequenz/client/microgrid/_component_data.py` & `frequenz-client-microgrid-0.4.0/src/frequenz/client/microgrid/_component_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 # License: MIT
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 """Component data types for data coming from a microgrid."""
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
-from datetime import datetime, timezone
+from datetime import datetime
 from typing import Self
 
-# pylint: disable=no-name-in-module
-from frequenz.api.microgrid.battery_pb2 import ComponentState as PbBatteryComponentState
-from frequenz.api.microgrid.battery_pb2 import Error as PbBatteryError
-from frequenz.api.microgrid.battery_pb2 import RelayState as PbBatteryRelayState
-from frequenz.api.microgrid.inverter_pb2 import (
-    ComponentState as PbInverterComponentState,
-)
-from frequenz.api.microgrid.inverter_pb2 import Error as PbInverterError
-from frequenz.api.microgrid.microgrid_pb2 import ComponentData as PbComponentData
+from frequenz.microgrid.betterproto.frequenz.api import microgrid
 
-# pylint: enable=no-name-in-module
-from ._component_states import EVChargerCableState, EVChargerComponentState
+from ._component_error import BatteryError, InverterError
+from ._component_states import (
+    BatteryComponentState,
+    BatteryRelayState,
+    EVChargerCableState,
+    EVChargerComponentState,
+    InverterComponentState,
+)
 
 
 @dataclass(frozen=True)
 class ComponentData(ABC):
     """A private base class for strongly typed component data classes."""
 
     component_id: int
@@ -33,32 +31,32 @@
     """The timestamp of when the data was measured."""
 
     # The `raw` attribute is excluded from the constructor as it can only be provided
     # when instantiating `ComponentData` using the `from_proto` method, which reads
     # data from a protobuf message. The whole protobuf message is stored as the `raw`
     # attribute. When `ComponentData` is not instantiated from a protobuf message,
     # i.e. using the constructor, `raw` will be set to `None`.
-    raw: PbComponentData | None = field(default=None, init=False)
+    raw: microgrid.ComponentData | None = field(default=None, init=False)
     """Raw component data as decoded from the wire."""
 
-    def _set_raw(self, raw: PbComponentData) -> None:
+    def _set_raw(self, raw: microgrid.ComponentData) -> None:
         """Store raw protobuf message.
 
         It is preferred to keep the dataclasses immutable (frozen) and make the `raw`
             attribute read-only, which is why the approach of writing to `__dict__`
             was used, instead of mutating the `self.raw = raw` attribute directly.
 
         Args:
             raw: raw component data as decoded from the wire.
         """
         self.__dict__["raw"] = raw
 
     @classmethod
     @abstractmethod
-    def from_proto(cls, raw: PbComponentData) -> Self:
+    def from_proto(cls, raw: microgrid.ComponentData) -> Self:
         """Create ComponentData from a protobuf message.
 
         Args:
             raw: raw component data as decoded from the wire.
 
         Returns:
             The instance created from the protobuf message.
@@ -117,26 +115,26 @@
         1,2 and 3 respectively.
     """
 
     frequency: float
     """The AC power frequency in Hertz (Hz)."""
 
     @classmethod
-    def from_proto(cls, raw: PbComponentData) -> Self:
+    def from_proto(cls, raw: microgrid.ComponentData) -> Self:
         """Create MeterData from a protobuf message.
 
         Args:
             raw: raw component data as decoded from the wire.
 
         Returns:
             Instance of MeterData created from the protobuf message.
         """
         meter_data = cls(
             component_id=raw.id,
-            timestamp=raw.ts.ToDatetime(tzinfo=timezone.utc),
+            timestamp=raw.ts,
             active_power=raw.meter.data.ac.power_active.value,
             active_power_per_phase=(
                 raw.meter.data.ac.phase_1.power_active.value,
                 raw.meter.data.ac.phase_2.power_active.value,
                 raw.meter.data.ac.phase_3.power_active.value,
             ),
             reactive_power=raw.meter.data.ac.power_reactive.value,
@@ -177,15 +175,14 @@
     """The SoC above which charge commands will be blocked by the system,
         in percent (%).
     """
 
     capacity: float
     """The capacity of the battery in Wh (Watt-hour)."""
 
-    # pylint: disable=line-too-long
     power_inclusion_lower_bound: float
     """Lower inclusion bound for battery power in watts.
 
     This is the lower limit of the range within which power requests are allowed for the
     battery.
 
     See [`frequenz.api.common.metrics_pb2.Metric.system_inclusion_bounds`][] and
@@ -221,54 +218,55 @@
     This is the upper limit of the range within which power requests are not allowed for
     the battery.
 
     See [`frequenz.api.common.metrics_pb2.Metric.system_inclusion_bounds`][] and
     [`frequenz.api.common.metrics_pb2.Metric.system_exclusion_bounds`][] for more
     details.
     """
-    # pylint: enable=line-too-long
 
     temperature: float
     """The (average) temperature reported by the battery, in Celsius (°C)."""
 
-    _relay_state: PbBatteryRelayState.ValueType
+    relay_state: BatteryRelayState
     """State of the battery relay."""
 
-    _component_state: PbBatteryComponentState.ValueType
+    component_state: BatteryComponentState
     """State of the battery."""
 
-    _errors: list[PbBatteryError]
+    errors: list[BatteryError]
     """List of errors in protobuf struct."""
 
     @classmethod
-    def from_proto(cls, raw: PbComponentData) -> Self:
+    def from_proto(cls, raw: microgrid.ComponentData) -> Self:
         """Create BatteryData from a protobuf message.
 
         Args:
             raw: raw component data as decoded from the wire.
 
         Returns:
             Instance of BatteryData created from the protobuf message.
         """
         raw_power = raw.battery.data.dc.power
         battery_data = cls(
             component_id=raw.id,
-            timestamp=raw.ts.ToDatetime(tzinfo=timezone.utc),
+            timestamp=raw.ts,
             soc=raw.battery.data.soc.avg,
             soc_lower_bound=raw.battery.data.soc.system_inclusion_bounds.lower,
             soc_upper_bound=raw.battery.data.soc.system_inclusion_bounds.upper,
             capacity=raw.battery.properties.capacity,
             power_inclusion_lower_bound=raw_power.system_inclusion_bounds.lower,
             power_exclusion_lower_bound=raw_power.system_exclusion_bounds.lower,
             power_inclusion_upper_bound=raw_power.system_inclusion_bounds.upper,
             power_exclusion_upper_bound=raw_power.system_exclusion_bounds.upper,
             temperature=raw.battery.data.temperature.avg,
-            _relay_state=raw.battery.state.relay_state,
-            _component_state=raw.battery.state.component_state,
-            _errors=list(raw.battery.errors),
+            relay_state=BatteryRelayState.from_pb(raw.battery.state.relay_state),
+            component_state=BatteryComponentState.from_pb(
+                raw.battery.state.component_state
+            ),
+            errors=[BatteryError.from_pb(e) for e in raw.battery.errors],
         )
         battery_data._set_raw(raw=raw)
         return battery_data
 
 
 @dataclass(frozen=True)
 class InverterData(ComponentData):  # pylint: disable=too-many-instance-attributes
@@ -318,15 +316,14 @@
     """
 
     voltage_per_phase: tuple[float, float, float]
     """The AC voltage in Volts (V) between the line and the neutral wire for
        phase/line 1, 2 and 3 respectively.
     """
 
-    # pylint: disable=line-too-long
     active_power_inclusion_lower_bound: float
     """Lower inclusion bound for inverter power in watts.
 
     This is the lower limit of the range within which power requests are allowed for the
     inverter.
 
     See [`frequenz.api.common.metrics_pb2.Metric.system_inclusion_bounds`][] and
@@ -362,39 +359,38 @@
     This is the upper limit of the range within which power requests are not allowed for
     the inverter.
 
     See [`frequenz.api.common.metrics_pb2.Metric.system_inclusion_bounds`][] and
     [`frequenz.api.common.metrics_pb2.Metric.system_exclusion_bounds`][] for more
     details.
     """
-    # pylint: enable=line-too-long
 
     frequency: float
     """AC frequency, in Hertz (Hz)."""
 
-    _component_state: PbInverterComponentState.ValueType
+    component_state: InverterComponentState
     """State of the inverter."""
 
-    _errors: list[PbInverterError]
+    errors: list[InverterError]
     """List of errors from the component."""
 
     @classmethod
-    def from_proto(cls, raw: PbComponentData) -> Self:
+    def from_proto(cls, raw: microgrid.ComponentData) -> Self:
         """Create InverterData from a protobuf message.
 
         Args:
             raw: raw component data as decoded from the wire.
 
         Returns:
             Instance of InverterData created from the protobuf message.
         """
         raw_power = raw.inverter.data.ac.power_active
         inverter_data = cls(
             component_id=raw.id,
-            timestamp=raw.ts.ToDatetime(tzinfo=timezone.utc),
+            timestamp=raw.ts,
             active_power=raw.inverter.data.ac.power_active.value,
             active_power_per_phase=(
                 raw.inverter.data.ac.phase_1.power_active.value,
                 raw.inverter.data.ac.phase_2.power_active.value,
                 raw.inverter.data.ac.phase_3.power_active.value,
             ),
             reactive_power=raw.inverter.data.ac.power_reactive.value,
@@ -414,16 +410,18 @@
                 raw.inverter.data.ac.phase_3.voltage.value,
             ),
             active_power_inclusion_lower_bound=raw_power.system_inclusion_bounds.lower,
             active_power_exclusion_lower_bound=raw_power.system_exclusion_bounds.lower,
             active_power_inclusion_upper_bound=raw_power.system_inclusion_bounds.upper,
             active_power_exclusion_upper_bound=raw_power.system_exclusion_bounds.upper,
             frequency=raw.inverter.data.ac.frequency.value,
-            _component_state=raw.inverter.state.component_state,
-            _errors=list(raw.inverter.errors),
+            component_state=InverterComponentState.from_pb(
+                raw.inverter.state.component_state
+            ),
+            errors=[InverterError.from_pb(e) for e in raw.inverter.errors],
         )
 
         inverter_data._set_raw(raw=raw)
         return inverter_data
 
 
 @dataclass(frozen=True)
@@ -528,27 +526,27 @@
     cable_state: EVChargerCableState
     """The state of the ev charger's cable."""
 
     component_state: EVChargerComponentState
     """The state of the ev charger."""
 
     @classmethod
-    def from_proto(cls, raw: PbComponentData) -> Self:
+    def from_proto(cls, raw: microgrid.ComponentData) -> Self:
         """Create EVChargerData from a protobuf message.
 
         Args:
             raw: raw component data as decoded from the wire.
 
         Returns:
             Instance of EVChargerData created from the protobuf message.
         """
         raw_power = raw.ev_charger.data.ac.power_active
         ev_charger_data = cls(
             component_id=raw.id,
-            timestamp=raw.ts.ToDatetime(tzinfo=timezone.utc),
+            timestamp=raw.ts,
             active_power=raw_power.value,
             active_power_per_phase=(
                 raw.ev_charger.data.ac.phase_1.power_active.value,
                 raw.ev_charger.data.ac.phase_2.power_active.value,
                 raw.ev_charger.data.ac.phase_3.power_active.value,
             ),
             reactive_power=raw.ev_charger.data.ac.power_reactive.value,
```

### Comparing `frequenz-client-microgrid-0.3.0/src/frequenz/client/microgrid/_connection.py` & `frequenz-client-microgrid-0.4.0/src/frequenz/client/microgrid/_connection.py`

 * *Files identical despite different names*

### Comparing `frequenz-client-microgrid-0.3.0/src/frequenz/client/microgrid/_constants.py` & `frequenz-client-microgrid-0.4.0/src/frequenz/client/microgrid/_constants.py`

 * *Files identical despite different names*

### Comparing `frequenz-client-microgrid-0.3.0/src/frequenz/client/microgrid/_metadata.py` & `frequenz-client-microgrid-0.4.0/src/frequenz/client/microgrid/_metadata.py`

 * *Files identical despite different names*

### Comparing `frequenz-client-microgrid-0.3.0/src/frequenz_client_microgrid.egg-info/PKG-INFO` & `frequenz-client-microgrid-0.4.0/src/frequenz_client_microgrid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-client-microgrid
-Version: 0.3.0
+Version: 0.4.0
 Summary: Microgrid API client for Python
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Documentation, https://frequenz-floss.github.io/frequenz-client-microgrid-python/
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-client-microgrid-python/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-client-microgrid-python/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-client-microgrid-python
```

### Comparing `frequenz-client-microgrid-0.3.0/src/frequenz_client_microgrid.egg-info/SOURCES.txt` & `frequenz-client-microgrid-0.4.0/src/frequenz_client_microgrid.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 README.md
 RELEASE_NOTES.md
 pyproject.toml
 src/frequenz/client/microgrid/__init__.py
 src/frequenz/client/microgrid/_client.py
 src/frequenz/client/microgrid/_component.py
 src/frequenz/client/microgrid/_component_data.py
+src/frequenz/client/microgrid/_component_error.py
 src/frequenz/client/microgrid/_component_states.py
 src/frequenz/client/microgrid/_connection.py
 src/frequenz/client/microgrid/_constants.py
+src/frequenz/client/microgrid/_exception.py
 src/frequenz/client/microgrid/_metadata.py
 src/frequenz/client/microgrid/conftest.py
 src/frequenz/client/microgrid/py.typed
 src/frequenz_client_microgrid.egg-info/PKG-INFO
 src/frequenz_client_microgrid.egg-info/SOURCES.txt
 src/frequenz_client_microgrid.egg-info/dependency_links.txt
 src/frequenz_client_microgrid.egg-info/requires.txt
```

### Comparing `frequenz-client-microgrid-0.3.0/src/frequenz_client_microgrid.egg-info/requires.txt` & `frequenz-client-microgrid-0.4.0/src/frequenz_client_microgrid.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-frequenz-api-microgrid<0.16.0,>=0.15.3
+betterproto==2.0.0b6
 frequenz-channels<2.0.0,>=1.0.0-rc1
-frequenz-client-base<0.4.0,>=0.3.0
-grpcio<2,>=1.54.2
-protobuf<5,>=4.21.6
+frequenz-client-base[grpclib]<0.5,>=0.4.0
+frequenz-microgrid-betterproto<0.16,>=0.15.3.1
 timezonefinder<7,>=6.2.0
 typing-extensions<5,>=4.5.0
 
 [dev]
 frequenz-client-microgrid[dev-flake8,dev-formatting,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]
 
 [dev-flake8]
@@ -33,15 +32,15 @@
 
 [dev-mypy]
 mypy==1.8.0
 types-Markdown==3.5.0.20240129
 frequenz-client-microgrid[dev-mkdocs,dev-noxfile,dev-pytest]
 
 [dev-noxfile]
-nox==2023.4.22
+nox==2024.4.15
 frequenz-repo-config[lib]==0.9.1
 
 [dev-pylint]
 pylint==3.1.0
 frequenz-client-microgrid[dev-mkdocs,dev-noxfile,dev-pytest]
 
 [dev-pytest]
```

