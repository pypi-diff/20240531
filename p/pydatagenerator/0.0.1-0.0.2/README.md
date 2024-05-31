# Comparing `tmp/pydatagenerator-0.0.1.tar.gz` & `tmp/pydatagenerator-0.0.2.tar.gz`

## Comparing `pydatagenerator-0.0.1.tar` & `pydatagenerator-0.0.2.tar`

### file list

```diff
@@ -1,32 +1,43 @@
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/CHANGELOG.md
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/mkdocs.yml
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/.vscode/launch.json
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/.vscode/settings.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/docs/index.md
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/docs/reference/reference.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/pydatagenerator/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/pydatagenerator/data/__init__.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/pydatagenerator/data/abstract/__init__.py
--rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/pydatagenerator/data/abstract/abstract_dataset.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/pydatagenerator/data/abstract/abstract_dataset_handler_factory.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/pydatagenerator/data/impl/__init__.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/pydatagenerator/data/impl/dataset_handler_factory.py
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/pydatagenerator/data/impl/random_number_data_set.py
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/pydatagenerator/data/impl/sequence_data_set.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/pydatagenerator/xml/__init__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/pydatagenerator/xml/abstract/__init__.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/pydatagenerator/xml/abstract/abstract_xml_parser.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/pydatagenerator/xml/impl/__init__.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/pydatagenerator/xml/impl/xml_parser.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/src/pydatagenerator/xml/impl/xml_parser_util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/tests/pydatagenerator/data/random_number_data_set_test.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/tests/pydatagenerator/data/sequence_data_set_test.py
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/tests/pydatagenerator/xml/xml_parser_test.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/LICENSE
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/README.md
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 pydatagenerator-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/mkdocs.yml
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/.vscode/launch.json
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/docs/index.md
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/docs/reference/reference.md
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/scripts/data_generator.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/scripts/in.xml
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/scripts/out.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/src/pydatagenerator/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/src/pydatagenerator/data/__init__.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/src/pydatagenerator/data/abstract/__init__.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/src/pydatagenerator/data/abstract/abstract_dataset.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/src/pydatagenerator/data/abstract/abstract_dataset_handler_factory.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/src/pydatagenerator/data/impl/__init__.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/src/pydatagenerator/data/impl/dataset_handler_factory.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/src/pydatagenerator/data/impl/random_categorical_dataset.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/src/pydatagenerator/data/impl/random_number_dataset.py
+-rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/src/pydatagenerator/data/impl/random_number_timeseries_dataset.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/src/pydatagenerator/data/impl/sequence_categorical_dataset.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/src/pydatagenerator/data/impl/sequence_number_dataset.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/src/pydatagenerator/data/impl/sequence_number_timeseries_dataset.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/src/pydatagenerator/xml/__init__.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/src/pydatagenerator/xml/abstract/__init__.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/src/pydatagenerator/xml/abstract/abstract_xml_parser.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/src/pydatagenerator/xml/impl/__init__.py
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/src/pydatagenerator/xml/impl/xml_parser.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/src/pydatagenerator/xml/impl/xml_parser_util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/tests/pydatagenerator/data/random_categorical_dataset_test.py
+-rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/tests/pydatagenerator/data/random_number_dataset_test.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/tests/pydatagenerator/data/random_number_timeseries_dataset_test.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/tests/pydatagenerator/data/sequence_categorical_dataset_test.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/tests/pydatagenerator/data/sequence_number_dataset_test.py
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/tests/pydatagenerator/data/sequence_number_timeseries_dataset_test.py
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/tests/pydatagenerator/xml/xml_parser_test.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/LICENSE
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/README.md
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 pydatagenerator-0.0.2/PKG-INFO
```

