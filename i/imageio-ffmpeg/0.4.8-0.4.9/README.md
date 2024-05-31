# Comparing `tmp/imageio-ffmpeg-0.4.8.tar.gz` & `tmp/imageio-ffmpeg-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imageio-ffmpeg-0.4.8.tar", last modified: Mon Jan  9 20:34:36 2023, max compression
+gzip compressed data, was "imageio-ffmpeg-0.4.9.tar", last modified: Tue Sep 12 10:01:36 2023, max compression
```

## Comparing `imageio-ffmpeg-0.4.8.tar` & `imageio-ffmpeg-0.4.9.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-01-09 20:34:36.757922 imageio-ffmpeg-0.4.8/
--rw-r--r--   0 almar      (501) staff       (20)     1312 2022-01-25 10:14:00.000000 imageio-ffmpeg-0.4.8/LICENSE
--rw-r--r--   0 almar      (501) staff       (20)       34 2022-01-25 10:14:00.000000 imageio-ffmpeg-0.4.8/MANIFEST.in
--rw-r--r--   0 almar      (501) staff       (20)     1575 2023-01-09 20:34:36.757127 imageio-ffmpeg-0.4.8/PKG-INFO
--rw-r--r--   0 almar      (501) staff       (20)     9725 2023-01-09 20:32:52.000000 imageio-ffmpeg-0.4.8/README.md
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-01-09 20:34:36.748029 imageio-ffmpeg-0.4.8/imageio_ffmpeg/
--rw-r--r--   0 almar      (501) staff       (20)      227 2022-01-25 10:14:00.000000 imageio-ffmpeg-0.4.8/imageio_ffmpeg/__init__.py
--rw-r--r--   0 almar      (501) staff       (20)     1609 2023-01-09 20:33:55.000000 imageio-ffmpeg-0.4.8/imageio_ffmpeg/_definitions.py
--rw-r--r--   0 almar      (501) staff       (20)    26953 2023-01-03 22:52:41.000000 imageio-ffmpeg-0.4.8/imageio_ffmpeg/_io.py
--rw-r--r--   0 almar      (501) staff       (20)     6925 2023-01-04 13:05:51.000000 imageio-ffmpeg-0.4.8/imageio_ffmpeg/_parsing.py
--rw-r--r--   0 almar      (501) staff       (20)     3470 2023-01-03 22:52:41.000000 imageio-ffmpeg-0.4.8/imageio_ffmpeg/_utils.py
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-01-09 20:34:36.756413 imageio-ffmpeg-0.4.8/imageio_ffmpeg/binaries/
--rw-r--r--   0 almar      (501) staff       (20)       45 2022-01-25 10:14:00.000000 imageio-ffmpeg-0.4.8/imageio_ffmpeg/binaries/README.md
-drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-01-09 20:34:36.755955 imageio-ffmpeg-0.4.8/imageio_ffmpeg.egg-info/
--rw-r--r--   0 almar      (501) staff       (20)     1575 2023-01-09 20:34:36.000000 imageio-ffmpeg-0.4.8/imageio_ffmpeg.egg-info/PKG-INFO
--rw-r--r--   0 almar      (501) staff       (20)      393 2023-01-09 20:34:36.000000 imageio-ffmpeg-0.4.8/imageio_ffmpeg.egg-info/SOURCES.txt
--rw-r--r--   0 almar      (501) staff       (20)        1 2023-01-09 20:34:36.000000 imageio-ffmpeg-0.4.8/imageio_ffmpeg.egg-info/dependency_links.txt
--rw-r--r--   0 almar      (501) staff       (20)        1 2023-01-09 20:34:36.000000 imageio-ffmpeg-0.4.8/imageio_ffmpeg.egg-info/not-zip-safe
--rw-r--r--   0 almar      (501) staff       (20)       15 2023-01-09 20:34:36.000000 imageio-ffmpeg-0.4.8/imageio_ffmpeg.egg-info/top_level.txt
--rw-r--r--   0 almar      (501) staff       (20)       38 2023-01-09 20:34:36.757975 imageio-ffmpeg-0.4.8/setup.cfg
--rw-r--r--   0 almar      (501) staff       (20)     2698 2022-04-13 08:52:15.000000 imageio-ffmpeg-0.4.8/setup.py
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-09-12 10:01:36.106277 imageio-ffmpeg-0.4.9/
+-rw-r--r--   0 almar      (501) staff       (20)     1312 2022-01-25 10:14:00.000000 imageio-ffmpeg-0.4.9/LICENSE
+-rw-r--r--   0 almar      (501) staff       (20)       34 2022-01-25 10:14:00.000000 imageio-ffmpeg-0.4.9/MANIFEST.in
+-rw-r--r--   0 almar      (501) staff       (20)     1626 2023-09-12 10:01:36.106146 imageio-ffmpeg-0.4.9/PKG-INFO
+-rw-r--r--   0 almar      (501) staff       (20)     9941 2023-09-11 13:59:57.000000 imageio-ffmpeg-0.4.9/README.md
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-09-12 10:01:36.104728 imageio-ffmpeg-0.4.9/imageio_ffmpeg/
+-rw-r--r--   0 almar      (501) staff       (20)      227 2023-09-11 13:59:57.000000 imageio-ffmpeg-0.4.9/imageio_ffmpeg/__init__.py
+-rw-r--r--   0 almar      (501) staff       (20)     1739 2023-09-12 09:58:53.000000 imageio-ffmpeg-0.4.9/imageio_ffmpeg/_definitions.py
+-rw-r--r--   0 almar      (501) staff       (20)    27047 2023-09-11 13:59:57.000000 imageio-ffmpeg-0.4.9/imageio_ffmpeg/_io.py
+-rw-r--r--   0 almar      (501) staff       (20)     6840 2023-09-12 09:52:53.000000 imageio-ffmpeg-0.4.9/imageio_ffmpeg/_parsing.py
+-rw-r--r--   0 almar      (501) staff       (20)     3471 2023-09-11 13:59:57.000000 imageio-ffmpeg-0.4.9/imageio_ffmpeg/_utils.py
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-09-12 10:01:36.105962 imageio-ffmpeg-0.4.9/imageio_ffmpeg/binaries/
+-rw-r--r--   0 almar      (501) staff       (20)       45 2022-01-25 10:14:00.000000 imageio-ffmpeg-0.4.9/imageio_ffmpeg/binaries/README.md
+drwxr-xr-x   0 almar      (501) staff       (20)        0 2023-09-12 10:01:36.105812 imageio-ffmpeg-0.4.9/imageio_ffmpeg.egg-info/
+-rw-r--r--   0 almar      (501) staff       (20)     1626 2023-09-12 10:01:35.000000 imageio-ffmpeg-0.4.9/imageio_ffmpeg.egg-info/PKG-INFO
+-rw-r--r--   0 almar      (501) staff       (20)      430 2023-09-12 10:01:36.000000 imageio-ffmpeg-0.4.9/imageio_ffmpeg.egg-info/SOURCES.txt
+-rw-r--r--   0 almar      (501) staff       (20)        1 2023-09-12 10:01:35.000000 imageio-ffmpeg-0.4.9/imageio_ffmpeg.egg-info/dependency_links.txt
+-rw-r--r--   0 almar      (501) staff       (20)        1 2023-09-12 10:01:35.000000 imageio-ffmpeg-0.4.9/imageio_ffmpeg.egg-info/not-zip-safe
+-rw-r--r--   0 almar      (501) staff       (20)       11 2023-09-12 10:01:35.000000 imageio-ffmpeg-0.4.9/imageio_ffmpeg.egg-info/requires.txt
+-rw-r--r--   0 almar      (501) staff       (20)       15 2023-09-12 10:01:35.000000 imageio-ffmpeg-0.4.9/imageio_ffmpeg.egg-info/top_level.txt
+-rw-r--r--   0 almar      (501) staff       (20)       38 2023-09-12 10:01:36.106318 imageio-ffmpeg-0.4.9/setup.cfg
+-rw-r--r--   0 almar      (501) staff       (20)     2752 2023-09-12 09:52:53.000000 imageio-ffmpeg-0.4.9/setup.py
```

### Comparing `imageio-ffmpeg-0.4.8/LICENSE` & `imageio-ffmpeg-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `imageio-ffmpeg-0.4.8/PKG-INFO` & `imageio-ffmpeg-0.4.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imageio-ffmpeg
-Version: 0.4.8
+Version: 0.4.9
 Summary: FFMPEG wrapper for Python
 Home-page: https://github.com/imageio/imageio-ffmpeg
 Download-URL: http://pypi.python.org/pypi/imageio-ffmpeg
 Author: imageio contributors
 Author-email: almar.klein@gmail.com
 License: BSD-2-Clause
 Keywords: video ffmpeg
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides: imageio_ffmpeg
 Requires-Python: >=3.5
 License-File: LICENSE
 
 FFMPEG wrapper for Python.
 
 Note that the platform-specific wheels contain the binary executable
```

