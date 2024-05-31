# Comparing `tmp/reka_api-2.0.0.tar.gz` & `tmp/reka_api-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reka_api-2.0.0.tar", max compression
+gzip compressed data, was "reka_api-3.0.5.tar", max compression
```

## Comparing `reka_api-2.0.0.tar` & `reka_api-3.0.5.tar`

### file list

```diff
@@ -1,14 +1,58 @@
--rw-r--r--   0        0        0    25738 2024-04-25 14:11:13.751171 reka_api-2.0.0/LICENSE
--rw-r--r--   0        0        0      149 2024-04-25 14:11:13.751171 reka_api-2.0.0/README.md
--rw-r--r--   0        0        0     1125 2024-04-25 14:11:13.751171 reka_api-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      764 2024-04-25 14:11:13.751171 reka_api-2.0.0/src/reka/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 14:11:13.751171 reka_api-2.0.0/src/reka/api/__init__.py
--rw-r--r--   0        0        0     7483 2024-04-25 14:11:13.751171 reka_api-2.0.0/src/reka/api/chat.py
--rw-r--r--   0        0        0     2077 2024-04-25 14:11:13.751171 reka_api-2.0.0/src/reka/api/dataset.py
--rw-r--r--   0        0        0     2223 2024-04-25 14:11:13.751171 reka_api-2.0.0/src/reka/api/driver.py
--rw-r--r--   0        0        0      694 2024-04-25 14:11:13.751171 reka_api-2.0.0/src/reka/api/job.py
--rw-r--r--   0        0        0      373 2024-04-25 14:11:13.751171 reka_api-2.0.0/src/reka/api/models.py
--rw-r--r--   0        0        0     3563 2024-04-25 14:11:13.751171 reka_api-2.0.0/src/reka/api/retrieval.py
--rw-r--r--   0        0        0     1136 2024-04-25 14:11:13.751171 reka_api-2.0.0/src/reka/errors.py
--rw-r--r--   0        0        0        0 2024-04-25 14:11:13.751171 reka_api-2.0.0/src/reka/py.typed
--rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 reka_api-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1057 2024-05-31 17:32:53.504624 reka_api-3.0.5/LICENSE
+-rw-r--r--   0        0        0     5577 2024-05-31 17:32:53.504624 reka_api-3.0.5/README.md
+-rw-r--r--   0        0        0     1649 2024-05-31 17:32:53.504624 reka_api-3.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1231 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/__init__.py
+-rw-r--r--   0        0        0       65 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/chat/__init__.py
+-rw-r--r--   0        0        0    27684 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/chat/client.py
+-rw-r--r--   0        0        0     5361 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/client.py
+-rw-r--r--   0        0        0     1126 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/core/api_error.py
+-rw-r--r--   0        0        0     1483 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      748 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/core/pydantic_utilities.py
+-rw-r--r--   0        0        0     1266 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/core/query_encoder.py
+-rw-r--r--   0        0        0      330 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/core/request_options.py
+-rw-r--r--   0        0        0     8148 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/core/unchecked_base_model.py
+-rw-r--r--   0        0        0      152 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/environment.py
+-rw-r--r--   0        0        0      170 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0       65 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/models/__init__.py
+-rw-r--r--   0        0        0     5028 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/models/client.py
+-rw-r--r--   0        0        0        0 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/py.typed
+-rw-r--r--   0        0        0     1476 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/__init__.py
+-rw-r--r--   0        0        0     1338 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/chat_message.py
+-rw-r--r--   0        0        0     1387 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/chat_message_chunk.py
+-rw-r--r--   0        0        0      239 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/chat_message_chunk_content_item.py
+-rw-r--r--   0        0        0      239 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/chat_message_input_content_item.py
+-rw-r--r--   0        0        0      240 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/chat_message_output_content_item.py
+-rw-r--r--   0        0        0     1351 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/chat_response.py
+-rw-r--r--   0        0        0      153 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/chat_role.py
+-rw-r--r--   0        0        0     1400 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/chunk_chat_response.py
+-rw-r--r--   0        0        0     1388 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/chunk_message_response.py
+-rw-r--r--   0        0        0      224 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/content.py
+-rw-r--r--   0        0        0      165 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/finish_reason.py
+-rw-r--r--   0        0        0     1272 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/http_validation_error.py
+-rw-r--r--   0        0        0      183 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/media_type.py
+-rw-r--r--   0        0        0     1373 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/message_response.py
+-rw-r--r--   0        0        0     1348 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/model.py
+-rw-r--r--   0        0        0     1572 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/typed_media_content.py
+-rw-r--r--   0        0        0     1530 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/typed_text.py
+-rw-r--r--   0        0        0     1267 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/usage.py
+-rw-r--r--   0        0        0     1291 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0      776 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/v2/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/v2/api/__init__.py
+-rw-r--r--   0        0        0     7489 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/v2/api/chat.py
+-rw-r--r--   0        0        0     2084 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/v2/api/dataset.py
+-rw-r--r--   0        0        0     2248 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/v2/api/driver.py
+-rw-r--r--   0        0        0      698 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/v2/api/job.py
+-rw-r--r--   0        0        0      376 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/v2/api/models.py
+-rw-r--r--   0        0        0     3573 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/v2/api/retrieval.py
+-rw-r--r--   0        0        0     1128 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/v2/errors.py
+-rw-r--r--   0        0        0        0 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/v2/py.typed
+-rw-r--r--   0        0        0       76 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/version.py
+-rw-r--r--   0        0        0     6817 1970-01-01 00:00:00.000000 reka_api-3.0.5/PKG-INFO
```

### Comparing `reka_api-2.0.0/src/reka/__init__.py` & `reka_api-3.0.5/src/reka/v2/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 # Grab it from an environment variable by default, but can be overriden
 API_KEY = os.getenv("REKA_API_KEY")
 # Default production server
 _SERVER = os.getenv("REKA_SERVER", "https://api.reka.ai")
 
 __version__ = importlib.metadata.version("reka-api")
