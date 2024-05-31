# Comparing `tmp/pgcooldown-0.2.8.tar.gz` & `tmp/pgcooldown-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgcooldown-0.2.8.tar", last modified: Sat Sep 16 10:34:26 2023, max compression
+gzip compressed data, was "pgcooldown-0.2.9.tar", last modified: Wed Jan 24 10:06:46 2024, max compression
```

## Comparing `pgcooldown-0.2.8.tar` & `pgcooldown-0.2.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-09-16 10:34:26.397270 pgcooldown-0.2.8/
--rw-rw-rw-   0        0        0     1093 2023-08-02 10:18:55.000000 pgcooldown-0.2.8/LICENSE
--rw-rw-rw-   0        0        0     2625 2023-09-16 10:34:26.396264 pgcooldown-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     1907 2023-08-30 21:39:47.000000 pgcooldown-0.2.8/README.md
--rw-rw-rw-   0        0        0      923 2023-09-16 10:24:26.000000 pgcooldown-0.2.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-09-16 10:34:26.397270 pgcooldown-0.2.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-09-16 10:34:26.379266 pgcooldown-0.2.8/src/
-drwxrwxrwx   0        0        0        0 2023-09-16 10:34:26.382266 pgcooldown-0.2.8/src/pgcooldown/
--rw-rw-rw-   0        0        0    17381 2023-09-16 10:32:34.000000 pgcooldown-0.2.8/src/pgcooldown/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-16 10:34:26.393263 pgcooldown-0.2.8/src/pgcooldown.egg-info/
--rw-rw-rw-   0        0        0     2625 2023-09-16 10:34:26.000000 pgcooldown-0.2.8/src/pgcooldown.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-09-16 10:34:26.000000 pgcooldown-0.2.8/src/pgcooldown.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-16 10:34:26.000000 pgcooldown-0.2.8/src/pgcooldown.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-09-16 10:34:26.000000 pgcooldown-0.2.8/src/pgcooldown.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-09-16 10:34:26.395266 pgcooldown-0.2.8/tests/
--rw-rw-rw-   0        0        0     3460 2023-09-16 10:04:31.000000 pgcooldown-0.2.8/tests/test_cooldown.py
--rw-rw-rw-   0        0        0      942 2023-08-21 13:55:56.000000 pgcooldown-0.2.8/tests/test_crond.py
--rw-rw-rw-   0        0        0     1639 2023-09-16 10:08:54.000000 pgcooldown-0.2.8/tests/test_lerpthing.py
+drwxrwxrwx   0        0        0        0 2024-01-24 10:06:46.157128 pgcooldown-0.2.9/
+-rw-rw-rw-   0        0        0     1093 2023-08-02 10:18:55.000000 pgcooldown-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0     3854 2024-01-24 10:06:46.156121 pgcooldown-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3024 2024-01-23 17:30:00.000000 pgcooldown-0.2.9/README.md
+-rw-rw-rw-   0        0        0      923 2024-01-24 10:05:24.000000 pgcooldown-0.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-01-24 10:06:46.157128 pgcooldown-0.2.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-01-24 10:06:46.138112 pgcooldown-0.2.9/src/
+drwxrwxrwx   0        0        0        0 2024-01-24 10:06:46.141103 pgcooldown-0.2.9/src/pgcooldown/
+-rw-rw-rw-   0        0        0    17581 2024-01-24 09:29:16.000000 pgcooldown-0.2.9/src/pgcooldown/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-24 10:06:46.155116 pgcooldown-0.2.9/src/pgcooldown.egg-info/
+-rw-rw-rw-   0        0        0     3854 2024-01-24 10:06:46.000000 pgcooldown-0.2.9/src/pgcooldown.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-01-24 10:06:46.000000 pgcooldown-0.2.9/src/pgcooldown.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-01-24 10:06:46.000000 pgcooldown-0.2.9/src/pgcooldown.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-01-24 10:06:46.000000 pgcooldown-0.2.9/src/pgcooldown.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-01-24 10:06:46.153612 pgcooldown-0.2.9/tests/
+-rw-rw-rw-   0        0        0     3777 2024-01-24 09:36:34.000000 pgcooldown-0.2.9/tests/test_cooldown.py
+-rw-rw-rw-   0        0        0      942 2023-08-21 13:55:56.000000 pgcooldown-0.2.9/tests/test_crond.py
+-rw-rw-rw-   0        0        0     1639 2023-09-16 10:08:54.000000 pgcooldown-0.2.9/tests/test_lerpthing.py
```

### Comparing `pgcooldown-0.2.8/LICENSE` & `pgcooldown-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pgcooldown-0.2.8/PKG-INFO` & `pgcooldown-0.2.9/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,59 @@
 Metadata-Version: 2.1
 Name: pgcooldown
