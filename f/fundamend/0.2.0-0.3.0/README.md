# Comparing `tmp/fundamend-0.2.0.tar.gz` & `tmp/fundamend-0.3.0.tar.gz`

## Comparing `fundamend-0.2.0.tar` & `fundamend-0.3.0.tar`

### file list

```diff
@@ -1,43 +1,49 @@
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 fundamend-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 fundamend-0.2.0/README.md
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 fundamend-0.2.0/domain-specific-terms.txt
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fundamend-0.2.0/requirements.txt
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 fundamend-0.2.0/tox.ini
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 fundamend-0.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 fundamend-0.2.0/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 fundamend-0.2.0/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 fundamend-0.2.0/.github/workflows/dev_test.yml
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fundamend-0.2.0/.github/workflows/formatting.yml
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fundamend-0.2.0/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 fundamend-0.2.0/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 fundamend-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 fundamend-0.2.0/.github/workflows/pythonlint.yml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 fundamend-0.2.0/.github/workflows/unittests.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fundamend-0.2.0/dev_requirements/requirements-coverage.in
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 fundamend-0.2.0/dev_requirements/requirements-coverage.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fundamend-0.2.0/dev_requirements/requirements-formatting.in
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 fundamend-0.2.0/dev_requirements/requirements-formatting.txt
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 fundamend-0.2.0/dev_requirements/requirements-linting.in
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fundamend-0.2.0/dev_requirements/requirements-linting.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 fundamend-0.2.0/dev_requirements/requirements-packaging.in
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 fundamend-0.2.0/dev_requirements/requirements-packaging.txt
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 fundamend-0.2.0/dev_requirements/requirements-spell_check.in
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 fundamend-0.2.0/dev_requirements/requirements-spell_check.txt
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 fundamend-0.2.0/dev_requirements/requirements-tests.in
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fundamend-0.2.0/dev_requirements/requirements-tests.txt
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 fundamend-0.2.0/dev_requirements/requirements-type_check.in
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 fundamend-0.2.0/dev_requirements/requirements-type_check.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fundamend-0.2.0/src/_fundamend_version.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 fundamend-0.2.0/src/fundamend/__init__.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 fundamend-0.2.0/src/fundamend/py.typed
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 fundamend-0.2.0/src/fundamend/models/__init__.py
--rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 fundamend-0.2.0/src/fundamend/models/anwendungshandbuch.py
--rw-r--r--   0        0        0     7599 2020-02-02 00:00:00.000000 fundamend-0.2.0/src/fundamend/models/messageimplementationguide.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 fundamend-0.2.0/src/fundamend/reader/__init__.py
--rw-r--r--   0        0        0     9129 2020-02-02 00:00:00.000000 fundamend-0.2.0/src/fundamend/reader/ahbreader.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 fundamend-0.2.0/src/fundamend/reader/element_distinction.py
--rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 fundamend-0.2.0/src/fundamend/reader/migreader.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fundamend-0.2.0/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 fundamend-0.2.0/LICENSE
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 fundamend-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 fundamend-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 fundamend-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     5339 2020-02-02 00:00:00.000000 fundamend-0.3.0/README.md
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 fundamend-0.3.0/domain-specific-terms.txt
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fundamend-0.3.0/requirements.txt
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 fundamend-0.3.0/tox.ini
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 fundamend-0.3.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 fundamend-0.3.0/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 fundamend-0.3.0/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 fundamend-0.3.0/.github/workflows/dev_test.yml
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fundamend-0.3.0/.github/workflows/formatting.yml
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fundamend-0.3.0/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 fundamend-0.3.0/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 fundamend-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 fundamend-0.3.0/.github/workflows/pythonlint.yml
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 fundamend-0.3.0/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fundamend-0.3.0/dev_requirements/requirements-coverage.in
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 fundamend-0.3.0/dev_requirements/requirements-coverage.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fundamend-0.3.0/dev_requirements/requirements-formatting.in
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 fundamend-0.3.0/dev_requirements/requirements-formatting.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 fundamend-0.3.0/dev_requirements/requirements-linting.in
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fundamend-0.3.0/dev_requirements/requirements-linting.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 fundamend-0.3.0/dev_requirements/requirements-packaging.in
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 fundamend-0.3.0/dev_requirements/requirements-packaging.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 fundamend-0.3.0/dev_requirements/requirements-pydantic.in
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 fundamend-0.3.0/dev_requirements/requirements-pydantic.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 fundamend-0.3.0/dev_requirements/requirements-spell_check.in
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 fundamend-0.3.0/dev_requirements/requirements-spell_check.txt
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 fundamend-0.3.0/dev_requirements/requirements-tests.in
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fundamend-0.3.0/dev_requirements/requirements-tests.txt
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 fundamend-0.3.0/dev_requirements/requirements-type_check.in
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 fundamend-0.3.0/dev_requirements/requirements-type_check.txt
+-rw-r--r--   0        0        0    10723 2020-02-02 00:00:00.000000 fundamend-0.3.0/json_schemas/Anwendungshandbuch.schema.json
+-rw-r--r--   0        0        0    10770 2020-02-02 00:00:00.000000 fundamend-0.3.0/json_schemas/MessageImplementationGuide.schema.json
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 fundamend-0.3.0/json_schemas/generate_json_schemas.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fundamend-0.3.0/src/_fundamend_version.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 fundamend-0.3.0/src/fundamend/__init__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 fundamend-0.3.0/src/fundamend/py.typed
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 fundamend-0.3.0/src/fundamend/models/__init__.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 fundamend-0.3.0/src/fundamend/models/_dataclass_wrapper.py
+-rw-r--r--   0        0        0     6330 2020-02-02 00:00:00.000000 fundamend-0.3.0/src/fundamend/models/anwendungshandbuch.py
+-rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 fundamend-0.3.0/src/fundamend/models/messageimplementationguide.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 fundamend-0.3.0/src/fundamend/reader/__init__.py
+-rw-r--r--   0        0        0     9129 2020-02-02 00:00:00.000000 fundamend-0.3.0/src/fundamend/reader/ahbreader.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 fundamend-0.3.0/src/fundamend/reader/element_distinction.py
+-rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 fundamend-0.3.0/src/fundamend/reader/migreader.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fundamend-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 fundamend-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 fundamend-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6366 2020-02-02 00:00:00.000000 fundamend-0.3.0/PKG-INFO
```

