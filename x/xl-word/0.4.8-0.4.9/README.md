# Comparing `tmp/xl_word-0.4.8.tar.gz` & `tmp/xl_word-0.4.9.tar.gz`

## Comparing `xl_word-0.4.8.tar` & `xl_word-0.4.9.tar`

### file list

```diff
@@ -1,42 +1,41 @@
--rw-r--r--   0        0        0    14003 2020-02-02 00:00:00.000000 xl_word-0.4.8/assets/h.docx
--rw-r--r--   0        0        0    13990 2020-02-02 00:00:00.000000 xl_word-0.4.8/assets/v.docx
--rw-r--r--   0        0        0    62053 2020-02-02 00:00:00.000000 xl_word-0.4.8/assets/img/word-template.png
--rw-r--r--   0        0        0    30134 2020-02-02 00:00:00.000000 xl_word-0.4.8/assets/img/wordx-tool.png
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 xl_word-0.4.8/src/wordx/.ctxt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 xl_word-0.4.8/src/wordx/__init__.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 xl_word-0.4.8/src/wordx/document.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 xl_word-0.4.8/src/wordx/mixins.py
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 xl_word-0.4.8/src/wordx/sheet.py
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 xl_word-0.4.8/src/wordx/word_file.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 xl_word-0.4.8/src/wordx/utils/fake_zip.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 xl_word-0.4.8/src/wordx/utils/tree.py
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 xl_word-0.4.8/tests/test_fake_zip.py
--rw-r--r--   0        0        0    11984 2020-02-02 00:00:00.000000 xl_word-0.4.8/tests/report/template.docx
--rw-r--r--   0        0        0    10073 2020-02-02 00:00:00.000000 xl_word-0.4.8/tests/report/test.docx
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 xl_word-0.4.8/tests/report/test.py
--rw-r--r--   0        0        0    15376 2020-02-02 00:00:00.000000 xl_word-0.4.8/tests/report/components/statement.xml
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 xl_word-0.4.8/tests/report/components/image/image.xml
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 xl_word-0.4.8/tests/report/components/page/blank.xml
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 xl_word-0.4.8/tests/report/components/page/horizontal.xml
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 xl_word-0.4.8/tests/report/components/page/pagination.xml
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 xl_word-0.4.8/tests/report/components/page/section.xml
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 xl_word-0.4.8/tests/report/components/page/vertical.xml
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 xl_word-0.4.8/tests/report/components/paragraph/empty_line.xml
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 xl_word-0.4.8/tests/report/components/paragraph/ident_paragraph.xml
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 xl_word-0.4.8/tests/report/components/paragraph/left_title.xml
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 xl_word-0.4.8/tests/report/components/paragraph/middle_title.xml
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 xl_word-0.4.8/tests/report/components/paragraph/paragraph.xml
--rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 xl_word-0.4.8/tests/report/components/table/table.xml
--rw-r--r--   0        0        0    14195 2020-02-02 00:00:00.000000 xl_word-0.4.8/tests/文档合并/123.docx
--rw-r--r--   0        0        0    14199 2020-02-02 00:00:00.000000 xl_word-0.4.8/tests/文档合并/456.docx
--rw-r--r--   0        0        0    12076 2020-02-02 00:00:00.000000 xl_word-0.4.8/tests/文档合并/merge.docx
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 xl_word-0.4.8/tests/文档合并/merge.py
--rw-r--r--   0        0        0    14003 2020-02-02 00:00:00.000000 xl_word-0.4.8/tool/h.docx
--rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 xl_word-0.4.8/tool/tool.pyw
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 xl_word-0.4.8/tool/tool.spec
--rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 xl_word-0.4.8/tool/utility.py
--rw-r--r--   0        0        0    13990 2020-02-02 00:00:00.000000 xl_word-0.4.8/tool/v.docx
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 xl_word-0.4.8/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xl_word-0.4.8/README.md
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 xl_word-0.4.8/pyproject.toml
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 xl_word-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0    14003 2020-02-02 00:00:00.000000 xl_word-0.4.9/assets/h.docx
+-rw-r--r--   0        0        0    13990 2020-02-02 00:00:00.000000 xl_word-0.4.9/assets/v.docx
+-rw-r--r--   0        0        0    62053 2020-02-02 00:00:00.000000 xl_word-0.4.9/assets/img/word-template.png
+-rw-r--r--   0        0        0    30134 2020-02-02 00:00:00.000000 xl_word-0.4.9/assets/img/wordx-tool.png
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 xl_word-0.4.9/src/xl_word/__init__.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 xl_word-0.4.9/src/xl_word/document.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 xl_word-0.4.9/src/xl_word/mixins.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 xl_word-0.4.9/src/xl_word/sheet.py
+-rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 xl_word-0.4.9/src/xl_word/word_file.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 xl_word-0.4.9/src/xl_word/utils/fake_zip.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 xl_word-0.4.9/src/xl_word/utils/tree.py
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 xl_word-0.4.9/tests/test_fake_zip.py
+-rw-r--r--   0        0        0    11984 2020-02-02 00:00:00.000000 xl_word-0.4.9/tests/report/template.docx
+-rw-r--r--   0        0        0    10073 2020-02-02 00:00:00.000000 xl_word-0.4.9/tests/report/test.docx
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 xl_word-0.4.9/tests/report/test.py
+-rw-r--r--   0        0        0    15376 2020-02-02 00:00:00.000000 xl_word-0.4.9/tests/report/components/statement.xml
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 xl_word-0.4.9/tests/report/components/image/image.xml
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 xl_word-0.4.9/tests/report/components/page/blank.xml
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 xl_word-0.4.9/tests/report/components/page/horizontal.xml
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 xl_word-0.4.9/tests/report/components/page/pagination.xml
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 xl_word-0.4.9/tests/report/components/page/section.xml
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 xl_word-0.4.9/tests/report/components/page/vertical.xml
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 xl_word-0.4.9/tests/report/components/paragraph/empty_line.xml
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 xl_word-0.4.9/tests/report/components/paragraph/ident_paragraph.xml
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 xl_word-0.4.9/tests/report/components/paragraph/left_title.xml
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 xl_word-0.4.9/tests/report/components/paragraph/middle_title.xml
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 xl_word-0.4.9/tests/report/components/paragraph/paragraph.xml
+-rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 xl_word-0.4.9/tests/report/components/table/table.xml
+-rw-r--r--   0        0        0    14195 2020-02-02 00:00:00.000000 xl_word-0.4.9/tests/文档合并/123.docx
+-rw-r--r--   0        0        0    14199 2020-02-02 00:00:00.000000 xl_word-0.4.9/tests/文档合并/456.docx
+-rw-r--r--   0        0        0    12076 2020-02-02 00:00:00.000000 xl_word-0.4.9/tests/文档合并/merge.docx
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 xl_word-0.4.9/tests/文档合并/merge.py
+-rw-r--r--   0        0        0    14003 2020-02-02 00:00:00.000000 xl_word-0.4.9/tool/h.docx
+-rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 xl_word-0.4.9/tool/tool.pyw
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 xl_word-0.4.9/tool/tool.spec
+-rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 xl_word-0.4.9/tool/utility.py
+-rw-r--r--   0        0        0    13990 2020-02-02 00:00:00.000000 xl_word-0.4.9/tool/v.docx
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 xl_word-0.4.9/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xl_word-0.4.9/README.md
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 xl_word-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 xl_word-0.4.9/PKG-INFO
```

