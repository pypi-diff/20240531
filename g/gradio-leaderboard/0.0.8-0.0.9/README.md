# Comparing `tmp/gradio_leaderboard-0.0.8.tar.gz` & `tmp/gradio_leaderboard-0.0.9.tar.gz`

## Comparing `gradio_leaderboard-0.0.8.tar` & `gradio_leaderboard-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/backend/gradio_leaderboard/__init__.py
--rw-r--r--   0        0        0    19251 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/backend/gradio_leaderboard/leaderboard.py
--rw-r--r--   0        0        0    34570 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/backend/gradio_leaderboard/leaderboard.pyi
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/backend/gradio_leaderboard/templates/component/__vite-browser-external-2447137e.js
--rw-r--r--   0        0        0  1006163 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/backend/gradio_leaderboard/templates/component/index.js
--rw-r--r--   0        0        0  1498407 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/backend/gradio_leaderboard/templates/component/style.css
--rw-r--r--   0        0        0    78062 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/backend/gradio_leaderboard/templates/component/wrapper-6f348d45-19fa94bf.js
--rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/backend/gradio_leaderboard/templates/example/index.js
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/backend/gradio_leaderboard/templates/example/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/demo/__init__.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/demo/app.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/demo/config.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/demo/css.css
--rw-r--r--   0        0        0    15319 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/demo/docs.md
--rw-r--r--   0        0        0   227857 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/demo/leaderboard_data.json
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/demo/space.py
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/frontend/Example.svelte
--rw-r--r--   0        0        0    11519 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/frontend/Index.svelte
--rw-r--r--   0        0        0    50149 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/frontend/package-lock.json
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/frontend/package.json
--rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/frontend/shared/Checkboxgroup.svelte
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/frontend/shared/EditableCell.svelte
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/frontend/shared/Example.svelte
--rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/frontend/shared/RangeSlider.svelte
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/frontend/shared/SimpleTextbox.svelte
--rw-r--r--   0        0        0    24334 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/frontend/shared/Table.svelte
--rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/frontend/shared/VirtualTable.svelte
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/frontend/shared/utils.ts
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/.gitignore
--rw-r--r--   0        0        0    14779 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/README.md
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    15901 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/backend/gradio_leaderboard/__init__.py
+-rw-r--r--   0        0        0    19251 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/backend/gradio_leaderboard/leaderboard.py
+-rw-r--r--   0        0        0    34570 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/backend/gradio_leaderboard/leaderboard.pyi
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/backend/gradio_leaderboard/templates/component/__vite-browser-external-2447137e.js
+-rw-r--r--   0        0        0  1006286 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/backend/gradio_leaderboard/templates/component/index.js
+-rw-r--r--   0        0        0  1498407 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/backend/gradio_leaderboard/templates/component/style.css
+-rw-r--r--   0        0        0    78062 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/backend/gradio_leaderboard/templates/component/wrapper-6f348d45-19fa94bf.js
+-rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/backend/gradio_leaderboard/templates/example/index.js
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/backend/gradio_leaderboard/templates/example/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/demo/__init__.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/demo/app.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/demo/config.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/demo/css.css
+-rw-r--r--   0        0        0    15319 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/demo/docs.md
+-rw-r--r--   0        0        0   227857 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/demo/leaderboard_data.json
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/demo/space.py
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/frontend/Example.svelte
+-rw-r--r--   0        0        0    11598 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/frontend/Index.svelte
+-rw-r--r--   0        0        0    50149 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/frontend/package-lock.json
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/frontend/package.json
+-rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/frontend/shared/Checkboxgroup.svelte
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/frontend/shared/EditableCell.svelte
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/frontend/shared/Example.svelte
+-rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/frontend/shared/RangeSlider.svelte
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/frontend/shared/SimpleTextbox.svelte
+-rw-r--r--   0        0        0    24334 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/frontend/shared/Table.svelte
+-rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/frontend/shared/VirtualTable.svelte
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/frontend/shared/utils.ts
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/.gitignore
+-rw-r--r--   0        0        0    14779 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/README.md
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    15901 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.9/PKG-INFO
```

### Comparing `gradio_leaderboard-0.0.8/backend/gradio_leaderboard/leaderboard.py` & `gradio_leaderboard-0.0.9/backend/gradio_leaderboard/leaderboard.py`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.8/backend/gradio_leaderboard/leaderboard.pyi` & `gradio_leaderboard-0.0.9/backend/gradio_leaderboard/leaderboard.pyi`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.8/backend/gradio_leaderboard/templates/component/index.js` & `gradio_leaderboard-0.0.9/backend/gradio_leaderboard/templates/component/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1464,15 +1464,15 @@
     async function l(c, u = {}) {
         return new Promise(async (h) => {
             const {
                 status_callback: p,
                 hf_token: _
             } = u, v = {
                 predict: Ne,
-                submit: ke,
+                submit: ve,
                 view_api: Be,
                 component_server: le
             };
             if ((typeof window > "u" || !("WebSocket" in window)) && !global.Websocket) {
                 const oe = await import("./wrapper-6f348d45-19fa94bf.js");
                 Af = (await import("./__vite-browser-external-2447137e.js")).Blob, global.WebSocket = oe.WebSocket;
             }
@@ -1495,16 +1495,16 @@
                 if (z = oe, window.location.protocol === "https:" && (z.root = z.root.replace("http://", "https://")), Y = km((oe == null ? void 0 : oe.dependencies) || []), z.auth_required)
                     return {
                         config: z,
                         ...v
                     };
                 try {
                     pe = await Be(z);
-                } catch (Q) {
-                    console.error(`Could not get api details: ${Q.message}`);
+                } catch (K) {
+                    console.error(`Could not get api details: ${K.message}`);
                 }
                 return {
                     config: z,
                     ...v
                 };
             }
             let pe;
@@ -1512,33 +1512,33 @@
                 if (p && p(oe), oe.status === "running")
                     try {
                         z = await Pu(
                             t,
                             `${T}//${O}`,
                             _
                         );
-                        const Q = await re(z);
-                        h(Q);
-                    } catch (Q) {
-                        console.error(Q), p && p({
+                        const K = await re(z);
+                        h(K);
+                    } catch (K) {
+                        console.error(K), p && p({
                             status: "error",
                             message: "Could not load this space.",
                             load_status: "error",
                             detail: "NOT_FOUND"
                         });
                     }
             }
             try {
                 z = await Pu(
                     t,
                     `${T}//${O}`,
                     _
                 );
                 const oe = await re(z),
-                    Q = new EventSource(
+                    K = new EventSource(
                         `${z.root}/heartbeat/${U}`
                     );
                 h(oe);
             } catch (oe) {
                 console.error(oe), P ? oa(
                     P,
                     kf.test(P) ? "space_name" : "subdomain",
@@ -1547,58 +1547,58 @@
                     status: "error",
                     message: "Could not load this space.",
                     load_status: "error",
                     detail: "NOT_FOUND"
                 });
             }
 
-            function Ne(oe, Q, de) {
+            function Ne(oe, K, de) {
                 let V = !1,
                     ee = !1,
                     we;
                 if (typeof oe == "number")
                     we = z.dependencies[oe];
                 else {
-                    const ve = oe.replace(/^\//, "");
-                    we = z.dependencies[Y[ve]];
+                    const ke = oe.replace(/^\//, "");
+                    we = z.dependencies[Y[ke]];
                 }
                 if (we.types.continuous)
                     throw new Error(
                         "Cannot call predict on this function as it may run forever. Use submit instead"
                     );
-                return new Promise((ve, $) => {
-                    const xe = ke(oe, Q, de);
+                return new Promise((ke, $) => {
+                    const xe = ve(oe, K, de);
                     let Se;
                     xe.on("data", (We) => {
-                        ee && (xe.destroy(), ve(We)), V = !0, Se = We;
+                        ee && (xe.destroy(), ke(We)), V = !0, Se = We;
                     }).on("status", (We) => {
-                        We.stage === "error" && $(We), We.stage === "complete" && (ee = !0, V && (xe.destroy(), ve(Se)));
+                        We.stage === "error" && $(We), We.stage === "complete" && (ee = !0, V && (xe.destroy(), ke(Se)));
                     });
                 });
             }
 
-            function ke(oe, Q, de, V = null) {
+            function ve(oe, K, de, V = null) {
                 let ee, we;
                 if (typeof oe == "number")
                     ee = oe, we = pe.unnamed_endpoints[ee];
                 else {
                     const ye = oe.replace(/^\//, "");
                     ee = Y[ye], we = pe.named_endpoints[oe.trim()];
                 }
                 if (typeof ee != "number")
                     throw new Error(
                         "There is no endpoint matching that name of fn_index matching that number."
                     );
-                let ve, $, xe = z.protocol ?? "ws";
+                let ke, $, xe = z.protocol ?? "ws";
                 const Se = typeof oe == "number" ? "/predict" : oe;
                 let We, Ie = null,
                     Xe = !1;
                 const Ue = {};
                 let zt = "";
-                typeof window < "u" && (zt = new URLSearchParams(window.location.search).toString()), o(`${z.root}`, Q, we, _).then(
+                typeof window < "u" && (zt = new URLSearchParams(window.location.search).toString()), o(`${z.root}`, K, we, _).then(
                     (ye) => {
                         if (We = {
                                 data: ye || [],
                                 event_data: de,
                                 fn_index: ee,
                                 trigger_id: V
                             }, Bm(ee, z))
@@ -1662,26 +1662,26 @@
                             });
                             let Ee = new URL(`${k}://${vf(
                 O,
                 z.path,
                 !0
               )}
 							/queue/join${zt ? "?" + zt : ""}`);
-                            ne && Ee.searchParams.set("__sign", ne), ve = new WebSocket(Ee), ve.onclose = (me) => {
+                            ne && Ee.searchParams.set("__sign", ne), ke = new WebSocket(Ee), ke.onclose = (me) => {
                                 me.wasClean || Re({
                                     type: "status",
                                     stage: "error",
                                     broken: !0,
                                     message: j0,
                                     queue: !0,
                                     endpoint: Se,
                                     fn_index: ee,
                                     time: /* @__PURE__ */ new Date()
                                 });
-                            }, ve.onmessage = function(me) {
+                            }, ke.onmessage = function(me) {
                                 const Oe = JSON.parse(me.data),
                                     {
                                         type: et,
                                         status: Ce,
                                         data: Le
                                     } = Ll(
                                         Oe,
@@ -1690,23 +1690,23 @@
                                 if (et === "update" && Ce && !Xe)
                                     Re({
                                         type: "status",
                                         endpoint: Se,
                                         fn_index: ee,
                                         time: /* @__PURE__ */ new Date(),
                                         ...Ce
-                                    }), Ce.stage === "error" && ve.close();
+                                    }), Ce.stage === "error" && ke.close();
                                 else if (et === "hash") {
-                                    ve.send(JSON.stringify({
+                                    ke.send(JSON.stringify({
                                         fn_index: ee,
                                         session_hash: U
                                     }));
                                     return;
                                 } else
-                                    et === "data" ? ve.send(JSON.stringify({
+                                    et === "data" ? ke.send(JSON.stringify({
                                         ...We,
                                         session_hash: U
                                     })) : et === "complete" ? Xe = Ce : et === "log" ? Re({
                                         type: "log",
                                         log: Le.log,
                                         level: Le.level,
                                         endpoint: Se,
@@ -1730,18 +1730,18 @@
                                     type: "status",
                                     time: /* @__PURE__ */ new Date(),
                                     ...Xe,
                                     stage: Ce == null ? void 0 : Ce.stage,
                                     queue: !0,
                                     endpoint: Se,
                                     fn_index: ee
-                                }), ve.close()));
+                                }), ke.close()));
                             }, Ru(z.version || "2.0.0", "3.6") < 0 && addEventListener(
                                 "open",
-                                () => ve.send(JSON.stringify({
+                                () => ke.send(JSON.stringify({
                                     hash: U
                                 }))
                             );
                         } else if (xe == "sse") {
                             Re({
                                 type: "status",
                                 stage: "pending",
@@ -1939,15 +1939,15 @@
                                                 fn_index: ee,
                                                 time: /* @__PURE__ */ new Date()
                                             }), ["sse_v2", "sse_v2.1"].includes(xe) && he();
                                         }
                                     };
                                     Ie in D && (D[Ie].forEach(
                                         (et) => Oe(et)
-                                    ), delete D[Ie]), R[Ie] = Oe, I.add(Ie), N || ce();
+                                    ), delete D[Ie]), R[Ie] = Oe, I.add(Ie), N || ue();
                                 }
                             }));
                     }
                 );
 
                 function Nn(ye, Fe) {
                     !E[ye] ? (E[ye] = [], Fe.data.forEach((me, Oe) => {
@@ -1969,26 +1969,26 @@
                 function $t(ye, Fe) {
                     const Ee = Ue,
                         me = Ee[ye] || [];
                     return Ee[ye] = me, me == null || me.push(Fe), {
                         on: $t,
                         off: Ot,
                         cancel: Ct,
-                        destroy: K
+                        destroy: Q
                     };
                 }
 
                 function Ot(ye, Fe) {
                     const Ee = Ue;
                     let me = Ee[ye] || [];
                     return me = me == null ? void 0 : me.filter((Oe) => Oe !== Fe), Ee[ye] = me, {
                         on: $t,
                         off: Ot,
                         cancel: Ct,
-                        destroy: K
+                        destroy: Q
                     };
                 }
                 async function Ct() {
                     const ye = {
                         stage: "complete",
                         queue: !1,
                         time: /* @__PURE__ */ new Date()
@@ -1996,17 +1996,17 @@
                     Xe = ye, Re({
                         ...ye,
                         type: "status",
                         endpoint: Se,
                         fn_index: ee
                     });
                     let Fe = {};
-                    xe === "ws" ? (ve && ve.readyState === 0 ? ve.addEventListener("open", () => {
-                        ve.close();
-                    }) : ve.close(), Fe = {
+                    xe === "ws" ? (ke && ke.readyState === 0 ? ke.addEventListener("open", () => {
+                        ke.close();
+                    }) : ke.close(), Fe = {
                         fn_index: ee,
                         session_hash: U
                     }) : ($.close(), Fe = {
                         event_id: Ie
                     });
                     try {
                         await t(`${z.root}/reset`, {
@@ -2019,35 +2019,35 @@
                     } catch {
                         console.warn(
                             "The `/reset` endpoint could not be called. Subsequent endpoint results may be unreliable."
                         );
                     }
                 }
 
-                function K() {
+                function Q() {
                     for (const ye in Ue)
                         Ue[ye].forEach((Fe) => {
                             Ot(ye, Fe);
                         });
                 }
                 return {
                     on: $t,
                     off: Ot,
                     cancel: Ct,
-                    destroy: K
+                    destroy: Q
                 };
             }
 
-            function ce() {
+            function ue() {
                 N = !0;
                 let oe = new URLSearchParams({
                         session_hash: U
                     }).toString(),
-                    Q = new URL(`${z.root}/queue/data?${oe}`);
-                C = e(Q), C.onmessage = async function(de) {
+                    K = new URL(`${z.root}/queue/data?${oe}`);
+                C = e(K), C.onmessage = async function(de) {
                     let V = JSON.parse(de.data);
                     if (V.msg === "close_stream") {
                         he();
                         return;
                     }
                     const ee = V.event_id;
                     if (!ee)
@@ -2073,61 +2073,61 @@
                     ), he();
                 };
             }
 
             function he() {
                 N = !1, C == null || C.close();
             }
-            async function le(oe, Q, de) {
+            async function le(oe, K, de) {
                 var V;
                 const ee = {
                     "Content-Type": "application/json"
                 };
                 _ && (ee.Authorization = `Bearer ${_}`);
-                let we, ve = z.components.find(
+                let we, ke = z.components.find(
                     (Se) => Se.id === oe
                 );
-                (V = ve == null ? void 0 : ve.props) != null && V.root_url ? we = ve.props.root_url : we = z.root;
+                (V = ke == null ? void 0 : ke.props) != null && V.root_url ? we = ke.props.root_url : we = z.root;
                 const $ = await t(
                     `${we}/component_server/`, {
                         method: "POST",
                         body: JSON.stringify({
                             data: de,
                             component_id: oe,
-                            fn_name: Q,
+                            fn_name: K,
                             session_hash: U
                         }),
                         headers: ee
                     }
                 );
                 if (!$.ok)
                     throw new Error(
                         "Could not connect to component server: " + $.statusText
                     );
                 return await $.json();
             }
             async function Be(oe) {
                 if (pe)
                     return pe;
-                const Q = {
+                const K = {
                     "Content-Type": "application/json"
                 };
-                _ && (Q.Authorization = `Bearer ${_}`);
+                _ && (K.Authorization = `Bearer ${_}`);
                 let de;
                 if (Ru(oe.version || "2.0.0", "3.30") < 0 ? de = await t(
                         "https://gradio-space-api-fetcher-v2.hf.space/api", {
                             method: "POST",
                             body: JSON.stringify({
                                 serialize: !1,
                                 config: JSON.stringify(oe)
                             }),
-                            headers: Q
+                            headers: K
                         }
                     ) : de = await t(`${oe.root}/info`, {
-                        headers: Q
+                        headers: K
                     }), !de.ok)
                     throw new Error(j0);
                 let V = await de.json();
                 return "api" in V && (V = V.api), V.named_endpoints["/predict"] && !V.unnamed_endpoints[0] && (V.unnamed_endpoints[0] = V.named_endpoints["/predict"]), Cm(V, oe, Y);
             }
         });
     }
@@ -6821,18 +6821,18 @@
     function z() {
         n(18, c = !c);
     }
 
     function Y() {
         navigator.clipboard.read().then(async (V) => {
             for (let ee = 0; ee < V.length; ee++) {
-                const we = V[ee].types.find((ve) => ve.startsWith("image/"));
+                const we = V[ee].types.find((ke) => ke.startsWith("image/"));
                 if (we) {
-                    V[ee].getType(we).then(async (ve) => {
-                        const $ = new File([ve], `clipboard.${we.replace("image/", "")}`);
+                    V[ee].getType(we).then(async (ke) => {
+                        const $ = new File([ke], `clipboard.${we.replace("image/", "")}`);
                         await pe([$]);
                     });
                     break;
                 }
             }
         });
     }
@@ -6866,25 +6866,25 @@
                 C("load", ee.files);
             }
     }
     async function Ne(V) {
         if (n(18, c = !1), !cc([V, "access", (we) => we.dataTransfer, "optionalAccess", (we) => we.files]))
             return;
         const ee = Array.from(V.dataTransfer.files).filter((we) => {
-            const ve = "." + we.name.split(".").pop();
-            return ve && Q3(D, ve, we.type) || (ve && Array.isArray(o) ? o.includes(ve) : ve === o) ? !0 : (C("error", `Invalid file type only ${o} allowed.`), !1);
+            const ke = "." + we.name.split(".").pop();
+            return ke && Q3(D, ke, we.type) || (ke && Array.isArray(o) ? o.includes(ke) : ke === o) ? !0 : (C("error", `Invalid file type only ${o} allowed.`), !1);
         });
         await pe(ee);
     }
 
-    function ke(V) {
+    function ve(V) {
         V0.call(this, t, V);
     }
 
-    function ce(V) {
+    function ue(V) {
         V0.call(this, t, V);
     }
 
     function he(V) {
         V0.call(this, t, V);
     }
 
@@ -6896,15 +6896,15 @@
         V0.call(this, t, V);
     }
 
     function oe(V) {
         V0.call(this, t, V);
     }
 
-    function Q(V) {
+    function K(V) {
         V0.call(this, t, V);
     }
 
     function de(V) {
         O3[V ? "unshift" : "push"](() => {
             U = V, n(2, U);
         });
@@ -6934,21 +6934,21 @@
         Me,
         Ne,
         c,
         O,
         pe,
         l,
         r,
-        ke,
-        ce,
+        ve,
+        ue,
         he,
         le,
         Be,
         oe,
-        Q,
+        K,
         de
     ];
 }
 class $3 extends R3 {
     constructor(e) {
         super(), H3(
             this,
@@ -7586,15 +7586,15 @@
         } catch {
             return console.warn("TrustedTypes policy " + o + " could not be created."), null;
         }
     };
 
 function bh() {
     let t = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : Fp();
-    const e = (ue) => bh(ue);
+    const e = (ce) => bh(ce);
     if (e.version = "3.1.0", e.removed = [], !t || !t.document || t.document.nodeType !== 9)
         return e.isSupported = !1, e;
     let {
         document: n
     } = t;
     const r = n,
         l = r.currentScript,
@@ -7611,16 +7611,16 @@
         } = t,
         O = h.prototype,
         P = Xs(O, "cloneNode"),
         U = Xs(O, "nextSibling"),
         M = Xs(O, "childNodes"),
         N = Xs(O, "parentNode");
     if (typeof c == "function") {
-        const ue = n.createElement("template");
-        ue.content && ue.content.ownerDocument && (n = ue.content.ownerDocument);
+        const ce = n.createElement("template");
+        ce.content && ce.content.ownerDocument && (n = ce.content.ownerDocument);
     }
     let D, E = "";
     const {
         implementation: C,
         createNodeIterator: R,
         createDocumentFragment: I,
         getElementsByTagName: z
@@ -7630,23 +7630,23 @@
     let ne = {};
     e.isSupported = typeof mh == "function" && typeof N == "function" && C && C.createHTMLDocument !== void 0;
     const {
         MUSTACHE_EXPR: re,
         ERB_EXPR: pe,
         TMPLIT_EXPR: Me,
         DATA_ATTR: Ne,
-        ARIA_ATTR: ke,
-        IS_SCRIPT_OR_DATA: ce,
+        ARIA_ATTR: ve,
+        IS_SCRIPT_OR_DATA: ue,
         ATTR_WHITESPACE: he,
         CUSTOM_ELEMENT: le
     } = yc;
     let {
         IS_ALLOWED_URI: Be
     } = yc, oe = null;
-    const Q = Ve({}, [...gc, ...Xl, ...Yl, ...Zl, ..._c]);
+    const K = Ve({}, [...gc, ...Xl, ...Yl, ...Zl, ..._c]);
     let de = null;
     const V = Ve({}, [...bc, ...Jl, ...wc, ...Ys]);
     let ee = Object.seal(ph(null, {
             tagNameCheck: {
                 writable: !0,
                 configurable: !1,
                 enumerable: !0,
@@ -7662,29 +7662,29 @@
                 writable: !0,
                 configurable: !1,
                 enumerable: !0,
                 value: !1
             }
         })),
         we = null,
-        ve = null,
+        ke = null,
         $ = !0,
         xe = !0,
         Se = !1,
         We = !0,
         Ie = !1,
         Xe = !0,
         Ue = !1,
         zt = !1,
         Nn = !1,
         Re = !1,
         $t = !1,
         Ot = !1,
         Ct = !0,
-        K = !1;
+        Q = !1;
     const ye = "user-content-";
     let Fe = !0,
         Ee = !1,
         me = {},
         Oe = null;
     const et = Ve({}, ["annotation-xml", "audio", "colgroup", "desc", "foreignobject", "head", "iframe", "math", "mi", "mn", "mo", "ms", "mtext", "noembed", "noframes", "noscript", "plaintext", "script", "style", "svg", "template", "thead", "title", "video", "xmp"]);
     let Ce = null;
@@ -7707,29 +7707,29 @@
         jt = function(G) {
             return G instanceof RegExp || G instanceof Function;
         },
         en = function() {
             let G = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : {};
             if (!(qn && qn === G)) {
                 if ((!G || typeof G != "object") && (G = {}), G = Y0(G), Pn = // eslint-disable-next-line unicorn/prefer-includes
-                    sr.indexOf(G.PARSER_MEDIA_TYPE) === -1 ? i0 : G.PARSER_MEDIA_TYPE, wt = Pn === "application/xhtml+xml" ? Wl : pi, oe = Ln(G, "ALLOWED_TAGS") ? Ve({}, G.ALLOWED_TAGS, wt) : Q, de = Ln(G, "ALLOWED_ATTR") ? Ve({}, G.ALLOWED_ATTR, wt) : V, Ut = Ln(G, "ALLOWED_NAMESPACES") ? Ve({}, G.ALLOWED_NAMESPACES, Wl) : s0, tt = Ln(G, "ADD_URI_SAFE_ATTR") ? Ve(
+                    sr.indexOf(G.PARSER_MEDIA_TYPE) === -1 ? i0 : G.PARSER_MEDIA_TYPE, wt = Pn === "application/xhtml+xml" ? Wl : pi, oe = Ln(G, "ALLOWED_TAGS") ? Ve({}, G.ALLOWED_TAGS, wt) : K, de = Ln(G, "ALLOWED_ATTR") ? Ve({}, G.ALLOWED_ATTR, wt) : V, Ut = Ln(G, "ALLOWED_NAMESPACES") ? Ve({}, G.ALLOWED_NAMESPACES, Wl) : s0, tt = Ln(G, "ADD_URI_SAFE_ATTR") ? Ve(
                         Y0(Rt),
                         // eslint-disable-line indent
                         G.ADD_URI_SAFE_ATTR,
                         // eslint-disable-line indent
                         wt
                         // eslint-disable-line indent
                     ) : Rt, Ce = Ln(G, "ADD_DATA_URI_TAGS") ? Ve(
                         Y0(Le),
                         // eslint-disable-line indent
                         G.ADD_DATA_URI_TAGS,
                         // eslint-disable-line indent
                         wt
                         // eslint-disable-line indent
-                    ) : Le, Oe = Ln(G, "FORBID_CONTENTS") ? Ve({}, G.FORBID_CONTENTS, wt) : et, we = Ln(G, "FORBID_TAGS") ? Ve({}, G.FORBID_TAGS, wt) : {}, ve = Ln(G, "FORBID_ATTR") ? Ve({}, G.FORBID_ATTR, wt) : {}, me = Ln(G, "USE_PROFILES") ? G.USE_PROFILES : !1, $ = G.ALLOW_ARIA_ATTR !== !1, xe = G.ALLOW_DATA_ATTR !== !1, Se = G.ALLOW_UNKNOWN_PROTOCOLS || !1, We = G.ALLOW_SELF_CLOSE_IN_ATTR !== !1, Ie = G.SAFE_FOR_TEMPLATES || !1, Xe = G.SAFE_FOR_XML !== !1, Ue = G.WHOLE_DOCUMENT || !1, Re = G.RETURN_DOM || !1, $t = G.RETURN_DOM_FRAGMENT || !1, Ot = G.RETURN_TRUSTED_TYPE || !1, Nn = G.FORCE_BODY || !1, Ct = G.SANITIZE_DOM !== !1, K = G.SANITIZE_NAMED_PROPS || !1, Fe = G.KEEP_CONTENT !== !1, Ee = G.IN_PLACE || !1, Be = G.ALLOWED_URI_REGEXP || gh, Ze = G.NAMESPACE || It, ee = G.CUSTOM_ELEMENT_HANDLING || {}, G.CUSTOM_ELEMENT_HANDLING && jt(G.CUSTOM_ELEMENT_HANDLING.tagNameCheck) && (ee.tagNameCheck = G.CUSTOM_ELEMENT_HANDLING.tagNameCheck), G.CUSTOM_ELEMENT_HANDLING && jt(G.CUSTOM_ELEMENT_HANDLING.attributeNameCheck) && (ee.attributeNameCheck = G.CUSTOM_ELEMENT_HANDLING.attributeNameCheck), G.CUSTOM_ELEMENT_HANDLING && typeof G.CUSTOM_ELEMENT_HANDLING.allowCustomizedBuiltInElements == "boolean" && (ee.allowCustomizedBuiltInElements = G.CUSTOM_ELEMENT_HANDLING.allowCustomizedBuiltInElements), Ie && (xe = !1), $t && (Re = !0), me && (oe = Ve({}, _c), de = [], me.html === !0 && (Ve(oe, gc), Ve(de, bc)), me.svg === !0 && (Ve(oe, Xl), Ve(de, Jl), Ve(de, Ys)), me.svgFilters === !0 && (Ve(oe, Yl), Ve(de, Jl), Ve(de, Ys)), me.mathMl === !0 && (Ve(oe, Zl), Ve(de, wc), Ve(de, Ys))), G.ADD_TAGS && (oe === Q && (oe = Y0(oe)), Ve(oe, G.ADD_TAGS, wt)), G.ADD_ATTR && (de === V && (de = Y0(de)), Ve(de, G.ADD_ATTR, wt)), G.ADD_URI_SAFE_ATTR && Ve(tt, G.ADD_URI_SAFE_ATTR, wt), G.FORBID_CONTENTS && (Oe === et && (Oe = Y0(Oe)), Ve(Oe, G.FORBID_CONTENTS, wt)), Fe && (oe["#text"] = !0), Ue && Ve(oe, ["html", "head", "body"]), oe.table && (Ve(oe, ["tbody"]), delete we.tbody), G.TRUSTED_TYPES_POLICY) {
+                    ) : Le, Oe = Ln(G, "FORBID_CONTENTS") ? Ve({}, G.FORBID_CONTENTS, wt) : et, we = Ln(G, "FORBID_TAGS") ? Ve({}, G.FORBID_TAGS, wt) : {}, ke = Ln(G, "FORBID_ATTR") ? Ve({}, G.FORBID_ATTR, wt) : {}, me = Ln(G, "USE_PROFILES") ? G.USE_PROFILES : !1, $ = G.ALLOW_ARIA_ATTR !== !1, xe = G.ALLOW_DATA_ATTR !== !1, Se = G.ALLOW_UNKNOWN_PROTOCOLS || !1, We = G.ALLOW_SELF_CLOSE_IN_ATTR !== !1, Ie = G.SAFE_FOR_TEMPLATES || !1, Xe = G.SAFE_FOR_XML !== !1, Ue = G.WHOLE_DOCUMENT || !1, Re = G.RETURN_DOM || !1, $t = G.RETURN_DOM_FRAGMENT || !1, Ot = G.RETURN_TRUSTED_TYPE || !1, Nn = G.FORCE_BODY || !1, Ct = G.SANITIZE_DOM !== !1, Q = G.SANITIZE_NAMED_PROPS || !1, Fe = G.KEEP_CONTENT !== !1, Ee = G.IN_PLACE || !1, Be = G.ALLOWED_URI_REGEXP || gh, Ze = G.NAMESPACE || It, ee = G.CUSTOM_ELEMENT_HANDLING || {}, G.CUSTOM_ELEMENT_HANDLING && jt(G.CUSTOM_ELEMENT_HANDLING.tagNameCheck) && (ee.tagNameCheck = G.CUSTOM_ELEMENT_HANDLING.tagNameCheck), G.CUSTOM_ELEMENT_HANDLING && jt(G.CUSTOM_ELEMENT_HANDLING.attributeNameCheck) && (ee.attributeNameCheck = G.CUSTOM_ELEMENT_HANDLING.attributeNameCheck), G.CUSTOM_ELEMENT_HANDLING && typeof G.CUSTOM_ELEMENT_HANDLING.allowCustomizedBuiltInElements == "boolean" && (ee.allowCustomizedBuiltInElements = G.CUSTOM_ELEMENT_HANDLING.allowCustomizedBuiltInElements), Ie && (xe = !1), $t && (Re = !0), me && (oe = Ve({}, _c), de = [], me.html === !0 && (Ve(oe, gc), Ve(de, bc)), me.svg === !0 && (Ve(oe, Xl), Ve(de, Jl), Ve(de, Ys)), me.svgFilters === !0 && (Ve(oe, Yl), Ve(de, Jl), Ve(de, Ys)), me.mathMl === !0 && (Ve(oe, Zl), Ve(de, wc), Ve(de, Ys))), G.ADD_TAGS && (oe === K && (oe = Y0(oe)), Ve(oe, G.ADD_TAGS, wt)), G.ADD_ATTR && (de === V && (de = Y0(de)), Ve(de, G.ADD_ATTR, wt)), G.ADD_URI_SAFE_ATTR && Ve(tt, G.ADD_URI_SAFE_ATTR, wt), G.FORBID_CONTENTS && (Oe === et && (Oe = Y0(Oe)), Ve(Oe, G.FORBID_CONTENTS, wt)), Fe && (oe["#text"] = !0), Ue && Ve(oe, ["html", "head", "body"]), oe.table && (Ve(oe, ["tbody"]), delete we.tbody), G.TRUSTED_TYPES_POLICY) {
                     if (typeof G.TRUSTED_TYPES_POLICY.createHTML != "function")
                         throw Yr('TRUSTED_TYPES_POLICY configuration option must provide a "createHTML" hook.');
                     if (typeof G.TRUSTED_TYPES_POLICY.createScriptURL != "function")
                         throw Yr('TRUSTED_TYPES_POLICY configuration option must provide a "createScriptURL" hook.');
                     D = G.TRUSTED_TYPES_POLICY, E = D.createHTML("");
                 } else
                     D === void 0 && (D = Cp(T, l)), D !== null && typeof E == "string" && (E = D.createHTML(""));
@@ -7856,30 +7856,30 @@
             }), G.textContent !== ie && (Wr(e.removed, {
                 element: G.cloneNode()
             }), G.textContent = ie)), B("afterSanitizeElements", G, null), !1);
         },
         fe = function(G, ie, x) {
             if (Ct && (ie === "id" || ie === "name") && (x in n || x in Ir))
                 return !1;
-            if (!(xe && !ve[ie] && an(Ne, ie))) {
-                if (!($ && an(ke, ie))) {
-                    if (!de[ie] || ve[ie]) {
+            if (!(xe && !ke[ie] && an(Ne, ie))) {
+                if (!($ && an(ve, ie))) {
+                    if (!de[ie] || ke[ie]) {
                         if (
                             // First condition does a very basic check if a) it's basically a valid custom element tagname AND
                             // b) if the tagName passes whatever the user has configured for CUSTOM_ELEMENT_HANDLING.tagNameCheck
                             // and c) if the attribute name passes whatever the user has configured for CUSTOM_ELEMENT_HANDLING.attributeNameCheck
                             !(pt(G) && (ee.tagNameCheck instanceof RegExp && an(ee.tagNameCheck, G) || ee.tagNameCheck instanceof Function && ee.tagNameCheck(G)) && (ee.attributeNameCheck instanceof RegExp && an(ee.attributeNameCheck, ie) || ee.attributeNameCheck instanceof Function && ee.attributeNameCheck(ie)) || // Alternative, second condition checks if it's an `is`-attribute, AND
                                 // the value passes whatever the user has configured for CUSTOM_ELEMENT_HANDLING.tagNameCheck
                                 ie === "is" && ee.allowCustomizedBuiltInElements && (ee.tagNameCheck instanceof RegExp && an(ee.tagNameCheck, x) || ee.tagNameCheck instanceof Function && ee.tagNameCheck(x)))
                         )
                             return !1;
                     } else if (!tt[ie]) {
                         if (!an(Be, Xr(x, he, ""))) {
                             if (!((ie === "src" || ie === "xlink:href" || ie === "href") && G !== "script" && pp(x, "data:") === 0 && Ce[G])) {
-                                if (!(Se && !an(ce, Xr(x, he, "")))) {
+                                if (!(Se && !an(ue, Xr(x, he, "")))) {
                                     if (x)
                                         return !1;
                                 }
                             }
                         }
                     }
                 }
@@ -7919,15 +7919,15 @@
                     continue;
                 }
                 Ie && Ws([re, pe, Me], (q0) => {
                     Ae = Xr(Ae, q0, " ");
                 });
                 const or = wt(G.nodeName);
                 if (fe(or, Gn, Ae)) {
-                    if (K && (Gn === "id" || Gn === "name") && (q(Lt, G), Ae = ye + Ae), D && typeof T == "object" && typeof T.getAttributeType == "function" && !Vt)
+                    if (Q && (Gn === "id" || Gn === "name") && (q(Lt, G), Ae = ye + Ae), D && typeof T == "object" && typeof T.getAttributeType == "function" && !Vt)
                         switch (T.getAttributeType(or, Gn)) {
                             case "TrustedHTML": {
                                 Ae = D.createHTML(Ae);
                                 break;
                             }
                             case "TrustedScriptURL": {
                                 Ae = D.createScriptURL(Ae);
@@ -7937,86 +7937,86 @@
                     try {
                         Vt ? G.setAttributeNS(Vt, Lt, Ae) : G.setAttribute(Lt, Ae), mc(e.removed);
                     } catch {}
                 }
             }
             B("afterSanitizeAttributes", G, null);
         },
-        De = function ue(G) {
+        De = function ce(G) {
             let ie = null;
             const x = g(G);
             for (B("beforeSanitizeShadowDOM", G, null); ie = x.nextNode();)
-                B("uponSanitizeShadowNode", ie, null), !ze(ie) && (ie.content instanceof o && ue(ie.content), Dn(ie));
+                B("uponSanitizeShadowNode", ie, null), !ze(ie) && (ie.content instanceof o && ce(ie.content), Dn(ie));
             B("afterSanitizeShadowDOM", G, null);
         };
-    return e.sanitize = function(ue) {
+    return e.sanitize = function(ce) {
         let G = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : {},
             ie = null,
             x = null,
             Ye = null,
             H = null;
-        if (ae = !ue, ae && (ue = "<!-->"), typeof ue != "string" && !y(ue))
-            if (typeof ue.toString == "function") {
-                if (ue = ue.toString(), typeof ue != "string")
+        if (ae = !ce, ae && (ce = "<!-->"), typeof ce != "string" && !y(ce))
+            if (typeof ce.toString == "function") {
+                if (ce = ce.toString(), typeof ce != "string")
                     throw Yr("dirty is not a string, aborting");
             } else
                 throw Yr("toString is not a function");
         if (!e.isSupported)
-            return ue;
-        if (zt || en(G), e.removed = [], typeof ue == "string" && (Ee = !1), Ee) {
-            if (ue.nodeName) {
-                const Un = wt(ue.nodeName);
+            return ce;
+        if (zt || en(G), e.removed = [], typeof ce == "string" && (Ee = !1), Ee) {
+            if (ce.nodeName) {
+                const Un = wt(ce.nodeName);
                 if (!oe[Un] || we[Un])
                     throw Yr("root node is forbidden and cannot be sanitized in-place");
             }
-        } else if (ue instanceof u)
-            ie = d("<!---->"), x = ie.ownerDocument.importNode(ue, !0), x.nodeType === 1 && x.nodeName === "BODY" || x.nodeName === "HTML" ? ie = x : ie.appendChild(x);
+        } else if (ce instanceof u)
+            ie = d("<!---->"), x = ie.ownerDocument.importNode(ce, !0), x.nodeType === 1 && x.nodeName === "BODY" || x.nodeName === "HTML" ? ie = x : ie.appendChild(x);
         else {
             if (!Re && !Ie && !Ue && // eslint-disable-next-line unicorn/prefer-includes
-                ue.indexOf("<") === -1)
-                return D && Ot ? D.createHTML(ue) : ue;
-            if (ie = d(ue), !ie)
+                ce.indexOf("<") === -1)
+                return D && Ot ? D.createHTML(ce) : ce;
+            if (ie = d(ce), !ie)
                 return Re ? null : Ot ? E : "";
         }
         ie && Nn && Qt(ie.firstChild);
-        const Lt = g(Ee ? ue : ie);
+        const Lt = g(Ee ? ce : ie);
         for (; Ye = Lt.nextNode();)
             ze(Ye) || (Ye.content instanceof o && De(Ye.content), Dn(Ye));
         if (Ee)
-            return ue;
+            return ce;
         if (Re) {
             if ($t)
                 for (H = I.call(ie.ownerDocument); ie.firstChild;)
                     H.appendChild(ie.firstChild);
             else
                 H = ie;
             return (de.shadowroot || de.shadowrootmode) && (H = Y.call(r, H, !0)), H;
         }
         let Vt = Ue ? ie.outerHTML : ie.innerHTML;
         return Ue && oe["!doctype"] && ie.ownerDocument && ie.ownerDocument.doctype && ie.ownerDocument.doctype.name && an(_h, ie.ownerDocument.doctype.name) && (Vt = "<!DOCTYPE " + ie.ownerDocument.doctype.name + `>
 ` + Vt), Ie && Ws([re, pe, Me], (Un) => {
             Vt = Xr(Vt, Un, " ");
         }), D && Ot ? D.createHTML(Vt) : Vt;
     }, e.setConfig = function() {
-        let ue = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : {};
-        en(ue), zt = !0;
+        let ce = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : {};
+        en(ce), zt = !0;
     }, e.clearConfig = function() {
         qn = null, zt = !1;
-    }, e.isValidAttribute = function(ue, G, ie) {
+    }, e.isValidAttribute = function(ce, G, ie) {
         qn || en({});
-        const x = wt(ue),
+        const x = wt(ce),
             Ye = wt(G);
         return fe(x, Ye, ie);
-    }, e.addHook = function(ue, G) {
-        typeof G == "function" && (ne[ue] = ne[ue] || [], Wr(ne[ue], G));
-    }, e.removeHook = function(ue) {
-        if (ne[ue])
-            return mc(ne[ue]);
-    }, e.removeHooks = function(ue) {
-        ne[ue] && (ne[ue] = []);
+    }, e.addHook = function(ce, G) {
+        typeof G == "function" && (ne[ce] = ne[ce] || [], Wr(ne[ce], G));
+    }, e.removeHook = function(ce) {
+        if (ne[ce])
+            return mc(ne[ce]);
+    }, e.removeHooks = function(ce) {
+        ne[ce] && (ne[ce] = []);
     }, e.removeAllHooks = function() {
         ne = {};
     }, e;
 }
 var vc = bh(),
     wh = {
         exports: {}
@@ -8295,21 +8295,21 @@
                         constructor(s, a, f) {
                             this.id = void 0, this.size = void 0, this.cramped = void 0, this.id = s, this.size = a, this.cramped = f;
                         }
                         /**
                          * Get the style of a superscript given a base in the current style.
                          */
                         sup() {
-                            return Ne[ke[this.id]];
+                            return Ne[ve[this.id]];
                         }
                         /**
                          * Get the style of a subscript given a base in the current style.
                          */
                         sub() {
-                            return Ne[ce[this.id]];
+                            return Ne[ue[this.id]];
                         }
                         /**
                          * Get the style of a fraction numerator given the fraction in the current
                          * style.
                          */
                         fracNum() {
                             return Ne[he[this.id]];
@@ -8346,21 +8346,21 @@
                         z = 2,
                         Y = 3,
                         ne = 4,
                         re = 5,
                         pe = 6,
                         Me = 7,
                         Ne = [new C(R, 0, !1), new C(I, 0, !0), new C(z, 1, !1), new C(Y, 1, !0), new C(ne, 2, !1), new C(re, 2, !0), new C(pe, 3, !1), new C(Me, 3, !0)],
-                        ke = [ne, re, ne, re, pe, Me, pe, Me],
-                        ce = [re, re, re, re, Me, Me, Me, Me],
+                        ve = [ne, re, ne, re, pe, Me, pe, Me],
+                        ue = [re, re, re, re, Me, Me, Me, Me],
                         he = [z, Y, ne, re, pe, Me, pe, Me],
                         le = [Y, Y, re, re, Me, Me, Me, Me],
                         Be = [I, I, Y, Y, re, re, Me, Me],
                         oe = [R, I, z, Y, z, Y, z, Y];
-                    var Q = {
+                    var K = {
                         DISPLAY: Ne[R],
                         TEXT: Ne[z],
                         SCRIPT: Ne[ne],
                         SCRIPTSCRIPT: Ne[pe]
                     };
                     const de = [{
                         // Latin characters beyond the Latin-1 characters we have metrics for.
@@ -8448,15 +8448,15 @@
 
                     function we(i) {
                         for (let s = 0; s < ee.length; s += 2)
                             if (i >= ee[s] && i <= ee[s + 1])
                                 return !0;
                         return !1;
                     }
-                    const ve = 80,
+                    const ke = 80,
                         $ = function(i, s) {
                             return "M95," + (622 + i + s) + `
 c-2.7,0,-7.17,-2.7,-13.5,-8c-5.8,-5.3,-9.5,-10,-9.5,-14
 c0,-2,0.3,-3.3,1,-4c1.3,-2.7,23.83,-20.7,67.5,-54
 c44.2,-33.3,65.8,-50.3,66.5,-51c1.3,-1.3,3,-2,5,-2c4.7,0,8.7,3.3,12,10
 s173,378,173,378c0.7,0,35.3,-71,104,-213c68.7,-142,137.5,-285,206.5,-429
 c69,-144,104.5,-217.7,106.5,-221
@@ -8528,30 +8528,30 @@
 219 661 l218 661zM702 ` + s + "H400000v" + (40 + i) + "H742z";
                         },
                         zt = function(i, s, a) {
                             s = 1e3 * s;
                             let f = "";
                             switch (i) {
                                 case "sqrtMain":
-                                    f = $(s, ve);
+                                    f = $(s, ke);
                                     break;
                                 case "sqrtSize1":
-                                    f = xe(s, ve);
+                                    f = xe(s, ke);
                                     break;
                                 case "sqrtSize2":
-                                    f = Se(s, ve);
+                                    f = Se(s, ke);
                                     break;
                                 case "sqrtSize3":
-                                    f = We(s, ve);
+                                    f = We(s, ke);
                                     break;
                                 case "sqrtSize4":
-                                    f = Ie(s, ve);
+                                    f = Ie(s, ke);
                                     break;
                                 case "sqrtTall":
-                                    f = Ue(s, ve, a);
+                                    f = Ue(s, ke, a);
                             }
                             return f;
                         },
                         Nn = function(i, s) {
                             switch (i) {
                                 case "⎜":
                                     return "M291 0 H417 V" + s + " H291z M291 0 H417 V" + s + " H291z";
@@ -10986,15 +10986,15 @@
                             937: [0, 0.61111, 0, 0, 0.525],
                             8216: [0, 0.61111, 0, 0, 0.525],
                             8217: [0, 0.61111, 0, 0, 0.525],
                             8242: [0, 0.61111, 0, 0, 0.525],
                             9251: [0.11111, 0.21944, 0, 0, 0.525]
                         }
                     };
-                    const K = {
+                    const Q = {
                             slant: [0.25, 0.25, 0.25],
                             // sigma1
                             space: [0, 0, 0],
                             // sigma2
                             stretch: [0, 0, 0],
                             // sigma3
                             shrink: [0, 0, 0],
@@ -11167,18 +11167,18 @@
                     }
                     const me = {};
 
                     function Oe(i) {
                         let s;
                         if (i >= 5 ? s = 0 : i >= 3 ? s = 1 : s = 2, !me[s]) {
                             const a = me[s] = {
-                                cssEmPerMu: K.quad[s] / 18
+                                cssEmPerMu: Q.quad[s] / 18
                             };
-                            for (const f in K)
-                                K.hasOwnProperty(f) && (a[f] = K[f][s]);
+                            for (const f in Q)
+                                Q.hasOwnProperty(f) && (a[f] = Q[f][s]);
                         }
                         return me[s];
                     }
                     const et = [
                             // Each element contains [textsize, scriptsize, scriptscriptsize].
                             // The size mappings are taken from TeX with \normalsize=10pt.
                             [1, 1, 1],
@@ -11693,21 +11693,21 @@
                         y = "main",
                         B = "ams",
                         ze = "accent-token",
                         fe = "bin",
                         pt = "close",
                         Dn = "inner",
                         De = "mathord",
-                        ue = "op-token",
+                        ce = "op-token",
                         G = "open",
                         ie = "punct",
                         x = "rel",
                         Ye = "spacing",
                         H = "textord";
-                    d(g, y, x, "≡", "\\equiv", !0), d(g, y, x, "≺", "\\prec", !0), d(g, y, x, "≻", "\\succ", !0), d(g, y, x, "∼", "\\sim", !0), d(g, y, x, "⊥", "\\perp"), d(g, y, x, "⪯", "\\preceq", !0), d(g, y, x, "⪰", "\\succeq", !0), d(g, y, x, "≃", "\\simeq", !0), d(g, y, x, "∣", "\\mid", !0), d(g, y, x, "≪", "\\ll", !0), d(g, y, x, "≫", "\\gg", !0), d(g, y, x, "≍", "\\asymp", !0), d(g, y, x, "∥", "\\parallel"), d(g, y, x, "⋈", "\\bowtie", !0), d(g, y, x, "⌣", "\\smile", !0), d(g, y, x, "⊑", "\\sqsubseteq", !0), d(g, y, x, "⊒", "\\sqsupseteq", !0), d(g, y, x, "≐", "\\doteq", !0), d(g, y, x, "⌢", "\\frown", !0), d(g, y, x, "∋", "\\ni", !0), d(g, y, x, "∝", "\\propto", !0), d(g, y, x, "⊢", "\\vdash", !0), d(g, y, x, "⊣", "\\dashv", !0), d(g, y, x, "∋", "\\owns"), d(g, y, ie, ".", "\\ldotp"), d(g, y, ie, "⋅", "\\cdotp"), d(g, y, H, "#", "\\#"), d(Z, y, H, "#", "\\#"), d(g, y, H, "&", "\\&"), d(Z, y, H, "&", "\\&"), d(g, y, H, "ℵ", "\\aleph", !0), d(g, y, H, "∀", "\\forall", !0), d(g, y, H, "ℏ", "\\hbar", !0), d(g, y, H, "∃", "\\exists", !0), d(g, y, H, "∇", "\\nabla", !0), d(g, y, H, "♭", "\\flat", !0), d(g, y, H, "ℓ", "\\ell", !0), d(g, y, H, "♮", "\\natural", !0), d(g, y, H, "♣", "\\clubsuit", !0), d(g, y, H, "℘", "\\wp", !0), d(g, y, H, "♯", "\\sharp", !0), d(g, y, H, "♢", "\\diamondsuit", !0), d(g, y, H, "ℜ", "\\Re", !0), d(g, y, H, "♡", "\\heartsuit", !0), d(g, y, H, "ℑ", "\\Im", !0), d(g, y, H, "♠", "\\spadesuit", !0), d(g, y, H, "§", "\\S", !0), d(Z, y, H, "§", "\\S"), d(g, y, H, "¶", "\\P", !0), d(Z, y, H, "¶", "\\P"), d(g, y, H, "†", "\\dag"), d(Z, y, H, "†", "\\dag"), d(Z, y, H, "†", "\\textdagger"), d(g, y, H, "‡", "\\ddag"), d(Z, y, H, "‡", "\\ddag"), d(Z, y, H, "‡", "\\textdaggerdbl"), d(g, y, pt, "⎱", "\\rmoustache", !0), d(g, y, G, "⎰", "\\lmoustache", !0), d(g, y, pt, "⟯", "\\rgroup", !0), d(g, y, G, "⟮", "\\lgroup", !0), d(g, y, fe, "∓", "\\mp", !0), d(g, y, fe, "⊖", "\\ominus", !0), d(g, y, fe, "⊎", "\\uplus", !0), d(g, y, fe, "⊓", "\\sqcap", !0), d(g, y, fe, "∗", "\\ast"), d(g, y, fe, "⊔", "\\sqcup", !0), d(g, y, fe, "◯", "\\bigcirc", !0), d(g, y, fe, "∙", "\\bullet", !0), d(g, y, fe, "‡", "\\ddagger"), d(g, y, fe, "≀", "\\wr", !0), d(g, y, fe, "⨿", "\\amalg"), d(g, y, fe, "&", "\\And"), d(g, y, x, "⟵", "\\longleftarrow", !0), d(g, y, x, "⇐", "\\Leftarrow", !0), d(g, y, x, "⟸", "\\Longleftarrow", !0), d(g, y, x, "⟶", "\\longrightarrow", !0), d(g, y, x, "⇒", "\\Rightarrow", !0), d(g, y, x, "⟹", "\\Longrightarrow", !0), d(g, y, x, "↔", "\\leftrightarrow", !0), d(g, y, x, "⟷", "\\longleftrightarrow", !0), d(g, y, x, "⇔", "\\Leftrightarrow", !0), d(g, y, x, "⟺", "\\Longleftrightarrow", !0), d(g, y, x, "↦", "\\mapsto", !0), d(g, y, x, "⟼", "\\longmapsto", !0), d(g, y, x, "↗", "\\nearrow", !0), d(g, y, x, "↩", "\\hookleftarrow", !0), d(g, y, x, "↪", "\\hookrightarrow", !0), d(g, y, x, "↘", "\\searrow", !0), d(g, y, x, "↼", "\\leftharpoonup", !0), d(g, y, x, "⇀", "\\rightharpoonup", !0), d(g, y, x, "↙", "\\swarrow", !0), d(g, y, x, "↽", "\\leftharpoondown", !0), d(g, y, x, "⇁", "\\rightharpoondown", !0), d(g, y, x, "↖", "\\nwarrow", !0), d(g, y, x, "⇌", "\\rightleftharpoons", !0), d(g, B, x, "≮", "\\nless", !0), d(g, B, x, "", "\\@nleqslant"), d(g, B, x, "", "\\@nleqq"), d(g, B, x, "⪇", "\\lneq", !0), d(g, B, x, "≨", "\\lneqq", !0), d(g, B, x, "", "\\@lvertneqq"), d(g, B, x, "⋦", "\\lnsim", !0), d(g, B, x, "⪉", "\\lnapprox", !0), d(g, B, x, "⊀", "\\nprec", !0), d(g, B, x, "⋠", "\\npreceq", !0), d(g, B, x, "⋨", "\\precnsim", !0), d(g, B, x, "⪹", "\\precnapprox", !0), d(g, B, x, "≁", "\\nsim", !0), d(g, B, x, "", "\\@nshortmid"), d(g, B, x, "∤", "\\nmid", !0), d(g, B, x, "⊬", "\\nvdash", !0), d(g, B, x, "⊭", "\\nvDash", !0), d(g, B, x, "⋪", "\\ntriangleleft"), d(g, B, x, "⋬", "\\ntrianglelefteq", !0), d(g, B, x, "⊊", "\\subsetneq", !0), d(g, B, x, "", "\\@varsubsetneq"), d(g, B, x, "⫋", "\\subsetneqq", !0), d(g, B, x, "", "\\@varsubsetneqq"), d(g, B, x, "≯", "\\ngtr", !0), d(g, B, x, "", "\\@ngeqslant"), d(g, B, x, "", "\\@ngeqq"), d(g, B, x, "⪈", "\\gneq", !0), d(g, B, x, "≩", "\\gneqq", !0), d(g, B, x, "", "\\@gvertneqq"), d(g, B, x, "⋧", "\\gnsim", !0), d(g, B, x, "⪊", "\\gnapprox", !0), d(g, B, x, "⊁", "\\nsucc", !0), d(g, B, x, "⋡", "\\nsucceq", !0), d(g, B, x, "⋩", "\\succnsim", !0), d(g, B, x, "⪺", "\\succnapprox", !0), d(g, B, x, "≆", "\\ncong", !0), d(g, B, x, "", "\\@nshortparallel"), d(g, B, x, "∦", "\\nparallel", !0), d(g, B, x, "⊯", "\\nVDash", !0), d(g, B, x, "⋫", "\\ntriangleright"), d(g, B, x, "⋭", "\\ntrianglerighteq", !0), d(g, B, x, "", "\\@nsupseteqq"), d(g, B, x, "⊋", "\\supsetneq", !0), d(g, B, x, "", "\\@varsupsetneq"), d(g, B, x, "⫌", "\\supsetneqq", !0), d(g, B, x, "", "\\@varsupsetneqq"), d(g, B, x, "⊮", "\\nVdash", !0), d(g, B, x, "⪵", "\\precneqq", !0), d(g, B, x, "⪶", "\\succneqq", !0), d(g, B, x, "", "\\@nsubseteqq"), d(g, B, fe, "⊴", "\\unlhd"), d(g, B, fe, "⊵", "\\unrhd"), d(g, B, x, "↚", "\\nleftarrow", !0), d(g, B, x, "↛", "\\nrightarrow", !0), d(g, B, x, "⇍", "\\nLeftarrow", !0), d(g, B, x, "⇏", "\\nRightarrow", !0), d(g, B, x, "↮", "\\nleftrightarrow", !0), d(g, B, x, "⇎", "\\nLeftrightarrow", !0), d(g, B, x, "△", "\\vartriangle"), d(g, B, H, "ℏ", "\\hslash"), d(g, B, H, "▽", "\\triangledown"), d(g, B, H, "◊", "\\lozenge"), d(g, B, H, "Ⓢ", "\\circledS"), d(g, B, H, "®", "\\circledR"), d(Z, B, H, "®", "\\circledR"), d(g, B, H, "∡", "\\measuredangle", !0), d(g, B, H, "∄", "\\nexists"), d(g, B, H, "℧", "\\mho"), d(g, B, H, "Ⅎ", "\\Finv", !0), d(g, B, H, "⅁", "\\Game", !0), d(g, B, H, "‵", "\\backprime"), d(g, B, H, "▲", "\\blacktriangle"), d(g, B, H, "▼", "\\blacktriangledown"), d(g, B, H, "■", "\\blacksquare"), d(g, B, H, "⧫", "\\blacklozenge"), d(g, B, H, "★", "\\bigstar"), d(g, B, H, "∢", "\\sphericalangle", !0), d(g, B, H, "∁", "\\complement", !0), d(g, B, H, "ð", "\\eth", !0), d(Z, y, H, "ð", "ð"), d(g, B, H, "╱", "\\diagup"), d(g, B, H, "╲", "\\diagdown"), d(g, B, H, "□", "\\square"), d(g, B, H, "□", "\\Box"), d(g, B, H, "◊", "\\Diamond"), d(g, B, H, "¥", "\\yen", !0), d(Z, B, H, "¥", "\\yen", !0), d(g, B, H, "✓", "\\checkmark", !0), d(Z, B, H, "✓", "\\checkmark"), d(g, B, H, "ℶ", "\\beth", !0), d(g, B, H, "ℸ", "\\daleth", !0), d(g, B, H, "ℷ", "\\gimel", !0), d(g, B, H, "ϝ", "\\digamma", !0), d(g, B, H, "ϰ", "\\varkappa"), d(g, B, G, "┌", "\\@ulcorner", !0), d(g, B, pt, "┐", "\\@urcorner", !0), d(g, B, G, "└", "\\@llcorner", !0), d(g, B, pt, "┘", "\\@lrcorner", !0), d(g, B, x, "≦", "\\leqq", !0), d(g, B, x, "⩽", "\\leqslant", !0), d(g, B, x, "⪕", "\\eqslantless", !0), d(g, B, x, "≲", "\\lesssim", !0), d(g, B, x, "⪅", "\\lessapprox", !0), d(g, B, x, "≊", "\\approxeq", !0), d(g, B, fe, "⋖", "\\lessdot"), d(g, B, x, "⋘", "\\lll", !0), d(g, B, x, "≶", "\\lessgtr", !0), d(g, B, x, "⋚", "\\lesseqgtr", !0), d(g, B, x, "⪋", "\\lesseqqgtr", !0), d(g, B, x, "≑", "\\doteqdot"), d(g, B, x, "≓", "\\risingdotseq", !0), d(g, B, x, "≒", "\\fallingdotseq", !0), d(g, B, x, "∽", "\\backsim", !0), d(g, B, x, "⋍", "\\backsimeq", !0), d(g, B, x, "⫅", "\\subseteqq", !0), d(g, B, x, "⋐", "\\Subset", !0), d(g, B, x, "⊏", "\\sqsubset", !0), d(g, B, x, "≼", "\\preccurlyeq", !0), d(g, B, x, "⋞", "\\curlyeqprec", !0), d(g, B, x, "≾", "\\precsim", !0), d(g, B, x, "⪷", "\\precapprox", !0), d(g, B, x, "⊲", "\\vartriangleleft"), d(g, B, x, "⊴", "\\trianglelefteq"), d(g, B, x, "⊨", "\\vDash", !0), d(g, B, x, "⊪", "\\Vvdash", !0), d(g, B, x, "⌣", "\\smallsmile"), d(g, B, x, "⌢", "\\smallfrown"), d(g, B, x, "≏", "\\bumpeq", !0), d(g, B, x, "≎", "\\Bumpeq", !0), d(g, B, x, "≧", "\\geqq", !0), d(g, B, x, "⩾", "\\geqslant", !0), d(g, B, x, "⪖", "\\eqslantgtr", !0), d(g, B, x, "≳", "\\gtrsim", !0), d(g, B, x, "⪆", "\\gtrapprox", !0), d(g, B, fe, "⋗", "\\gtrdot"), d(g, B, x, "⋙", "\\ggg", !0), d(g, B, x, "≷", "\\gtrless", !0), d(g, B, x, "⋛", "\\gtreqless", !0), d(g, B, x, "⪌", "\\gtreqqless", !0), d(g, B, x, "≖", "\\eqcirc", !0), d(g, B, x, "≗", "\\circeq", !0), d(g, B, x, "≜", "\\triangleq", !0), d(g, B, x, "∼", "\\thicksim"), d(g, B, x, "≈", "\\thickapprox"), d(g, B, x, "⫆", "\\supseteqq", !0), d(g, B, x, "⋑", "\\Supset", !0), d(g, B, x, "⊐", "\\sqsupset", !0), d(g, B, x, "≽", "\\succcurlyeq", !0), d(g, B, x, "⋟", "\\curlyeqsucc", !0), d(g, B, x, "≿", "\\succsim", !0), d(g, B, x, "⪸", "\\succapprox", !0), d(g, B, x, "⊳", "\\vartriangleright"), d(g, B, x, "⊵", "\\trianglerighteq"), d(g, B, x, "⊩", "\\Vdash", !0), d(g, B, x, "∣", "\\shortmid"), d(g, B, x, "∥", "\\shortparallel"), d(g, B, x, "≬", "\\between", !0), d(g, B, x, "⋔", "\\pitchfork", !0), d(g, B, x, "∝", "\\varpropto"), d(g, B, x, "◀", "\\blacktriangleleft"), d(g, B, x, "∴", "\\therefore", !0), d(g, B, x, "∍", "\\backepsilon"), d(g, B, x, "▶", "\\blacktriangleright"), d(g, B, x, "∵", "\\because", !0), d(g, B, x, "⋘", "\\llless"), d(g, B, x, "⋙", "\\gggtr"), d(g, B, fe, "⊲", "\\lhd"), d(g, B, fe, "⊳", "\\rhd"), d(g, B, x, "≂", "\\eqsim", !0), d(g, y, x, "⋈", "\\Join"), d(g, B, x, "≑", "\\Doteq", !0), d(g, B, fe, "∔", "\\dotplus", !0), d(g, B, fe, "∖", "\\smallsetminus"), d(g, B, fe, "⋒", "\\Cap", !0), d(g, B, fe, "⋓", "\\Cup", !0), d(g, B, fe, "⩞", "\\doublebarwedge", !0), d(g, B, fe, "⊟", "\\boxminus", !0), d(g, B, fe, "⊞", "\\boxplus", !0), d(g, B, fe, "⋇", "\\divideontimes", !0), d(g, B, fe, "⋉", "\\ltimes", !0), d(g, B, fe, "⋊", "\\rtimes", !0), d(g, B, fe, "⋋", "\\leftthreetimes", !0), d(g, B, fe, "⋌", "\\rightthreetimes", !0), d(g, B, fe, "⋏", "\\curlywedge", !0), d(g, B, fe, "⋎", "\\curlyvee", !0), d(g, B, fe, "⊝", "\\circleddash", !0), d(g, B, fe, "⊛", "\\circledast", !0), d(g, B, fe, "⋅", "\\centerdot"), d(g, B, fe, "⊺", "\\intercal", !0), d(g, B, fe, "⋒", "\\doublecap"), d(g, B, fe, "⋓", "\\doublecup"), d(g, B, fe, "⊠", "\\boxtimes", !0), d(g, B, x, "⇢", "\\dashrightarrow", !0), d(g, B, x, "⇠", "\\dashleftarrow", !0), d(g, B, x, "⇇", "\\leftleftarrows", !0), d(g, B, x, "⇆", "\\leftrightarrows", !0), d(g, B, x, "⇚", "\\Lleftarrow", !0), d(g, B, x, "↞", "\\twoheadleftarrow", !0), d(g, B, x, "↢", "\\leftarrowtail", !0), d(g, B, x, "↫", "\\looparrowleft", !0), d(g, B, x, "⇋", "\\leftrightharpoons", !0), d(g, B, x, "↶", "\\curvearrowleft", !0), d(g, B, x, "↺", "\\circlearrowleft", !0), d(g, B, x, "↰", "\\Lsh", !0), d(g, B, x, "⇈", "\\upuparrows", !0), d(g, B, x, "↿", "\\upharpoonleft", !0), d(g, B, x, "⇃", "\\downharpoonleft", !0), d(g, y, x, "⊶", "\\origof", !0), d(g, y, x, "⊷", "\\imageof", !0), d(g, B, x, "⊸", "\\multimap", !0), d(g, B, x, "↭", "\\leftrightsquigarrow", !0), d(g, B, x, "⇉", "\\rightrightarrows", !0), d(g, B, x, "⇄", "\\rightleftarrows", !0), d(g, B, x, "↠", "\\twoheadrightarrow", !0), d(g, B, x, "↣", "\\rightarrowtail", !0), d(g, B, x, "↬", "\\looparrowright", !0), d(g, B, x, "↷", "\\curvearrowright", !0), d(g, B, x, "↻", "\\circlearrowright", !0), d(g, B, x, "↱", "\\Rsh", !0), d(g, B, x, "⇊", "\\downdownarrows", !0), d(g, B, x, "↾", "\\upharpoonright", !0), d(g, B, x, "⇂", "\\downharpoonright", !0), d(g, B, x, "⇝", "\\rightsquigarrow", !0), d(g, B, x, "⇝", "\\leadsto"), d(g, B, x, "⇛", "\\Rrightarrow", !0), d(g, B, x, "↾", "\\restriction"), d(g, y, H, "‘", "`"), d(g, y, H, "$", "\\$"), d(Z, y, H, "$", "\\$"), d(Z, y, H, "$", "\\textdollar"), d(g, y, H, "%", "\\%"), d(Z, y, H, "%", "\\%"), d(g, y, H, "_", "\\_"), d(Z, y, H, "_", "\\_"), d(Z, y, H, "_", "\\textunderscore"), d(g, y, H, "∠", "\\angle", !0), d(g, y, H, "∞", "\\infty", !0), d(g, y, H, "′", "\\prime"), d(g, y, H, "△", "\\triangle"), d(g, y, H, "Γ", "\\Gamma", !0), d(g, y, H, "Δ", "\\Delta", !0), d(g, y, H, "Θ", "\\Theta", !0), d(g, y, H, "Λ", "\\Lambda", !0), d(g, y, H, "Ξ", "\\Xi", !0), d(g, y, H, "Π", "\\Pi", !0), d(g, y, H, "Σ", "\\Sigma", !0), d(g, y, H, "Υ", "\\Upsilon", !0), d(g, y, H, "Φ", "\\Phi", !0), d(g, y, H, "Ψ", "\\Psi", !0), d(g, y, H, "Ω", "\\Omega", !0), d(g, y, H, "A", "Α"), d(g, y, H, "B", "Β"), d(g, y, H, "E", "Ε"), d(g, y, H, "Z", "Ζ"), d(g, y, H, "H", "Η"), d(g, y, H, "I", "Ι"), d(g, y, H, "K", "Κ"), d(g, y, H, "M", "Μ"), d(g, y, H, "N", "Ν"), d(g, y, H, "O", "Ο"), d(g, y, H, "P", "Ρ"), d(g, y, H, "T", "Τ"), d(g, y, H, "X", "Χ"), d(g, y, H, "¬", "\\neg", !0), d(g, y, H, "¬", "\\lnot"), d(g, y, H, "⊤", "\\top"), d(g, y, H, "⊥", "\\bot"), d(g, y, H, "∅", "\\emptyset"), d(g, B, H, "∅", "\\varnothing"), d(g, y, De, "α", "\\alpha", !0), d(g, y, De, "β", "\\beta", !0), d(g, y, De, "γ", "\\gamma", !0), d(g, y, De, "δ", "\\delta", !0), d(g, y, De, "ϵ", "\\epsilon", !0), d(g, y, De, "ζ", "\\zeta", !0), d(g, y, De, "η", "\\eta", !0), d(g, y, De, "θ", "\\theta", !0), d(g, y, De, "ι", "\\iota", !0), d(g, y, De, "κ", "\\kappa", !0), d(g, y, De, "λ", "\\lambda", !0), d(g, y, De, "μ", "\\mu", !0), d(g, y, De, "ν", "\\nu", !0), d(g, y, De, "ξ", "\\xi", !0), d(g, y, De, "ο", "\\omicron", !0), d(g, y, De, "π", "\\pi", !0), d(g, y, De, "ρ", "\\rho", !0), d(g, y, De, "σ", "\\sigma", !0), d(g, y, De, "τ", "\\tau", !0), d(g, y, De, "υ", "\\upsilon", !0), d(g, y, De, "ϕ", "\\phi", !0), d(g, y, De, "χ", "\\chi", !0), d(g, y, De, "ψ", "\\psi", !0), d(g, y, De, "ω", "\\omega", !0), d(g, y, De, "ε", "\\varepsilon", !0), d(g, y, De, "ϑ", "\\vartheta", !0), d(g, y, De, "ϖ", "\\varpi", !0), d(g, y, De, "ϱ", "\\varrho", !0), d(g, y, De, "ς", "\\varsigma", !0), d(g, y, De, "φ", "\\varphi", !0), d(g, y, fe, "∗", "*", !0), d(g, y, fe, "+", "+"), d(g, y, fe, "−", "-", !0), d(g, y, fe, "⋅", "\\cdot", !0), d(g, y, fe, "∘", "\\circ", !0), d(g, y, fe, "÷", "\\div", !0), d(g, y, fe, "±", "\\pm", !0), d(g, y, fe, "×", "\\times", !0), d(g, y, fe, "∩", "\\cap", !0), d(g, y, fe, "∪", "\\cup", !0), d(g, y, fe, "∖", "\\setminus", !0), d(g, y, fe, "∧", "\\land"), d(g, y, fe, "∨", "\\lor"), d(g, y, fe, "∧", "\\wedge", !0), d(g, y, fe, "∨", "\\vee", !0), d(g, y, H, "√", "\\surd"), d(g, y, G, "⟨", "\\langle", !0), d(g, y, G, "∣", "\\lvert"), d(g, y, G, "∥", "\\lVert"), d(g, y, pt, "?", "?"), d(g, y, pt, "!", "!"), d(g, y, pt, "⟩", "\\rangle", !0), d(g, y, pt, "∣", "\\rvert"), d(g, y, pt, "∥", "\\rVert"), d(g, y, x, "=", "="), d(g, y, x, ":", ":"), d(g, y, x, "≈", "\\approx", !0), d(g, y, x, "≅", "\\cong", !0), d(g, y, x, "≥", "\\ge"), d(g, y, x, "≥", "\\geq", !0), d(g, y, x, "←", "\\gets"), d(g, y, x, ">", "\\gt", !0), d(g, y, x, "∈", "\\in", !0), d(g, y, x, "", "\\@not"), d(g, y, x, "⊂", "\\subset", !0), d(g, y, x, "⊃", "\\supset", !0), d(g, y, x, "⊆", "\\subseteq", !0), d(g, y, x, "⊇", "\\supseteq", !0), d(g, B, x, "⊈", "\\nsubseteq", !0), d(g, B, x, "⊉", "\\nsupseteq", !0), d(g, y, x, "⊨", "\\models"), d(g, y, x, "←", "\\leftarrow", !0), d(g, y, x, "≤", "\\le"), d(g, y, x, "≤", "\\leq", !0), d(g, y, x, "<", "\\lt", !0), d(g, y, x, "→", "\\rightarrow", !0), d(g, y, x, "→", "\\to"), d(g, B, x, "≱", "\\ngeq", !0), d(g, B, x, "≰", "\\nleq", !0), d(g, y, Ye, " ", "\\ "), d(g, y, Ye, " ", "\\space"), d(g, y, Ye, " ", "\\nobreakspace"), d(Z, y, Ye, " ", "\\ "), d(Z, y, Ye, " ", " "), d(Z, y, Ye, " ", "\\space"), d(Z, y, Ye, " ", "\\nobreakspace"), d(g, y, Ye, null, "\\nobreak"), d(g, y, Ye, null, "\\allowbreak"), d(g, y, ie, ",", ","), d(g, y, ie, ";", ";"), d(g, B, fe, "⊼", "\\barwedge", !0), d(g, B, fe, "⊻", "\\veebar", !0), d(g, y, fe, "⊙", "\\odot", !0), d(g, y, fe, "⊕", "\\oplus", !0), d(g, y, fe, "⊗", "\\otimes", !0), d(g, y, H, "∂", "\\partial", !0), d(g, y, fe, "⊘", "\\oslash", !0), d(g, B, fe, "⊚", "\\circledcirc", !0), d(g, B, fe, "⊡", "\\boxdot", !0), d(g, y, fe, "△", "\\bigtriangleup"), d(g, y, fe, "▽", "\\bigtriangledown"), d(g, y, fe, "†", "\\dagger"), d(g, y, fe, "⋄", "\\diamond"), d(g, y, fe, "⋆", "\\star"), d(g, y, fe, "◃", "\\triangleleft"), d(g, y, fe, "▹", "\\triangleright"), d(g, y, G, "{", "\\{"), d(Z, y, H, "{", "\\{"), d(Z, y, H, "{", "\\textbraceleft"), d(g, y, pt, "}", "\\}"), d(Z, y, H, "}", "\\}"), d(Z, y, H, "}", "\\textbraceright"), d(g, y, G, "{", "\\lbrace"), d(g, y, pt, "}", "\\rbrace"), d(g, y, G, "[", "\\lbrack", !0), d(Z, y, H, "[", "\\lbrack", !0), d(g, y, pt, "]", "\\rbrack", !0), d(Z, y, H, "]", "\\rbrack", !0), d(g, y, G, "(", "\\lparen", !0), d(g, y, pt, ")", "\\rparen", !0), d(Z, y, H, "<", "\\textless", !0), d(Z, y, H, ">", "\\textgreater", !0), d(g, y, G, "⌊", "\\lfloor", !0), d(g, y, pt, "⌋", "\\rfloor", !0), d(g, y, G, "⌈", "\\lceil", !0), d(g, y, pt, "⌉", "\\rceil", !0), d(g, y, H, "\\", "\\backslash"), d(g, y, H, "∣", "|"), d(g, y, H, "∣", "\\vert"), d(Z, y, H, "|", "\\textbar", !0), d(g, y, H, "∥", "\\|"), d(g, y, H, "∥", "\\Vert"), d(Z, y, H, "∥", "\\textbardbl"), d(Z, y, H, "~", "\\textasciitilde"), d(Z, y, H, "\\", "\\textbackslash"), d(Z, y, H, "^", "\\textasciicircum"), d(g, y, x, "↑", "\\uparrow", !0), d(g, y, x, "⇑", "\\Uparrow", !0), d(g, y, x, "↓", "\\downarrow", !0), d(g, y, x, "⇓", "\\Downarrow", !0), d(g, y, x, "↕", "\\updownarrow", !0), d(g, y, x, "⇕", "\\Updownarrow", !0), d(g, y, ue, "∐", "\\coprod"), d(g, y, ue, "⋁", "\\bigvee"), d(g, y, ue, "⋀", "\\bigwedge"), d(g, y, ue, "⨄", "\\biguplus"), d(g, y, ue, "⋂", "\\bigcap"), d(g, y, ue, "⋃", "\\bigcup"), d(g, y, ue, "∫", "\\int"), d(g, y, ue, "∫", "\\intop"), d(g, y, ue, "∬", "\\iint"), d(g, y, ue, "∭", "\\iiint"), d(g, y, ue, "∏", "\\prod"), d(g, y, ue, "∑", "\\sum"), d(g, y, ue, "⨂", "\\bigotimes"), d(g, y, ue, "⨁", "\\bigoplus"), d(g, y, ue, "⨀", "\\bigodot"), d(g, y, ue, "∮", "\\oint"), d(g, y, ue, "∯", "\\oiint"), d(g, y, ue, "∰", "\\oiiint"), d(g, y, ue, "⨆", "\\bigsqcup"), d(g, y, ue, "∫", "\\smallint"), d(Z, y, Dn, "…", "\\textellipsis"), d(g, y, Dn, "…", "\\mathellipsis"), d(Z, y, Dn, "…", "\\ldots", !0), d(g, y, Dn, "…", "\\ldots", !0), d(g, y, Dn, "⋯", "\\@cdots", !0), d(g, y, Dn, "⋱", "\\ddots", !0), d(g, y, H, "⋮", "\\varvdots"), d(g, y, ze, "ˊ", "\\acute"), d(g, y, ze, "ˋ", "\\grave"), d(g, y, ze, "¨", "\\ddot"), d(g, y, ze, "~", "\\tilde"), d(g, y, ze, "ˉ", "\\bar"), d(g, y, ze, "˘", "\\breve"), d(g, y, ze, "ˇ", "\\check"), d(g, y, ze, "^", "\\hat"), d(g, y, ze, "⃗", "\\vec"), d(g, y, ze, "˙", "\\dot"), d(g, y, ze, "˚", "\\mathring"), d(g, y, De, "", "\\@imath"), d(g, y, De, "", "\\@jmath"), d(g, y, H, "ı", "ı"), d(g, y, H, "ȷ", "ȷ"), d(Z, y, H, "ı", "\\i", !0), d(Z, y, H, "ȷ", "\\j", !0), d(Z, y, H, "ß", "\\ss", !0), d(Z, y, H, "æ", "\\ae", !0), d(Z, y, H, "œ", "\\oe", !0), d(Z, y, H, "ø", "\\o", !0), d(Z, y, H, "Æ", "\\AE", !0), d(Z, y, H, "Œ", "\\OE", !0), d(Z, y, H, "Ø", "\\O", !0), d(Z, y, ze, "ˊ", "\\'"), d(Z, y, ze, "ˋ", "\\`"), d(Z, y, ze, "ˆ", "\\^"), d(Z, y, ze, "˜", "\\~"), d(Z, y, ze, "ˉ", "\\="), d(Z, y, ze, "˘", "\\u"), d(Z, y, ze, "˙", "\\."), d(Z, y, ze, "¸", "\\c"), d(Z, y, ze, "˚", "\\r"), d(Z, y, ze, "ˇ", "\\v"), d(Z, y, ze, "¨", '\\"'), d(Z, y, ze, "˝", "\\H"), d(Z, y, ze, "◯", "\\textcircled");
+                    d(g, y, x, "≡", "\\equiv", !0), d(g, y, x, "≺", "\\prec", !0), d(g, y, x, "≻", "\\succ", !0), d(g, y, x, "∼", "\\sim", !0), d(g, y, x, "⊥", "\\perp"), d(g, y, x, "⪯", "\\preceq", !0), d(g, y, x, "⪰", "\\succeq", !0), d(g, y, x, "≃", "\\simeq", !0), d(g, y, x, "∣", "\\mid", !0), d(g, y, x, "≪", "\\ll", !0), d(g, y, x, "≫", "\\gg", !0), d(g, y, x, "≍", "\\asymp", !0), d(g, y, x, "∥", "\\parallel"), d(g, y, x, "⋈", "\\bowtie", !0), d(g, y, x, "⌣", "\\smile", !0), d(g, y, x, "⊑", "\\sqsubseteq", !0), d(g, y, x, "⊒", "\\sqsupseteq", !0), d(g, y, x, "≐", "\\doteq", !0), d(g, y, x, "⌢", "\\frown", !0), d(g, y, x, "∋", "\\ni", !0), d(g, y, x, "∝", "\\propto", !0), d(g, y, x, "⊢", "\\vdash", !0), d(g, y, x, "⊣", "\\dashv", !0), d(g, y, x, "∋", "\\owns"), d(g, y, ie, ".", "\\ldotp"), d(g, y, ie, "⋅", "\\cdotp"), d(g, y, H, "#", "\\#"), d(Z, y, H, "#", "\\#"), d(g, y, H, "&", "\\&"), d(Z, y, H, "&", "\\&"), d(g, y, H, "ℵ", "\\aleph", !0), d(g, y, H, "∀", "\\forall", !0), d(g, y, H, "ℏ", "\\hbar", !0), d(g, y, H, "∃", "\\exists", !0), d(g, y, H, "∇", "\\nabla", !0), d(g, y, H, "♭", "\\flat", !0), d(g, y, H, "ℓ", "\\ell", !0), d(g, y, H, "♮", "\\natural", !0), d(g, y, H, "♣", "\\clubsuit", !0), d(g, y, H, "℘", "\\wp", !0), d(g, y, H, "♯", "\\sharp", !0), d(g, y, H, "♢", "\\diamondsuit", !0), d(g, y, H, "ℜ", "\\Re", !0), d(g, y, H, "♡", "\\heartsuit", !0), d(g, y, H, "ℑ", "\\Im", !0), d(g, y, H, "♠", "\\spadesuit", !0), d(g, y, H, "§", "\\S", !0), d(Z, y, H, "§", "\\S"), d(g, y, H, "¶", "\\P", !0), d(Z, y, H, "¶", "\\P"), d(g, y, H, "†", "\\dag"), d(Z, y, H, "†", "\\dag"), d(Z, y, H, "†", "\\textdagger"), d(g, y, H, "‡", "\\ddag"), d(Z, y, H, "‡", "\\ddag"), d(Z, y, H, "‡", "\\textdaggerdbl"), d(g, y, pt, "⎱", "\\rmoustache", !0), d(g, y, G, "⎰", "\\lmoustache", !0), d(g, y, pt, "⟯", "\\rgroup", !0), d(g, y, G, "⟮", "\\lgroup", !0), d(g, y, fe, "∓", "\\mp", !0), d(g, y, fe, "⊖", "\\ominus", !0), d(g, y, fe, "⊎", "\\uplus", !0), d(g, y, fe, "⊓", "\\sqcap", !0), d(g, y, fe, "∗", "\\ast"), d(g, y, fe, "⊔", "\\sqcup", !0), d(g, y, fe, "◯", "\\bigcirc", !0), d(g, y, fe, "∙", "\\bullet", !0), d(g, y, fe, "‡", "\\ddagger"), d(g, y, fe, "≀", "\\wr", !0), d(g, y, fe, "⨿", "\\amalg"), d(g, y, fe, "&", "\\And"), d(g, y, x, "⟵", "\\longleftarrow", !0), d(g, y, x, "⇐", "\\Leftarrow", !0), d(g, y, x, "⟸", "\\Longleftarrow", !0), d(g, y, x, "⟶", "\\longrightarrow", !0), d(g, y, x, "⇒", "\\Rightarrow", !0), d(g, y, x, "⟹", "\\Longrightarrow", !0), d(g, y, x, "↔", "\\leftrightarrow", !0), d(g, y, x, "⟷", "\\longleftrightarrow", !0), d(g, y, x, "⇔", "\\Leftrightarrow", !0), d(g, y, x, "⟺", "\\Longleftrightarrow", !0), d(g, y, x, "↦", "\\mapsto", !0), d(g, y, x, "⟼", "\\longmapsto", !0), d(g, y, x, "↗", "\\nearrow", !0), d(g, y, x, "↩", "\\hookleftarrow", !0), d(g, y, x, "↪", "\\hookrightarrow", !0), d(g, y, x, "↘", "\\searrow", !0), d(g, y, x, "↼", "\\leftharpoonup", !0), d(g, y, x, "⇀", "\\rightharpoonup", !0), d(g, y, x, "↙", "\\swarrow", !0), d(g, y, x, "↽", "\\leftharpoondown", !0), d(g, y, x, "⇁", "\\rightharpoondown", !0), d(g, y, x, "↖", "\\nwarrow", !0), d(g, y, x, "⇌", "\\rightleftharpoons", !0), d(g, B, x, "≮", "\\nless", !0), d(g, B, x, "", "\\@nleqslant"), d(g, B, x, "", "\\@nleqq"), d(g, B, x, "⪇", "\\lneq", !0), d(g, B, x, "≨", "\\lneqq", !0), d(g, B, x, "", "\\@lvertneqq"), d(g, B, x, "⋦", "\\lnsim", !0), d(g, B, x, "⪉", "\\lnapprox", !0), d(g, B, x, "⊀", "\\nprec", !0), d(g, B, x, "⋠", "\\npreceq", !0), d(g, B, x, "⋨", "\\precnsim", !0), d(g, B, x, "⪹", "\\precnapprox", !0), d(g, B, x, "≁", "\\nsim", !0), d(g, B, x, "", "\\@nshortmid"), d(g, B, x, "∤", "\\nmid", !0), d(g, B, x, "⊬", "\\nvdash", !0), d(g, B, x, "⊭", "\\nvDash", !0), d(g, B, x, "⋪", "\\ntriangleleft"), d(g, B, x, "⋬", "\\ntrianglelefteq", !0), d(g, B, x, "⊊", "\\subsetneq", !0), d(g, B, x, "", "\\@varsubsetneq"), d(g, B, x, "⫋", "\\subsetneqq", !0), d(g, B, x, "", "\\@varsubsetneqq"), d(g, B, x, "≯", "\\ngtr", !0), d(g, B, x, "", "\\@ngeqslant"), d(g, B, x, "", "\\@ngeqq"), d(g, B, x, "⪈", "\\gneq", !0), d(g, B, x, "≩", "\\gneqq", !0), d(g, B, x, "", "\\@gvertneqq"), d(g, B, x, "⋧", "\\gnsim", !0), d(g, B, x, "⪊", "\\gnapprox", !0), d(g, B, x, "⊁", "\\nsucc", !0), d(g, B, x, "⋡", "\\nsucceq", !0), d(g, B, x, "⋩", "\\succnsim", !0), d(g, B, x, "⪺", "\\succnapprox", !0), d(g, B, x, "≆", "\\ncong", !0), d(g, B, x, "", "\\@nshortparallel"), d(g, B, x, "∦", "\\nparallel", !0), d(g, B, x, "⊯", "\\nVDash", !0), d(g, B, x, "⋫", "\\ntriangleright"), d(g, B, x, "⋭", "\\ntrianglerighteq", !0), d(g, B, x, "", "\\@nsupseteqq"), d(g, B, x, "⊋", "\\supsetneq", !0), d(g, B, x, "", "\\@varsupsetneq"), d(g, B, x, "⫌", "\\supsetneqq", !0), d(g, B, x, "", "\\@varsupsetneqq"), d(g, B, x, "⊮", "\\nVdash", !0), d(g, B, x, "⪵", "\\precneqq", !0), d(g, B, x, "⪶", "\\succneqq", !0), d(g, B, x, "", "\\@nsubseteqq"), d(g, B, fe, "⊴", "\\unlhd"), d(g, B, fe, "⊵", "\\unrhd"), d(g, B, x, "↚", "\\nleftarrow", !0), d(g, B, x, "↛", "\\nrightarrow", !0), d(g, B, x, "⇍", "\\nLeftarrow", !0), d(g, B, x, "⇏", "\\nRightarrow", !0), d(g, B, x, "↮", "\\nleftrightarrow", !0), d(g, B, x, "⇎", "\\nLeftrightarrow", !0), d(g, B, x, "△", "\\vartriangle"), d(g, B, H, "ℏ", "\\hslash"), d(g, B, H, "▽", "\\triangledown"), d(g, B, H, "◊", "\\lozenge"), d(g, B, H, "Ⓢ", "\\circledS"), d(g, B, H, "®", "\\circledR"), d(Z, B, H, "®", "\\circledR"), d(g, B, H, "∡", "\\measuredangle", !0), d(g, B, H, "∄", "\\nexists"), d(g, B, H, "℧", "\\mho"), d(g, B, H, "Ⅎ", "\\Finv", !0), d(g, B, H, "⅁", "\\Game", !0), d(g, B, H, "‵", "\\backprime"), d(g, B, H, "▲", "\\blacktriangle"), d(g, B, H, "▼", "\\blacktriangledown"), d(g, B, H, "■", "\\blacksquare"), d(g, B, H, "⧫", "\\blacklozenge"), d(g, B, H, "★", "\\bigstar"), d(g, B, H, "∢", "\\sphericalangle", !0), d(g, B, H, "∁", "\\complement", !0), d(g, B, H, "ð", "\\eth", !0), d(Z, y, H, "ð", "ð"), d(g, B, H, "╱", "\\diagup"), d(g, B, H, "╲", "\\diagdown"), d(g, B, H, "□", "\\square"), d(g, B, H, "□", "\\Box"), d(g, B, H, "◊", "\\Diamond"), d(g, B, H, "¥", "\\yen", !0), d(Z, B, H, "¥", "\\yen", !0), d(g, B, H, "✓", "\\checkmark", !0), d(Z, B, H, "✓", "\\checkmark"), d(g, B, H, "ℶ", "\\beth", !0), d(g, B, H, "ℸ", "\\daleth", !0), d(g, B, H, "ℷ", "\\gimel", !0), d(g, B, H, "ϝ", "\\digamma", !0), d(g, B, H, "ϰ", "\\varkappa"), d(g, B, G, "┌", "\\@ulcorner", !0), d(g, B, pt, "┐", "\\@urcorner", !0), d(g, B, G, "└", "\\@llcorner", !0), d(g, B, pt, "┘", "\\@lrcorner", !0), d(g, B, x, "≦", "\\leqq", !0), d(g, B, x, "⩽", "\\leqslant", !0), d(g, B, x, "⪕", "\\eqslantless", !0), d(g, B, x, "≲", "\\lesssim", !0), d(g, B, x, "⪅", "\\lessapprox", !0), d(g, B, x, "≊", "\\approxeq", !0), d(g, B, fe, "⋖", "\\lessdot"), d(g, B, x, "⋘", "\\lll", !0), d(g, B, x, "≶", "\\lessgtr", !0), d(g, B, x, "⋚", "\\lesseqgtr", !0), d(g, B, x, "⪋", "\\lesseqqgtr", !0), d(g, B, x, "≑", "\\doteqdot"), d(g, B, x, "≓", "\\risingdotseq", !0), d(g, B, x, "≒", "\\fallingdotseq", !0), d(g, B, x, "∽", "\\backsim", !0), d(g, B, x, "⋍", "\\backsimeq", !0), d(g, B, x, "⫅", "\\subseteqq", !0), d(g, B, x, "⋐", "\\Subset", !0), d(g, B, x, "⊏", "\\sqsubset", !0), d(g, B, x, "≼", "\\preccurlyeq", !0), d(g, B, x, "⋞", "\\curlyeqprec", !0), d(g, B, x, "≾", "\\precsim", !0), d(g, B, x, "⪷", "\\precapprox", !0), d(g, B, x, "⊲", "\\vartriangleleft"), d(g, B, x, "⊴", "\\trianglelefteq"), d(g, B, x, "⊨", "\\vDash", !0), d(g, B, x, "⊪", "\\Vvdash", !0), d(g, B, x, "⌣", "\\smallsmile"), d(g, B, x, "⌢", "\\smallfrown"), d(g, B, x, "≏", "\\bumpeq", !0), d(g, B, x, "≎", "\\Bumpeq", !0), d(g, B, x, "≧", "\\geqq", !0), d(g, B, x, "⩾", "\\geqslant", !0), d(g, B, x, "⪖", "\\eqslantgtr", !0), d(g, B, x, "≳", "\\gtrsim", !0), d(g, B, x, "⪆", "\\gtrapprox", !0), d(g, B, fe, "⋗", "\\gtrdot"), d(g, B, x, "⋙", "\\ggg", !0), d(g, B, x, "≷", "\\gtrless", !0), d(g, B, x, "⋛", "\\gtreqless", !0), d(g, B, x, "⪌", "\\gtreqqless", !0), d(g, B, x, "≖", "\\eqcirc", !0), d(g, B, x, "≗", "\\circeq", !0), d(g, B, x, "≜", "\\triangleq", !0), d(g, B, x, "∼", "\\thicksim"), d(g, B, x, "≈", "\\thickapprox"), d(g, B, x, "⫆", "\\supseteqq", !0), d(g, B, x, "⋑", "\\Supset", !0), d(g, B, x, "⊐", "\\sqsupset", !0), d(g, B, x, "≽", "\\succcurlyeq", !0), d(g, B, x, "⋟", "\\curlyeqsucc", !0), d(g, B, x, "≿", "\\succsim", !0), d(g, B, x, "⪸", "\\succapprox", !0), d(g, B, x, "⊳", "\\vartriangleright"), d(g, B, x, "⊵", "\\trianglerighteq"), d(g, B, x, "⊩", "\\Vdash", !0), d(g, B, x, "∣", "\\shortmid"), d(g, B, x, "∥", "\\shortparallel"), d(g, B, x, "≬", "\\between", !0), d(g, B, x, "⋔", "\\pitchfork", !0), d(g, B, x, "∝", "\\varpropto"), d(g, B, x, "◀", "\\blacktriangleleft"), d(g, B, x, "∴", "\\therefore", !0), d(g, B, x, "∍", "\\backepsilon"), d(g, B, x, "▶", "\\blacktriangleright"), d(g, B, x, "∵", "\\because", !0), d(g, B, x, "⋘", "\\llless"), d(g, B, x, "⋙", "\\gggtr"), d(g, B, fe, "⊲", "\\lhd"), d(g, B, fe, "⊳", "\\rhd"), d(g, B, x, "≂", "\\eqsim", !0), d(g, y, x, "⋈", "\\Join"), d(g, B, x, "≑", "\\Doteq", !0), d(g, B, fe, "∔", "\\dotplus", !0), d(g, B, fe, "∖", "\\smallsetminus"), d(g, B, fe, "⋒", "\\Cap", !0), d(g, B, fe, "⋓", "\\Cup", !0), d(g, B, fe, "⩞", "\\doublebarwedge", !0), d(g, B, fe, "⊟", "\\boxminus", !0), d(g, B, fe, "⊞", "\\boxplus", !0), d(g, B, fe, "⋇", "\\divideontimes", !0), d(g, B, fe, "⋉", "\\ltimes", !0), d(g, B, fe, "⋊", "\\rtimes", !0), d(g, B, fe, "⋋", "\\leftthreetimes", !0), d(g, B, fe, "⋌", "\\rightthreetimes", !0), d(g, B, fe, "⋏", "\\curlywedge", !0), d(g, B, fe, "⋎", "\\curlyvee", !0), d(g, B, fe, "⊝", "\\circleddash", !0), d(g, B, fe, "⊛", "\\circledast", !0), d(g, B, fe, "⋅", "\\centerdot"), d(g, B, fe, "⊺", "\\intercal", !0), d(g, B, fe, "⋒", "\\doublecap"), d(g, B, fe, "⋓", "\\doublecup"), d(g, B, fe, "⊠", "\\boxtimes", !0), d(g, B, x, "⇢", "\\dashrightarrow", !0), d(g, B, x, "⇠", "\\dashleftarrow", !0), d(g, B, x, "⇇", "\\leftleftarrows", !0), d(g, B, x, "⇆", "\\leftrightarrows", !0), d(g, B, x, "⇚", "\\Lleftarrow", !0), d(g, B, x, "↞", "\\twoheadleftarrow", !0), d(g, B, x, "↢", "\\leftarrowtail", !0), d(g, B, x, "↫", "\\looparrowleft", !0), d(g, B, x, "⇋", "\\leftrightharpoons", !0), d(g, B, x, "↶", "\\curvearrowleft", !0), d(g, B, x, "↺", "\\circlearrowleft", !0), d(g, B, x, "↰", "\\Lsh", !0), d(g, B, x, "⇈", "\\upuparrows", !0), d(g, B, x, "↿", "\\upharpoonleft", !0), d(g, B, x, "⇃", "\\downharpoonleft", !0), d(g, y, x, "⊶", "\\origof", !0), d(g, y, x, "⊷", "\\imageof", !0), d(g, B, x, "⊸", "\\multimap", !0), d(g, B, x, "↭", "\\leftrightsquigarrow", !0), d(g, B, x, "⇉", "\\rightrightarrows", !0), d(g, B, x, "⇄", "\\rightleftarrows", !0), d(g, B, x, "↠", "\\twoheadrightarrow", !0), d(g, B, x, "↣", "\\rightarrowtail", !0), d(g, B, x, "↬", "\\looparrowright", !0), d(g, B, x, "↷", "\\curvearrowright", !0), d(g, B, x, "↻", "\\circlearrowright", !0), d(g, B, x, "↱", "\\Rsh", !0), d(g, B, x, "⇊", "\\downdownarrows", !0), d(g, B, x, "↾", "\\upharpoonright", !0), d(g, B, x, "⇂", "\\downharpoonright", !0), d(g, B, x, "⇝", "\\rightsquigarrow", !0), d(g, B, x, "⇝", "\\leadsto"), d(g, B, x, "⇛", "\\Rrightarrow", !0), d(g, B, x, "↾", "\\restriction"), d(g, y, H, "‘", "`"), d(g, y, H, "$", "\\$"), d(Z, y, H, "$", "\\$"), d(Z, y, H, "$", "\\textdollar"), d(g, y, H, "%", "\\%"), d(Z, y, H, "%", "\\%"), d(g, y, H, "_", "\\_"), d(Z, y, H, "_", "\\_"), d(Z, y, H, "_", "\\textunderscore"), d(g, y, H, "∠", "\\angle", !0), d(g, y, H, "∞", "\\infty", !0), d(g, y, H, "′", "\\prime"), d(g, y, H, "△", "\\triangle"), d(g, y, H, "Γ", "\\Gamma", !0), d(g, y, H, "Δ", "\\Delta", !0), d(g, y, H, "Θ", "\\Theta", !0), d(g, y, H, "Λ", "\\Lambda", !0), d(g, y, H, "Ξ", "\\Xi", !0), d(g, y, H, "Π", "\\Pi", !0), d(g, y, H, "Σ", "\\Sigma", !0), d(g, y, H, "Υ", "\\Upsilon", !0), d(g, y, H, "Φ", "\\Phi", !0), d(g, y, H, "Ψ", "\\Psi", !0), d(g, y, H, "Ω", "\\Omega", !0), d(g, y, H, "A", "Α"), d(g, y, H, "B", "Β"), d(g, y, H, "E", "Ε"), d(g, y, H, "Z", "Ζ"), d(g, y, H, "H", "Η"), d(g, y, H, "I", "Ι"), d(g, y, H, "K", "Κ"), d(g, y, H, "M", "Μ"), d(g, y, H, "N", "Ν"), d(g, y, H, "O", "Ο"), d(g, y, H, "P", "Ρ"), d(g, y, H, "T", "Τ"), d(g, y, H, "X", "Χ"), d(g, y, H, "¬", "\\neg", !0), d(g, y, H, "¬", "\\lnot"), d(g, y, H, "⊤", "\\top"), d(g, y, H, "⊥", "\\bot"), d(g, y, H, "∅", "\\emptyset"), d(g, B, H, "∅", "\\varnothing"), d(g, y, De, "α", "\\alpha", !0), d(g, y, De, "β", "\\beta", !0), d(g, y, De, "γ", "\\gamma", !0), d(g, y, De, "δ", "\\delta", !0), d(g, y, De, "ϵ", "\\epsilon", !0), d(g, y, De, "ζ", "\\zeta", !0), d(g, y, De, "η", "\\eta", !0), d(g, y, De, "θ", "\\theta", !0), d(g, y, De, "ι", "\\iota", !0), d(g, y, De, "κ", "\\kappa", !0), d(g, y, De, "λ", "\\lambda", !0), d(g, y, De, "μ", "\\mu", !0), d(g, y, De, "ν", "\\nu", !0), d(g, y, De, "ξ", "\\xi", !0), d(g, y, De, "ο", "\\omicron", !0), d(g, y, De, "π", "\\pi", !0), d(g, y, De, "ρ", "\\rho", !0), d(g, y, De, "σ", "\\sigma", !0), d(g, y, De, "τ", "\\tau", !0), d(g, y, De, "υ", "\\upsilon", !0), d(g, y, De, "ϕ", "\\phi", !0), d(g, y, De, "χ", "\\chi", !0), d(g, y, De, "ψ", "\\psi", !0), d(g, y, De, "ω", "\\omega", !0), d(g, y, De, "ε", "\\varepsilon", !0), d(g, y, De, "ϑ", "\\vartheta", !0), d(g, y, De, "ϖ", "\\varpi", !0), d(g, y, De, "ϱ", "\\varrho", !0), d(g, y, De, "ς", "\\varsigma", !0), d(g, y, De, "φ", "\\varphi", !0), d(g, y, fe, "∗", "*", !0), d(g, y, fe, "+", "+"), d(g, y, fe, "−", "-", !0), d(g, y, fe, "⋅", "\\cdot", !0), d(g, y, fe, "∘", "\\circ", !0), d(g, y, fe, "÷", "\\div", !0), d(g, y, fe, "±", "\\pm", !0), d(g, y, fe, "×", "\\times", !0), d(g, y, fe, "∩", "\\cap", !0), d(g, y, fe, "∪", "\\cup", !0), d(g, y, fe, "∖", "\\setminus", !0), d(g, y, fe, "∧", "\\land"), d(g, y, fe, "∨", "\\lor"), d(g, y, fe, "∧", "\\wedge", !0), d(g, y, fe, "∨", "\\vee", !0), d(g, y, H, "√", "\\surd"), d(g, y, G, "⟨", "\\langle", !0), d(g, y, G, "∣", "\\lvert"), d(g, y, G, "∥", "\\lVert"), d(g, y, pt, "?", "?"), d(g, y, pt, "!", "!"), d(g, y, pt, "⟩", "\\rangle", !0), d(g, y, pt, "∣", "\\rvert"), d(g, y, pt, "∥", "\\rVert"), d(g, y, x, "=", "="), d(g, y, x, ":", ":"), d(g, y, x, "≈", "\\approx", !0), d(g, y, x, "≅", "\\cong", !0), d(g, y, x, "≥", "\\ge"), d(g, y, x, "≥", "\\geq", !0), d(g, y, x, "←", "\\gets"), d(g, y, x, ">", "\\gt", !0), d(g, y, x, "∈", "\\in", !0), d(g, y, x, "", "\\@not"), d(g, y, x, "⊂", "\\subset", !0), d(g, y, x, "⊃", "\\supset", !0), d(g, y, x, "⊆", "\\subseteq", !0), d(g, y, x, "⊇", "\\supseteq", !0), d(g, B, x, "⊈", "\\nsubseteq", !0), d(g, B, x, "⊉", "\\nsupseteq", !0), d(g, y, x, "⊨", "\\models"), d(g, y, x, "←", "\\leftarrow", !0), d(g, y, x, "≤", "\\le"), d(g, y, x, "≤", "\\leq", !0), d(g, y, x, "<", "\\lt", !0), d(g, y, x, "→", "\\rightarrow", !0), d(g, y, x, "→", "\\to"), d(g, B, x, "≱", "\\ngeq", !0), d(g, B, x, "≰", "\\nleq", !0), d(g, y, Ye, " ", "\\ "), d(g, y, Ye, " ", "\\space"), d(g, y, Ye, " ", "\\nobreakspace"), d(Z, y, Ye, " ", "\\ "), d(Z, y, Ye, " ", " "), d(Z, y, Ye, " ", "\\space"), d(Z, y, Ye, " ", "\\nobreakspace"), d(g, y, Ye, null, "\\nobreak"), d(g, y, Ye, null, "\\allowbreak"), d(g, y, ie, ",", ","), d(g, y, ie, ";", ";"), d(g, B, fe, "⊼", "\\barwedge", !0), d(g, B, fe, "⊻", "\\veebar", !0), d(g, y, fe, "⊙", "\\odot", !0), d(g, y, fe, "⊕", "\\oplus", !0), d(g, y, fe, "⊗", "\\otimes", !0), d(g, y, H, "∂", "\\partial", !0), d(g, y, fe, "⊘", "\\oslash", !0), d(g, B, fe, "⊚", "\\circledcirc", !0), d(g, B, fe, "⊡", "\\boxdot", !0), d(g, y, fe, "△", "\\bigtriangleup"), d(g, y, fe, "▽", "\\bigtriangledown"), d(g, y, fe, "†", "\\dagger"), d(g, y, fe, "⋄", "\\diamond"), d(g, y, fe, "⋆", "\\star"), d(g, y, fe, "◃", "\\triangleleft"), d(g, y, fe, "▹", "\\triangleright"), d(g, y, G, "{", "\\{"), d(Z, y, H, "{", "\\{"), d(Z, y, H, "{", "\\textbraceleft"), d(g, y, pt, "}", "\\}"), d(Z, y, H, "}", "\\}"), d(Z, y, H, "}", "\\textbraceright"), d(g, y, G, "{", "\\lbrace"), d(g, y, pt, "}", "\\rbrace"), d(g, y, G, "[", "\\lbrack", !0), d(Z, y, H, "[", "\\lbrack", !0), d(g, y, pt, "]", "\\rbrack", !0), d(Z, y, H, "]", "\\rbrack", !0), d(g, y, G, "(", "\\lparen", !0), d(g, y, pt, ")", "\\rparen", !0), d(Z, y, H, "<", "\\textless", !0), d(Z, y, H, ">", "\\textgreater", !0), d(g, y, G, "⌊", "\\lfloor", !0), d(g, y, pt, "⌋", "\\rfloor", !0), d(g, y, G, "⌈", "\\lceil", !0), d(g, y, pt, "⌉", "\\rceil", !0), d(g, y, H, "\\", "\\backslash"), d(g, y, H, "∣", "|"), d(g, y, H, "∣", "\\vert"), d(Z, y, H, "|", "\\textbar", !0), d(g, y, H, "∥", "\\|"), d(g, y, H, "∥", "\\Vert"), d(Z, y, H, "∥", "\\textbardbl"), d(Z, y, H, "~", "\\textasciitilde"), d(Z, y, H, "\\", "\\textbackslash"), d(Z, y, H, "^", "\\textasciicircum"), d(g, y, x, "↑", "\\uparrow", !0), d(g, y, x, "⇑", "\\Uparrow", !0), d(g, y, x, "↓", "\\downarrow", !0), d(g, y, x, "⇓", "\\Downarrow", !0), d(g, y, x, "↕", "\\updownarrow", !0), d(g, y, x, "⇕", "\\Updownarrow", !0), d(g, y, ce, "∐", "\\coprod"), d(g, y, ce, "⋁", "\\bigvee"), d(g, y, ce, "⋀", "\\bigwedge"), d(g, y, ce, "⨄", "\\biguplus"), d(g, y, ce, "⋂", "\\bigcap"), d(g, y, ce, "⋃", "\\bigcup"), d(g, y, ce, "∫", "\\int"), d(g, y, ce, "∫", "\\intop"), d(g, y, ce, "∬", "\\iint"), d(g, y, ce, "∭", "\\iiint"), d(g, y, ce, "∏", "\\prod"), d(g, y, ce, "∑", "\\sum"), d(g, y, ce, "⨂", "\\bigotimes"), d(g, y, ce, "⨁", "\\bigoplus"), d(g, y, ce, "⨀", "\\bigodot"), d(g, y, ce, "∮", "\\oint"), d(g, y, ce, "∯", "\\oiint"), d(g, y, ce, "∰", "\\oiiint"), d(g, y, ce, "⨆", "\\bigsqcup"), d(g, y, ce, "∫", "\\smallint"), d(Z, y, Dn, "…", "\\textellipsis"), d(g, y, Dn, "…", "\\mathellipsis"), d(Z, y, Dn, "…", "\\ldots", !0), d(g, y, Dn, "…", "\\ldots", !0), d(g, y, Dn, "⋯", "\\@cdots", !0), d(g, y, Dn, "⋱", "\\ddots", !0), d(g, y, H, "⋮", "\\varvdots"), d(g, y, ze, "ˊ", "\\acute"), d(g, y, ze, "ˋ", "\\grave"), d(g, y, ze, "¨", "\\ddot"), d(g, y, ze, "~", "\\tilde"), d(g, y, ze, "ˉ", "\\bar"), d(g, y, ze, "˘", "\\breve"), d(g, y, ze, "ˇ", "\\check"), d(g, y, ze, "^", "\\hat"), d(g, y, ze, "⃗", "\\vec"), d(g, y, ze, "˙", "\\dot"), d(g, y, ze, "˚", "\\mathring"), d(g, y, De, "", "\\@imath"), d(g, y, De, "", "\\@jmath"), d(g, y, H, "ı", "ı"), d(g, y, H, "ȷ", "ȷ"), d(Z, y, H, "ı", "\\i", !0), d(Z, y, H, "ȷ", "\\j", !0), d(Z, y, H, "ß", "\\ss", !0), d(Z, y, H, "æ", "\\ae", !0), d(Z, y, H, "œ", "\\oe", !0), d(Z, y, H, "ø", "\\o", !0), d(Z, y, H, "Æ", "\\AE", !0), d(Z, y, H, "Œ", "\\OE", !0), d(Z, y, H, "Ø", "\\O", !0), d(Z, y, ze, "ˊ", "\\'"), d(Z, y, ze, "ˋ", "\\`"), d(Z, y, ze, "ˆ", "\\^"), d(Z, y, ze, "˜", "\\~"), d(Z, y, ze, "ˉ", "\\="), d(Z, y, ze, "˘", "\\u"), d(Z, y, ze, "˙", "\\."), d(Z, y, ze, "¸", "\\c"), d(Z, y, ze, "˚", "\\r"), d(Z, y, ze, "ˇ", "\\v"), d(Z, y, ze, "¨", '\\"'), d(Z, y, ze, "˝", "\\H"), d(Z, y, ze, "◯", "\\textcircled");
                     const Lt = {
                         "--": !0,
                         "---": !0,
                         "``": !0,
                         "''": !0
                     };
                     d(Z, y, H, "–", "--", !0), d(Z, y, H, "–", "\\textendash"), d(Z, y, H, "—", "---", !0), d(Z, y, H, "—", "\\textemdash"), d(Z, y, H, "‘", "`", !0), d(Z, y, H, "‘", "\\textquoteleft"), d(Z, y, H, "’", "'", !0), d(Z, y, H, "’", "\\textquoteright"), d(Z, y, H, "“", "``", !0), d(Z, y, H, "“", "\\textquotedblleft"), d(Z, y, H, "”", "''", !0), d(Z, y, H, "”", "\\textquotedblright"), d(g, y, H, "°", "\\degree", !0), d(Z, y, H, "°", "\\degree"), d(Z, y, H, "°", "\\textdegree", !0), d(g, y, H, "£", "\\pounds"), d(g, y, H, "£", "\\mathsterling", !0), d(Z, y, H, "£", "\\pounds"), d(Z, y, H, "£", "\\textsterling", !0), d(g, B, H, "✠", "\\maltese"), d(Z, B, H, "✠", "\\maltese");
@@ -12305,18 +12305,18 @@
                         Nt = function(i) {
                             return i.type === "ordgroup" ? i.body : [i];
                         },
                         a0 = X.makeSpan,
                         _d = ["leftmost", "mbin", "mopen", "mrel", "mop", "mpunct"],
                         bd = ["rightmost", "mrel", "mclose", "mpunct"],
                         wd = {
-                            display: Q.DISPLAY,
-                            text: Q.TEXT,
-                            script: Q.SCRIPT,
-                            scriptscript: Q.SCRIPTSCRIPT
+                            display: K.DISPLAY,
+                            text: K.TEXT,
+                            script: K.SCRIPT,
+                            scriptscript: K.SCRIPTSCRIPT
                         },
                         yd = {
                             mord: "mord",
                             mop: "mop",
                             mbin: "mbin",
                             mrel: "mrel",
                             mopen: "mopen",
@@ -12665,15 +12665,15 @@
                             L = new se.MathNode("math", [F]);
                         L.setAttribute("xmlns", "http://www.w3.org/1998/Math/MathML"), f && L.setAttribute("display", "block");
                         const j = m ? "katex" : "katex-mathml";
                         return X.makeSpan([j], [L]);
                     }
                     const Do = function(i) {
                             return new Rt({
-                                style: i.displayMode ? Q.DISPLAY : Q.TEXT,
+                                style: i.displayMode ? K.DISPLAY : K.TEXT,
                                 maxSize: i.maxSize,
                                 minRuleThickness: i.minRuleThickness
                             });
                         },
                         Ao = function(i, s) {
                             if (s.displayMode) {
                                 const a = ["katex-display"];
@@ -13900,16 +13900,16 @@
                             return a && zo(A, f, s), A;
                         },
                         Od = function(i, s, a, f) {
                             return X.makeSymbol(i, "Size" + s + "-Regular", a, f);
                         },
                         Ro = function(i, s, a, f, m, b) {
                             const w = Od(i, s, m, f),
-                                A = cl(X.makeSpan(["delimsizing", "size" + s], [w], f), Q.TEXT, f, b);
-                            return a && zo(A, f, Q.TEXT), A;
+                                A = cl(X.makeSpan(["delimsizing", "size" + s], [w], f), K.TEXT, f, b);
+                            return a && zo(A, f, K.TEXT), A;
                         },
                         fl = function(i, s, a) {
                             let f;
                             return s === "Size1-Regular" ? f = "delim-size1" : f = "delim-size4", {
                                 type: "elem",
                                 elem: X.makeSpan(["delimsizinginner", f], [X.makeSpan([], [X.makeSymbol(i, s, a)])])
                             };
@@ -13986,21 +13986,21 @@
                                     ot.push(hl(F, Mt, f));
                                 } else {
                                     const Mt = (xn - be - Ke - lt) / 2 + 2 * dl;
                                     ot.push(hl(F, Mt, f)), ot.push(Ls), ot.push(fl(A, J, m)), ot.push(Ls), ot.push(hl(F, Mt, f));
                                 }
                                 ot.push(Ls), ot.push(fl(w, J, m));
                             }
-                            const gt = f.havingBaseStyle(Q.TEXT),
+                            const gt = f.havingBaseStyle(K.TEXT),
                                 yt = X.makeVList({
                                     positionType: "bottom",
                                     positionData: rt,
                                     children: ot
                                 }, gt);
-                            return cl(X.makeSpan(["delimsizing", "mult"], [yt], gt), Q.TEXT, f, b);
+                            return cl(X.makeSpan(["delimsizing", "mult"], [yt], gt), K.TEXT, f, b);
                         },
                         ml = 80,
                         pl = 0.08,
                         gl = function(i, s, a, f, m) {
                             const b = zt(i, f, a),
                                 w = new dn(i, b),
                                 A = new en([w], {
@@ -14040,21 +14040,21 @@
                                 return Ro(i, s, !1, a, f, m);
                             if (M.contains(Pd, i))
                                 return Oo(i, Ur[s], !1, a, f, m);
                             throw new o("Illegal delimiter: '" + i + "'");
                         },
                         Ud = [{
                             type: "small",
-                            style: Q.SCRIPTSCRIPT
+                            style: K.SCRIPTSCRIPT
                         }, {
                             type: "small",
-                            style: Q.SCRIPT
+                            style: K.SCRIPT
                         }, {
                             type: "small",
-                            style: Q.TEXT
+                            style: K.TEXT
                         }, {
                             type: "large",
                             size: 1
                         }, {
                             type: "large",
                             size: 2
                         }, {
@@ -14062,33 +14062,33 @@
                             size: 3
                         }, {
                             type: "large",
                             size: 4
                         }],
                         Gd = [{
                             type: "small",
-                            style: Q.SCRIPTSCRIPT
+                            style: K.SCRIPTSCRIPT
                         }, {
                             type: "small",
-                            style: Q.SCRIPT
+                            style: K.SCRIPT
                         }, {
                             type: "small",
-                            style: Q.TEXT
+                            style: K.TEXT
                         }, {
                             type: "stack"
                         }],
                         Ho = [{
                             type: "small",
-                            style: Q.SCRIPTSCRIPT
+                            style: K.SCRIPTSCRIPT
                         }, {
                             type: "small",
-                            style: Q.SCRIPT
+                            style: K.SCRIPT
                         }, {
                             type: "small",
-                            style: Q.TEXT
+                            style: K.TEXT
                         }, {
                             type: "large",
                             size: 1
                         }, {
                             type: "large",
                             size: 2
                         }, {
@@ -14784,15 +14784,15 @@
                                     // From LaTeX \showthe\arrayrulewidth. Equals 0.04 em.
                                     s.fontMetrics().arrayRuleWidth,
                                     s.minRuleThickness
                                     // User override.
                                 ),
                                 j = 1 / s.fontMetrics().ptPerEm;
                             let W = 5 * j;
-                            i.colSeparationType && i.colSeparationType === "small" && (W = 0.2778 * (s.havingStyle(Q.SCRIPT).sizeMultiplier / s.sizeMultiplier));
+                            i.colSeparationType && i.colSeparationType === "small" && (W = 0.2778 * (s.havingStyle(K.SCRIPT).sizeMultiplier / s.sizeMultiplier));
                             const J = i.colSeparationType === "CD" ? Ze({
                                     number: 3,
                                     unit: "ex"
                                 }, s) : 12 * j,
                                 te = 3 * j,
                                 be = i.arraystretch * J,
                                 Te = 0.7 * be,
@@ -15426,15 +15426,15 @@
                             };
                         },
                         htmlBuilder: Zo,
                         mathmlBuilder: Jo
                     });
                     const Ko = (i, s) => {
                             let a = s;
-                            return i === "display" ? a = a.id >= Q.SCRIPT.id ? a.text() : Q.DISPLAY : i === "text" && a.size === Q.DISPLAY.size ? a = Q.TEXT : i === "script" ? a = Q.SCRIPT : i === "scriptscript" && (a = Q.SCRIPTSCRIPT), a;
+                            return i === "display" ? a = a.id >= K.SCRIPT.id ? a.text() : K.DISPLAY : i === "text" && a.size === K.DISPLAY.size ? a = K.TEXT : i === "script" ? a = K.SCRIPT : i === "scriptscript" && (a = K.SCRIPTSCRIPT), a;
                         },
                         vl = (i, s) => {
                             const a = Ko(i.size, s.style),
                                 f = a.fracNum(),
                                 m = a.fracDen();
                             let b;
                             b = s.havingStyle(f);
@@ -15445,15 +15445,15 @@
                                 w.height = w.height < Ke ? Ke : w.height, w.depth = w.depth < lt ? lt : w.depth;
                             }
                             b = s.havingStyle(m);
                             const A = nt(i.denom, b, s);
                             let F, L, j;
                             i.hasBarLine ? (i.barSize ? (L = Ze(i.barSize, s), F = X.makeLineSpan("frac-line", s, L)) : F = X.makeLineSpan("frac-line", s), L = F.height, j = F.height) : (F = null, L = 0, j = s.fontMetrics().defaultRuleThickness);
                             let W, J, te;
-                            a.size === Q.DISPLAY.size || i.size === "display" ? (W = s.fontMetrics().num1, L > 0 ? J = 3 * j : J = 7 * j, te = s.fontMetrics().denom1) : (L > 0 ? (W = s.fontMetrics().num2, J = j) : (W = s.fontMetrics().num3, J = 3 * j), te = s.fontMetrics().denom2);
+                            a.size === K.DISPLAY.size || i.size === "display" ? (W = s.fontMetrics().num1, L > 0 ? J = 3 * j : J = 7 * j, te = s.fontMetrics().denom1) : (L > 0 ? (W = s.fontMetrics().num2, J = j) : (W = s.fontMetrics().num3, J = 3 * j), te = s.fontMetrics().denom2);
                             let be;
                             if (F) {
                                 const Ke = s.fontMetrics().axisHeight;
                                 W - w.depth - (Ke + 0.5 * L) < J && (W += J - (W - w.depth - (Ke + 0.5 * L))), Ke - 0.5 * L - (A.height - te) < J && (te += J - (Ke - 0.5 * L - (A.height - te)));
                                 const lt = -(Ke - 0.5 * L);
                                 be = X.makeVList({
                                     positionType: "individualShift",
@@ -15484,30 +15484,30 @@
                                         elem: w,
                                         shift: -W
                                     }]
                                 }, s);
                             }
                             b = s.havingStyle(a), be.height *= b.sizeMultiplier / s.sizeMultiplier, be.depth *= b.sizeMultiplier / s.sizeMultiplier;
                             let Te;
-                            a.size === Q.DISPLAY.size ? Te = s.fontMetrics().delim1 : a.size === Q.SCRIPTSCRIPT.size ? Te = s.havingStyle(Q.SCRIPT).fontMetrics().delim2 : Te = s.fontMetrics().delim2;
+                            a.size === K.DISPLAY.size ? Te = s.fontMetrics().delim1 : a.size === K.SCRIPTSCRIPT.size ? Te = s.havingStyle(K.SCRIPT).fontMetrics().delim2 : Te = s.fontMetrics().delim2;
                             let Je, Ge;
                             return i.leftDelim == null ? Je = Hr(s, ["mopen"]) : Je = u0.customSizedDelim(i.leftDelim, Te, !0, s.havingStyle(a), i.mode, ["mopen"]), i.continued ? Ge = X.makeSpan([]) : i.rightDelim == null ? Ge = Hr(s, ["mclose"]) : Ge = u0.customSizedDelim(i.rightDelim, Te, !0, s.havingStyle(a), i.mode, ["mclose"]), X.makeSpan(["mord"].concat(b.sizingClasses(s)), [Je, X.makeSpan(["mfrac"], [be]), Ge], s);
                         },
                         kl = (i, s) => {
                             let a = new se.MathNode("mfrac", [ft(i.numer, s), ft(i.denom, s)]);
                             if (!i.hasBarLine)
                                 a.setAttribute("linethickness", "0px");
                             else if (i.barSize) {
                                 const m = Ze(i.barSize, s);
                                 a.setAttribute("linethickness", ae(m));
                             }
                             const f = Ko(i.size, s.style);
                             if (f.size !== s.style.size) {
                                 a = new se.MathNode("mstyle", [a]);
-                                const m = f.size === Q.DISPLAY.size ? "true" : "false";
+                                const m = f.size === K.DISPLAY.size ? "true" : "false";
                                 a.setAttribute("displaystyle", m), a.setAttribute("scriptlevel", "0");
                             }
                             if (i.leftDelim != null || i.rightDelim != null) {
                                 const m = [];
                                 if (i.leftDelim != null) {
                                     const b = new se.MathNode("mo", [new se.TextNode(i.leftDelim.replace("\\", ""))]);
                                     b.setAttribute("fence", "true"), m.push(b);
@@ -15767,15 +15767,15 @@
                         htmlBuilder: vl,
                         mathmlBuilder: kl
                     });
                     const tu = (i, s) => {
                         const a = s.style;
                         let f, m;
                         i.type === "supsub" ? (f = i.sup ? nt(i.sup, s.havingStyle(a.sup()), s) : nt(i.sub, s.havingStyle(a.sub()), s), m = He(i.base, "horizBrace")) : m = He(i, "horizBrace");
-                        const b = nt(m.base, s.havingBaseStyle(Q.DISPLAY)),
+                        const b = nt(m.base, s.havingBaseStyle(K.DISPLAY)),
                             w = o0.svgSpan(m, s);
                         let A;
                         if (m.isOver ? (A = X.makeVList({
                                 positionType: "firstBaseline",
                                 children: [{
                                     type: "elem",
                                     elem: b
@@ -16257,21 +16257,21 @@
                         },
                         handler(i, s) {
                             throw new o("Mismatched " + i.funcName);
                         }
                     });
                     const nu = (i, s) => {
                         switch (s.style.size) {
-                            case Q.DISPLAY.size:
+                            case K.DISPLAY.size:
                                 return i.display;
-                            case Q.TEXT.size:
+                            case K.TEXT.size:
                                 return i.text;
-                            case Q.SCRIPT.size:
+                            case K.SCRIPT.size:
                                 return i.script;
-                            case Q.SCRIPTSCRIPT.size:
+                            case K.SCRIPTSCRIPT.size:
                                 return i.scriptscript;
                             default:
                                 return i.text;
                         }
                     };
                     _e({
                         type: "mathchoice",
@@ -16404,15 +16404,15 @@
                         su = ["\\smallint"],
                         ur = (i, s) => {
                             let a, f, m = !1,
                                 b;
                             i.type === "supsub" ? (a = i.sup, f = i.sub, b = He(i.base, "op"), m = !0) : b = He(i, "op");
                             const w = s.style;
                             let A = !1;
-                            w.size === Q.DISPLAY.size && b.symbol && !M.contains(su, b.name) && (A = !0);
+                            w.size === K.DISPLAY.size && b.symbol && !M.contains(su, b.name) && (A = !0);
                             let F;
                             if (b.symbol) {
                                 const W = A ? "Size2-Regular" : "Size1-Regular";
                                 let J = "";
                                 if ((b.name === "\\oiint" || b.name === "\\oiiint") && (J = b.name.slice(1), b.name = J === "oiint" ? "\\iint" : "\\iiint"), F = X.makeSymbol(b.name, W, "math", s, ["mop", "op-symbol", A ? "large-op" : "small-op"]), J.length > 0) {
                                     const te = F.italic,
                                         be = X.staticSvg(J + "Size" + (A ? "2" : "1"), s);
@@ -17032,15 +17032,15 @@
                             };
                         },
                         htmlBuilder(i, s) {
                             let a = nt(i.body, s.havingCrampedStyle());
                             a.height === 0 && (a.height = s.fontMetrics().xHeight), a = X.wrapFragment(a, s);
                             const m = s.fontMetrics().defaultRuleThickness;
                             let b = m;
-                            s.style.id < Q.TEXT.id && (b = s.fontMetrics().xHeight);
+                            s.style.id < K.TEXT.id && (b = s.fontMetrics().xHeight);
                             let w = m + b / 4;
                             const A = a.height + a.depth + w + m,
                                 {
                                     span: F,
                                     ruleWidth: L,
                                     advanceWidth: j
                                 } = u0.sqrtImage(A, s),
@@ -17062,15 +17062,15 @@
                                     elem: F
                                 }, {
                                     type: "kern",
                                     size: L
                                 }]
                             }, s);
                             if (i.index) {
-                                const be = s.havingStyle(Q.SCRIPTSCRIPT),
+                                const be = s.havingStyle(K.SCRIPTSCRIPT),
                                     Te = nt(i.index, be, s),
                                     Je = 0.6 * (te.height - te.depth),
                                     Ge = X.makeVList({
                                         positionType: "shift",
                                         positionData: -Je,
                                         children: [{
                                             type: "elem",
@@ -17087,18 +17087,18 @@
                                 body: a,
                                 index: f
                             } = i;
                             return f ? new se.MathNode("mroot", [ft(a, s), ft(f, s)]) : new se.MathNode("msqrt", [ft(a, s)]);
                         }
                     });
                     const ou = {
-                        display: Q.DISPLAY,
-                        text: Q.TEXT,
-                        script: Q.SCRIPT,
-                        scriptscript: Q.SCRIPTSCRIPT
+                        display: K.DISPLAY,
+                        text: K.TEXT,
+                        script: K.SCRIPT,
+                        scriptscript: K.SCRIPTSCRIPT
                     };
                     _e({
                         type: "styling",
                         names: ["\\displaystyle", "\\textstyle", "\\scriptstyle", "\\scriptscriptstyle"],
                         props: {
                             numArgs: 0,
                             allowedInText: !0,
@@ -17138,15 +17138,15 @@
                                     scriptscript: ["2", "false"]
                                 } [i.style];
                             return b.setAttribute("scriptlevel", A[0]), b.setAttribute("displaystyle", A[1]), b;
                         }
                     });
                     const Zd = function(i, s) {
                         const a = i.base;
-                        return a ? a.type === "op" ? a.limits && (s.style.size === Q.DISPLAY.size || a.alwaysHandleSupSub) ? ur : null : a.type === "operatorname" ? a.alwaysHandleSupSub && (s.style.size === Q.DISPLAY.size || a.limits) ? iu : null : a.type === "accent" ? M.isCharacterBox(a.base) ? ol : null : a.type === "horizBrace" && !i.sub === a.isOver ? tu : null : null;
+                        return a ? a.type === "op" ? a.limits && (s.style.size === K.DISPLAY.size || a.alwaysHandleSupSub) ? ur : null : a.type === "operatorname" ? a.alwaysHandleSupSub && (s.style.size === K.DISPLAY.size || a.limits) ? iu : null : a.type === "accent" ? M.isCharacterBox(a.base) ? ol : null : a.type === "horizBrace" && !i.sub === a.isOver ? tu : null : null;
                     };
                     G0({
                         type: "supsub",
                         htmlBuilder(i, s) {
                             const a = Zd(i, s);
                             if (a)
                                 return a(i, s);
@@ -17165,15 +17165,15 @@
                                 A = nt(m, lt, s), J || (j = w.height - lt.fontMetrics().supDrop * lt.sizeMultiplier / s.sizeMultiplier);
                             }
                             if (b) {
                                 const lt = s.havingStyle(s.style.sub());
                                 F = nt(b, lt, s), J || (W = w.depth + lt.fontMetrics().subDrop * lt.sizeMultiplier / s.sizeMultiplier);
                             }
                             let te;
-                            s.style === Q.DISPLAY ? te = L.sup1 : s.style.cramped ? te = L.sup3 : te = L.sup2;
+                            s.style === K.DISPLAY ? te = L.sup1 : s.style.cramped ? te = L.sup3 : te = L.sup2;
                             const be = s.sizeMultiplier,
                                 Te = ae(0.5 / L.ptPerEm / be);
                             let Je = null;
                             if (F) {
                                 const lt = i.base && i.base.type === "op" && i.base.name && (i.base.name === "\\oiint" || i.base.name === "\\oiiint");
                                 (w instanceof jt || lt) && (Je = ae(-w.italic));
                             }
@@ -17238,22 +17238,22 @@
                             i.sub && b.push(ft(i.sub, s)), i.sup && b.push(ft(i.sup, s));
                             let w;
                             if (a)
                                 w = f ? "mover" : "munder";
                             else if (i.sub)
                                 if (i.sup) {
                                     const A = i.base;
-                                    A && A.type === "op" && A.limits && s.style === Q.DISPLAY || A && A.type === "operatorname" && A.alwaysHandleSupSub && (s.style === Q.DISPLAY || A.limits) ? w = "munderover" : w = "msubsup";
+                                    A && A.type === "op" && A.limits && s.style === K.DISPLAY || A && A.type === "operatorname" && A.alwaysHandleSupSub && (s.style === K.DISPLAY || A.limits) ? w = "munderover" : w = "msubsup";
                                 } else {
                                     const A = i.base;
-                                    A && A.type === "op" && A.limits && (s.style === Q.DISPLAY || A.alwaysHandleSupSub) || A && A.type === "operatorname" && A.alwaysHandleSupSub && (A.limits || s.style === Q.DISPLAY) ? w = "munder" : w = "msub";
+                                    A && A.type === "op" && A.limits && (s.style === K.DISPLAY || A.alwaysHandleSupSub) || A && A.type === "operatorname" && A.alwaysHandleSupSub && (A.limits || s.style === K.DISPLAY) ? w = "munder" : w = "msub";
                                 }
                             else {
                                 const A = i.base;
-                                A && A.type === "op" && A.limits && (s.style === Q.DISPLAY || A.alwaysHandleSupSub) || A && A.type === "operatorname" && A.alwaysHandleSupSub && (A.limits || s.style === Q.DISPLAY) ? w = "mover" : w = "msup";
+                                A && A.type === "op" && A.limits && (s.style === K.DISPLAY || A.alwaysHandleSupSub) || A && A.type === "operatorname" && A.alwaysHandleSupSub && (A.limits || s.style === K.DISPLAY) ? w = "mover" : w = "msup";
                             }
                             return new se.MathNode(w, b);
                         }
                     }), G0({
                         type: "atom",
                         htmlBuilder(i, s) {
                             return X.mathsym(i.text, i.mode, s, ["m" + i.family]);
@@ -22031,51 +22031,51 @@
                     for (var ne = 0; ne < Y.length; ++ne) {
                         if (I && I.cause == z + "," + ne)
                             return;
                         var re = Y[ne],
                             pe = re.inside,
                             Me = !!re.lookbehind,
                             Ne = !!re.greedy,
-                            ke = re.alias;
+                            ve = re.alias;
                         if (Ne && !re.pattern.global) {
-                            var ce = re.pattern.toString().match(/[imsuy]*$/)[0];
-                            re.pattern = RegExp(re.pattern.source, ce + "g");
+                            var ue = re.pattern.toString().match(/[imsuy]*$/)[0];
+                            re.pattern = RegExp(re.pattern.source, ue + "g");
                         }
                         for (var he = re.pattern || re, le = C.next, Be = R; le !== D.tail && !(I && Be >= I.reach); Be += le.value.length, le = le.next) {
                             var oe = le.value;
                             if (D.length > N.length)
                                 return;
                             if (!(oe instanceof h)) {
-                                var Q = 1,
+                                var K = 1,
                                     de;
                                 if (Ne) {
                                     if (de = p(he, Be, N, Me), !de || de.index >= N.length)
                                         break;
-                                    var ve = de.index,
+                                    var ke = de.index,
                                         V = de.index + de[0].length,
                                         ee = Be;
-                                    for (ee += le.value.length; ve >= ee;)
+                                    for (ee += le.value.length; ke >= ee;)
                                         le = le.next, ee += le.value.length;
                                     if (ee -= le.value.length, Be = ee, le.value instanceof h)
                                         continue;
                                     for (var we = le; we !== D.tail && (ee < V || typeof we.value == "string"); we = we.next)
-                                        Q++, ee += we.value.length;
-                                    Q--, oe = N.slice(Be, ee), de.index -= Be;
+                                        K++, ee += we.value.length;
+                                    K--, oe = N.slice(Be, ee), de.index -= Be;
                                 } else if (de = p(he, 0, oe, Me), !de)
                                     continue;
-                                var ve = de.index,
+                                var ke = de.index,
                                     $ = de[0],
-                                    xe = oe.slice(0, ve),
-                                    Se = oe.slice(ve + $.length),
+                                    xe = oe.slice(0, ke),
+                                    Se = oe.slice(ke + $.length),
                                     We = Be + oe.length;
                                 I && We > I.reach && (I.reach = We);
                                 var Ie = le.prev;
-                                xe && (Ie = k(D, Ie, xe), Be += xe.length), T(D, Ie, Q);
-                                var Xe = new h(z, pe ? u.tokenize($, pe) : $, ke, $);
-                                if (le = k(D, Ie, Xe), Se && k(D, le, Se), Q > 1) {
+                                xe && (Ie = k(D, Ie, xe), Be += xe.length), T(D, Ie, K);
+                                var Xe = new h(z, pe ? u.tokenize($, pe) : $, ve, $);
+                                if (le = k(D, Ie, Xe), Se && k(D, le, Se), K > 1) {
                                     var Ue = {
                                         cause: z + "," + ne,
                                         reach: We
                                     };
                                     _(N, D, E, le.prev, Be, Ue), I && Ue.reach > I.reach && (I.reach = Ue.reach);
                                 }
                             }
@@ -24286,16 +24286,16 @@
         R, I = !1,
         z = 0,
         Y = 0,
         ne = null,
         re = null,
         pe = 0,
         Me = null,
-        Ne, ke = null,
-        ce = !0;
+        Ne, ve = null,
+        ue = !0;
     const he = () => {
         n(0, u = n(26, ne = n(19, oe = null))), n(24, z = performance.now()), n(25, Y = 0), I = !0, le();
     };
 
     function le() {
         requestAnimationFrame(() => {
             n(25, Y = (performance.now() - z) / 1e3), I && le();
@@ -24306,38 +24306,38 @@
         n(25, Y = 0), n(0, u = n(26, ne = n(19, oe = null))), I && (I = !1);
     }
     g6(() => {
         I && Be();
     });
     let oe = null;
 
-    function Q(V) {
+    function K(V) {
         qc[V ? "unshift" : "push"](() => {
-            ke = V, n(16, ke), n(7, P), n(14, Me), n(15, Ne);
+            ve = V, n(16, ve), n(7, P), n(14, Me), n(15, Ne);
         });
     }
 
     function de(V) {
         qc[V ? "unshift" : "push"](() => {
             R = V, n(13, R);
         });
     }
     return t.$$set = (V) => {
         "i18n" in V && n(1, c = V.i18n), "eta" in V && n(0, u = V.eta), "queue_position" in V && n(2, h = V.queue_position), "queue_size" in V && n(3, p = V.queue_size), "status" in V && n(4, _ = V.status), "scroll_to_output" in V && n(21, v = V.scroll_to_output), "timer" in V && n(5, k = V.timer), "show_progress" in V && n(6, T = V.show_progress), "message" in V && n(22, O = V.message), "progress" in V && n(7, P = V.progress), "variant" in V && n(8, U = V.variant), "loading_text" in V && n(9, M = V.loading_text), "absolute" in V && n(10, N = V.absolute), "translucent" in V && n(11, D = V.translucent), "border" in V && n(12, E = V.border), "autoscroll" in V && n(23, C = V.autoscroll), "$$scope" in V && n(28, o = V.$$scope);
     }, t.$$.update = () => {
         t.$$.dirty[0] & /*eta, old_eta, timer_start, eta_from_start*/
             218103809 && (u === null && n(0, u = ne), u != null && ne !== u && (n(27, re = (performance.now() - z) / 1e3 + u), n(19, oe = re.toFixed(1)), n(26, ne = u))), t.$$.dirty[0] & /*eta_from_start, timer_diff*/
             167772160 && n(17, pe = re === null || re <= 0 || !Y ? null : Math.min(Y / re, 1)), t.$$.dirty[0] & /*progress*/
-            128 && P != null && n(18, ce = !1), t.$$.dirty[0] & /*progress, progress_level, progress_bar, last_progress_level*/
+            128 && P != null && n(18, ue = !1), t.$$.dirty[0] & /*progress, progress_level, progress_bar, last_progress_level*/
             114816 && (P != null ? n(14, Me = P.map((V) => {
                 if (V.index != null && V.length != null)
                     return V.index / V.length;
                 if (V.progress != null)
                     return V.progress;
-            })) : n(14, Me = null), Me ? (n(15, Ne = Me[Me.length - 1]), ke && (Ne === 0 ? n(16, ke.style.transition = "0", ke) : n(16, ke.style.transition = "150ms", ke))) : n(15, Ne = void 0)), t.$$.dirty[0] & /*status*/
+            })) : n(14, Me = null), Me ? (n(15, Ne = Me[Me.length - 1]), ve && (Ne === 0 ? n(16, ve.style.transition = "0", ve) : n(16, ve.style.transition = "150ms", ve))) : n(15, Ne = void 0)), t.$$.dirty[0] & /*status*/
             16 && (_ === "pending" ? he() : Be()), t.$$.dirty[0] & /*el, scroll_to_output, status, autoscroll*/
             10493968 && R && v && (_ === "pending" || _ === "complete") && F6(R, C), t.$$.dirty[0] & /*status, message*/
             4194320, t.$$.dirty[0] & /*timer_diff*/
             33554432 && n(20, r = Y.toFixed(1));
     }, [
         u,
         c,
@@ -24351,29 +24351,29 @@
         M,
         N,
         D,
         E,
         R,
         Me,
         Ne,
-        ke,
+        ve,
         pe,
-        ce,
+        ue,
         oe,
         r,
         v,
         O,
         C,
         z,
         Y,
         ne,
         re,
         o,
         l,
-        Q,
+        K,
         de
     ];
 }
 class io extends i6 {
     constructor(e) {
         super(), f6(
             this,
@@ -25212,23 +25212,23 @@
         P, U = 0,
         M = 0,
         N = [],
         D, E, C = 0,
         R, I = 0,
         z = [],
         Y, ne = 0;
-    async function re(Q) {
+    async function re(K) {
         if (I === 0)
             return;
         const {
             scrollTop: de
         } = R;
         n(13, p = R.offsetWidth - R.clientWidth), ne = C - (de - U);
         let V = _;
-        for (; ne < u && V < Q.length;) {
+        for (; ne < u && V < K.length;) {
             let $ = E[V - _];
             $ || (n(11, v = V + 1), await ti(), $ = E[V - _]);
             let xe = p1([
                 $,
                 "optionalAccess",
                 (We) => We.getBoundingClientRect,
                 "call",
@@ -25237,136 +25237,136 @@
                 (We) => We.height
             ]);
             xe || (xe = T);
             const Se = N[V] = xe;
             ne += Se, V += 1;
         }
         n(11, v = V);
-        const ee = Q.length - v,
+        const ee = K.length - v,
             we = R.offsetHeight - R.clientHeight;
         we > 0 && (ne += we);
-        let ve = N.filter(($) => typeof $ == "number");
-        n(1, T = ve.reduce(($, xe) => $ + xe, 0) / ve.length), n(2, O = ee * T), N.length = Q.length, await ti(), u ? ne < u ? n(12, h = ne + 2) : n(12, h = u) : n(12, h = ne + 1), await ti();
+        let ke = N.filter(($) => typeof $ == "number");
+        n(1, T = ke.reduce(($, xe) => $ + xe, 0) / ke.length), n(2, O = ee * T), N.length = K.length, await ti(), u ? ne < u ? n(12, h = ne + 2) : n(12, h = u) : n(12, h = ne + 1), await ti();
     }
-    async function pe(Q) {
+    async function pe(K) {
         requestAnimationFrame(async () => {
-            if (typeof Q != "number")
+            if (typeof K != "number")
                 return;
-            const de = typeof Q != "number" ? !1 : Me(Q);
-            de !== !0 && (de === "back" && await ke(Q, {
+            const de = typeof K != "number" ? !1 : Me(K);
+            de !== !0 && (de === "back" && await ve(K, {
                 behavior: "instant"
-            }), de === "forwards" && await ke(Q, {
+            }), de === "forwards" && await ve(K, {
                 behavior: "instant"
             }, !0));
         });
     }
 
-    function Me(Q) {
-        const de = E && E[Q - _];
-        if (!de && Q < _)
+    function Me(K) {
+        const de = E && E[K - _];
+        if (!de && K < _)
             return "back";
-        if (!de && Q >= v - 1)
+        if (!de && K >= v - 1)
             return "forwards";
         const {
             top: V
         } = R.getBoundingClientRect(), {
             top: ee,
             bottom: we
         } = de.getBoundingClientRect();
         return ee - V < 37 ? "back" : we - V > I ? "forwards" : !0;
     }
-    async function Ne(Q) {
+    async function Ne(K) {
         const de = R.scrollTop;
         E = P.children;
         const V = r.length < _,
             ee = p7(E[1], "border-top-width"),
             we = 0;
-        V && await ke(r.length - 1, {
+        V && await ve(r.length - 1, {
             behavior: "auto"
         });
-        let ve = 0;
+        let ke = 0;
         for (let Xe = 0; Xe < E.length; Xe += 1)
             N[_ + Xe] = E[Xe].getBoundingClientRect().height;
         let $ = 0,
             xe = U + ee / 2,
             Se = [];
         for (; $ < r.length;) {
             const Xe = N[$] || T;
             if (Se[$] = Xe, xe + Xe + we > de) {
-                ve = $, n(6, C = xe - (U + ee / 2));
+                ke = $, n(6, C = xe - (U + ee / 2));
                 break;
             }
             xe += Xe, $ += 1;
         }
-        for (ve = Math.max(0, ve); $ < r.length;) {
+        for (ke = Math.max(0, ke); $ < r.length;) {
             const Xe = N[$] || T;
             if (xe += Xe, $ += 1, xe > de + I)
                 break;
         }
-        n(10, _ = ve), n(11, v = $);
+        n(10, _ = ke), n(11, v = $);
         const We = r.length - v;
         v === 0 && n(11, v = 10), n(1, T = (xe - U) / v);
         let Ie = We * T;
         for (; $ < r.length;)
             $ += 1, N[$] = T;
         n(2, O = Ie), isFinite(O) || n(2, O = 2e5);
     }
-    async function ke(Q, de, V = !1) {
+    async function ve(K, de, V = !1) {
         await ti();
         const ee = T;
-        let we = Q * ee;
+        let we = K * ee;
         V && (we = we - I + ee + U);
-        const ve = R.offsetHeight - R.clientHeight;
-        ve > 0 && (we += ve);
+        const ke = R.offsetHeight - R.clientHeight;
+        ke > 0 && (we += ke);
         const $ = {
             top: we,
             behavior: "smooth",
             ...de
         };
         R.scrollTo($);
     }
     o7(() => {
         E = P.children, n(18, D = !0), re(c);
     });
 
-    function ce() {
+    function ue() {
         U = this.offsetHeight, n(4, U);
     }
 
-    function he(Q) {
-        l1[Q ? "unshift" : "push"](() => {
-            P = Q, n(3, P);
+    function he(K) {
+        l1[K ? "unshift" : "push"](() => {
+            P = K, n(3, P);
         });
     }
 
     function le() {
         M = this.offsetHeight, n(5, M);
     }
 
-    function Be(Q) {
-        l1[Q ? "unshift" : "push"](() => {
-            R = Q, n(7, R);
+    function Be(K) {
+        l1[K ? "unshift" : "push"](() => {
+            R = K, n(7, R);
         });
     }
 
     function oe() {
-        var Q;
-        Y = (Q = $6.entries.get(this)) == null ? void 0 : Q.contentRect, n(0, Y);
+        var K;
+        Y = (K = $6.entries.get(this)) == null ? void 0 : K.contentRect, n(0, Y);
     }
-    return t.$$set = (Q) => {
-        "items" in Q && n(14, c = Q.items), "max_height" in Q && n(15, u = Q.max_height), "actual_height" in Q && n(12, h = Q.actual_height), "table_scrollbar_width" in Q && n(13, p = Q.table_scrollbar_width), "start" in Q && n(10, _ = Q.start), "end" in Q && n(11, v = Q.end), "selected" in Q && n(16, k = Q.selected), "$$scope" in Q && n(20, o = Q.$$scope);
+    return t.$$set = (K) => {
+        "items" in K && n(14, c = K.items), "max_height" in K && n(15, u = K.max_height), "actual_height" in K && n(12, h = K.actual_height), "table_scrollbar_width" in K && n(13, p = K.table_scrollbar_width), "start" in K && n(10, _ = K.start), "end" in K && n(11, v = K.end), "selected" in K && n(16, k = K.selected), "$$scope" in K && n(20, o = K.$$scope);
     }, t.$$.update = () => {
         t.$$.dirty[0] & /*viewport_box*/
-            1 && (I = p1([Y, "optionalAccess", (Q) => Q.height]) || 0), t.$$.dirty[0] & /*items*/
+            1 && (I = p1([Y, "optionalAccess", (K) => K.height]) || 0), t.$$.dirty[0] & /*items*/
             16384 && n(19, r = c), t.$$.dirty[0] & /*mounted, sortedItems*/
             786432 && D && requestAnimationFrame(() => re(r)), t.$$.dirty[0] & /*selected*/
             65536 && pe(k), t.$$.dirty[0] & /*sortedItems, start, end*/
-            527360 && n(8, z = r.slice(_, v).map((Q, de) => ({
+            527360 && n(8, z = r.slice(_, v).map((K, de) => ({
                 index: de + _,
-                data: Q
+                data: K
             })));
     }, [
         Y,
         T,
         O,
         P,
         U,
@@ -25378,20 +25378,20 @@
         _,
         v,
         h,
         p,
         c,
         u,
         k,
-        ke,
+        ve,
         D,
         r,
         o,
         l,
-        ce,
+        ue,
         he,
         le,
         Be,
         oe
     ];
 }
 class _7 extends e7 {
@@ -26772,39 +26772,39 @@
             t[1] && /*label*/
             t[1].length !== 0 && v1(t)
         ),
         Y = F0(
             /*_headers*/
             t[24]
         );
-    const ne = (ce) => (
+    const ne = (ue) => (
         /*id*/
-        ce[90]
+        ue[90]
     );
-    for (let ce = 0; ce < Y.length; ce += 1) {
-        let he = w1(t, Y, ce),
+    for (let ue = 0; ue < Y.length; ue += 1) {
+        let he = w1(t, Y, ue),
             le = ne(he);
-        p.set(le, h[ce] = k1(le, he));
+        p.set(le, h[ue] = k1(le, he));
     }
     let re = F0(
         /*max*/
         t[35]
     );
-    const pe = (ce) => (
+    const pe = (ue) => (
         /*id*/
-        ce[90]
+        ue[90]
     );
-    for (let ce = 0; ce < re.length; ce += 1) {
-        let he = b1(t, re, ce),
+    for (let ue = 0; ue < re.length; ue += 1) {
+        let he = b1(t, re, ue),
             le = pe(he);
-        O.set(le, T[ce] = D1(le, he));
+        O.set(le, T[ue] = D1(le, he));
     }
 
-    function Me(ce) {
-        t[69](ce);
+    function Me(ue) {
+        t[69](ue);
     }
     let Ne = {
         flex: !1,
         center: !1,
         boundedheight: !1,
         disable_click: !0,
         root: (
@@ -26823,27 +26823,27 @@
         t[29]), M = new $3({
         props: Ne
     }), Hn.push(() => N0(M, "dragging", Me)), M.$on(
         "load",
         /*load_handler*/
         t[70]
     );
-    let ke = (
+    let ve = (
         /*editable*/
         t[6] && F1(t)
     );
     return {
         c() {
             e = bt("div"), I && I.c(), n = hn(), r = bt("div"), l = bt("table"), z && z.c(), o = hn(), c = bt("thead"), u = bt("tr");
-            for (let ce = 0; ce < h.length; ce += 1)
-                h[ce].c();
+            for (let ue = 0; ue < h.length; ue += 1)
+                h[ue].c();
             _ = hn(), v = bt("tbody"), k = bt("tr");
-            for (let ce = 0; ce < T.length; ce += 1)
-                T[ce].c();
-            U = hn(), L0(M.$$.fragment), D = hn(), ke && ke.c(), ge(u, "class", "svelte-13e3mz4"), ge(c, "class", "svelte-13e3mz4"), ge(k, "class", "svelte-13e3mz4"), ge(l, "class", "svelte-13e3mz4"), kt(
+            for (let ue = 0; ue < T.length; ue += 1)
+                T[ue].c();
+            U = hn(), L0(M.$$.fragment), D = hn(), ve && ve.c(), ge(u, "class", "svelte-13e3mz4"), ge(c, "class", "svelte-13e3mz4"), ge(k, "class", "svelte-13e3mz4"), ge(l, "class", "svelte-13e3mz4"), kt(
                 l,
                 "fixed-layout",
                 /*column_widths*/
                 t[12].length != 0
             ), ge(r, "class", "table-wrap svelte-13e3mz4"), z0(
                 r,
                 "height",
@@ -26859,26 +26859,26 @@
                 e,
                 "label",
                 /*label*/
                 t[1] && /*label*/
                 t[1].length !== 0
             );
         },
-        m(ce, he) {
-            St(ce, e, he), I && I.m(e, null), it(e, n), it(e, r), it(r, l), z && z.m(l, null), it(l, o), it(l, c), it(c, u);
+        m(ue, he) {
+            St(ue, e, he), I && I.m(e, null), it(e, n), it(e, r), it(r, l), z && z.m(l, null), it(l, o), it(l, c), it(c, u);
             for (let le = 0; le < h.length; le += 1)
                 h[le] && h[le].m(u, null);
             it(l, _), it(l, v), it(v, k);
             for (let le = 0; le < T.length; le += 1)
                 T[le] && T[le].m(k, null);
             P = k7.observe(
                 l,
                 /*table_1_elementresizecontentbox_handler*/
                 t[54].bind(l)
-            ), t[55](l), it(r, U), P0(M, r, null), t[71](r), it(e, D), ke && ke.m(e, null), E = !0, C || (R = [
+            ), t[55](l), it(r, U), P0(M, r, null), t[71](r), it(e, D), ve && ve.m(e, null), E = !0, C || (R = [
                 C0(
                     window,
                     "click",
                     /*handle_click_outside*/
                     t[45]
                 ),
                 C0(
@@ -26898,98 +26898,98 @@
                     "keydown",
                     /*keydown_handler*/
                     t[72]
                 ),
                 y7(mm.call(null, e))
             ], C = !0);
         },
-        p(ce, he) {
+        p(ue, he) {
             /*label*/
-            ce[1] && /*label*/
-                ce[1].length !== 0 && /*show_label*/
-                ce[2] ? I ? I.p(ce, he) : (I = y1(ce), I.c(), I.m(e, n)) : I && (I.d(1), I = null), /*label*/
-                ce[1] && /*label*/
-                ce[1].length !== 0 ? z ? z.p(ce, he) : (z = v1(ce), z.c(), z.m(l, o)) : z && (z.d(1), z = null), he[0] & /*_headers, sort_by, sort_direction, header_edit, column_widths, latex_delimiters, line_breaks*/
+            ue[1] && /*label*/
+                ue[1].length !== 0 && /*show_label*/
+                ue[2] ? I ? I.p(ue, he) : (I = y1(ue), I.c(), I.m(e, n)) : I && (I.d(1), I = null), /*label*/
+                ue[1] && /*label*/
+                ue[1].length !== 0 ? z ? z.p(ue, he) : (z = v1(ue), z.c(), z.m(l, o)) : z && (z.d(1), z = null), he[0] & /*_headers, sort_by, sort_direction, header_edit, column_widths, latex_delimiters, line_breaks*/
                 84678688 | he[1] & /*get_sort_status*/
                 32 && (Y = F0(
                     /*_headers*/
-                    ce[24]
-                ), d0(), h = Oi(h, he, ne, 1, ce, Y, p, u, Ri, k1, null, w1), h0()), he[0] & /*cells, latex_delimiters, line_breaks, datatype*/
+                    ue[24]
+                ), d0(), h = Oi(h, he, ne, 1, ue, Y, p, u, Ri, k1, null, w1), h0()), he[0] & /*cells, latex_delimiters, line_breaks, datatype*/
                 1050657 | he[1] & /*max*/
                 16 && (re = F0(
                     /*max*/
-                    ce[35]
-                ), d0(), T = Oi(T, he, pe, 1, ce, re, O, k, Ri, D1, null, b1), h0()), (!E || he[0] & /*column_widths*/
+                    ue[35]
+                ), d0(), T = Oi(T, he, pe, 1, ue, re, O, k, Ri, D1, null, b1), h0()), (!E || he[0] & /*column_widths*/
                     4096) && kt(
                     l,
                     "fixed-layout",
                     /*column_widths*/
-                    ce[12].length != 0
+                    ue[12].length != 0
                 );
             const le = {};
             he[0] & /*root*/
                 256 && (le.root = /*root*/
-                    ce[8]), he[0] & /*height, data, styling, selected, display_value, latex_delimiters, line_breaks, editable, editing, datatype, clear_on_focus, els, parent, hide_columns, _headers, sort_by, sort_direction, header_edit, selected_header, select_on_focus, label*/
+                    ue[8]), he[0] & /*height, data, styling, selected, display_value, latex_delimiters, line_breaks, editable, editing, datatype, clear_on_focus, els, parent, hide_columns, _headers, sort_by, sort_direction, header_edit, selected_header, select_on_focus, label*/
                 1607461987 | he[1] & /*selected_index, table_height, scrollbar_width*/
                 14 | he[3] & /*$$scope*/
                 16 && (le.$$scope = {
                     dirty: he,
-                    ctx: ce
+                    ctx: ue
                 }), !N && he[0] & /*dragging*/
                 536870912 && (N = !0, le.dragging = /*dragging*/
-                    ce[29], B0(() => N = !1)), M.$set(le), (!E || he[1] & /*table_height*/
+                    ue[29], B0(() => N = !1)), M.$set(le), (!E || he[1] & /*table_height*/
                     2) && z0(
                     r,
                     "height",
                     /*table_height*/
-                    ce[32] + "px"
+                    ue[32] + "px"
                 ), (!E || he[0] & /*dragging*/
                     536870912) && kt(
                     r,
                     "dragging",
                     /*dragging*/
-                    ce[29]
+                    ue[29]
                 ), (!E || he[0] & /*wrap*/
                     128) && kt(r, "no-wrap", ! /*wrap*/
-                    ce[7]), /*editable*/
-                ce[6] ? ke ? (ke.p(ce, he), he[0] & /*editable*/
-                    64 && ht(ke, 1)) : (ke = F1(ce), ke.c(), ht(ke, 1), ke.m(e, null)) : ke && (d0(), Bt(ke, 1, 1, () => {
-                    ke = null;
+                    ue[7]), /*editable*/
+                ue[6] ? ve ? (ve.p(ue, he), he[0] & /*editable*/
+                    64 && ht(ve, 1)) : (ve = F1(ue), ve.c(), ht(ve, 1), ve.m(e, null)) : ve && (d0(), Bt(ve, 1, 1, () => {
+                    ve = null;
                 }), h0()), (!E || he[0] & /*label*/
                     2) && kt(
                     e,
                     "label",
                     /*label*/
-                    ce[1] && /*label*/
-                    ce[1].length !== 0
+                    ue[1] && /*label*/
+                    ue[1].length !== 0
                 );
         },
-        i(ce) {
+        i(ue) {
             if (!E) {
                 for (let he = 0; he < Y.length; he += 1)
                     ht(h[he]);
                 for (let he = 0; he < re.length; he += 1)
                     ht(T[he]);
-                ht(M.$$.fragment, ce), ht(ke), E = !0;
+                ht(M.$$.fragment, ue), ht(ve), E = !0;
             }
         },
-        o(ce) {
+        o(ue) {
             for (let he = 0; he < h.length; he += 1)
                 Bt(h[he]);
             for (let he = 0; he < T.length; he += 1)
                 Bt(T[he]);
-            Bt(M.$$.fragment, ce), Bt(ke), E = !1;
+            Bt(M.$$.fragment, ue), Bt(ve), E = !1;
         },
-        d(ce) {
-            ce && At(e), I && I.d(), z && z.d();
+        d(ue) {
+            ue && At(e), I && I.d(), z && z.d();
             for (let he = 0; he < h.length; he += 1)
                 h[he].d();
             for (let he = 0; he < T.length; he += 1)
                 T[he].d();
-            P(), t[55](null), H0(M), t[71](null), ke && ke.d(), C = !1, Wh(R);
+            P(), t[55](null), H0(M), t[71](null), ve && ve.d(), C = !1, Wh(R);
         }
     };
 }
 
 function B1(t, e) {
     return t ?? e();
 }
@@ -27146,38 +27146,38 @@
                 cell: null
             }, pe), {
                 value: B1(mr([q, "optionalAccess", (pt) => pt[Z], "optionalAccess", (pt) => pt[B]]), () => ""),
                 id: ze
             };
         }));
     }
-    let ke = Me(h),
-        ce;
+    let ve = Me(h),
+        ue;
 
     function he() {
-        n(24, ke = Me(h)), n(50, ce = h.slice()), oe();
+        n(24, ve = Me(h)), n(50, ue = h.slice()), oe();
     }
     let le = [
             []
         ],
         Be;
     async function oe() {
         Y("change", {
             data: le.map((q) => q.map(({
                 value: d
             }) => d)),
-            headers: ke.map((q) => q.value),
+            headers: ve.map((q) => q.value),
             metadata: T ? null : {
                 display_value: R,
                 styling: I
             }
         });
     }
 
-    function Q(q, d, g) {
+    function K(q, d, g) {
         if (!d)
             return "none";
         if (h[d] === q) {
             if (g === "asc")
                 return "ascending";
             if (g === "des")
                 return "descending";
@@ -27211,25 +27211,25 @@
             n(28, Ue = y), n(16, C = !1);
         else {
             const B = mr([le, "access", (ze) => ze[Z], "optionalAccess", (ze) => ze[y]]);
             n(16, C = B ? [Z, y] : C);
         }
     }
     let we = !1;
-    async function ve(q) {
+    async function ke(q) {
         if (Ue !== !1 && Ie === !1)
             switch (q.key) {
                 case "ArrowDown":
                     n(16, C = [0, Ue]), n(28, Ue = !1);
                     return;
                 case "ArrowLeft":
                     n(28, Ue = Ue > 0 ? Ue - 1 : Ue);
                     return;
                 case "ArrowRight":
-                    n(28, Ue = Ue < ke.length - 1 ? Ue + 1 : Ue);
+                    n(28, Ue = Ue < ve.length - 1 ? Ue + 1 : Ue);
                     return;
                 case "Escape":
                     q.preventDefault(), n(28, Ue = !1);
                     break;
                 case "Enter":
                     q.preventDefault();
                     break;
@@ -27270,17 +27270,17 @@
                 let Z = q.shiftKey ? -1 : 1,
                     y = le[d][g + Z],
                     B = mr([
                         le,
                         "optionalAccess",
                         (ze) => ze[d + Z],
                         "optionalAccess",
-                        (ze) => ze[Z > 0 ? 0 : ke.length - 1]
+                        (ze) => ze[Z > 0 ? 0 : ve.length - 1]
                     ]);
-                (y || B) && (q.preventDefault(), n(16, C = y ? [d, g + Z] : [d + Z, Z > 0 ? 0 : ke.length - 1])), n(22, ne = !1);
+                (y || B) && (q.preventDefault(), n(16, C = y ? [d, g + Z] : [d + Z, Z > 0 ? 0 : ve.length - 1])), n(22, ne = !1);
                 break;
             default:
                 if (!T)
                     break;
                 (!ne || ne && Cn(ne, [d, g])) && q.key.length === 1 && (n(25, we = !0), n(22, ne = [d, g]));
         }
     }
@@ -27363,19 +27363,19 @@
                     "optionalAccess",
                     (fe) => fe.target,
                     "optionalAccess",
                     (fe) => fe.result
                 ]) || typeof Z.target.result != "string")
                 return;
             const [y] = N7(Z.target.result, [",", "	"]), [B, ...ze] = wm(y).parseRows(Z.target.result);
-            n(24, ke = Me(_[1] === "fixed" ? B.slice(0, _[0]) : B)), n(49, p = ze), d.removeEventListener("loadend", g);
+            n(24, ve = Me(_[1] === "fixed" ? B.slice(0, _[0]) : B)), n(49, p = ze), d.removeEventListener("loadend", g);
         }
         d.addEventListener("loadend", g), d.readAsText(q);
     }
-    let K = !1;
+    let Q = !1;
 
     function ye(q) {
         let d = q[0].slice();
         for (let g = 0; g < q.length; g++)
             for (let Z = 0; Z < q[g].length; Z++)
                 `${d[Z].value}`.length < `${q[g][Z].value}`.length && (d[Z] = q[g][Z]);
         return d;
@@ -27394,27 +27394,27 @@
 
     function Le(q, d, g, Z, y) {
         let B = null;
         if (C && C[0] in le && C[1] in le[C[0]] && (B = le[C[0]][C[1]].id), typeof Z != "number" || !y)
             return;
         const ze = [...Array(q.length).keys()];
         if (y === "asc")
-            ze.sort((De, ue) => q[De][Z].value < q[ue][Z].value ? -1 : 1);
+            ze.sort((De, ce) => q[De][Z].value < q[ce][Z].value ? -1 : 1);
         else if (y === "des")
-            ze.sort((De, ue) => q[De][Z].value > q[ue][Z].value ? -1 : 1);
+            ze.sort((De, ce) => q[De][Z].value > q[ce][Z].value ? -1 : 1);
         else
             return;
         const fe = [...q],
             pt = d ? [...d] : null,
             Dn = g ? [...g] : null;
-        if (ze.forEach((De, ue) => {
-                q[ue] = fe[De], d && pt && (d[ue] = pt[De]), g && Dn && (g[ue] = Dn[De]);
+        if (ze.forEach((De, ce) => {
+                q[ce] = fe[De], d && pt && (d[ce] = pt[De]), g && Dn && (g[ce] = Dn[De]);
             }), n(17, le), n(49, p), n(51, Be), B) {
-            const [De, ue] = de(B);
-            n(16, C = [De, ue]);
+            const [De, ce] = de(B);
+            n(16, C = [De, ce]);
         }
     }
     let tt = !1;
     S7(() => {
         const q = new IntersectionObserver((d, g) => {
             d.forEach((Z) => {
                 Z.isIntersecting && !tt && (Oe(), n(17, le), n(49, p), n(51, Be)), tt = Z.isIntersecting;
@@ -27452,15 +27452,15 @@
     }
     const Ut = () => (n(25, we = !1), Ee.focus()),
         s0 = (q, d) => V(q, d),
         Pn = (q, d) => $(q, d),
         sr = (q, d) => V(q, d);
 
     function i0(q, d) {
-        t.$$.not_equal(ke[d].value, q) && (ke[d].value = q, n(24, ke));
+        t.$$.not_equal(ve[d].value, q) && (ve[d].value = q, n(24, ve));
     }
 
     function wt(q, d) {
         t.$$.not_equal(pe[d].input, q) && (pe[d].input = q, n(23, pe));
     }
     const qn = (q) => zt(q),
         Ir = (q) => We(q);
@@ -27474,39 +27474,39 @@
     }
 
     function dn(q) {
         Ce = q, n(33, Ce);
     }
 
     function g0(q) {
-        K = q, n(29, K);
+        Q = q, n(29, Q);
     }
     const ir = (q) => Ct(z7(q.detail.data));
 
     function lr(q) {
         Hn[q ? "unshift" : "push"](() => {
             Ee = q, n(30, Ee);
         });
     }
-    const ar = (q) => ve(q),
+    const ar = (q) => ke(q),
         Lr = (q) => (q.stopPropagation(), Re()),
         Qt = (q) => (q.stopPropagation(), $t());
     return t.$$set = (q) => {
         "datatype" in q && n(0, o = q.datatype), "label" in q && n(1, c = q.label), "show_label" in q && n(2, u = q.show_label), "headers" in q && n(48, h = q.headers), "values" in q && n(49, p = q.values), "col_count" in q && n(3, _ = q.col_count), "row_count" in q && n(4, v = q.row_count), "latex_delimiters" in q && n(5, k = q.latex_delimiters), "editable" in q && n(6, T = q.editable), "wrap" in q && n(7, O = q.wrap), "root" in q && n(8, P = q.root), "i18n" in q && n(9, U = q.i18n), "height" in q && n(10, M = q.height), "line_breaks" in q && n(11, N = q.line_breaks), "column_widths" in q && n(12, D = q.column_widths), "hide_columns" in q && n(13, E = q.hide_columns), "display_value" in q && n(14, R = q.display_value), "styling" in q && n(15, I = q.styling);
     }, t.$$.update = () => {
         if (t.$$.dirty[0] & /*selected*/
             65536 && C !== !1) {
             const [q, d] = C;
             !isNaN(q) && !isNaN(d) && Y("select", {
                 index: [q, d],
                 value: re(q, d)
             });
         }
         t.$$.dirty[1] & /*headers, old_headers*/
-            655360 && (Cn(h, ce) || he()), t.$$.dirty[1] & /*values, old_val*/
+            655360 && (Cn(h, ue) || he()), t.$$.dirty[1] & /*values, old_val*/
             1310720 && (Cn(p, Be) || (n(17, le = Ne(p)), n(51, Be = p))), t.$$.dirty[0] & /*data*/
             131072 && le && oe(), t.$$.dirty[0] & /*data*/
             131072 && n(35, r = ye(le)), t.$$.dirty[0] & /*cells*/
             1048576 && Fe[0] && Oe(), t.$$.dirty[0] & /*data, display_value, styling, sort_by, sort_direction*/
             966656 && Le(le, R, I, Se, xe), t.$$.dirty[0] & /*selected*/
             65536 && n(34, l = !!C && C[0]);
     }, [
@@ -27530,41 +27530,41 @@
         le,
         xe,
         Se,
         Fe,
         z,
         ne,
         pe,
-        ke,
+        ve,
         we,
         Ie,
         Xe,
         Ue,
-        K,
+        Q,
         Ee,
         me,
         et,
         Ce,
         l,
         r,
-        Q,
+        K,
         V,
-        ve,
+        ke,
         $,
         We,
         zt,
         Nn,
         Re,
         $t,
         Ot,
         Ct,
         Oe,
         h,
         p,
-        ce,
+        ue,
         Be,
         Rt,
         Jt,
         kn,
         It,
         Ze,
         ae,
@@ -30391,48 +30391,48 @@
         (h === null || Y.length < h) && (n(12, Y = [...Y, $]), re("select", {
             index: typeof $ == "number" ? $ : -1,
             value: typeof $ == "number" ? R[$] : $,
             selected: !0
         })), Y.length === h && (n(14, E = !1), n(16, z = null), M.blur());
     }
 
-    function ke($) {
+    function ve($) {
         const xe = parseInt($.detail.target.dataset.index);
-        ce(xe);
+        ue(xe);
     }
 
-    function ce($) {
+    function ue($) {
         Y.includes($) ? Me($) : Ne($), n(10, N = "");
     }
 
     function he($) {
         n(12, Y = []), n(10, N = ""), $.preventDefault();
     }
 
     function le($) {
         n(11, I = p.map((xe, Se) => Se)), (h === null || Y.length < h) && n(14, E = !0), re("focus");
     }
 
     function Be($) {
-        n(14, [E, z] = D9($, z, I), E, (n(16, z), n(3, p), n(27, _), n(10, N), n(28, D), n(7, O), n(11, I))), $.key === "Enter" && (z !== null ? ce(z) : O && (Ne(N), n(10, N = ""))), $.key === "Backspace" && N === "" && n(12, Y = [...Y.slice(0, -1)]), Y.length === h && (n(14, E = !1), n(16, z = null));
+        n(14, [E, z] = D9($, z, I), E, (n(16, z), n(3, p), n(27, _), n(10, N), n(28, D), n(7, O), n(11, I))), $.key === "Enter" && (z !== null ? ue(z) : O && (Ne(N), n(10, N = ""))), $.key === "Backspace" && N === "" && n(12, Y = [...Y.slice(0, -1)]), Y.length === h && (n(14, E = !1), n(16, z = null));
     }
 
     function oe() {
         o === void 0 ? n(12, Y = []) : Array.isArray(o) && n(12, Y = o.map(($) => {
             const xe = R.indexOf($);
             if (xe !== -1)
                 return xe;
             if (O)
                 return $;
         }).filter(($) => $ !== void 0));
     }
     F9(() => {
         n(25, u = !1);
     });
-    const Q = ($) => Me($),
+    const K = ($) => Me($),
         de = ($, xe) => {
             xe.key === "Enter" && Me($);
         };
 
     function V() {
         N = this.value, n(10, N);
     }
@@ -30442,15 +30442,15 @@
             M = $, n(13, M);
         });
     }
     const we = ($) => re("key_up", {
             key: $.key,
             input_value: N
         }),
-        ve = ($) => {
+        ke = ($) => {
             $.key === "Enter" && he($);
         };
     return t.$$set = ($) => {
         "label" in $ && n(0, r = $.label), "info" in $ && n(1, l = $.info), "value" in $ && n(24, o = $.value), "value_is_output" in $ && n(25, u = $.value_is_output), "max_choices" in $ && n(2, h = $.max_choices), "choices" in $ && n(3, p = $.choices), "disabled" in $ && n(4, v = $.disabled), "show_label" in $ && n(5, k = $.show_label), "container" in $ && n(6, T = $.container), "allow_custom_value" in $ && n(7, O = $.allow_custom_value), "filterable" in $ && n(8, P = $.filterable), "i18n" in $ && n(9, U = $.i18n);
     }, t.$$.update = () => {
         t.$$.dirty[0] & /*choices*/
             8 && (n(15, C = p.map(($) => $[0])), n(29, R = p.map(($) => $[1]))), t.$$.dirty[0] & /*choices, old_choices, input_text, old_input_text, allow_custom_value, filtered_indices*/
@@ -30475,31 +30475,31 @@
         M,
         E,
         C,
         z,
         re,
         pe,
         Me,
-        ke,
+        ve,
         he,
         le,
         Be,
         o,
         u,
         c,
         _,
         D,
         R,
         ne,
-        Q,
+        K,
         de,
         V,
         ee,
         we,
-        ve
+        ke
     ];
 }
 class O9 extends A9 {
     constructor(e) {
         super(), x9(
             this,
             e,
@@ -32033,18 +32033,18 @@
         latex_delimiters: ne
     } = e, {
         height: re = void 0
     } = e, {
         loading_status: pe
     } = e, {
         interactive: Me
-    } = e, Ne, ke = u.headers.map((K) => K), ce = u.data.map((K) => K), he, le, Be, oe = [], Q = null, de = E.default_selection.length ? E.default_selection : ke;
-    async function V(K) {
-        let ye = K || u;
-        n(20, Ne = ke), n(23, Be = ce ? [...ce] : []);
+    } = e, Ne, ve = u.headers.map((Q) => Q), ue = u.data.map((Q) => Q), he, le, Be, oe = [], K = null, de = E.default_selection.length ? E.default_selection : ve;
+    async function V(Q) {
+        let ye = Q || u;
+        n(20, Ne = ve), n(23, Be = ue ? [...ue] : []);
         const Fe = Ne.filter((me) => de.includes(me)),
             Ee = Fe.map((me) => Ne.indexOf(me));
         n(20, Ne = Fe), n(23, Be = Be.map((me) => Ee.map((Oe) => me[Oe]))), n(21, he = S0([
             ye,
             "optionalAccess",
             (me) => me.metadata,
             "optionalAccess",
@@ -32070,41 +32070,41 @@
                 (me) => me.metadata,
                 "optionalAccess",
                 (me) => me.styling
             ])
         ] : null), await o_(), Y.dispatch("change"), _ || Y.dispatch("input");
     }
 
-    function ee(K, ye) {
-        const Fe = ke.filter((me) => ye.includes(me)),
-            Ee = Fe.map((me) => ke.indexOf(me));
-        return n(20, Ne = Fe), K = K.map((me) => Ee.map((Oe) => me[Oe])), K;
+    function ee(Q, ye) {
+        const Fe = ve.filter((me) => ye.includes(me)),
+            Ee = Fe.map((me) => ve.indexOf(me));
+        return n(20, Ne = Fe), Q = Q.map((me) => Ee.map((Oe) => me[Oe])), Q;
     }
 
-    function we(K, ye) {
-        if (K.type === "checkbox" && !ye)
-            return Array(ce.length).fill(!0);
-        if (n(23, Be = ce), Array.isArray(ye) && !ye.length)
+    function we(Q, ye) {
+        if (Q.type === "checkbox" && !ye)
+            return Array(ue.length).fill(!0);
+        if (n(23, Be = ue), Array.isArray(ye) && !ye.length)
             return Array(Be.length).fill(!1);
         let Fe;
-        if (K.type === "slider") {
+        if (Q.type === "slider") {
             const [Ee, me] = ye;
-            Fe = (Oe) => v_(Oe[ke.indexOf(K.column)], Ee, me);
+            Fe = (Oe) => v_(Oe[ve.indexOf(Q.column)], Ee, me);
         } else
-            K.type == "checkbox" ? Fe = (Ee) => Ee[ke.indexOf(K.column)] === ye : Fe = (Ee) => ye.some((me) => Ee[ke.indexOf(K.column)] === me);
+            Q.type == "checkbox" ? Fe = (Ee) => Ee[ve.indexOf(Q.column)] === ye : Fe = (Ee) => ye.some((me) => Ee[ve.indexOf(Q.column)] === me);
         return Be.map(Fe);
     }
 
-    function ve(K, ye, Fe, Ee) {
+    function ke(Q, ye, Fe, Ee) {
         if (!Ee)
-            return new Array(K.length).fill(!0);
+            return new Array(Q.length).fill(!0);
         const me = Ee.split(";").map((Ce) => Ce.trim()).filter((Ce) => Ce.length),
-            Oe = new Array(K.length).fill(!1);
+            Oe = new Array(Q.length).fill(!1);
         let et = !1;
-        for (let Ce = 0; Ce < K.length; Ce++) {
+        for (let Ce = 0; Ce < Q.length; Ce++) {
             let Le = Array(),
                 tt = Array();
             for (let Rt = 0; Rt < me.length; Rt++) {
                 let Jt = me[Rt],
                     kn = ye.indexOf(Fe.primary_column);
                 const It = Jt.indexOf(":");
                 if (It !== -1) {
@@ -32113,79 +32113,79 @@
                         et || Y.dispatch("warning", `Column ${Ut} not found in secondary columns of search_columns`), et = !0;
                         continue;
                     }
                     const s0 = ye.indexOf(Ut);
                     s0 !== -1 && (kn = s0, Jt = Jt.substring(It + 1).trim());
                 }
                 const Ze = It !== -1 ? tt : Le;
-                (K[Ce][kn] === null ? "" : K[Ce][kn].toString()).toLowerCase().includes(Jt.toLowerCase()) ? Ze.push(!0) : Ze.push(!1);
+                (Q[Ce][kn] === null ? "" : Q[Ce][kn].toString()).toLowerCase().includes(Jt.toLowerCase()) ? Ze.push(!0) : Ze.push(!1);
             }
             Le.length && !tt.length ? Oe[Ce] = Le.some((Rt) => Rt) : tt.length && !Le.length ? Oe[Ce] = tt.every((Rt) => !!Rt) : Le.length && tt.length && (Oe[Ce] = Le.some((Rt) => Rt) && tt.every((Rt) => !!Rt));
         }
         return Oe;
     }
 
-    function $(K) {
-        return D.find((ye) => ye.column === K);
+    function $(Q) {
+        return D.find((ye) => ye.column === Q);
     }
 
-    function xe(K, ye, Fe, Ee, me) {
+    function xe(Q, ye, Fe, Ee, me) {
         console.log("filter_values", Fe);
-        const Oe = ve(ce, ye, Ee, me),
+        const Oe = ke(ue, ye, Ee, me),
             et = Fe.map((Ce) => we($(Ce[0]), Ce[1])).concat([Oe]);
-        return K.filter((Ce, Le) => et.every((tt) => tt[Le]));
+        return Q.filter((Ce, Le) => et.every((tt) => tt[Le]));
     }
 
-    function Se(K, ye, Fe) {
-        n(23, Be = ee(ce, K)), n(23, Be = xe(Be, ke, ye, R, Fe)), Be.length === 0 && n(23, Be = [Array(K.length).fill("")]);
+    function Se(Q, ye, Fe) {
+        n(23, Be = ee(ue, Q)), n(23, Be = xe(Be, ve, ye, R, Fe)), Be.length === 0 && n(23, Be = [Array(Q.length).fill("")]);
     }
     V(), a_(() => {
         n(27, _ = !1);
-    }), (Array.isArray(u) && S0([u, "optionalAccess", (K) => K[0], "optionalAccess", (K) => K.length]) === 0 || S0([
+    }), (Array.isArray(u) && S0([u, "optionalAccess", (Q) => Q[0], "optionalAccess", (Q) => Q.length]) === 0 || S0([
         u,
         "access",
-        (K) => K.data,
+        (Q) => Q.data,
         "optionalAccess",
-        (K) => K[0],
+        (Q) => Q[0],
         "optionalAccess",
-        (K) => K.length
+        (Q) => Q.length
     ]) === 0) && (u = {
         data: [
-            Array(S0([v, "optionalAccess", (K) => K[0]]) || 3).fill("")
+            Array(S0([v, "optionalAccess", (Q) => Q[0]]) || 3).fill("")
         ],
-        headers: Array(S0([v, "optionalAccess", (K) => K[0]]) || 3).fill("").map((K, ye) => `${ye + 1}`),
+        headers: Array(S0([v, "optionalAccess", (Q) => Q[0]]) || 3).fill("").map((Q, ye) => `${ye + 1}`),
         metadata: null
     });
-    const We = D.filter((K) => K.type !== "checkbox"),
-        Ie = D.filter((K) => K.type === "checkbox");
-    Ie.forEach((K, ye) => {
-        K.default && n(17, oe[We.length + ye] = [K.column, K.default], oe);
+    const We = D.filter((Q) => Q.type !== "checkbox"),
+        Ie = D.filter((Q) => Q.type === "checkbox");
+    Ie.forEach((Q, ye) => {
+        Q.default && n(17, oe[We.length + ye] = [Q.column, Q.default], oe);
     });
-    const Xe = (K) => n(18, Q = K.detail),
-        Ue = (K) => !(C.includes(K) || E.cant_deselect.includes(K));
+    const Xe = (Q) => n(18, K = Q.detail),
+        Ue = (Q) => !(C.includes(Q) || E.cant_deselect.includes(Q));
 
-    function zt(K) {
-        de = K, n(19, de);
+    function zt(Q) {
+        de = Q, n(19, de);
     }
-    const Nn = (K, ye, Fe) => n(17, oe[K] = [ye.column, Fe.detail], oe),
-        Re = (K, ye, Fe) => n(17, oe[K] = [ye.column, Fe.detail], oe),
-        $t = (K, ye, Fe) => n(17, oe[K] = [ye.column, Fe.detail], oe),
-        Ot = (K) => {
+    const Nn = (Q, ye, Fe) => n(17, oe[Q] = [ye.column, Fe.detail], oe),
+        Re = (Q, ye, Fe) => n(17, oe[Q] = [ye.column, Fe.detail], oe),
+        $t = (Q, ye, Fe) => n(17, oe[Q] = [ye.column, Fe.detail], oe),
+        Ot = (Q) => {
             Ie.forEach((ye, Fe) => {
-                n(17, oe[We.length + Fe] = [ye.column, K.detail.includes(ye.column)], oe);
+                n(17, oe[We.length + Fe] = [ye.column, Q.detail.includes(ye.column)], oe);
             });
         },
-        Ct = (K) => Y.dispatch("select", K.detail);
-    return t.$$set = (K) => {
-        "headers" in K && n(0, r = K.headers), "elem_id" in K && n(28, l = K.elem_id), "elem_classes" in K && n(29, o = K.elem_classes), "visible" in K && n(30, c = K.visible), "value" in K && n(26, u = K.value), "bool_checkboxgroup_label" in K && n(1, h = K.bool_checkboxgroup_label), "value_is_output" in K && n(27, _ = K.value_is_output), "col_count" in K && n(31, v = K.col_count), "label" in K && n(2, k = K.label), "show_label" in K && n(3, T = K.show_label), "wrap" in K && n(4, O = K.wrap), "datatype" in K && n(5, P = K.datatype), "scale" in K && n(32, U = K.scale), "min_width" in K && n(33, M = K.min_width), "root" in K && n(6, N = K.root), "filter_columns" in K && n(34, D = K.filter_columns), "select_columns_config" in K && n(7, E = K.select_columns_config), "hide_columns" in K && n(8, C = K.hide_columns), "search_columns" in K && n(9, R = K.search_columns), "line_breaks" in K && n(10, I = K.line_breaks), "column_widths" in K && n(11, z = K.column_widths), "gradio" in K && n(12, Y = K.gradio), "latex_delimiters" in K && n(13, ne = K.latex_delimiters), "height" in K && n(14, re = K.height), "loading_status" in K && n(15, pe = K.loading_status), "interactive" in K && n(16, Me = K.interactive);
+        Ct = (Q) => Y.dispatch("select", Q.detail);
+    return t.$$set = (Q) => {
+        "headers" in Q && n(0, r = Q.headers), "elem_id" in Q && n(28, l = Q.elem_id), "elem_classes" in Q && n(29, o = Q.elem_classes), "visible" in Q && n(30, c = Q.visible), "value" in Q && n(26, u = Q.value), "bool_checkboxgroup_label" in Q && n(1, h = Q.bool_checkboxgroup_label), "value_is_output" in Q && n(27, _ = Q.value_is_output), "col_count" in Q && n(31, v = Q.col_count), "label" in Q && n(2, k = Q.label), "show_label" in Q && n(3, T = Q.show_label), "wrap" in Q && n(4, O = Q.wrap), "datatype" in Q && n(5, P = Q.datatype), "scale" in Q && n(32, U = Q.scale), "min_width" in Q && n(33, M = Q.min_width), "root" in Q && n(6, N = Q.root), "filter_columns" in Q && n(34, D = Q.filter_columns), "select_columns_config" in Q && n(7, E = Q.select_columns_config), "hide_columns" in Q && n(8, C = Q.hide_columns), "search_columns" in Q && n(9, R = Q.search_columns), "line_breaks" in Q && n(10, I = Q.line_breaks), "column_widths" in Q && n(11, z = Q.column_widths), "gradio" in Q && n(12, Y = Q.gradio), "latex_delimiters" in Q && n(13, ne = Q.latex_delimiters), "height" in Q && n(14, re = Q.height), "loading_status" in Q && n(15, pe = Q.loading_status), "interactive" in Q && n(16, Me = Q.interactive);
     }, t.$$.update = () => {
         t.$$.dirty[0] & /*default_selection, filter_values, search_value*/
-            917504 && Se(de, oe, Q), t.$$.dirty[0] & /*value*/
+            917504 && Se(de, oe, K), t.$$.dirty[0] & /*value*/
             67108864 | t.$$.dirty[1] & /*old_value*/
-            16;
+            16 && JSON.stringify(u) !== p && (n(35, p = JSON.stringify(u)), ve = u.headers.map((Q) => Q), ue = u.data.map((Q) => Q), V());
     }, [
         r,
         h,
         k,
         T,
         O,
         P,
@@ -32197,15 +32197,15 @@
         z,
         Y,
         ne,
         re,
         pe,
         Me,
         oe,
-        Q,
+        K,
         de,
         Ne,
         he,
         le,
         Be,
         We,
         Ie,
```

### Comparing `gradio_leaderboard-0.0.8/backend/gradio_leaderboard/templates/component/style.css` & `gradio_leaderboard-0.0.9/backend/gradio_leaderboard/templates/component/style.css`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.8/backend/gradio_leaderboard/templates/component/wrapper-6f348d45-19fa94bf.js` & `gradio_leaderboard-0.0.9/backend/gradio_leaderboard/templates/component/wrapper-6f348d45-19fa94bf.js`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.8/backend/gradio_leaderboard/templates/example/index.js` & `gradio_leaderboard-0.0.9/backend/gradio_leaderboard/templates/example/index.js`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.8/backend/gradio_leaderboard/templates/example/style.css` & `gradio_leaderboard-0.0.9/backend/gradio_leaderboard/templates/example/style.css`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.8/demo/app.py` & `gradio_leaderboard-0.0.9/demo/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 with gr.Blocks() as demo:
     gr.Markdown("""
     # 🥇 Leaderboard Component
     """)
     with gr.Tabs():
         with gr.Tab("Demo"):
-            Leaderboard(
+            lb = Leaderboard(
                 value=df,
                 select_columns=SelectColumns(
                     default_selection=config.ON_LOAD_COLUMNS,
                     cant_deselect=["T", "Model"],
                     label="Select Columns to Display:",
                 ),
                 search_columns=["model_name_for_query", "Type"],
@@ -33,12 +33,15 @@
                     ColumnFilter("MOE", type="boolean", default=False, label="MoE"),
                     ColumnFilter("Flagged", type="boolean", default=False),
                     ColumnFilter("#Params (B)", type="slider", default=[30, 80]),
                 ],
                 datatype=config.TYPES,
                 column_widths=["2%", "33%"],
             )
+            button = gr.Button(value="Update")
+            button.click(lambda: df.iloc[100:], None, lb)
         with gr.Tab("Docs"):
             gr.Markdown((Path(__file__).parent / "docs.md").read_text())
+        
 
 if __name__ == "__main__":
     demo.launch()
```

### Comparing `gradio_leaderboard-0.0.8/demo/config.py` & `gradio_leaderboard-0.0.9/demo/config.py`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.8/demo/css.css` & `gradio_leaderboard-0.0.9/demo/css.css`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.8/demo/docs.md` & `gradio_leaderboard-0.0.9/demo/docs.md`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.8/demo/leaderboard_data.json` & `gradio_leaderboard-0.0.9/demo/leaderboard_data.json`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.8/demo/space.py` & `gradio_leaderboard-0.0.9/demo/space.py`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.8/frontend/Example.svelte` & `gradio_leaderboard-0.0.9/frontend/Example.svelte`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.8/frontend/Index.svelte` & `gradio_leaderboard-0.0.9/frontend/Index.svelte`

 * *Files 2% similar despite different names*

```diff
@@ -210,16 +210,18 @@
 	handle_change();
 
 	afterUpdate(() => {
 		value_is_output = false;
 	});
 
 	$: {
-		if (old_value && JSON.stringify(value) !== old_value) {
+		if (JSON.stringify(value) !== old_value) {
 			old_value = JSON.stringify(value);
+			original_headers = value.headers.map(s => s);
+			original_data = value.data.map(s => s);
 			handle_change();
 		}
 	}
 
 	if (
 		(Array.isArray(value) && value?.[0]?.length === 0) ||
 		value.data?.[0]?.length === 0
```

### Comparing `gradio_leaderboard-0.0.8/frontend/package-lock.json` & `gradio_leaderboard-0.0.9/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.8/frontend/package.json` & `gradio_leaderboard-0.0.9/frontend/package.json`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.8/frontend/shared/Checkboxgroup.svelte` & `gradio_leaderboard-0.0.9/frontend/shared/Checkboxgroup.svelte`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.8/frontend/shared/EditableCell.svelte` & `gradio_leaderboard-0.0.9/frontend/shared/EditableCell.svelte`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.8/frontend/shared/RangeSlider.svelte` & `gradio_leaderboard-0.0.9/frontend/shared/RangeSlider.svelte`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.8/frontend/shared/SimpleTextbox.svelte` & `gradio_leaderboard-0.0.9/frontend/shared/SimpleTextbox.svelte`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.8/frontend/shared/Table.svelte` & `gradio_leaderboard-0.0.9/frontend/shared/Table.svelte`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.8/frontend/shared/VirtualTable.svelte` & `gradio_leaderboard-0.0.9/frontend/shared/VirtualTable.svelte`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.8/frontend/shared/utils.ts` & `gradio_leaderboard-0.0.9/frontend/shared/utils.ts`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.8/README.md` & `gradio_leaderboard-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.8/pyproject.toml` & `gradio_leaderboard-0.0.9/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "gradio_leaderboard"
-version = "0.0.8"
+version = "0.0.9"
 description = "Super fast , batteries included Leaderboard component ⚡️"
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.8"
 authors = [{ name = "YOUR NAME", email = "YOUREMAIL@domain.com" }]
 keywords = ["gradio-custom-component", "gradio-template-Dataframe", "leaderboard", "dataframe", "data", "table"]
 # Add dependencies here
@@ -32,11 +32,11 @@
   'Topic :: Scientific/Engineering :: Visualization',
 ]
 
 [project.optional-dependencies]
 dev = ["build", "twine"]
 
 [tool.hatch.build]
-artifacts = ["/backend/gradio_leaderboard/templates", "*.pyi", "backend/gradio_leaderboard/templates"]
+artifacts = ["/backend/gradio_leaderboard/templates", "*.pyi", "backend/gradio_leaderboard/templates", "backend/gradio_leaderboard/templates", "backend/gradio_leaderboard/templates"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["/backend/gradio_leaderboard"]
```

### Comparing `gradio_leaderboard-0.0.8/PKG-INFO` & `gradio_leaderboard-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gradio_leaderboard
-Version: 0.0.8
+Version: 0.0.9
 Summary: Super fast , batteries included Leaderboard component ⚡️
 Author-email: YOUR NAME <YOUREMAIL@domain.com>
 License-Expression: MIT
 Keywords: data,dataframe,gradio-custom-component,gradio-template-Dataframe,leaderboard,table
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

