# Comparing `tmp/pandas-ods-reader-0.1.4.tar.gz` & `tmp/pandas_ods_reader-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-ods-reader-0.1.4.tar", max compression
+gzip compressed data, was "pandas_ods_reader-0.2.0.tar", max compression
```

## Comparing `pandas-ods-reader-0.1.4.tar` & `pandas_ods_reader-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1063 2021-10-03 15:05:38.294888 pandas-ods-reader-0.1.4/LICENSE.txt
--rw-r--r--   0        0        0     1451 2021-10-03 15:05:38.294888 pandas-ods-reader-0.1.4/README.md
--rw-r--r--   0        0        0      208 2021-10-04 15:04:12.773256 pandas-ods-reader-0.1.4/pandas_ods_reader/__init__.py
--rw-r--r--   0        0        0     2637 2021-10-03 15:05:38.310933 pandas-ods-reader-0.1.4/pandas_ods_reader/algo.py
--rw-r--r--   0        0        0     1157 2021-10-04 14:47:18.979161 pandas-ods-reader-0.1.4/pandas_ods_reader/main.py
--rw-r--r--   0        0        0     1977 2021-10-03 15:05:38.310933 pandas-ods-reader-0.1.4/pandas_ods_reader/parsers/fods.py
--rw-r--r--   0        0        0      592 2021-10-03 15:05:38.310933 pandas-ods-reader-0.1.4/pandas_ods_reader/parsers/ods.py
--rw-r--r--   0        0        0      912 2021-10-03 15:05:38.310933 pandas-ods-reader-0.1.4/pandas_ods_reader/utils.py
--rw-r--r--   0        0        0      835 2021-10-04 15:50:55.175387 pandas-ods-reader-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2439 1970-01-01 00:00:00.000000 pandas-ods-reader-0.1.4/setup.py
--rw-r--r--   0        0        0     2530 1970-01-01 00:00:00.000000 pandas-ods-reader-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-31 15:13:51.330055 pandas_ods_reader-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     1451 2024-05-31 15:13:51.330055 pandas_ods_reader-0.2.0/README.md
+-rw-r--r--   0        0        0      208 2024-05-31 15:13:51.330055 pandas_ods_reader-0.2.0/pandas_ods_reader/__init__.py
+-rw-r--r--   0        0        0     3071 2024-05-31 15:13:51.330055 pandas_ods_reader-0.2.0/pandas_ods_reader/algo.py
+-rw-r--r--   0        0        0     1515 2024-05-31 15:13:51.330055 pandas_ods_reader-0.2.0/pandas_ods_reader/main.py
+-rw-r--r--   0        0        0     2354 2024-05-31 15:13:51.330055 pandas_ods_reader-0.2.0/pandas_ods_reader/parsers/fods.py
+-rw-r--r--   0        0        0      993 2024-05-31 15:13:51.331055 pandas_ods_reader-0.2.0/pandas_ods_reader/parsers/ods.py
+-rw-r--r--   0        0        0      962 2024-05-31 15:13:51.331055 pandas_ods_reader-0.2.0/pandas_ods_reader/utils.py
+-rw-r--r--   0        0        0     1047 2024-05-31 15:13:51.332055 pandas_ods_reader-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2333 1970-01-01 00:00:00.000000 pandas_ods_reader-0.2.0/PKG-INFO
```

### Comparing `pandas-ods-reader-0.1.4/LICENSE.txt` & `pandas_ods_reader-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pandas-ods-reader-0.1.4/README.md` & `pandas_ods_reader-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pandas-ods-reader-0.1.4/pandas_ods_reader/parsers/fods.py` & `pandas_ods_reader-0.2.0/pandas_ods_reader/parsers/fods.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from pathlib import Path
+from typing import Iterator, Optional, Tuple, Union
+
 from lxml import etree
 
 
 BODY_TAG = "office:body"
 SPREADSHEET_TAG = "office:spreadsheet"
 OFFICE_KEY = "office"
 TABLE_KEY = "table"
@@ -9,57 +12,63 @@
 TABLE_ROW_TAG = "table:table-row"
 TABLE_CELL_TAG = "table:table-cell"
 TABLE_CELL_TEXT_TAG = "text:p"
 TABLE_CELL_REPEATED_ATTRIB = "number-columns-repeated"
 VALUE_TYPE_ATTRIB = "value-type"
 
 
-def get_doc(file_or_path):
+def get_doc(file_or_path: Path) -> etree._ElementTree:
     return etree.parse(str(file_or_path))
 
 
