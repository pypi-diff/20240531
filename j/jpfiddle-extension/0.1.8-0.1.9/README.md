# Comparing `tmp/jpfiddle_extension-0.1.8.tar.gz` & `tmp/jpfiddle_extension-0.1.9.tar.gz`

## Comparing `jpfiddle_extension-0.1.8.tar` & `jpfiddle_extension-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.8/.copier-answers.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.8/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.8/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.8/CHANGELOG.md
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.8/RELEASE.md
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.8/install.json
--rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.8/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.8/setup.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.8/tsconfig.json
--rw-r--r--   0        0        0   199866 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.8/yarn.lock
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.8/jpfiddle_extension/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.8/jpfiddle_extension/_version.py
--rw-r--r--   0        0        0     5601 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.8/jpfiddle_extension/labextension/package.json
--rw-r--r--   0        0        0     5684 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.8/jpfiddle_extension/labextension/static/509.9c3efff5d95b2c2d6a12.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.8/jpfiddle_extension/labextension/static/728.151b68248be6f9ed2608.js
--rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.8/jpfiddle_extension/labextension/static/remoteEntry.6cce3e9dd2f0f36f5708.js
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.8/jpfiddle_extension/labextension/static/style.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.8/jpfiddle_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0    11580 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.8/src/index.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.8/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.8/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.8/style/index.js
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.8/.gitignore
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.8/LICENSE
--rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.8/README.md
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     5317 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.9/.copier-answers.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.9/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.9/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.9/CHANGELOG.md
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.9/RELEASE.md
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.9/install.json
+-rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.9/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.9/setup.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.9/tsconfig.json
+-rw-r--r--   0        0        0   199866 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.9/yarn.lock
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.9/jpfiddle_extension/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.9/jpfiddle_extension/_version.py
+-rw-r--r--   0        0        0     5601 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.9/jpfiddle_extension/labextension/package.json
+-rw-r--r--   0        0        0     5717 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.9/jpfiddle_extension/labextension/static/509.01c7f1d7159590f5d686.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.9/jpfiddle_extension/labextension/static/728.151b68248be6f9ed2608.js
+-rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.9/jpfiddle_extension/labextension/static/remoteEntry.b1a9892eb9774e74f369.js
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.9/jpfiddle_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.9/jpfiddle_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    11916 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.9/src/index.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.9/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.9/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.9/style/index.js
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.9/README.md
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     5317 2020-02-02 00:00:00.000000 jpfiddle_extension-0.1.9/PKG-INFO
```

### Comparing `jpfiddle_extension-0.1.8/RELEASE.md` & `jpfiddle_extension-0.1.9/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.8/package.json` & `jpfiddle_extension-0.1.9/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.1.9'"}*

```diff
@@ -179,9 +179,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.8"
+    "version": "0.1.9"
 }
```

### Comparing `jpfiddle_extension-0.1.8/tsconfig.json` & `jpfiddle_extension-0.1.9/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.8/yarn.lock` & `jpfiddle_extension-0.1.9/yarn.lock`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.8/jpfiddle_extension/__init__.py` & `jpfiddle_extension-0.1.9/jpfiddle_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.8/jpfiddle_extension/labextension/package.json` & `jpfiddle_extension-0.1.9/jpfiddle_extension/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9785879629629629%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.b1a9892eb9774e74f369.js'}}",*

 * * "'version'": "'0.1.9'"}*

```diff
@@ -99,15 +99,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "src/**/*.{ts,tsx}"
     ],
     "homepage": "https://github.com/magland/jpfiddle_extension",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.6cce3e9dd2f0f36f5708.js",
+            "load": "static/remoteEntry.b1a9892eb9774e74f369.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jpfiddle_extension/labextension"
     },
     "keywords": [
         "jupyter",
@@ -184,9 +184,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.8"
+    "version": "0.1.9"
 }
```

