# Comparing `tmp/ilcdlib-4.7.0.tar.gz` & `tmp/ilcdlib-4.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilcdlib-4.7.0.tar", max compression
+gzip compressed data, was "ilcdlib-4.8.0.tar", max compression
```

## Comparing `ilcdlib-4.7.0.tar` & `ilcdlib-4.8.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0    11357 2024-05-24 03:16:30.801500 ilcdlib-4.7.0/LICENSE
--rw-r--r--   0        0        0     4949 2024-05-24 03:16:30.801500 ilcdlib-4.7.0/README.md
--rw-r--r--   0        0        0     3525 2024-05-24 03:16:30.801500 ilcdlib-4.7.0/pyproject.toml
--rw-r--r--   0        0        0      837 2024-05-24 03:16:30.801500 ilcdlib-4.7.0/src/ilcdlib/__init__.py
--rw-r--r--   0        0        0      910 2024-05-24 03:16:30.801500 ilcdlib-4.7.0/src/ilcdlib/__main__.py
--rw-r--r--   0        0        0      855 2024-05-24 03:16:30.801500 ilcdlib-4.7.0/src/ilcdlib/__version__.py
--rw-r--r--   0        0        0     2959 2024-05-24 03:16:30.801500 ilcdlib-4.7.0/src/ilcdlib/cli.py
--rw-r--r--   0        0        0    19110 2024-05-24 03:16:30.801500 ilcdlib-4.7.0/src/ilcdlib/common.py
--rw-r--r--   0        0        0      837 2024-05-24 03:16:30.801500 ilcdlib-4.7.0/src/ilcdlib/compat/__init__.py
--rw-r--r--   0        0        0     1158 2024-05-24 03:16:30.801500 ilcdlib-4.7.0/src/ilcdlib/compat/pydantic.py
--rw-r--r--   0        0        0     1835 2024-05-24 03:16:30.801500 ilcdlib-4.7.0/src/ilcdlib/const.py
--rw-r--r--   0        0        0     4934 2024-05-24 03:16:30.801500 ilcdlib-4.7.0/src/ilcdlib/data/category_mapping/epdnorge.csv
--rw-r--r--   0        0        0    51577 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/data/category_mapping/oekobaudat.csv
--rw-r--r--   0        0        0   172140 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/data/ilcd_epd_ref.zip
--rw-r--r--   0        0        0     6488 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/dto.py
--rw-r--r--   0        0        0      837 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/entity/__init__.py
--rw-r--r--   0        0        0     7064 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/entity/base_scope_set_reader.py
--rw-r--r--   0        0        0     3361 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/entity/category.py
--rw-r--r--   0        0        0     3052 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/entity/compliance.py
--rw-r--r--   0        0        0     6003 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/entity/contact.py
--rw-r--r--   0        0        0     4173 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/entity/exchage.py
--rw-r--r--   0        0        0     8138 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/entity/flow.py
--rw-r--r--   0        0        0     4224 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/entity/lcia.py
--rw-r--r--   0        0        0     5213 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/entity/material.py
--rw-r--r--   0        0        0     3930 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/entity/pcr.py
--rw-r--r--   0        0        0     3437 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/entity/source.py
--rw-r--r--   0        0        0     3788 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/entity/unit.py
--rw-r--r--   0        0        0     3326 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/entity/validation.py
--rw-r--r--   0        0        0      837 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/epd/__init__.py
--rw-r--r--   0        0        0    10064 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/epd/cli.py
--rw-r--r--   0        0        0      837 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/epd/dialect/__init__.py
--rw-r--r--   0        0        0     6864 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/epd/dialect/environdec.py
--rw-r--r--   0        0        0     2170 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/epd/dialect/epditaly.py
--rw-r--r--   0        0        0     5947 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/epd/dialect/epdnorge.py
--rw-r--r--   0        0        0     1329 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/epd/dialect/indata.py
--rw-r--r--   0        0        0     2326 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/epd/dialect/itb.py
--rw-r--r--   0        0        0     3876 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/epd/dialect/oekobaudat.py
--rw-r--r--   0        0        0     3644 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/epd/factory.py
--rw-r--r--   0        0        0    35487 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/epd/reader.py
--rw-r--r--   0        0        0     2248 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/extension.py
--rw-r--r--   0        0        0     7895 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/http_common.py
--rw-r--r--   0        0        0      837 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/mapping/__init__.py
--rw-r--r--   0        0        0    10680 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/mapping/category.py
--rw-r--r--   0        0        0     3603 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/mapping/common.py
--rw-r--r--   0        0        0     1168 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/mapping/compliance.py
--rw-r--r--   0        0        0     1512 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/mapping/flows.py
--rw-r--r--   0        0        0     3538 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/mapping/impacts.py
--rw-r--r--   0        0        0     1651 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/mapping/indicators.py
--rw-r--r--   0        0        0     1212 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/mapping/properties.py
--rw-r--r--   0        0        0     6247 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/mapping/units.py
--rw-r--r--   0        0        0      837 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/medium/__init__.py
--rw-r--r--   0        0        0     7531 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/medium/archive.py
--rw-r--r--   0        0        0     6496 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/medium/soda4lca.py
--rw-r--r--   0        0        0        0 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/py.typed
--rw-r--r--   0        0        0     1435 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/reference_data.py
--rw-r--r--   0        0        0      837 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/sanitizing/__init__.py
--rw-r--r--   0        0        0     1866 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/sanitizing/domain.py
--rw-r--r--   0        0        0     1336 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/sanitizing/phone.py
--rw-r--r--   0        0        0     1122 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/sanitizing/text.py
--rw-r--r--   0        0        0      837 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/soda4lca/__init__.py
--rw-r--r--   0        0        0    11347 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/soda4lca/api_client.py
--rw-r--r--   0        0        0     2755 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/soda4lca/api_client_4x.py
--rw-r--r--   0        0        0     1206 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/type.py
--rw-r--r--   0        0        0     6465 2024-05-24 03:16:30.809500 ilcdlib-4.7.0/src/ilcdlib/utils.py
--rw-r--r--   0        0        0     2399 2024-05-24 03:16:30.809500 ilcdlib-4.7.0/src/ilcdlib/xml_parser.py
--rw-r--r--   0        0        0     6082 1970-01-01 00:00:00.000000 ilcdlib-4.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-31 18:51:32.566246 ilcdlib-4.8.0/LICENSE
+-rw-r--r--   0        0        0     4949 2024-05-31 18:51:32.566246 ilcdlib-4.8.0/README.md
+-rw-r--r--   0        0        0     3525 2024-05-31 18:51:32.566246 ilcdlib-4.8.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2024-05-31 18:51:32.566246 ilcdlib-4.8.0/src/ilcdlib/__init__.py
+-rw-r--r--   0        0        0      910 2024-05-31 18:51:32.566246 ilcdlib-4.8.0/src/ilcdlib/__main__.py
+-rw-r--r--   0        0        0      855 2024-05-31 18:51:32.566246 ilcdlib-4.8.0/src/ilcdlib/__version__.py
+-rw-r--r--   0        0        0     2959 2024-05-31 18:51:32.566246 ilcdlib-4.8.0/src/ilcdlib/cli.py
+-rw-r--r--   0        0        0    19110 2024-05-31 18:51:32.566246 ilcdlib-4.8.0/src/ilcdlib/common.py
+-rw-r--r--   0        0        0      837 2024-05-31 18:51:32.566246 ilcdlib-4.8.0/src/ilcdlib/compat/__init__.py
+-rw-r--r--   0        0        0     1158 2024-05-31 18:51:32.566246 ilcdlib-4.8.0/src/ilcdlib/compat/pydantic.py
+-rw-r--r--   0        0        0     1835 2024-05-31 18:51:32.566246 ilcdlib-4.8.0/src/ilcdlib/const.py
+-rw-r--r--   0        0        0     4934 2024-05-31 18:51:32.566246 ilcdlib-4.8.0/src/ilcdlib/data/category_mapping/epdnorge.csv
+-rw-r--r--   0        0        0    51577 2024-05-31 18:51:32.566246 ilcdlib-4.8.0/src/ilcdlib/data/category_mapping/oekobaudat.csv
+-rw-r--r--   0        0        0   172140 2024-05-31 18:51:32.566246 ilcdlib-4.8.0/src/ilcdlib/data/ilcd_epd_ref.zip
+-rw-r--r--   0        0        0     6488 2024-05-31 18:51:32.566246 ilcdlib-4.8.0/src/ilcdlib/dto.py
+-rw-r--r--   0        0        0      837 2024-05-31 18:51:32.566246 ilcdlib-4.8.0/src/ilcdlib/entity/__init__.py
+-rw-r--r--   0        0        0     7064 2024-05-31 18:51:32.566246 ilcdlib-4.8.0/src/ilcdlib/entity/base_scope_set_reader.py
+-rw-r--r--   0        0        0     3361 2024-05-31 18:51:32.566246 ilcdlib-4.8.0/src/ilcdlib/entity/category.py
+-rw-r--r--   0        0        0     3052 2024-05-31 18:51:32.566246 ilcdlib-4.8.0/src/ilcdlib/entity/compliance.py
+-rw-r--r--   0        0        0     6003 2024-05-31 18:51:32.566246 ilcdlib-4.8.0/src/ilcdlib/entity/contact.py
+-rw-r--r--   0        0        0     4173 2024-05-31 18:51:32.566246 ilcdlib-4.8.0/src/ilcdlib/entity/exchage.py
+-rw-r--r--   0        0        0     8138 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/entity/flow.py
+-rw-r--r--   0        0        0     4224 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/entity/lcia.py
+-rw-r--r--   0        0        0     5213 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/entity/material.py
+-rw-r--r--   0        0        0     3930 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/entity/pcr.py
+-rw-r--r--   0        0        0     3437 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/entity/source.py
+-rw-r--r--   0        0        0     3788 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/entity/unit.py
+-rw-r--r--   0        0        0     3326 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/entity/validation.py
+-rw-r--r--   0        0        0      837 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/epd/__init__.py
+-rw-r--r--   0        0        0    10064 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/epd/cli.py
+-rw-r--r--   0        0        0      837 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/epd/dialect/__init__.py
+-rw-r--r--   0        0        0     6864 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/epd/dialect/environdec.py
+-rw-r--r--   0        0        0     2170 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/epd/dialect/epditaly.py
+-rw-r--r--   0        0        0     6425 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/epd/dialect/epdnorge.py
+-rw-r--r--   0        0        0     1329 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/epd/dialect/indata.py
+-rw-r--r--   0        0        0     2326 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/epd/dialect/itb.py
+-rw-r--r--   0        0        0     3876 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/epd/dialect/oekobaudat.py
+-rw-r--r--   0        0        0     3644 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/epd/factory.py
+-rw-r--r--   0        0        0    35677 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/epd/reader.py
+-rw-r--r--   0        0        0     2248 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/extension.py
+-rw-r--r--   0        0        0     7895 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/http_common.py
+-rw-r--r--   0        0        0      837 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/mapping/__init__.py
+-rw-r--r--   0        0        0    10680 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/mapping/category.py
+-rw-r--r--   0        0        0     3603 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/mapping/common.py
+-rw-r--r--   0        0        0     1168 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/mapping/compliance.py
+-rw-r--r--   0        0        0     1512 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/mapping/flows.py
+-rw-r--r--   0        0        0     3610 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/mapping/impacts.py
+-rw-r--r--   0        0        0     1651 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/mapping/indicators.py
+-rw-r--r--   0        0        0     1212 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/mapping/properties.py
+-rw-r--r--   0        0        0     6247 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/mapping/units.py
+-rw-r--r--   0        0        0      837 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/medium/__init__.py
+-rw-r--r--   0        0        0     7531 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/medium/archive.py
+-rw-r--r--   0        0        0     6496 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/medium/soda4lca.py
+-rw-r--r--   0        0        0        0 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/py.typed
+-rw-r--r--   0        0        0     1435 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/reference_data.py
+-rw-r--r--   0        0        0      837 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/sanitizing/__init__.py
+-rw-r--r--   0        0        0     1866 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/sanitizing/domain.py
+-rw-r--r--   0        0        0     1336 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/sanitizing/phone.py
+-rw-r--r--   0        0        0     1122 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/sanitizing/text.py
+-rw-r--r--   0        0        0      837 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/soda4lca/__init__.py
+-rw-r--r--   0        0        0    11347 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/soda4lca/api_client.py
+-rw-r--r--   0        0        0     2755 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/soda4lca/api_client_4x.py
+-rw-r--r--   0        0        0     1206 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/type.py
+-rw-r--r--   0        0        0     6465 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/utils.py
+-rw-r--r--   0        0        0     2399 2024-05-31 18:51:32.570246 ilcdlib-4.8.0/src/ilcdlib/xml_parser.py
+-rw-r--r--   0        0        0     6082 1970-01-01 00:00:00.000000 ilcdlib-4.8.0/PKG-INFO
```

### Comparing `ilcdlib-4.7.0/LICENSE` & `ilcdlib-4.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/README.md` & `ilcdlib-4.8.0/README.md`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/pyproject.toml` & `ilcdlib-4.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ilcdlib"
-version = "4.7.0"
+version = "4.8.0"
 license = "Apache-2.0"
 description = "A toolkit for reading and writing ILCD format and it's derivatives"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <open-source@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/ilcdlib"
 keywords = []
 classifiers = [
```

