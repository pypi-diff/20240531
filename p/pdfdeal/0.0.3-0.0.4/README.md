# Comparing `tmp/pdfdeal-0.0.3.tar.gz` & `tmp/pdfdeal-0.0.4.tar.gz`

## Comparing `pdfdeal-0.0.3.tar` & `pdfdeal-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,13 @@
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 pdfdeal-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pdfdeal-0.0.3/src/pdfdeal/__init__.py
--rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 pdfdeal-0.0.3/src/pdfdeal/file_tools.py
--rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 pdfdeal-0.0.3/src/pdfdeal/get_file.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 pdfdeal-0.0.3/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pdfdeal-0.0.3/LICENSE
--rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 pdfdeal-0.0.3/README.md
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 pdfdeal-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 pdfdeal-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 pdfdeal-0.0.4/README_CN.md
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pdfdeal-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 pdfdeal-0.0.4/docs/doc2x.md
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 pdfdeal-0.0.4/docs/doc2x_cn.md
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pdfdeal-0.0.4/src/pdfdeal/__init__.py
+-rw-r--r--   0        0        0     9973 2020-02-02 00:00:00.000000 pdfdeal-0.0.4/src/pdfdeal/doc2x.py
+-rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 pdfdeal-0.0.4/src/pdfdeal/file_tools.py
+-rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 pdfdeal-0.0.4/src/pdfdeal/get_file.py
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 pdfdeal-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pdfdeal-0.0.4/LICENSE
+-rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 pdfdeal-0.0.4/README.md
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 pdfdeal-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5825 2020-02-02 00:00:00.000000 pdfdeal-0.0.4/PKG-INFO
```

### Comparing `pdfdeal-0.0.3/.github/workflows/python-publish.yml` & `pdfdeal-0.0.4/.github/workflows/python-publish.yml`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # documentation.
 
 name: Upload Python Package
 
 on:
   release:
     types: [published]
+  workflow_dispatch:
 
 permissions:
   contents: read
 
 jobs:
   release-build:
     runs-on: ubuntu-latest
```

### Comparing `pdfdeal-0.0.3/src/pdfdeal/file_tools.py` & `pdfdeal-0.0.4/src/pdfdeal/file_tools.py`

 * *Files identical despite different names*

### Comparing `pdfdeal-0.0.3/src/pdfdeal/get_file.py` & `pdfdeal-0.0.4/src/pdfdeal/get_file.py`

 * *Files identical despite different names*

### Comparing `pdfdeal-0.0.3/.gitignore` & `pdfdeal-0.0.4/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+test.png
 test.py
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
```

### Comparing `pdfdeal-0.0.3/LICENSE` & `pdfdeal-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfdeal-0.0.3/README.md` & `pdfdeal-0.0.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,51 @@
 # pdfdeal
 
