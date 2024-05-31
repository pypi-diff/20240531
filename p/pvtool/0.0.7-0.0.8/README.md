# Comparing `tmp/pvtool-0.0.7.tar.gz` & `tmp/pvtool-0.0.8.tar.gz`

## Comparing `pvtool-0.0.7.tar` & `pvtool-0.0.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 pvtool-0.0.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 pvtool-0.0.7/README.md
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 pvtool-0.0.7/requirements.in
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 pvtool-0.0.7/requirements.txt
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 pvtool-0.0.7/tox.ini
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pvtool-0.0.7/.github/dependabot.yml
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 pvtool-0.0.7/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 pvtool-0.0.7/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 pvtool-0.0.7/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 pvtool-0.0.7/.github/workflows/formatting.yml
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 pvtool-0.0.7/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 pvtool-0.0.7/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 pvtool-0.0.7/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 pvtool-0.0.7/.github/workflows/pythonlint.yml
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 pvtool-0.0.7/.github/workflows/unittests.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pvtool-0.0.7/dev_requirements/requirements-coverage.in
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 pvtool-0.0.7/dev_requirements/requirements-coverage.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 pvtool-0.0.7/dev_requirements/requirements-formatting.in
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 pvtool-0.0.7/dev_requirements/requirements-formatting.txt
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 pvtool-0.0.7/dev_requirements/requirements-linting.in
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 pvtool-0.0.7/dev_requirements/requirements-linting.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pvtool-0.0.7/dev_requirements/requirements-packaging.in
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 pvtool-0.0.7/dev_requirements/requirements-packaging.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pvtool-0.0.7/dev_requirements/requirements-tests.in
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 pvtool-0.0.7/dev_requirements/requirements-tests.txt
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 pvtool-0.0.7/dev_requirements/requirements-type_check.in
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 pvtool-0.0.7/dev_requirements/requirements-type_check.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pvtool-0.0.7/src/_your_package_version.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 pvtool-0.0.7/src/pvtool/__init__.py
--rw-r--r--   0        0        0    20851 2020-02-02 00:00:00.000000 pvtool-0.0.7/src/pvtool/customer_loader.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 pvtool-0.0.7/src/pvtool/malo_id_validation.py
--rw-r--r--   0        0        0     9484 2020-02-02 00:00:00.000000 pvtool-0.0.7/src/pvtool/network_loader.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 pvtool-0.0.7/src/pvtool/py.typed
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 pvtool-0.0.7/src/pvtool/resource_loader.py
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 pvtool-0.0.7/src/pvtool/utils.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pvtool-0.0.7/src/pvtool/validation_manager.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 pvtool-0.0.7/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 pvtool-0.0.7/LICENSE
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 pvtool-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 pvtool-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 pvtool-0.0.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 pvtool-0.0.8/README.md
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 pvtool-0.0.8/requirements.in
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 pvtool-0.0.8/requirements.txt
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 pvtool-0.0.8/tox.ini
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pvtool-0.0.8/.github/dependabot.yml
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 pvtool-0.0.8/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 pvtool-0.0.8/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 pvtool-0.0.8/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 pvtool-0.0.8/.github/workflows/formatting.yml
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 pvtool-0.0.8/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 pvtool-0.0.8/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 pvtool-0.0.8/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 pvtool-0.0.8/.github/workflows/pythonlint.yml
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 pvtool-0.0.8/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pvtool-0.0.8/dev_requirements/requirements-coverage.in
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 pvtool-0.0.8/dev_requirements/requirements-coverage.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 pvtool-0.0.8/dev_requirements/requirements-formatting.in
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 pvtool-0.0.8/dev_requirements/requirements-formatting.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 pvtool-0.0.8/dev_requirements/requirements-linting.in
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 pvtool-0.0.8/dev_requirements/requirements-linting.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pvtool-0.0.8/dev_requirements/requirements-packaging.in
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pvtool-0.0.8/dev_requirements/requirements-packaging.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pvtool-0.0.8/dev_requirements/requirements-tests.in
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 pvtool-0.0.8/dev_requirements/requirements-tests.txt
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 pvtool-0.0.8/dev_requirements/requirements-type_check.in
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 pvtool-0.0.8/dev_requirements/requirements-type_check.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pvtool-0.0.8/src/_your_package_version.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 pvtool-0.0.8/src/pvtool/__init__.py
+-rw-r--r--   0        0        0    21108 2020-02-02 00:00:00.000000 pvtool-0.0.8/src/pvtool/customer_loader.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 pvtool-0.0.8/src/pvtool/malo_id_validation.py
+-rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 pvtool-0.0.8/src/pvtool/network_loader.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 pvtool-0.0.8/src/pvtool/py.typed
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 pvtool-0.0.8/src/pvtool/resource_loader.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 pvtool-0.0.8/src/pvtool/utils.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 pvtool-0.0.8/src/pvtool/validation_manager.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 pvtool-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 pvtool-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 pvtool-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 pvtool-0.0.8/PKG-INFO
```

### Comparing `pvtool-0.0.7/.pre-commit-config.yaml` & `pvtool-0.0.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pvtool-0.0.7/README.md` & `pvtool-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pvtool-0.0.7/requirements.txt` & `pvtool-0.0.8/requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,72 +2,65 @@
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile requirements.in
 #
 annotated-types==0.5.0
     # via pydantic