### Comparing `imageio-ffmpeg-0.4.8/README.md` & `imageio-ffmpeg-0.4.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -103,14 +103,29 @@
 
 The library can be configured at runtime by setting the following environment
 variables:
 * `IMAGEIO_FFMPEG_EXE=[file name]` -- override the ffmpeg executable;
 * `IMAGEIO_FFMPEG_NO_PREVENT_SIGINT=1` -- don't prevent propagation of SIGINT
   to the ffmpeg process.
 
+## Developers
+
+Dev deps:
+```
+pip install invoke black flake8
+```
+
+We use invoke:
+
+```
+invoke autoformat
+invoke lint
+invoke -l  # to get a list of all tasks
+invoke update-readme  # after changes to the docstrings
+```
 
 ## API
 
 ```py
 def read_frames(
     path,
     pix_fmt="rgb24",
```

### Comparing `imageio-ffmpeg-0.4.8/imageio_ffmpeg/_definitions.py` & `imageio-ffmpeg-0.4.9/imageio_ffmpeg/_definitions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-import sys
+import platform
 import struct
+import sys
 
-__version__ = "0.4.8"
+__version__ = "0.4.9"
 
 
 def get_platform():
     bits = struct.calcsize("P") * 8
     if sys.platform.startswith("linux"):