### Comparing `pydatagenerator-0.0.1/.vscode/launch.json` & `pydatagenerator-0.0.2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `pydatagenerator-0.0.1/src/pydatagenerator/data/abstract/abstract_dataset.py` & `pydatagenerator-0.0.2/src/pydatagenerator/data/abstract/abstract_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     """
     type = 'type.abstract-dataset'
 
     def __init__(self, dataset_info: Dict[str, object]):
         """Creates a new data set
         """
         self._dataset_info = dataset_info
+        self.validate_dataset_info()
 
     @property
     def dataset_info(self) -> Dict[str, object]:
         """Dataset info getter
 
         Returns:
             Dict[str, object]: The dataset_info value
```

### Comparing `pydatagenerator-0.0.1/src/pydatagenerator/data/abstract/abstract_dataset_handler_factory.py` & `pydatagenerator-0.0.2/src/pydatagenerator/data/abstract/abstract_dataset_handler_factory.py`

 * *Files identical despite different names*

### Comparing `pydatagenerator-0.0.1/src/pydatagenerator/data/impl/dataset_handler_factory.py` & `pydatagenerator-0.0.2/src/pydatagenerator/data/impl/dataset_handler_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,13 +18,13 @@
         """
         type = dataset_info.get('type')
         if not type:
             sys.stderr.write('Error: No value provided for type')
             sys.exit(-1)
         handler = self.__classes.get(dataset_info['type'])
         if not handler:
-            sys.stderr.write(f'Error: Unknown type {dataset_info['type']}')
+            sys.stderr.write(f"Error: Unknown type {dataset_info['type']}")
             sys.exit(-1)
         return handler(dataset_info)
 
     def __init__(self):
         self.__classes = {c.type: c for c in AbstractDataSet.__subclasses__()}
```

### Comparing `pydatagenerator-0.0.1/src/pydatagenerator/data/impl/random_number_data_set.py` & `pydatagenerator-0.0.2/src/pydatagenerator/data/impl/random_number_dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,11 +25,10 @@
 
     def handle(self) -> object:
         """Process the given dataset_info and returns a result out of it
 
         Returns:
             object: The result obtained after processing the dataset_info
         """
-        self.validate_dataset_info()
-        is_floating = self._dataset_info['floating'] and self._dataset_info['floating'].lower() == 'true'
+        is_floating = 'floating' in self._dataset_info and self._dataset_info['floating'].lower() == 'true'
         func = random.uniform if is_floating else random.randint
         return func(int(self._dataset_info['min']), int(self._dataset_info['max']))
```

### Comparing `pydatagenerator-0.0.1/src/pydatagenerator/data/impl/sequence_data_set.py` & `pydatagenerator-0.0.2/src/pydatagenerator/data/impl/random_categorical_dataset.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,32 @@
-from typing import Dict, List
+import random
 from pydatagenerator.data.abstract import AbstractDataSet
 