-attrs==23.1.0
-    # via bomf
 bidict==0.22.1
     # via
     #   bomf
     #   pvframework
-bo4e==0.5.6
-    # via bomf
-bomf==0.8.1
+bomf==0.11.0
     # via
     #   -r requirements.in
     #   ibims
 dnspython==2.4.2
     # via email-validator
 email-validator==2.0.0.post2
     # via pydantic
 frozendict==2.3.8
     # via
     #   bomf
     #   pvframework
-ibims==0.1.11
+ibims==0.1.13
     # via -r requirements.in
 idna==3.4
     # via email-validator
+importlib-resources==6.4.0
+    # via schwifty
 injector==0.21.0
     # via bomf
-iso3166==2.1.1
-    # via
-    #   bo4e
-    #   schwifty
 more-itertools==10.2.0
     # via -r requirements.in
 networkx==3.1
     # via
     #   bomf
     #   pvframework
 pvframework==0.0.8
     # via
     #   -r requirements.in
     #   bomf
 pycountry==22.3.5
     # via schwifty
-pydantic[email]==2.5.3
+pydantic[email]==2.7.1
     # via
     #   -r requirements.in
-    #   bo4e
     #   bomf
-pydantic-core==2.14.6
+pydantic-core==2.18.2
     # via pydantic
-pyhumps==3.8.0
-    # via bo4e
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via -r requirements.in
 python-generics==0.0.2
     # via bomf
-pytz==2023.3.post1
+pytz==2024.1
     # via -r requirements.in
-schwifty==2024.1.1.post0
+rstr==3.2.2
+    # via schwifty
+schwifty==2024.5.3
     # via -r requirements.in
 six==1.16.0
     # via python-dateutil
 typeguard==4.1.5
     # via
     #   bomf
     #   pvframework
```

### Comparing `pvtool-0.0.7/tox.ini` & `pvtool-0.0.8/tox.ini`

 * *Files identical despite different names*

### Comparing `pvtool-0.0.7/.github/dependabot.yml` & `pvtool-0.0.8/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pvtool-0.0.7/.github/workflows/codeql-analysis.yml` & `pvtool-0.0.8/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `pvtool-0.0.7/.github/workflows/coverage.yml` & `pvtool-0.0.8/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `pvtool-0.0.7/.github/workflows/dependabot_automerge.yml` & `pvtool-0.0.8/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `pvtool-0.0.7/.github/workflows/formatting.yml` & `pvtool-0.0.8/.github/workflows/formatting.yml`

 * *Files identical despite different names*

### Comparing `pvtool-0.0.7/.github/workflows/packaging_test.yml` & `pvtool-0.0.8/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `pvtool-0.0.7/.github/workflows/python-publish.yml` & `pvtool-0.0.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pvtool-0.0.7/.github/workflows/pythonlint.yml` & `pvtool-0.0.8/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `pvtool-0.0.7/.github/workflows/unittests.yml` & `pvtool-0.0.8/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `pvtool-0.0.7/dev_requirements/requirements-packaging.txt` & `pvtool-0.0.8/dev_requirements/requirements-packaging.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,78 +1,74 @@
 #
-# This file is autogenerated by pip-compile with python 3.10
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.12
+# by the following command:
 #
-#    pip-compile requirements-packaging.in
+#    pip-compile dev_requirements/requirements-packaging.in
 #
-bleach==6.0.0
-    # via readme-renderer
-build==1.0.3
+build==1.2.1
     # via -r dev_requirements/requirements-packaging.in
-certifi==2023.7.22
+certifi==2024.2.2
     # via requests
-cffi==1.15.1
+cffi==1.16.0
     # via cryptography
-charset-normalizer==3.1.0
+charset-normalizer==3.3.2
     # via requests
-cryptography==41.0.3
+cryptography==42.0.5
     # via secretstorage
 docutils==0.20.1
     # via readme-renderer