### Comparing `ilcdlib-4.7.0/src/ilcdlib/__init__.py` & `ilcdlib-4.8.0/src/ilcdlib/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/__main__.py` & `ilcdlib-4.8.0/src/ilcdlib/__main__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/__version__.py` & `ilcdlib-4.8.0/src/ilcdlib/__version__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/cli.py` & `ilcdlib-4.8.0/src/ilcdlib/cli.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/common.py` & `ilcdlib-4.8.0/src/ilcdlib/common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/compat/__init__.py` & `ilcdlib-4.8.0/src/ilcdlib/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/compat/pydantic.py` & `ilcdlib-4.8.0/src/ilcdlib/compat/pydantic.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/const.py` & `ilcdlib-4.8.0/src/ilcdlib/const.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/data/category_mapping/epdnorge.csv` & `ilcdlib-4.8.0/src/ilcdlib/data/category_mapping/epdnorge.csv`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/data/category_mapping/oekobaudat.csv` & `ilcdlib-4.8.0/src/ilcdlib/data/category_mapping/oekobaudat.csv`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/data/ilcd_epd_ref.zip` & `ilcdlib-4.8.0/src/ilcdlib/data/ilcd_epd_ref.zip`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/dto.py` & `ilcdlib-4.8.0/src/ilcdlib/dto.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/entity/__init__.py` & `ilcdlib-4.8.0/src/ilcdlib/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/entity/base_scope_set_reader.py` & `ilcdlib-4.8.0/src/ilcdlib/entity/base_scope_set_reader.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/entity/category.py` & `ilcdlib-4.8.0/src/ilcdlib/entity/category.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/entity/compliance.py` & `ilcdlib-4.8.0/src/ilcdlib/entity/compliance.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/entity/contact.py` & `ilcdlib-4.8.0/src/ilcdlib/entity/contact.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/entity/exchage.py` & `ilcdlib-4.8.0/src/ilcdlib/entity/exchage.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/entity/flow.py` & `ilcdlib-4.8.0/src/ilcdlib/entity/flow.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/entity/lcia.py` & `ilcdlib-4.8.0/src/ilcdlib/entity/lcia.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/entity/material.py` & `ilcdlib-4.8.0/src/ilcdlib/entity/material.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/entity/pcr.py` & `ilcdlib-4.8.0/src/ilcdlib/entity/pcr.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/entity/source.py` & `ilcdlib-4.8.0/src/ilcdlib/entity/source.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/entity/unit.py` & `ilcdlib-4.8.0/src/ilcdlib/entity/unit.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/entity/validation.py` & `ilcdlib-4.8.0/src/ilcdlib/entity/validation.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/epd/__init__.py` & `ilcdlib-4.8.0/src/ilcdlib/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/epd/cli.py` & `ilcdlib-4.8.0/src/ilcdlib/epd/cli.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/epd/dialect/__init__.py` & `ilcdlib-4.8.0/src/ilcdlib/epd/dialect/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/epd/dialect/environdec.py` & `ilcdlib-4.8.0/src/ilcdlib/epd/dialect/environdec.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/epd/dialect/epditaly.py` & `ilcdlib-4.8.0/src/ilcdlib/epd/dialect/epditaly.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/epd/dialect/epdnorge.py` & `ilcdlib-4.8.0/src/ilcdlib/epd/dialect/epdnorge.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 import datetime
 
