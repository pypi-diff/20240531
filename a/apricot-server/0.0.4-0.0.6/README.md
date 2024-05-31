# Comparing `tmp/apricot_server-0.0.4.tar.gz` & `tmp/apricot_server-0.0.6.tar.gz`

## Comparing `apricot_server-0.0.4.tar` & `apricot_server-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,44 @@
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 apricot_server-0.0.4/.markdownlint.json
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 apricot_server-0.0.4/Dockerfile
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 apricot_server-0.0.4/run.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 apricot_server-0.0.4/.github/workflows/lint.yaml
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 apricot_server-0.0.4/.github/workflows/publish_docker.yaml
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 apricot_server-0.0.4/apricot/__about__.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 apricot_server-0.0.4/apricot/__init__.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 apricot_server-0.0.4/apricot/apricot_server.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 apricot_server-0.0.4/apricot/ldap/__init__.py
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 apricot_server-0.0.4/apricot/ldap/oauth_ldap_entry.py
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 apricot_server-0.0.4/apricot/ldap/oauth_ldap_server_factory.py
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 apricot_server-0.0.4/apricot/ldap/oauth_ldap_tree.py
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 apricot_server-0.0.4/apricot/ldap/read_only_ldap_server.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 apricot_server-0.0.4/apricot/oauth/__init__.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 apricot_server-0.0.4/apricot/oauth/enums.py
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 apricot_server-0.0.4/apricot/oauth/microsoft_entra_client.py
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 apricot_server-0.0.4/apricot/oauth/oauth_client.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 apricot_server-0.0.4/apricot/oauth/types.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 apricot_server-0.0.4/docker/docker-compose.yaml
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 apricot_server-0.0.4/docker/entrypoint.sh
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 apricot_server-0.0.4/.gitignore
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 apricot_server-0.0.4/LICENSE
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 apricot_server-0.0.4/README.md
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 apricot_server-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 apricot_server-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 apricot_server-0.0.6/.markdownlint.json
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 apricot_server-0.0.6/Dockerfile
+-rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 apricot_server-0.0.6/run.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 apricot_server-0.0.6/.github/workflows/lint.yaml
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 apricot_server-0.0.6/.github/workflows/publish_docker.yaml
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/__about__.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/__init__.py
+-rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/apricot_server.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/types.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/cache/__init__.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/cache/local_cache.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/cache/redis_cache.py
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/cache/uid_cache.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/ldap/__init__.py
+-rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/ldap/oauth_ldap_entry.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/ldap/oauth_ldap_server_factory.py
+-rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/ldap/oauth_ldap_tree.py
+-rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/ldap/read_only_ldap_server.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/models/__init__.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/models/ldap_attribute_adaptor.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/models/ldap_group_of_names.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/models/ldap_inetorgperson.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/models/ldap_object_class.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/models/ldap_organizational_person.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/models/ldap_person.py
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/models/ldap_posix_account.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/models/ldap_posix_group.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/models/overlay_memberof.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/models/overlay_oauthentry.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/oauth/__init__.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/oauth/enums.py
+-rw-r--r--   0        0        0     6990 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/oauth/keycloak_client.py
+-rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/oauth/microsoft_entra_client.py
+-rw-r--r--   0        0        0     6432 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/oauth/oauth_client.py
+-rw-r--r--   0        0        0     8833 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/oauth/oauth_data_adaptor.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/patches/__init__.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 apricot_server-0.0.6/apricot/patches/ldap_string.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 apricot_server-0.0.6/docker/docker-compose.yaml
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 apricot_server-0.0.6/docker/entrypoint.sh
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 apricot_server-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 apricot_server-0.0.6/LICENSE
+-rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 apricot_server-0.0.6/README.md
+-rw-r--r--   0        0        0     4749 2020-02-02 00:00:00.000000 apricot_server-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     8287 2020-02-02 00:00:00.000000 apricot_server-0.0.6/PKG-INFO
```

### Comparing `apricot_server-0.0.4/.github/workflows/lint.yaml` & `apricot_server-0.0.6/.github/workflows/lint.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -6,40 +6,43 @@
   push:
     branches: [main]
   pull_request:
     branches: [main]
 
 jobs:
   lint_markdown:
+    name: Lint Markdown files
     runs-on: ubuntu-latest
     steps:
       - name: Checkout code
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
       - name: Lint Markdown
         uses: articulate/actions-markdownlint@v1
         with:
           config: .markdownlint.json
 
   lint_python:
+    name: Lint Python files
     runs-on: ubuntu-latest
     steps:
       - name: Checkout code
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: 3.11
       - name: Install hatch
         run: pip install hatch
       - name: Lint Python
         run: hatch run lint:all
 
   lint_yaml:
+    name: Lint YAML files
     runs-on: ubuntu-latest
     steps:
       - name: Checkout code
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
       - name: Lint YAML
         uses: karancode/yamllint-github-action@v2.1.1
         with:
           yamllint_strict: true
           yamllint_comment: false
```

### Comparing `apricot_server-0.0.4/.github/workflows/publish_docker.yaml` & `apricot_server-0.0.6/.github/workflows/publish_docker.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -16,29 +16,28 @@
     name: Build Docker image and publish to GitHub container repository
     runs-on: ubuntu-latest
     permissions:
       packages: write
       contents: read
     steps:
       - name: Check out the repo
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
 
       - name: Log in to the Container registry