### Comparing `xl_word-0.4.8/assets/h.docx` & `xl_word-0.4.9/assets/h.docx`

 * *Files identical despite different names*

### Comparing `xl_word-0.4.8/assets/v.docx` & `xl_word-0.4.9/assets/v.docx`

 * *Files identical despite different names*

### Comparing `xl_word-0.4.8/assets/img/word-template.png` & `xl_word-0.4.9/assets/img/word-template.png`

 * *Files identical despite different names*

### Comparing `xl_word-0.4.8/assets/img/wordx-tool.png` & `xl_word-0.4.9/assets/img/wordx-tool.png`

 * *Files identical despite different names*

### Comparing `xl_word-0.4.8/src/wordx/document.py` & `xl_word-0.4.9/src/xl_word/document.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from wordx.sheet import Sheet
+from xl_word.sheet import Sheet
 from pathlib import Path
 import os 
 
 
 class Document(Sheet):
     """Word表单对象"""
     def __init__(self, tpl_path, component_folder=None, xml_folder=None):
```

### Comparing `xl_word-0.4.8/src/wordx/mixins.py` & `xl_word-0.4.9/src/xl_word/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from wordx.utils.tree import Tree, E
+from xl_word.utils.tree import Tree, E
 import random
 
 
 class RelationMixin:
     def get_relations(self, xml_file):
         '''获取指定xml文件的资源映射
         wf.get_relations('document.xml')
```

### Comparing `xl_word-0.4.8/src/wordx/sheet.py` & `xl_word-0.4.9/src/xl_word/sheet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from wordx.word_file import WordFile
+from xl_word.word_file import WordFile
 from jinja2 import Template
 from pathlib import Path
 import math 
 
 
 class Sheet(WordFile):
     """Word表单对象"""
@@ -39,15 +39,15 @@
             return xml_string
         except AttributeError as e:
             pass
         except FileNotFoundError as e:
             print(e)
 
     def render_and_add_xml(self, xml_type, data):
-        xml_content = self.render_template(self.retrieve(f'word/{xml_type}.xml'), data)
+        xml_content = self.render_template(self[f'word/{xml_type}.xml'].decode(), data)
         return self.add_xml(xml_type, xml_content)
 
     def render(self, data):
         self.render_xml('header', data)
         self.render_xml('footer', data)
         self.render_xml('document', data)
         return self
```

### Comparing `xl_word-0.4.8/src/wordx/word_file.py` & `xl_word-0.4.9/src/xl_word/word_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from wordx.utils.fake_zip import FakeZip
-from wordx.utils.tree import Tree, E
-from wordx.mixins import RelationMixin
+from xl_word.utils.fake_zip import FakeZip
+from xl_word.utils.tree import Tree, E
+from xl_word.mixins import RelationMixin
 from io import BytesIO
 import random
 
 
 class WordFile(RelationMixin, FakeZip):
     '''Word文档对象'''
     def __init__(self, file_path):
```

### Comparing `xl_word-0.4.8/src/wordx/utils/fake_zip.py` & `xl_word-0.4.9/src/xl_word/utils/fake_zip.py`

 * *Files identical despite different names*

### Comparing `xl_word-0.4.8/tests/test_fake_zip.py` & `xl_word-0.4.9/tests/test_fake_zip.py`

 * *Files identical despite different names*

### Comparing `xl_word-0.4.8/tests/report/template.docx` & `xl_word-0.4.9/tests/report/template.docx`

 * *Files identical despite different names*

### Comparing `xl_word-0.4.8/tests/report/test.docx` & `xl_word-0.4.9/tests/report/test.docx`

 * *Files identical despite different names*

### Comparing `xl_word-0.4.8/tests/report/components/statement.xml` & `xl_word-0.4.9/tests/report/components/statement.xml`

 * *Files identical despite different names*

### Comparing `xl_word-0.4.8/tests/report/components/page/pagination.xml` & `xl_word-0.4.9/tests/report/components/page/pagination.xml`

 * *Files identical despite different names*

### Comparing `xl_word-0.4.8/tests/report/components/paragraph/left_title.xml` & `xl_word-0.4.9/tests/report/components/paragraph/left_title.xml`

 * *Files identical despite different names*

### Comparing `xl_word-0.4.8/tests/report/components/paragraph/middle_title.xml` & `xl_word-0.4.9/tests/report/components/paragraph/middle_title.xml`

 * *Files identical despite different names*

### Comparing `xl_word-0.4.8/tests/report/components/table/table.xml` & `xl_word-0.4.9/tests/report/components/table/table.xml`

 * *Files identical despite different names*

### Comparing `xl_word-0.4.8/tests/文档合并/123.docx` & `xl_word-0.4.9/tests/文档合并/123.docx`

 * *Files identical despite different names*

### Comparing `xl_word-0.4.8/tests/文档合并/456.docx` & `xl_word-0.4.9/tests/文档合并/456.docx`

 * *Files identical despite different names*

### Comparing `xl_word-0.4.8/tests/文档合并/merge.docx` & `xl_word-0.4.9/tests/文档合并/merge.docx`

 * *Files identical despite different names*

### Comparing `xl_word-0.4.8/tool/h.docx` & `xl_word-0.4.9/tool/h.docx`

 * *Files identical despite different names*

### Comparing `xl_word-0.4.8/tool/tool.pyw` & `xl_word-0.4.9/tool/tool.pyw`

 * *Files identical despite different names*

### Comparing `xl_word-0.4.8/tool/tool.spec` & `xl_word-0.4.9/tool/tool.spec`

 * *Files identical despite different names*

### Comparing `xl_word-0.4.8/tool/utility.py` & `xl_word-0.4.9/tool/utility.py`

 * *Files identical despite different names*

### Comparing `xl_word-0.4.8/tool/v.docx` & `xl_word-0.4.9/tool/v.docx`

 * *Files identical despite different names*