+from openepd.model.pcr import Pcr
+
 from ilcdlib.dto import MappedCategory, OpenEpdIlcdOrg, ValidationDto
 from ilcdlib.epd.reader import IlcdEpdReader
 from ilcdlib.mapping.category import CsvCategoryMapper
 from ilcdlib.type import LangDef
 
 
 class EpdNorgeCategoryMapper(CsvCategoryMapper):
@@ -133,7 +135,18 @@
                 "common:shortDescription",
             ),
             ("en", None),
         )
         if developer:
             return OpenEpdIlcdOrg(name=developer)
         return super().get_data_entry_by(lang, base_url)
+
+    def get_pcr(self, lang: LangDef, base_url: str | None = None) -> Pcr | None:
+        """Return the PCR."""
+        pcr = super().get_pcr(lang, base_url)
+        if pcr is not None and pcr.name:
+            pcr.name = (
+                pcr.name.replace("Product descriptions and scenarios are based on", "")
+                .replace("This also applies for inorganic coatings", "")
+                .strip()
+            )
+        return pcr
```

### Comparing `ilcdlib-4.7.0/src/ilcdlib/epd/dialect/indata.py` & `ilcdlib-4.8.0/src/ilcdlib/epd/dialect/indata.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/epd/dialect/itb.py` & `ilcdlib-4.8.0/src/ilcdlib/epd/dialect/itb.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/epd/dialect/oekobaudat.py` & `ilcdlib-4.8.0/src/ilcdlib/epd/dialect/oekobaudat.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/epd/factory.py` & `ilcdlib-4.8.0/src/ilcdlib/epd/factory.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/epd/reader.py` & `ilcdlib-4.8.0/src/ilcdlib/epd/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import datetime
 import itertools
 from typing import IO, Type
 
 from openepd.model.common import Amount, Measurement
 from openepd.model.epd import Epd
 from openepd.model.lcia import Impacts, ImpactSet, OutputFlowSet, ResourceUseSet