+        architecture = platform.machine()
+        if architecture == "aarch64":
+            return "linuxaarch64"
         return "linux{}".format(bits)
     elif sys.platform.startswith("freebsd"):
         return "freebsd{}".format(bits)
     elif sys.platform.startswith("win"):
         return "win{}".format(bits)
     elif sys.platform.startswith("cygwin"):
         return "win{}".format(bits)
```

### Comparing `imageio-ffmpeg-0.4.8/imageio_ffmpeg/_io.py` & `imageio-ffmpeg-0.4.9/imageio_ffmpeg/_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-import sys
-import time
 import pathlib
 import subprocess
-from functools import lru_cache
+import sys
+import time
 from collections import defaultdict
+from functools import lru_cache
 
-from ._utils import get_ffmpeg_exe, _popen_kwargs, logger
-from ._parsing import LogCatcher, parse_ffmpeg_header, cvsecs
-
+from ._parsing import LogCatcher, cvsecs, parse_ffmpeg_header
+from ._utils import _popen_kwargs, get_ffmpeg_exe, logger
 
 ISWIN = sys.platform.startswith("win")
 
 h264_encoder_preference = defaultdict(lambda: -1)
 # The libx264 was the default encoder for a longe time with imageio
 h264_encoder_preference["libx264"] = 100
 
@@ -160,15 +159,17 @@
         "null",
         "-",
     ]
     try:
         out = subprocess.check_output(cmd, stderr=subprocess.STDOUT, **_popen_kwargs())
     except subprocess.CalledProcessError as err:
         out = err.output.decode(errors="ignore")
-        raise RuntimeError("FFMEG call failed with {}:\n{}".format(err.returncode, out))
+        raise RuntimeError(
+            "FFMPEG call failed with {}:\n{}".format(err.returncode, out)
+        )
 
     # Note that other than with the subprocess calls below, ffmpeg wont hang here.
     # Worst case Python will stop/crash and ffmpeg will continue running until done.
 
     nframes = nsecs = None
     for line in reversed(out.splitlines()):
         if line.startswith(b"frame="):
@@ -260,33 +261,32 @@
 
     pre_output_params = ["-pix_fmt", pix_fmt, "-vcodec", "rawvideo", "-f", "image2pipe"]
 
     cmd = [get_ffmpeg_exe()]
     cmd += input_params + ["-i", path]
     cmd += pre_output_params + output_params + ["-"]
 