-idna==3.4
+idna==3.6
     # via requests
-importlib-metadata==6.7.0
+importlib-metadata==7.0.2
     # via
     #   keyring
     #   twine
-jaraco-classes==3.2.3
+jaraco-classes==3.3.1
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
-keyring==23.13.1
+keyring==24.3.1
     # via twine
 markdown-it-py==3.0.0
     # via rich
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==10.2.0
     # via jaraco-classes
-packaging==23.1
+nh3==0.2.15
+    # via readme-renderer
+packaging==24.0
     # via build
-pkginfo==1.9.6
+pkginfo==1.10.0
     # via twine
 pycparser==2.21
     # via cffi
-pygments==2.15.1
+pygments==2.17.2
     # via
     #   readme-renderer
     #   rich
 pyproject-hooks==1.0.0
     # via build
-readme-renderer==37.3
+readme-renderer==43.0
     # via twine
 requests==2.31.0
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==13.4.2
+rich==13.7.1
     # via twine
 secretstorage==3.3.3
     # via keyring
-six==1.16.0
-    # via bleach
-twine==4.0.2
+twine==5.1.0
     # via -r dev_requirements/requirements-packaging.in
-urllib3==2.0.3
+urllib3==2.2.1
     # via
     #   requests
     #   twine
-webencodings==0.5.1
-    # via bleach
-zipp==3.15.0
+zipp==3.18.1
     # via importlib-metadata
```

### Comparing `pvtool-0.0.7/src/pvtool/customer_loader.py` & `pvtool-0.0.8/src/pvtool/customer_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Contains validation logic for TripicaCustomerLoaderDataSet
 """
+
 import re
 from datetime import date, datetime
 from typing import Any, Generator, Optional, TypeAlias, TypeVar
 
 from bomf.config import MigrationConfig
 from dateutil.relativedelta import relativedelta
 from email_validator import validate_email
@@ -16,14 +17,15 @@
     ParallelQueryMappedValidator,
     PathMappedValidator,
     Query,
     QueryMappedValidator,
     ValidationManager,
     Validator,
 )
+from pvframework.errors import ValidationMode
 from pvframework.types import SyncValidatorFunction
 from pvframework.utils import param, required_field
 from pytz import timezone
 from schwifty import BIC, IBAN
 
 from .utils import migration_config
 from .validation_manager import ValidationManagerWithConfig
@@ -352,15 +354,16 @@
         """
         This method provides a ValidationManager for customer loader with an injected MigrationConfig
         """
         customer_manager = ValidationManagerWithConfig[TripicaCustomerLoaderDataSet](
             config, manager_id="CustomerLoader"
         )
         customer_manager.register(
-            PathMappedValidator(validate_geschaeftspartner_anrede, {"anrede": "geschaeftspartner.anrede"})
+            PathMappedValidator(validate_geschaeftspartner_anrede, {"anrede": "geschaeftspartner.anrede"}),
+            mode=ValidationMode.WARNING,
         )
         customer_manager.register(PathMappedValidator(validate_str_is_stripped, {"string": "geschaeftspartner.name1"}))
         customer_manager.register(PathMappedValidator(validate_str_is_stripped, {"string": "geschaeftspartner.name2"}))
         customer_manager.register(
             PathMappedValidator(validate_geschaeftspartner_name3, {"name3": "geschaeftspartner.name3"})
         )
         customer_manager.register(PathMappedValidator(validate_e_mail, {"e_mail": "geschaeftspartner.e_mail_adresse"}))
@@ -371,24 +374,28 @@
         )
         customer_manager.register(
             PathMappedValidator(validate_date_in_past_required, {"past_date": "geschaeftspartner.erstellungsdatum"})
         )
         customer_manager.register(
             PathMappedValidator(
                 validate_geschaeftspartner_geburtsdatum, {"geburtsdatum": "geschaeftspartner.geburtstag"}
-            )
+            ),
+            mode=ValidationMode.WARNING,
         )
         customer_manager.register(
-            PathMappedValidator(validate_telefonnummer, {"telefonnummer": "geschaeftspartner.telefonnummer_privat"})
+            PathMappedValidator(validate_telefonnummer, {"telefonnummer": "geschaeftspartner.telefonnummer_privat"}),
+            mode=ValidationMode.WARNING,
         )
         customer_manager.register(
-            PathMappedValidator(validate_telefonnummer, {"telefonnummer": "geschaeftspartner.telefonnummer_geschaeft"})
+            PathMappedValidator(validate_telefonnummer, {"telefonnummer": "geschaeftspartner.telefonnummer_geschaeft"}),
+            mode=ValidationMode.WARNING,
         )
         customer_manager.register(
-            PathMappedValidator(validate_telefonnummer, {"telefonnummer": "geschaeftspartner.telefonnummer_mobil"})
+            PathMappedValidator(validate_telefonnummer, {"telefonnummer": "geschaeftspartner.telefonnummer_mobil"}),
+            mode=ValidationMode.WARNING,
         )
         customer_manager.register(
             QueryMappedValidator(
                 validate_address_deutsch, {"address": Query().path("liefer_adressen").iter(iter_contract_id_dict)}
             )
         )
         customer_manager.register(
```

### Comparing `pvtool-0.0.7/src/pvtool/malo_id_validation.py` & `pvtool-0.0.8/src/pvtool/malo_id_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 validators that were included in the bo4e package prior to version 0.6.0
 """