+from openepd.model.pcr import Pcr
 from openepd.model.specs import Specs
 from openepd.model.standard import Standard
 
 from ilcdlib import const
 from ilcdlib.common import BaseIlcdMediumSpecificReader, IlcdXmlReader, OpenEpdEdpSupportReader
 from ilcdlib.const import IlcdDatasetType, IlcdTypeOfReview
 from ilcdlib.dto import (
@@ -604,14 +605,20 @@
     def get_program_operator_id(self) -> str | None:
         """Get document identifier assigned by program operator."""
         return self._get_text(
             self.epd_el_tree,
             ("process:administrativeInformation", "process:publicationAndOwnership", "common:registrationNumber"),
         )
 
+    def get_pcr(self, lang: LangDef, base_url: str | None = None) -> Pcr | None:
+        """Return the PCR."""
+        pcr_reader = self.get_pcr_reader()
+        pcr = pcr_reader.to_openepd_pcr(lang, base_url) if pcr_reader else None
+        return pcr
+
     def get_lcia_results_reader(self) -> IlcdLciaResultsReader | None:
         """Return the LCIA results reader."""
         element = self._get_el(
             self.epd_el_tree,
             ("process:LCIAResults",),
         )
         return self.lcia_results_reader_cls(element, self.data_provider) if element is not None else None
@@ -694,16 +701,14 @@
         )
         publisher_reader = self.get_publisher_reader()
         publisher = publisher_reader.to_openepd_org(lang, base_url, provider_domain) if publisher_reader else None
         program_operator_reader = self.get_program_operator_reader()
         program_operator = (
             program_operator_reader.to_openepd_org(lang, base_url, provider_domain) if program_operator_reader else None
         )
