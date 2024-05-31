# Comparing `tmp/changy-0.1.2.tar.gz` & `tmp/changy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "changy-0.1.2.tar", max compression
+gzip compressed data, was "changy-0.3.0.tar", max compression
```

## Comparing `changy-0.1.2.tar` & `changy-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0     1504 2024-05-31 11:17:29.563136 changy-0.1.2/LICENSE
--rw-r--r--   0        0        0      358 2024-05-31 11:17:29.563136 changy-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-05-31 11:17:29.567136 changy-0.1.2/changy/__init__.py
--rw-r--r--   0        0        0        0 2024-05-31 11:17:29.567136 changy-0.1.2/changy/cli/__init__.py
--rw-r--r--   0        0        0      334 2024-05-31 11:17:29.567136 changy-0.1.2/changy/cli/__main__.py
--rw-r--r--   0        0        0       34 2024-05-31 11:17:29.567136 changy-0.1.2/changy/cli/application.py
--rw-r--r--   0        0        0      128 2024-05-31 11:17:29.567136 changy-0.1.2/changy/cli/changelog.py
--rw-r--r--   0        0        0      200 2024-05-31 11:17:29.567136 changy-0.1.2/changy/cli/unreleased.py
--rw-r--r--   0        0        0      145 2024-05-31 11:17:29.567136 changy-0.1.2/changy/cli/version.py
--rw-r--r--   0        0        0      477 2024-05-31 11:17:29.567136 changy-0.1.2/changy/constants.py
--rw-r--r--   0        0        0     2942 2024-05-31 11:17:29.567136 changy-0.1.2/changy/logic.py
--rw-r--r--   0        0        0      768 2024-05-31 11:17:29.567136 changy-0.1.2/changy/settings.py
--rw-r--r--   0        0        0        0 2024-05-31 11:17:29.567136 changy-0.1.2/changy/tests/__init__.py
--rw-r--r--   0        0        0       29 2024-05-31 11:17:29.567136 changy-0.1.2/changy/tests/test_logic.py
--rw-r--r--   0        0        0     1953 2024-05-31 11:17:37.627241 changy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1456 1970-01-01 00:00:00.000000 changy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1504 2024-05-31 14:02:52.064836 changy-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2858 2024-05-31 14:02:52.064836 changy-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-31 14:02:52.068836 changy-0.3.0/changy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 14:02:52.068836 changy-0.3.0/changy/cli/__init__.py
+-rw-r--r--   0        0        0      381 2024-05-31 14:02:52.068836 changy-0.3.0/changy/cli/__main__.py
+-rw-r--r--   0        0        0       34 2024-05-31 14:02:52.068836 changy-0.3.0/changy/cli/application.py
+-rw-r--r--   0        0        0      175 2024-05-31 14:02:52.068836 changy-0.3.0/changy/cli/changelog.py
+-rw-r--r--   0        0        0      287 2024-05-31 14:02:52.068836 changy-0.3.0/changy/cli/unreleased.py
+-rw-r--r--   0        0        0      262 2024-05-31 14:02:52.068836 changy-0.3.0/changy/cli/version.py
+-rw-r--r--   0        0        0      477 2024-05-31 14:02:52.068836 changy-0.3.0/changy/constants.py
+-rw-r--r--   0        0        0     1500 2024-05-31 14:02:52.068836 changy-0.3.0/changy/errors.py
+-rw-r--r--   0        0        0     3613 2024-05-31 14:02:52.068836 changy-0.3.0/changy/logic.py
+-rw-r--r--   0        0        0      768 2024-05-31 14:02:52.068836 changy-0.3.0/changy/settings.py
+-rw-r--r--   0        0        0        0 2024-05-31 14:02:52.068836 changy-0.3.0/changy/tests/__init__.py
+-rw-r--r--   0        0        0       29 2024-05-31 14:02:52.068836 changy-0.3.0/changy/tests/test_logic.py
+-rw-r--r--   0        0        0      231 2024-05-31 14:02:52.068836 changy-0.3.0/changy/utils.py
+-rw-r--r--   0        0        0     1953 2024-05-31 14:03:00.952864 changy-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3956 1970-01-01 00:00:00.000000 changy-0.3.0/PKG-INFO
```

### Comparing `changy-0.1.2/LICENSE` & `changy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `changy-0.1.2/changy/logic.py` & `changy-0.3.0/changy/logic.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime
 import re
 from pathlib import Path
 
 import pydantic
 
 from changy import constants as c
+from changy import errors
 from changy.settings import settings
 
 VERSION_DATETIME_FORMAT = "%Y-%m-%dT%H-%M-%S"
 CHANGES_FILE_REGEX = re.compile(r"(\d{4}-\d{2}-\d{2}T\d{2}-\d{2}-\d{2})_(.*)\.md")
 
 workdir = Path.cwd()
 configs_dir = workdir / settings.changelog_sources_dir
@@ -21,87 +22,118 @@
 next_release_file = configs_dir / settings.next_release_changes_file
 
 
 class Changes(pydantic.BaseModel):
     time: datetime.datetime
     version: str
     text: str
+    file: Path
 
     @property
     def version_header(self) -> str:
         return f"{self.version} on {self.time.strftime('%Y-%m-%d')}"
 
 
+def config_dir_must_exist():
+    if not configs_dir.exists():
+        raise errors.ChangesDirDoesNotExist(directory=configs_dir)
+
+
+def load_changes() -> list[Changes]:
+    changes_list = []
+
+    for file in configs_dir.iterdir():
+        match = CHANGES_FILE_REGEX.match(file.name)
+
+        if not match:
+            continue
+
+        time, version = match.groups()
+        text = file.read_text()
+
+        changes = Changes(
+            time=datetime.datetime.strptime(time, VERSION_DATETIME_FORMAT), file=file, version=version, text=text
+        )
+
+        changes_list.append(changes)
+
+    changes_list.sort(key=lambda x: x.time, reverse=True)
+
+    return changes_list
+
+
 def init() -> None:
 
     if configs_dir.exists():
-        raise NotImplementedError("already initialized")
+        raise errors.AlreadyInitialized()
 
     configs_dir.mkdir()
     header_file.write_text(c.default_changelog_header)
     changes_template_file.write_text(c.default_change_file_template)
 
     create_unreleased()
 
 
 def create_unreleased() -> None:
+    config_dir_must_exist()
     unreleased_changes_file.write_text(c.default_change_file_template)
 
 
 def approve_unreleased() -> None:
+    config_dir_must_exist()
+
     if not unreleased_changes_file.exists():
-        raise NotImplementedError("unreleased.md not found")
+        errors.NoUnreleasedChanges(file=unreleased_changes_file)
 
     unreleased_changes_file.rename(next_release_file)
 
 
-def create_version(version: str) -> None:
+def create_version(version: str) -> Path:
+    config_dir_must_exist()
+
+    changes = load_changes()
+
+    for change in changes:
+        if change.version == version:
+            raise errors.VersionAlreadyExists(file=change.file, version=version)
+
     time = datetime.datetime.now().strftime(VERSION_DATETIME_FORMAT)
 
     version_file_name = f"{time}_{version}.md"
 
     next_version_file = configs_dir / version_file_name
 
     if not next_release_file.exists():
-        raise NotImplementedError("next_release.md not found")
+        raise errors.NoApprovedChanges(file=next_release_file)
 
     next_release_file.rename(next_version_file)
 
     create_unreleased()
 
+    return next_version_file
+
 
 def create_changelog() -> None:
+    config_dir_must_exist()
 
     if next_release_file.exists():
-        raise NotImplementedError("Changelog is in process of updating, do something with next_release.md first")
-
-    header = header_file.read_text()
-
-    releases = []
-
-    for file in configs_dir.iterdir():
-        match = CHANGES_FILE_REGEX.match(file.name)
+        raise errors.ApprovedChangesFileExists(file=next_release_file)
 
-        if not match:
-            continue
-
-        time, version = match.groups()
-        text = file.read_text()
-
-        changes = Changes(time=datetime.datetime.strptime(time, VERSION_DATETIME_FORMAT), version=version, text=text)
+    if not unreleased_changes_file.exists():
+        raise errors.NoUnreleasedChanges(file=unreleased_changes_file)
 
-        releases.append(changes)
+    header = header_file.read_text()
 
-    releases.sort(key=lambda x: x.time, reverse=True)
+    releases = load_changes()
 
     content = [header]
 
-    if unreleased_changes_file.exists():
-        text = unreleased_changes_file.read_text()
-        unreleased_text = text.format(version_header="Unreleased")
-        content.append(unreleased_text)
+    # add unreleased changes
+    text = unreleased_changes_file.read_text()
+    unreleased_text = text.format(version_header="Unreleased")
+    content.append(unreleased_text)
 
     content.extend(change.text.format(version_header=change.version_header) for change in releases)
 
     content = [x.strip() for x in content]
 
     changelog_file.write_text("\n\n".join(content))
```

### Comparing `changy-0.1.2/changy/settings.py` & `changy-0.3.0/changy/settings.py`

 * *Files identical despite different names*

### Comparing `changy-0.1.2/pyproject.toml` & `changy-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "changy"
-version = "0.1.2"
+version = "0.3.0"
 description = "Simplest changelog manager, oriented to human editing, not to special message formatting in commits and tags.."
 readme = "README.md"
 repository = "https://github.com/Tiendil/changy"
 authors = ["Aliaksei Yaletski (Tiendil) <a.eletsky@gmail.com>"]
 license = "BSD-3-Clause"
 keywords = ["changelog", "release-notes", "release-automation", "release-management", "changelog-generator", "changelog-formatter"]
 classifiers = [
```

