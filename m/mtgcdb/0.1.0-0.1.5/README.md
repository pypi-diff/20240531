# Comparing `tmp/mtgcdb-0.1.0.tar.gz` & `tmp/mtgcdb-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtgcdb-0.1.0.tar", max compression
+gzip compressed data, was "mtgcdb-0.1.5.tar", max compression
```

## Comparing `mtgcdb-0.1.0.tar` & `mtgcdb-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11558 2024-05-29 23:49:18.304814 mtgcdb-0.1.0/LICENSE
--rw-r--r--   0        0        0      642 2024-05-30 22:55:02.197490 mtgcdb-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      220 2024-05-30 20:30:12.028108 mtgcdb-0.1.0/README.md
--rw-r--r--   0        0        0       77 2024-05-30 22:53:23.816971 mtgcdb-0.1.0/src/mtgcdb/__init__.py
--rw-r--r--   0        0        0     1244 2024-05-30 20:16:38.036663 mtgcdb-0.1.0/src/mtgcdb/card.py
--rw-r--r--   0        0        0     3588 2024-05-30 20:19:13.904340 mtgcdb-0.1.0/src/mtgcdb/db.py
--rw-r--r--   0        0        0     4993 2024-05-30 20:19:22.658428 mtgcdb-0.1.0/src/mtgcdb/mtgcdb.py
--rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 mtgcdb-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-30 23:50:57.330439 mtgcdb-0.1.5/LICENSE
+-rw-r--r--   0        0        0      203 2024-05-30 23:50:57.330439 mtgcdb-0.1.5/README.md
+-rw-r--r--   0        0        0      612 2024-05-30 23:51:04.714466 mtgcdb-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       71 2024-05-30 23:50:57.334439 mtgcdb-0.1.5/src/mtgcdb/__init__.py
+-rw-r--r--   0        0        0     1201 2024-05-30 23:50:57.334439 mtgcdb-0.1.5/src/mtgcdb/card.py
+-rw-r--r--   0        0        0     3483 2024-05-30 23:50:57.334439 mtgcdb-0.1.5/src/mtgcdb/db.py
+-rw-r--r--   0        0        0     4848 2024-05-30 23:50:57.334439 mtgcdb-0.1.5/src/mtgcdb/mtgcdb.py
+-rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 mtgcdb-0.1.5/PKG-INFO
```

### Comparing `mtgcdb-0.1.0/LICENSE` & `mtgcdb-0.1.5/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `mtgcdb-0.1.0/pyproject.toml` & `mtgcdb-0.1.5/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-[tool.ruff]
-line-length = 88
-
-[tool.mypy]
-disable_error_code = "import-untyped"
-
-[tool.poetry]
-name = "mtgcdb"
-version = "0.1.0"
-description = "MTG Card Database"
-authors = ["j6e <jongares@hotmail.com>"]
-license = "Apache 2.0"
-readme = "README.md"
-packages = [{ include = "mtgcdb", from = "./src/"}]
-
-[tool.poetry.dependencies]
-python = "^3.11"
-SQLAlchemy = "^2.0.30"
-httpx = "^0.27.0"
-loguru = "^0.7.2"
-
-[tool.poetry.group.dev.dependencies]
-pre-commit = "^3.7.1"
-ruff = "^0.4.6"
-pytest = "^8.2.1"
-pytest-dependency = "^0.6.0"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.ruff]
+line-length = 88
+
+[tool.mypy]
+disable_error_code = "import-untyped"
+
+[tool.poetry]
+name = "mtgcdb"
+version = "0.1.5"
+description = "MTG Card Database"
+authors = ["j6e <jongares@hotmail.com>"]
+license = "Apache 2.0"
+readme = "README.md"
+packages = [{ include = "mtgcdb", from = "./src/"}]
+
+[tool.poetry.dependencies]
+python = "^3.11"
+SQLAlchemy = "^2.0.30"
+httpx = "^0.27.0"
+loguru = "^0.7.2"
+
+[tool.poetry.group.dev.dependencies]
+pre-commit = "^3.7.1"
+ruff = "^0.4.6"
+pytest = "^8.2.1"
+pytest-dependency = "^0.6.0"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `mtgcdb-0.1.0/src/mtgcdb/card.py` & `mtgcdb-0.1.5/src/mtgcdb/card.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from typing import Optional
-
-from sqlalchemy import ForeignKey
-from sqlalchemy.ext.automap import automap_base
-from sqlalchemy.orm import Mapped, mapped_column, relationship
-
-Base = automap_base()
-
-
-class Card(Base):  # type: ignore
-    __tablename__ = "cards"
-    extend_existing = True
-
-    uuid: Mapped[str] = mapped_column(primary_key=True)
-    name: Mapped[str]
-    faceName: Mapped[str]
-    types: Mapped[str]
-    subtypes: Mapped[str]
-    setCode: Mapped[str]
-    power: Mapped[Optional[str]]
-    toughness: Mapped[Optional[str]]
-    text: Mapped[str]
-    manaValue: Mapped[float]
-    manaCost: Mapped[str]
-    colors: Mapped[str]
-    colorIdentity: Mapped[str]
-    rarity: Mapped[str]
-
-    def __repr__(self) -> str:
-        return f"Card(name={self.name}, types={self.types}, manaCost={self.manaCost})"
-
-    identifier: Mapped["CardIdentifier"] = relationship(
-        back_populates="card", viewonly=True, lazy="joined"
-    )
-
-
-class CardIdentifier(Base):  # type: ignore
-    __tablename__ = "cardIdentifiers"
-
-    uuid = mapped_column(ForeignKey("cards.uuid"), primary_key=True)
-    scryfallId: Mapped[str]
-
-    card: Mapped[Card] = relationship(back_populates="identifier", viewonly=True)
+from typing import Optional
+
+from sqlalchemy import ForeignKey
+from sqlalchemy.ext.automap import automap_base
+from sqlalchemy.orm import Mapped, mapped_column, relationship
+
+Base = automap_base()
+
+
+class Card(Base):  # type: ignore
+    __tablename__ = "cards"
+    extend_existing = True
+
+    uuid: Mapped[str] = mapped_column(primary_key=True)
+    name: Mapped[str]
+    faceName: Mapped[str]
+    types: Mapped[str]
+    subtypes: Mapped[str]
+    setCode: Mapped[str]
+    power: Mapped[Optional[str]]
+    toughness: Mapped[Optional[str]]
+    text: Mapped[str]
+    manaValue: Mapped[float]
+    manaCost: Mapped[str]
+    colors: Mapped[str]
+    colorIdentity: Mapped[str]
+    rarity: Mapped[str]
+
+    def __repr__(self) -> str:
+        return f"Card(name={self.name}, types={self.types}, manaCost={self.manaCost})"
+
+    identifier: Mapped["CardIdentifier"] = relationship(
+        back_populates="card", viewonly=True, lazy="joined"
+    )
+
+
+class CardIdentifier(Base):  # type: ignore
+    __tablename__ = "cardIdentifiers"
+
+    uuid = mapped_column(ForeignKey("cards.uuid"), primary_key=True)
+    scryfallId: Mapped[str]
+
+    card: Mapped[Card] = relationship(back_populates="identifier", viewonly=True)
```

### Comparing `mtgcdb-0.1.0/src/mtgcdb/db.py` & `mtgcdb-0.1.5/src/mtgcdb/db.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-import io
-import os
-from datetime import datetime
-from pathlib import Path
-from zipfile import ZipFile
-
-import httpx
-from loguru import logger
-
-CURRENT_FILE_PATH = Path(__file__).resolve()
-DB_GENERIC_PATH = CURRENT_FILE_PATH.parent.parent.parent / "db"
-DB_FOLDER_NAME = "{time}"
-CARD_DB_DOWNLOAD_URL = "https://mtgjson.com/api/v5/AllPrintings.sqlite.zip"
-AUTO_UPDATE_DB = True
-AUTO_UPDATE_DB_INTERVAL = 24 * 7  # in hours
-
-logger.disable("mtgcdb")
-
-
-def download_card_definitions_db() -> Path:
-    """Download card definitions DB"""
-    logger.info(f"Downloading card definitions DB from {CARD_DB_DOWNLOAD_URL}")
-    response = httpx.get(CARD_DB_DOWNLOAD_URL)
-    if response.status_code != 200:
-        logger.error(
-            f"Failed to download card definitions DB. Status code: {response.status_code}"
-        )
-        raise Exception("Failed to download card definitions DB")
-
-    zip_db = ZipFile(io.BytesIO(response.content))
-    current_time = datetime.now().strftime("%Y%m%dT%H%M%S")
-    db_folder_path = DB_GENERIC_PATH / DB_FOLDER_NAME.format(time=current_time)
-    db_folder_path.mkdir(parents=True, exist_ok=True)
-    zip_db.extractall(path=db_folder_path)
-    db_path = db_folder_path / "AllPrintings.sqlite"
-
-    if os.path.exists(db_path):
-        logger.success(f"Card definitions saved to {db_path}")
-    else:
-        raise Exception("Failed to extract card definitions DB")
-
-    return db_path
-
-
-def get_most_recent_db() -> Path | None:
-    """Get the most recent card definitions DB"""
-    DB_GENERIC_PATH.mkdir(parents=True, exist_ok=True)
-    db_folders = os.listdir(DB_GENERIC_PATH)
-    if not db_folders:
-        return None
-
-    db_folders.sort()
-    latest_db_folder = db_folders[-1]
-    latest_db_folder_path = DB_GENERIC_PATH / latest_db_folder
-    db_files = os.listdir(latest_db_folder_path)
-    if not db_files:
-        return None
-
-    db_files.sort()
-    latest_db_file = db_files[0]
-    latest_db_file_path = latest_db_folder_path / latest_db_file
-    return latest_db_file_path
-
-
-def clean_old_dbs() -> None:
-    """Clean old card definitions DBs"""
-    db_folders = os.listdir(DB_GENERIC_PATH)
-    if not db_folders:
-        return
-
-    db_folders.sort()
-    for db_folder in db_folders[:-1]:
-        db_folder_path = DB_GENERIC_PATH / db_folder
-        logger.info(f"Removing old card definitions DB: {db_folder_path}")
-        # Remove the folder and its contents
-        for file in db_folder_path.iterdir():
-            file.unlink()
-        db_folder_path.rmdir()
-
-
-def update_or_pass() -> Path:
-    """Check if the card definitions DB should be updated.
-    Returns the path to the most recent DB. If no DB is found, download a new one."""
-
-    db_path = get_most_recent_db()
-    if not db_path:
-        logger.info("No card definitions DB found")
-        return download_card_definitions_db()
-
-    latest_db_folder = db_path.parent.name
-    db_file_time = datetime.strptime(latest_db_folder, "%Y%m%dT%H%M%S")
-    time_diff = datetime.now() - db_file_time
-    time_diff_hours = time_diff.total_seconds() / 3600
-
-    if time_diff_hours >= AUTO_UPDATE_DB_INTERVAL and AUTO_UPDATE_DB:
-        logger.info(
-            f"Updating card definitions DB. Last updated {time_diff_hours/7:.2f} days ago"
-        )
-        clean_old_dbs()
-        return download_card_definitions_db()
-    else:
-        logger.info(
-            f"Skipping card definitions DB update. Last updated {time_diff_hours/7:.2f} days ago"
-        )
-        return db_path
+import io
+import os
+from datetime import datetime
+from pathlib import Path
+from zipfile import ZipFile
+
+import httpx
+from loguru import logger
+
+CURRENT_FILE_PATH = Path(__file__).resolve()
+DB_GENERIC_PATH = CURRENT_FILE_PATH.parent.parent.parent / "db"
+DB_FOLDER_NAME = "{time}"
+CARD_DB_DOWNLOAD_URL = "https://mtgjson.com/api/v5/AllPrintings.sqlite.zip"
+AUTO_UPDATE_DB = True
+AUTO_UPDATE_DB_INTERVAL = 24 * 7  # in hours
+
+logger.disable("mtgcdb")
+
+
+def download_card_definitions_db() -> Path:
+    """Download card definitions DB"""
+    logger.info(f"Downloading card definitions DB from {CARD_DB_DOWNLOAD_URL}")
+    response = httpx.get(CARD_DB_DOWNLOAD_URL)
+    if response.status_code != 200:
+        logger.error(
+            f"Failed to download card definitions DB. Status code: {response.status_code}"
+        )
+        raise Exception("Failed to download card definitions DB")
+
+    zip_db = ZipFile(io.BytesIO(response.content))
+    current_time = datetime.now().strftime("%Y%m%dT%H%M%S")
+    db_folder_path = DB_GENERIC_PATH / DB_FOLDER_NAME.format(time=current_time)
+    db_folder_path.mkdir(parents=True, exist_ok=True)
+    zip_db.extractall(path=db_folder_path)
+    db_path = db_folder_path / "AllPrintings.sqlite"
+
+    if os.path.exists(db_path):
+        logger.success(f"Card definitions saved to {db_path}")
+    else:
+        raise Exception("Failed to extract card definitions DB")
+
+    return db_path
+
+
+def get_most_recent_db() -> Path | None:
+    """Get the most recent card definitions DB"""
+    DB_GENERIC_PATH.mkdir(parents=True, exist_ok=True)
+    db_folders = os.listdir(DB_GENERIC_PATH)
+    if not db_folders:
+        return None
+
+    db_folders.sort()
+    latest_db_folder = db_folders[-1]
+    latest_db_folder_path = DB_GENERIC_PATH / latest_db_folder
+    db_files = os.listdir(latest_db_folder_path)
+    if not db_files:
+        return None
+
+    db_files.sort()
+    latest_db_file = db_files[0]
+    latest_db_file_path = latest_db_folder_path / latest_db_file
+    return latest_db_file_path
+
+
+def clean_old_dbs() -> None:
+    """Clean old card definitions DBs"""
+    db_folders = os.listdir(DB_GENERIC_PATH)
+    if not db_folders:
+        return
+
+    db_folders.sort()
+    for db_folder in db_folders[:-1]:
+        db_folder_path = DB_GENERIC_PATH / db_folder
+        logger.info(f"Removing old card definitions DB: {db_folder_path}")
+        # Remove the folder and its contents
+        for file in db_folder_path.iterdir():
+            file.unlink()
+        db_folder_path.rmdir()
+
+
+def update_or_pass() -> Path:
+    """Check if the card definitions DB should be updated.
+    Returns the path to the most recent DB. If no DB is found, download a new one."""
+
+    db_path = get_most_recent_db()
+    if not db_path:
+        logger.info("No card definitions DB found")
+        return download_card_definitions_db()
+
+    latest_db_folder = db_path.parent.name
+    db_file_time = datetime.strptime(latest_db_folder, "%Y%m%dT%H%M%S")
+    time_diff = datetime.now() - db_file_time
+    time_diff_hours = time_diff.total_seconds() / 3600
+
+    if time_diff_hours >= AUTO_UPDATE_DB_INTERVAL and AUTO_UPDATE_DB:
+        logger.info(
+            f"Updating card definitions DB. Last updated {time_diff_hours/7:.2f} days ago"
+        )
+        clean_old_dbs()
+        return download_card_definitions_db()
+    else:
+        logger.info(
+            f"Skipping card definitions DB update. Last updated {time_diff_hours/7:.2f} days ago"
+        )
+        return db_path
```

### Comparing `mtgcdb-0.1.0/src/mtgcdb/mtgcdb.py` & `mtgcdb-0.1.5/src/mtgcdb/mtgcdb.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,145 +1,145 @@
-from collections.abc import Sequence
-from functools import lru_cache
-from pathlib import Path
-
-from sqlalchemy import create_engine, or_, select
-from sqlalchemy.orm import sessionmaker
-
-from mtgcdb.card import Base, Card
-from mtgcdb.db import clean_old_dbs, download_card_definitions_db, update_or_pass
-
-
-class MTGCDB:
-    """Magic: The Gathering card database singleton"""
-
-    __instance: "MTGCDB | None" = None
-
-    def __init__(self, force_update: bool = False):
-        if (
-            MTGCDB.__instance is not None
-            and hasattr(self, "engine")
-            and hasattr(self, "Session")
-        ):
-            return MTGCDB.__instance  # type: ignore
-
-        self.db_path = update_or_pass() if not force_update else self.update_db()
-        self.engine = create_engine(f"sqlite:///{self.db_path}", echo=False)
-        self.Session = sessionmaker(bind=self.engine)
-        Base.prepare(self.engine)
-
-        MTGCDB.__instance = self
-
-    def update_db(self) -> Path:
-        clean_old_dbs()
-        return download_card_definitions_db()
-
-    @lru_cache(maxsize=1024)
-    def get_card_by_name(self, name: str, set_code: str | None = None) -> Card:
-        """Get a card by its name
-
-        Args:
-            name (str): exact card name
-            set_code (str | None, optional): 3 letters of the set code. Defaults to None.
-
-        Returns:
-            Card:
-        """
-        with self.Session() as session:
-            query = select(Card).where(Card.name == name)
-            if set_code:
-                query = query.where(Card.setCode == set_code)
-            card = session.scalars(query).first()
-            if not card:
-                card = self.get_card_by_face_name(name, set_code=set_code)
-            return card
-
-    @lru_cache(maxsize=1024)
-    def get_card_by_face_name(
-        self, face_name: str, set_code: str | None = None
-    ) -> Card:
-        """Get a card by its front face name
-
-        Args:
-            face_name (str): exact front face name
-            set_code (str | None, optional): 3 letters of the set code. Defaults to None.
-
-        Returns:
-            Card:
-        """
-        with self.Session() as session:
-            query = select(Card).where(Card.faceName == face_name)
-            if set_code:
-                query = query.where(Card.setCode == set_code)
-            card = session.scalars(query).first()
-            if not card:
-                raise ValueError(f"Card faceName={face_name} not found in database")
-            return card
-
-    def get_card_image_url_from_name(
-        self, name: str, set_code: str | None = None, img_type: str = "normal"
-    ) -> str:
-        """Get the image URL of a card by its name
-
-        Args:
-            name (str): exact card name
-            set_code (str | None, optional):  3 letters of the set code. Defaults to None.
-            img_type (str, optional): One of "png", "normal", "large" or "small". Defaults to "normal".
-              See https://scryfall.com/docs/api/images for more info.
-
-        Returns:
-            str: URL of the card image
-        """
-        c = self.get_card_by_name(name, set_code=set_code)
-        img_format = "png" if img_type == "png" else "jpg"
-        scryfall_id = c.identifier.scryfallId
-        url = f"https://cards.scryfall.io/{img_type}/front/{scryfall_id[0]}/{scryfall_id[1]}/{scryfall_id}.{img_format}"
-        return url
-
-    def get_cards_by_names(self, names: list[str]) -> list[Card]:
-        """Get a list of cards by their names
-
-        Args:
-            names (list[str]): List of exact card names
-
-        Returns:
-            list[Card]: List of cards
-        """
-        with self.Session() as session:
-            query = select(Card).where(
-                or_(Card.name.in_(names), Card.faceName.in_(names))
-            )
-            results = session.scalars(query).all()
-        return _deduplicate_cards_by_name(results)
-
-    @lru_cache(maxsize=8)
-    def get_cards_by_set_code(self, setCode: str) -> list[Card]:
-        """Get all cards from a set by its set code
-
-        Args:
-            setCode (str): Set code (3 letters)
-
-        Returns:
-            list[Card]: List of cards from the set
-        """
-        with self.Session() as session:
-            query = select(Card).where(Card.setCode == setCode)
-            results = session.scalars(query).all()
-        return _deduplicate_cards_by_name(results)
-
-
-def _deduplicate_cards_by_name(cards: Sequence[Card]) -> list[Card]:
-    """Deduplicate a list of cards by their names
-
-    Args:
-        cards (Sequence[Card]): List of cards
-
-    Returns:
-        list[Card]: Deduplicated list of cards
-    """
-    card_names = set()
-    dedup_cards = []
-    for card in cards:
-        if card.name not in card_names:
-            dedup_cards.append(card)
-            card_names.add(card.name)
-    return dedup_cards
+from collections.abc import Sequence
+from functools import lru_cache
+from pathlib import Path
+
+from sqlalchemy import create_engine, or_, select
+from sqlalchemy.orm import sessionmaker
+
+from mtgcdb.card import Base, Card
+from mtgcdb.db import clean_old_dbs, download_card_definitions_db, update_or_pass
+
+
+class MTGCDB:
+    """Magic: The Gathering card database singleton"""
+
+    __instance: "MTGCDB | None" = None
+
+    def __init__(self, force_update: bool = False):
+        if (
+            MTGCDB.__instance is not None
+            and hasattr(self, "engine")
+            and hasattr(self, "Session")
+        ):
+            return MTGCDB.__instance  # type: ignore
+
+        self.db_path = update_or_pass() if not force_update else self.update_db()
+        self.engine = create_engine(f"sqlite:///{self.db_path}", echo=False)
+        self.Session = sessionmaker(bind=self.engine)
+        Base.prepare(self.engine)
+
+        MTGCDB.__instance = self
+
+    def update_db(self) -> Path:
+        clean_old_dbs()
+        return download_card_definitions_db()
+
+    @lru_cache(maxsize=1024)
+    def get_card_by_name(self, name: str, set_code: str | None = None) -> Card:
+        """Get a card by its name
+
+        Args:
+            name (str): exact card name
+            set_code (str | None, optional): 3 letters of the set code. Defaults to None.
+
+        Returns:
+            Card:
+        """
+        with self.Session() as session:
+            query = select(Card).where(Card.name == name)
+            if set_code:
+                query = query.where(Card.setCode == set_code)
+            card = session.scalars(query).first()
+            if not card:
+                card = self.get_card_by_face_name(name, set_code=set_code)
+            return card
+
+    @lru_cache(maxsize=1024)
+    def get_card_by_face_name(
+        self, face_name: str, set_code: str | None = None
+    ) -> Card:
+        """Get a card by its front face name
+
+        Args:
+            face_name (str): exact front face name
+            set_code (str | None, optional): 3 letters of the set code. Defaults to None.
+
+        Returns:
+            Card:
+        """
+        with self.Session() as session:
+            query = select(Card).where(Card.faceName == face_name)
+            if set_code:
+                query = query.where(Card.setCode == set_code)
+            card = session.scalars(query).first()
+            if not card:
+                raise ValueError(f"Card faceName={face_name} not found in database")
+            return card
+
+    def get_card_image_url_from_name(
+        self, name: str, set_code: str | None = None, img_type: str = "normal"
+    ) -> str:
+        """Get the image URL of a card by its name
+
+        Args:
+            name (str): exact card name
+            set_code (str | None, optional):  3 letters of the set code. Defaults to None.
+            img_type (str, optional): One of "png", "normal", "large" or "small". Defaults to "normal".
+              See https://scryfall.com/docs/api/images for more info.
+
+        Returns:
+            str: URL of the card image
+        """
+        c = self.get_card_by_name(name, set_code=set_code)
+        img_format = "png" if img_type == "png" else "jpg"
+        scryfall_id = c.identifier.scryfallId
+        url = f"https://cards.scryfall.io/{img_type}/front/{scryfall_id[0]}/{scryfall_id[1]}/{scryfall_id}.{img_format}"
+        return url
+
+    def get_cards_by_names(self, names: list[str]) -> list[Card]:
+        """Get a list of cards by their names
+
+        Args:
+            names (list[str]): List of exact card names
+
+        Returns:
+            list[Card]: List of cards
+        """
+        with self.Session() as session:
+            query = select(Card).where(
+                or_(Card.name.in_(names), Card.faceName.in_(names))
+            )
+            results = session.scalars(query).all()
+        return _deduplicate_cards_by_name(results)
+
+    @lru_cache(maxsize=8)
+    def get_cards_by_set_code(self, setCode: str) -> list[Card]:
+        """Get all cards from a set by its set code
+
+        Args:
+            setCode (str): Set code (3 letters)
+
+        Returns:
+            list[Card]: List of cards from the set
+        """
+        with self.Session() as session:
+            query = select(Card).where(Card.setCode == setCode)
+            results = session.scalars(query).all()
+        return _deduplicate_cards_by_name(results)
+
+
+def _deduplicate_cards_by_name(cards: Sequence[Card]) -> list[Card]:
+    """Deduplicate a list of cards by their names
+
+    Args:
+        cards (Sequence[Card]): List of cards
+
+    Returns:
+        list[Card]: Deduplicated list of cards
+    """
+    card_names = set()
+    dedup_cards = []
+    for card in cards:
+        if card.name not in card_names:
+            dedup_cards.append(card)
+            card_names.add(card.name)
+    return dedup_cards
```

### Comparing `mtgcdb-0.1.0/PKG-INFO` & `mtgcdb-0.1.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtgcdb
-Version: 0.1.0
+Version: 0.1.5
 Summary: MTG Card Database
 License: Apache 2.0
 Author: j6e
 Author-email: jongares@hotmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

