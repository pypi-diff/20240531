# Comparing `tmp/gradio_pdf-0.0.8.tar.gz` & `tmp/gradio_pdf-0.0.9.tar.gz`

## Comparing `gradio_pdf-0.0.8.tar` & `gradio_pdf-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 gradio_pdf-0.0.8/backend/gradio_pdf/__init__.py
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 gradio_pdf-0.0.8/backend/gradio_pdf/pdf.py
--rw-r--r--   0        0        0    12279 2020-02-02 00:00:00.000000 gradio_pdf-0.0.8/backend/gradio_pdf/pdf.pyi
--rw-r--r--   0        0        0   688959 2020-02-02 00:00:00.000000 gradio_pdf-0.0.8/backend/gradio_pdf/templates/component/Index-BYwJN1i6.js
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 gradio_pdf-0.0.8/backend/gradio_pdf/templates/component/index.js
--rw-r--r--   0        0        0    14825 2020-02-02 00:00:00.000000 gradio_pdf-0.0.8/backend/gradio_pdf/templates/component/style.css
--rw-r--r--   0        0        0    77959 2020-02-02 00:00:00.000000 gradio_pdf-0.0.8/backend/gradio_pdf/templates/component/wrapper-98f94c21-DqR3tIm1.js
--rw-r--r--   0        0        0   560970 2020-02-02 00:00:00.000000 gradio_pdf-0.0.8/backend/gradio_pdf/templates/example/index.js
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 gradio_pdf-0.0.8/backend/gradio_pdf/templates/example/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_pdf-0.0.8/demo/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 gradio_pdf-0.0.8/demo/_app.py
--rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 gradio_pdf-0.0.8/demo/app.py
--rw-r--r--   0        0        0   127928 2020-02-02 00:00:00.000000 gradio_pdf-0.0.8/demo/contract.pdf
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_pdf-0.0.8/demo/css.css
--rw-r--r--   0        0        0   372153 2020-02-02 00:00:00.000000 gradio_pdf-0.0.8/demo/invoice_2.pdf
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 gradio_pdf-0.0.8/demo/requirements.txt
--rw-r--r--   0        0        0    34705 2020-02-02 00:00:00.000000 gradio_pdf-0.0.8/demo/sample_invoice.pdf
--rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 gradio_pdf-0.0.8/demo/space.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 gradio_pdf-0.0.8/frontend/Example.svelte
--rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 gradio_pdf-0.0.8/frontend/Index.svelte
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 gradio_pdf-0.0.8/frontend/PdfUploadText.svelte
--rw-r--r--   0        0        0   174508 2020-02-02 00:00:00.000000 gradio_pdf-0.0.8/frontend/package-lock.json
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 gradio_pdf-0.0.8/frontend/package.json
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 gradio_pdf-0.0.8/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 gradio_pdf-0.0.8/LICENSE
--rw-r--r--   0        0        0    10505 2020-02-02 00:00:00.000000 gradio_pdf-0.0.8/README.md
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 gradio_pdf-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    11771 2020-02-02 00:00:00.000000 gradio_pdf-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 gradio_pdf-0.0.9/backend/gradio_pdf/__init__.py
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 gradio_pdf-0.0.9/backend/gradio_pdf/pdf.py
+-rw-r--r--   0        0        0    12279 2020-02-02 00:00:00.000000 gradio_pdf-0.0.9/backend/gradio_pdf/pdf.pyi
+-rw-r--r--   0        0        0   689115 2020-02-02 00:00:00.000000 gradio_pdf-0.0.9/backend/gradio_pdf/templates/component/Index--Ld6fSuw.js
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 gradio_pdf-0.0.9/backend/gradio_pdf/templates/component/index.js
+-rw-r--r--   0        0        0    14825 2020-02-02 00:00:00.000000 gradio_pdf-0.0.9/backend/gradio_pdf/templates/component/style.css
+-rw-r--r--   0        0        0    77959 2020-02-02 00:00:00.000000 gradio_pdf-0.0.9/backend/gradio_pdf/templates/component/wrapper-98f94c21-D4kvqJe-.js
+-rw-r--r--   0        0        0   560970 2020-02-02 00:00:00.000000 gradio_pdf-0.0.9/backend/gradio_pdf/templates/example/index.js
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 gradio_pdf-0.0.9/backend/gradio_pdf/templates/example/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_pdf-0.0.9/demo/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 gradio_pdf-0.0.9/demo/_app.py
+-rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 gradio_pdf-0.0.9/demo/app.py
+-rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 gradio_pdf-0.0.9/demo/app2.py
+-rw-r--r--   0        0        0   127928 2020-02-02 00:00:00.000000 gradio_pdf-0.0.9/demo/contract.pdf
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_pdf-0.0.9/demo/css.css
+-rw-r--r--   0        0        0   372153 2020-02-02 00:00:00.000000 gradio_pdf-0.0.9/demo/invoice_2.pdf
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 gradio_pdf-0.0.9/demo/requirements.txt
+-rw-r--r--   0        0        0    34705 2020-02-02 00:00:00.000000 gradio_pdf-0.0.9/demo/sample_invoice.pdf
+-rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 gradio_pdf-0.0.9/demo/space.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 gradio_pdf-0.0.9/frontend/Example.svelte
+-rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 gradio_pdf-0.0.9/frontend/Index.svelte
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 gradio_pdf-0.0.9/frontend/PdfUploadText.svelte
+-rw-r--r--   0        0        0   174508 2020-02-02 00:00:00.000000 gradio_pdf-0.0.9/frontend/package-lock.json
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 gradio_pdf-0.0.9/frontend/package.json
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 gradio_pdf-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 gradio_pdf-0.0.9/LICENSE
+-rw-r--r--   0        0        0    10505 2020-02-02 00:00:00.000000 gradio_pdf-0.0.9/README.md
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 gradio_pdf-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    11771 2020-02-02 00:00:00.000000 gradio_pdf-0.0.9/PKG-INFO
```

### Comparing `gradio_pdf-0.0.8/backend/gradio_pdf/pdf.py` & `gradio_pdf-0.0.9/backend/gradio_pdf/pdf.py`

 * *Files identical despite different names*

### Comparing `gradio_pdf-0.0.8/backend/gradio_pdf/pdf.pyi` & `gradio_pdf-0.0.9/backend/gradio_pdf/pdf.pyi`

 * *Files identical despite different names*

### Comparing `gradio_pdf-0.0.8/backend/gradio_pdf/templates/component/Index-BYwJN1i6.js` & `gradio_pdf-0.0.9/backend/gradio_pdf/templates/component/Index--Ld6fSuw.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -2923,15 +2923,15 @@
         absolute: E = !0
     } = t, {
         translucent: S = !1
     } = t, {
         border: g = !1
     } = t, {
         autoscroll: v
-    } = t, $, M = !1, _ = 0, N = 0, D = null, X = 0, Y = null, I, U = null, G = !0;
+    } = t, $, M = !1, _ = 0, N = 0, D = null, X = 0, Y = null, I, j = null, G = !0;
     const V = () => {
         n(25, _ = performance.now()), n(26, N = 0), M = !0, H();
     };
 
     function H() {
         requestAnimationFrame(() => {
             n(26, N = (performance.now() - _) / 1e3), M && H();
@@ -2944,15 +2944,15 @@
     onDestroy(() => {
         M && st();
     });
     let dt = null;
 
     function yt(k) {
         binding_callbacks$2[k ? "unshift" : "push"](() => {
-            U = k, n(16, U), n(7, m), n(14, Y), n(15, I);
+            j = k, n(16, j), n(7, m), n(14, Y), n(15, I);
         });
     }
 
     function gt(k) {
         binding_callbacks$2[k ? "unshift" : "push"](() => {
             $ = k, n(13, $);
         });
@@ -2965,15 +2965,15 @@
             67108865 && n(17, X = A === null || A <= 0 || !N ? null : Math.min(N / A, 1)), i.$$.dirty[0] & /*progress*/
             128 && m != null && n(18, G = !1), i.$$.dirty[0] & /*progress, progress_level, progress_bar, last_progress_level*/
             114816 && (m != null ? n(14, Y = m.map((k) => {
                 if (k.index != null && k.length != null)
                     return k.index / k.length;
                 if (k.progress != null)
                     return k.progress;
-            })) : n(14, Y = null), Y ? (n(15, I = Y[Y.length - 1]), U && (I === 0 ? n(16, U.style.transition = "0", U) : n(16, U.style.transition = "150ms", U))) : n(15, I = void 0)), i.$$.dirty[0] & /*status*/
+            })) : n(14, Y = null), Y ? (n(15, I = Y[Y.length - 1]), j && (I === 0 ? n(16, j.style.transition = "0", j) : n(16, j.style.transition = "150ms", j))) : n(15, I = void 0)), i.$$.dirty[0] & /*status*/
             16 && (F === "pending" ? V() : st()), i.$$.dirty[0] & /*el, scroll_to_output, status, autoscroll*/
             20979728 && $ && R && (F === "pending" || F === "complete") && scroll_into_view($, v), i.$$.dirty[0] & /*status, message*/
             8388624, i.$$.dirty[0] & /*timer_diff*/
             67108864 && n(20, e = N.toFixed(1));
     }, [
         A,
         f,
@@ -2987,15 +2987,15 @@
         x,
         E,
         S,
         g,
         $,
         Y,
         I,
-        U,
+        j,
         X,
         G,
         dt,
         e,
         a,
         R,
         P,
@@ -3292,15 +3292,15 @@
             } = A, R = {
                 predict: N,
                 submit: D,
                 view_api: Y,
                 component_server: X
             }, w = F ?? !0;
             if ((typeof window > "u" || !("WebSocket" in window)) && !global.Websocket) {
-                const I = await import("./wrapper-98f94c21-DqR3tIm1.js");
+                const I = await import("./wrapper-98f94c21-D4kvqJe-.js");
                 NodeBlob = (await Promise.resolve().then(() => __viteBrowserExternal)).Blob, global.WebSocket = I.WebSocket;
             }
             const {
                 ws_protocol: T,
                 http_protocol: P,
                 host: m,
                 space_id: C
@@ -3312,16 +3312,16 @@
                 if (S = I, g = map_names_to_ids((I == null ? void 0 : I.dependencies) || []), S.auth_required)
                     return {
                         config: S,
                         ...R
                     };
                 try {
                     M = await Y(S);
-                } catch (U) {
-                    console.error(`Could not get api details: ${U.message}`);
+                } catch (j) {
+                    console.error(`Could not get api details: ${j.message}`);
                 }
                 return {
                     config: S,
                     ...R
                 };
             }
             let M;
@@ -3329,18 +3329,18 @@
                 if (h && h(I), I.status === "running")
                     try {
                         S = await resolve_config(
                             i,
                             `${P}//${m}`,
                             o
                         );
-                        const U = await $(S);
-                        a(U);
-                    } catch (U) {
-                        console.error(U), h && h({
+                        const j = await $(S);
+                        a(j);
+                    } catch (j) {
+                        console.error(j), h && h({
                             status: "error",
                             message: "Could not load this space.",
                             load_status: "error",
                             detail: "NOT_FOUND"
                         });
                     }
             }
@@ -3361,40 +3361,40 @@
                     status: "error",
                     message: "Could not load this space.",
                     load_status: "error",
                     detail: "NOT_FOUND"
                 });
             }
 