### Comparing `fundamend-0.2.0/.pre-commit-config.yaml` & `fundamend-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fundamend-0.2.0/README.md` & `fundamend-0.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -75,14 +75,62 @@
     "25008",
     "25009",
 }
 ```
 
 Die vollständigen Beispiele finden sich in den [unittests](unittests).
 
+### Verwendung mit Pydantic
+Per default verwendet fundamend die [dataclasses aus der Python-Standardlibrary](https://docs.python.org/3/library/dataclasses.html).
+Es lässt sich aber auch direkt mit [Pydantic](https://docs.pydantic.dev/latest/) und den [Pydantic dataclasses](https://docs.pydantic.dev/2.7/concepts/dataclasses/) verwenden.
+Wenn entweder pydantic schon installiert ist, oder mittels
+```bash
+pip install fundamend[pydantic]
+```
+mit installiert wird, dann sind Datenmodelle, die von `AhbReader` und `MigReader` zurückgegeben werden, automatisch pydantic Objekte.
+
+Mit Pydantic können die Ergebnisse auch leicht bspw. als JSON exportiert werden:
+```python
+from pathlib import Path
+
+from pydantic import RootModel
+from fundamend import Anwendungshandbuch, AhbReader
+
+ahb = AhbReader(Path("UTILTS_AHB_1.1d_Konsultationsfassung_2024_04_02.xml")).read()
+ahb_json = RootModel[Anwendungshandbuch](ahb).model_dump(mode="json")
+```
+
+Das Ergebnis sieht dann so aus:
+```json
+{
+  "veroeffentlichungsdatum": "2024-04-02",
+  "autor": "BDEW",
+  "versionsnummer": "1.1d",
+  "anwendungsfaelle": [
+    {
+      "pruefidentifikator": "25001",
+      "beschreibung": "Berechnungsformel",
+      "kommunikation_von": "NB an MSB / LF",
+      "format": "AWF",
+      "segments": [
+        {
+          "id": "UNH",
+          "name": "Nachrichten-Kopfsegment",
+          "number": "00001",
+          "ahb_status": "Muss",
+          "data_elements": [
+            {
+              "id": "D_0062",
+              "name": "Nachrichten-Referenznummer",
+              "codes": []
+            },
+```
+
+### JSON Schemas
+Das fundamend Datenmodell ist auch als JSON Schema verfügbar: [`json_schemas`](json_schemas).
 
 ## Verwendung und Mitwirken
 Der Code ist MIT-lizenziert und kann daher frei verwendet werden.
 Wir freuen uns über Pull Requests an den main-Branch dieses Repositories.
 
 ## Hochfrequenz
 Die [Hochfrequenz Unternehmensberatung GmbH](https://www.hochfrequenz.de) ist eine Beratung für Energieversorger im deutschsprachigen Raum.
```

### Comparing `fundamend-0.2.0/tox.ini` & `fundamend-0.3.0/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
 [testenv:type_check]
 # the type_check environment checks the type hints using mypy
 setenv = PYTHONPATH = {toxinidir}/src
 deps =
     {[testenv:tests]deps}
     -r dev_requirements/requirements-type_check.txt
+    -r dev_requirements/requirements-pydantic.txt
 commands =
     mypy --show-error-codes src/fundamend --strict
     mypy --show-error-codes unittests --strict
     # add single files (ending with .py) or packages here
 
 [testenv:spell_check]
 # the spellcheck environment checks the code for typos
@@ -54,14 +55,15 @@
 
 [testenv:coverage]
 # the coverage environment is called by the Github Action that runs the coverage measurement
 changedir = unittests
 deps =
     {[testenv:tests]deps}
     -r dev_requirements/requirements-coverage.txt
+    -r dev_requirements/requirements-pydantic.txt
 setenv = PYTHONPATH = {toxinidir}/src
 commands =
     coverage run -m pytest --basetemp={envtmpdir} {posargs}
     coverage html --omit .tox/*,unittests/*
     coverage report --fail-under 95 --omit .tox/*,unittests/*
 
 [testenv:compile_requirements]
@@ -89,7 +91,15 @@
 [testenv:test_packaging]
 skip_install = true
 deps =
     -r dev_requirements/requirements-packaging.txt
 commands =
     python -m build
     twine check dist/*
+
+[testenv:json_schemas]
+usedevelop = True
+deps =
+    -r requirements.txt
+    -r dev_requirements/requirements-pydantictxt
+commands =
+    python json_schemas/generate_json_schemas.py
```

### Comparing `fundamend-0.2.0/.github/dependabot.yml` & `fundamend-0.3.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `fundamend-0.2.0/.github/workflows/coverage.yml` & `fundamend-0.3.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `fundamend-0.2.0/.github/workflows/dependabot_automerge.yml` & `fundamend-0.3.0/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `fundamend-0.2.0/.github/workflows/dev_test.yml` & `fundamend-0.3.0/.github/workflows/dev_test.yml`

 * *Files identical despite different names*

### Comparing `fundamend-0.2.0/.github/workflows/formatting.yml` & `fundamend-0.3.0/.github/workflows/formatting.yml`

 * *Files identical despite different names*

### Comparing `fundamend-0.2.0/.github/workflows/packaging_test.yml` & `fundamend-0.3.0/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `fundamend-0.2.0/.github/workflows/python-publish.yml` & `fundamend-0.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fundamend-0.2.0/.github/workflows/pythonlint.yml` & `fundamend-0.3.0/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `fundamend-0.2.0/dev_requirements/requirements-packaging.txt` & `fundamend-0.3.0/dev_requirements/requirements-packaging.txt`

 * *Files identical despite different names*

### Comparing `fundamend-0.2.0/src/fundamend/models/anwendungshandbuch.py` & `fundamend-0.3.0/src/fundamend/models/anwendungshandbuch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """"model classes for Anwendungshandbücher (AHB)"""
 
 # pylint:disable=duplicate-code
 # the structures are similar, still we decided against inheritance, so there's naturally a little bit of duplication
 
-from dataclasses import dataclass
 from datetime import date
 
+from ._dataclass_wrapper import dataclass
+
 
 @dataclass(kw_only=True, eq=True, frozen=True)
 class Code:
     """
     a single code element inside an AHB DataElement
     """
```

### Comparing `fundamend-0.2.0/src/fundamend/models/messageimplementationguide.py` & `fundamend-0.3.0/src/fundamend/models/messageimplementationguide.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """classes that represent MIGs"""
 
-from dataclasses import dataclass
 from datetime import date
 from enum import StrEnum
 
+from ._dataclass_wrapper import dataclass
+
 # I didn't invent the data model ;)
 # pylint:disable=too-many-instance-attributes
 
 
 class MigStatus(StrEnum):
     """
     status of a MIG element
```

### Comparing `fundamend-0.2.0/src/fundamend/reader/ahbreader.py` & `fundamend-0.3.0/src/fundamend/reader/ahbreader.py`

 * *Files identical despite different names*

### Comparing `fundamend-0.2.0/src/fundamend/reader/element_distinction.py` & `fundamend-0.3.0/src/fundamend/reader/element_distinction.py`

 * *Files identical despite different names*

### Comparing `fundamend-0.2.0/src/fundamend/reader/migreader.py` & `fundamend-0.3.0/src/fundamend/reader/migreader.py`

 * *Files identical despite different names*

### Comparing `fundamend-0.2.0/.gitignore` & `fundamend-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fundamend-0.2.0/LICENSE` & `fundamend-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fundamend-0.2.0/pyproject.toml` & `fundamend-0.3.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -12,17 +12,22 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
-dependencies = []     # add all the dependencies here
+dependencies = [] # add all the fundamend dependencies here, None so far
 dynamic = ["readme", "version"]
 
+[project.optional-dependencies]
+pydantic = ["pydantic>=2"] # if you install fundamend[pydantic], the dataclasses from pydantic will be used
+
+
+
 [project.urls]
 Changelog = "https://github.com/Hochfrequenz/xml-fundamend-python/releases"
 Homepage = "https://github.com/Hochfrequenz/xml-fundamend-python"
 
 [tool.black]
 line-length = 120
 target_version = ["py311", "py312"]
```

### Comparing `fundamend-0.2.0/PKG-INFO` & `fundamend-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fundamend
-Version: 0.2.0
+Version: 0.3.0
 Summary: XML basierte Formate und DatemModelle für die Energiewirtschaft in Deutschland
 Project-URL: Changelog, https://github.com/Hochfrequenz/xml-fundamend-python/releases
 Project-URL: Homepage, https://github.com/Hochfrequenz/xml-fundamend-python
 Author-email: Hochfrequenz Unternehmensberatung GmbH <info+github@hochfrequenz.de>
 License: MIT
 License-File: LICENSE
 Keywords: AHB,BDEW,MIG,Marktkommunikation,XML
@@ -14,14 +14,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.11
+Provides-Extra: pydantic
+Requires-Dist: pydantic>=2; extra == 'pydantic'
 Description-Content-Type: text/markdown
 
 # FUNDAMEND - Formate und DAtenModelle für die ENergiewirtschaft in Deutschland
 
 Dieses Repository enthält das Python-Paket `fundamend`, das XML-basierte MIGs und AHBs als Python-Objekte einliest.
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
@@ -97,14 +99,62 @@
     "25008",
     "25009",
 }
 ```
 
 Die vollständigen Beispiele finden sich in den [unittests](unittests).
 
+### Verwendung mit Pydantic
+Per default verwendet fundamend die [dataclasses aus der Python-Standardlibrary](https://docs.python.org/3/library/dataclasses.html).
+Es lässt sich aber auch direkt mit [Pydantic](https://docs.pydantic.dev/latest/) und den [Pydantic dataclasses](https://docs.pydantic.dev/2.7/concepts/dataclasses/) verwenden.
+Wenn entweder pydantic schon installiert ist, oder mittels
+```bash
+pip install fundamend[pydantic]
+```
+mit installiert wird, dann sind Datenmodelle, die von `AhbReader` und `MigReader` zurückgegeben werden, automatisch pydantic Objekte.
+
+Mit Pydantic können die Ergebnisse auch leicht bspw. als JSON exportiert werden:
+```python
+from pathlib import Path
+
+from pydantic import RootModel
+from fundamend import Anwendungshandbuch, AhbReader
+
+ahb = AhbReader(Path("UTILTS_AHB_1.1d_Konsultationsfassung_2024_04_02.xml")).read()
+ahb_json = RootModel[Anwendungshandbuch](ahb).model_dump(mode="json")
+```
+
+Das Ergebnis sieht dann so aus:
+```json
+{
+  "veroeffentlichungsdatum": "2024-04-02",
+  "autor": "BDEW",
+  "versionsnummer": "1.1d",
+  "anwendungsfaelle": [
+    {
+      "pruefidentifikator": "25001",
+      "beschreibung": "Berechnungsformel",
+      "kommunikation_von": "NB an MSB / LF",
+      "format": "AWF",
+      "segments": [
+        {
+          "id": "UNH",
+          "name": "Nachrichten-Kopfsegment",
+          "number": "00001",
+          "ahb_status": "Muss",
+          "data_elements": [
+            {
+              "id": "D_0062",
+              "name": "Nachrichten-Referenznummer",
+              "codes": []
+            },
+```
+
+### JSON Schemas
+Das fundamend Datenmodell ist auch als JSON Schema verfügbar: [`json_schemas`](json_schemas).
 
 ## Verwendung und Mitwirken
 Der Code ist MIT-lizenziert und kann daher frei verwendet werden.
 Wir freuen uns über Pull Requests an den main-Branch dieses Repositories.
 
 ## Hochfrequenz
 Die [Hochfrequenz Unternehmensberatung GmbH](https://www.hochfrequenz.de) ist eine Beratung für Energieversorger im deutschsprachigen Raum.
```