-from reka.api.chat import chat
-from reka.api.dataset import add_dataset, delete_dataset, list_datasets
-from reka.api.models import list_models
-from reka.api.retrieval import (
+from reka.v2.api.chat import chat
+from reka.v2.api.dataset import add_dataset, delete_dataset, list_datasets
+from reka.v2.api.models import list_models
+from reka.v2.api.retrieval import (
     PrepareRetrievalStatusResponse,
     prepare_retrieval,
     retrieval_job_status,
 )
 
 __all__ = [
     "chat",
```

### Comparing `reka_api-2.0.0/src/reka/api/chat.py` & `reka_api-3.0.5/src/reka/v2/api/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Chat-related server interactions (including VLM chat)"""
 
 from __future__ import annotations
 
 import base64
 from typing import Any, Dict, List, Literal, Optional, TypedDict, cast
 
-import reka.api.driver as driver
-from reka.errors import InvalidConversationError
+import reka.v2.api.driver as driver
+from reka.v2.errors import InvalidConversationError
 
 
 class ModelTurn(TypedDict):
     """A turn in a conversation output by the model."""
 
     type: Literal["model"]
     text: str
```

### Comparing `reka_api-2.0.0/src/reka/api/dataset.py` & `reka_api-3.0.5/src/reka/v2/api/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Dataset-related server interactions."""
+
 from typing import Any, Dict, List, Optional, cast
 
 from requests.exceptions import HTTPError
 
-import reka.api.driver as driver
-from reka.errors import DatasetError
+import reka.v2.api.driver as driver
+from reka.v2.errors import DatasetError
 
 
 def list_datasets() -> List[str]:
     """List all datasets available to the user of the `API_KEY`.
 
     Returns:
        List of dataset names.
```

### Comparing `reka_api-2.0.0/src/reka/api/driver.py` & `reka_api-3.0.5/src/reka/v2/api/driver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 """Wrapper around requests, handling authentication, reka server, and exceptions."""
+
 import json
 import logging
 from typing import Any, Dict, Optional, cast
 
 import requests
 
-import reka
-from reka.errors import AuthError
+import reka.v2 as rekav2
+from reka.v2.errors import AuthError
 
 
 def make_request(
     method: str,
     endpoint: str,
     headers: Optional[Dict[str, str]] = None,
     data: Optional[Dict[str, Optional[str]]] = None,
     json: Any = None,
     files: Any = None,
 ) -> Dict[str, Any]:
     """Wrapper around requests, handling authentication, reka server, and exceptions."""
     headers = headers or {}
-    if reka.API_KEY is None:
+    if rekav2.API_KEY is None:
         raise AuthError(
-            reason='Reka API key not set. Set in code with `reka.API_KEY = "your-key"`, '
+            reason='Reka API key not set. Set in code with `rekav2.API_KEY = "your-key"`, '
             'or using the environment variable `export REKA_API_KEY="your-key"`.'
         )
 
-    headers["X-Api-Key"] = reka.API_KEY
+    headers["X-Api-Key"] = rekav2.API_KEY
 
     try:
         response = requests.request(
             method=method,
-            url=f"{reka._SERVER}/{endpoint}",
+            url=f"{rekav2._SERVER}/{endpoint}",
             headers=headers,
             data=data,
             files=files,
             json=json,
         )
         logging.debug(f"Received response {response.text}.")
         response.raise_for_status()
```

### Comparing `reka_api-2.0.0/src/reka/api/job.py` & `reka_api-3.0.5/src/reka/v2/api/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Job-related server interactions, i.e. retrieval, finetuning."""
+
 from enum import Enum
 from typing import Any, Dict
 
-import reka.api.driver as driver
+import reka.v2.api.driver as driver
 
 
 class JobStatus(Enum):
     PENDING = "PENDING"
     RUNNING = "RUNNING"
     ERROR = "ERROR"
     COMPLETE = "COMPLETE"
```

### Comparing `reka_api-2.0.0/src/reka/api/retrieval.py` & `reka_api-3.0.5/src/reka/v2/api/retrieval.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Retrieval-related server interactions, i.e. retrieval, finetuning."""
+
 from __future__ import annotations
 
 import dataclasses
 from typing import Any, Dict, List, cast
 
 from requests.exceptions import HTTPError
 
-import reka.api.driver as driver
-import reka.api.job as job
-from reka.errors import RetrievalError
+import reka.v2.api.driver as driver
+import reka.v2.api.job as job
+from reka.v2.errors import RetrievalError
 
 
 @dataclasses.dataclass
 class PrepareRetrievalStatusResponse:
     """Status of a `prepare-retrieval` job.
 
     Args:
```

### Comparing `reka_api-2.0.0/src/reka/errors.py` & `reka_api-3.0.5/src/reka/v2/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,13 +39,11 @@
 
 class RetrievalError(RekaError):
     """Something wrong with retrieval"""
 
     ...
 
 
-class AuthError(RekaError, ValueError):
-    ...
+class AuthError(RekaError, ValueError): ...
 
 
-class InvalidConversationError(RekaError):
-    ...
+class InvalidConversationError(RekaError): ...
```