-        pcr_reader = self.get_pcr_reader()
-        pcr = pcr_reader.to_openepd_pcr(lang, base_url) if pcr_reader else None
         declared_unit = self.get_declared_unit()
         quantitative_props = self.get_quantitative_product_props_str(lang)
         own_ref = self.get_own_reference()
         product_name = self.get_product_name(lang)
         if product_name and quantitative_props:
             product_name += "; " + quantitative_props
         material_properties = self.get_material_properties()
@@ -755,15 +760,15 @@
             program_operator=program_operator,
             product_classes=product_classes,
             manufacturing_description=self.get_technology_description(lang),
             product_usage_description=self.get_technological_applicability(lang),
             lca_discussion=self.get_lca_discussion(lang),
             third_party_verifier=self.get_third_party_verifier(ilcd_validations),
             third_party_verifier_email=self.get_third_party_verifier_email(ilcd_validations),
-            pcr=pcr,
+            pcr=self.get_pcr(lang, base_url),
             declared_unit=declared_unit,
             impacts=self.get_impacts(scenario_names, lca_method=lcia_method),
             resource_uses=self.get_resource_uses(scenario_names),
             output_flows=self.get_output_flows(scenario_names),
             specs=specs,
             compliance=compliance,
         )
```

### Comparing `ilcdlib-4.7.0/src/ilcdlib/extension.py` & `ilcdlib-4.8.0/src/ilcdlib/extension.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/http_common.py` & `ilcdlib-4.8.0/src/ilcdlib/http_common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/mapping/__init__.py` & `ilcdlib-4.8.0/src/ilcdlib/mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/mapping/category.py` & `ilcdlib-4.8.0/src/ilcdlib/mapping/category.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/mapping/common.py` & `ilcdlib-4.8.0/src/ilcdlib/mapping/common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/mapping/compliance.py` & `ilcdlib-4.8.0/src/ilcdlib/mapping/compliance.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/mapping/flows.py` & `ilcdlib-4.8.0/src/ilcdlib/mapping/flows.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/mapping/impacts.py` & `ilcdlib-4.8.0/src/ilcdlib/mapping/impacts.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     }
 
 
 class ImpactsKeywordToOpenIdMapper(KeyValueMapper[str]):
     """Map keywords to openEPD impact names.""" ""
 
     KV = {
-        "gwp-biogenic": ["biogenic"],
         "gwp-luluc": ["luluc"],
         "gwp-nonCO2": ["CO2", "non fossil"],
         "ep-marine": ["marine"],
         "ep-fresh": ["freshwater", "fw"],
         "ep-terr": ["terrestrial"],
         "odp": ["odp", "ozone layer"],
         "ap": ["ap", "acidification"],
@@ -58,14 +57,15 @@
     }
 
 
 class ImpactsRegexToOpenIdMapper(RegexMapper[str]):
     """Map impact names using regex.""" ""
 
     PATTERNS = {
+        "gwp-biogenic": r"^(?!.*\b(non|except|IOBC)\b)(?=.*\b(biogenic)\b)(?=.*\b(gwp|global warming)\b).*$",
         "gwp-fossil": r"^(?!.*\bnon\b)(?=.*\b(fossil)\b)(?=.*\b(gwp|global warming)\b).*$",
         "gwp": r"^(?!.*\b(fossil|luluc|CO2|total)\b)(?=.*\b(gwp|global warming)\b).*$",
     }
 
 
 class DefaultImpactsToOpenIdMapper(BaseDataMapper[str, str]):
     """Map default impacts to openEPD impact names."""
