# Comparing `tmp/cumo-0.33.5.tar.gz` & `tmp/cumo-0.33.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cumo-0.33.5.tar", max compression
+gzip compressed data, was "cumo-0.33.6.tar", max compression
```

## Comparing `cumo-0.33.5.tar` & `cumo-0.33.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1275 2024-04-30 05:18:38.310001 cumo-0.33.5/README.md
--rw-r--r--   0        0        0        7 2024-04-18 06:06:53.389837 cumo-0.33.5/cumo/.gitignore
--rw-r--r--   0        0        0      117 2024-04-18 06:06:53.389837 cumo-0.33.5/cumo/__init__.py
--rw-r--r--   0        0        0     3683 2024-04-18 06:06:53.389837 cumo-0.33.5/cumo/__main__.py
--rw-r--r--   0        0        0        9 2024-04-18 06:06:53.389837 cumo-0.33.5/cumo/_internal/.gitignore
--rw-r--r--   0        0        0        0 2024-04-18 06:06:53.389837 cumo-0.33.5/cumo/_internal/__init__.py
--rw-r--r--   0        0        0     1675 2024-04-18 06:06:53.389837 cumo-0.33.5/cumo/_internal/down_sample.py
--rw-r--r--   0        0        0        0 2024-04-18 06:06:53.389837 cumo-0.33.5/cumo/_internal/members/__init__.py
--rw-r--r--   0        0        0     8722 2024-04-18 06:06:53.389837 cumo-0.33.5/cumo/_internal/members/camera.py
--rw-r--r--   0        0        0     1177 2024-04-18 06:06:53.389837 cumo-0.33.5/cumo/_internal/members/capture_screen.py
--rw-r--r--   0        0        0    12413 2024-04-18 06:06:53.389837 cumo-0.33.5/cumo/_internal/members/custom_control.py
--rw-r--r--   0        0        0     5927 2024-04-18 06:06:53.389837 cumo-0.33.5/cumo/_internal/members/event_handler.py
--rw-r--r--   0        0        0      974 2024-04-18 06:06:53.389837 cumo-0.33.5/cumo/_internal/members/internal_utils.py
--rw-r--r--   0        0        0     6396 2024-04-18 06:06:53.389837 cumo-0.33.5/cumo/_internal/members/keyboard_event_handler.py
--rw-r--r--   0        0        0     1360 2024-04-18 06:06:53.389837 cumo-0.33.5/cumo/_internal/members/remove_object.py
--rw-r--r--   0        0        0    20526 2024-04-18 06:06:53.389837 cumo-0.33.5/cumo/_internal/members/send_object.py
--rw-r--r--   0        0        0    10336 2024-04-18 06:06:53.389837 cumo-0.33.5/cumo/_internal/members/set_custom_control.py
--rw-r--r--   0        0        0     1045 2024-04-18 06:06:53.389837 cumo-0.33.5/cumo/_internal/members/set_enable.py
--rw-r--r--   0        0        0     1256 2024-04-18 06:06:53.389837 cumo-0.33.5/cumo/_internal/members/utils.py
--rw-r--r--   0        0        0        0 2024-04-30 05:18:30.582007 cumo-0.33.5/cumo/_internal/protobuf/__init__.py
--rw-r--r--   0        0        0     3923 2024-04-30 05:18:30.578007 cumo-0.33.5/cumo/_internal/protobuf/client_pb2.py
--rw-r--r--   0        0        0    10387 2024-04-30 05:18:30.578007 cumo-0.33.5/cumo/_internal/protobuf/client_pb2.pyi
--rw-r--r--   0        0        0    12303 2024-04-30 05:18:30.402007 cumo-0.33.5/cumo/_internal/protobuf/server_pb2.py
--rw-r--r--   0        0        0    40121 2024-04-30 05:18:30.402007 cumo-0.33.5/cumo/_internal/protobuf/server_pb2.pyi
--rw-r--r--   0        0        0     4200 2024-04-18 06:06:53.393837 cumo-0.33.5/cumo/_internal/server.py
--rw-r--r--   0        0        0     1509 2024-04-18 06:06:53.393837 cumo-0.33.5/cumo/_vendor/pypcd/LICENSE
--rw-r--r--   0        0        0    28920 2024-04-18 06:06:53.393837 cumo-0.33.5/cumo/_vendor/pypcd/pypcd.py
--rw-r--r--   0        0        0     1119 2024-04-18 06:06:53.393837 cumo-0.33.5/cumo/camera_state.py
--rw-r--r--   0        0        0      924 2024-04-18 06:06:53.393837 cumo-0.33.5/cumo/keyboard_event.py
--rw-r--r--   0        0        0     3554 2024-04-18 06:06:53.393837 cumo-0.33.5/cumo/pointcloudviewer.py
--rw-r--r--   0        0        0  5077405 2024-04-30 05:18:38.310001 cumo-0.33.5/cumo/public/bundle-e4641802.js
--rw-r--r--   0        0        0   243028 2024-04-30 05:18:38.310001 cumo-0.33.5/cumo/public/bundle.js.LICENSE.txt
--rw-r--r--   0        0        0      515 2024-04-30 05:18:38.310001 cumo-0.33.5/cumo/public/index-31f52342.css
--rw-r--r--   0        0        0      281 2024-04-30 05:18:38.310001 cumo-0.33.5/cumo/public/index.html
--rw-r--r--   0        0        0     1219 2024-04-30 05:16:20.678248 cumo-0.33.5/pyproject.toml
--rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 cumo-0.33.5/PKG-INFO
+-rw-r--r--   0        0        0     3201 2024-05-31 04:53:07.228729 cumo-0.33.6/README.md
+-rw-r--r--   0        0        0        7 2024-04-18 06:06:53.389837 cumo-0.33.6/cumo/.gitignore
+-rw-r--r--   0        0        0      117 2024-04-18 06:06:53.389837 cumo-0.33.6/cumo/__init__.py
+-rw-r--r--   0        0        0     3683 2024-05-31 04:51:45.625120 cumo-0.33.6/cumo/__main__.py
+-rw-r--r--   0        0        0        9 2024-04-18 06:06:53.389837 cumo-0.33.6/cumo/_internal/.gitignore
+-rw-r--r--   0        0        0        0 2024-04-18 06:06:53.389837 cumo-0.33.6/cumo/_internal/__init__.py
+-rw-r--r--   0        0        0     1675 2024-04-18 06:06:53.389837 cumo-0.33.6/cumo/_internal/down_sample.py
+-rw-r--r--   0        0        0        0 2024-04-18 06:06:53.389837 cumo-0.33.6/cumo/_internal/members/__init__.py
+-rw-r--r--   0        0        0     8722 2024-04-18 06:06:53.389837 cumo-0.33.6/cumo/_internal/members/camera.py
+-rw-r--r--   0        0        0     1177 2024-04-18 06:06:53.389837 cumo-0.33.6/cumo/_internal/members/capture_screen.py
+-rw-r--r--   0        0        0    12413 2024-04-18 06:06:53.389837 cumo-0.33.6/cumo/_internal/members/custom_control.py
+-rw-r--r--   0        0        0     5927 2024-04-18 06:06:53.389837 cumo-0.33.6/cumo/_internal/members/event_handler.py
+-rw-r--r--   0        0        0      974 2024-04-18 06:06:53.389837 cumo-0.33.6/cumo/_internal/members/internal_utils.py
+-rw-r--r--   0        0        0     6396 2024-04-18 06:06:53.389837 cumo-0.33.6/cumo/_internal/members/keyboard_event_handler.py
+-rw-r--r--   0        0        0     1360 2024-04-18 06:06:53.389837 cumo-0.33.6/cumo/_internal/members/remove_object.py
+-rw-r--r--   0        0        0    20526 2024-04-18 06:06:53.389837 cumo-0.33.6/cumo/_internal/members/send_object.py
+-rw-r--r--   0        0        0    10336 2024-04-18 06:06:53.389837 cumo-0.33.6/cumo/_internal/members/set_custom_control.py
+-rw-r--r--   0        0        0     1045 2024-04-18 06:06:53.389837 cumo-0.33.6/cumo/_internal/members/set_enable.py
+-rw-r--r--   0        0        0     1256 2024-04-18 06:06:53.389837 cumo-0.33.6/cumo/_internal/members/utils.py
+-rw-r--r--   0        0        0        0 2024-05-31 04:52:48.860817 cumo-0.33.6/cumo/_internal/protobuf/__init__.py
+-rw-r--r--   0        0        0     3923 2024-05-31 04:52:48.856817 cumo-0.33.6/cumo/_internal/protobuf/client_pb2.py
+-rw-r--r--   0        0        0    10387 2024-05-31 04:52:48.856817 cumo-0.33.6/cumo/_internal/protobuf/client_pb2.pyi
+-rw-r--r--   0        0        0    12303 2024-05-31 04:52:48.440819 cumo-0.33.6/cumo/_internal/protobuf/server_pb2.py
+-rw-r--r--   0        0        0    40121 2024-05-31 04:52:48.440819 cumo-0.33.6/cumo/_internal/protobuf/server_pb2.pyi
+-rw-r--r--   0        0        0     4200 2024-04-18 06:06:53.393837 cumo-0.33.6/cumo/_internal/server.py
+-rw-r--r--   0        0        0     1509 2024-04-18 06:06:53.393837 cumo-0.33.6/cumo/_vendor/pypcd/LICENSE
+-rw-r--r--   0        0        0    28920 2024-04-18 06:06:53.393837 cumo-0.33.6/cumo/_vendor/pypcd/pypcd.py
+-rw-r--r--   0        0        0     1119 2024-04-18 06:06:53.393837 cumo-0.33.6/cumo/camera_state.py
+-rw-r--r--   0        0        0      924 2024-04-18 06:06:53.393837 cumo-0.33.6/cumo/keyboard_event.py
+-rw-r--r--   0        0        0     3554 2024-04-18 06:06:53.393837 cumo-0.33.6/cumo/pointcloudviewer.py
+-rw-r--r--   0        0        0  5077907 2024-05-31 04:53:07.228729 cumo-0.33.6/cumo/public/bundle-49f3a59c.js
+-rw-r--r--   0        0        0   243028 2024-05-31 04:53:07.228729 cumo-0.33.6/cumo/public/bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0      515 2024-05-31 04:53:07.224729 cumo-0.33.6/cumo/public/index-31f52342.css
+-rw-r--r--   0        0        0      281 2024-05-31 04:53:07.224729 cumo-0.33.6/cumo/public/index.html
+-rw-r--r--   0        0        0     1219 2024-05-31 04:52:43.416843 cumo-0.33.6/pyproject.toml
+-rw-r--r--   0        0        0     4528 1970-01-01 00:00:00.000000 cumo-0.33.6/PKG-INFO
```

### Comparing `cumo-0.33.5/cumo/__main__.py` & `cumo-0.33.6/cumo/__main__.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.5/cumo/_internal/down_sample.py` & `cumo-0.33.6/cumo/_internal/down_sample.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.5/cumo/_internal/members/camera.py` & `cumo-0.33.6/cumo/_internal/members/camera.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.5/cumo/_internal/members/capture_screen.py` & `cumo-0.33.6/cumo/_internal/members/capture_screen.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.5/cumo/_internal/members/custom_control.py` & `cumo-0.33.6/cumo/_internal/members/custom_control.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.5/cumo/_internal/members/event_handler.py` & `cumo-0.33.6/cumo/_internal/members/event_handler.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.5/cumo/_internal/members/internal_utils.py` & `cumo-0.33.6/cumo/_internal/members/internal_utils.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.5/cumo/_internal/members/keyboard_event_handler.py` & `cumo-0.33.6/cumo/_internal/members/keyboard_event_handler.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.5/cumo/_internal/members/remove_object.py` & `cumo-0.33.6/cumo/_internal/members/remove_object.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.5/cumo/_internal/members/send_object.py` & `cumo-0.33.6/cumo/_internal/members/send_object.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.5/cumo/_internal/members/set_custom_control.py` & `cumo-0.33.6/cumo/_internal/members/set_custom_control.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.5/cumo/_internal/members/set_enable.py` & `cumo-0.33.6/cumo/_internal/members/set_enable.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.5/cumo/_internal/members/utils.py` & `cumo-0.33.6/cumo/_internal/members/utils.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.5/cumo/_internal/protobuf/client_pb2.py` & `cumo-0.33.6/cumo/_internal/protobuf/client_pb2.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.5/cumo/_internal/protobuf/client_pb2.pyi` & `cumo-0.33.6/cumo/_internal/protobuf/client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cumo-0.33.5/cumo/_internal/protobuf/server_pb2.py` & `cumo-0.33.6/cumo/_internal/protobuf/server_pb2.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.5/cumo/_internal/protobuf/server_pb2.pyi` & `cumo-0.33.6/cumo/_internal/protobuf/server_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cumo-0.33.5/cumo/_internal/server.py` & `cumo-0.33.6/cumo/_internal/server.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.5/cumo/_vendor/pypcd/LICENSE` & `cumo-0.33.6/cumo/_vendor/pypcd/LICENSE`

 * *Files identical despite different names*

### Comparing `cumo-0.33.5/cumo/_vendor/pypcd/pypcd.py` & `cumo-0.33.6/cumo/_vendor/pypcd/pypcd.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.5/cumo/camera_state.py` & `cumo-0.33.6/cumo/camera_state.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.5/cumo/keyboard_event.py` & `cumo-0.33.6/cumo/keyboard_event.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.5/cumo/pointcloudviewer.py` & `cumo-0.33.6/cumo/pointcloudviewer.py`

 * *Files identical despite different names*

### Comparing `cumo-0.33.5/cumo/public/bundle-e4641802.js` & `cumo-0.33.6/cumo/public/bundle-49f3a59c.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -123650,29 +123650,50 @@
         var t;
         this.canvas !== null && (this.canvas.removeEventListener("contextmenu", this.onContextMenu), this.canvas.removeEventListener("pointerdown", this.onPointerDown), this.canvas.removeEventListener("wheel", this.onMouseWheel), this.canvas.ownerDocument.removeEventListener("pointermove", this.onPointerMove), this.canvas.ownerDocument.removeEventListener("pointerup", this.onPointerUp), window.removeEventListener("keydown", this.onKeyDown), window.removeEventListener("keyup", this.onKeyUp), window.removeEventListener("resize", this.onResize), (t = this.canvasObserver) == null || t.disconnect())
     }
     checkInputs() {
         this.update()
     }
     rotateCamera() {
-        if (this.camera === null) return;
-        const t = new Vector3(this.moveCurr.x - this.movePrev.x, this.moveCurr.y - this.movePrev.y, 0);
-        let r = t.length();
-        if (r) {
-            this.target.subtractToRef(this.camera.position, this.eye);
-            const s = this.eye.clone();
-            s.normalize();
-            const n = this.camera.upVector.clone();
-            n.normalize();
-            const o = n.cross(s);
-            o.normalize(), n.scaleInPlace(this.moveCurr.y - this.movePrev.y), o.scaleInPlace(this.moveCurr.x - this.movePrev.x), n.addToRef(o, t);
-            const c = t.cross(s).normalize();
-            r *= this.rotateSpeed;
-            const h = Quaternion.RotationAxis(c, r).normalize();
-            this.eye.applyRotationQuaternionInPlace(h), this.noRoll || (this.camera.upVector = this.camera.upVector.normalizeToNew().applyRotationQuaternion(h).normalizeToNew()), this.movePrev.copyFrom(this.moveCurr)
+        if (this.camera !== null) {
+            if (this.noRoll) {
+                this.target.subtractToRef(this.camera.position, this.eye);
+                const t = this.eye.clone();
+                let r = -(this.moveCurr.x - this.movePrev.x);
+                if (r) {
+                    const n = this.camera.upVector.clone();
+                    n.normalize(), r *= this.rotateSpeed;
+                    const o = Quaternion.RotationAxis(n, r).normalize();
+                    this.eye.applyRotationQuaternionInPlace(o)
+                }
+                let s = this.moveCurr.y - this.movePrev.y;
+                if (s) {
+                    const n = this.camera.upVector.cross(t);
+                    n.normalize(), s *= this.rotateSpeed;
+                    const o = Quaternion.RotationAxis(n, s).normalize();
+                    this.eye.applyRotationQuaternionInPlace(o)
+                }
+            } else {
+                const t = new Vector3(this.moveCurr.x - this.movePrev.x, this.moveCurr.y - this.movePrev.y, 0);
+                let r = t.length();
+                if (r) {
+                    this.target.subtractToRef(this.camera.position, this.eye);
+                    const s = this.eye.clone();
+                    s.normalize();
+                    const n = this.camera.upVector.clone();
+                    n.normalize();
+                    const o = n.cross(s);
+                    o.normalize(), n.scaleInPlace(this.moveCurr.y - this.movePrev.y), o.scaleInPlace(this.moveCurr.x - this.movePrev.x), n.addToRef(o, t);
+                    const c = t.cross(s).normalize();
+                    r *= this.rotateSpeed;
+                    const h = Quaternion.RotationAxis(c, r).normalize();
+                    this.eye.applyRotationQuaternionInPlace(h), this.camera.upVector = this.camera.upVector.normalizeToNew().applyRotationQuaternion(h).normalizeToNew()
+                }
+            }
+            this.movePrev.copyFrom(this.moveCurr)
         }
     }
     zoomCamera() {
         if (this.camera === null) return;
         const t = 1 + (this.zoomEnd.y - this.zoomStart.y) * this.zoomSpeed;
         if (t !== 1 && t > 0) {
             this.target.subtractToRef(this.camera.position, this.eye);
```

### Comparing `cumo-0.33.5/cumo/public/bundle.js.LICENSE.txt` & `cumo-0.33.6/cumo/public/bundle.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cumo-0.33.5/cumo/public/index-31f52342.css` & `cumo-0.33.6/cumo/public/index-31f52342.css`

 * *Files identical despite different names*

### Comparing `cumo-0.33.5/pyproject.toml` & `cumo-0.33.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 readme = "README.md"
 name = "cumo"
-version = "0.33.5"
+version = "0.33.6"
 description = "Webブラウザ上に点群を描画する python ライブラリ"
 authors = ["Kurusugawa Computer"]
 license = "BSD"
 keywords = ["point-cloud", "pcd"]
 repository = "https://github.com/kurusugawa-computer/cumo"
 classifiers = [
 	"Development Status :: 3 - Alpha",
```

