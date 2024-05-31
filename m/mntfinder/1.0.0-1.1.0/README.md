# Comparing `tmp/mntfinder-1.0.0.tar.gz` & `tmp/mntfinder-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mntfinder-1.0.0.tar", last modified: Sat May 25 17:02:35 2024, max compression
+gzip compressed data, was "mntfinder-1.1.0.tar", last modified: Fri May 31 15:27:56 2024, max compression
```

## Comparing `mntfinder-1.0.0.tar` & `mntfinder-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwx------   0 miketsu   (1000) miketsu   (1000)        0 2024-05-25 17:02:35.542869 mntfinder-1.0.0/
--rw-------   0 miketsu   (1000) miketsu   (1000)     1094 2024-01-04 17:03:50.000000 mntfinder-1.0.0/LICENSE
--rw-r--r--   0 miketsu   (1000) miketsu   (1000)     7351 2024-05-25 17:02:35.542869 mntfinder-1.0.0/PKG-INFO
--rw-------   0 miketsu   (1000) miketsu   (1000)     5413 2024-05-25 17:02:13.000000 mntfinder-1.0.0/README.md
--rw-------   0 miketsu   (1000) miketsu   (1000)     1004 2024-01-07 18:46:09.000000 mntfinder-1.0.0/pyproject.toml
--rw-------   0 miketsu   (1000) miketsu   (1000)        6 2024-01-07 18:51:16.000000 mntfinder-1.0.0/requirements.txt
--rw-------   0 miketsu   (1000) miketsu   (1000)       38 2024-05-25 17:02:35.542869 mntfinder-1.0.0/setup.cfg
-drwx------   0 miketsu   (1000) miketsu   (1000)        0 2024-05-25 17:02:35.541869 mntfinder-1.0.0/src/
-drwx------   0 miketsu   (1000) miketsu   (1000)        0 2024-05-25 17:02:35.542869 mntfinder-1.0.0/src/mntfinder.egg-info/
--rw-r--r--   0 miketsu   (1000) miketsu   (1000)     7351 2024-05-25 17:02:35.000000 mntfinder-1.0.0/src/mntfinder.egg-info/PKG-INFO
--rw-------   0 miketsu   (1000) miketsu   (1000)      250 2024-05-25 17:02:35.000000 mntfinder-1.0.0/src/mntfinder.egg-info/SOURCES.txt
--rw-------   0 miketsu   (1000) miketsu   (1000)        1 2024-05-25 17:02:35.000000 mntfinder-1.0.0/src/mntfinder.egg-info/dependency_links.txt
--rw-------   0 miketsu   (1000) miketsu   (1000)        6 2024-05-25 17:02:35.000000 mntfinder-1.0.0/src/mntfinder.egg-info/requires.txt
--rw-------   0 miketsu   (1000) miketsu   (1000)       10 2024-05-25 17:02:35.000000 mntfinder-1.0.0/src/mntfinder.egg-info/top_level.txt
--rw-------   0 miketsu   (1000) miketsu   (1000)     6139 2024-05-25 17:02:13.000000 mntfinder-1.0.0/src/mntfinder.py
+drwx------   0 miketsu   (1000) miketsu   (1000)        0 2024-05-31 15:27:56.894797 mntfinder-1.1.0/
+-rw-------   0 miketsu   (1000) miketsu   (1000)     1094 2024-01-04 17:03:50.000000 mntfinder-1.1.0/LICENSE
+-rw-r--r--   0 miketsu   (1000) miketsu   (1000)    11270 2024-05-31 15:27:56.893797 mntfinder-1.1.0/PKG-INFO
+-rw-------   0 miketsu   (1000) miketsu   (1000)     9332 2024-05-31 15:19:17.000000 mntfinder-1.1.0/README.md
+-rw-------   0 miketsu   (1000) miketsu   (1000)     1004 2024-01-07 18:46:09.000000 mntfinder-1.1.0/pyproject.toml
+-rw-------   0 miketsu   (1000) miketsu   (1000)        6 2024-01-07 18:51:16.000000 mntfinder-1.1.0/requirements.txt
+-rw-------   0 miketsu   (1000) miketsu   (1000)       38 2024-05-31 15:27:56.894797 mntfinder-1.1.0/setup.cfg
+drwx------   0 miketsu   (1000) miketsu   (1000)        0 2024-05-31 15:27:56.892798 mntfinder-1.1.0/src/
+drwx------   0 miketsu   (1000) miketsu   (1000)        0 2024-05-31 15:27:56.893797 mntfinder-1.1.0/src/mntfinder.egg-info/
+-rw-r--r--   0 miketsu   (1000) miketsu   (1000)    11270 2024-05-31 15:27:56.000000 mntfinder-1.1.0/src/mntfinder.egg-info/PKG-INFO
+-rw-------   0 miketsu   (1000) miketsu   (1000)      250 2024-05-31 15:27:56.000000 mntfinder-1.1.0/src/mntfinder.egg-info/SOURCES.txt
+-rw-------   0 miketsu   (1000) miketsu   (1000)        1 2024-05-31 15:27:56.000000 mntfinder-1.1.0/src/mntfinder.egg-info/dependency_links.txt
+-rw-------   0 miketsu   (1000) miketsu   (1000)        6 2024-05-31 15:27:56.000000 mntfinder-1.1.0/src/mntfinder.egg-info/requires.txt
+-rw-------   0 miketsu   (1000) miketsu   (1000)       10 2024-05-31 15:27:56.000000 mntfinder-1.1.0/src/mntfinder.egg-info/top_level.txt
+-rw-------   0 miketsu   (1000) miketsu   (1000)     6556 2024-05-31 15:26:44.000000 mntfinder-1.1.0/src/mntfinder.py
```

### Comparing `mntfinder-1.0.0/LICENSE` & `mntfinder-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mntfinder-1.0.0/pyproject.toml` & `mntfinder-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mntfinder-1.0.0/src/mntfinder.py` & `mntfinder-1.1.0/src/mntfinder.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # -*- encoding: utf-8 -*-
 import os
