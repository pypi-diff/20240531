# Comparing `tmp/edwh_auth_rbac-0.4.0.tar.gz` & `tmp/edwh_auth_rbac-0.4.1.tar.gz`

## Comparing `edwh_auth_rbac-0.4.0.tar` & `edwh_auth_rbac-0.4.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/.gitignore
--rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/class_index.html
--rw-r--r--   0        0        0    24699 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/coverage_html_cb_da166b87.js
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/favicon_32_cb_58284776.png
--rw-r--r--   0        0        0    36695 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/function_index.html
--rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/keybd_closed_cb_ce680311.png
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/status.json
--rw-r--r--   0        0        0    14077 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/style_cb_8e611ae1.css
--rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/z_438b44bce6437be6___init___py.html
--rw-r--r--   0        0        0     7068 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/z_438b44bce6437be6_helpers_py.html
--rw-r--r--   0        0        0    15181 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/z_438b44bce6437be6_migrations_py.html
--rw-r--r--   0        0        0   123833 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/z_438b44bce6437be6_model_py.html
--rw-r--r--   0        0        0    61606 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/z_438b44bce6437be6_rbac_py.html
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/z_a44f0ac069e85531___init___py.html
--rw-r--r--   0        0        0    60186 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/htmlcov/z_a44f0ac069e85531_test_rbac_py.html
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/src/edwh_auth_rbac/__init__.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/src/edwh_auth_rbac/helpers.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/src/edwh_auth_rbac/migrations.py
--rw-r--r--   0        0        0    14365 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/src/edwh_auth_rbac/model.py
--rw-r--r--   0        0        0     8432 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/src/edwh_auth_rbac/rbac.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/tests/test_migrate.py
--rw-r--r--   0        0        0     8435 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/tests/test_rbac.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/.gitignore
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/README.md
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.1/CHANGELOG.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.1/htmlcov/.gitignore
+-rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.1/htmlcov/class_index.html
+-rw-r--r--   0        0        0    24699 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.1/htmlcov/coverage_html_cb_da166b87.js
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.1/htmlcov/favicon_32_cb_58284776.png
+-rw-r--r--   0        0        0    36695 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.1/htmlcov/function_index.html
+-rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.1/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.1/htmlcov/keybd_closed_cb_ce680311.png
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.1/htmlcov/status.json
+-rw-r--r--   0        0        0    14077 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.1/htmlcov/style_cb_8e611ae1.css
+-rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.1/htmlcov/z_438b44bce6437be6___init___py.html
+-rw-r--r--   0        0        0     7068 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.1/htmlcov/z_438b44bce6437be6_helpers_py.html
+-rw-r--r--   0        0        0    15181 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.1/htmlcov/z_438b44bce6437be6_migrations_py.html
+-rw-r--r--   0        0        0   123833 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.1/htmlcov/z_438b44bce6437be6_model_py.html
+-rw-r--r--   0        0        0    61608 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.1/htmlcov/z_438b44bce6437be6_rbac_py.html
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.1/htmlcov/z_a44f0ac069e85531___init___py.html
+-rw-r--r--   0        0        0    60186 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.1/htmlcov/z_a44f0ac069e85531_test_rbac_py.html
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.1/src/edwh_auth_rbac/__init__.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.1/src/edwh_auth_rbac/helpers.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.1/src/edwh_auth_rbac/migrations.py
+-rw-r--r--   0        0        0    14365 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.1/src/edwh_auth_rbac/model.py
+-rw-r--r--   0        0        0     8520 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.1/src/edwh_auth_rbac/rbac.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.1/tests/test_migrate.py
+-rw-r--r--   0        0        0     8435 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.1/tests/test_rbac.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.1/.gitignore
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.1/README.md
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.4.1/PKG-INFO
```

### Comparing `edwh_auth_rbac-0.4.0/CHANGELOG.md` & `edwh_auth_rbac-0.4.1/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.4.1 (2024-05-30)
+
+### Fix
+
+* Memberhips -> memberships; get_ functions can return None ([`ebd7a0b`](https://github.com/educationwarehouse/edwh-auth-rbac/commit/ebd7a0b4940af61e54639eab80cddb256662f239))
+
 ## v0.4.0 (2024-05-30)
 
 ### Feature
 
 * Support BYOG (bring your own gid) for all relevant add_ functions (item, group, user; not membership, permission) ([`aeb06d9`](https://github.com/educationwarehouse/edwh-auth-rbac/commit/aeb06d9ad7ba385c57fbc6836da878bd1775ae49))
 
 ## v0.3.0 (2024-05-29)
```

### Comparing `edwh_auth_rbac-0.4.0/htmlcov/class_index.html` & `edwh_auth_rbac-0.4.1/htmlcov/class_index.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.4.0/htmlcov/coverage_html_cb_da166b87.js` & `edwh_auth_rbac-0.4.1/htmlcov/coverage_html_cb_da166b87.js`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.4.0/htmlcov/favicon_32_cb_58284776.png` & `edwh_auth_rbac-0.4.1/htmlcov/favicon_32_cb_58284776.png`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.4.0/htmlcov/function_index.html` & `edwh_auth_rbac-0.4.1/htmlcov/function_index.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.4.0/htmlcov/index.html` & `edwh_auth_rbac-0.4.1/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.4.0/htmlcov/keybd_closed_cb_ce680311.png` & `edwh_auth_rbac-0.4.1/htmlcov/keybd_closed_cb_ce680311.png`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.4.0/htmlcov/status.json` & `edwh_auth_rbac-0.4.1/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.4.0/htmlcov/style_cb_8e611ae1.css` & `edwh_auth_rbac-0.4.1/htmlcov/style_cb_8e611ae1.css`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.4.0/htmlcov/z_438b44bce6437be6___init___py.html` & `edwh_auth_rbac-0.4.1/htmlcov/z_438b44bce6437be6___init___py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.4.0/htmlcov/z_438b44bce6437be6_helpers_py.html` & `edwh_auth_rbac-0.4.1/htmlcov/z_438b44bce6437be6_helpers_py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.4.0/htmlcov/z_438b44bce6437be6_migrations_py.html` & `edwh_auth_rbac-0.4.1/htmlcov/z_438b44bce6437be6_migrations_py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.4.0/htmlcov/z_438b44bce6437be6_model_py.html` & `edwh_auth_rbac-0.4.1/htmlcov/z_438b44bce6437be6_model_py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.4.0/htmlcov/z_438b44bce6437be6_rbac_py.html` & `edwh_auth_rbac-0.4.1/htmlcov/z_438b44bce6437be6_rbac_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -172,23 +172,23 @@
     <p class="pln"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">            <span class="nam">firstname</span><span class="op">=</span><span class="nam">name</span> <span class="key">if</span> <span class="nam">name</span> <span class="key">else</span> <span class="nam">firstname</span> <span class="key">if</span> <span class="nam">firstname</span> <span class="key">else</span> <span class="nam">user</span><span class="op">.</span><span class="nam">firstname</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">            <span class="nam">lastname</span><span class="op">=</span><span class="nam">lastname</span> <span class="key">if</span> <span class="nam">lastname</span> <span class="key">else</span> <span class="nam">user</span><span class="op">.</span><span class="nam">lastname</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">            <span class="nam">fullname</span><span class="op">=</span><span class="nam">fullname</span> <span class="key">if</span> <span class="nam">fullname</span> <span class="key">else</span> <span class="nam">user</span><span class="op">.</span><span class="nam">fullname</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">            <span class="nam">password</span><span class="op">=</span><span class="nam">Password</span><span class="op">.</span><span class="nam">encode</span><span class="op">(</span><span class="nam">password</span><span class="op">)</span> <span class="key">if</span> <span class="nam">password</span> <span class="key">else</span> <span class="nam">user</span><span class="op">.</span><span class="nam">encoded_password</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">.</span><span class="nam">commit</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">    <span class="key">def</span> <span class="nam">get_user</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">return_memberhips</span><span class="op">=</span><span class="key">False</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">    <span class="key">def</span> <span class="nam">get_user</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">return_memberships</span><span class="op">=</span><span class="key">False</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">        <span class="nam">rec</span> <span class="op">=</span> <span class="nam">model</span><span class="op">.</span><span class="nam">get_user</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">,</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">        <span class="nam">result</span> <span class="op">=</span> <span class="nam">dict</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">            <span class="nam">object_id</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">object_id</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">            <span class="nam">email</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">email</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">            <span class="nam">firstname</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">firstname</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">            <span class="nam">fullname</span><span class="op">=</span><span class="nam">rec</span><span class="op">.</span><span class="nam">fullname</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">        <span class="key">if</span> <span class="nam">return_memberhips</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">        <span class="key">if</span> <span class="nam">return_memberships</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">            <span class="nam">result</span><span class="op">[</span><span class="str">"memberships"</span><span class="op">]</span> <span class="op">=</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">                <span class="nam">dict</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">                    <span class="nam">object_id</span><span class="op">=</span><span class="nam">m</span><span class="op">.</span><span class="nam">object_id</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">                    <span class="nam">object_type</span><span class="op">=</span><span class="nam">m</span><span class="op">.</span><span class="nam">object_type</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">                    <span class="nam">email</span><span class="op">=</span><span class="nam">m</span><span class="op">.</span><span class="nam">email</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">                    <span class="nam">firstname</span><span class="op">=</span><span class="nam">m</span><span class="op">.</span><span class="nam">firstname</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">                    <span class="nam">fullname</span><span class="op">=</span><span class="nam">m</span><span class="op">.</span><span class="nam">fullname</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
```

#### html2text {}

```diff
@@ -109,23 +109,23 @@
 _9_0 firstname=name if name else firstname if firstname else user.firstname, 
 _9_1 lastname=lastname if lastname else user.lastname, 
 _9_2 fullname=fullname if fullname else user.fullname, 
 _9_3 password=Password.encode(password) if password else user.encoded_password, 
 _9_4 ) 
 _9_5 self.db.commit() 
 _9_6 
-_9_7 def get_user(self, key, return_memberhips=False): 
+_9_7 def get_user(self, key, return_memberships=False): 
 _9_8 rec = model.get_user(self.db, key) 
 _9_9 result = dict( 
 _1_0_0 object_id=rec.object_id, 
 _1_0_1 email=rec.email, 
 _1_0_2 firstname=rec.firstname, 
 _1_0_3 fullname=rec.fullname, 
 _1_0_4 ) 
-_1_0_5 if return_memberhips: 
+_1_0_5 if return_memberships: 
 _1_0_6 result["memberships"] = [ 
 _1_0_7 dict( 
 _1_0_8 object_id=m.object_id, 
 _1_0_9 object_type=m.object_type, 
 _1_1_0 email=m.email, 
 _1_1_1 firstname=m.firstname, 
 _1_1_2 fullname=m.fullname,
```

### Comparing `edwh_auth_rbac-0.4.0/htmlcov/z_a44f0ac069e85531___init___py.html` & `edwh_auth_rbac-0.4.1/htmlcov/z_a44f0ac069e85531___init___py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.4.0/htmlcov/z_a44f0ac069e85531_test_rbac_py.html` & `edwh_auth_rbac-0.4.1/htmlcov/z_a44f0ac069e85531_test_rbac_py.html`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.4.0/src/edwh_auth_rbac/migrations.py` & `edwh_auth_rbac-0.4.1/src/edwh_auth_rbac/migrations.py`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.4.0/src/edwh_auth_rbac/model.py` & `edwh_auth_rbac-0.4.1/src/edwh_auth_rbac/model.py`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.4.0/src/edwh_auth_rbac/rbac.py` & `edwh_auth_rbac-0.4.1/src/edwh_auth_rbac/rbac.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,37 +168,41 @@
             firstname=name if name else firstname if firstname else user.firstname,
             lastname=lastname if lastname else user.lastname,
             fullname=fullname if fullname else user.fullname,
             password=Password.encode(password) if password else user.encoded_password,
         )
         # self.# db.commit()
 
-    def get_user(self, key: IdentityKey, return_memberhips: bool = False) -> UserDict:
-        rec = model.get_user(self.db, key)
+    def get_user(self, key: IdentityKey, return_memberships: bool = False) -> UserDict | None:
+        if not (rec := model.get_user(self.db, key)):
+            return None
+
         result: UserDict = dict(
             object_id=rec.object_id,
             email=rec.email,
             firstname=rec.firstname,
             fullname=rec.fullname,
         )
-        if return_memberhips:
+        if return_memberships:
             result["memberships"] = [
                 dict(
                     object_id=m.object_id,
                     object_type=m.object_type,
                     email=m.email,
                     firstname=m.firstname,
                     fullname=m.fullname,
                 )
                 for m in model.get_memberships(self.db, rec.object_id, bare=False)
             ]
         return result
 
-    def get_group(self, key, return_members=True) -> GroupDict:
-        group_rec = model.get_group(self.db, key)
+    def get_group(self, key, return_members=True) -> GroupDict | None:
+        if not (group_rec := model.get_group(self.db, key)):
+            return None
+
         members = []
         if return_members:
             members = model.get_members(self.db, group_rec.object_id, bare=False)
             members = [
                 dict(
                     object_id=member.object_id,
                     object_type=member.object_type,
```

### Comparing `edwh_auth_rbac-0.4.0/tests/test_migrate.py` & `edwh_auth_rbac-0.4.1/tests/test_migrate.py`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.4.0/tests/test_rbac.py` & `edwh_auth_rbac-0.4.1/tests/test_rbac.py`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.4.0/pyproject.toml` & `edwh_auth_rbac-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_auth_rbac-0.4.0/PKG-INFO` & `edwh_auth_rbac-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: edwh-auth-rbac
-Version: 0.4.0
+Version: 0.4.1
 Summary: Recursive Memberships and Permissions for the Education Warehouse Authentication System
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-auth-rbac#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-auth-rbac/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-auth-rbac
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>
 License-Expression: MIT
 Keywords: edwh,omgeving,whitelabel
```