+
 import re
 
 from pydantic_core.core_schema import ValidationInfo
 
 
 def _get_malo_id_checksum(malo_id: str) -> str:
     """
```

### Comparing `pvtool-0.0.7/src/pvtool/network_loader.py` & `pvtool-0.0.8/src/pvtool/network_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Contains validation logic for TripicaNetworkLoaderDataSet
 """
+
 import re
 from typing import Iterator
 
 from ibims.bo4e import Kundentyp, Rollencodetyp, Sparte, Tarifart, Zaehlerauspraegung, Zaehlwerk
 from ibims.datasets import TripicaNetworkLoaderDataSet
 from injector import Module, provider
 from pvframework import PathMappedValidator, Query, QueryMappedValidator, ValidationManager, Validator
```

### Comparing `pvtool-0.0.7/src/pvtool/resource_loader.py` & `pvtool-0.0.8/src/pvtool/resource_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Contains validation logic for TripicaResourceLoaderDataSet
 """
+
 import re
 
 from ibims.bo4e import Sparte
 from ibims.datasets import TripicaResourceLoaderDataSet
 from injector import Module, provider
 from pvframework import PathMappedValidator, ValidationManager, Validator
 from pvframework.utils import param
```

### Comparing `pvtool-0.0.7/src/pvtool/utils.py` & `pvtool-0.0.8/src/pvtool/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Contains utility functions to be used in the PV-Tool.
 """
+
 import inspect
 from typing import Optional
 
 from bomf.config import MigrationConfig
 from pvframework import ValidationManager
 
 from .validation_manager import ValidationManagerWithConfig
```

### Comparing `pvtool-0.0.7/src/pvtool/validation_manager.py` & `pvtool-0.0.8/src/pvtool/validation_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 This module contains the ValidationManager classes used throughout the PV-Tool.
 """
+
 from bomf.config import MigrationConfig
 from injector import inject
 from pvframework import ValidationManager
 from pvframework.types import DataSetT
 
 
 class ValidationManagerWithConfig(ValidationManager[DataSetT]):
```

### Comparing `pvtool-0.0.7/.gitignore` & `pvtool-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `pvtool-0.0.7/LICENSE` & `pvtool-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pvtool-0.0.7/pyproject.toml` & `pvtool-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "bomf",
     "pvframework>=0.0.8",
-    "ibims>=0.1.11",
+    "ibims>=0.1.12",
     "python-dateutil",
     "pydantic[email]",
     "more_itertools",
     "pytz",
     "schwifty",
 ]     # add all the dependencies from requirements.in here, too
 dynamic = ["readme", "version"]
```

### Comparing `pvtool-0.0.7/PKG-INFO` & `pvtool-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pvtool
-Version: 0.0.7
+Version: 0.0.8
 Summary: This tool contains validation logic for the BO4E migration data model (ibims). It uses the pvframework. 
 Project-URL: Changelog, https://github.com/Hochfrequenz/pedantic-validator-tool/releases
 Project-URL: Homepage, https://github.com/Hochfrequenz/pedantic-validator-tool
 Author-email: Hochfrequenz Unternehmensberatung GmbH <info@hochfrequenz.de>
 License: MIT
 License-File: LICENSE
 Keywords: bo4e,migration,python,validation
@@ -15,15 +15,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.11
 Requires-Dist: bomf
-Requires-Dist: ibims>=0.1.11
+Requires-Dist: ibims>=0.1.12
 Requires-Dist: more-itertools
 Requires-Dist: pvframework>=0.0.8
 Requires-Dist: pydantic[email]
 Requires-Dist: python-dateutil
 Requires-Dist: pytz
 Requires-Dist: schwifty
 Description-Content-Type: text/markdown
```