+import warnings
 from pathlib import PosixPath as Path
 from typing import Iterator
 
 import attrs
 
 __all__ = ['MountPointInfo', 'getMountPoint', 'getAllMountPoints', 'isAMountPoint']
 
-__version__ = '1.0.0'
+__version__ = '1.1.0'
 
 
-@attrs.define(slots=True, kw_only=True, eq=False, order=False)
+@attrs.frozen(slots=True, kw_only=True, eq=False, order=False, hash=True)
 class MountPointInfo(os.PathLike[str]):
     """
     A class representing information about a mount point.
 
     The instance can be used as path-like objects by ``os.path.*``, ``pathlib.Path``, etc.
     When the instance is used as a path, it reflects the value of the attribute ``target``.
 
@@ -23,65 +24,84 @@
         target (Path): The target path of the mount point.
         fstype (str): The file system type of the mount point.
         options (tuple[str, ...]): The options associated with the mount point.
         freq (int): The frequency of filesystem checks.
         passno (int): The pass number used by the filesystem checker.
 
     Methods:
-        isStillMounted(self) -> bool:
+        isAlive(self) -> bool:
             Returns ``False`` when called if attribute ``target`` is no longer a mount point; otherwise it returns ``True``.
-
-            Once this method starts returning ``False``, it will not return ``True`` on any subsequent calls.
+        isStillMounted(self) -> bool:
+            Deprecated. Use method ``isAlive()`` instead.
     """
-    source: str = attrs.field(validator=attrs.validators.instance_of(str), on_setattr=attrs.setters.frozen)
-    target: Path = attrs.field(validator=attrs.validators.instance_of(Path), on_setattr=attrs.setters.frozen)
-    fstype: str = attrs.field(validator=attrs.validators.instance_of(str), on_setattr=attrs.setters.frozen)
+    source: str = attrs.field(validator=attrs.validators.instance_of(str))
+    target: Path = attrs.field(validator=attrs.validators.instance_of(Path))
+    fstype: str = attrs.field(validator=attrs.validators.instance_of(str))
     options: tuple[str, ...] = attrs.field(
         validator=attrs.validators.deep_iterable(
             attrs.validators.instance_of(str),
             attrs.validators.instance_of(tuple)
-        ),
-        on_setattr=attrs.setters.frozen
+        )
     )
