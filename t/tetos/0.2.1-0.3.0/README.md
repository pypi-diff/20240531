# Comparing `tmp/tetos-0.2.1.tar.gz` & `tmp/tetos-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tetos-0.2.1.tar", last modified: Tue Apr 23 03:38:30 2024, max compression
+gzip compressed data, was "tetos-0.3.0.tar", last modified: Fri May 31 08:45:34 2024, max compression
```

## Comparing `tetos-0.2.1.tar` & `tetos-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      551 2024-04-23 03:38:27.538346 tetos-0.2.1/LICENSE
--rw-r--r--   0        0        0     3277 2024-04-23 03:38:27.538346 tetos-0.2.1/README.md
--rw-r--r--   0        0        0     1777 2024-04-23 03:38:30.490347 tetos-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1062 2024-04-23 03:38:27.538346 tetos-0.2.1/src/tetos/__init__.py
--rw-r--r--   0        0        0      664 2024-04-23 03:38:27.538346 tetos-0.2.1/src/tetos/__main__.py
--rw-r--r--   0        0        0     3776 2024-04-23 03:38:27.538346 tetos-0.2.1/src/tetos/azure.py
--rw-r--r--   0        0        0     5210 2024-04-23 03:38:27.538346 tetos-0.2.1/src/tetos/baidu.py
--rw-r--r--   0        0        0     3161 2024-04-23 03:38:27.538346 tetos-0.2.1/src/tetos/base.py
--rw-r--r--   0        0        0    26479 2024-04-23 03:38:27.538346 tetos-0.2.1/src/tetos/consts.py
--rw-r--r--   0        0        0     2471 2024-04-23 03:38:27.538346 tetos-0.2.1/src/tetos/edge.py
--rw-r--r--   0        0        0     4891 2024-04-23 03:38:27.538346 tetos-0.2.1/src/tetos/google.py
--rw-r--r--   0        0        0     4457 2024-04-23 03:38:27.538346 tetos-0.2.1/src/tetos/minimax.py
--rw-r--r--   0        0        0     2770 2024-04-23 03:38:27.538346 tetos-0.2.1/src/tetos/openai.py
--rw-r--r--   0        0        0     9090 2024-04-23 03:38:27.538346 tetos-0.2.1/src/tetos/volc.py
--rw-r--r--   0        0        0     1934 2024-04-23 03:38:27.538346 tetos-0.2.1/tests/test_speakers.py
--rw-r--r--   0        0        0     4402 1970-01-01 00:00:00.000000 tetos-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      551 2024-04-17 03:19:05.344967 tetos-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5280 2024-05-31 03:22:21.023117 tetos-0.3.0/README.md
+-rw-r--r--   0        0        0     1801 2024-05-31 08:45:34.617595 tetos-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1115 2024-05-31 03:08:09.195180 tetos-0.3.0/src/tetos/__init__.py
+-rw-r--r--   0        0        0      664 2024-04-23 03:31:20.584312 tetos-0.3.0/src/tetos/__main__.py
+-rw-r--r--   0        0        0     3776 2024-04-22 08:05:48.167145 tetos-0.3.0/src/tetos/azure.py
+-rw-r--r--   0        0        0     5210 2024-04-19 04:11:26.252158 tetos-0.3.0/src/tetos/baidu.py
+-rw-r--r--   0        0        0     3322 2024-05-31 02:43:07.636265 tetos-0.3.0/src/tetos/base.py
+-rw-r--r--   0        0        0    26479 2024-04-23 01:53:56.265418 tetos-0.3.0/src/tetos/consts.py
+-rw-r--r--   0        0        0     2471 2024-04-22 08:05:48.169802 tetos-0.3.0/src/tetos/edge.py
+-rw-r--r--   0        0        0     4891 2024-04-18 01:07:15.396936 tetos-0.3.0/src/tetos/google.py
+-rw-r--r--   0        0        0     4457 2024-04-23 02:20:51.251633 tetos-0.3.0/src/tetos/minimax.py
+-rw-r--r--   0        0        0     2770 2024-04-18 00:38:06.458907 tetos-0.3.0/src/tetos/openai.py
+-rw-r--r--   0        0        0     8927 2024-05-31 02:43:17.448543 tetos-0.3.0/src/tetos/volc.py
+-rw-r--r--   0        0        0     5695 2024-05-31 03:17:48.901302 tetos-0.3.0/src/tetos/xunfei.py
+-rw-r--r--   0        0        0     2376 2024-05-31 03:09:28.541433 tetos-0.3.0/tests/test_speakers.py
+-rw-r--r--   0        0        0     6437 1970-01-01 00:00:00.000000 tetos-0.3.0/PKG-INFO
```

### Comparing `tetos-0.2.1/LICENSE` & `tetos-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tetos-0.2.1/pyproject.toml` & `tetos-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     "edge-tts>=6.1.10",
     "openai>=1.20.0",
     "mutagen>=1.47.0",
     "azure-cognitiveservices-speech>=1.37.0",
     "anyio>=4.3.0",
     "click>=8.1.7",
     "google-cloud-texttospeech>=2.16.3",
+    "websockets>=12.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 dynamic = []
 keywords = [
     "tts",
     "text-to-speech",
@@ -31,15 +32,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
-version = "0.2.1"
+version = "0.3.0"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.urls]
 Repository = "https://github.com/frostming/tetos"
 Documentation = "https://tetos.readthedocs.io/latest/"