-            function N(I, U, G) {
+            function N(I, j, G) {
                 let V = !1,
                     H = !1,
                     st;
                 if (typeof I == "number")
                     st = S.dependencies[I];
                 else {
                     const dt = I.replace(/^\//, "");
                     st = S.dependencies[g[dt]];
                 }
                 if (st.types.continuous)
                     throw new Error(
                         "Cannot call predict on this function as it may run forever. Use submit instead"
                     );
                 return new Promise((dt, yt) => {
-                    const gt = D(I, U, G);
+                    const gt = D(I, j, G);
                     let k;
                     gt.on("data", (l) => {
                         H && (gt.destroy(), dt(l)), V = !0, k = l;
                     }).on("status", (l) => {
                         l.stage === "error" && yt(l), l.stage === "complete" && (H = !0, V && (gt.destroy(), dt(k)));
                     });
                 });
             }
 
-            function D(I, U, G) {
+            function D(I, j, G) {
                 let V, H;
                 if (typeof I == "number")
                     V = I, H = M.unnamed_endpoints[V];
                 else {
                     const Z = I.replace(/^\//, "");
                     V = g[Z], H = M.named_endpoints[I.trim()];
                 }
@@ -3406,15 +3406,15 @@
                 const gt = typeof I == "number" ? "/predict" : I;
                 let k, l = null,
                     u = !1;
                 const d = {};
                 let b = "";
                 typeof window < "u" && (b = new URLSearchParams(window.location.search).toString()), p(
                     `${P}//${resolve_root(m, S.path, !0)}`,
-                    U,
+                    j,
                     H,
                     o
                 ).then((Z) => {
                     if (k = {
                             data: Z || [],
                             event_data: G,
                             fn_index: V
@@ -3746,15 +3746,15 @@
                 return {
                     on: O,
                     off: B,
                     cancel: z,
                     destroy: it
                 };
             }
-            async function X(I, U, G) {
+            async function X(I, j, G) {
                 var V;
                 const H = {
                     "Content-Type": "application/json"
                 };
                 o && (H.Authorization = `Bearer ${o}`);
                 let st, dt = S.components.find(
                     (k) => k.id === I
@@ -3766,45 +3766,45 @@
         )}/`;
                 const yt = await i(
                     `${st}component_server/`, {
                         method: "POST",
                         body: JSON.stringify({
                             data: G,
                             component_id: I,
-                            fn_name: U,
+                            fn_name: j,
                             session_hash: x
                         }),
                         headers: H
                     }
                 );
                 if (!yt.ok)
                     throw new Error(
                         "Could not connect to component server: " + yt.statusText
                     );
                 return await yt.json();
             }
             async function Y(I) {
                 if (M)
                     return M;
-                const U = {
+                const j = {
                     "Content-Type": "application/json"
                 };
-                o && (U.Authorization = `Bearer ${o}`);
+                o && (j.Authorization = `Bearer ${o}`);
                 let G;
                 if (semiver(I.version || "2.0.0", "3.30") < 0 ? G = await i(
                         "https://gradio-space-api-fetcher-v2.hf.space/api", {
                             method: "POST",
                             body: JSON.stringify({
                                 serialize: !1,
                                 config: JSON.stringify(I)
                             }),
-                            headers: U
+                            headers: j
                         }
                     ) : G = await i(`${I.root}/info`, {
-                        headers: U
+                        headers: j
                     }), !G.ok)
                     throw new Error(BROKEN_CONNECTION_MSG);
                 let V = await G.json();
                 return "api" in V && (V = V.api), V.named_endpoints["/predict"] && !V.unnamed_endpoints[0] && (V.unnamed_endpoints[0] = V.named_endpoints["/predict"]), transform_api_info(V, I, g);
             }
         });
     }
@@ -4537,15 +4537,15 @@
         bubble.call(this, i, G);
     }
 
     function I(G) {
         bubble.call(this, i, G);
     }
 
-    function U(G) {
+    function j(G) {
         binding_callbacks$1[G ? "unshift" : "push"](() => {
             m = G, n(7, m);
         });
     }
     return i.$$set = (G) => {
         "filetype" in G && n(0, f = G.filetype), "dragging" in G && n(11, A = G.dragging), "boundedheight" in G && n(1, a = G.boundedheight), "center" in G && n(2, h = G.center), "flex" in G && n(3, o = G.flex), "file_count" in G && n(4, F = G.file_count), "disable_click" in G && n(12, R = G.disable_click), "root" in G && n(13, w = G.root), "hidden" in G && n(5, T = G.hidden), "$$scope" in G && n(15, s = G.$$scope);
     }, [
@@ -4569,15 +4569,15 @@
         M,
         _,
         N,
         D,
         X,
         Y,
         I,
-        U
+        j
     ];
 }
 class Upload extends SvelteComponent$2 {
     constructor(t) {
         super(), init$2(this, t, instance$2, create_fragment$2, safe_not_equal$2, {
             filetype: 0,
             dragging: 11,
@@ -4856,15 +4856,15 @@
             var __webpack_modules__ = [,
                     /* 1 */
                     /***/
                     (i, t) => {
                         var Vt;
                         Object.defineProperty(t, "__esModule", {
                             value: !0
-                        }), t.VerbosityLevel = t.Util = t.UnknownErrorException = t.UnexpectedResponseException = t.TextRenderingMode = t.RenderingIntentFlag = t.PromiseCapability = t.PermissionFlag = t.PasswordResponses = t.PasswordException = t.PageActionEventType = t.OPS = t.MissingPDFException = t.MAX_IMAGE_SIZE_TO_CACHE = t.LINE_FACTOR = t.LINE_DESCENT_FACTOR = t.InvalidPDFException = t.ImageKind = t.IDENTITY_MATRIX = t.FormatError = t.FeatureTest = t.FONT_IDENTITY_MATRIX = t.DocumentActionEventType = t.CMapCompressionType = t.BaseException = t.BASELINE_FACTOR = t.AnnotationType = t.AnnotationReplyType = t.AnnotationPrefix = t.AnnotationMode = t.AnnotationFlag = t.AnnotationFieldFlag = t.AnnotationEditorType = t.AnnotationEditorPrefix = t.AnnotationEditorParamsType = t.AnnotationBorderStyleType = t.AnnotationActionEventType = t.AbortException = void 0, t.assert = st, t.bytesToString = z, t.createValidAbsoluteUrl = yt, t.getModificationDate = Tt, t.getUuid = Gt, t.getVerbosityLevel = U, t.info = G, t.isArrayBuffer = pt, t.isArrayEqual = Ct, t.isNodeJS = void 0, t.normalizeUnicode = zt, t.objectFromMap = ht, t.objectSize = lt, t.setVerbosityLevel = I, t.shadow = gt, t.string32 = Z, t.stringToBytes = it, t.stringToPDFString = _t, t.stringToUTF8String = rt, t.unreachable = H, t.utf8StringToString = at, t.warn = V;
+                        }), t.VerbosityLevel = t.Util = t.UnknownErrorException = t.UnexpectedResponseException = t.TextRenderingMode = t.RenderingIntentFlag = t.PromiseCapability = t.PermissionFlag = t.PasswordResponses = t.PasswordException = t.PageActionEventType = t.OPS = t.MissingPDFException = t.MAX_IMAGE_SIZE_TO_CACHE = t.LINE_FACTOR = t.LINE_DESCENT_FACTOR = t.InvalidPDFException = t.ImageKind = t.IDENTITY_MATRIX = t.FormatError = t.FeatureTest = t.FONT_IDENTITY_MATRIX = t.DocumentActionEventType = t.CMapCompressionType = t.BaseException = t.BASELINE_FACTOR = t.AnnotationType = t.AnnotationReplyType = t.AnnotationPrefix = t.AnnotationMode = t.AnnotationFlag = t.AnnotationFieldFlag = t.AnnotationEditorType = t.AnnotationEditorPrefix = t.AnnotationEditorParamsType = t.AnnotationBorderStyleType = t.AnnotationActionEventType = t.AbortException = void 0, t.assert = st, t.bytesToString = z, t.createValidAbsoluteUrl = yt, t.getModificationDate = Tt, t.getUuid = Gt, t.getVerbosityLevel = j, t.info = G, t.isArrayBuffer = pt, t.isArrayEqual = Ct, t.isNodeJS = void 0, t.normalizeUnicode = zt, t.objectFromMap = ht, t.objectSize = lt, t.setVerbosityLevel = I, t.shadow = gt, t.string32 = Z, t.stringToBytes = it, t.stringToPDFString = _t, t.stringToUTF8String = rt, t.unreachable = H, t.utf8StringToString = at, t.warn = V;
                         const n = typeof process == "object" && process + "" == "[object process]" && !process.versions.nw && !(process.versions.electron && process.type && process.type !== "browser");
                         t.isNodeJS = n;
                         const e = [1, 0, 0, 1, 0, 0];
                         t.IDENTITY_MATRIX = e;
                         const s = [1e-3, 0, 0, 1e-3, 0, 0];
                         t.FONT_IDENTITY_MATRIX = s;
                         const p = 1e7;
@@ -5160,15 +5160,15 @@
                         t.PasswordResponses = X;
                         let Y = _.WARNINGS;
 
                         function I(ut) {
                             Number.isInteger(ut) && (Y = ut);
                         }
 
-                        function U() {
+                        function j() {
                             return Y;
                         }
 
                         function G(ut) {
                             Y >= _.INFOS && console.log(`Info: ${ut}`);
                         }
 
@@ -5413,23 +5413,23 @@
                             }
                             static bezierBoundingBox(nt, Q, At, wt, te, Qt, et, Et) {
                                 const Ot = [],
                                     Pt = [
                                         [],
                                         []
                                     ];
-                                let $t, Nt, Jt, vt, Yt, Lt, j, c;
+                                let $t, Nt, Jt, vt, Yt, Lt, U, c;
                                 for (let tt = 0; tt < 2; ++tt) {
                                     if (tt === 0 ? (Nt = 6 * nt - 12 * At + 6 * te, $t = -3 * nt + 9 * At - 9 * te + 3 * et, Jt = 3 * At - 3 * nt) : (Nt = 6 * Q - 12 * wt + 6 * Qt, $t = -3 * Q + 9 * wt - 9 * Qt + 3 * Et, Jt = 3 * wt - 3 * Q), Math.abs($t) < 1e-12) {
                                         if (Math.abs(Nt) < 1e-12)
                                             continue;
                                         vt = -Jt / Nt, 0 < vt && vt < 1 && Ot.push(vt);
                                         continue;
                                     }
-                                    j = Nt * Nt - 4 * Jt * $t, c = Math.sqrt(j), !(j < 0) && (Yt = (-Nt + c) / (2 * $t), 0 < Yt && Yt < 1 && Ot.push(Yt), Lt = (-Nt - c) / (2 * $t), 0 < Lt && Lt < 1 && Ot.push(Lt));
+                                    U = Nt * Nt - 4 * Jt * $t, c = Math.sqrt(U), !(U < 0) && (Yt = (-Nt + c) / (2 * $t), 0 < Yt && Yt < 1 && Ot.push(Yt), Lt = (-Nt - c) / (2 * $t), 0 < Lt && Lt < 1 && Ot.push(Lt));
                                 }
                                 let L = Ot.length,
                                     q;
                                 const K = L;
                                 for (; L--;)
                                     vt = Ot[L], q = 1 - vt, Pt[0][L] = q * q * q * nt + 3 * q * q * vt * At + 3 * q * vt * vt * te + vt * vt * vt * et, Pt[1][L] = q * q * q * Q + 3 * q * q * vt * wt + 3 * q * vt * vt * Qt + vt * vt * vt * Et;
                                 return Pt[0][K] = nt, Pt[1][K] = Q, Pt[0][K + 1] = et, Pt[1][K + 1] = Et, Pt[0].length = Pt[1].length = K + 2, [Math.min(...Pt[0]), Math.min(...Pt[1]), Math.max(...Pt[0]), Math.max(...Pt[1])];
@@ -5576,15 +5576,15 @@
                                 {
                                     docId: N
                                 } = _,
                                 D = M.url ? getUrlProp(M.url) : null,
                                 X = M.data ? getDataProp(M.data) : null,
                                 Y = M.httpHeaders || null,
                                 I = M.withCredentials === !0,
-                                U = M.password ?? null,
+                                j = M.password ?? null,
                                 G = M.range instanceof PDFDataRangeTransport ? M.range : null,
                                 V = Number.isInteger(M.rangeChunkSize) && M.rangeChunkSize > 0 ? M.rangeChunkSize : DEFAULT_RANGE_CHUNK_SIZE;
                             let H = M.worker instanceof PDFWorker ? M.worker : null;
                             const st = M.verbosity,
                                 dt = typeof M.docBaseUrl == "string" && !(0, _display_utils.isDataScheme)(M.docBaseUrl) ? M.docBaseUrl : null,
                                 yt = typeof M.cMapUrl == "string" ? M.cMapUrl : null,
                                 gt = M.cMapPacked !== !1,
@@ -5632,15 +5632,15 @@
                                 };
                                 H = Bt.port ? PDFWorker.fromPort(Bt) : new PDFWorker(Bt), _._worker = H;
                             }
                             const Ct = {
                                     docId: N,
                                     apiVersion: "3.11.174",
                                     data: X,
-                                    password: U,
+                                    password: j,
                                     disableAutoFetch: ft,
                                     rangeChunkSize: V,
                                     length: Rt,
                                     docBaseUrl: dt,
                                     enableXfa: Z,
                                     evaluatorOptions: {
                                         maxImageSize: b,
@@ -5970,23 +5970,23 @@
                             render({
                                 canvasContext: _,
                                 viewport: N,
                                 intent: D = "display",
                                 annotationMode: X = _util.AnnotationMode.ENABLE,
                                 transform: Y = null,
                                 background: I = null,
-                                optionalContentConfigPromise: U = null,
+                                optionalContentConfigPromise: j = null,
                                 annotationCanvasMap: G = null,
                                 pageColors: V = null,
                                 printAnnotationStorage: H = null
                             }) {
                                 var u, d;
                                 (u = this._stats) == null || u.time("Overall");
                                 const st = this._transport.getRenderingIntent(D, X, H);
-                                ot(this, e, !1), J(this, f, we).call(this), U || (U = this._transport.getOptionalContentConfig());
+                                ot(this, e, !1), J(this, f, we).call(this), j || (j = this._transport.getOptionalContentConfig());
                                 let dt = this._intentStates.get(st.cacheKey);
                                 dt || (dt = /* @__PURE__ */ Object.create(null), this._intentStates.set(st.cacheKey, dt)), dt.streamReaderCancelTimeout && (clearTimeout(dt.streamReaderCancelTimeout), dt.streamReaderCancelTimeout = null);
                                 const yt = !!(st.renderingIntent & _util.RenderingIntentFlag.PRINT);
                                 dt.displayReadyCapability || (dt.displayReadyCapability = new _util.PromiseCapability(), dt.operatorList = {
                                     fnArray: [],
                                     argsArray: [],
                                     lastChunk: !1,
@@ -6016,15 +6016,15 @@
                                         filterFactory: this._transport.filterFactory,
                                         useRequestAnimationFrame: !yt,
                                         pdfBug: this._pdfBug,
                                         pageColors: V
                                     });
                                 (dt.renderTasks || (dt.renderTasks = /* @__PURE__ */ new Set())).add(k);
                                 const l = k.task;
-                                return Promise.all([dt.displayReadyCapability.promise, U]).then(([b, y]) => {
+                                return Promise.all([dt.displayReadyCapability.promise, j]).then(([b, y]) => {
                                     var O;
                                     if (this.destroyed) {
                                         gt();
                                         return;
                                     }
                                     (O = this._stats) == null || O.time("Rendering"), k.initializeGraphics({
                                         transparency: b,
@@ -6036,21 +6036,21 @@
                                 intent: _ = "display",
                                 annotationMode: N = _util.AnnotationMode.ENABLE,
                                 printAnnotationStorage: D = null
                             } = {}) {
                                 var G;
 
                                 function X() {
-                                    I.operatorList.lastChunk && (I.opListReadCapability.resolve(I.operatorList), I.renderTasks.delete(U));
+                                    I.operatorList.lastChunk && (I.opListReadCapability.resolve(I.operatorList), I.renderTasks.delete(j));
                                 }
                                 const Y = this._transport.getRenderingIntent(_, N, D, !0);
                                 let I = this._intentStates.get(Y.cacheKey);
                                 I || (I = /* @__PURE__ */ Object.create(null), this._intentStates.set(Y.cacheKey, I));
-                                let U;
-                                return I.opListReadCapability || (U = /* @__PURE__ */ Object.create(null), U.operatorListChanged = X, I.opListReadCapability = new _util.PromiseCapability(), (I.renderTasks || (I.renderTasks = /* @__PURE__ */ new Set())).add(U), I.operatorList = {
+                                let j;
+                                return I.opListReadCapability || (j = /* @__PURE__ */ Object.create(null), j.operatorListChanged = X, I.opListReadCapability = new _util.PromiseCapability(), (I.renderTasks || (I.renderTasks = /* @__PURE__ */ new Set())).add(j), I.operatorList = {
                                     fnArray: [],
                                     argsArray: [],
                                     lastChunk: !1,
                                     separateAnnots: null
                                 }, (G = this._stats) == null || G.time("Page Request"), this._pumpOperatorList(Y)), I.opListReadCapability.promise;
                             }
                             streamTextContent({
@@ -6075,22 +6075,22 @@
                                 return new Promise(function(D, X) {
                                     function Y() {
                                         I.read().then(function({
                                             value: G,
                                             done: V
                                         }) {
                                             if (V) {
-                                                D(U);
+                                                D(j);
                                                 return;
                                             }
-                                            Object.assign(U.styles, G.styles), U.items.push(...G.items), Y();
+                                            Object.assign(j.styles, G.styles), j.items.push(...G.items), Y();
                                         }, X);
                                     }
                                     const I = N.getReader(),
-                                        U = {
+                                        j = {
                                             items: [],
                                             styles: /* @__PURE__ */ Object.create(null)
                                         };
                                     Y();
                                 });
                             }
                             getStructTree() {
@@ -6131,23 +6131,23 @@
                                 renderingIntent: _,
                                 cacheKey: N,
                                 annotationStorageSerializable: D
                             }) {
                                 const {
                                     map: X,
                                     transfers: Y
-                                } = D, U = this._transport.messageHandler.sendWithStream("GetOperatorList", {
+                                } = D, j = this._transport.messageHandler.sendWithStream("GetOperatorList", {
                                     pageIndex: this._pageIndex,
                                     intent: _,
                                     cacheKey: N,
                                     annotationStorage: X
                                 }, Y).getReader(), G = this._intentStates.get(N);
-                                G.streamReader = U;
+                                G.streamReader = j;
                                 const V = () => {
-                                    U.read().then(({
+                                    j.read().then(({
                                         value: H,
                                         done: st
                                     }) => {
                                         if (st) {
                                             G.streamReader = null;
                                             return;
                                         }
@@ -6518,19 +6518,19 @@
                                         });
                                     };
                                 }), _.on("ReaderHeadersReady", (D) => {
                                     const X = new _util.PromiseCapability(),
                                         Y = this._fullReader;
                                     return Y.headersReady.then(() => {
                                         var I;
-                                        (!Y.isStreamingSupported || !Y.isRangeSupported) && (this._lastProgress && ((I = N.onProgress) == null || I.call(N, this._lastProgress)), Y.onProgress = (U) => {
+                                        (!Y.isStreamingSupported || !Y.isRangeSupported) && (this._lastProgress && ((I = N.onProgress) == null || I.call(N, this._lastProgress)), Y.onProgress = (j) => {
                                             var G;
                                             (G = N.onProgress) == null || G.call(N, {
-                                                loaded: U.loaded,
-                                                total: U.total
+                                                loaded: j.loaded,
+                                                total: j.total
                                             });
                                         }), X.resolve({
                                             isStreamingSupported: Y.isStreamingSupported,
                                             isRangeSupported: Y.isRangeSupported,
                                             contentLength: Y.contentLength
                                         });
                                     }, X.reject), X.promise;
@@ -6540,28 +6540,28 @@
                                     if (!Y) {
                                         X.close();
                                         return;
                                     }
                                     X.onPull = () => {
                                         Y.read().then(function({
                                             value: I,
-                                            done: U
+                                            done: j
                                         }) {
-                                            if (U) {
+                                            if (j) {
                                                 X.close();
                                                 return;
                                             }
                                             (0, _util.assert)(I instanceof ArrayBuffer, "GetRangeReader - expected an ArrayBuffer."), X.enqueue(new Uint8Array(I), 1, [I]);
                                         }).catch((I) => {
                                             X.error(I);
                                         });
                                     }, X.onCancel = (I) => {
-                                        Y.cancel(I), X.ready.catch((U) => {
+                                        Y.cancel(I), X.ready.catch((j) => {
                                             if (!this.destroyed)
-                                                throw U;
+                                                throw j;
                                         });
                                     };
                                 }), _.on("GetDoc", ({
                                     pdfInfo: D
                                 }) => {
                                     this._numPages = D.numPages, this._htmlForXfa = D.htmlForXfa, delete D.htmlForXfa, N._capability.resolve(new PDFDocumentProxy(D, this));
                                 }), _.on("DocException", function(D) {
@@ -6612,64 +6612,64 @@
                                         return;
                                     r(this, w).get(D.pageIndex)._startRenderPage(D.transparency, D.cacheKey);
                                 }), _.on("commonobj", ([D, X, Y]) => {
                                     var I;
                                     if (!this.destroyed && !this.commonObjs.has(D))
                                         switch (X) {
                                             case "Font":
-                                                const U = this._params;
+                                                const j = this._params;
                                                 if ("error" in Y) {
                                                     const H = Y.error;
                                                     (0, _util.warn)(`Error during font loading: ${H}`), this.commonObjs.resolve(D, H);
                                                     break;
                                                 }
-                                                const G = U.pdfBug && ((I = globalThis.FontInspector) != null && I.enabled) ? (H, st) => globalThis.FontInspector.fontAdded(H, st) : null,
+                                                const G = j.pdfBug && ((I = globalThis.FontInspector) != null && I.enabled) ? (H, st) => globalThis.FontInspector.fontAdded(H, st) : null,
                                                     V = new _font_loader.FontFaceObject(Y, {
-                                                        isEvalSupported: U.isEvalSupported,
-                                                        disableFontFace: U.disableFontFace,
-                                                        ignoreErrors: U.ignoreErrors,
+                                                        isEvalSupported: j.isEvalSupported,
+                                                        disableFontFace: j.disableFontFace,
+                                                        ignoreErrors: j.ignoreErrors,
                                                         inspectFont: G
                                                     });
                                                 this.fontLoader.bind(V).catch((H) => _.sendWithPromise("FontFallback", {
                                                     id: D
                                                 })).finally(() => {
-                                                    !U.fontExtraProperties && V.data && (V.data = null), this.commonObjs.resolve(D, V);
+                                                    !j.fontExtraProperties && V.data && (V.data = null), this.commonObjs.resolve(D, V);
                                                 });
                                                 break;
                                             case "FontPath":
                                             case "Image":
                                             case "Pattern":
                                                 this.commonObjs.resolve(D, Y);
                                                 break;
                                             default:
                                                 throw new Error(`Got unknown common object type ${X}`);
                                         }
                                 }), _.on("obj", ([D, X, Y, I]) => {
                                     var G;
                                     if (this.destroyed)
                                         return;
-                                    const U = r(this, w).get(X);
-                                    if (!U.objs.has(D))
+                                    const j = r(this, w).get(X);
+                                    if (!j.objs.has(D))
                                         switch (Y) {
                                             case "Image":
-                                                if (U.objs.resolve(D, I), I) {
+                                                if (j.objs.resolve(D, I), I) {
                                                     let V;
                                                     if (I.bitmap) {
                                                         const {
                                                             width: H,
                                                             height: st
                                                         } = I;
                                                         V = H * st * 4;
                                                     } else
                                                         V = ((G = I.data) == null ? void 0 : G.length) || 0;
-                                                    V > _util.MAX_IMAGE_SIZE_TO_CACHE && (U._maybeCleanupAfterRender = !0);
+                                                    V > _util.MAX_IMAGE_SIZE_TO_CACHE && (j._maybeCleanupAfterRender = !0);
                                                 }
                                                 break;
                                             case "Pattern":
-                                                U.objs.resolve(D, I);
+                                                j.objs.resolve(D, I);
                                                 break;
                                             default:
                                                 throw new Error(`Got unknown object type ${Y}`);
                                         }
                                 }), _.on("DocProgress", (D) => {
                                     var X;
                                     this.destroyed || (X = N.onProgress) == null || X.call(N, {
@@ -6898,39 +6898,39 @@
                             constructor({
                                 callback: _,
                                 params: N,
                                 objs: D,
                                 commonObjs: X,
                                 annotationCanvasMap: Y,
                                 operatorList: I,
-                                pageIndex: U,
+                                pageIndex: j,
                                 canvasFactory: G,
                                 filterFactory: V,
                                 useRequestAnimationFrame: H = !1,
                                 pdfBug: st = !1,
                                 pageColors: dt = null
                             }) {
-                                this.callback = _, this.params = N, this.objs = D, this.commonObjs = X, this.annotationCanvasMap = Y, this.operatorListIdx = null, this.operatorList = I, this._pageIndex = U, this.canvasFactory = G, this.filterFactory = V, this._pdfBug = st, this.pageColors = dt, this.running = !1, this.graphicsReadyCallback = null, this.graphicsReady = !1, this._useRequestAnimationFrame = H === !0 && typeof window < "u", this.cancelled = !1, this.capability = new _util.PromiseCapability(), this.task = new RenderTask(this), this._cancelBound = this.cancel.bind(this), this._continueBound = this._continue.bind(this), this._scheduleNextBound = this._scheduleNext.bind(this), this._nextBound = this._next.bind(this), this._canvas = N.canvasContext.canvas;
+                                this.callback = _, this.params = N, this.objs = D, this.commonObjs = X, this.annotationCanvasMap = Y, this.operatorListIdx = null, this.operatorList = I, this._pageIndex = j, this.canvasFactory = G, this.filterFactory = V, this._pdfBug = st, this.pageColors = dt, this.running = !1, this.graphicsReadyCallback = null, this.graphicsReady = !1, this._useRequestAnimationFrame = H === !0 && typeof window < "u", this.cancelled = !1, this.capability = new _util.PromiseCapability(), this.task = new RenderTask(this), this._cancelBound = this.cancel.bind(this), this._continueBound = this._continue.bind(this), this._scheduleNextBound = this._scheduleNext.bind(this), this._nextBound = this._next.bind(this), this._canvas = N.canvasContext.canvas;
                             }
                             get completed() {
                                 return this.capability.promise.catch(function() {});
                             }
                             initializeGraphics({
                                 transparency: _ = !1,
                                 optionalContentConfig: N
                             }) {
-                                var U, G;
+                                var j, G;
                                 if (this.cancelled)
                                     return;
                                 if (this._canvas) {
                                     if (r($, v).has(this._canvas))
                                         throw new Error("Cannot use the same canvas during multiple render() operations. Use different canvas or ensure previous operations were cancelled or completed.");
                                     r($, v).add(this._canvas);
                                 }
-                                this._pdfBug && ((U = globalThis.StepperManager) != null && U.enabled) && (this.stepper = globalThis.StepperManager.create(this._pageIndex), this.stepper.init(this.operatorList), this.stepper.nextBreakPoint = this.stepper.getNextBreakPoint());
+                                this._pdfBug && ((j = globalThis.StepperManager) != null && j.enabled) && (this.stepper = globalThis.StepperManager.create(this._pageIndex), this.stepper.init(this.operatorList), this.stepper.nextBreakPoint = this.stepper.getNextBreakPoint());
                                 const {
                                     canvasContext: D,
                                     viewport: X,
                                     transform: Y,
                                     background: I
                                 } = this.params;
                                 this.gfx = new _canvas.CanvasGraphics(D, this.commonObjs, this.objs, this.canvasFactory, this.filterFactory, {
@@ -7732,28 +7732,28 @@
                                 };
                             }
                         }
                     },
                     /* 5 */
                     /***/
                     (i, t, n) => {
-                        var w, T, P, m, C, He, S, g, v, $, M, kn, D, X, Y, I, U, G, V, H, st, dt, yt, gt, k, l, u, d, b, y, O, B, z, it, Z, lt, ht, mt, ft, kt, Rt, St, It, _t, rt, at, pt, Tn, Tt, ze, Wt, Ge, zt, Ce, qt, Xe, ut, Ve, Q, re, wt, _e, Qt, Pn, Et, Fn, Pt, Ye, Nt, me, vt, Ke;
+                        var w, T, P, m, C, He, S, g, v, $, M, kn, D, X, Y, I, j, G, V, H, st, dt, yt, gt, k, l, u, d, b, y, O, B, z, it, Z, lt, ht, mt, ft, kt, Rt, St, It, _t, rt, at, pt, Tn, Tt, ze, Wt, Ge, zt, Ce, qt, Xe, ut, Ve, Q, re, wt, _e, Qt, Pn, Et, Fn, Pt, Ye, Nt, me, vt, Ke;
                         Object.defineProperty(t, "__esModule", {
                             value: !0
                         }), t.KeyboardManager = t.CommandManager = t.ColorManager = t.AnnotationEditorUIManager = void 0, t.bindEvents = p, t.opacityToHex = f;
                         var e = n(1),
                             s = n(6);
 
-                        function p(j, c, L) {
+                        function p(U, c, L) {
                             for (const q of L)
-                                c.addEventListener(q, j[q].bind(j));
+                                c.addEventListener(q, U[q].bind(U));
                         }
 
-                        function f(j) {
-                            return Math.round(Math.min(255, Math.max(1, 255 * j))).toString(16).padStart(2, "0");
+                        function f(U) {
+                            return Math.round(Math.min(255, Math.max(1, 255 * U))).toString(16).padStart(2, "0");
                         }
                         class A {
                             constructor() {
                                 W(this, w, 0);
                             }
                             getId() {
                                 return `${e.AnnotationEditorPrefix}${ge(this, w)._++}`;
@@ -7985,15 +7985,15 @@
                                 W(this, Pt);
                                 W(this, Nt);
                                 W(this, vt);
                                 W(this, D, null);
                                 W(this, X, /* @__PURE__ */ new Map());
                                 W(this, Y, /* @__PURE__ */ new Map());
                                 W(this, I, null);
-                                W(this, U, null);
+                                W(this, j, null);
                                 W(this, G, new h());
                                 W(this, V, 0);
                                 W(this, H, /* @__PURE__ */ new Set());
                                 W(this, st, null);
                                 W(this, dt, null);
                                 W(this, yt, /* @__PURE__ */ new Set());
                                 W(this, gt, null);
@@ -8021,15 +8021,15 @@
                                     hasSomethingToRedo: !1,
                                     hasSelectedEditor: !1
                                 });
                                 W(this, It, [0, 0]);
                                 W(this, _t, null);
                                 W(this, rt, null);
                                 W(this, at, null);
-                                ot(this, rt, c), ot(this, at, L), ot(this, I, q), this._eventBus = K, this._eventBus._on("editingaction", r(this, mt)), this._eventBus._on("pagechanging", r(this, ft)), this._eventBus._on("scalechanging", r(this, kt)), this._eventBus._on("rotationchanging", r(this, Rt)), ot(this, U, tt.annotationStorage), ot(this, gt, tt.filterFactory), ot(this, O, ct), this.viewParameters = {
+                                ot(this, rt, c), ot(this, at, L), ot(this, I, q), this._eventBus = K, this._eventBus._on("editingaction", r(this, mt)), this._eventBus._on("pagechanging", r(this, ft)), this._eventBus._on("scalechanging", r(this, kt)), this._eventBus._on("rotationchanging", r(this, Rt)), ot(this, j, tt.annotationStorage), ot(this, gt, tt.filterFactory), ot(this, O, ct), this.viewParameters = {
                                     realScale: s.PixelsPerInch.PDF_TO_CSS_UNITS,
                                     rotation: 0
                                 };
                             }
                             static get _keyboardManager() {
                                 const c = Lt.prototype,
                                     L = (tt) => {
@@ -8161,15 +8161,15 @@
                             }
                             onRotationChanging({
                                 pagesRotation: c
                             }) {
                                 this.commitOrRemove(), this.viewParameters.rotation = c;
                             }
                             addToAnnotationStorage(c) {
-                                !c.isEmpty() && r(this, U) && !r(this, U).has(c.id) && r(this, U).setValue(c.id, c);
+                                !c.isEmpty() && r(this, j) && !r(this, j).has(c.id) && r(this, j).setValue(c.id, c);
                             }
                             blur() {
                                 if (!this.hasSelection)
                                     return;
                                 const {
                                     activeElement: c
                                 } = document;
@@ -8355,15 +8355,15 @@
                                 return r(this, X).get(c);
                             }
                             addEditor(c) {
                                 r(this, X).set(c.id, c);
                             }
                             removeEditor(c) {
                                 var L;
-                                r(this, X).delete(c.id), this.unselect(c), (!c.annotationElementId || !r(this, H).has(c.annotationElementId)) && ((L = r(this, U)) == null || L.remove(c.id));
+                                r(this, X).delete(c.id), this.unselect(c), (!c.annotationElementId || !r(this, H).has(c.annotationElementId)) && ((L = r(this, j)) == null || L.remove(c.id));
                             }
                             addDeletedAnnotationElement(c) {
                                 r(this, H).add(c.annotationElementId), c.deleted = !0;
                             }
                             isDeletedAnnotationElement(c) {
                                 return r(this, H).has(c);
                             }
@@ -8563,15 +8563,15 @@
                             getMode() {
                                 return r(this, b);
                             }
                             get imageManager() {
                                 return (0, e.shadow)(this, "imageManager", new a());
                             }
                         };
-                        D = new WeakMap(), X = new WeakMap(), Y = new WeakMap(), I = new WeakMap(), U = new WeakMap(), G = new WeakMap(), V = new WeakMap(), H = new WeakMap(), st = new WeakMap(), dt = new WeakMap(), yt = new WeakMap(), gt = new WeakMap(), k = new WeakMap(), l = new WeakMap(), u = new WeakMap(), d = new WeakMap(), b = new WeakMap(), y = new WeakMap(), O = new WeakMap(), B = new WeakMap(), z = new WeakMap(), it = new WeakMap(), Z = new WeakMap(), lt = new WeakMap(), ht = new WeakMap(), mt = new WeakMap(), ft = new WeakMap(), kt = new WeakMap(), Rt = new WeakMap(), St = new WeakMap(), It = new WeakMap(), _t = new WeakMap(), rt = new WeakMap(), at = new WeakMap(), pt = new WeakSet(), Tn = function() {
+                        D = new WeakMap(), X = new WeakMap(), Y = new WeakMap(), I = new WeakMap(), j = new WeakMap(), G = new WeakMap(), V = new WeakMap(), H = new WeakMap(), st = new WeakMap(), dt = new WeakMap(), yt = new WeakMap(), gt = new WeakMap(), k = new WeakMap(), l = new WeakMap(), u = new WeakMap(), d = new WeakMap(), b = new WeakMap(), y = new WeakMap(), O = new WeakMap(), B = new WeakMap(), z = new WeakMap(), it = new WeakMap(), Z = new WeakMap(), lt = new WeakMap(), ht = new WeakMap(), mt = new WeakMap(), ft = new WeakMap(), kt = new WeakMap(), Rt = new WeakMap(), St = new WeakMap(), It = new WeakMap(), _t = new WeakMap(), rt = new WeakMap(), at = new WeakMap(), pt = new WeakSet(), Tn = function() {
                             window.addEventListener("focus", r(this, z)), window.addEventListener("blur", r(this, B));
                         }, Tt = new WeakSet(), ze = function() {
                             window.removeEventListener("focus", r(this, z)), window.removeEventListener("blur", r(this, B));
                         }, Wt = new WeakSet(), Ge = function() {
                             window.addEventListener("keydown", r(this, ht), {
                                 capture: !0
                             });
@@ -8628,15 +8628,15 @@
                     },
                     /* 6 */
                     /***/
                     (i, t, n) => {
                         var V, H, st, dt, yt, gt, k, l, u, d, b, y, de, B, ue, it, Je, lt, ke, mt, Te, kt, be, St, ye;
                         Object.defineProperty(t, "__esModule", {
                             value: !0
-                        }), t.StatTimer = t.RenderingCancelledException = t.PixelsPerInch = t.PageViewport = t.PDFDateString = t.DOMStandardFontDataFactory = t.DOMSVGFactory = t.DOMFilterFactory = t.DOMCanvasFactory = t.DOMCMapReaderFactory = void 0, t.deprecated = $, t.getColorValues = X, t.getCurrentTransform = Y, t.getCurrentTransformInverse = I, t.getFilenameFromUrl = C, t.getPdfFilenameFromUrl = x, t.getRGB = D, t.getXfaPageViewport = N, t.isDataScheme = P, t.isPdfFile = m, t.isValidFetchUrl = S, t.loadScript = v, t.noContextMenu = g, t.setLayerDimensions = U;
+                        }), t.StatTimer = t.RenderingCancelledException = t.PixelsPerInch = t.PageViewport = t.PDFDateString = t.DOMStandardFontDataFactory = t.DOMSVGFactory = t.DOMFilterFactory = t.DOMCanvasFactory = t.DOMCMapReaderFactory = void 0, t.deprecated = $, t.getColorValues = X, t.getCurrentTransform = Y, t.getCurrentTransformInverse = I, t.getFilenameFromUrl = C, t.getPdfFilenameFromUrl = x, t.getRGB = D, t.getXfaPageViewport = N, t.isDataScheme = P, t.isPdfFile = m, t.isValidFetchUrl = S, t.loadScript = v, t.noContextMenu = g, t.setLayerDimensions = j;
                         var e = n(7),
                             s = n(1);
                         const p = "http://www.w3.org/2000/svg",
                             G = class G {};
                         ee(G, "CSS", 96), ee(G, "PDF", 72), ee(G, "PDF_TO_CSS_UNITS", G.CSS / G.PDF);
                         let f = G;
                         t.PixelsPerInch = f;
@@ -9104,15 +9104,15 @@
                                 d: Ct,
                                 e: Tt,
                                 f: Bt
                             } = _t.getTransform().invertSelf();
                             return [rt, at, pt, Ct, Tt, Bt];
                         }
 
-                        function U(_t, rt, at = !1, pt = !0) {
+                        function j(_t, rt, at = !1, pt = !0) {
                             if (rt instanceof w) {
                                 const {
                                     pageWidth: Ct,
                                     pageHeight: Tt
                                 } = rt.rawDims, {
                                     style: Bt
                                 } = _t, Wt = s.FeatureTest.isCSSRoundSupported, jt = `var(--scale-factor) * ${Ct}px`, zt = `var(--scale-factor) * ${Tt}px`, Gt = Wt ? `round(${jt}, 1px)` : `calc(${jt})`, qt = Wt ? `round(${zt}, 1px)` : `calc(${zt})`;
@@ -9411,17 +9411,17 @@
                             }
                             _prepareFontLoadEvent(a, h) {
                                 function o(D, X) {
                                     return D.charCodeAt(X) << 24 | D.charCodeAt(X + 1) << 16 | D.charCodeAt(X + 2) << 8 | D.charCodeAt(X + 3) & 255;
                                 }
 
                                 function F(D, X, Y, I) {
-                                    const U = D.substring(0, X),
+                                    const j = D.substring(0, X),
                                         G = D.substring(X + Y);
-                                    return U + I + G;
+                                    return j + I + G;
                                 }
                                 let R, w;
                                 const T = this._document.createElement("canvas");
                                 T.width = 1, T.height = 1;
                                 const P = T.getContext("2d");
                                 let m = 0;
 
@@ -9952,15 +9952,15 @@
                             const u = e.Util.singularValueDecompose2dScale(k);
                             u[0] = Math.fround(u[0]), u[1] = Math.fround(u[1]);
                             const d = Math.fround((globalThis.devicePixelRatio || 1) * s.PixelsPerInch.PDF_TO_CSS_UNITS);
                             return l !== void 0 ? l : u[0] <= d || u[1] <= d;
                         }
                         const Y = ["butt", "round", "square"],
                             I = ["miter", "round", "bevel"],
-                            U = {},
+                            j = {},
                             G = {},
                             gt = class gt {
                                 constructor(l, u, d, b, y, {
                                     optionalContentConfig: O,
                                     markedContentStack: B = null
                                 }, z, it) {
                                     W(this, H);
@@ -10275,15 +10275,15 @@
                                 closeEOFillStroke() {
                                     this.pendingEOFill = !0, this.closePath(), this.fillStroke();
                                 }
                                 endPath() {
                                     this.consumePath();
                                 }
                                 clip() {
-                                    this.pendingClip = U;
+                                    this.pendingClip = j;
                                 }
                                 eoClip() {
                                     this.pendingClip = G;
                                 }
                                 beginText() {
                                     this.current.textMatrix = e.IDENTITY_MATRIX, this.current.textMatrixScale = 1, this.current.x = this.current.lineX = 0, this.current.y = this.current.lineY = 0;
                                 }
@@ -10970,43 +10970,43 @@
                             const _ = x.coords,
                                 N = x.colors,
                                 D = C.data,
                                 X = C.width * 4;
                             let Y;
                             _[E + 1] > _[S + 1] && (Y = E, E = S, S = Y, Y = v, v = $, $ = Y), _[S + 1] > _[g + 1] && (Y = S, S = g, g = Y, Y = $, $ = M, M = Y), _[E + 1] > _[S + 1] && (Y = E, E = S, S = Y, Y = v, v = $, $ = Y);
                             const I = (_[E] + x.offsetX) * x.scaleX,
-                                U = (_[E + 1] + x.offsetY) * x.scaleY,
+                                j = (_[E + 1] + x.offsetY) * x.scaleY,
                                 G = (_[S] + x.offsetX) * x.scaleX,
                                 V = (_[S + 1] + x.offsetY) * x.scaleY,
                                 H = (_[g] + x.offsetX) * x.scaleX,
                                 st = (_[g + 1] + x.offsetY) * x.scaleY;
-                            if (U >= st)
+                            if (j >= st)
                                 return;
                             const dt = N[v],
                                 yt = N[v + 1],
                                 gt = N[v + 2],
                                 k = N[$],
                                 l = N[$ + 1],
                                 u = N[$ + 2],
                                 d = N[M],
                                 b = N[M + 1],
                                 y = N[M + 2],
-                                O = Math.round(U),
+                                O = Math.round(j),
                                 B = Math.round(st);
                             let z, it, Z, lt, ht, mt, ft, kt;
                             for (let Rt = O; Rt <= B; Rt++) {
                                 if (Rt < V) {
-                                    const at = Rt < U ? 0 : (U - Rt) / (U - V);
+                                    const at = Rt < j ? 0 : (j - Rt) / (j - V);
                                     z = I - (I - G) * at, it = dt - (dt - k) * at, Z = yt - (yt - l) * at, lt = gt - (gt - u) * at;
                                 } else {
                                     let at;
                                     Rt > st ? at = 1 : V === st ? at = 0 : at = (V - Rt) / (V - st), z = G - (G - H) * at, it = k - (k - d) * at, Z = l - (l - b) * at, lt = u - (u - y) * at;
                                 }
                                 let St;
-                                Rt < U ? St = 0 : Rt > st ? St = 1 : St = (U - Rt) / (U - st), ht = I - (I - H) * St, mt = dt - (dt - d) * St, ft = yt - (yt - b) * St, kt = gt - (gt - y) * St;
+                                Rt < j ? St = 0 : Rt > st ? St = 1 : St = (j - Rt) / (j - st), ht = I - (I - H) * St, mt = dt - (dt - d) * St, ft = yt - (yt - b) * St, kt = gt - (gt - y) * St;
                                 const It = Math.round(Math.min(z, ht)),
                                     _t = Math.round(Math.max(z, ht));
                                 let rt = X * Rt + It * 4;
                                 for (let at = It; at <= _t; at++)
                                     St = (z - at) / (z - ht), St < 0 ? St = 0 : St > 1 && (St = 1), D[rt++] = it - (it - mt) * St | 0, D[rt++] = Z - (Z - ft) * St | 0, D[rt++] = lt - (lt - kt) * St | 0, D[rt++] = 255;
                             }
                         }
@@ -11042,22 +11042,22 @@
                                 const M = Math.floor(this._bounds[0]),
                                     _ = Math.floor(this._bounds[1]),
                                     N = Math.ceil(this._bounds[2]) - M,
                                     D = Math.ceil(this._bounds[3]) - _,
                                     X = Math.min(Math.ceil(Math.abs(N * x[0] * 1.1)), 3e3),
                                     Y = Math.min(Math.ceil(Math.abs(D * x[1] * 1.1)), 3e3),
                                     I = N / X,
-                                    U = D / Y,
+                                    j = D / Y,
                                     G = {
                                         coords: this._coords,
                                         colors: this._colors,
                                         offsetX: -M,
                                         offsetY: -_,
                                         scaleX: 1 / I,
-                                        scaleY: 1 / U
+                                        scaleY: 1 / j
                                     },
                                     V = X + 2 * 2,
                                     H = Y + 2 * 2,
                                     st = S.getCanvas("mesh", V, H, !1),
                                     dt = st.context,
                                     yt = dt.createImageData(X, Y);
                                 if (E) {
@@ -11066,17 +11066,17 @@
                                         k[l] = E[0], k[l + 1] = E[1], k[l + 2] = E[2], k[l + 3] = 255;
                                 }
                                 for (const k of this._figures)
                                     o(yt, k, G);
                                 return dt.putImageData(yt, 2, 2), {
                                     canvas: st.canvas,
                                     offsetX: M - 2 * I,
-                                    offsetY: _ - 2 * U,
+                                    offsetY: _ - 2 * j,
                                     scaleX: I,
-                                    scaleY: U
+                                    scaleY: j
                                 };
                             }
                             getPattern(x, E, S, g) {
                                 f(x, this._bbox);
                                 let v;
                                 if (g === p.SHADING)
                                     v = e.Util.singularValueDecompose2dScale((0, s.getCurrentTransform)(x));
@@ -11123,17 +11123,17 @@
                                         _ = this.color,
                                         N = this.canvasGraphicsFactory;
                                     (0, e.info)("TilingType: " + M);
                                     const D = S[0],
                                         X = S[1],
                                         Y = S[2],
                                         I = S[3],
-                                        U = e.Util.singularValueDecompose2dScale(this.matrix),
+                                        j = e.Util.singularValueDecompose2dScale(this.matrix),
                                         G = e.Util.singularValueDecompose2dScale(this.baseTransform),
-                                        V = [U[0] * G[0], U[1] * G[1]],
+                                        V = [j[0] * G[0], j[1] * G[1]],
                                         H = this.getSizeAndScale(g, this.ctx.canvas.width, V[0]),
                                         st = this.getSizeAndScale(v, this.ctx.canvas.height, V[1]),
                                         dt = x.cachedCanvases.getCanvas("pattern", H.size, st.size, !0),
                                         yt = dt.context,
                                         gt = N.createCanvasGraphics(yt);
                                     gt.groupLevel = x.groupLevel, this.setFillAndStrokeStyleToContext(gt, $, _);
                                     let k = D,
@@ -12885,89 +12885,89 @@
                                 const $ = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/=";
                                 let M = `data:${g};base64,`;
                                 for (let _ = 0, N = S.length; _ < N; _ += 3) {
                                     const D = S[_] & 255,
                                         X = S[_ + 1] & 255,
                                         Y = S[_ + 2] & 255,
                                         I = D >> 2,
-                                        U = (D & 3) << 4 | X >> 4,
+                                        j = (D & 3) << 4 | X >> 4,
                                         G = _ + 1 < N ? (X & 15) << 2 | Y >> 6 : 64,
                                         V = _ + 2 < N ? Y & 63 : 64;
-                                    M += $[I] + $[U] + $[G] + $[V];
+                                    M += $[I] + $[j] + $[G] + $[V];
                                 }
                                 return M;
                             },
                             F = function() {
                                 const S = new Uint8Array([137, 80, 78, 71, 13, 10, 26, 10]),
                                     g = 12,
                                     v = new Int32Array(256);
                                 for (let Y = 0; Y < 256; Y++) {
                                     let I = Y;
-                                    for (let U = 0; U < 8; U++)
+                                    for (let j = 0; j < 8; j++)
                                         I = I & 1 ? 3988292384 ^ I >> 1 & 2147483647 : I >> 1 & 2147483647;
                                     v[Y] = I;
                                 }
 
-                                function $(Y, I, U) {
+                                function $(Y, I, j) {
                                     let G = -1;
-                                    for (let V = I; V < U; V++) {
+                                    for (let V = I; V < j; V++) {
                                         const H = (G ^ Y[V]) & 255,
                                             st = v[H];
                                         G = G >>> 8 ^ st;
                                     }
                                     return G ^ -1;
                                 }
 
-                                function M(Y, I, U, G) {
+                                function M(Y, I, j, G) {
                                     let V = G;
                                     const H = I.length;
-                                    U[V] = H >> 24 & 255, U[V + 1] = H >> 16 & 255, U[V + 2] = H >> 8 & 255, U[V + 3] = H & 255, V += 4, U[V] = Y.charCodeAt(0) & 255, U[V + 1] = Y.charCodeAt(1) & 255, U[V + 2] = Y.charCodeAt(2) & 255, U[V + 3] = Y.charCodeAt(3) & 255, V += 4, U.set(I, V), V += I.length;
-                                    const st = $(U, G + 4, V);
-                                    U[V] = st >> 24 & 255, U[V + 1] = st >> 16 & 255, U[V + 2] = st >> 8 & 255, U[V + 3] = st & 255;
+                                    j[V] = H >> 24 & 255, j[V + 1] = H >> 16 & 255, j[V + 2] = H >> 8 & 255, j[V + 3] = H & 255, V += 4, j[V] = Y.charCodeAt(0) & 255, j[V + 1] = Y.charCodeAt(1) & 255, j[V + 2] = Y.charCodeAt(2) & 255, j[V + 3] = Y.charCodeAt(3) & 255, V += 4, j.set(I, V), V += I.length;
+                                    const st = $(j, G + 4, V);
+                                    j[V] = st >> 24 & 255, j[V + 1] = st >> 16 & 255, j[V + 2] = st >> 8 & 255, j[V + 3] = st & 255;
                                 }
 
-                                function _(Y, I, U) {
+                                function _(Y, I, j) {
                                     let G = 1,
                                         V = 0;
-                                    for (let H = I; H < U; ++H)
+                                    for (let H = I; H < j; ++H)
                                         G = (G + (Y[H] & 255)) % 65521, V = (V + G) % 65521;
                                     return V << 16 | G;
                                 }
 
                                 function N(Y) {
                                     if (!s.isNodeJS)
                                         return D(Y);
                                     try {
                                         const I = parseInt(process.versions.node) >= 8 ? Y : Buffer.from(Y),
-                                            U = require$$5.deflateSync(I, {
+                                            j = require$$5.deflateSync(I, {
                                                 level: 9
                                             });
-                                        return U instanceof Uint8Array ? U : new Uint8Array(U);
+                                        return j instanceof Uint8Array ? j : new Uint8Array(j);
                                     } catch (I) {
                                         (0, s.warn)("Not compressing PNG because zlib.deflateSync is unavailable: " + I);
                                     }
                                     return D(Y);
                                 }
 
                                 function D(Y) {
                                     let I = Y.length;
-                                    const U = 65535,
-                                        G = Math.ceil(I / U),
+                                    const j = 65535,
+                                        G = Math.ceil(I / j),
                                         V = new Uint8Array(2 + I + G * 5 + 4);
                                     let H = 0;
                                     V[H++] = 120, V[H++] = 156;
                                     let st = 0;
-                                    for (; I > U;)
-                                        V[H++] = 0, V[H++] = 255, V[H++] = 255, V[H++] = 0, V[H++] = 0, V.set(Y.subarray(st, st + U), H), H += U, st += U, I -= U;
+                                    for (; I > j;)
+                                        V[H++] = 0, V[H++] = 255, V[H++] = 255, V[H++] = 0, V[H++] = 0, V.set(Y.subarray(st, st + j), H), H += j, st += j, I -= j;
                                     V[H++] = 1, V[H++] = I & 255, V[H++] = I >> 8 & 255, V[H++] = ~I & 65535 & 255, V[H++] = (~I & 65535) >> 8 & 255, V.set(Y.subarray(st), H), H += Y.length - st;
                                     const dt = _(Y, 0, Y.length);
                                     return V[H++] = dt >> 24 & 255, V[H++] = dt >> 16 & 255, V[H++] = dt >> 8 & 255, V[H++] = dt & 255, V;
                                 }
 
-                                function X(Y, I, U, G) {
+                                function X(Y, I, j, G) {
                                     const V = Y.width,
                                         H = Y.height;
                                     let st, dt, yt;
                                     const gt = Y.data;
                                     switch (I) {
                                         case s.ImageKind.GRAYSCALE_1BPP:
                                             dt = 0, st = 1, yt = V + 7 >> 3;
@@ -12995,19 +12995,19 @@
                                         }
                                     }
                                     const d = new Uint8Array([V >> 24 & 255, V >> 16 & 255, V >> 8 & 255, V & 255, H >> 24 & 255, H >> 16 & 255, H >> 8 & 255, H & 255, st, dt, 0, 0, 0]),
                                         b = N(k),
                                         y = S.length + g * 3 + d.length + b.length,
                                         O = new Uint8Array(y);
                                     let B = 0;
-                                    return O.set(S, B), B += S.length, M("IHDR", d, O, B), B += g + d.length, M("IDATA", b, O, B), B += g + b.length, M("IEND", new Uint8Array(0), O, B), o(O, "image/png", U);
+                                    return O.set(S, B), B += S.length, M("IHDR", d, O, B), B += g + d.length, M("IDATA", b, O, B), B += g + b.length, M("IEND", new Uint8Array(0), O, B), o(O, "image/png", j);
                                 }
-                                return function(I, U, G) {
+                                return function(I, j, G) {
                                     const V = I.kind === void 0 ? s.ImageKind.GRAYSCALE_1BPP : I.kind;
-                                    return X(I, V, U, G);
+                                    return X(I, V, j, G);
                                 };
                             }();
                         class R {
                             constructor() {
                                 this.fontSizeScale = 1, this.fontWeight = p.fontWeight, this.fontSize = 0, this.textMatrix = s.IDENTITY_MATRIX, this.fontMatrix = s.FONT_IDENTITY_MATRIX, this.leading = 0, this.textRenderingMode = s.TextRenderingMode.FILL, this.textMatrixScale = 1, this.x = 0, this.y = 0, this.lineX = 0, this.lineY = 0, this.charSpacing = 0, this.wordSpacing = 0, this.textHScale = 1, this.textRise = 0, this.fillColor = p.fillColor, this.strokeColor = "#000000", this.fillAlpha = 1, this.strokeAlpha = 1, this.lineWidth = 1, this.lineJoin = "", this.lineCap = "", this.miterLimit = 0, this.dashArray = [], this.dashPhase = 0, this.dependencies = [], this.activeClipUrl = null, this.clipGroup = null, this.maskId = "";
                             }
                             clone() {
@@ -13311,24 +13311,24 @@
                                     return;
                                 const _ = v.fontSizeScale,
                                     N = v.charSpacing,
                                     D = v.wordSpacing,
                                     X = v.fontDirection,
                                     Y = v.textHScale * X,
                                     I = $.vertical,
-                                    U = I ? 1 : -1,
+                                    j = I ? 1 : -1,
                                     G = $.defaultVMetrics,
                                     V = M * v.fontMatrix[0];
                                 let H = 0;
                                 for (const yt of g) {
                                     if (yt === null) {
                                         H += X * D;
                                         continue;
                                     } else if (typeof yt == "number") {
-                                        H += U * yt * M / 1e3;
+                                        H += j * yt * M / 1e3;
                                         continue;
                                     }
                                     const gt = (yt.isSpace ? D : 0) + N,
                                         k = yt.fontChar;
                                     let l, u, d = yt.width;
                                     if (I) {
                                         let y;
@@ -13420,28 +13420,28 @@
                             _makeTilingPattern(g) {
                                 const v = g[1],
                                     $ = g[2],
                                     M = g[3] || s.IDENTITY_MATRIX,
                                     [_, N, D, X] = g[4],
                                     Y = g[5],
                                     I = g[6],
-                                    U = g[7],
+                                    j = g[7],
                                     G = `shading${x++}`,
                                     [V, H, st, dt] = s.Util.normalizeRect([...s.Util.applyTransform([_, N], M), ...s.Util.applyTransform([D, X], M)]),
                                     [yt, gt] = s.Util.singularValueDecompose2dScale(M),
                                     k = Y * yt,
                                     l = I * gt,
                                     u = this.svgFactory.createElement("svg:pattern");
                                 u.setAttributeNS(null, "id", G), u.setAttributeNS(null, "patternUnits", "userSpaceOnUse"), u.setAttributeNS(null, "width", k), u.setAttributeNS(null, "height", l), u.setAttributeNS(null, "x", `${V}`), u.setAttributeNS(null, "y", `${H}`);
                                 const d = this.svg,
                                     b = this.transformMatrix,
                                     y = this.current.fillColor,
                                     O = this.current.strokeColor,
                                     B = this.svgFactory.create(st - V, dt - H);
-                                if (this.svg = B, this.transformMatrix = M, U === 2) {
+                                if (this.svg = B, this.transformMatrix = M, j === 2) {
                                     const z = s.Util.makeHexColor(...v);
                                     this.current.fillColor = z, this.current.strokeColor = z;
                                 }
                                 return this.executeOpTree(this.convertOpList($)), this.svg = d, this.transformMatrix = b, this.current.fillColor = y, this.current.strokeColor = O, u.append(B.childNodes[0]), this.defs.append(u), `url(#${G})`;
                             }
                             _makeShadingPattern(g) {
                                 switch (typeof g == "string" && (g = this.objs.get(g)), g[0]) {
@@ -13489,17 +13489,17 @@
                                     D = 0;
                                 for (const X of g)
                                     switch (X | 0) {
                                         case s.OPS.rectangle:
                                             M = v[D++], _ = v[D++];
                                             const Y = v[D++],
                                                 I = v[D++],
-                                                U = M + Y,
+                                                j = M + Y,
                                                 G = _ + I;
-                                            N.push("M", T(M), T(_), "L", T(U), T(_), "L", T(U), T(G), "L", T(M), T(G), "Z");
+                                            N.push("M", T(M), T(_), "L", T(j), T(_), "L", T(j), T(G), "L", T(M), T(G), "Z");
                                             break;
                                         case s.OPS.moveTo:
                                             M = v[D++], _ = v[D++], N.push("M", T(M), T(_));
                                             break;
                                         case s.OPS.lineTo:
                                             M = v[D++], _ = v[D++], N.push("L", T(M), T(_));
                                             break;
@@ -13820,23 +13820,23 @@
                             const _ = Math.hypot(v[2], v[3]),
                                 N = _ * o(M.fontFamily, C._isOffscreenCanvasSupported);
                             let D, X;
                             $ === 0 ? (D = v[4], X = v[5] - N) : (D = v[4] + N * Math.sin($), X = v[5] - N * Math.cos($));
                             const Y = "calc(var(--scale-factor)*",
                                 I = S.style;
                             C._container === C._rootContainer ? (I.left = `${(100 * D / C._pageWidth).toFixed(2)}%`, I.top = `${(100 * X / C._pageHeight).toFixed(2)}%`) : (I.left = `${Y}${D.toFixed(2)}px)`, I.top = `${Y}${X.toFixed(2)}px)`), I.fontSize = `${Y}${_.toFixed(2)}px)`, I.fontFamily = M.fontFamily, g.fontSize = _, S.setAttribute("role", "presentation"), S.textContent = x.str, S.dir = x.dir, C._fontInspectorEnabled && (S.dataset.fontName = x.fontName), $ !== 0 && (g.angle = $ * (180 / Math.PI));
-                            let U = !1;
+                            let j = !1;
                             if (x.str.length > 1)
-                                U = !0;
+                                j = !0;
                             else if (x.str !== " " && x.transform[0] !== x.transform[3]) {
                                 const G = Math.abs(x.transform[0]),
                                     V = Math.abs(x.transform[3]);
-                                G !== V && Math.max(G, V) / Math.min(G, V) > 1.5 && (U = !0);
+                                G !== V && Math.max(G, V) / Math.min(G, V) > 1.5 && (j = !0);
                             }
-                            U && (g.canvasWidth = M.vertical ? x.height : x.width), C._textDivProperties.set(S, g), C._isReadableStream && C._layoutText(S);
+                            j && (g.canvasWidth = M.vertical ? x.height : x.width), C._textDivProperties.set(S, g), C._isReadableStream && C._layoutText(S);
                         }
 
                         function R(C) {
                             const {
                                 div: x,
                                 scale: E,
                                 properties: S,
@@ -14013,15 +14013,15 @@
                             p = n(28),
                             f = n(33),
                             A = n(6),
                             a = n(34);
                         const X = class X {
                             constructor({
                                 uiManager: I,
-                                pageIndex: U,
+                                pageIndex: j,
                                 div: G,
                                 accessibilityManager: V,
                                 annotationLayer: H,
                                 viewport: st,
                                 l10n: dt
                             }) {
                                 W(this, S);
@@ -14040,15 +14040,15 @@
                                 W(this, E, void 0);
                                 const yt = [p.FreeTextEditor, f.InkEditor, a.StampEditor];
                                 if (!X._initialized) {
                                     X._initialized = !0;
                                     for (const gt of yt)
                                         gt.initialize(dt);
                                 }
-                                I.registerEditorTypes(yt), ot(this, E, I), this.pageIndex = U, this.div = G, ot(this, o, V), ot(this, R, H), this.viewport = st, r(this, E).addLayer(this);
+                                I.registerEditorTypes(yt), ot(this, E, I), this.pageIndex = j, this.div = G, ot(this, o, V), ot(this, R, H), this.viewport = st, r(this, E).addLayer(this);
                             }
                             get isEmpty() {
                                 return r(this, P).size === 0;
                             }
                             updateToolbar(I) {
                                 r(this, E).updateToolbar(I);
                             }
@@ -14079,129 +14079,129 @@
                             enable() {
                                 this.div.style.pointerEvents = "auto";
                                 const I = /* @__PURE__ */ new Set();
                                 for (const G of r(this, P).values())
                                     G.enableEditing(), G.annotationElementId && I.add(G.annotationElementId);
                                 if (!r(this, R))
                                     return;
-                                const U = r(this, R).getEditableAnnotations();
-                                for (const G of U) {
+                                const j = r(this, R).getEditableAnnotations();
+                                for (const G of j) {
                                     if (G.hide(), r(this, E).isDeletedAnnotationElement(G.data.id) || I.has(G.data.id))
                                         continue;
                                     const V = this.deserialize(G);
                                     V && (this.addOrRebuild(V), V.enableEditing());
                                 }
                             }
                             disable() {
-                                var U;
+                                var j;
                                 ot(this, x, !0), this.div.style.pointerEvents = "none";
                                 const I = /* @__PURE__ */ new Set();
                                 for (const G of r(this, P).values()) {
                                     if (G.disableEditing(), !G.annotationElementId || G.serialize() !== null) {
                                         I.add(G.annotationElementId);
                                         continue;
                                     }
-                                    (U = this.getEditableAnnotation(G.annotationElementId)) == null || U.show(), G.remove();
+                                    (j = this.getEditableAnnotation(G.annotationElementId)) == null || j.show(), G.remove();
                                 }
                                 if (r(this, R)) {
                                     const G = r(this, R).getEditableAnnotations();
                                     for (const V of G) {
                                         const {
                                             id: H
                                         } = V.data;
                                         I.has(H) || r(this, E).isDeletedAnnotationElement(H) || V.show();
                                     }
                                 }
                                 J(this, N, sn).call(this), this.isEmpty && (this.div.hidden = !0), ot(this, x, !1);
                             }
                             getEditableAnnotation(I) {
-                                var U;
-                                return ((U = r(this, R)) == null ? void 0 : U.getEditableAnnotation(I)) || null;
+                                var j;
+                                return ((j = r(this, R)) == null ? void 0 : j.getEditableAnnotation(I)) || null;
                             }
                             setActiveEditor(I) {
                                 r(this, E).getActive() !== I && r(this, E).setActiveEditor(I);
                             }
                             enableClick() {
                                 this.div.addEventListener("pointerdown", r(this, T)), this.div.addEventListener("pointerup", r(this, w));
                             }
                             disableClick() {
                                 this.div.removeEventListener("pointerdown", r(this, T)), this.div.removeEventListener("pointerup", r(this, w));
                             }
                             attach(I) {
                                 r(this, P).set(I.id, I);
                                 const {
-                                    annotationElementId: U
+                                    annotationElementId: j
                                 } = I;
-                                U && r(this, E).isDeletedAnnotationElement(U) && r(this, E).removeDeletedAnnotationElement(I);
+                                j && r(this, E).isDeletedAnnotationElement(j) && r(this, E).removeDeletedAnnotationElement(I);
                             }
                             detach(I) {
-                                var U;
-                                r(this, P).delete(I.id), (U = r(this, o)) == null || U.removePointerInTextLayer(I.contentDiv), !r(this, x) && I.annotationElementId && r(this, E).addDeletedAnnotationElement(I);
+                                var j;
+                                r(this, P).delete(I.id), (j = r(this, o)) == null || j.removePointerInTextLayer(I.contentDiv), !r(this, x) && I.annotationElementId && r(this, E).addDeletedAnnotationElement(I);
                             }
                             remove(I) {
                                 this.detach(I), r(this, E).removeEditor(I), I.div.contains(document.activeElement) && setTimeout(() => {
                                     r(this, E).focusMainContainer();
                                 }, 0), I.div.remove(), I.isAttachedToDOM = !1, r(this, C) || this.addInkEditorIfNeeded(!1);
                             }
                             changeParent(I) {
-                                var U;
-                                I.parent !== this && (I.annotationElementId && (r(this, E).addDeletedAnnotationElement(I.annotationElementId), s.AnnotationEditor.deleteAnnotationElement(I), I.annotationElementId = null), this.attach(I), (U = I.parent) == null || U.detach(I), I.setParent(this), I.div && I.isAttachedToDOM && (I.div.remove(), this.div.append(I.div)));
+                                var j;
+                                I.parent !== this && (I.annotationElementId && (r(this, E).addDeletedAnnotationElement(I.annotationElementId), s.AnnotationEditor.deleteAnnotationElement(I), I.annotationElementId = null), this.attach(I), (j = I.parent) == null || j.detach(I), I.setParent(this), I.div && I.isAttachedToDOM && (I.div.remove(), this.div.append(I.div)));
                             }
                             add(I) {
                                 if (this.changeParent(I), r(this, E).addEditor(I), this.attach(I), !I.isAttachedToDOM) {
-                                    const U = I.render();
-                                    this.div.append(U), I.isAttachedToDOM = !0;
+                                    const j = I.render();
+                                    this.div.append(j), I.isAttachedToDOM = !0;
                                 }
                                 I.fixAndSetPosition(), I.onceAdded(), r(this, E).addToAnnotationStorage(I);
                             }
                             moveEditorInDOM(I) {
                                 var G;
                                 if (!I.isAttachedToDOM)
                                     return;
                                 const {
-                                    activeElement: U
+                                    activeElement: j
                                 } = document;
-                                I.div.contains(U) && (I._focusEventsAllowed = !1, setTimeout(() => {
+                                I.div.contains(j) && (I._focusEventsAllowed = !1, setTimeout(() => {
                                     I.div.contains(document.activeElement) ? I._focusEventsAllowed = !0 : (I.div.addEventListener("focusin", () => {
                                         I._focusEventsAllowed = !0;
                                     }, {
                                         once: !0
-                                    }), U.focus());
+                                    }), j.focus());
                                 }, 0)), I._structTreeParentId = (G = r(this, o)) == null ? void 0 : G.moveElementInDOM(this.div, I.div, I.contentDiv, !0);
                             }
                             addOrRebuild(I) {
                                 I.needsToBeRebuilt() ? I.rebuild() : this.add(I);
                             }
                             addUndoableEditor(I) {
-                                const U = () => I._uiManager.rebuild(I),
+                                const j = () => I._uiManager.rebuild(I),
                                     G = () => {
                                         I.remove();
                                     };
                                 this.addCommands({
-                                    cmd: U,
+                                    cmd: j,
                                     undo: G,
                                     mustExec: !1
                                 });
                             }
                             getNextId() {
                                 return r(this, E).getId();
                             }
-                            pasteEditor(I, U) {
+                            pasteEditor(I, j) {
                                 r(this, E).updateToolbar(I), r(this, E).updateMode(I);
                                 const {
                                     offsetX: G,
                                     offsetY: V
                                 } = J(this, M, nn).call(this), H = this.getNextId(), st = J(this, S, en).call(this, {
                                     parent: this,
                                     id: H,
                                     x: G,
                                     y: V,
                                     uiManager: r(this, E),
                                     isCentered: !0,
-                                    ...U
+                                    ...j
                                 });
                                 st && this.add(st);
                             }
                             deserialize(I) {
                                 switch (I.annotationType ?? I.annotationEditorType) {
                                     case e.AnnotationEditorType.FREETEXT:
                                         return p.FreeTextEditor.deserialize(I, this, r(this, E));
@@ -14225,17 +14225,17 @@
                                 return r(this, E).isSelected(I);
                             }
                             unselect(I) {
                                 r(this, E).unselect(I);
                             }
                             pointerup(I) {
                                 const {
-                                    isMac: U
+                                    isMac: j
                                 } = e.FeatureTest.platform;
-                                if (!(I.button !== 0 || I.ctrlKey && U) && I.target === this.div && r(this, m)) {
+                                if (!(I.button !== 0 || I.ctrlKey && j) && I.target === this.div && r(this, m)) {
                                     if (ot(this, m, !1), !r(this, F)) {
                                         ot(this, F, !0);
                                         return;
                                     }
                                     if (r(this, E).getMode() === e.AnnotationEditorType.STAMP) {
                                         r(this, E).unselectAll();
                                         return;
@@ -14245,84 +14245,84 @@
                             }
                             pointerdown(I) {
                                 if (r(this, m)) {
                                     ot(this, m, !1);
                                     return;
                                 }
                                 const {
-                                    isMac: U
+                                    isMac: j
                                 } = e.FeatureTest.platform;
-                                if (I.button !== 0 || I.ctrlKey && U || I.target !== this.div)
+                                if (I.button !== 0 || I.ctrlKey && j || I.target !== this.div)
                                     return;
                                 ot(this, m, !0);
                                 const G = r(this, E).getActive();
                                 ot(this, F, !G || G.isEmpty());
                             }
-                            findNewParent(I, U, G) {
-                                const V = r(this, E).findParent(U, G);
+                            findNewParent(I, j, G) {
+                                const V = r(this, E).findParent(j, G);
                                 return V === null || V === this ? !1 : (V.changeParent(I), !0);
                             }
                             destroy() {
-                                var I, U;
+                                var I, j;
                                 ((I = r(this, E).getActive()) == null ? void 0 : I.parent) === this && (r(this, E).commitOrRemove(), r(this, E).setActiveEditor(null));
                                 for (const G of r(this, P).values())
-                                    (U = r(this, o)) == null || U.removePointerInTextLayer(G.contentDiv), G.setParent(null), G.isAttachedToDOM = !1, G.div.remove();
+                                    (j = r(this, o)) == null || j.removePointerInTextLayer(G.contentDiv), G.setParent(null), G.isAttachedToDOM = !1, G.div.remove();
                                 this.div = null, r(this, P).clear(), r(this, E).removeLayer(this);
                             }
                             render({
                                 viewport: I
                             }) {
                                 this.viewport = I, (0, A.setLayerDimensions)(this.div, I);
-                                for (const U of r(this, E).getEditors(this.pageIndex))
-                                    this.add(U);
+                                for (const j of r(this, E).getEditors(this.pageIndex))
+                                    this.add(j);
                                 this.updateMode();
                             }
                             update({
                                 viewport: I
                             }) {
                                 r(this, E).commitOrRemove(), this.viewport = I, (0, A.setLayerDimensions)(this.div, {
                                     rotation: I.rotation
                                 }), this.updateMode();
                             }
                             get pageDimensions() {
                                 const {
                                     pageWidth: I,
-                                    pageHeight: U
+                                    pageHeight: j
                                 } = this.viewport.rawDims;
-                                return [I, U];
+                                return [I, j];
                             }
                         };
                         o = new WeakMap(), F = new WeakMap(), R = new WeakMap(), w = new WeakMap(), T = new WeakMap(), P = new WeakMap(), m = new WeakMap(), C = new WeakMap(), x = new WeakMap(), E = new WeakMap(), S = new WeakSet(), en = function(I) {
                             switch (r(this, E).getMode()) {
                                 case e.AnnotationEditorType.FREETEXT:
                                     return new p.FreeTextEditor(I);
                                 case e.AnnotationEditorType.INK:
                                     return new f.InkEditor(I);
                                 case e.AnnotationEditorType.STAMP:
                                     return new a.StampEditor(I);
                             }
                             return null;
-                        }, v = new WeakSet(), Fe = function(I, U) {
+                        }, v = new WeakSet(), Fe = function(I, j) {
                             const G = this.getNextId(),
                                 V = J(this, S, en).call(this, {
                                     parent: this,
                                     id: G,
                                     x: I.offsetX,
                                     y: I.offsetY,
                                     uiManager: r(this, E),
-                                    isCentered: U
+                                    isCentered: j
                                 });
                             return V && this.add(V), V;
                         }, M = new WeakSet(), nn = function() {
                             const {
                                 x: I,
-                                y: U,
+                                y: j,
                                 width: G,
                                 height: V
-                            } = this.div.getBoundingClientRect(), H = Math.max(0, I), st = Math.max(0, U), dt = Math.min(window.innerWidth, I + G), yt = Math.min(window.innerHeight, U + V), gt = (H + dt) / 2 - I, k = (st + yt) / 2 - U, [l, u] = this.viewport.rotation % 180 === 0 ? [gt, k] : [k, gt];
+                            } = this.div.getBoundingClientRect(), H = Math.max(0, I), st = Math.max(0, j), dt = Math.min(window.innerWidth, I + G), yt = Math.min(window.innerHeight, j + V), gt = (H + dt) / 2 - I, k = (st + yt) / 2 - j, [l, u] = this.viewport.rotation % 180 === 0 ? [gt, k] : [k, gt];
                             return {
                                 offsetX: l,
                                 offsetY: u
                             };
                         }, N = new WeakSet(), sn = function() {
                             ot(this, C, !0);
                             for (const I of r(this, P).values())
@@ -14339,15 +14339,15 @@
                         Object.defineProperty(t, "__esModule", {
                             value: !0
                         }), t.FreeTextEditor = void 0;
                         var e = n(1),
                             s = n(5),
                             p = n(4),
                             f = n(29);
-                        const U = class U extends p.AnnotationEditor {
+                        const j = class j extends p.AnnotationEditor {
                             constructor(H) {
                                 super({
                                     ...H,
                                     name: "freeTextEditor"
                                 });
                                 W(this, C);
                                 W(this, E);
@@ -14361,18 +14361,18 @@
                                 W(this, o, this.editorDivInput.bind(this));
                                 W(this, F, this.editorDivKeydown.bind(this));
                                 W(this, R, void 0);
                                 W(this, w, "");
                                 W(this, T, `${this.id}-editor`);
                                 W(this, P, void 0);
                                 W(this, m, null);
-                                ot(this, R, H.color || U._defaultColor || p.AnnotationEditor._defaultLineColor), ot(this, P, H.fontSize || U._defaultFontSize);
+                                ot(this, R, H.color || j._defaultColor || p.AnnotationEditor._defaultLineColor), ot(this, P, H.fontSize || j._defaultFontSize);
                             }
                             static get _keyboardManager() {
-                                const H = U.prototype,
+                                const H = j.prototype,
                                     st = (gt) => gt.isEmpty(),
                                     dt = s.AnnotationEditorUIManager.TRANSLATE_SMALL,
                                     yt = s.AnnotationEditorUIManager.TRANSLATE_BIG;
                                 return (0, e.shadow)(this, "_keyboardManager", new s.KeyboardManager([
                                     [
                                         ["ctrl+s", "mac+meta+s", "ctrl+p", "mac+meta+p"], H.commitOrRemove, {
                                             bubbles: !0
@@ -14437,18 +14437,18 @@
                                 });
                                 const st = getComputedStyle(document.documentElement);
                                 this._internalPadding = parseFloat(st.getPropertyValue("--freetext-padding"));
                             }
                             static updateDefaultParams(H, st) {
                                 switch (H) {
                                     case e.AnnotationEditorParamsType.FREETEXT_SIZE:
-                                        U._defaultFontSize = st;
+                                        j._defaultFontSize = st;
                                         break;
                                     case e.AnnotationEditorParamsType.FREETEXT_COLOR:
-                                        U._defaultColor = st;
+                                        j._defaultColor = st;
                                         break;
                                 }
                             }
                             updateParams(H, st) {
                                 switch (H) {
                                     case e.AnnotationEditorParamsType.FREETEXT_SIZE:
                                         J(this, C, xn).call(this, st);
@@ -14456,30 +14456,30 @@
                                     case e.AnnotationEditorParamsType.FREETEXT_COLOR:
                                         J(this, E, Dn).call(this, st);
                                         break;
                                 }
                             }
                             static get defaultPropertiesToUpdate() {
                                 return [
-                                    [e.AnnotationEditorParamsType.FREETEXT_SIZE, U._defaultFontSize],
-                                    [e.AnnotationEditorParamsType.FREETEXT_COLOR, U._defaultColor || p.AnnotationEditor._defaultLineColor]
+                                    [e.AnnotationEditorParamsType.FREETEXT_SIZE, j._defaultFontSize],
+                                    [e.AnnotationEditorParamsType.FREETEXT_COLOR, j._defaultColor || p.AnnotationEditor._defaultLineColor]
                                 ];
                             }
                             get propertiesToUpdate() {
                                 return [
                                     [e.AnnotationEditorParamsType.FREETEXT_SIZE, r(this, P)],
                                     [e.AnnotationEditorParamsType.FREETEXT_COLOR, r(this, R)]
                                 ];
                             }
                             _translateEmpty(H, st) {
                                 this._uiManager.translateSelectedEditors(H, st, !0);
                             }
                             getInitialTranslation() {
                                 const H = this.parentScale;
-                                return [-U._internalPadding * H, -(U._internalPadding + r(this, P)) * H];
+                                return [-j._internalPadding * H, -(j._internalPadding + r(this, P)) * H];
                             }
                             rebuild() {
                                 this.parent && (super.rebuild(), this.div !== null && (this.isAttachedToDOM || this.parent.add(this)));
                             }
                             enableEditMode() {
                                 this.isInEditMode() || (this.parent.setEditingState(!1), this.parent.updateToolbar(e.AnnotationEditorType.FREETEXT), super.enableEditMode(), this.overlayDiv.classList.remove("enabled"), this.editorDiv.contentEditable = !0, this._isDraggable = !1, this.div.removeAttribute("aria-activedescendant"), this.editorDiv.addEventListener("keydown", r(this, F)), this.editorDiv.addEventListener("focus", r(this, h)), this.editorDiv.addEventListener("blur", r(this, a)), this.editorDiv.addEventListener("input", r(this, o)));
                             }
@@ -14539,15 +14539,15 @@
                             dblclick(H) {
                                 this.enterInEditMode();
                             }
                             keydown(H) {
                                 H.target === this.div && H.key === "Enter" && (this.enterInEditMode(), H.preventDefault());
                             }
                             editorDivKeydown(H) {
-                                U._keyboardManager.exec(this, H);
+                                j._keyboardManager.exec(this, H);
                             }
                             editorDivFocus(H) {
                                 this.isEditing = !0;
                             }
                             editorDivBlur(H) {
                                 this.isEditing = !1;
                             }
@@ -14654,15 +14654,15 @@
                                     return null;
                                 if (this.deleted)
                                     return {
                                         pageIndex: this.pageIndex,
                                         id: this.annotationElementId,
                                         deleted: !0
                                     };
-                                const st = U._internalPadding * this.parentScale,
+                                const st = j._internalPadding * this.parentScale,
                                     dt = this.getRect(st, st),
                                     yt = p.AnnotationEditor._colorManager.convert(this.isAttachedToDOM ? getComputedStyle(this.editorDiv).color : r(this, R)),
                                     gt = {
                                         annotationType: e.AnnotationEditorType.FREETEXT,
                                         color: yt,
                                         fontSize: r(this, P),
                                         value: r(this, w),
@@ -14746,18 +14746,18 @@
                         }, Y = new WeakSet(), an = function(H = !1) {
                             if (!this.annotationElementId)
                                 return;
                             if (J(this, $, Ae).call(this), !H && (this.width === 0 || this.height === 0)) {
                                 setTimeout(() => J(this, Y, an).call(this, !0), 0);
                                 return;
                             }
-                            const st = U._internalPadding * this.parentScale;
+                            const st = j._internalPadding * this.parentScale;
                             r(this, m).rect = this.getRect(st, st);
-                        }, ee(U, "_freeTextDefaultContent", ""), ee(U, "_internalPadding", 0), ee(U, "_defaultColor", null), ee(U, "_defaultFontSize", 10), ee(U, "_type", "freetext");
-                        let A = U;
+                        }, ee(j, "_freeTextDefaultContent", ""), ee(j, "_internalPadding", 0), ee(j, "_defaultColor", null), ee(j, "_defaultFontSize", 10), ee(j, "_type", "freetext");
+                        let A = j;
                         t.FreeTextEditor = A;
                     },
                     /* 29 */
                     /***/
                     (i, t, n) => {
                         var u, b, ce, O, On, z, it, Z, lt, ht, mt, ft, kt, Rt, St, It, _t, rt, at, pt, Ct, Tt, Bt, $n, jt, Me, Gt, on, Vt, ln, nt, Q, At, wt, te, Qt, et, cn, Ot, Pt, $t, Nt, Nn, vt, hn;
                         Object.defineProperty(t, "__esModule", {
@@ -14776,87 +14776,87 @@
                         function R(Lt) {
                             return {
                                 width: Lt[2] - Lt[0],
                                 height: Lt[3] - Lt[1]
                             };
                         }
                         class w {
-                            static create(j) {
-                                switch (j.data.annotationType) {
+                            static create(U) {
+                                switch (U.data.annotationType) {
                                     case e.AnnotationType.LINK:
-                                        return new P(j);
+                                        return new P(U);
                                     case e.AnnotationType.TEXT:
-                                        return new m(j);
+                                        return new m(U);
                                     case e.AnnotationType.WIDGET:
-                                        switch (j.data.fieldType) {
+                                        switch (U.data.fieldType) {
                                             case "Tx":
-                                                return new x(j);
+                                                return new x(U);
                                             case "Btn":
-                                                return j.data.radioButton ? new g(j) : j.data.checkBox ? new S(j) : new v(j);
+                                                return U.data.radioButton ? new g(U) : U.data.checkBox ? new S(U) : new v(U);
                                             case "Ch":
-                                                return new $(j);
+                                                return new $(U);
                                             case "Sig":
-                                                return new E(j);
+                                                return new E(U);
                                         }
-                                        return new C(j);
+                                        return new C(U);
                                     case e.AnnotationType.POPUP:
-                                        return new M(j);
+                                        return new M(U);
                                     case e.AnnotationType.FREETEXT:
-                                        return new N(j);
+                                        return new N(U);
                                     case e.AnnotationType.LINE:
-                                        return new D(j);
+                                        return new D(U);
                                     case e.AnnotationType.SQUARE:
-                                        return new X(j);
+                                        return new X(U);
                                     case e.AnnotationType.CIRCLE:
-                                        return new Y(j);
+                                        return new Y(U);
                                     case e.AnnotationType.POLYLINE:
-                                        return new I(j);
+                                        return new I(U);
                                     case e.AnnotationType.CARET:
-                                        return new G(j);
+                                        return new G(U);
                                     case e.AnnotationType.INK:
-                                        return new V(j);
+                                        return new V(U);
                                     case e.AnnotationType.POLYGON:
-                                        return new U(j);
+                                        return new j(U);
                                     case e.AnnotationType.HIGHLIGHT:
-                                        return new H(j);
+                                        return new H(U);
                                     case e.AnnotationType.UNDERLINE:
-                                        return new st(j);
+                                        return new st(U);
                                     case e.AnnotationType.SQUIGGLY:
-                                        return new dt(j);
+                                        return new dt(U);
                                     case e.AnnotationType.STRIKEOUT:
-                                        return new yt(j);
+                                        return new yt(U);
                                     case e.AnnotationType.STAMP:
-                                        return new gt(j);
+                                        return new gt(U);
                                     case e.AnnotationType.FILEATTACHMENT:
-                                        return new k(j);
+                                        return new k(U);
                                     default:
-                                        return new T(j);
+                                        return new T(U);
                                 }
                             }
                         }
                         const d = class d {
-                            constructor(j, {
+                            constructor(U, {
                                 isRenderable: c = !1,
                                 ignoreBorder: L = !1,
                                 createQuadrilaterals: q = !1
                             } = {}) {
                                 W(this, u, !1);
-                                this.isRenderable = c, this.data = j.data, this.layer = j.layer, this.linkService = j.linkService, this.downloadManager = j.downloadManager, this.imageResourcesPath = j.imageResourcesPath, this.renderForms = j.renderForms, this.svgFactory = j.svgFactory, this.annotationStorage = j.annotationStorage, this.enableScripting = j.enableScripting, this.hasJSActions = j.hasJSActions, this._fieldObjects = j.fieldObjects, this.parent = j.parent, c && (this.container = this._createContainer(L)), q && this._createQuadrilaterals();
+                                this.isRenderable = c, this.data = U.data, this.layer = U.layer, this.linkService = U.linkService, this.downloadManager = U.downloadManager, this.imageResourcesPath = U.imageResourcesPath, this.renderForms = U.renderForms, this.svgFactory = U.svgFactory, this.annotationStorage = U.annotationStorage, this.enableScripting = U.enableScripting, this.hasJSActions = U.hasJSActions, this._fieldObjects = U.fieldObjects, this.parent = U.parent, c && (this.container = this._createContainer(L)), q && this._createQuadrilaterals();
                             }
                             static _hasPopupData({
-                                titleObj: j,
+                                titleObj: U,
                                 contentsObj: c,
                                 richText: L
                             }) {
-                                return !!(j != null && j.str || c != null && c.str || L != null && L.str);
+                                return !!(U != null && U.str || c != null && c.str || L != null && L.str);
                             }
                             get hasPopupData() {
                                 return d._hasPopupData(this.data);
                             }
-                            _createContainer(j) {
+                            _createContainer(U) {
                                 const {
                                     data: c,
                                     parent: {
                                         page: L,
                                         viewport: q
                                     }
                                 } = this, K = document.createElement("section");
@@ -14873,15 +14873,15 @@
                                     } = c;
                                     return !c.hasOwnCanvas && Ut !== 0 && this.setRotation(Ut, K), K;
                                 }
                                 const {
                                     width: Ft,
                                     height: Ht
                                 } = R(c.rect), xt = e.Util.normalizeRect([c.rect[0], L.view[3] - c.rect[1] + L.view[1], c.rect[2], L.view[3] - c.rect[3] + L.view[1]]);
-                                if (!j && c.borderStyle.width > 0) {
+                                if (!U && c.borderStyle.width > 0) {
                                     K.style.borderWidth = `${c.borderStyle.width}px`;
                                     const Ut = c.borderStyle.horizontalCornerRadius,
                                         Xt = c.borderStyle.verticalCornerRadius;
                                     if (Ut > 0 || Xt > 0) {
                                         const Zt = `calc(${Ut}px * var(--scale-factor)) / calc(${Xt}px * var(--scale-factor))`;
                                         K.style.borderRadius = Zt;
                                     } else if (this instanceof g) {
@@ -14910,29 +14910,29 @@
                                 }
                                 K.style.left = `${100 * (xt[0] - bt) / tt}%`, K.style.top = `${100 * (xt[1] - Mt) / ct}%`;
                                 const {
                                     rotation: Dt
                                 } = c;
                                 return c.hasOwnCanvas || Dt === 0 ? (K.style.width = `${100 * Ft / tt}%`, K.style.height = `${100 * Ht / ct}%`) : this.setRotation(Dt, K), K;
                             }
-                            setRotation(j, c = this.container) {
+                            setRotation(U, c = this.container) {
                                 if (!this.data.rect)
                                     return;
                                 const {
                                     pageWidth: L,
                                     pageHeight: q
                                 } = this.parent.viewport.rawDims, {
                                     width: K,
                                     height: tt
                                 } = R(this.data.rect);
                                 let ct, bt;
-                                j % 180 === 0 ? (ct = 100 * K / L, bt = 100 * tt / q) : (ct = 100 * tt / L, bt = 100 * K / q), c.style.width = `${ct}%`, c.style.height = `${bt}%`, c.setAttribute("data-main-rotation", (360 - j) % 360);
+                                U % 180 === 0 ? (ct = 100 * K / L, bt = 100 * tt / q) : (ct = 100 * tt / L, bt = 100 * K / q), c.style.width = `${ct}%`, c.style.height = `${bt}%`, c.setAttribute("data-main-rotation", (360 - U) % 360);
                             }
                             get _commonActions() {
-                                const j = (c, L, q) => {
+                                const U = (c, L, q) => {
                                     const K = q.detail[c],
                                         tt = K[0],
                                         ct = K.slice(1);
                                     q.target.style[L] = f.ColorConverters[`${tt}_HTML`](ct), this.annotationStorage.setValue(this.data.id, {
                                         [L]: f.ColorConverters[`${tt}_rgb`](ct)
                                     });
                                 };
@@ -14971,83 +14971,83 @@
                                     readonly: (c) => {
                                         c.target.disabled = c.detail.readonly;
                                     },
                                     required: (c) => {
                                         this._setRequired(c.target, c.detail.required);
                                     },
                                     bgColor: (c) => {
-                                        j("bgColor", "backgroundColor", c);
+                                        U("bgColor", "backgroundColor", c);
                                     },
                                     fillColor: (c) => {
-                                        j("fillColor", "backgroundColor", c);
+                                        U("fillColor", "backgroundColor", c);
                                     },
                                     fgColor: (c) => {
-                                        j("fgColor", "color", c);
+                                        U("fgColor", "color", c);
                                     },
                                     textColor: (c) => {
-                                        j("textColor", "color", c);
+                                        U("textColor", "color", c);
                                     },
                                     borderColor: (c) => {
-                                        j("borderColor", "borderColor", c);
+                                        U("borderColor", "borderColor", c);
                                     },
                                     strokeColor: (c) => {
-                                        j("strokeColor", "borderColor", c);
+                                        U("strokeColor", "borderColor", c);
                                     },
                                     rotation: (c) => {
                                         const L = c.detail.rotation;
                                         this.setRotation(L), this.annotationStorage.setValue(this.data.id, {
                                             rotation: L
                                         });
                                     }
                                 });
                             }
-                            _dispatchEventFromSandbox(j, c) {
+                            _dispatchEventFromSandbox(U, c) {
                                 const L = this._commonActions;
                                 for (const q of Object.keys(c.detail)) {
-                                    const K = j[q] || L[q];
+                                    const K = U[q] || L[q];
                                     K == null || K(c);
                                 }
                             }
-                            _setDefaultPropertiesFromJS(j) {
+                            _setDefaultPropertiesFromJS(U) {
                                 if (!this.enableScripting)
                                     return;
                                 const c = this.annotationStorage.getRawValue(this.data.id);
                                 if (!c)
                                     return;
                                 const L = this._commonActions;
                                 for (const [q, K] of Object.entries(c)) {
                                     const tt = L[q];
                                     if (tt) {
                                         const ct = {
                                             detail: {
                                                 [q]: K
                                             },
-                                            target: j
+                                            target: U
                                         };
                                         tt(ct), delete c[q];
                                     }
                                 }
                             }
                             _createQuadrilaterals() {
                                 if (!this.container)
                                     return;
                                 const {
-                                    quadPoints: j
+                                    quadPoints: U
                                 } = this.data;
-                                if (!j)
+                                if (!U)
                                     return;
                                 const [c, L, q, K] = this.data.rect;
-                                if (j.length === 1) {
+                                if (U.length === 1) {
                                     const [, {
                                         x: Xt,
                                         y: Kt
                                     }, {
                                         x: Zt,
                                         y: ie
-                                    }] = j[0];
+                                    }] = U[0];
                                     if (q === Xt && K === Kt && c === Zt && L === ie)
                                         return;
                                 }
                                 const {
                                     style: tt
                                 } = this.container;
                                 let ct;
@@ -15072,30 +15072,30 @@
                                 Dt.setAttribute("id", Ut), Dt.setAttribute("clipPathUnits", "objectBoundingBox"), xt.append(Dt);
                                 for (const [, {
                                         x: Xt,
                                         y: Kt
                                     }, {
                                         x: Zt,
                                         y: ie
-                                    }] of j) {
+                                    }] of U) {
                                     const ne = Ft.createElement("rect"),
                                         se = (Zt - c) / bt,
                                         oe = (K - Kt) / Mt,
                                         le = (Xt - Zt) / bt,
                                         An = (Kt - ie) / Mt;
                                     ne.setAttribute("x", se), ne.setAttribute("y", oe), ne.setAttribute("width", le), ne.setAttribute("height", An), Dt.append(ne), ct == null || ct.push(`<rect vector-effect="non-scaling-stroke" x="${se}" y="${oe}" width="${le}" height="${An}"/>`);
                                 }
                                 r(this, u) && (ct.push("</g></svg>')"), tt.backgroundImage = ct.join("")), this.container.append(Ht), this.container.style.clipPath = `url(#${Ut})`;
                             }
                             _createPopup() {
                                 const {
-                                    container: j,
+                                    container: U,
                                     data: c
                                 } = this;
-                                j.setAttribute("aria-haspopup", "dialog");
+                                U.setAttribute("aria-haspopup", "dialog");
                                 const L = new M({
                                     data: {
                                         color: c.color,
                                         titleObj: c.titleObj,
                                         modificationDate: c.modificationDate,
                                         contentsObj: c.contentsObj,
                                         richText: c.richText,
@@ -15108,18 +15108,18 @@
                                     elements: [this]
                                 });
                                 this.parent.div.append(L.render());
                             }
                             render() {
                                 (0, e.unreachable)("Abstract method `AnnotationElement.render` called");
                             }
-                            _getElementsByName(j, c = null) {
+                            _getElementsByName(U, c = null) {
                                 const L = [];
                                 if (this._fieldObjects) {
-                                    const q = this._fieldObjects[j];
+                                    const q = this._fieldObjects[U];
                                     if (q)
                                         for (const {
                                                 page: K,
                                                 id: tt,
                                                 exportValues: ct
                                             }
                                             of q) {
@@ -15135,57 +15135,57 @@
                                                 id: tt,
                                                 exportValue: bt,
                                                 domElement: Mt
                                             });
                                         }
                                     return L;
                                 }
-                                for (const q of document.getElementsByName(j)) {
+                                for (const q of document.getElementsByName(U)) {
                                     const {
                                         exportValue: K
                                     } = q, tt = q.getAttribute("data-element-id");
                                     tt !== c && F.has(q) && L.push({
                                         id: tt,
                                         exportValue: K,
                                         domElement: q
                                     });
                                 }
                                 return L;
                             }
                             show() {
-                                var j;
-                                this.container && (this.container.hidden = !1), (j = this.popup) == null || j.maybeShow();
+                                var U;
+                                this.container && (this.container.hidden = !1), (U = this.popup) == null || U.maybeShow();
                             }
                             hide() {
-                                var j;
-                                this.container && (this.container.hidden = !0), (j = this.popup) == null || j.forceHide();
+                                var U;
+                                this.container && (this.container.hidden = !0), (U = this.popup) == null || U.forceHide();
                             }
                             getElementsToTriggerPopup() {
                                 return this.container;
                             }
                             addHighlightArea() {
-                                const j = this.getElementsToTriggerPopup();
-                                if (Array.isArray(j))
-                                    for (const c of j)
+                                const U = this.getElementsToTriggerPopup();
+                                if (Array.isArray(U))
+                                    for (const c of U)
                                         c.classList.add("highlightArea");
                                 else
-                                    j.classList.add("highlightArea");
+                                    U.classList.add("highlightArea");
                             }
                             _editOnDoubleClick() {
                                 const {
-                                    annotationEditorType: j,
+                                    annotationEditorType: U,
                                     data: {
                                         id: c
                                     }
                                 } = this;
                                 this.container.addEventListener("dblclick", () => {
                                     var L;
                                     (L = this.linkService.eventBus) == null || L.dispatch("switchannotationeditormode", {
                                         source: this,
-                                        mode: j,
+                                        mode: U,
                                         editId: c
                                     });
                                 });
                             }
                         };
                         u = new WeakMap();
                         let T = d;
@@ -15329,56 +15329,56 @@
                         }
                         b = new WeakSet(), ce = function() {
                             this.container.setAttribute("data-internal-link", "");
                         }, O = new WeakSet(), On = function(c, L) {
                             c.href = this.linkService.getAnchorUrl(""), c.onclick = () => (this.linkService.executeSetOCGState(L), !1), J(this, b, ce).call(this);
                         };
                         class m extends T {
-                            constructor(j) {
-                                super(j, {
+                            constructor(U) {
+                                super(U, {
                                     isRenderable: !0
                                 });
                             }
                             render() {
                                 this.container.classList.add("textAnnotation");
-                                const j = document.createElement("img");
-                                return j.src = this.imageResourcesPath + "annotation-" + this.data.name.toLowerCase() + ".svg", j.alt = "[{{type}} Annotation]", j.dataset.l10nId = "text_annotation_type", j.dataset.l10nArgs = JSON.stringify({
+                                const U = document.createElement("img");
+                                return U.src = this.imageResourcesPath + "annotation-" + this.data.name.toLowerCase() + ".svg", U.alt = "[{{type}} Annotation]", U.dataset.l10nId = "text_annotation_type", U.dataset.l10nArgs = JSON.stringify({
                                     type: this.data.name
-                                }), !this.data.popupRef && this.hasPopupData && this._createPopup(), this.container.append(j), this.container;
+                                }), !this.data.popupRef && this.hasPopupData && this._createPopup(), this.container.append(U), this.container;
                             }
                         }
                         class C extends T {
                             render() {
                                 return this.data.alternativeText && (this.container.title = this.data.alternativeText), this.container;
                             }
-                            showElementAndHideCanvas(j) {
+                            showElementAndHideCanvas(U) {
                                 var c;
-                                this.data.hasOwnCanvas && (((c = j.previousSibling) == null ? void 0 : c.nodeName) === "CANVAS" && (j.previousSibling.hidden = !0), j.hidden = !1);
+                                this.data.hasOwnCanvas && (((c = U.previousSibling) == null ? void 0 : c.nodeName) === "CANVAS" && (U.previousSibling.hidden = !0), U.hidden = !1);
                             }
-                            _getKeyModifier(j) {
+                            _getKeyModifier(U) {
                                 const {
                                     isWin: c,
                                     isMac: L
                                 } = e.FeatureTest.platform;
-                                return c && j.ctrlKey || L && j.metaKey;
+                                return c && U.ctrlKey || L && U.metaKey;
                             }
-                            _setEventListener(j, c, L, q, K) {
-                                L.includes("mouse") ? j.addEventListener(L, (tt) => {
+                            _setEventListener(U, c, L, q, K) {
+                                L.includes("mouse") ? U.addEventListener(L, (tt) => {
                                     var ct;
                                     (ct = this.linkService.eventBus) == null || ct.dispatch("dispatcheventinsandbox", {
                                         source: this,
                                         detail: {
                                             id: this.data.id,
                                             name: q,
                                             value: K(tt),
                                             shift: tt.shiftKey,
                                             modifier: this._getKeyModifier(tt)
                                         }
                                     });
-                                }) : j.addEventListener(L, (tt) => {
+                                }) : U.addEventListener(L, (tt) => {
                                     var ct;
                                     if (L === "blur") {
                                         if (!c.focused || !tt.relatedTarget)
                                             return;
                                         c.focused = !1;
                                     } else if (L === "focus") {
                                         if (c.focused)
@@ -15391,91 +15391,91 @@
                                             id: this.data.id,
                                             name: q,
                                             value: K(tt)
                                         }
                                     }));
                                 });
                             }
-                            _setEventListeners(j, c, L, q) {
+                            _setEventListeners(U, c, L, q) {
                                 var K, tt, ct;
                                 for (const [bt, Mt] of L)
                                     (Mt === "Action" || (K = this.data.actions) != null && K[Mt]) && ((Mt === "Focus" || Mt === "Blur") && (c || (c = {
                                         focused: !1
-                                    })), this._setEventListener(j, c, bt, Mt, q), Mt === "Focus" && !((tt = this.data.actions) != null && tt.Blur) ? this._setEventListener(j, c, "blur", "Blur", null) : Mt === "Blur" && !((ct = this.data.actions) != null && ct.Focus) && this._setEventListener(j, c, "focus", "Focus", null));
+                                    })), this._setEventListener(U, c, bt, Mt, q), Mt === "Focus" && !((tt = this.data.actions) != null && tt.Blur) ? this._setEventListener(U, c, "blur", "Blur", null) : Mt === "Blur" && !((ct = this.data.actions) != null && ct.Focus) && this._setEventListener(U, c, "focus", "Focus", null));
                             }
-                            _setBackgroundColor(j) {
+                            _setBackgroundColor(U) {
                                 const c = this.data.backgroundColor || null;
-                                j.style.backgroundColor = c === null ? "transparent" : e.Util.makeHexColor(c[0], c[1], c[2]);
+                                U.style.backgroundColor = c === null ? "transparent" : e.Util.makeHexColor(c[0], c[1], c[2]);
                             }
-                            _setTextStyle(j) {
+                            _setTextStyle(U) {
                                 const c = ["left", "center", "right"],
                                     {
                                         fontColor: L
                                     } = this.data.defaultAppearanceData,
                                     q = this.data.defaultAppearanceData.fontSize || o,
-                                    K = j.style;
+                                    K = U.style;
                                 let tt;
                                 const ct = 2,
                                     bt = (Mt) => Math.round(10 * Mt) / 10;
                                 if (this.data.multiLine) {
                                     const Mt = Math.abs(this.data.rect[3] - this.data.rect[1] - ct),
                                         Ft = Math.round(Mt / (e.LINE_FACTOR * q)) || 1,
                                         Ht = Mt / Ft;
                                     tt = Math.min(q, bt(Ht / e.LINE_FACTOR));
                                 } else {
                                     const Mt = Math.abs(this.data.rect[3] - this.data.rect[1] - ct);
                                     tt = Math.min(q, bt(Mt / e.LINE_FACTOR));
                                 }
                                 K.fontSize = `calc(${tt}px * var(--scale-factor))`, K.color = e.Util.makeHexColor(L[0], L[1], L[2]), this.data.textAlignment !== null && (K.textAlign = c[this.data.textAlignment]);
                             }
-                            _setRequired(j, c) {
-                                c ? j.setAttribute("required", !0) : j.removeAttribute("required"), j.setAttribute("aria-required", c);
+                            _setRequired(U, c) {
+                                c ? U.setAttribute("required", !0) : U.removeAttribute("required"), U.setAttribute("aria-required", c);
                             }
                         }
                         class x extends C {
-                            constructor(j) {
-                                const c = j.renderForms || !j.data.hasAppearance && !!j.data.fieldValue;
-                                super(j, {
+                            constructor(U) {
+                                const c = U.renderForms || !U.data.hasAppearance && !!U.data.fieldValue;
+                                super(U, {
                                     isRenderable: c
                                 });
                             }
-                            setPropertyOnSiblings(j, c, L, q) {
+                            setPropertyOnSiblings(U, c, L, q) {
                                 const K = this.annotationStorage;
-                                for (const tt of this._getElementsByName(j.name, j.id))
+                                for (const tt of this._getElementsByName(U.name, U.id))
                                     tt.domElement && (tt.domElement[c] = L), K.setValue(tt.id, {
                                         [q]: L
                                     });
                             }
                             render() {
                                 var q, K;
-                                const j = this.annotationStorage,
+                                const U = this.annotationStorage,
                                     c = this.data.id;
                                 this.container.classList.add("textWidgetAnnotation");
                                 let L = null;
                                 if (this.renderForms) {
-                                    const tt = j.getValue(c, {
+                                    const tt = U.getValue(c, {
                                         value: this.data.fieldValue
                                     });
                                     let ct = tt.value || "";
-                                    const bt = j.getValue(c, {
+                                    const bt = U.getValue(c, {
                                         charLimit: this.data.maxLen
                                     }).charLimit;
                                     bt && ct.length > bt && (ct = ct.slice(0, bt));
                                     let Mt = tt.formattedValue || ((q = this.data.textContent) == null ? void 0 : q.join(`
 `)) || null;
                                     Mt && this.data.comb && (Mt = Mt.replaceAll(/\s+/g, ""));
                                     const Ft = {
                                         userValue: ct,
                                         formattedValue: Mt,
                                         lastCommittedValue: null,
                                         commitKey: 1,
                                         focused: !1
                                     };
                                     this.data.multiLine ? (L = document.createElement("textarea"), L.textContent = Mt ?? ct, this.data.doNotScroll && (L.style.overflowY = "hidden")) : (L = document.createElement("input"), L.type = "text", L.setAttribute("value", Mt ?? ct), this.data.doNotScroll && (L.style.overflowX = "hidden")), this.data.hasOwnCanvas && (L.hidden = !0), F.add(L), L.setAttribute("data-element-id", c), L.disabled = this.data.readOnly, L.name = this.data.fieldName, L.tabIndex = h, this._setRequired(L, this.data.required), bt && (L.maxLength = bt), L.addEventListener("input", (xt) => {
-                                        j.setValue(c, {
+                                        U.setValue(c, {
                                             value: xt.target.value
                                         }), this.setPropertyOnSiblings(L, "value", xt.target.value, "value"), Ft.formattedValue = null;
                                     }), L.addEventListener("resetform", (xt) => {
                                         const Dt = this.data.defaultFieldValue ?? "";
                                         L.value = Ft.userValue = Dt, Ft.formattedValue = null;
                                     });
                                     let Ht = (xt) => {
@@ -15492,23 +15492,23 @@
                                                 target: Ut
                                             } = Dt;
                                             Ft.userValue && (Ut.value = Ft.userValue), Ft.lastCommittedValue = Ut.value, Ft.commitKey = 1, Ft.focused = !0;
                                         }), L.addEventListener("updatefromsandbox", (Dt) => {
                                             this.showElementAndHideCanvas(Dt.target);
                                             const Ut = {
                                                 value(Xt) {
-                                                    Ft.userValue = Xt.detail.value ?? "", j.setValue(c, {
+                                                    Ft.userValue = Xt.detail.value ?? "", U.setValue(c, {
                                                         value: Ft.userValue.toString()
                                                     }), Xt.target.value = Ft.userValue;
                                                 },
                                                 formattedValue(Xt) {
                                                     const {
                                                         formattedValue: Kt
                                                     } = Xt.detail;
-                                                    Ft.formattedValue = Kt, Kt != null && Xt.target !== document.activeElement && (Xt.target.value = Kt), j.setValue(c, {
+                                                    Ft.formattedValue = Kt, Kt != null && Xt.target !== document.activeElement && (Xt.target.value = Kt), U.setValue(c, {
                                                         formattedValue: Kt
                                                     });
                                                 },
                                                 selRange(Xt) {
                                                     Xt.target.setSelectionRange(...Xt.detail.selRange);
                                                 },
                                                 charLimit: (Xt) => {
@@ -15520,15 +15520,15 @@
                                                     } = Xt;
                                                     if (Kt === 0) {
                                                         Zt.removeAttribute("maxLength");
                                                         return;
                                                     }
                                                     Zt.setAttribute("maxLength", Kt);
                                                     let ie = Ft.userValue;
-                                                    !ie || ie.length <= Kt || (ie = ie.slice(0, Kt), Zt.value = Ft.userValue = ie, j.setValue(c, {
+                                                    !ie || ie.length <= Kt || (ie = ie.slice(0, Kt), Zt.value = Ft.userValue = ie, U.setValue(c, {
                                                         value: ie
                                                     }), (ne = this.linkService.eventBus) == null || ne.dispatch("dispatcheventinsandbox", {
                                                         source: this,
                                                         detail: {
                                                             id: c,
                                                             name: "Keystroke",
                                                             value: ie,
@@ -15642,58 +15642,58 @@
                                     }
                                 } else
                                     L = document.createElement("div"), L.textContent = this.data.fieldValue, L.style.verticalAlign = "middle", L.style.display = "table-cell";
                                 return this._setTextStyle(L), this._setBackgroundColor(L), this._setDefaultPropertiesFromJS(L), this.container.append(L), this.container;
                             }
                         }
                         class E extends C {
-                            constructor(j) {
-                                super(j, {
-                                    isRenderable: !!j.data.hasOwnCanvas
+                            constructor(U) {
+                                super(U, {
+                                    isRenderable: !!U.data.hasOwnCanvas
                                 });
                             }
                         }
                         class S extends C {
-                            constructor(j) {
-                                super(j, {
-                                    isRenderable: j.renderForms
+                            constructor(U) {
+                                super(U, {
+                                    isRenderable: U.renderForms
                                 });
                             }
                             render() {
-                                const j = this.annotationStorage,
+                                const U = this.annotationStorage,
                                     c = this.data,
                                     L = c.id;
-                                let q = j.getValue(L, {
+                                let q = U.getValue(L, {
                                     value: c.exportValue === c.fieldValue
                                 }).value;
-                                typeof q == "string" && (q = q !== "Off", j.setValue(L, {
+                                typeof q == "string" && (q = q !== "Off", U.setValue(L, {
                                     value: q
                                 })), this.container.classList.add("buttonWidgetAnnotation", "checkBox");
                                 const K = document.createElement("input");
                                 return F.add(K), K.setAttribute("data-element-id", L), K.disabled = c.readOnly, this._setRequired(K, this.data.required), K.type = "checkbox", K.name = c.fieldName, q && K.setAttribute("checked", !0), K.setAttribute("exportValue", c.exportValue), K.tabIndex = h, K.addEventListener("change", (tt) => {
                                     const {
                                         name: ct,
                                         checked: bt
                                     } = tt.target;
                                     for (const Mt of this._getElementsByName(ct, L)) {
                                         const Ft = bt && Mt.exportValue === c.exportValue;
-                                        Mt.domElement && (Mt.domElement.checked = Ft), j.setValue(Mt.id, {
+                                        Mt.domElement && (Mt.domElement.checked = Ft), U.setValue(Mt.id, {
                                             value: Ft
                                         });
                                     }
-                                    j.setValue(L, {
+                                    U.setValue(L, {
                                         value: bt
                                     });
                                 }), K.addEventListener("resetform", (tt) => {
                                     const ct = c.defaultFieldValue || "Off";
                                     tt.target.checked = ct === c.exportValue;
                                 }), this.enableScripting && this.hasJSActions && (K.addEventListener("updatefromsandbox", (tt) => {
                                     const ct = {
                                         value(bt) {
-                                            bt.target.checked = bt.detail.value !== "Off", j.setValue(L, {
+                                            bt.target.checked = bt.detail.value !== "Off", U.setValue(L, {
                                                 value: bt.target.checked
                                             });
                                         }
                                     };
                                     this._dispatchEventFromSandbox(ct, tt);
                                 }), this._setEventListeners(K, null, [
                                     ["change", "Validate"],
@@ -15704,55 +15704,55 @@
                                     ["mouseenter", "Mouse Enter"],
                                     ["mouseleave", "Mouse Exit"],
                                     ["mouseup", "Mouse Up"]
                                 ], (tt) => tt.target.checked)), this._setBackgroundColor(K), this._setDefaultPropertiesFromJS(K), this.container.append(K), this.container;
                             }
                         }
                         class g extends C {
-                            constructor(j) {
-                                super(j, {
-                                    isRenderable: j.renderForms
+                            constructor(U) {
+                                super(U, {
+                                    isRenderable: U.renderForms
                                 });
                             }
                             render() {
                                 this.container.classList.add("buttonWidgetAnnotation", "radioButton");
-                                const j = this.annotationStorage,
+                                const U = this.annotationStorage,
                                     c = this.data,
                                     L = c.id;
-                                let q = j.getValue(L, {
+                                let q = U.getValue(L, {
                                     value: c.fieldValue === c.buttonValue
                                 }).value;
-                                typeof q == "string" && (q = q !== c.buttonValue, j.setValue(L, {
+                                typeof q == "string" && (q = q !== c.buttonValue, U.setValue(L, {
                                     value: q
                                 }));
                                 const K = document.createElement("input");
                                 if (F.add(K), K.setAttribute("data-element-id", L), K.disabled = c.readOnly, this._setRequired(K, this.data.required), K.type = "radio", K.name = c.fieldName, q && K.setAttribute("checked", !0), K.tabIndex = h, K.addEventListener("change", (tt) => {
                                         const {
                                             name: ct,
                                             checked: bt
                                         } = tt.target;
                                         for (const Mt of this._getElementsByName(ct, L))
-                                            j.setValue(Mt.id, {
+                                            U.setValue(Mt.id, {
                                                 value: !1
                                             });
-                                        j.setValue(L, {
+                                        U.setValue(L, {
                                             value: bt
                                         });
                                     }), K.addEventListener("resetform", (tt) => {
                                         const ct = c.defaultFieldValue;
                                         tt.target.checked = ct != null && ct === c.buttonValue;
                                     }), this.enableScripting && this.hasJSActions) {
                                     const tt = c.buttonValue;
                                     K.addEventListener("updatefromsandbox", (ct) => {
                                         const bt = {
                                             value: (Mt) => {
                                                 const Ft = tt === Mt.detail.value;
                                                 for (const Ht of this._getElementsByName(Mt.target.name)) {
                                                     const xt = Ft && Ht.id === L;
-                                                    Ht.domElement && (Ht.domElement.checked = xt), j.setValue(Ht.id, {
+                                                    Ht.domElement && (Ht.domElement.checked = xt), U.setValue(Ht.id, {
                                                         value: xt
                                                     });
                                                 }
                                             }
                                         };
                                         this._dispatchEventFromSandbox(bt, ct);
                                     }), this._setEventListeners(K, null, [
@@ -15766,39 +15766,39 @@
                                         ["mouseup", "Mouse Up"]
                                     ], (ct) => ct.target.checked);
                                 }
                                 return this._setBackgroundColor(K), this._setDefaultPropertiesFromJS(K), this.container.append(K), this.container;
                             }
                         }
                         class v extends P {
-                            constructor(j) {
-                                super(j, {
-                                    ignoreBorder: j.data.hasAppearance
+                            constructor(U) {
+                                super(U, {
+                                    ignoreBorder: U.data.hasAppearance
                                 });
                             }
                             render() {
-                                const j = super.render();
-                                j.classList.add("buttonWidgetAnnotation", "pushButton"), this.data.alternativeText && (j.title = this.data.alternativeText);
-                                const c = j.lastChild;
+                                const U = super.render();
+                                U.classList.add("buttonWidgetAnnotation", "pushButton"), this.data.alternativeText && (U.title = this.data.alternativeText);
+                                const c = U.lastChild;
                                 return this.enableScripting && this.hasJSActions && c && (this._setDefaultPropertiesFromJS(c), c.addEventListener("updatefromsandbox", (L) => {
                                     this._dispatchEventFromSandbox({}, L);
-                                })), j;
+                                })), U;
                             }
                         }
                         class $ extends C {
-                            constructor(j) {
-                                super(j, {
-                                    isRenderable: j.renderForms
+                            constructor(U) {
+                                super(U, {
+                                    isRenderable: U.renderForms
                                 });
                             }
                             render() {
                                 this.container.classList.add("choiceWidgetAnnotation");
-                                const j = this.annotationStorage,
+                                const U = this.annotationStorage,
                                     c = this.data.id,
-                                    L = j.getValue(c, {
+                                    L = U.getValue(c, {
                                         value: this.data.fieldValue
                                     }),
                                     q = document.createElement("select");
                                 F.add(q), q.setAttribute("data-element-id", c), q.disabled = this.data.readOnly, this._setRequired(q, this.data.required), q.name = this.data.fieldName, q.tabIndex = h;
                                 let K = this.data.combo && this.data.options.length > 0;
                                 this.data.combo || (q.size = this.data.options.length, this.data.multiSelect && (q.multiple = !0)), q.addEventListener("resetform", (Ft) => {
                                     const Ht = this.data.defaultFieldValue;
@@ -15836,44 +15836,44 @@
                                     const Ht = {
                                         value(xt) {
                                             tt == null || tt();
                                             const Dt = xt.detail.value,
                                                 Ut = new Set(Array.isArray(Dt) ? Dt : [Dt]);
                                             for (const Xt of q.options)
                                                 Xt.selected = Ut.has(Xt.value);
-                                            j.setValue(c, {
+                                            U.setValue(c, {
                                                 value: ct(!0)
                                             }), bt = ct(!1);
                                         },
                                         multipleSelection(xt) {
                                             q.multiple = !0;
                                         },
                                         remove(xt) {
                                             const Dt = q.options,
                                                 Ut = xt.detail.remove;
-                                            Dt[Ut].selected = !1, q.remove(Ut), Dt.length > 0 && Array.prototype.findIndex.call(Dt, (Kt) => Kt.selected) === -1 && (Dt[0].selected = !0), j.setValue(c, {
+                                            Dt[Ut].selected = !1, q.remove(Ut), Dt.length > 0 && Array.prototype.findIndex.call(Dt, (Kt) => Kt.selected) === -1 && (Dt[0].selected = !0), U.setValue(c, {
                                                 value: ct(!0),
                                                 items: Mt(xt)
                                             }), bt = ct(!1);
                                         },
                                         clear(xt) {
                                             for (; q.length !== 0;)
                                                 q.remove(0);
-                                            j.setValue(c, {
+                                            U.setValue(c, {
                                                 value: null,
                                                 items: []
                                             }), bt = ct(!1);
                                         },
                                         insert(xt) {
                                             const {
                                                 index: Dt,
                                                 displayValue: Ut,
                                                 exportValue: Xt
                                             } = xt.detail.insert, Kt = q.children[Dt], Zt = document.createElement("option");
-                                            Zt.textContent = Ut, Zt.value = Xt, Kt ? Kt.before(Zt) : q.append(Zt), j.setValue(c, {
+                                            Zt.textContent = Ut, Zt.value = Xt, Kt ? Kt.before(Zt) : q.append(Zt), U.setValue(c, {
                                                 value: ct(!0),
                                                 items: Mt(xt)
                                             }), bt = ct(!1);
                                         },
                                         items(xt) {
                                             const {
                                                 items: Dt
@@ -15883,36 +15883,36 @@
                                             for (const Ut of Dt) {
                                                 const {
                                                     displayValue: Xt,
                                                     exportValue: Kt
                                                 } = Ut, Zt = document.createElement("option");
                                                 Zt.textContent = Xt, Zt.value = Kt, q.append(Zt);
                                             }
-                                            q.options.length > 0 && (q.options[0].selected = !0), j.setValue(c, {
+                                            q.options.length > 0 && (q.options[0].selected = !0), U.setValue(c, {
                                                 value: ct(!0),
                                                 items: Mt(xt)
                                             }), bt = ct(!1);
                                         },
                                         indices(xt) {
                                             const Dt = new Set(xt.detail.indices);
                                             for (const Ut of xt.target.options)
                                                 Ut.selected = Dt.has(Ut.index);
-                                            j.setValue(c, {
+                                            U.setValue(c, {
                                                 value: ct(!0)
                                             }), bt = ct(!1);
                                         },
                                         editable(xt) {
                                             xt.target.disabled = !xt.detail.editable;
                                         }
                                     };
                                     this._dispatchEventFromSandbox(Ht, Ft);
                                 }), q.addEventListener("input", (Ft) => {
                                     var xt;
                                     const Ht = ct(!0);
-                                    j.setValue(c, {
+                                    U.setValue(c, {
                                         value: Ht
                                     }), Ft.preventDefault(), (xt = this.linkService.eventBus) == null || xt.dispatch("dispatcheventinsandbox", {
                                         source: this,
                                         detail: {
                                             id: c,
                                             name: "Keystroke",
                                             value: bt,
@@ -15928,54 +15928,54 @@
                                     ["mousedown", "Mouse Down"],
                                     ["mouseenter", "Mouse Enter"],
                                     ["mouseleave", "Mouse Exit"],
                                     ["mouseup", "Mouse Up"],
                                     ["input", "Action"],
                                     ["input", "Validate"]
                                 ], (Ft) => Ft.target.value)) : q.addEventListener("input", function(Ft) {
-                                    j.setValue(c, {
+                                    U.setValue(c, {
                                         value: ct(!0)
                                     });
                                 }), this.data.combo && this._setTextStyle(q), this._setBackgroundColor(q), this._setDefaultPropertiesFromJS(q), this.container.append(q), this.container;
                             }
                         }
                         class M extends T {
-                            constructor(j) {
+                            constructor(U) {
                                 const {
                                     data: c,
                                     elements: L
-                                } = j;
-                                super(j, {
+                                } = U;
+                                super(U, {
                                     isRenderable: T._hasPopupData(c)
                                 }), this.elements = L;
                             }
                             render() {
                                 this.container.classList.add("popupAnnotation");
-                                const j = new _({
+                                const U = new _({
                                         container: this.container,
                                         color: this.data.color,
                                         titleObj: this.data.titleObj,
                                         modificationDate: this.data.modificationDate,
                                         contentsObj: this.data.contentsObj,
                                         richText: this.data.richText,
                                         rect: this.data.rect,
                                         parentRect: this.data.parentRect || null,
                                         parent: this.parent,
                                         elements: this.elements,
                                         open: this.data.open
                                     }),
                                     c = [];
                                 for (const L of this.elements)
-                                    L.popup = j, c.push(L.data.id), L.addHighlightArea();
+                                    L.popup = U, c.push(L.data.id), L.addHighlightArea();
                                 return this.container.setAttribute("aria-controls", c.map((L) => `${e.AnnotationPrefix}${L}`).join(",")), this.container;
                             }
                         }
                         class _ {
                             constructor({
-                                container: j,
+                                container: U,
                                 color: c,
                                 elements: L,
                                 titleObj: q,
                                 modificationDate: K,
                                 contentsObj: tt,
                                 richText: ct,
                                 parent: bt,
@@ -16001,15 +16001,15 @@
                                 W(this, _t, !1);
                                 W(this, rt, null);
                                 W(this, at, null);
                                 W(this, pt, null);
                                 W(this, Ct, null);
                                 W(this, Tt, !1);
                                 var Dt;
-                                ot(this, ft, j), ot(this, Ct, q), ot(this, kt, tt), ot(this, pt, ct), ot(this, St, bt), ot(this, mt, c), ot(this, at, Mt), ot(this, It, Ft), ot(this, Rt, L);
+                                ot(this, ft, U), ot(this, Ct, q), ot(this, kt, tt), ot(this, pt, ct), ot(this, St, bt), ot(this, mt, c), ot(this, at, Mt), ot(this, It, Ft), ot(this, Rt, L);
                                 const xt = s.PDFDateString.toDateObject(K);
                                 xt && ot(this, z, bt.l10n.get("annotation_date_string", {
                                     date: xt.toLocaleDateString(),
                                     time: xt.toLocaleTimeString()
                                 })), this.trigger = L.flatMap((Ut) => Ut.getElementsToTriggerPopup());
                                 for (const Ut of this.trigger)
                                     Ut.addEventListener("click", r(this, ht)), Ut.addEventListener("mouseenter", r(this, lt)), Ut.addEventListener("mouseleave", r(this, Z)), Ut.classList.add("popupTriggerArea");
@@ -16018,15 +16018,15 @@
                                 r(this, ft).hidden = !0, Ht && J(this, jt, Me).call(this);
                             }
                             render() {
                                 if (r(this, rt))
                                     return;
                                 const {
                                     page: {
-                                        view: j
+                                        view: U
                                     },
                                     viewport: {
                                         rawDims: {
                                             pageWidth: c,
                                             pageHeight: L,
                                             pageX: q,
                                             pageY: K
@@ -16064,30 +16064,30 @@
                                 let Ht = !!r(this, It),
                                     xt = Ht ? r(this, It) : r(this, at);
                                 for (const ne of r(this, Rt))
                                     if (!xt || e.Util.intersect(ne.data.rect, xt) !== null) {
                                         xt = ne.data.rect, Ht = !0;
                                         break;
                                     }
-                                const Dt = e.Util.normalizeRect([xt[0], j[3] - xt[1] + j[1], xt[2], j[3] - xt[3] + j[1]]),
+                                const Dt = e.Util.normalizeRect([xt[0], U[3] - xt[1] + U[1], xt[2], U[3] - xt[3] + U[1]]),
                                     Xt = Ht ? xt[2] - xt[0] + 5 : 0,
                                     Kt = Dt[0] + Xt,
                                     Zt = Dt[1],
                                     {
                                         style: ie
                                     } = r(this, ft);
                                 ie.left = `${100 * (Kt - q) / c}%`, ie.top = `${100 * (Zt - K) / L}%`, r(this, ft).append(tt);
                             }
                             _formatContents({
-                                str: j,
+                                str: U,
                                 dir: c
                             }) {
                                 const L = document.createElement("p");
                                 L.classList.add("popupContent"), L.dir = c;
-                                const q = j.split(/(?:\r\n?|\n)/);
+                                const q = U.split(/(?:\r\n?|\n)/);
                                 for (let K = 0, tt = q.length; K < tt; ++K) {
                                     const ct = q[K];
                                     L.append(document.createTextNode(ct)), K < tt - 1 && L.append(document.createElement("br"));
                                 }
                                 return L;
                             }
                             forceHide() {
@@ -16096,39 +16096,39 @@
                             maybeShow() {
                                 r(this, Tt) && (ot(this, Tt, !1), r(this, ft).hidden = !1);
                             }
                             get isVisible() {
                                 return r(this, ft).hidden === !1;
                             }
                         }
-                        z = new WeakMap(), it = new WeakMap(), Z = new WeakMap(), lt = new WeakMap(), ht = new WeakMap(), mt = new WeakMap(), ft = new WeakMap(), kt = new WeakMap(), Rt = new WeakMap(), St = new WeakMap(), It = new WeakMap(), _t = new WeakMap(), rt = new WeakMap(), at = new WeakMap(), pt = new WeakMap(), Ct = new WeakMap(), Tt = new WeakMap(), Bt = new WeakSet(), $n = function(j) {
-                            j.altKey || j.shiftKey || j.ctrlKey || j.metaKey || (j.key === "Enter" || j.key === "Escape" && r(this, _t)) && J(this, jt, Me).call(this);
+                        z = new WeakMap(), it = new WeakMap(), Z = new WeakMap(), lt = new WeakMap(), ht = new WeakMap(), mt = new WeakMap(), ft = new WeakMap(), kt = new WeakMap(), Rt = new WeakMap(), St = new WeakMap(), It = new WeakMap(), _t = new WeakMap(), rt = new WeakMap(), at = new WeakMap(), pt = new WeakMap(), Ct = new WeakMap(), Tt = new WeakMap(), Bt = new WeakSet(), $n = function(U) {
+                            U.altKey || U.shiftKey || U.ctrlKey || U.metaKey || (U.key === "Enter" || U.key === "Escape" && r(this, _t)) && J(this, jt, Me).call(this);
                         }, jt = new WeakSet(), Me = function() {
                             ot(this, _t, !r(this, _t)), r(this, _t) ? (J(this, Gt, on).call(this), r(this, ft).addEventListener("click", r(this, ht)), r(this, ft).addEventListener("keydown", r(this, it))) : (J(this, Vt, ln).call(this), r(this, ft).removeEventListener("click", r(this, ht)), r(this, ft).removeEventListener("keydown", r(this, it)));
                         }, Gt = new WeakSet(), on = function() {
                             r(this, rt) || this.render(), this.isVisible ? r(this, _t) && r(this, ft).classList.add("focused") : (r(this, ft).hidden = !1, r(this, ft).style.zIndex = parseInt(r(this, ft).style.zIndex) + 1e3);
                         }, Vt = new WeakSet(), ln = function() {
                             r(this, ft).classList.remove("focused"), !(r(this, _t) || !this.isVisible) && (r(this, ft).hidden = !0, r(this, ft).style.zIndex = parseInt(r(this, ft).style.zIndex) - 1e3);
                         };
                         class N extends T {
-                            constructor(j) {
-                                super(j, {
+                            constructor(U) {
+                                super(U, {
                                     isRenderable: !0,
                                     ignoreBorder: !0
-                                }), this.textContent = j.data.textContent, this.textPosition = j.data.textPosition, this.annotationEditorType = e.AnnotationEditorType.FREETEXT;
+                                }), this.textContent = U.data.textContent, this.textPosition = U.data.textPosition, this.annotationEditorType = e.AnnotationEditorType.FREETEXT;
                             }
                             render() {
                                 if (this.container.classList.add("freeTextAnnotation"), this.textContent) {
-                                    const j = document.createElement("div");
-                                    j.classList.add("annotationTextContent"), j.setAttribute("role", "comment");
+                                    const U = document.createElement("div");
+                                    U.classList.add("annotationTextContent"), U.setAttribute("role", "comment");
                                     for (const c of this.textContent) {
                                         const L = document.createElement("span");
-                                        L.textContent = c, j.append(L);
+                                        L.textContent = c, U.append(L);
                                     }
-                                    this.container.append(j);
+                                    this.container.append(U);
                                 }
                                 return !this.data.popupRef && this.hasPopupData && this._createPopup(), this._editOnDoubleClick(), this.container;
                             }
                         }
                         t.FreeTextAnnotationElement = N;
                         class D extends T {
                             constructor(c) {
@@ -16244,22 +16244,22 @@
                                 return r(this, wt);
                             }
                             addHighlightArea() {
                                 this.container.classList.add("highlightArea");
                             }
                         }
                         wt = new WeakMap();
-                        class U extends I {
-                            constructor(j) {
-                                super(j), this.containerClassName = "polygonAnnotation", this.svgElementName = "svg:polygon";
+                        class j extends I {
+                            constructor(U) {
+                                super(U), this.containerClassName = "polygonAnnotation", this.svgElementName = "svg:polygon";
                             }
                         }
                         class G extends T {
-                            constructor(j) {
-                                super(j, {
+                            constructor(U) {
+                                super(U, {
                                     isRenderable: !0,
                                     ignoreBorder: !0
                                 });
                             }
                             render() {
                                 return this.container.classList.add("caretAnnotation"), !this.data.popupRef && this.hasPopupData && this._createPopup(), this.container;
                             }
@@ -16299,64 +16299,64 @@
                             }
                             addHighlightArea() {
                                 this.container.classList.add("highlightArea");
                             }
                         }
                         te = new WeakMap(), t.InkAnnotationElement = V;
                         class H extends T {
-                            constructor(j) {
-                                super(j, {
+                            constructor(U) {
+                                super(U, {
                                     isRenderable: !0,
                                     ignoreBorder: !0,
                                     createQuadrilaterals: !0
                                 });
                             }
                             render() {
                                 return !this.data.popupRef && this.hasPopupData && this._createPopup(), this.container.classList.add("highlightAnnotation"), this.container;
                             }
                         }
                         class st extends T {
-                            constructor(j) {
-                                super(j, {
+                            constructor(U) {
+                                super(U, {
                                     isRenderable: !0,
                                     ignoreBorder: !0,
                                     createQuadrilaterals: !0
                                 });
                             }
                             render() {
                                 return !this.data.popupRef && this.hasPopupData && this._createPopup(), this.container.classList.add("underlineAnnotation"), this.container;
                             }
                         }
                         class dt extends T {
-                            constructor(j) {
-                                super(j, {
+                            constructor(U) {
+                                super(U, {
                                     isRenderable: !0,
                                     ignoreBorder: !0,
                                     createQuadrilaterals: !0
                                 });
                             }
                             render() {
                                 return !this.data.popupRef && this.hasPopupData && this._createPopup(), this.container.classList.add("squigglyAnnotation"), this.container;
                             }
                         }
                         class yt extends T {
-                            constructor(j) {
-                                super(j, {
+                            constructor(U) {
+                                super(U, {
                                     isRenderable: !0,
                                     ignoreBorder: !0,
                                     createQuadrilaterals: !0
                                 });
                             }
                             render() {
                                 return !this.data.popupRef && this.hasPopupData && this._createPopup(), this.container.classList.add("strikeoutAnnotation"), this.container;
                             }
                         }
                         class gt extends T {
-                            constructor(j) {
-                                super(j, {
+                            constructor(U) {
+                                super(U, {
                                     isRenderable: !0,
                                     ignoreBorder: !0
                                 });
                             }
                             render() {
                                 return this.container.classList.add("stampAnnotation"), !this.data.popupRef && this.hasPopupData && this._createPopup(), this.container;
                             }
@@ -16404,46 +16404,46 @@
                         }
                         Qt = new WeakMap(), et = new WeakSet(), cn = function() {
                             var c;
                             (c = this.downloadManager) == null || c.openOrDownloadData(this.container, this.content, this.filename);
                         };
                         class l {
                             constructor({
-                                div: j,
+                                div: U,
                                 accessibilityManager: c,
                                 annotationCanvasMap: L,
                                 l10n: q,
                                 page: K,
                                 viewport: tt
                             }) {
                                 W(this, Nt);
                                 W(this, vt);
                                 W(this, Ot, null);
                                 W(this, Pt, null);
                                 W(this, $t, /* @__PURE__ */ new Map());
-                                this.div = j, ot(this, Ot, c), ot(this, Pt, L), this.l10n = q, this.page = K, this.viewport = tt, this.zIndex = 0, this.l10n || (this.l10n = A.NullL10n);
+                                this.div = U, ot(this, Ot, c), ot(this, Pt, L), this.l10n = q, this.page = K, this.viewport = tt, this.zIndex = 0, this.l10n || (this.l10n = A.NullL10n);
                             }
-                            async render(j) {
+                            async render(U) {
                                 const {
                                     annotations: c
-                                } = j, L = this.div;
+                                } = U, L = this.div;
                                 (0, s.setLayerDimensions)(L, this.viewport);
                                 const q = /* @__PURE__ */ new Map(),
                                     K = {
                                         data: null,
                                         layer: L,
-                                        linkService: j.linkService,
-                                        downloadManager: j.downloadManager,
-                                        imageResourcesPath: j.imageResourcesPath || "",
-                                        renderForms: j.renderForms !== !1,
+                                        linkService: U.linkService,
+                                        downloadManager: U.downloadManager,
+                                        imageResourcesPath: U.imageResourcesPath || "",
+                                        renderForms: U.renderForms !== !1,
                                         svgFactory: new s.DOMSVGFactory(),
-                                        annotationStorage: j.annotationStorage || new p.AnnotationStorage(),
-                                        enableScripting: j.enableScripting === !0,
-                                        hasJSActions: j.hasJSActions,
-                                        fieldObjects: j.fieldObjects,
+                                        annotationStorage: U.annotationStorage || new p.AnnotationStorage(),
+                                        enableScripting: U.enableScripting === !0,
+                                        hasJSActions: U.hasJSActions,
+                                        fieldObjects: U.fieldObjects,
                                         parent: this,
                                         elements: null
                                     };
                                 for (const tt of c) {
                                     if (tt.noHTML)
                                         continue;
                                     const ct = tt.annotationType === e.AnnotationType.POPUP;
@@ -16471,38 +16471,38 @@
                                     bt.annotationEditorType > 0 && r(this, $t).set(bt.data.id, bt);
                                     const Mt = bt.render();
                                     tt.hidden && (Mt.style.visibility = "hidden"), J(this, Nt, Nn).call(this, Mt, tt.id);
                                 }
                                 J(this, vt, hn).call(this), await this.l10n.translate(L);
                             }
                             update({
-                                viewport: j
+                                viewport: U
                             }) {
                                 const c = this.div;
-                                this.viewport = j, (0, s.setLayerDimensions)(c, {
-                                    rotation: j.rotation
+                                this.viewport = U, (0, s.setLayerDimensions)(c, {
+                                    rotation: U.rotation
                                 }), J(this, vt, hn).call(this), c.hidden = !1;
                             }
                             getEditableAnnotations() {
                                 return Array.from(r(this, $t).values());
                             }
-                            getEditableAnnotation(j) {
-                                return r(this, $t).get(j);
+                            getEditableAnnotation(U) {
+                                return r(this, $t).get(U);
                             }
                         }
-                        Ot = new WeakMap(), Pt = new WeakMap(), $t = new WeakMap(), Nt = new WeakSet(), Nn = function(j, c) {
+                        Ot = new WeakMap(), Pt = new WeakMap(), $t = new WeakMap(), Nt = new WeakSet(), Nn = function(U, c) {
                             var q;
-                            const L = j.firstChild || j;
-                            L.id = `${e.AnnotationPrefix}${c}`, this.div.append(j), (q = r(this, Ot)) == null || q.moveElementInDOM(this.div, j, L, !1);
+                            const L = U.firstChild || U;
+                            L.id = `${e.AnnotationPrefix}${c}`, this.div.append(U), (q = r(this, Ot)) == null || q.moveElementInDOM(this.div, U, L, !1);
                         }, vt = new WeakSet(), hn = function() {
                             if (!r(this, Pt))
                                 return;
-                            const j = this.div;
+                            const U = this.div;
                             for (const [c, L] of r(this, Pt)) {
-                                const q = j.querySelector(`[data-annotation-id="${c}"]`);
+                                const q = U.querySelector(`[data-annotation-id="${c}"]`);
                                 if (!q)
                                     continue;
                                 const {
                                     firstChild: K
                                 } = q;
                                 K ? K.nodeName === "CANVAS" ? K.replaceWith(L) : K.before(L) : q.append(L);
                             }
@@ -16819,15 +16819,15 @@
                             }
                         }
                         t.XfaLayer = s;
                     },
                     /* 33 */
                     /***/
                     (i, t, n) => {
-                        var h, o, F, R, w, T, P, m, C, x, E, S, g, v, $, Bn, _, Un, D, jn, Y, qn, U, dn, V, Wn, st, un, yt, Hn, k, zn, u, Gn, b, Xn, O, Vn, z, ae, Z, pn, ht, Re, ft, xe, Rt, fe, It, gn, rt, De, pt, Yn, Tt, _n, Wt, Kn, zt, Jn, qt, mn, ut, Ie, Q, pe;
+                        var h, o, F, R, w, T, P, m, C, x, E, S, g, v, $, Bn, _, Un, D, jn, Y, qn, j, dn, V, Wn, st, un, yt, Hn, k, zn, u, Gn, b, Xn, O, Vn, z, ae, Z, pn, ht, Re, ft, xe, Rt, fe, It, gn, rt, De, pt, Yn, Tt, _n, Wt, Kn, zt, Jn, qt, mn, ut, Ie, Q, pe;
                         Object.defineProperty(t, "__esModule", {
                             value: !0
                         }), t.InkEditor = void 0;
                         var e = n(1),
                             s = n(4),
                             p = n(29),
                             f = n(6),
@@ -16838,15 +16838,15 @@
                                     ...et,
                                     name: "inkEditor"
                                 });
                                 W(this, $);
                                 W(this, _);
                                 W(this, D);
                                 W(this, Y);
-                                W(this, U);
+                                W(this, j);
                                 W(this, V);
                                 W(this, st);
                                 W(this, yt);
                                 W(this, k);
                                 W(this, u);
                                 W(this, b);
                                 W(this, O);
@@ -17000,22 +17000,22 @@
                                 if (et instanceof p.InkAnnotationElement)
                                     return null;
                                 const Pt = super.deserialize(et, Et, Ot);
                                 Pt.thickness = et.thickness, Pt.color = e.Util.makeHexColor(...et.color), Pt.opacity = et.opacity;
                                 const [$t, Nt] = Pt.pageDimensions, Jt = Pt.width * $t, vt = Pt.height * Nt, Yt = Pt.parentScale, Lt = et.thickness / 2;
                                 ot(Pt, m, !0), ot(Pt, S, Math.round(Jt)), ot(Pt, g, Math.round(vt));
                                 const {
-                                    paths: j,
+                                    paths: U,
                                     rect: c,
                                     rotation: L
                                 } = et;
                                 for (let {
                                         bezier: bt
                                     }
-                                    of j) {
+                                    of U) {
                                     bt = J(K = wt, Wt, Kn).call(K, bt, c, L);
                                     const Mt = [];
                                     Pt.paths.push(Mt);
                                     let Ft = Yt * (bt[0] - Lt),
                                         Ht = Yt * (bt[1] - Lt);
                                     for (let Dt = 2, Ut = bt.length; Dt < Ut; Dt += 6) {
                                         const Xt = Yt * (bt[Dt] - Lt),
@@ -17109,26 +17109,26 @@
                                 case 180:
                                     return [Et, Ot, Et, Ot];
                                 case 270:
                                     return [Et, 0, Ot, Et];
                                 default:
                                     return [0, 0, Et, Ot];
                             }
-                        }, U = new WeakSet(), dn = function() {
+                        }, j = new WeakSet(), dn = function() {
                             const {
                                 ctx: et,
                                 color: Et,
                                 opacity: Ot,
                                 thickness: Pt,
                                 parentScale: $t,
                                 scaleFactor: Nt
                             } = this;
                             et.lineWidth = Pt * $t / Nt, et.lineCap = "round", et.lineJoin = "round", et.miterLimit = 10, et.strokeStyle = `${Et}${(0, A.opacityToHex)(Ot)}`;
                         }, V = new WeakSet(), Wn = function(et, Et) {
-                            this.canvas.addEventListener("contextmenu", f.noContextMenu), this.canvas.addEventListener("pointerleave", r(this, R)), this.canvas.addEventListener("pointermove", r(this, F)), this.canvas.addEventListener("pointerup", r(this, w)), this.canvas.removeEventListener("pointerdown", r(this, T)), this.isEditing = !0, r(this, x) || (ot(this, x, !0), J(this, Rt, fe).call(this), this.thickness || (this.thickness = wt._defaultThickness), this.color || (this.color = wt._defaultColor || s.AnnotationEditor._defaultLineColor), this.opacity ?? (this.opacity = wt._defaultOpacity)), this.currentPath.push([et, Et]), ot(this, C, !1), J(this, U, dn).call(this), ot(this, v, () => {
+                            this.canvas.addEventListener("contextmenu", f.noContextMenu), this.canvas.addEventListener("pointerleave", r(this, R)), this.canvas.addEventListener("pointermove", r(this, F)), this.canvas.addEventListener("pointerup", r(this, w)), this.canvas.removeEventListener("pointerdown", r(this, T)), this.isEditing = !0, r(this, x) || (ot(this, x, !0), J(this, Rt, fe).call(this), this.thickness || (this.thickness = wt._defaultThickness), this.color || (this.color = wt._defaultColor || s.AnnotationEditor._defaultLineColor), this.opacity ?? (this.opacity = wt._defaultOpacity)), this.currentPath.push([et, Et]), ot(this, C, !1), J(this, j, dn).call(this), ot(this, v, () => {
                                 J(this, u, Gn).call(this), r(this, v) && window.requestAnimationFrame(r(this, v));
                             }), window.requestAnimationFrame(r(this, v));
                         }, st = new WeakSet(), un = function(et, Et) {
                             const [Ot, Pt] = this.currentPath.at(-1);
                             if (this.currentPath.length > 1 && et === Ot && Et === Pt)
                                 return;
                             const $t = this.currentPath;
@@ -17184,40 +17184,40 @@
                             for (const Nt of this.bezierPath2D)
                                 $t.stroke(Nt);
                             $t.stroke(r(this, P)), $t.restore();
                         }, b = new WeakSet(), Xn = function(et, Et, Ot, Pt, $t, Nt, Jt) {
                             const vt = (Et + Pt) / 2,
                                 Yt = (Ot + $t) / 2,
                                 Lt = (Pt + Nt) / 2,
-                                j = ($t + Jt) / 2;
-                            et.bezierCurveTo(vt + 2 * (Pt - vt) / 3, Yt + 2 * ($t - Yt) / 3, Lt + 2 * (Pt - Lt) / 3, j + 2 * ($t - j) / 3, Lt, j);
+                                U = ($t + Jt) / 2;
+                            et.bezierCurveTo(vt + 2 * (Pt - vt) / 3, Yt + 2 * ($t - Yt) / 3, Lt + 2 * (Pt - Lt) / 3, U + 2 * ($t - U) / 3, Lt, U);
                         }, O = new WeakSet(), Vn = function() {
                             const et = this.currentPath;
                             if (et.length <= 2)
                                 return [
                                     [et[0], et[0], et.at(-1), et.at(-1)]
                                 ];
                             const Et = [];
                             let Ot, [Pt, $t] = et[0];
                             for (Ot = 1; Ot < et.length - 2; Ot++) {
                                 const [c, L] = et[Ot], [q, K] = et[Ot + 1], tt = (c + q) / 2, ct = (L + K) / 2, bt = [Pt + 2 * (c - Pt) / 3, $t + 2 * (L - $t) / 3], Mt = [tt + 2 * (c - tt) / 3, ct + 2 * (L - ct) / 3];
                                 Et.push([
                                     [Pt, $t], bt, Mt, [tt, ct]
                                 ]), [Pt, $t] = [tt, ct];
                             }
-                            const [Nt, Jt] = et[Ot], [vt, Yt] = et[Ot + 1], Lt = [Pt + 2 * (Nt - Pt) / 3, $t + 2 * (Jt - $t) / 3], j = [vt + 2 * (Nt - vt) / 3, Yt + 2 * (Jt - Yt) / 3];
+                            const [Nt, Jt] = et[Ot], [vt, Yt] = et[Ot + 1], Lt = [Pt + 2 * (Nt - Pt) / 3, $t + 2 * (Jt - $t) / 3], U = [vt + 2 * (Nt - vt) / 3, Yt + 2 * (Jt - Yt) / 3];
                             return Et.push([
-                                [Pt, $t], Lt, j, [vt, Yt]
+                                [Pt, $t], Lt, U, [vt, Yt]
                             ]), Et;
                         }, z = new WeakSet(), ae = function() {
                             if (this.isEmpty()) {
                                 J(this, rt, De).call(this);
                                 return;
                             }
-                            J(this, U, dn).call(this);
+                            J(this, j, dn).call(this);
                             const {
                                 canvas: et,
                                 ctx: Et
                             } = this;
                             Et.setTransform(1, 0, 0, 1, 0, 0), Et.clearRect(0, 0, et.width, et.height), J(this, rt, De).call(this);
                             for (const Ot of this.bezierPath2D)
                                 Et.stroke(Ot);
@@ -17311,19 +17311,19 @@
                             return et;
                         }, zt = new WeakSet(), Jn = function(et, Et, Ot, Pt) {
                             var Yt, Lt;
                             const $t = [],
                                 Nt = this.thickness / 2,
                                 Jt = et * Et + Nt,
                                 vt = et * Ot + Nt;
-                            for (const j of this.paths) {
+                            for (const U of this.paths) {
                                 const c = [],
                                     L = [];
-                                for (let q = 0, K = j.length; q < K; q++) {
-                                    const [tt, ct, bt, Mt] = j[q], Ft = et * tt[0] + Jt, Ht = et * tt[1] + vt, xt = et * ct[0] + Jt, Dt = et * ct[1] + vt, Ut = et * bt[0] + Jt, Xt = et * bt[1] + vt, Kt = et * Mt[0] + Jt, Zt = et * Mt[1] + vt;
+                                for (let q = 0, K = U.length; q < K; q++) {
+                                    const [tt, ct, bt, Mt] = U[q], Ft = et * tt[0] + Jt, Ht = et * tt[1] + vt, xt = et * ct[0] + Jt, Dt = et * ct[1] + vt, Ut = et * bt[0] + Jt, Xt = et * bt[1] + vt, Kt = et * Mt[0] + Jt, Zt = et * Mt[1] + vt;
                                     q === 0 && (c.push(Ft, Ht), L.push(Ft, Ht)), c.push(xt, Dt, Ut, Xt, Kt, Zt), L.push(xt, Dt), q === K - 1 && L.push(Kt, Zt);
                                 }
                                 $t.push({
                                     bezier: J(Yt = wt, Tt, _n).call(Yt, c, Pt, this.rotation),
                                     points: J(Lt = wt, Tt, _n).call(Lt, L, Pt, this.rotation)
                                 });
                             }
@@ -18069,15 +18069,15 @@
         "click",
         /*next_page*/
         i[18]
     ), {
         c() {
             create_component(t.$$.fragment), n = space(), e = element("div"), s = element("canvas"), p = space(), f = element("div"), create_component(A.$$.fragment), a = space(), h = element("span"), o = text(
                 /*currentPage*/
-                i[15]
+                i[14]
             ), F = text(" / "), R = text(
                 /*numPages*/
                 i[13]
             ), w = space(), create_component(T.$$.fragment), attr(e, "class", "pdf-canvas svelte-qxsbof"), set_style(
                 e,
                 "height",
                 /*height*/
@@ -18100,18 +18100,18 @@
                 );
             const E = {};
             C & /*$$scope*/
                 536870912 && (E.$$scope = {
                     dirty: C,
                     ctx: m
                 }), A.$set(E), (!P || C & /*currentPage*/
-                    32768) && set_data(
+                    16384) && set_data(
                     o,
                     /*currentPage*/
-                    m[15]
+                    m[14]
                 ), (!P || C & /*numPages*/
                     8192) && set_data(
                     R,
                     /*numPages*/
                     m[13]
                 );
             const S = {};
@@ -18325,15 +18325,15 @@
             destroy_component(t, e);
         }
     };
 }
 
 function instance(i, t, n) {
     let e;
-    var s = this && this.__awaiter || function(U, G, V, H) {
+    var s = this && this.__awaiter || function(j, G, V, H) {
         function st(dt) {
             return dt instanceof V ? dt : new V(function(yt) {
                 yt(dt);
             });
         }
         return new(V || (V = Promise))(function(dt, yt) {
             function gt(u) {
@@ -18351,15 +18351,15 @@
                     yt(d);
                 }
             }
 
             function l(u) {
                 u.done ? dt(u.value) : st(u.value).then(gt, k);
             }
-            l((H = H.apply(U, G || [])).next());
+            l((H = H.apply(j, G || [])).next());
         });
     };
     let {
         elem_id: p = ""
     } = t, {
         elem_classes: f = []
     } = t, {
@@ -18395,65 +18395,66 @@
 
     function M() {
         return s(this, void 0, void 0, function*() {
             n(12, E = null), yield tick(), x.dispatch("change");
         });
     }
 
-    function _(U) {
+    function _(j) {
         return s(this, arguments, void 0, function*({
             detail: G
         }) {
             n(0, a = G), yield tick(), x.dispatch("change"), x.dispatch("upload");
         });
     }
 
-    function N(U) {
+    function N(j) {
         return s(this, void 0, void 0, function*() {
-            g = yield pdfExports.getDocument(U.url).promise, n(13, v = g.numPages), D();
+            g = yield pdfExports.getDocument(j.url).promise, n(13, v = g.numPages), n(14, e = Math.min(Math.max(w, 1), v)), D(e);
         });
     }
 
-    function D() {
-        g.getPage(e).then((U) => {
-            const G = $.getContext("2d");
-            G.clearRect(0, 0, $.width, $.height);
-            let V = U.getViewport({
+    function D(j) {
+        console.log("current Page here", j), g.getPage(j).then((G) => {
+            const V = $.getContext("2d");
+            V.clearRect(0, 0, $.width, $.height);
+            let H = G.getViewport({
                     scale: 1
                 }),
-                H = R / V.height;
-            V = U.getViewport({
-                scale: H
+                st = R / H.height;
+            H = G.getViewport({
+                scale: st
             });
-            const st = {
-                canvasContext: G,
-                viewport: V
+            const dt = {
+                canvasContext: V,
+                viewport: H
             };
-            n(14, $.width = V.width, $), n(14, $.height = V.height, $), U.render(st);
+            n(15, $.width = H.width, $), n(15, $.height = H.height, $), G.render(dt);
         });
     }
 
     function X() {
-        e >= v || (n(15, e++, e), D());
+        e >= v || (n(14, e++, e), D(e));
     }
 
     function Y() {
-        e != 1 && (n(15, e--, e), D());
+        e != 1 && (n(14, e--, e), D(e));
     }
 
-    function I(U) {
-        binding_callbacks[U ? "unshift" : "push"](() => {
-            $ = U, n(14, $);
+    function I(j) {
+        binding_callbacks[j ? "unshift" : "push"](() => {
+            $ = j, n(15, $);
         });
     }
-    return i.$$set = (U) => {
-        "elem_id" in U && n(2, p = U.elem_id), "elem_classes" in U && n(3, f = U.elem_classes), "visible" in U && n(4, A = U.visible), "value" in U && n(0, a = U.value), "container" in U && n(5, h = U.container), "scale" in U && n(6, o = U.scale), "root" in U && n(7, F = U.root), "height" in U && n(1, R = U.height), "starting_page" in U && n(20, w = U.starting_page), "label" in U && n(8, T = U.label), "proxy_url" in U && n(21, P = U.proxy_url), "min_width" in U && n(9, m = U.min_width), "loading_status" in U && n(10, C = U.loading_status), "gradio" in U && n(11, x = U.gradio);
+    return i.$$set = (j) => {
+        "elem_id" in j && n(2, p = j.elem_id), "elem_classes" in j && n(3, f = j.elem_classes), "visible" in j && n(4, A = j.visible), "value" in j && n(0, a = j.value), "container" in j && n(5, h = j.container), "scale" in j && n(6, o = j.scale), "root" in j && n(7, F = j.root), "height" in j && n(1, R = j.height), "starting_page" in j && n(20, w = j.starting_page), "label" in j && n(8, T = j.label), "proxy_url" in j && n(21, P = j.proxy_url), "min_width" in j && n(9, m = j.min_width), "loading_status" in j && n(10, C = j.loading_status), "gradio" in j && n(11, x = j.gradio);
     }, i.$$.update = () => {
         i.$$.dirty & /*starting_page, numPages*/
-            1056768 && n(15, e = Math.min(Math.max(w, 1), v)), i.$$.dirty & /*height*/
+            1056768 && n(14, e = Math.min(Math.max(w, 1), v)), i.$$.dirty & /*currentPage*/
+            16384 && console.log("currentPage", e), i.$$.dirty & /*height*/
             2 && n(1, R = R || 500), i.$$.dirty & /*value, root, proxy_url*/
             2097281 && n(12, E = normalise_file(a, F, P)), i.$$.dirty & /*old_value, _value, gradio*/
             4200448 && JSON.stringify(S) != JSON.stringify(E) && (E && N(E), n(22, S = E), x.dispatch("change"));
     }, [
         a,
         R,
         p,
@@ -18464,16 +18465,16 @@
         F,
         T,
         m,
         C,
         x,
         E,
         v,
-        $,
         e,
+        $,
         M,
         _,
         X,
         Y,
         w,
         P,
         S,
```

### Comparing `gradio_pdf-0.0.8/backend/gradio_pdf/templates/component/style.css` & `gradio_pdf-0.0.9/backend/gradio_pdf/templates/component/style.css`

 * *Files identical despite different names*

### Comparing `gradio_pdf-0.0.8/backend/gradio_pdf/templates/component/wrapper-98f94c21-DqR3tIm1.js` & `gradio_pdf-0.0.9/backend/gradio_pdf/templates/component/wrapper-98f94c21-D4kvqJe-.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     r as S
-} from "./Index-BYwJN1i6.js";
+} from "./Index--Ld6fSuw.js";
 
 function z(s) {
     return s && s.__esModule && Object.prototype.hasOwnProperty.call(s, "default") ? s.default : s;
 }
 
 function gt(s) {
     if (s.__esModule)
```

### Comparing `gradio_pdf-0.0.8/backend/gradio_pdf/templates/example/index.js` & `gradio_pdf-0.0.9/backend/gradio_pdf/templates/example/index.js`

 * *Files identical despite different names*

### Comparing `gradio_pdf-0.0.8/demo/_app.py` & `gradio_pdf-0.0.9/demo/_app.py`

 * *Files identical despite different names*

### Comparing `gradio_pdf-0.0.8/demo/app.py` & `gradio_pdf-0.0.9/demo/app.py`

 * *Files identical despite different names*

### Comparing `gradio_pdf-0.0.8/demo/contract.pdf` & `gradio_pdf-0.0.9/demo/contract.pdf`

 * *Files identical despite different names*

### Comparing `gradio_pdf-0.0.8/demo/css.css` & `gradio_pdf-0.0.9/demo/css.css`

 * *Files identical despite different names*

### Comparing `gradio_pdf-0.0.8/demo/invoice_2.pdf` & `gradio_pdf-0.0.9/demo/invoice_2.pdf`

 * *Files identical despite different names*

### Comparing `gradio_pdf-0.0.8/demo/sample_invoice.pdf` & `gradio_pdf-0.0.9/demo/sample_invoice.pdf`

 * *Files identical despite different names*

### Comparing `gradio_pdf-0.0.8/demo/space.py` & `gradio_pdf-0.0.9/demo/space.py`

 * *Files identical despite different names*

### Comparing `gradio_pdf-0.0.8/frontend/Example.svelte` & `gradio_pdf-0.0.9/frontend/Example.svelte`

 * *Files identical despite different names*

### Comparing `gradio_pdf-0.0.8/frontend/Index.svelte` & `gradio_pdf-0.0.9/frontend/Index.svelte`

 * *Files 9% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 		let _value = value;
 		let old_value = _value;
 		let pdfDoc;
 		let numPages = 1;
 		let canvasRef;
 
 		$: currentPage = Math.min(Math.max(starting_page, 1), numPages);
+		$: console.log("currentPage", currentPage);
 
 		async function handle_clear() {
 			_value = null;
 			await tick();
 			gradio.dispatch("change");
 		}
 
@@ -54,19 +55,21 @@
 		}
 
 
 		async function get_doc(value: FileData) {
 			const loadingTask = pdfjsLib.getDocument(value.url);
 			pdfDoc = await loadingTask.promise;
 			numPages = pdfDoc.numPages;
-			render_page();
+			currentPage = Math.min(Math.max(starting_page, 1), numPages)
+			render_page(currentPage);
 		}
 
-		function render_page() {
+		function render_page(currentPage) {
 		// Render a specific page of the PDF onto the canvas
+			console.log("current Page here", currentPage);
 			pdfDoc.getPage(currentPage).then(page => {
 				const ctx  = canvasRef.getContext('2d')
 				ctx.clearRect(0, 0, canvasRef.width, canvasRef.height);
 				let viewport = page.getViewport({ scale: 1 });
 				let scale = height / viewport.height;
 				viewport = page.getViewport({ scale: scale });
 
@@ -81,23 +84,23 @@
 		}
 
 		function next_page() {
 			if (currentPage >= numPages) {
 				return;
 			}
 			currentPage++;
-			render_page();
+			render_page(currentPage);
 		}
 
 		function prev_page() {
 			if (currentPage == 1) {
 				return;
 			}
 			currentPage--;
-			render_page();
+			render_page(currentPage);
 		}
 
 		$: height = height || 500;
 		
 		// Compute the url to fetch the file from the backend\
 		// whenever a new value is passed in.
 		$: _value = normalise_file(value, root, proxy_url);
```

### Comparing `gradio_pdf-0.0.8/frontend/PdfUploadText.svelte` & `gradio_pdf-0.0.9/frontend/PdfUploadText.svelte`

 * *Files identical despite different names*

### Comparing `gradio_pdf-0.0.8/frontend/package-lock.json` & `gradio_pdf-0.0.9/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `gradio_pdf-0.0.8/frontend/package.json` & `gradio_pdf-0.0.9/frontend/package.json`

 * *Files identical despite different names*

### Comparing `gradio_pdf-0.0.8/LICENSE` & `gradio_pdf-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gradio_pdf-0.0.8/README.md` & `gradio_pdf-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `gradio_pdf-0.0.8/pyproject.toml` & `gradio_pdf-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "gradio_pdf"
-version = "0.0.8"
+version = "0.0.9"
 description = "Easily display PDFs in Gradio"
 readme = "README.md"
 license = "Apache-2.0"
 requires-python = ">=3.8"
 authors = [{ name = "Freddy Boulton", email = "alfonsoboulton@gmail.com" }]
 keywords = [
   "Documents",
```

### Comparing `gradio_pdf-0.0.8/PKG-INFO` & `gradio_pdf-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gradio_pdf
-Version: 0.0.8
+Version: 0.0.9
 Summary: Easily display PDFs in Gradio
 Project-URL: repository, https://github.com/freddyaboulton/gradio-pdf
 Project-URL: space, https://huggingface.co/spaces/freddyaboulton/gradio_pdf
 Author-email: Freddy Boulton <alfonsoboulton@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: Document QA,Documents,PDF,gradio,gradio custom component,gradio-template-Fallback
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: gradio_pdf Version: 0.0.8 Summary: Easily display
+Metadata-Version: 2.3 Name: gradio_pdf Version: 0.0.9 Summary: Easily display
 PDFs in Gradio Project-URL: repository, https://github.com/freddyaboulton/
 gradio-pdf Project-URL: space, https://huggingface.co/spaces/freddyaboulton/
 gradio_pdf Author-email: Freddy Boulton
 gmail.com> License-Expression: Apache-2.0 License-File: LICENSE Keywords:
 Document QA,Documents,PDF,gradio,gradio custom component,gradio-template-
 Fallback Classifier: Development Status :: 3 - Alpha Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
```