-Version: 0.2.8
+Version: 0.2.9
 Summary: A cooldown/counter class to wait for stuff in games
 Author-email: Michael Lamertz <michael.lamertz@gmail.com>
 Project-URL: homepage, https://github.com/dickerdackel/pgcooldown
 Project-URL: bugtracker, https://github.com/DickerDackel/pgcooldown/issues
 Project-URL: changelog, https://github.com/dickerdackel/pgcooldown/ChangeLog.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Software Development :: Libraries :: pygame
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# IMPORTANT
+Breaking change!  Properties gone!
+
+I was aware, that there is a slight overhead when using properties, but
+during A benchmark, that difference turned out to be 17%.
+
+Since this package is still marked as Alpha and probably nobody is using
+it besides me, the interface is now changed from properties to functions
+in all places.
+
+Tests needed to be adapted, but run clean now (and also more exact using
+`pytest.approx` instead of `round`.
+
+The following properties now need to be called as functions:
+
+```
+    cold                -> cold()
+    cold.setter         -> set_cold(bool)
+    hot                 -> hot()
+    temperature         -> temperature()
+    temperature.setter  -> set_to(val)
+    remaining           -> remaining()
+    remaining.setter    -> set_to(val)
+    normalized          -> normalized()
+    v                   -> removed, just use instance()
+```
+
+As stated initially, this is 17% less overhead when testing for cold,
+etc.  Performance of LerpThing increased from 1.3mio calls to 1.8mio due
+to this change.
+
+Sorry for any inconvenience, if anybody is using this, but that bad
+design decision needed to be fixed before any more people would use this.
+
+---
+
 # pgcooldown
 
 Cooldown & co...
 
 This module started with just the Cooldown class, which can be used check if a
 specified time has passed.  It is mostly indended to be used to control
 objects in a game loop, but it is general enough for other purposes as well.
```

### Comparing `pgcooldown-0.2.8/pyproject.toml` & `pgcooldown-0.2.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "pgcooldown"
 description = "A cooldown/counter class to wait for stuff in games"
-version = "0.2.8"
+version = "0.2.9"
 readme = "README.md"
 
 authors = [
     { name="Michael Lamertz", email="michael.lamertz@gmail.com" }
 ]
 
 classifiers = [
```

### Comparing `pgcooldown-0.2.8/src/pgcooldown/__init__.py` & `pgcooldown-0.2.9/src/pgcooldown/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,27 +126,30 @@
         Has the time of the cooldown run out?
 
     hot: bool
         Is there stil time remaining before cooldown?  This is just for
         convenience to not write `cooldown not cold` all over the place.
 
     """
-    def __init__(self, duration, cold=False):
+    def __init__(self, duration, cold=False, paused=False):
         if isinstance(duration, Cooldown):
             self.duration = duration.duration
         else:
             self.duration = float(duration)
         self.t0 = time.time()
-        self.paused = False
-        self._remaining = 0
+        self.paused = paused
+        self._remaining = duration if paused else 0
         self.set_cold(cold)
 
     def __call__(self):
         return self.remaining()
 
+    def __repr__(self):
+        return f'Cooldown(duration={self.duration}, cold={self.cold()}, paused={self.paused})'
+
     def __hash__(self): id(self)  # noqa: E704
     def __bool__(self): return self.hot()  # noqa: E704
     def __int__(self): return int(self.temperature())  # noqa: E704
     def __float__(self): return float(self.temperature())  # noqa: E704
     def __lt__(self, other): return float(self) < other  # noqa: E704
     def __le__(self, other): return float(self) <= other  # noqa: E704
     def __eq__(self, other): return float(self) == other  # noqa: E704
@@ -156,14 +159,16 @@
 
     def reset(self, new=0, wrap=False):
         """reset the cooldown, optionally pass a new temperature.
 
         To reuse the cooldown, it can be reset at any time, optionally with a
         new duration.
 
+        reset() also clears pause.
+
         Parameters
         ----------
         new: float = 0
             If not 0, set a new timeout value for the cooldown
 
         wrap: bool = False
             If `wrap` is `True` and the cooldown is cold, take the time
```

### Comparing `pgcooldown-0.2.8/src/pgcooldown.egg-info/PKG-INFO` & `pgcooldown-0.2.9/src/pgcooldown.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,59 @@
 Metadata-Version: 2.1
 Name: pgcooldown
-Version: 0.2.8
+Version: 0.2.9
 Summary: A cooldown/counter class to wait for stuff in games
 Author-email: Michael Lamertz <michael.lamertz@gmail.com>
 Project-URL: homepage, https://github.com/dickerdackel/pgcooldown
 Project-URL: bugtracker, https://github.com/DickerDackel/pgcooldown/issues
 Project-URL: changelog, https://github.com/dickerdackel/pgcooldown/ChangeLog.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Software Development :: Libraries :: pygame
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# IMPORTANT
+Breaking change!  Properties gone!
+
+I was aware, that there is a slight overhead when using properties, but
+during A benchmark, that difference turned out to be 17%.
+
+Since this package is still marked as Alpha and probably nobody is using
+it besides me, the interface is now changed from properties to functions
+in all places.
+
+Tests needed to be adapted, but run clean now (and also more exact using
+`pytest.approx` instead of `round`.
+
+The following properties now need to be called as functions:
+
+```
+    cold                -> cold()
+    cold.setter         -> set_cold(bool)
+    hot                 -> hot()
+    temperature         -> temperature()
+    temperature.setter  -> set_to(val)
+    remaining           -> remaining()
+    remaining.setter    -> set_to(val)
+    normalized          -> normalized()
+    v                   -> removed, just use instance()
+```
+
+As stated initially, this is 17% less overhead when testing for cold,
+etc.  Performance of LerpThing increased from 1.3mio calls to 1.8mio due
+to this change.
+
+Sorry for any inconvenience, if anybody is using this, but that bad
+design decision needed to be fixed before any more people would use this.
+
+---
+
 # pgcooldown
 
 Cooldown & co...
 
 This module started with just the Cooldown class, which can be used check if a
 specified time has passed.  It is mostly indended to be used to control
 objects in a game loop, but it is general enough for other purposes as well.
```

### Comparing `pgcooldown-0.2.8/tests/test_cooldown.py` & `pgcooldown-0.2.9/tests/test_cooldown.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,26 @@
     assert not c.hot()
 
     c = Cooldown(0)
     assert c.cold()
     assert c.remaining() == 0
     assert not c.hot()
 
+    c = Cooldown(10, paused=True)
+    assert c.paused
+    assert c.remaining() == 10
+    c.start()
+    sleep(1)
+    assert approx(c.remaining(), abs=0.01) == c.duration - 1
+
+
+def test_repr():
+    c = Cooldown(10)
+    assert repr(c) == 'Cooldown(duration=10.0, cold=False, paused=False)'
+
 
 def test_cold():
     c = Cooldown(0.1)
     sleep(0.2)
     assert c.cold()
 
     c = Cooldown(1)
@@ -139,14 +151,15 @@
     assert bool(c)
     assert int(c) == 10
     assert float(c) == 10.0
 
 
 if __name__ == '__main__':
     test_init()
+    test_repr()
     test_cold()
     test_reset()
     test_wrap()
     test_remaining()
     test_set_to()
     test_pause()
     test_normalized()
```

### Comparing `pgcooldown-0.2.8/tests/test_crond.py` & `pgcooldown-0.2.9/tests/test_crond.py`

 * *Files identical despite different names*

### Comparing `pgcooldown-0.2.8/tests/test_lerpthing.py` & `pgcooldown-0.2.9/tests/test_lerpthing.py`

 * *Files identical despite different names*