```

### Comparing `tetos-0.2.1/src/tetos/__init__.py` & `tetos-0.3.0/src/tetos/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 from .baidu import BaiduSpeaker
 from .base import Speaker
 from .edge import EdgeSpeaker
 from .google import GoogleSpeaker
 from .minimax import MinimaxSpeaker
 from .openai import OpenAISpeaker
 from .volc import VolcSpeaker
+from .xunfei import XunfeiSpeaker
 
 ALL_SPEAKERS: Sequence[type[Speaker]] = [
     AzureSpeaker,
     BaiduSpeaker,
     EdgeSpeaker,
     GoogleSpeaker,
     MinimaxSpeaker,
     OpenAISpeaker,
     VolcSpeaker,
+    XunfeiSpeaker,
 ]
 
 
 def get_speaker(name: str) -> type[Speaker]:
     """Get a speaker by name.
 
     Args:
```

### Comparing `tetos-0.2.1/src/tetos/__main__.py` & `tetos-0.3.0/src/tetos/__main__.py`

 * *Files identical despite different names*

### Comparing `tetos-0.2.1/src/tetos/azure.py` & `tetos-0.3.0/src/tetos/azure.py`

 * *Files identical despite different names*

### Comparing `tetos-0.2.1/src/tetos/baidu.py` & `tetos-0.3.0/src/tetos/baidu.py`

 * *Files identical despite different names*

### Comparing `tetos-0.2.1/src/tetos/base.py` & `tetos-0.3.0/src/tetos/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from __future__ import annotations
 
 import abc
+import hashlib
+import hmac
 from pathlib import Path
 from typing import Any, Callable, TypeVar
 
 import click
 
 F = TypeVar("F", bound=Callable[..., Any])
 
@@ -108,7 +110,11 @@
         return func
 
     return decorator
 
 
 def filter_none(d: dict[str, Any]) -> dict[str, Any]:
     return {k: v for k, v in d.items() if v is not None}
+
+
+def hmac_sha256(content: str, secret: bytes) -> bytes:
+    return hmac.new(secret, content.encode("utf8"), hashlib.sha256).digest()
```

### Comparing `tetos-0.2.1/src/tetos/consts.py` & `tetos-0.3.0/src/tetos/consts.py`

 * *Files identical despite different names*

### Comparing `tetos-0.2.1/src/tetos/edge.py` & `tetos-0.3.0/src/tetos/edge.py`

 * *Files identical despite different names*

### Comparing `tetos-0.2.1/src/tetos/google.py` & `tetos-0.3.0/src/tetos/google.py`

 * *Files identical despite different names*

### Comparing `tetos-0.2.1/src/tetos/minimax.py` & `tetos-0.3.0/src/tetos/minimax.py`

 * *Files identical despite different names*

### Comparing `tetos-0.2.1/src/tetos/openai.py` & `tetos-0.3.0/src/tetos/openai.py`

 * *Files identical despite different names*

### Comparing `tetos-0.2.1/src/tetos/volc.py` & `tetos-0.3.0/src/tetos/volc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from __future__ import annotations
 
 import base64
 import hashlib
-import hmac
 import json
 import logging
 import time
 from datetime import datetime, timezone
 from pathlib import Path
 from typing import Any, Generator, cast
 
 import anyio
 import click
 from click.core import Command as Command
 from httpx import AsyncClient, Auth, Request
 from httpx._models import Response
 
-from .base import Speaker, SynthesizeError, common_options
+from .base import Speaker, SynthesizeError, common_options, hmac_sha256
 from .consts import VOLC_SUPPORTED_VOICES
 
 logger = logging.getLogger(__name__)
 
 
 class VolcSignAuth(Auth):
     ALGORITHM = "HMAC-SHA256"
@@ -31,18 +30,14 @@
         self, access_key: str, secret_key: str, service: str, region: str
     ) -> None:
         self.access_key = access_key
         self.secret_key = secret_key
         self.service = service
         self.region = region
 
-    @staticmethod
-    def hmac_sha256(key: bytes, content: str) -> bytes:
-        return hmac.new(key, content.encode("utf-8"), hashlib.sha256).digest()
-
     def auth_flow(self, request: Request) -> Generator[Request, Response, None]:
         x_content_sha256 = hashlib.sha256(request.content).hexdigest()
         x_date = datetime.now(timezone.utc).strftime("%Y%m%dT%H%M%SZ")
         signed_headers = "content-type;host;x-content-sha256;x-date"
         canonical_request = "\n".join(
             [
                 request.method.upper(),
@@ -66,16 +61,16 @@
                 x_date,
                 credential_scope,
                 canonical_request_hash,
             ]
         )
         sign_key = self.secret_key.encode()
         for scope in credential_scope.split("/"):
-            sign_key = self.hmac_sha256(sign_key, scope)
-        signature = self.hmac_sha256(sign_key, string_to_sign).hex()
+            sign_key = hmac_sha256(scope, sign_key)
+        signature = hmac_sha256(string_to_sign, sign_key).hex()
         authorization = (
             f"{self.ALGORITHM} Credential={self.access_key}/{credential_scope}"
             f", SignedHeaders={signed_headers}, Signature={signature}"
         )
         request.headers.update(
             {
                 "Authorization": authorization,
```