-def get_sheet(spreadsheet, sheet_id):
+def get_sheet(spreadsheet: etree._Element, sheet_id: Union[str, int]) -> etree._Element:
     namespaces = spreadsheet.nsmap
     if isinstance(sheet_id, str):
         sheet = spreadsheet.find(
-            f"{TABLE_TAG}[@table:name='{sheet_id}']", namespaces=namespaces
+            f"{TABLE_TAG}[@table:name='{sheet_id}']",
+            namespaces=namespaces,
         )
         if sheet is None:
             raise KeyError(f"There is no sheet named {sheet_id}.")
         return sheet
     tables = spreadsheet.findall(TABLE_TAG, namespaces=namespaces)
     if sheet_id == 0 or sheet_id > len(tables):
         raise IndexError(f"There is no sheet at index {sheet_id}.")
     return tables[sheet_id - 1]
 
 
-def get_rows(doc, sheet_id):
+def get_rows(
+    doc: etree._ElementTree,
+    sheet_id: Union[str, int],
+) -> Iterator[etree._Element]:
     if not isinstance(sheet_id, (str, int)):
         raise ValueError("Sheet id has to be either `str` or `int`")
     root = doc.getroot()
     namespaces = root.nsmap
-    spreadsheet = doc.find(BODY_TAG, namespaces=namespaces).find(
+    spreadsheet = doc.find(BODY_TAG, namespaces=namespaces).find(  # type: ignore
         SPREADSHEET_TAG, namespaces=namespaces
     )
     sheet = get_sheet(spreadsheet, sheet_id)
-    rows = sheet.findall(TABLE_ROW_TAG, namespaces=namespaces)
-    return rows
+    return sheet.iterfind(TABLE_ROW_TAG, namespaces=namespaces)
 
 
-def is_float(cell):
+def is_float(cell: etree._Element) -> bool:
     return (
         cell.attrib.get(f"{{{cell.nsmap[OFFICE_KEY]}}}{VALUE_TYPE_ATTRIB}") == "float"
     )
 
 
-def get_value(cell, parsed=False):
+def get_value(
+    cell: etree._Element,
+    parsed: bool = False,
+) -> Tuple[Optional[Union[str, float]], int]:
     text = cell.find(TABLE_CELL_TEXT_TAG, namespaces=cell.nsmap)
     if text is None:
         return None, 0
-    value = text.text
+    value: Union[str, float] = text.text or ""
     if parsed and is_float(cell):
         value = float(value)
-    n_repeated = cell.attrib.get(
+    _n_repeated = cell.attrib.get(
         f"{{{cell.nsmap[TABLE_KEY]}}}{TABLE_CELL_REPEATED_ATTRIB}"
     )
-    n_repeated = int(n_repeated) if n_repeated is not None else 0
+    n_repeated = int(_n_repeated) if _n_repeated is not None else 0
     return value, n_repeated
```

### Comparing `pandas-ods-reader-0.1.4/pandas_ods_reader/utils.py` & `pandas_ods_reader-0.2.0/pandas_ods_reader/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Provides utility functions for the parser"""
+import pandas as pd
 
 
 def ods_info(doc):
     """Print the number of sheets, their names, and number of rows and columns"""
     print("Spreadsheet contains {:d} sheet(s).".format(len(doc.sheets)))
     for sheet in doc.sheets:
         print("-" * 40)
@@ -10,16 +11,16 @@
         print(
             "Size of Sheet : (rows={:d}, cols={:d})".format(
                 sheet.nrows(), sheet.ncols()
             )
         )
 
 
-def sanitize_df(df):
-    """Drop empty rows and columns from the DataFrame and returns it"""
+def sanitize_df(df: pd.DataFrame) -> pd.DataFrame:
+    """Drop empty rows and columns from the DataFrame and return it."""
     # Delete empty rows
     for i in df.index.tolist()[-1::-1]:
         if df.iloc[i].isna().all():
             df.drop(i, inplace=True)
         else:
             break
     # Delete empty columns
```

### Comparing `pandas-ods-reader-0.1.4/PKG-INFO` & `pandas_ods_reader-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 Metadata-Version: 2.1
 Name: pandas-ods-reader
-Version: 0.1.4
+Version: 0.2.0
 Summary: Read in .ods and .fods files and return a pandas.DataFrame.
 Home-page: https://github.com/iuvbio/pandas_ods_reader
 License: MIT
 Keywords: data,io,pandas,ods
 Author: iuvbio
 Author-email: iuvbio@users.noreply.github.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8.1,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Dist: ezodf (>=0.3.2,<0.4.0)
-Requires-Dist: importlib_metadata (>=4.8.1,<5.0.0); python_version >= "3.7" and python_version < "3.8"
-Requires-Dist: lxml (>=4.6.3,<5.0.0)
-Requires-Dist: pandas (>=1.0.0,<2.0.0)
+Requires-Dist: lxml (>=4.9.2,<5.0.0)
+Requires-Dist: pandas (>=1.5.2,<2.0.0)
 Project-URL: Repository, https://github.com/iuvbio/pandas_ods_reader
 Description-Content-Type: text/markdown
 
 pandas-ods-reader
 ===
 
 Provides a function to read in a **.ods** or **.fods** file and returns a pandas DataFrame.
```