```

### Comparing `ilcdlib-4.7.0/src/ilcdlib/mapping/indicators.py` & `ilcdlib-4.8.0/src/ilcdlib/mapping/indicators.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/mapping/properties.py` & `ilcdlib-4.8.0/src/ilcdlib/mapping/properties.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/mapping/units.py` & `ilcdlib-4.8.0/src/ilcdlib/mapping/units.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/medium/__init__.py` & `ilcdlib-4.8.0/src/ilcdlib/medium/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/medium/archive.py` & `ilcdlib-4.8.0/src/ilcdlib/medium/archive.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/medium/soda4lca.py` & `ilcdlib-4.8.0/src/ilcdlib/medium/soda4lca.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/reference_data.py` & `ilcdlib-4.8.0/src/ilcdlib/reference_data.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/sanitizing/__init__.py` & `ilcdlib-4.8.0/src/ilcdlib/sanitizing/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/sanitizing/domain.py` & `ilcdlib-4.8.0/src/ilcdlib/sanitizing/domain.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/sanitizing/phone.py` & `ilcdlib-4.8.0/src/ilcdlib/sanitizing/phone.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/sanitizing/text.py` & `ilcdlib-4.8.0/src/ilcdlib/sanitizing/text.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/soda4lca/__init__.py` & `ilcdlib-4.8.0/src/ilcdlib/soda4lca/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/soda4lca/api_client.py` & `ilcdlib-4.8.0/src/ilcdlib/soda4lca/api_client.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/soda4lca/api_client_4x.py` & `ilcdlib-4.8.0/src/ilcdlib/soda4lca/api_client_4x.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/type.py` & `ilcdlib-4.8.0/src/ilcdlib/type.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/utils.py` & `ilcdlib-4.8.0/src/ilcdlib/utils.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/src/ilcdlib/xml_parser.py` & `ilcdlib-4.8.0/src/ilcdlib/xml_parser.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.7.0/PKG-INFO` & `ilcdlib-4.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilcdlib
-Version: 4.7.0
+Version: 4.8.0
 Summary: A toolkit for reading and writing ILCD format and it's derivatives
 Home-page: https://github.com/cchangelabs/ilcdlib
 License: Apache-2.0
 Author: C-Change Labs
 Author-email: support@c-change-labs.com
 Maintainer: C-Change Labs
 Maintainer-email: open-source@c-change-labs.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ilcdlib Version: 4.7.0 Summary: A toolkit for
+Metadata-Version: 2.1 Name: ilcdlib Version: 4.8.0 Summary: A toolkit for
 reading and writing ILCD format and it's derivatives Home-page: https://
 github.com/cchangelabs/ilcdlib License: Apache-2.0 Author: C-Change Labs
 Author-email: support@c-change-labs.com Maintainer: C-Change Labs Maintainer-
 email: open-source@c-change-labs.com Requires-Python: >=3.11,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