-        uses: docker/login-action@v2
+        uses: docker/login-action@v3
         with:
           registry: ghcr.io
           username: ${{ github.actor }}
           password: ${{ secrets.GITHUB_TOKEN }}
 
       - name: Extract metadata (tags, labels) for Docker
         id: meta
-        uses: docker/metadata-action@v4
+        uses: docker/metadata-action@v5
         with:
-          images: |
-            ghcr.io/${{ github.repository }}
+          images: ghcr.io/${{ github.repository }}
 
       - name: Build and publish Docker images
-        uses: docker/build-push-action@v4
+        uses: docker/build-push-action@v5
         with:
           push: true
           tags: ${{ steps.meta.outputs.tags }}
           labels: ${{ steps.meta.outputs.labels }}
```

### Comparing `apricot_server-0.0.4/apricot/ldap/oauth_ldap_entry.py` & `apricot_server-0.0.6/apricot/ldap/oauth_ldap_entry.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import cast
+from __future__ import annotations
+
+from typing import Self, cast
 
 from ldaptor.inmemory import ReadOnlyInMemoryLDAPEntry
 from ldaptor.protocols.ldap.distinguishedname import (
     DistinguishedName,
     RelativeDistinguishedName,
 )
 from ldaptor.protocols.ldap.ldaperrors import (
@@ -12,79 +14,79 @@
 from twisted.internet import defer
 from twisted.python import log
 
 from apricot.oauth import LDAPAttributeDict, OAuthClient
 
 
 class OAuthLDAPEntry(ReadOnlyInMemoryLDAPEntry):
+    """An LDAP entry that represents a view of an OAuth object."""
+
     dn: DistinguishedName
     attributes: LDAPAttributeDict
 
     def __init__(
-        self,
+        self: Self,
         dn: DistinguishedName | str,
         attributes: LDAPAttributeDict,
         oauth_client: OAuthClient | None = None,
     ) -> None:
-        """
-        Initialize the object.
+        """Initialize the object.
 
         @param dn: Distinguished Name of the object
         @param attributes: Attributes of the object.
         @param oauth_client: An OAuth client used for binding
         """
         self.oauth_client_ = oauth_client
         if not isinstance(dn, DistinguishedName):
             dn = DistinguishedName(stringValue=dn)
         super().__init__(dn, attributes)
 
-    def __str__(self) -> str:
+    def __str__(self: Self) -> str:
         output = bytes(self.toWire()).decode("utf-8")
         for child in self._children.values():
             try:
                 # Indent children by two spaces
                 indent = "  "
                 output += (
                     f"{indent}{str(child).strip()}".replace("\n", f"\n{indent}")
                     + "\n\n"
                 )
             except TypeError:
                 pass
         return output
 
     @property
-    def oauth_client(self) -> OAuthClient:
-        if not self.oauth_client_:
-            if hasattr(self._parent, "oauth_client"):
-                self.oauth_client_ = self._parent.oauth_client
+    def oauth_client(self: Self) -> OAuthClient:
+        if not self.oauth_client_ and hasattr(self._parent, "oauth_client"):
+            self.oauth_client_ = self._parent.oauth_client
         if not isinstance(self.oauth_client_, OAuthClient):
             msg = f"OAuthClient is of incorrect type {type(self.oauth_client_)}"
             raise TypeError(msg)
         return self.oauth_client_
 
-    @property
-    def username(self) -> str:
-        username = self.dn.split()[0].getText().split("CN=")[1]
-        domain = self.dn.getDomainName()
-        return f"{username}@{domain}"
-
     def add_child(
-        self, rdn: RelativeDistinguishedName | str, attributes: LDAPAttributeDict
-    ) -> "OAuthLDAPEntry":
+        self: Self,
+        rdn: RelativeDistinguishedName | str,
+        attributes: LDAPAttributeDict,
+    ) -> OAuthLDAPEntry:
         if isinstance(rdn, str):
             rdn = RelativeDistinguishedName(stringValue=rdn)
         try:
             output = self.addChild(rdn, attributes)
         except LDAPEntryAlreadyExists:
             log.msg(f"Refusing to add child '{rdn.getText()}' as it already exists.")
             output = self._children[rdn.getText()]
         return cast(OAuthLDAPEntry, output)
 
-    def bind(self, password: bytes) -> defer.Deferred["OAuthLDAPEntry"]:
-        def _bind(password: bytes) -> "OAuthLDAPEntry":
+    def bind(self: Self, password: bytes) -> defer.Deferred[OAuthLDAPEntry]:
+        def _bind(password: bytes) -> OAuthLDAPEntry:
+            oauth_username = next(iter(self.get("oauth_username", "unknown")))
             s_password = password.decode("utf-8")
-            if self.oauth_client.verify(username=self.username, password=s_password):
+            if self.oauth_client.verify(username=oauth_username, password=s_password):
                 return self
-            msg = f"Invalid password for user '{self.username}'."
+            msg = f"Invalid password for user '{oauth_username}'."
             raise LDAPInvalidCredentials(msg)
 
         return defer.maybeDeferred(_bind, password)
+
+    def list_children(self: Self) -> list[OAuthLDAPEntry]:
+        return [cast(OAuthLDAPEntry, entry) for entry in self._children.values()]
```

### Comparing `apricot_server-0.0.4/LICENSE` & `apricot_server-0.0.6/LICENSE`

 * *Files identical despite different names*