### Comparing `jpfiddle_extension-0.1.8/jpfiddle_extension/labextension/static/509.9c3efff5d95b2c2d6a12.js` & `jpfiddle_extension-0.1.9/jpfiddle_extension/labextension/static/509.01c7f1d7159590f5d686.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -19,19 +19,19 @@
                                         if ("save" === o.type && o.newValue) {
                                             if ("directory" === o.newValue.type) return;
                                             const n = o.newValue.path;
                                             if (!n) return void console.warn("No file path found in fileChanged event");
                                             if ("" !== t && !n.startsWith(t + "/")) return void console.warn("File path does not start with fiddleId:", n, t);
                                             const i = "" !== t ? n.slice(t.length + 1) : n;
                                             console.log("File saved:", i, o);
-                                            const a = await e.serviceManager.contents.get(n);
-                                            window.parent.postMessage({
+                                            let a = o.newValue.content;
+                                            null === a && (a = (await e.serviceManager.contents.get(n)).content), window.parent.postMessage({
                                                 type: "file-saved",
                                                 path: i,
-                                                content: a.content
+                                                content: a
                                             }, "*")
                                         } else if ("delete" === o.type && o.oldValue) {
                                         const e = o.oldValue.path;
                                         if (!e) return void console.warn("No file path found in fileChanged event");
                                         if ("" !== t && !e.startsWith(t + "/")) return void console.warn("File path does not start with fiddleId:", e, t);
                                         const n = "" !== t ? e.slice(t.length + 1) : e;
                                         console.log("File deleted:", n, o), window.parent.postMessage({
```

### Comparing `jpfiddle_extension-0.1.8/jpfiddle_extension/labextension/static/728.151b68248be6f9ed2608.js` & `jpfiddle_extension-0.1.9/jpfiddle_extension/labextension/static/728.151b68248be6f9ed2608.js`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.8/jpfiddle_extension/labextension/static/remoteEntry.6cce3e9dd2f0f36f5708.js` & `jpfiddle_extension-0.1.9/jpfiddle_extension/labextension/static/remoteEntry.b1a9892eb9774e74f369.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -43,18 +43,18 @@
         }), r
     }, o.d = (e, r) => {
         for (var t in r) o.o(r, t) && !o.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, o.f = {}, o.e = e => Promise.all(Object.keys(o.f).reduce(((r, t) => (o.f[t](e, r), r)), [])), o.u = e => e + "." + {
-        509: "9c3efff5d95b2c2d6a12",
+        509: "01c7f1d7159590f5d686",
         728: "151b68248be6f9ed2608"
     } [e] + ".js?v=" + {
-        509: "9c3efff5d95b2c2d6a12",
+        509: "01c7f1d7159590f5d686",
         728: "151b68248be6f9ed2608"
     } [e], o.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -106,15 +106,15 @@
                     var i = a[e] = a[e] || {},
                         l = i[r];
                     (!l || !l.loaded && (1 != !l.eager ? n : d > l.from)) && (i[r] = {
                         get: () => o.e(509).then((() => () => o(509))),
                         from: d,
                         eager: !1
                     })
-                })("jpfiddle_extension", "0.1.8"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                })("jpfiddle_extension", "0.1.9"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         o.g.importScripts && (e = o.g.location + "");
         var r = o.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jpfiddle_extension-0.1.8/jpfiddle_extension/labextension/static/third-party-licenses.json` & `jpfiddle_extension-0.1.9/jpfiddle_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.8/src/index.ts` & `jpfiddle_extension-0.1.9/src/index.ts`

 * *Files 2% similar despite different names*

```diff
@@ -55,20 +55,27 @@
           fiddleId
         );
         return;
       }
       const path =
         fiddleId !== '' ? fullPath.slice(fiddleId.length + 1) : fullPath;
       console.log('File saved:', path, change);
-      const vv = await app.serviceManager.contents.get(fullPath);
+      // This is tricky. Depending on the storage mechanism (memory or indexdb)
+      // the content may exist either in change.newValue.content or it needs to be
+      // fetched asynchronously using app.serviceManager.contents.get
+      let content = change.newValue.content;
+      if (content === null) {
+        const vv = await app.serviceManager.contents.get(fullPath);
+        content = vv.content;
+      }
       window.parent.postMessage(
         {
           type: 'file-saved',
           path,
-          content: vv.content
+          content
         },
         '*'
       );
     } else if (change.type === 'delete' && change.oldValue) {
       const fullPath = change.oldValue.path;
       if (!fullPath) {
         console.warn('No file path found in fileChanged event');
```

### Comparing `jpfiddle_extension-0.1.8/.gitignore` & `jpfiddle_extension-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.8/LICENSE` & `jpfiddle_extension-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.8/README.md` & `jpfiddle_extension-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.8/pyproject.toml` & `jpfiddle_extension-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jpfiddle_extension-0.1.8/PKG-INFO` & `jpfiddle_extension-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jpfiddle_extension
-Version: 0.1.8
+Version: 0.1.9
 Dynamic: Keywords
 Summary: A JupyterLab extension for jpfiddle.
 Project-URL: Homepage, https://github.com/magland/jpfiddle_extension
 Project-URL: Bug Tracker, https://github.com/magland/jpfiddle_extension/issues
 Project-URL: Repository, https://github.com/magland/jpfiddle_extension.git
 Author-email: Jeremy Magland <jmagland@flatironinstitute.org>
 License: BSD 3-Clause License
```

