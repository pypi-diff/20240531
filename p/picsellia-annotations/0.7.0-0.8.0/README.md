# Comparing `tmp/picsellia_annotations-0.7.0.tar.gz` & `tmp/picsellia_annotations-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picsellia_annotations-0.7.0.tar", max compression
+gzip compressed data, was "picsellia_annotations-0.8.0.tar", max compression
```

## Comparing `picsellia_annotations-0.7.0.tar` & `picsellia_annotations-0.8.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2024-01-16 15:05:49.045977 picsellia_annotations-0.7.0/LICENSE
--rw-r--r--   0        0        0       22 2024-01-25 14:57:41.019122 picsellia_annotations-0.7.0/picsellia_annotations/__init__.py
--rw-r--r--   0        0        0     2815 2024-01-25 14:45:42.078412 picsellia_annotations-0.7.0/picsellia_annotations/coco.py
--rw-r--r--   0        0        0       79 2024-01-16 15:05:49.045977 picsellia_annotations-0.7.0/picsellia_annotations/exceptions.py
--rw-r--r--   0        0        0     2208 2024-01-25 14:45:42.078412 picsellia_annotations-0.7.0/picsellia_annotations/utils.py
--rw-r--r--   0        0        0      659 2024-01-25 14:38:57.283555 picsellia_annotations-0.7.0/picsellia_annotations/video_coco.py
--rw-r--r--   0        0        0     1598 2024-01-16 15:05:49.045977 picsellia_annotations-0.7.0/picsellia_annotations/voc.py
--rw-r--r--   0        0        0      493 2024-01-25 14:57:41.019122 picsellia_annotations-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 picsellia_annotations-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-02-15 14:04:51.733446 picsellia_annotations-0.8.0/LICENSE
+-rw-r--r--   0        0        0       22 2024-02-15 14:04:51.733446 picsellia_annotations-0.8.0/picsellia_annotations/__init__.py
+-rw-r--r--   0        0        0     3320 2024-02-15 14:04:51.733446 picsellia_annotations-0.8.0/picsellia_annotations/coco.py
+-rw-r--r--   0        0        0       79 2024-01-16 15:05:49.045977 picsellia_annotations-0.8.0/picsellia_annotations/exceptions.py
+-rw-r--r--   0        0        0     2225 2024-02-15 14:04:51.733446 picsellia_annotations-0.8.0/picsellia_annotations/utils.py
+-rw-r--r--   0        0        0      931 2024-02-15 14:04:51.733446 picsellia_annotations-0.8.0/picsellia_annotations/video_coco.py
+-rw-r--r--   0        0        0     1847 2024-02-15 14:04:51.737445 picsellia_annotations-0.8.0/picsellia_annotations/voc.py
+-rw-r--r--   0        0        0      568 2024-02-15 14:04:51.737445 picsellia_annotations-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 picsellia_annotations-0.8.0/PKG-INFO
```

### Comparing `picsellia_annotations-0.7.0/LICENSE` & `picsellia_annotations-0.8.0/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `picsellia_annotations-0.7.0/picsellia_annotations/utils.py` & `picsellia_annotations-0.8.0/picsellia_annotations/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 def read_video_coco_file(file_path: str) -> VideoCOCOFile:
     return _read_file(file_path, VideoCOCOFile)
 
 
 def write_coco_file(cocofile: COCOFile) -> str:
     try:
-        return cocofile.json()
+        return cocofile.model_dump_json()
     except Exception as e:  # pragma: no cover
         raise ParsingError(str(e))
 
 
 def read_pascal_voc_file(
     file_path: str, check_polygon_consistency: bool = False
 ) -> PascalVOCFile:
@@ -67,13 +67,13 @@
 
 
 def write_pascal_voc_file(
     voc: PascalVOCFile, output=None, pretty: bool = True, full_document: bool = False
 ) -> str:
     try:
         xmlstr = xmltodict.unparse(
-            voc.dict(), output=output, full_document=full_document, pretty=pretty
+            voc.model_dump(), output=output, full_document=full_document, pretty=pretty
         )
     except Exception as e:  # pragma: no cover
         raise ParsingError(str(e))
 
     return xmlstr
```

### Comparing `picsellia_annotations-0.7.0/picsellia_annotations/voc.py` & `picsellia_annotations-0.8.0/picsellia_annotations/voc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, List, Optional, Union
 
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 
 
 class Size(BaseModel):
     width: int
     height: int
     depth: int
 
@@ -18,20 +18,20 @@
     xmax: Union[int, float]
     ymin: Union[int, float]
     ymax: Union[int, float]
 
 
 class Object(BaseModel):
     name: str
-    pose: Optional[str]
-    truncated: Optional[int]
-    difficult: Optional[int]
-    occluded: Optional[int]
-    bndbox: Optional[BndBox]
-    polygon: Optional[Dict[str, Union[int, float]]]
+    pose: Optional[str] = Field(default=None)
+    truncated: Optional[int] = Field(default=None)
+    difficult: Optional[int] = Field(default=None)
+    occluded: Optional[int] = Field(default=None)
+    bndbox: Optional[BndBox] = Field(default=None)
+    polygon: Optional[Dict[str, Union[int, float]]] = Field(default=None)
 
     def is_rle(self) -> bool:
         return False
 
     def is_polygon(self) -> bool:
         return self.polygon is not None
 
@@ -53,16 +53,16 @@
 
         return coords
 
 
 class Annotation(BaseModel):
     filename: str
     object: Union[Object, List[Object]]
-    path: Optional[str]
-    folder: Optional[str]
-    source: Optional[Source]
-    size: Optional[Size]
-    segmented: Optional[int]
+    path: Optional[str] = Field(default=None)
+    folder: Optional[str] = Field(default=None)
+    source: Optional[Source] = Field(default=None)
+    size: Optional[Size] = Field(default=None)
+    segmented: Optional[int] = Field(default=None)
 
 
 class PascalVOCFile(BaseModel):
     annotation: Annotation
```

### Comparing `picsellia_annotations-0.7.0/PKG-INFO` & `picsellia_annotations-0.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: picsellia-annotations
-Version: 0.7.0
+Version: 0.8.0
 Summary: Package with pydantic schemas of COCO files and VOC File and some utils to read those annotations files
 Author: Thomas Darget
 Author-email: thomasdarget@hotmail.fr
-Requires-Python: >=3.7,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: pydantic (>=1.9,<2.0)
+Requires-Dist: pydantic (>=2.0.0,<3.0.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
```