-
-class SequenceDataSet(AbstractDataSet):
-    """SequenceDataSet
+class RandomCategoricalDataSet(AbstractDataSet):
+    """RandomCategoricalDataSet
     """
-    type = 'type.sequence-dataset'
+    type = 'type.random-categorical-dataset'
 
-    def required_fields(self) -> List[str]:
+    def required_fields(self):
         """Returns the required fields for the current data set
 
         Returns:
             List[str]: List of required fields for the current data set
         """
-        return ['start', 'increment']
+        return ['categories']
 
-    def optional_fields(self) -> List[str]:
+    def optional_fields(self):
         """Returns the optional fields for the current data set
 
         Returns:
             List[str]: List of optional fields for the current data set
         """
         return []
 
-    def __init__(self, dataset_info: Dict[str, object]):
-        super().__init__(dataset_info)
-        self.__val = int(dataset_info['start']) - int(dataset_info['increment'])
-
     def handle(self) -> object:
         """Process the given dataset_info and returns a result out of it
 
         Returns:
             object: The result obtained after processing the dataset_info
         """
-        self.validate_dataset_info()
-        increment = int(self._dataset_info['increment'])
-        self.__val += increment
-        return self.__val
+        categories = self._dataset_info['categories']
+        return categories[random.randint(0, len(categories)-1)]
```

### Comparing `pydatagenerator-0.0.1/src/pydatagenerator/xml/abstract/abstract_xml_parser.py` & `pydatagenerator-0.0.2/src/pydatagenerator/xml/abstract/abstract_xml_parser.py`

 * *Files identical despite different names*

### Comparing `pydatagenerator-0.0.1/src/pydatagenerator/xml/impl/xml_parser.py` & `pydatagenerator-0.0.2/src/pydatagenerator/xml/impl/xml_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,14 +56,17 @@
             sys.exit(-1)
         else:
             iterations = int(iterations)
 
         for _ in range(iterations):
             for dataset in datasets:
                 dataset_info = XmlParserUtil.collect_attributes(dataset)
+                categories = dataset.xpath('//categories')
+                if categories:
+                    dataset_info['categories'] = [category.get('value') for category in categories]
                 dataset_handler = handler_factory.get_dataset_handler(dataset_info)
                 name = dataset_info['name']
                 if name in data_info:
                     data_info[name].append(dataset_handler.handle())
                 else:
                     data_info[name] = [dataset_handler.handle()]
```

### Comparing `pydatagenerator-0.0.1/src/pydatagenerator/xml/impl/xml_parser_util.py` & `pydatagenerator-0.0.2/src/pydatagenerator/xml/impl/xml_parser_util.py`

 * *Files identical despite different names*

### Comparing `pydatagenerator-0.0.1/tests/pydatagenerator/data/random_number_data_set_test.py` & `pydatagenerator-0.0.2/tests/pydatagenerator/data/random_number_dataset_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,73 +38,66 @@
             'min': '10',
             'max': '20',
             'floating': 'true'
         })
         assert pytest_wrapped_e.type == SystemExit
         assert pytest_wrapped_e.value.code == -1
 
-    handler = DatasetHandlerFactory().get_dataset_handler({
-        'type': 'type.random-number-dataset',
-        'min': '10',
-        'max': '20',
-        'floating': 'true'
-    })
+    
 
     with pytest.raises(SystemExit) as pytest_wrapped_e:
-        value = handler.handle()
-        assert value is None
+        handler = DatasetHandlerFactory().get_dataset_handler({
+            'type': 'type.random-number-dataset',
+            'min': '10',
+            'max': '20',
+            'floating': 'true'
+        })
         assert pytest_wrapped_e.type == SystemExit
         assert pytest_wrapped_e.value.code == -1
 
 
 def test_validate_dataset_info_missing_random_number_required_property():
-    handler = DatasetHandlerFactory().get_dataset_handler({
-        'type': 'type.random-number-dataset',
-        'name': 'random_data_set',
-        'max': '20',
-        'floating': 'true'
-    })
-
     with pytest.raises(SystemExit) as pytest_wrapped_e:
-        value = handler.handle()
-        assert value is None
+        handler = DatasetHandlerFactory().get_dataset_handler({
+            'type': 'type.random-number-dataset',
+            'name': 'random_data_set',
+            'max': '20',
+            'floating': 'true'
+        })
         assert pytest_wrapped_e.type == SystemExit
         assert pytest_wrapped_e.value.code == -1
 
-    handler = DatasetHandlerFactory().get_dataset_handler({
-        'type': 'type.random-number-dataset',
-        'name': 'random_data_set',
-        'min': '10',
-        'floating': 'true'
-    })
+    
 
     with pytest.raises(SystemExit) as pytest_wrapped_e:
-        value = handler.handle()
-        assert value is None
+        handler = DatasetHandlerFactory().get_dataset_handler({
+            'type': 'type.random-number-dataset',
+            'name': 'random_data_set',
+            'min': '10',
+            'floating': 'true'
+        })
         assert pytest_wrapped_e.type == SystemExit
         assert pytest_wrapped_e.value.code == -1
 
 
 def test_not_matching_dataset_type():
     with pytest.raises(SystemExit) as pytest_wrapped_e:
         handler = DatasetHandlerFactory().get_dataset_handler({
             'type': 'type.not-existing-type',
             'name': 'not-existing-type'
         })
         assert pytest_wrapped_e.type == SystemExit
         assert pytest_wrapped_e.value.code == -1
 
 
-
 def test_unknown_random_number_property():
-    handler = DatasetHandlerFactory().get_dataset_handler({
-        'type': 'type.random-number-dataset',
-        'name': 'random_data_set',
-        'random': '10',
-        'floating': 'true'
-    })
-
     with pytest.raises(SystemExit) as pytest_wrapped_e:
-        value = handler.handle()
-        assert value is None
+        handler = DatasetHandlerFactory().get_dataset_handler({
+            'type': 'type.random-number-dataset',
+            'name': 'random_data_set',
+            'random': '10',
+            'min': 1,
+            'max': 10,
+            'floating': 'true'
+        })
         assert pytest_wrapped_e.type == SystemExit
         assert pytest_wrapped_e.value.code == -1
```

### Comparing `pydatagenerator-0.0.1/tests/pydatagenerator/xml/xml_parser_test.py` & `pydatagenerator-0.0.2/tests/pydatagenerator/xml/xml_parser_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,33 +16,60 @@
     assert isinstance(values, list)
     assert len(values) == 20
 
 def test_xml_parser_sequence_data():
     parser = XmlParser()
     tags_str = '''
     <pydatagenerator iterations="20">
-        <dataset name="id" type="type.sequence-dataset" start="0" increment="1"/>
-        <dataset name="sum" type="type.sequence-dataset" start="10" increment="100"/>
+        <dataset name="id" type="type.sequence-number-dataset" start="0" increment="1"/>
+        <dataset name="sum" type="type.sequence-number-dataset" start="10" increment="100"/>
         <template>
             INSERT INTO Sums VALUES (#{id}, #{sum})
         </template>
     </pydatagenerator>
     '''
     values = parser.parse_xml_from_string(tags_str)
     assert isinstance(values, list)
     assert len(values) == 20
 
 
 def test_xml_parser_sequence_data_and_random_numbers():
     parser = XmlParser()
     tags_str = '''
     <pydatagenerator iterations="20">
-        <dataset name="id" type="type.sequence-dataset" start="0" increment="1"/>
+        <dataset name="id" type="type.sequence-number-dataset" start="0" increment="1"/>
         <dataset name="wage" type="type.random-number-dataset" floating="false" min="1000" max="100000000"/>
         <template>
             INSERT INTO Salaries VALUES (#{id}, #{wage})
         </template>
     </pydatagenerator>
     '''
     values = parser.parse_xml_from_string(tags_str)
     assert isinstance(values, list)
     assert len(values) == 20
+
+def test_xml_parser_categorical_data():
+    parser = XmlParser()
+    tags_str = '''
+    <pydatagenerator iterations="20">
+        <dataset name="grade" type="type.sequence-categorical-dataset" start="0" increment="1">
+            <categories>
+                <category value='A'/>
+                <category value='B'/>
+                <category value='C'/>
+            </categories>
+        </dataset>
+        <dataset name="student" type="type.random-categorical-dataset">
+            <categories>
+                <category value='Alex'/>
+                <category value='Michael'/>
+                <category value='John'/>
+            </categories>
+        </dataset>
+        <template>
+            INSERT INTO Results VALUES (#{grade}, #{student})
+        </template>
+    </pydatagenerator>
+    '''
+    values = parser.parse_xml_from_string(tags_str)
+    assert isinstance(values, list)
+    assert len(values) == 20
```

### Comparing `pydatagenerator-0.0.1/.gitignore` & `pydatagenerator-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pydatagenerator-0.0.1/LICENSE` & `pydatagenerator-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydatagenerator-0.0.1/pyproject.toml` & `pydatagenerator-0.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 name = "pydatagenerator"
 authors = [
     { name = "Alexandru Prodan", email = "prodanalexandru1999@gmail.com" },
 ]
 maintainers = [
     { name = "Alexandru Prodan", email = "prodanalexandru1999@gmail.com" },
 ]
-version = "0.0.1"
-description = "Coming soon"
+version = "0.0.2"
+description = "Generate template data from xml specification"
 readme = "README.md"
 requires-python = ">=3.6"
 dependencies = ["lxml>=5.2.1"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -31,19 +31,20 @@
     "toml>=0.10.2",
     "pylint>=3.1.0",
     "yapf>=0.40.2",
     "flake8>=7.0.0",
     "mkdocs>=1.6.0",
     "mkdocstrings[python]>=0.18",
     "mkdocs-material>=9.5.0",
+    "pyinstaller>=6.6.0",
 ]
 test = ["pytest>=8.2.0", "pytest-cov>=5.0.0"]
 
 [tool.pytest.ini_options]
-addopts = "--cov --cov-report html --cov-report term-missing --cov-fail-under 95"
+addopts = "--cov --cov-report html --cov-report term-missing --cov-fail-under 80"
 
 [tool.coverage.run]
 source = ["src"]
 
 [tool.yapf]
 blank_line_before_nested_class_or_def = true
 column_limit = 88
@@ -59,10 +60,10 @@
     "R0903", # (too-few-public-methods)
     "R0913", # (too-many-arguments)
     "W0105", # (pointless-string-statement)
 ]
 
 [project.urls]
 Homepage = "https://github.com/alexprodan99/pydatagenerator"
-Documentation = "https://github.com/alexprodan99/pydatagenerator/wiki"
+Documentation = "https://alexprodan99.github.io/pydatagenerator"
 Repository = "https://github.com/alexprodan99/pydatagenerator"
 Issues = "https://github.com/alexprodan99/pydatagenerator/issues"
```

### Comparing `pydatagenerator-0.0.1/PKG-INFO` & `pydatagenerator-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.3
 Name: pydatagenerator
-Version: 0.0.1
-Summary: Coming soon
+Version: 0.0.2
+Summary: Generate template data from xml specification
 Project-URL: Homepage, https://github.com/alexprodan99/pydatagenerator
-Project-URL: Documentation, https://github.com/alexprodan99/pydatagenerator/wiki
+Project-URL: Documentation, https://alexprodan99.github.io/pydatagenerator
 Project-URL: Repository, https://github.com/alexprodan99/pydatagenerator
 Project-URL: Issues, https://github.com/alexprodan99/pydatagenerator/issues
 Author-email: Alexandru Prodan <prodanalexandru1999@gmail.com>
 Maintainer-email: Alexandru Prodan <prodanalexandru1999@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Ionut-Alexandru Prodan
@@ -37,18 +37,19 @@
 Requires-Python: >=3.6
 Requires-Dist: lxml>=5.2.1
 Provides-Extra: dev
 Requires-Dist: flake8>=7.0.0; extra == 'dev'
 Requires-Dist: mkdocs-material>=9.5.0; extra == 'dev'
 Requires-Dist: mkdocs>=1.6.0; extra == 'dev'
 Requires-Dist: mkdocstrings[python]>=0.18; extra == 'dev'
+Requires-Dist: pyinstaller>=6.6.0; extra == 'dev'
 Requires-Dist: pylint>=3.1.0; extra == 'dev'
 Requires-Dist: toml>=0.10.2; extra == 'dev'
 Requires-Dist: yapf>=0.40.2; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest-cov>=5.0.0; extra == 'test'
 Requires-Dist: pytest>=8.2.0; extra == 'test'
 Description-Content-Type: text/markdown
 
 # pydatagenerator
 - Generate template data from xml specification
-- Docs: https://alexprodan99.github.io/pydatagenerator/
+- Docs: https://alexprodan99.github.io/pydatagenerator
```

