# Comparing `tmp/fundamend-0.1.1.tar.gz` & `tmp/fundamend-0.2.0.tar.gz`

## Comparing `fundamend-0.1.1.tar` & `fundamend-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,43 @@
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 fundamend-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 fundamend-0.1.1/README.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fundamend-0.1.1/domain-specific-terms.txt
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fundamend-0.1.1/requirements.txt
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 fundamend-0.1.1/tox.ini
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 fundamend-0.1.1/.github/dependabot.yml
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 fundamend-0.1.1/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 fundamend-0.1.1/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 fundamend-0.1.1/.github/workflows/dev_test.yml
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fundamend-0.1.1/.github/workflows/formatting.yml
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fundamend-0.1.1/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 fundamend-0.1.1/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 fundamend-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 fundamend-0.1.1/.github/workflows/pythonlint.yml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 fundamend-0.1.1/.github/workflows/unittests.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fundamend-0.1.1/dev_requirements/requirements-coverage.in
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 fundamend-0.1.1/dev_requirements/requirements-coverage.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fundamend-0.1.1/dev_requirements/requirements-formatting.in
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 fundamend-0.1.1/dev_requirements/requirements-formatting.txt
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 fundamend-0.1.1/dev_requirements/requirements-linting.in
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fundamend-0.1.1/dev_requirements/requirements-linting.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 fundamend-0.1.1/dev_requirements/requirements-packaging.in
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 fundamend-0.1.1/dev_requirements/requirements-packaging.txt
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 fundamend-0.1.1/dev_requirements/requirements-spell_check.in
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 fundamend-0.1.1/dev_requirements/requirements-spell_check.txt
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 fundamend-0.1.1/dev_requirements/requirements-tests.in
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fundamend-0.1.1/dev_requirements/requirements-tests.txt
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 fundamend-0.1.1/dev_requirements/requirements-type_check.in
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 fundamend-0.1.1/dev_requirements/requirements-type_check.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fundamend-0.1.1/src/_fundamend_version.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 fundamend-0.1.1/src/fundamend/__init__.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 fundamend-0.1.1/src/fundamend/py.typed
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 fundamend-0.1.1/src/fundamend/models/__init__.py
--rw-r--r--   0        0        0     7599 2020-02-02 00:00:00.000000 fundamend-0.1.1/src/fundamend/models/messageimplementationguide.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 fundamend-0.1.1/src/fundamend/reader/__init__.py
--rw-r--r--   0        0        0     7492 2020-02-02 00:00:00.000000 fundamend-0.1.1/src/fundamend/reader/migreader.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fundamend-0.1.1/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 fundamend-0.1.1/LICENSE
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 fundamend-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 fundamend-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 fundamend-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 fundamend-0.2.0/README.md
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 fundamend-0.2.0/domain-specific-terms.txt
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fundamend-0.2.0/requirements.txt
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 fundamend-0.2.0/tox.ini
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 fundamend-0.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 fundamend-0.2.0/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 fundamend-0.2.0/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 fundamend-0.2.0/.github/workflows/dev_test.yml
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fundamend-0.2.0/.github/workflows/formatting.yml
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fundamend-0.2.0/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 fundamend-0.2.0/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 fundamend-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 fundamend-0.2.0/.github/workflows/pythonlint.yml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 fundamend-0.2.0/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fundamend-0.2.0/dev_requirements/requirements-coverage.in
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 fundamend-0.2.0/dev_requirements/requirements-coverage.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fundamend-0.2.0/dev_requirements/requirements-formatting.in
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 fundamend-0.2.0/dev_requirements/requirements-formatting.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 fundamend-0.2.0/dev_requirements/requirements-linting.in
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fundamend-0.2.0/dev_requirements/requirements-linting.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 fundamend-0.2.0/dev_requirements/requirements-packaging.in
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 fundamend-0.2.0/dev_requirements/requirements-packaging.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 fundamend-0.2.0/dev_requirements/requirements-spell_check.in
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 fundamend-0.2.0/dev_requirements/requirements-spell_check.txt
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 fundamend-0.2.0/dev_requirements/requirements-tests.in
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fundamend-0.2.0/dev_requirements/requirements-tests.txt
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 fundamend-0.2.0/dev_requirements/requirements-type_check.in
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 fundamend-0.2.0/dev_requirements/requirements-type_check.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fundamend-0.2.0/src/_fundamend_version.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 fundamend-0.2.0/src/fundamend/__init__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 fundamend-0.2.0/src/fundamend/py.typed
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 fundamend-0.2.0/src/fundamend/models/__init__.py
+-rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 fundamend-0.2.0/src/fundamend/models/anwendungshandbuch.py
+-rw-r--r--   0        0        0     7599 2020-02-02 00:00:00.000000 fundamend-0.2.0/src/fundamend/models/messageimplementationguide.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 fundamend-0.2.0/src/fundamend/reader/__init__.py
+-rw-r--r--   0        0        0     9129 2020-02-02 00:00:00.000000 fundamend-0.2.0/src/fundamend/reader/ahbreader.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 fundamend-0.2.0/src/fundamend/reader/element_distinction.py
+-rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 fundamend-0.2.0/src/fundamend/reader/migreader.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fundamend-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 fundamend-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 fundamend-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 fundamend-0.2.0/PKG-INFO
```

### Comparing `fundamend-0.1.1/.pre-commit-config.yaml` & `fundamend-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fundamend-0.1.1/README.md` & `fundamend-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 # FUNDAMEND - Formate und DAtenModelle für die ENergiewirtschaft in Deutschland
 
