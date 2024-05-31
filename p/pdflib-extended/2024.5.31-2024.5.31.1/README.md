# Comparing `tmp/pdflib_extended-2024.5.31.tar.gz` & `tmp/pdflib_extended-2024.5.31.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdflib_extended-2024.5.31.tar", max compression
+gzip compressed data, was "pdflib_extended-2024.5.31.1.tar", max compression
```

## Comparing `pdflib_extended-2024.5.31.tar` & `pdflib_extended-2024.5.31.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0        0 2024-05-31 19:23:46.183854 pdflib_extended-2024.5.31/README.md
--rw-r--r--   0        0        0      885 2024-05-31 19:23:57.103950 pdflib_extended-2024.5.31/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-31 19:23:46.183854 pdflib_extended-2024.5.31/src/pdflib_extended/__init__.py
--rw-r--r--   0        0        0        0 2024-05-31 19:23:46.183854 pdflib_extended-2024.5.31/src/pdflib_extended/core/__init__.py
--rw-r--r--   0        0        0    15405 2024-05-31 19:23:46.183854 pdflib_extended-2024.5.31/src/pdflib_extended/core/binaries/linux/pdflib_py.pyi
--rw-r--r--   0        0        0 12241752 2024-05-31 19:23:46.247855 pdflib_extended-2024.5.31/src/pdflib_extended/core/binaries/linux/pdflib_py.so
--rw-r--r--   0        0        0  6616576 2024-05-31 19:23:46.283855 pdflib_extended-2024.5.31/src/pdflib_extended/core/binaries/windows/pdflib_py.pyd
--rw-r--r--   0        0        0    15405 2024-05-31 19:23:46.283855 pdflib_extended-2024.5.31/src/pdflib_extended/core/binaries/windows/pdflib_py.pyi
--rw-r--r--   0        0        0    19863 2024-05-31 19:23:46.283855 pdflib_extended-2024.5.31/src/pdflib_extended/core/pdflib_base.py
--rw-r--r--   0        0        0      302 2024-05-31 19:23:46.283855 pdflib_extended-2024.5.31/src/pdflib_extended/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-31 19:23:46.283855 pdflib_extended-2024.5.31/src/pdflib_extended/extensions/__init__.py
--rw-r--r--   0        0        0     3869 2024-05-31 19:23:46.283855 pdflib_extended-2024.5.31/src/pdflib_extended/extensions/barcodes.py
--rw-r--r--   0        0        0      360 2024-05-31 19:23:46.283855 pdflib_extended-2024.5.31/src/pdflib_extended/extensions/classes.py
--rw-r--r--   0        0        0     5131 2024-05-31 19:23:46.287855 pdflib_extended-2024.5.31/src/pdflib_extended/extensions/contexts.py
--rw-r--r--   0        0        0      708 2024-05-31 19:23:46.287855 pdflib_extended-2024.5.31/src/pdflib_extended/extensions/shapes.py
--rw-r--r--   0        0        0     1018 2024-05-31 19:23:46.287855 pdflib_extended-2024.5.31/src/pdflib_extended/extensions/text.py
--rw-r--r--   0        0        0     2113 2024-05-31 19:23:46.287855 pdflib_extended-2024.5.31/src/pdflib_extended/pdflib.py
--rw-r--r--   0        0        0        0 2024-05-31 19:23:46.287855 pdflib_extended-2024.5.31/src/pdflib_extended/py.typed
--rw-r--r--   0        0        0    22144 2024-05-31 19:23:46.287855 pdflib_extended-2024.5.31/src/pdflib_extended/resources/fonts/LibreBarcode128-Regular.ttf
--rw-r--r--   0        0        0   130832 2024-05-31 19:23:46.287855 pdflib_extended-2024.5.31/src/pdflib_extended/resources/fonts/OpenSans-Regular.ttf
--rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 pdflib_extended-2024.5.31/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-31 20:27:46.822221 pdflib_extended-2024.5.31.1/README.md
+-rw-r--r--   0        0        0      887 2024-05-31 20:27:55.562231 pdflib_extended-2024.5.31.1/pyproject.toml
+-rw-r--r--   0        0        0       29 2024-05-31 20:27:55.558231 pdflib_extended-2024.5.31.1/src/pdflib_extended/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 20:27:46.822221 pdflib_extended-2024.5.31.1/src/pdflib_extended/core/__init__.py
+-rw-r--r--   0        0        0    15405 2024-05-31 20:27:46.826221 pdflib_extended-2024.5.31.1/src/pdflib_extended/core/binaries/linux/pdflib_py.pyi
+-rw-r--r--   0        0        0 12241752 2024-05-31 20:27:46.890221 pdflib_extended-2024.5.31.1/src/pdflib_extended/core/binaries/linux/pdflib_py.so
+-rw-r--r--   0        0        0  6616576 2024-05-31 20:27:46.926221 pdflib_extended-2024.5.31.1/src/pdflib_extended/core/binaries/windows/pdflib_py.pyd
+-rw-r--r--   0        0        0    15405 2024-05-31 20:27:46.926221 pdflib_extended-2024.5.31.1/src/pdflib_extended/core/binaries/windows/pdflib_py.pyi
+-rw-r--r--   0        0        0    19863 2024-05-31 20:27:46.926221 pdflib_extended-2024.5.31.1/src/pdflib_extended/core/pdflib_base.py
+-rw-r--r--   0        0        0      302 2024-05-31 20:27:46.926221 pdflib_extended-2024.5.31.1/src/pdflib_extended/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-31 20:27:46.926221 pdflib_extended-2024.5.31.1/src/pdflib_extended/extensions/__init__.py
+-rw-r--r--   0        0        0     3856 2024-05-31 20:27:46.926221 pdflib_extended-2024.5.31.1/src/pdflib_extended/extensions/barcodes.py
+-rw-r--r--   0        0        0      360 2024-05-31 20:27:46.926221 pdflib_extended-2024.5.31.1/src/pdflib_extended/extensions/classes.py
+-rw-r--r--   0        0        0     5103 2024-05-31 20:27:46.926221 pdflib_extended-2024.5.31.1/src/pdflib_extended/extensions/contexts.py
+-rw-r--r--   0        0        0      694 2024-05-31 20:27:46.926221 pdflib_extended-2024.5.31.1/src/pdflib_extended/extensions/shapes.py
+-rw-r--r--   0        0        0     1004 2024-05-31 20:27:46.926221 pdflib_extended-2024.5.31.1/src/pdflib_extended/extensions/text.py
+-rw-r--r--   0        0        0     2098 2024-05-31 20:27:46.926221 pdflib_extended-2024.5.31.1/src/pdflib_extended/pdflib.py
+-rw-r--r--   0        0        0        0 2024-05-31 20:27:46.926221 pdflib_extended-2024.5.31.1/src/pdflib_extended/py.typed
+-rw-r--r--   0        0        0    22144 2024-05-31 20:27:46.926221 pdflib_extended-2024.5.31.1/src/pdflib_extended/resources/fonts/LibreBarcode128-Regular.ttf
+-rw-r--r--   0        0        0   130832 2024-05-31 20:27:46.926221 pdflib_extended-2024.5.31.1/src/pdflib_extended/resources/fonts/OpenSans-Regular.ttf
+-rw-r--r--   0        0        0      483 1970-01-01 00:00:00.000000 pdflib_extended-2024.5.31.1/PKG-INFO
```

### Comparing `pdflib_extended-2024.5.31/pyproject.toml` & `pdflib_extended-2024.5.31.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdflib-extended"
-version = "2024.05.31"
+version = "2024.05.31.1"
 description = ""
 authors = ["RichardS <richards@eoshost.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pylibdmtx = "^0.1.10"
```

### Comparing `pdflib_extended-2024.5.31/src/pdflib_extended/core/binaries/linux/pdflib_py.pyi` & `pdflib_extended-2024.5.31.1/src/pdflib_extended/core/binaries/linux/pdflib_py.pyi`

 * *Files identical despite different names*

### Comparing `pdflib_extended-2024.5.31/src/pdflib_extended/core/binaries/linux/pdflib_py.so` & `pdflib_extended-2024.5.31.1/src/pdflib_extended/core/binaries/linux/pdflib_py.so`

 * *Files identical despite different names*

### Comparing `pdflib_extended-2024.5.31/src/pdflib_extended/core/binaries/windows/pdflib_py.pyi` & `pdflib_extended-2024.5.31.1/src/pdflib_extended/core/binaries/windows/pdflib_py.pyi`

 * *Files identical despite different names*

### Comparing `pdflib_extended-2024.5.31/src/pdflib_extended/core/pdflib_base.py` & `pdflib_extended-2024.5.31.1/src/pdflib_extended/core/pdflib_base.py`

 * *Files identical despite different names*

### Comparing `pdflib_extended-2024.5.31/src/pdflib_extended/extensions/barcodes.py` & `pdflib_extended-2024.5.31.1/src/pdflib_extended/extensions/barcodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from PIL import Image
 from io import BytesIO
-from pylibdmtx.pylibdmtx import encode, Encoded
 from typing import Union, Optional
 
-from pdflib_extended.core.pdflib_base import PDFlibBase
+from PIL import Image
+from pylibdmtx.pylibdmtx import encode, Encoded
+
 from .classes import Point, Box
 from .text import text_box
+from ..core.pdflib_base import PDFlibBase
 
 
 def datamatrix(p: PDFlibBase, data: str, point: Point, scale: float) -> int:
     """
     Creates a datamatrix.
 
     :param p:
```

### Comparing `pdflib_extended-2024.5.31/src/pdflib_extended/extensions/contexts.py` & `pdflib_extended-2024.5.31.1/src/pdflib_extended/extensions/contexts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from contextlib import AbstractContextManager
 from pathlib import Path
 from typing import Union, Optional, Self, ContextManager
 
-from pdflib_extended.core.pdflib_base import PDFlibBase
-from pdflib_extended.exceptions import (
+from ..core.pdflib_base import PDFlibBase
+from ..exceptions import (
     InvalidDocumentHandle,
     InvalidPageHandle,
     DocumentWriteException,
     EmptyNewDocumentException,
     InvalidImageHandle,
 )
```

### Comparing `pdflib_extended-2024.5.31/src/pdflib_extended/extensions/shapes.py` & `pdflib_extended-2024.5.31.1/src/pdflib_extended/extensions/shapes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pdflib_extended.core.pdflib_base import PDFlibBase
+from ..core.pdflib_base import PDFlibBase
 from .classes import Box
 
 
 def rectangle(p: PDFlibBase, box: Box, c: float, m: float, y: float, k: float) -> int:
     page_height: float = p.get_option("pageheight", "") / 72
 
     # Adjust box to be drawn correctly
```

### Comparing `pdflib_extended-2024.5.31/src/pdflib_extended/extensions/text.py` & `pdflib_extended-2024.5.31.1/src/pdflib_extended/extensions/text.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from ..exceptions import InvalidTextflowHandle
-from pdflib_extended.core.pdflib_base import PDFlibBase
+from ..core.pdflib_base import PDFlibBase
 from .classes import Box
+from ..exceptions import InvalidTextflowHandle
 
 
 def text_box(
     p: PDFlibBase,
     text: str,
     box: Box,
     font_name: str,
```

### Comparing `pdflib_extended-2024.5.31/src/pdflib_extended/pdflib.py` & `pdflib_extended-2024.5.31.1/src/pdflib_extended/pdflib.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 from typing import ContextManager, Union, Optional
 
-from pdflib_extended.extensions.contexts import Document, NewDocument, Image
 from .core.pdflib_base import PDFlibBase
 from .extensions.barcodes import omr, code_128, datamatrix
 from .extensions.classes import Point, Box
+from .extensions.contexts import Document, NewDocument, Image
 from .extensions.shapes import rectangle
 from .extensions.text import text_box
 
 BASE_DIR = Path(__file__).resolve().parent
 
 
 class PDFlib(PDFlibBase):
```

### Comparing `pdflib_extended-2024.5.31/src/pdflib_extended/resources/fonts/LibreBarcode128-Regular.ttf` & `pdflib_extended-2024.5.31.1/src/pdflib_extended/resources/fonts/LibreBarcode128-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pdflib_extended-2024.5.31/src/pdflib_extended/resources/fonts/OpenSans-Regular.ttf` & `pdflib_extended-2024.5.31.1/src/pdflib_extended/resources/fonts/OpenSans-Regular.ttf`

 * *Files identical despite different names*