+For better RAG!
+
+🗺️ ENGLISH | [简体中文](README_CN.md)
+
 Easier to deal with PDF, extract readable text and OCR to recognise image text and clean the format. Make it more suitable for knowledge base construction.
 
 Its going to use [easyocr](https://github.com/JaidedAI/EasyOCR) to recognise the image and add it to the original text. If the output format uses pdf format, this ensures that the text is on the same number of pages in the new PDF as the original. You can use knowledge base applications (such as [Dify](https://github.com/langgenius/dify),[FastGPT](https://github.com/labring/FastGPT)) after the PDF processing, so that theoretically can reach a better recognition rate.
 
 ![image](https://github.com/Menghuan1918/pdfdeal/assets/122662527/371a17c5-e0cb-464b-a1c4-61d2963c772f)
 
-> The figure above shows a comparison of the results before and after the processing of the same PDF
+> The figure above shows a comparison of the results before and after the processing of the same PDF(version > 0.0.2 will have better results).
 > Unprocessed document encoding results <----> Processed file encoding results
 
+## Support for Doc2x
+
+Added support for Doc2x, which currently has a daily 500-page **free** usage quota, and its recognition of tables/formulas is excellent. 
+
+You can also use Doc2x support module **alone** to convert pdf to markdown/latex/docx directly like below. See [Doc2x Support](./docs/doc2x.md) for more.
+
+```python
+from pdfdeal.doc2x import Doc2x
+Client = Doc2x(api_key=your_api)
+Client.pdf2file(pdf_file="./ppt/test.pdf", output_path="./output", output_format="md_dollar", ocr=True)
+```
+
 ## Usage
+See the [example codes](https://github.com/Menghuan1918/pdfdeal?tab=readme-ov-file#processes-all-the-files-in-a-file-and-saves-them-in-the-output-folder).
+
 ### Install
 Install from PyPI:
 
 ```bash
 pip install 'pdfdeal[easyocr]'
 ```
 
 Using `pytesseract`, make sure you have install [tesseract](https://github.com/tesseract-ocr/tesseract) first:
 
 ```bash
 pip install 'pdfdeal[pytesseract]'
 ```
 
-Using own custom OCR function or skip OCR:
+Using own custom OCR function or Doc2x or skip OCR:
 
 ```bash
 pip install pdfdeal
 ```
 
 Install from source:
 
@@ -103,8 +121,12 @@
 print(f"Save processed file to {output_path}")
 ```
 
 ### Skip OCR
 
 ```python
 print(deal_pdf(input="test.pdf",ocr="pass"))
-```
+```
+
+### Doc2x support
+
+See [Doc2x Support](./docs/doc2x.md).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pdfdeal-0.0.3/pyproject.toml` & `pdfdeal-0.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pdfdeal"
-version = "0.0.3"
+version = "0.0.4"
 authors = [{ name = "Menghuan1918", email = "menghuan@menghuan1918.com" }]
 description = "Easier to deal with PDF, extract readable text and OCR to recognise image text and clean the format. Make it more suitable for knowledge base construction."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `pdfdeal-0.0.3/PKG-INFO` & `pdfdeal-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pdfdeal
-Version: 0.0.3
+Version: 0.0.4
 Summary: Easier to deal with PDF, extract readable text and OCR to recognise image text and clean the format. Make it more suitable for knowledge base construction.
 Project-URL: Homepage, https://github.com/Menghuan1918/pdfdeal
 Project-URL: Issues, https://github.com/Menghuan1918/pdfdeal/issues
 Author-email: Menghuan1918 <menghuan@menghuan1918.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,38 +22,56 @@
 Requires-Dist: easyocr; extra == 'easyocr'
 Provides-Extra: pytesseract
 Requires-Dist: pytesseract; extra == 'pytesseract'
 Description-Content-Type: text/markdown
 
 # pdfdeal
 
+For better RAG!
+
+🗺️ ENGLISH | [简体中文](README_CN.md)
+
 Easier to deal with PDF, extract readable text and OCR to recognise image text and clean the format. Make it more suitable for knowledge base construction.
 
 Its going to use [easyocr](https://github.com/JaidedAI/EasyOCR) to recognise the image and add it to the original text. If the output format uses pdf format, this ensures that the text is on the same number of pages in the new PDF as the original. You can use knowledge base applications (such as [Dify](https://github.com/langgenius/dify),[FastGPT](https://github.com/labring/FastGPT)) after the PDF processing, so that theoretically can reach a better recognition rate.
 
 ![image](https://github.com/Menghuan1918/pdfdeal/assets/122662527/371a17c5-e0cb-464b-a1c4-61d2963c772f)
 
-> The figure above shows a comparison of the results before and after the processing of the same PDF
+> The figure above shows a comparison of the results before and after the processing of the same PDF(version > 0.0.2 will have better results).
 > Unprocessed document encoding results <----> Processed file encoding results
 
+## Support for Doc2x
+
+Added support for Doc2x, which currently has a daily 500-page **free** usage quota, and its recognition of tables/formulas is excellent. 
+
+You can also use Doc2x support module **alone** to convert pdf to markdown/latex/docx directly like below. See [Doc2x Support](./docs/doc2x.md) for more.
+
+```python
+from pdfdeal.doc2x import Doc2x
+Client = Doc2x(api_key=your_api)
+Client.pdf2file(pdf_file="./ppt/test.pdf", output_path="./output", output_format="md_dollar", ocr=True)
+```
+
 ## Usage
+See the [example codes](https://github.com/Menghuan1918/pdfdeal?tab=readme-ov-file#processes-all-the-files-in-a-file-and-saves-them-in-the-output-folder).
+
 ### Install
 Install from PyPI:
 
 ```bash
 pip install 'pdfdeal[easyocr]'
 ```
 
 Using `pytesseract`, make sure you have install [tesseract](https://github.com/tesseract-ocr/tesseract) first:
 
 ```bash
 pip install 'pdfdeal[pytesseract]'
 ```
 
-Using own custom OCR function or skip OCR:
+Using own custom OCR function or Doc2x or skip OCR:
 
 ```bash
 pip install pdfdeal
 ```
 
 Install from source:
 
@@ -129,8 +147,12 @@
 print(f"Save processed file to {output_path}")
 ```
 
 ### Skip OCR
 
 ```python
 print(deal_pdf(input="test.pdf",ocr="pass"))
-```
+```
+
+### Doc2x support
+
+See [Doc2x Support](./docs/doc2x.md).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