-Dieses Repository enthält das Python-Paket `fundamend`.
+Dieses Repository enthält das Python-Paket `fundamend`, das XML-basierte MIGs und AHBs als Python-Objekte einliest.
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
 ![Python Versions (officially) supported](https://img.shields.io/pypi/pyversions/fundamend.svg)
 ![Pypi status badge](https://img.shields.io/pypi/v/fundamend)
 ![Unittests status badge](https://github.com/Hochfrequenz/xml-fundamend-python/workflows/Unittests/badge.svg)
 ![Coverage status badge](https://github.com/Hochfrequenz/xml-fundamend-python/workflows/Coverage/badge.svg)
 ![Linting status badge](https://github.com/Hochfrequenz/xml-fundamend-python/workflows/Linting/badge.svg)
 ![Black status badge](https://github.com/Hochfrequenz/xml-fundamend-python/workflows/Formatting/badge.svg)
 
 ## Sinn und Zweck
 Seit 2024 bietet der BDEW (endlich) maschinenlesbare MIG- und AHB-Spezifikationen an, wo zuvor nur PDF oder Word-Dateien veröffentlicht wurden.
 Das ist ein wichtiger Schritt für eine echte Digitalisierung der Marktkommunikation im deutschen Energiemarkt.
 
-Die nun maschinenlesbaren Informationen über den Aufgabe von EDIFACT-Nachrichten sind XML-basiert.
+Die nun maschinenlesbaren Informationen über den Aufbau von EDIFACT-Nachrichten sind XML-basiert.
 
 Dieses Repository enthält ein kleines Python-Paket, das die XML-Dateien einliest und als vollständig typisierte Python-Objekte zur Verfügung stellt, damit sich niemand mit XML herumschlagen muss.
 Das ist alles.
 
+Hochfrequenz stellt mit [migmose](https://github.com/Hochfrequenz/migmose) auch ein Tool bereit, das maschinenlesbare MIGs aus `.docx`-Dateien scraped.
+
 ## Installation und Verwendung
 Das Paket ist auf PyPI verfügbar und kann mit pip installiert werden:
 ```bash
 pip install fundamend
 ```
 
+### Message Implementation Guides (MIG) deserialisieren
 ```python
 from pathlib import Path
 from fundamend import MigReader, MessageImplementationGuide
 
 # Angenommen, mig_utilts.xml enthält:
 # <?xml version="1.0" encoding="UTF-8"?>
 # <M_UTILTS Versionsnummer="1.1c"
@@ -39,16 +42,47 @@
 
 reader = MigReader(Path("pfad/zur/mig_utils.xml"))
 mig = reader.read()
 assert isinstance(mig, MessageImplementationGuide)
 assert mig.format == "UTILTS"
 ```
 
-Aktuell (Version 0.1) können nur MIGs gelesen werden.
-Der AHB-Teil soll aber folgen.
+### Anwendungshandbuch (AHB) deserialisieren
+```python
+from pathlib import Path
+from fundamend import AhbReader, Anwendungshandbuch
+
+# Angenommen, ahb_utilts.xml enthält:
+# <?xml version="1.0" encoding="UTF-8"?>
+# <AHB Versionsnummer="1.1d"
+#    Veroeffentlichungsdatum="02.04.2024"
+#    Author="BDEW">
+#    <AWF Pruefidentifikator="25001" Beschreibung="Berechnungsformel" Kommunikation_von="NB an MSB / LF">
+#    ...
+#   </AWF>
+# </AHB>
+
+reader = AhbReader(Path("pfad/zur/ahb_utils.xml"))
+ahb = reader.read()
+assert isinstance(ahb, Anwendungshandbuch)
+assert {awf.pruefidentifikator for awf in ahb.anwendungsfaelle} == {
+    "25001",
+    "25002",
+    "25003",
+    "25004",
+    "25005",
+    "25006",
+    "25007",
+    "25008",
+    "25009",
+}
+```
+
+Die vollständigen Beispiele finden sich in den [unittests](unittests).
+
 
 ## Verwendung und Mitwirken
 Der Code ist MIT-lizenziert und kann daher frei verwendet werden.
 Wir freuen uns über Pull Requests an den main-Branch dieses Repositories.
 
 ## Hochfrequenz
 Die [Hochfrequenz Unternehmensberatung GmbH](https://www.hochfrequenz.de) ist eine Beratung für Energieversorger im deutschsprachigen Raum.
```

### Comparing `fundamend-0.1.1/tox.ini` & `fundamend-0.2.0/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 deps =
     {[testenv:tests]deps}
     -r dev_requirements/requirements-coverage.txt
 setenv = PYTHONPATH = {toxinidir}/src
 commands =
     coverage run -m pytest --basetemp={envtmpdir} {posargs}
     coverage html --omit .tox/*,unittests/*
-    coverage report --fail-under 80 --omit .tox/*,unittests/*
+    coverage report --fail-under 95 --omit .tox/*,unittests/*
 
 [testenv:compile_requirements]
 deps =
     pip-compile-multi
 commands =
     pip-compile-multi -d dev_requirements --autoresolve
```

### Comparing `fundamend-0.1.1/.github/dependabot.yml` & `fundamend-0.2.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `fundamend-0.1.1/.github/workflows/coverage.yml` & `fundamend-0.2.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `fundamend-0.1.1/.github/workflows/dependabot_automerge.yml` & `fundamend-0.2.0/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `fundamend-0.1.1/.github/workflows/dev_test.yml` & `fundamend-0.2.0/.github/workflows/dev_test.yml`

 * *Files identical despite different names*

### Comparing `fundamend-0.1.1/.github/workflows/formatting.yml` & `fundamend-0.2.0/.github/workflows/formatting.yml`

 * *Files identical despite different names*

### Comparing `fundamend-0.1.1/.github/workflows/packaging_test.yml` & `fundamend-0.2.0/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `fundamend-0.1.1/.github/workflows/python-publish.yml` & `fundamend-0.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fundamend-0.1.1/.github/workflows/pythonlint.yml` & `fundamend-0.2.0/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `fundamend-0.1.1/.github/workflows/unittests.yml` & `fundamend-0.2.0/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `fundamend-0.1.1/dev_requirements/requirements-packaging.txt` & `fundamend-0.2.0/dev_requirements/requirements-packaging.txt`

 * *Files identical despite different names*

### Comparing `fundamend-0.1.1/src/fundamend/models/messageimplementationguide.py` & `fundamend-0.2.0/src/fundamend/models/messageimplementationguide.py`

 * *Files identical despite different names*

### Comparing `fundamend-0.1.1/src/fundamend/reader/migreader.py` & `fundamend-0.2.0/src/fundamend/reader/migreader.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,49 +11,21 @@
     DataElement,
     DataElementGroup,
     MessageImplementationGuide,
     MigStatus,
     Segment,
     SegmentGroup,
 )
-
-
-def _is_segment_group(element: ET.Element) -> bool:
-    """
-    returns True if the given element is a segment group
-    """
-    return element.tag.startswith("G_SG")
-
-
-def _is_segment(element: ET.Element) -> bool:
-    """
-    returns True if the given element is a segment
-    """
-    return element.tag.startswith("S_")
-
-
-def _is_data_element_group(element: ET.Element) -> bool:
-    """
-    returns True if the given element is a data element group
-    """
-    return element.tag.startswith("C_")
-
-
-def _is_data_element(element: ET.Element) -> bool:
-    """
-    returns True if the given element is a data element
-    """
-    return element.tag.startswith("D_")
-
-
-def _is_code(element: ET.Element) -> bool:
-    """
-    returns True if the given element is a code
-    """
-    return element.tag == "Code"
+from fundamend.reader.element_distinction import (
+    _is_code,
+    _is_data_element,
+    _is_data_element_group,
+    _is_segment,
+    _is_segment_group,
+)
 
 
 def _to_code(element: ET.Element) -> Code:
     assert _is_code(element)
     return Code(name=element.attrib["Name"], description=element.attrib["Description"] or None, value=element.text)
```

### Comparing `fundamend-0.1.1/.gitignore` & `fundamend-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fundamend-0.1.1/LICENSE` & `fundamend-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fundamend-0.1.1/pyproject.toml` & `fundamend-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fundamend-0.1.1/PKG-INFO` & `fundamend-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fundamend
-Version: 0.1.1
+Version: 0.2.0
 Summary: XML basierte Formate und DatemModelle für die Energiewirtschaft in Deutschland
 Project-URL: Changelog, https://github.com/Hochfrequenz/xml-fundamend-python/releases
 Project-URL: Homepage, https://github.com/Hochfrequenz/xml-fundamend-python
 Author-email: Hochfrequenz Unternehmensberatung GmbH <info+github@hochfrequenz.de>
 License: MIT
 License-File: LICENSE
 Keywords: AHB,BDEW,MIG,Marktkommunikation,XML
@@ -18,39 +18,42 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # FUNDAMEND - Formate und DAtenModelle für die ENergiewirtschaft in Deutschland
 
-Dieses Repository enthält das Python-Paket `fundamend`.
+Dieses Repository enthält das Python-Paket `fundamend`, das XML-basierte MIGs und AHBs als Python-Objekte einliest.
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
 ![Python Versions (officially) supported](https://img.shields.io/pypi/pyversions/fundamend.svg)
 ![Pypi status badge](https://img.shields.io/pypi/v/fundamend)
 ![Unittests status badge](https://github.com/Hochfrequenz/xml-fundamend-python/workflows/Unittests/badge.svg)
 ![Coverage status badge](https://github.com/Hochfrequenz/xml-fundamend-python/workflows/Coverage/badge.svg)
 ![Linting status badge](https://github.com/Hochfrequenz/xml-fundamend-python/workflows/Linting/badge.svg)
 ![Black status badge](https://github.com/Hochfrequenz/xml-fundamend-python/workflows/Formatting/badge.svg)
 
 ## Sinn und Zweck
 Seit 2024 bietet der BDEW (endlich) maschinenlesbare MIG- und AHB-Spezifikationen an, wo zuvor nur PDF oder Word-Dateien veröffentlicht wurden.
 Das ist ein wichtiger Schritt für eine echte Digitalisierung der Marktkommunikation im deutschen Energiemarkt.
 
-Die nun maschinenlesbaren Informationen über den Aufgabe von EDIFACT-Nachrichten sind XML-basiert.
+Die nun maschinenlesbaren Informationen über den Aufbau von EDIFACT-Nachrichten sind XML-basiert.
 
 Dieses Repository enthält ein kleines Python-Paket, das die XML-Dateien einliest und als vollständig typisierte Python-Objekte zur Verfügung stellt, damit sich niemand mit XML herumschlagen muss.
 Das ist alles.
 
+Hochfrequenz stellt mit [migmose](https://github.com/Hochfrequenz/migmose) auch ein Tool bereit, das maschinenlesbare MIGs aus `.docx`-Dateien scraped.
+
 ## Installation und Verwendung
 Das Paket ist auf PyPI verfügbar und kann mit pip installiert werden:
 ```bash
 pip install fundamend
 ```
 
+### Message Implementation Guides (MIG) deserialisieren
 ```python
 from pathlib import Path
 from fundamend import MigReader, MessageImplementationGuide
 
 # Angenommen, mig_utilts.xml enthält:
 # <?xml version="1.0" encoding="UTF-8"?>
 # <M_UTILTS Versionsnummer="1.1c"
@@ -61,16 +64,47 @@
 
 reader = MigReader(Path("pfad/zur/mig_utils.xml"))
 mig = reader.read()
 assert isinstance(mig, MessageImplementationGuide)
 assert mig.format == "UTILTS"
 ```
 
-Aktuell (Version 0.1) können nur MIGs gelesen werden.
-Der AHB-Teil soll aber folgen.
+### Anwendungshandbuch (AHB) deserialisieren
+```python
+from pathlib import Path
+from fundamend import AhbReader, Anwendungshandbuch
+
+# Angenommen, ahb_utilts.xml enthält:
+# <?xml version="1.0" encoding="UTF-8"?>
+# <AHB Versionsnummer="1.1d"
+#    Veroeffentlichungsdatum="02.04.2024"
+#    Author="BDEW">
+#    <AWF Pruefidentifikator="25001" Beschreibung="Berechnungsformel" Kommunikation_von="NB an MSB / LF">
+#    ...
+#   </AWF>
+# </AHB>
+
+reader = AhbReader(Path("pfad/zur/ahb_utils.xml"))
+ahb = reader.read()
+assert isinstance(ahb, Anwendungshandbuch)
+assert {awf.pruefidentifikator for awf in ahb.anwendungsfaelle} == {
+    "25001",
+    "25002",
+    "25003",
+    "25004",
+    "25005",
+    "25006",
+    "25007",
+    "25008",
+    "25009",
+}
+```
+
+Die vollständigen Beispiele finden sich in den [unittests](unittests).
+
 
 ## Verwendung und Mitwirken
 Der Code ist MIT-lizenziert und kann daher frei verwendet werden.
 Wir freuen uns über Pull Requests an den main-Branch dieses Repositories.
 
 ## Hochfrequenz
 Die [Hochfrequenz Unternehmensberatung GmbH](https://www.hochfrequenz.de) ist eine Beratung für Energieversorger im deutschsprachigen Raum.
```