-    freq: int = attrs.field(validator=attrs.validators.instance_of(int), on_setattr=attrs.setters.frozen)
-    passno: int = attrs.field(validator=attrs.validators.instance_of(int), on_setattr=attrs.setters.frozen)
-    __mounted: bool = attrs.field(init=False, repr=False, default=True)
+    freq: int = attrs.field(validator=attrs.validators.instance_of(int))
+    passno: int = attrs.field(validator=attrs.validators.instance_of(int))
+
+    def __eq(self, other: 'MountPointInfo', /) -> bool:
+        return all(
+            getattr(self, attr) == getattr(other, attr) for attr in attrs.asdict(self)  # type:ignore
+        )
 
     def __eq__(self, other: 'MountPointInfo', /) -> bool:
         if type(other) is not type(self):
             return NotImplemented
-        if not self.isStillMounted():
+        return self.isAlive() and other.isAlive() and self.__eq(other)
+
+    def __lt__(self, other: 'MountPointInfo', /) -> bool:
+        if type(other) is not type(self):
             return NotImplemented
-        if not other.isStillMounted():
+        return self.target < other.target
+
+    def __le__(self, other: 'MountPointInfo', /) -> bool:
+        return NotImplemented
+
+    def __gt__(self, other: 'MountPointInfo', /) -> bool:
+        if type(other) is not type(self):
             return NotImplemented
-        return (
-                other.source == self.source
-                and other.target == self.target
-                and other.fstype == self.fstype
-                and other.options == self.options
-                and other.freq == self.freq
-                and other.passno == self.passno
-        )
+        return self.target > other.target
+
+    def __ge__(self, other: 'MountPointInfo', /) -> bool:
+        return NotImplemented
 
     def __fspath__(self) -> str:
         return os.fspath(self.target)
 
     def isStillMounted(self) -> bool:
         """
         Returns ``False`` when called if attribute ``target`` is no longer a mount point; otherwise it returns ``True``.
 
-        Once this method starts returning ``False``, it will not return ``True`` on any subsequent calls.
+        Now this method is deprecated, please use method ``isAlive()`` instead.
+        """
+        warnings.warn(
+            'Method isStillMounted() is deprecated. Please use method isAlive() instead.',
+            DeprecationWarning
+        )
+        return self.isAlive()
+
+    def isAlive(self) -> bool:
+        """
+        Returns ``False`` when called if attribute ``target`` is no longer a mount point; otherwise it returns ``True``.
         """
-        if not self.__mounted:
-            return self.__mounted
+        if os.path.ismount(self.target):
+            try:
+                if mnt := getMountPoint(self.target):
+                    return self.__eq(mnt)
+            except ValueError:
+                pass
 
-        mounted = self.target.is_mount()
-        if not mounted:
-            self.__mounted = mounted
-        return mounted
+        return False
 
 
 def _mountsFileLineToMountPointInfo(line: str) -> MountPointInfo:
     line_parts = [s.replace('\\040', ' ').replace('\\012', '\n') for s in line.strip(' \n').split(' ')]
     if len(line_parts) != 6:
         raise ValueError(f'Not a valid line of mount info: {line!r}')
 
@@ -100,24 +120,23 @@
 
     target = Path(str(bytes(raw_target, encoding='raw_unicode_escape'), encoding='unicode_escape')).resolve()
 
     return MountPointInfo(source=source, target=target, fstype=fstype, options=options, freq=freq, passno=passno)
 
 
 def _iteratedParseMountInfoFile() -> Iterator[MountPointInfo]:
-    mount_info_file = Path('/proc') / 'mounts'
+    mount_info_file = Path('/proc/mounts')
 
     with open(mount_info_file, mode='r', newline='') as f:
         mount_info_text = f.read()
 
     for line in mount_info_text.split('\n'):
         if line:
             mount_point_info = _mountsFileLineToMountPointInfo(line)
-            if mount_point_info.isStillMounted():
-                yield mount_point_info
+            yield mount_point_info
 
 
 def getMountPoint(target: str | bytes | os.PathLike) -> MountPointInfo | None:
     """
     Get the ``MountPointInfo`` object corresponding to the given target path.
 
     Parameters:
@@ -152,9 +171,11 @@
     Parameters:
         target (str | bytes | os.PathLike | MountPointInfo): The target to check if it is a mount point or not.
 
     Returns:
         bool: ``True`` if the ``target`` is a mount point and still mounted, ``False`` otherwise.
     """
     if isinstance(target, MountPointInfo):
-        return target.isStillMounted()
-    return bool(getMountPoint(target))
+        return target.isAlive()
+    if mnt := getMountPoint(target):
+        return mnt.isAlive()
+    return False
```