-    p = subprocess.Popen(
+    process = subprocess.Popen(
         cmd,
         stdin=subprocess.PIPE,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         **_popen_kwargs(prevent_sigint=True)
     )
 
-    log_catcher = LogCatcher(p.stderr)
+    log_catcher = LogCatcher(process.stderr)
 
     # Init policy by which to terminate ffmpeg. May be set to "kill" later.
     stop_policy = "timeout"  # not wait; ffmpeg should be able to quit quickly
 
     # Enter try block directly after opening the process.
     # We terminate ffmpeg in the finally clause.
     # Generators are automatically closed when they get deleted,
     # so the finally block is guaranteed to run.
     try:
-
         # ----- Load meta data
 
         # Wait for the log catcher to get the meta information
         etime = time.time() + 10.0
         while log_catcher.is_alive() and not log_catcher.header and time.time() < etime:
             time.sleep(0.01)
 
@@ -299,29 +299,29 @@
             raise IOError("{} not found! Wrong path?".format(path))
 
         meta = parse_ffmpeg_header(log_catcher.header)
         yield meta
 
         # ----- Read frames
 
-        w, h = meta["size"]
-        framesize_bits = w * h * bits_per_pixel
+        width, height = meta["size"]
+        framesize_bits = width * height * bits_per_pixel
         framesize_bytes = framesize_bits / 8
         assert (
             framesize_bytes.is_integer()
         ), "incorrect bits_per_pixel, framesize in bytes must be an int"
         framesize_bytes = int(framesize_bytes)
         framenr = 0
 
         while True:
             framenr += 1
             try:
                 bb = bytes()
                 while len(bb) < framesize_bytes:
-                    extra_bytes = p.stdout.read(framesize_bytes - len(bb))
+                    extra_bytes = process.stdout.read(framesize_bytes - len(bb))
                     if not extra_bytes:
                         if len(bb) == 0:
                             return
                         else:
                             raise RuntimeError(
                                 "End of file reached before full frame could be read."
                             )
@@ -347,49 +347,48 @@
         raise
 
     finally:
         # Stop the LogCatcher thread, which reads from stderr.
         log_catcher.stop_me()
 
         # Make sure that ffmpeg is terminated.
-        if p.poll() is None:
-
+        if process.poll() is None:
             # Ask ffmpeg to quit
             try:
                 # I read somewhere that modern ffmpeg on Linux prefers a
                 # "ctrl-c", but tests so far suggests sending q is more robust.
                 # > p.send_signal(signal.SIGINT)
                 # Sending q via communicate works, but can hang (see #17)
                 # > p.communicate(b"q")
                 # So let's do similar to what communicate does, but without
                 # reading stdout (which may block). It looks like only closing
                 # stdout is enough (tried Windows+Linux), but let's play safe.
                 # Found that writing to stdin can cause "Invalid argument" on
                 # Windows # and "Broken Pipe" on Unix.
                 # p.stdin.write(b"q")  # commented out in v0.4.1
-                p.stdout.close()
-                p.stdin.close()
+                process.stdout.close()
+                process.stdin.close()
                 # p.stderr.close() -> not here, the log_catcher closes it
             except Exception as err:  # pragma: no cover
                 logger.warning("Error while attempting stop ffmpeg (r): " + str(err))
 
             if stop_policy == "timeout":
                 # Wait until timeout, produce a warning and kill if it still exists
                 try:
                     etime = time.time() + 1.5
-                    while time.time() < etime and p.poll() is None:
+                    while time.time() < etime and process.poll() is None:
                         time.sleep(0.01)
                 finally:
-                    if p.poll() is None:  # pragma: no cover
+                    if process.poll() is None:  # pragma: no cover
                         logger.warning("We had to kill ffmpeg to stop it.")
-                        p.kill()
+                        process.kill()
 
             else:  # stop_policy == "kill"
                 # Just kill it
-                p.kill()
+                process.kill()
 
 
 def write_frames(
     path,
     size,
     pix_fmt_in="rgb24",
     pix_fmt_out="yuv420p",
@@ -606,20 +605,18 @@
     # ----- Write frames
 
     # Enter try block directly after opening the process.
     # We terminate ffmpeg in the finally clause.
     # Generators are automatically closed when they get deleted,
     # so the finally block is guaranteed to run.
     try:
-
         # Just keep going until the generator.close() is called (raises GeneratorExit).
         # This could also happen when the generator is deleted somehow.
         nframes = 0
         while True:
-
             # Get frame
             bb = yield
 
             # framesize = size[0] * size[1] * depth * bpp
             # assert isinstance(bb, bytes), "Frame must be send as bytes"
             # assert len(bb) == framesize, "Frame must have width*height*depth*bpp bytes"
             # Actually, we accept anything that can be written to file.
@@ -650,18 +647,16 @@
 
     except BaseException:
         # Detect KeyboardInterrupt / SystemExit: don't wait for ffmpeg to quit
         stop_policy = "kill"
         raise
 
     finally:
-
         # Make sure that ffmpeg is terminated.
         if p.poll() is None:
-
             # Tell ffmpeg that we're done
             try:
                 p.stdin.close()
             except Exception as err:  # pragma: no cover
                 logger.warning("Error while attempting stop ffmpeg (w): " + str(err))
 
             if stop_policy == "timeout":
```

### Comparing `imageio-ffmpeg-0.4.8/imageio_ffmpeg/_parsing.py` & `imageio-ffmpeg-0.4.9/imageio_ffmpeg/_parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
-import time
 import threading
+import time
 
 from ._utils import logger
 
 
 class LogCatcher(threading.Thread):
     """Thread to keep reading from stderr so that the buffer does not
     fill up and stalls the ffmpeg process. On stderr a message is send
@@ -45,15 +45,14 @@
             while self.is_alive() and time.time() < etime:  # pragma: no cover
                 time.sleep(0.01)
         # Return str
         lines = b"\n".join(self._lines)
         return self._header + "\n" + lines.decode("utf-8", "ignore")
 
     def run(self):
-
         # Create ref here so it still exists even if Py is shutting down
         limit_lines_local = limit_lines
 
         while not self._should_stop:
             time.sleep(0)
             # Read one line. Detect when closed, and exit
             try:
@@ -158,17 +157,16 @@
         )
 
     # get the frame rate.
     # matches can be empty, see #171, assume nframes = inf
     # the regexp omits values of "1k tbr" which seems a specific edge-case #262
     # it seems that tbr is generally to be preferred #262
     fps = 0
-    for line in (videolines[0], videolines[-1]):
-        matches = re.findall(r" ([0-9]+\.?[0-9]*) (tbr|fps)", line)
-        matches.sort(key=lambda x: x[1] == "tbr", reverse=True)
+    for line in [videolines[0]]:
+        matches = re.findall(r" ([0-9]+\.?[0-9]*) (fps)", line)
         if matches:
             fps = float(matches[0][0].strip())
     meta["fps"] = fps
 
     # get the size of the original stream, of the form 460x320 (w x h)
     line = videolines[0]
     match = re.search(" [0-9]*x[0-9]*(,| )", line)
```

### Comparing `imageio-ffmpeg-0.4.8/imageio_ffmpeg/_utils.py` & `imageio-ffmpeg-0.4.9/imageio_ffmpeg/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-import os
-import sys
 import logging
+import os
 import subprocess
+import sys
 from functools import lru_cache
+
 from pkg_resources import resource_filename
 
-from ._definitions import get_platform, FNAME_PER_PLATFORM
+from ._definitions import FNAME_PER_PLATFORM, get_platform
 
 logger = logging.getLogger("imageio_ffmpeg")
 
 
 def get_ffmpeg_exe():
     """
     Get the ffmpeg executable file. This can be the binary defined by
```

### Comparing `imageio-ffmpeg-0.4.8/imageio_ffmpeg.egg-info/PKG-INFO` & `imageio-ffmpeg-0.4.9/imageio_ffmpeg.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imageio-ffmpeg
-Version: 0.4.8
+Version: 0.4.9
 Summary: FFMPEG wrapper for Python
 Home-page: https://github.com/imageio/imageio-ffmpeg
 Download-URL: http://pypi.python.org/pypi/imageio-ffmpeg
 Author: imageio contributors
 Author-email: almar.klein@gmail.com
 License: BSD-2-Clause
 Keywords: video ffmpeg
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides: imageio_ffmpeg
 Requires-Python: >=3.5
 License-File: LICENSE
 
 FFMPEG wrapper for Python.
 
 Note that the platform-specific wheels contain the binary executable
```

### Comparing `imageio-ffmpeg-0.4.8/setup.py` & `imageio-ffmpeg-0.4.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,16 +53,16 @@
     download_url="http://pypi.python.org/pypi/imageio-ffmpeg",
     keywords="video ffmpeg",
     description="FFMPEG wrapper for Python",
     long_description=long_description,
     platforms="any",
     provides=["imageio_ffmpeg"],
     python_requires=">=3.5",
-    setup_requires=["pip>19"],
-    install_requires=[],
+    setup_requires=[],
+    install_requires=["setuptools"],
     packages=["imageio_ffmpeg"],
     package_dir={"imageio_ffmpeg": "imageio_ffmpeg"},
     package_data={"imageio_ffmpeg": ["binaries/*.*"]},
     include_package_data=True,
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
@@ -77,9 +77,10 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

