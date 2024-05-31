# Comparing `tmp/skillsnetwork_jupyter_extension-2.3.1.tar.gz` & `tmp/skillsnetwork_jupyter_extension-2.3.1rc0.tar.gz`

## Comparing `skillsnetwork_jupyter_extension-2.3.1.tar` & `skillsnetwork_jupyter_extension-2.3.1rc0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/.copier-answers.yml
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/.prettierignore
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/.tool-versions
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/.whitesource
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/.yarnrc.yml
--rw-r--r--   0        0        0     8360 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/CHANGELOG.md
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/CODEOWNERS
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/RELEASE.md
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/install.json
--rw-r--r--   0        0        0     7172 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/setup.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/tsconfig.json
--rw-r--r--   0        0        0   227036 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/yarn.lock
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/jupyter-config/server-config/skillsnetwork_jupyter_extension.json
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/schema/toolbar.json
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/skillsnetwork_jupyter_extension/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/skillsnetwork_jupyter_extension/_version.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/skillsnetwork_jupyter_extension/handlers.py
--rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/skillsnetwork_jupyter_extension/labextension/package.json
--rw-r--r--   0        0        0     7172 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/package.json.orig
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/toolbar.json
--rw-r--r--   0        0        0    21557 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/skillsnetwork_jupyter_extension/labextension/static/496.b3c32afd949d9a1b151d.js
--rw-r--r--   0        0        0    30112 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/skillsnetwork_jupyter_extension/labextension/static/636.605077303a876f967661.js
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/skillsnetwork_jupyter_extension/labextension/static/648.64f5e2269a630e211878.js
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/skillsnetwork_jupyter_extension/labextension/static/736.7b5f76df818add15df8b.js
--rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/skillsnetwork_jupyter_extension/labextension/static/944.dddd8170d5a83693b53a.js
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/skillsnetwork_jupyter_extension/labextension/static/956.fb9e1ea921bfd97d8c96.js
--rw-r--r--   0        0        0     8833 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/skillsnetwork_jupyter_extension/labextension/static/remoteEntry.fc9cbf978ae25d1a7c1a.js
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/skillsnetwork_jupyter_extension/labextension/static/style.js
--rw-r--r--   0        0        0     8806 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/skillsnetwork_jupyter_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/src/config.ts
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/src/dialog.ts
--rw-r--r--   0        0        0     7355 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/src/handler.ts
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/src/index.ts
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/src/sn-file-library.ts
--rw-r--r--   0        0        0    23806 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/src/tools.ts
--rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/src/menu/index.ts
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/src/theme/index.ts
--rw-r--r--   0        0        0     7424 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/src/toolbar/index.ts
--rw-r--r--   0        0        0   880991 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/static/extension_demo.gif
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/style/index.js
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/LICENSE
--rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/README.md
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/pyproject.toml
--rw-r--r--   0        0        0    19091 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/.copier-answers.yml
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/.prettierignore
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/.tool-versions
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/.whitesource
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/.yarnrc.yml
+-rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/CHANGELOG.md
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/CODEOWNERS
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/RELEASE.md
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/install.json
+-rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/setup.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/tsconfig.json
+-rw-r--r--   0        0        0   227036 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/yarn.lock
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/jupyter-config/server-config/skillsnetwork_jupyter_extension.json
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/schema/toolbar.json
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/skillsnetwork_jupyter_extension/__init__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/skillsnetwork_jupyter_extension/_version.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/skillsnetwork_jupyter_extension/handlers.py
+-rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/skillsnetwork_jupyter_extension/labextension/package.json
+-rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/package.json.orig
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/toolbar.json
+-rw-r--r--   0        0        0    21557 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/skillsnetwork_jupyter_extension/labextension/static/496.b3c32afd949d9a1b151d.js
+-rw-r--r--   0        0        0    30112 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/skillsnetwork_jupyter_extension/labextension/static/636.605077303a876f967661.js
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/skillsnetwork_jupyter_extension/labextension/static/648.64f5e2269a630e211878.js
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/skillsnetwork_jupyter_extension/labextension/static/736.7b5f76df818add15df8b.js
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/skillsnetwork_jupyter_extension/labextension/static/944.dddd8170d5a83693b53a.js
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/skillsnetwork_jupyter_extension/labextension/static/956.fb9e1ea921bfd97d8c96.js
+-rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/skillsnetwork_jupyter_extension/labextension/static/remoteEntry.87ea629458a4819e8895.js
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/skillsnetwork_jupyter_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     8806 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/skillsnetwork_jupyter_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/src/config.ts
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/src/dialog.ts
+-rw-r--r--   0        0        0     7355 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/src/handler.ts
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/src/index.ts
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/src/sn-file-library.ts
+-rw-r--r--   0        0        0    23806 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/src/tools.ts
+-rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/src/menu/index.ts
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/src/theme/index.ts
+-rw-r--r--   0        0        0     7424 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/src/toolbar/index.ts
+-rw-r--r--   0        0        0   880991 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/static/extension_demo.gif
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/style/index.js
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/LICENSE
+-rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/README.md
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/pyproject.toml
+-rw-r--r--   0        0        0    19094 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.1rc0/PKG-INFO
```

### Comparing `skillsnetwork_jupyter_extension-2.3.1/.copier-answers.yml` & `skillsnetwork_jupyter_extension-2.3.1rc0/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.1/CHANGELOG.md` & `skillsnetwork_jupyter_extension-2.3.1rc0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,17 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
-## 2.3.1
-
-([Full Changelog](https://github.com/ibm-skills-network/skillsnetwork-jupyter-extension/compare/v2.3.0...88072262573ce5934a1fcbe25d07e2f511ce18e6))
-
-### Bugs fixed
-
-- chore: visual changes and fixes [#43](https://github.com/ibm-skills-network/skillsnetwork-jupyter-extension/pull/43) ([@ElioDiNino](https://github.com/ElioDiNino))
-
-### Contributors to this release
-
-([GitHub contributors page for this release](https://github.com/ibm-skills-network/skillsnetwork-jupyter-extension/graphs/contributors?from=2024-05-14&to=2024-05-31&type=c))
-
-[@ElioDiNino](https://github.com/search?q=repo%3Aibm-skills-network%2Fskillsnetwork-jupyter-extension+involves%3AElioDiNino+updated%3A2024-05-14..2024-05-31&type=Issues)
-
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 2.3.1rc0
 
 No merged PRs
 
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 2.3.0
 
 ([Full Changelog](https://github.com/ibm-skills-network/skillsnetwork-jupyter-extension/compare/v2.2.0...b7798725deb194abe06a41a17b74cd019ed6c4f8))
 
 ### Enhancements made
 
 - feat: support opening notebooks in folders for authoring [#38](https://github.com/ibm-skills-network/skillsnetwork-jupyter-extension/pull/38) ([@ElioDiNino](https://github.com/ElioDiNino))
```

### Comparing `skillsnetwork_jupyter_extension-2.3.1/CODEOWNERS` & `skillsnetwork_jupyter_extension-2.3.1rc0/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.1/RELEASE.md` & `skillsnetwork_jupyter_extension-2.3.1rc0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.1/package.json` & `skillsnetwork_jupyter_extension-2.3.1rc0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'2.3.1-rc0'"}*

```diff
@@ -202,9 +202,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "2.3.1"
+    "version": "2.3.1-rc0"
 }
```

### Comparing `skillsnetwork_jupyter_extension-2.3.1/tsconfig.json` & `skillsnetwork_jupyter_extension-2.3.1rc0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.1/yarn.lock` & `skillsnetwork_jupyter_extension-2.3.1rc0/yarn.lock`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.1/schema/toolbar.json` & `skillsnetwork_jupyter_extension-2.3.1rc0/schema/toolbar.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.1/skillsnetwork_jupyter_extension/__init__.py` & `skillsnetwork_jupyter_extension-2.3.1rc0/skillsnetwork_jupyter_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.1/skillsnetwork_jupyter_extension/handlers.py` & `skillsnetwork_jupyter_extension-2.3.1rc0/skillsnetwork_jupyter_extension/handlers.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.1/skillsnetwork_jupyter_extension/labextension/package.json` & `skillsnetwork_jupyter_extension-2.3.1rc0/skillsnetwork_jupyter_extension/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9788194444444445%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.87ea629458a4819e8895.js'}}",*

 * * "'version'": "'2.3.1-rc0'"}*

```diff
@@ -111,15 +111,15 @@
         "src/**/*.{ts,tsx}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/ibm-skills-network/skillsnetwork-jupyter-extension",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.fc9cbf978ae25d1a7c1a.js",
+            "load": "static/remoteEntry.87ea629458a4819e8895.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "skillsnetwork_jupyter_extension"
                 },
@@ -207,9 +207,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "2.3.1"
+    "version": "2.3.1-rc0"
 }
```

### Comparing `skillsnetwork_jupyter_extension-2.3.1/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/package.json.orig` & `skillsnetwork_jupyter_extension-2.3.1rc0/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'2.3.1-rc0'"}*

```diff
@@ -202,9 +202,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "2.3.1"
+    "version": "2.3.1-rc0"
 }
```

### Comparing `skillsnetwork_jupyter_extension-2.3.1/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/toolbar.json` & `skillsnetwork_jupyter_extension-2.3.1rc0/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/toolbar.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.1/skillsnetwork_jupyter_extension/labextension/static/496.b3c32afd949d9a1b151d.js` & `skillsnetwork_jupyter_extension-2.3.1rc0/skillsnetwork_jupyter_extension/labextension/static/496.b3c32afd949d9a1b151d.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.1/skillsnetwork_jupyter_extension/labextension/static/636.605077303a876f967661.js` & `skillsnetwork_jupyter_extension-2.3.1rc0/skillsnetwork_jupyter_extension/labextension/static/636.605077303a876f967661.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.1/skillsnetwork_jupyter_extension/labextension/static/648.64f5e2269a630e211878.js` & `skillsnetwork_jupyter_extension-2.3.1rc0/skillsnetwork_jupyter_extension/labextension/static/648.64f5e2269a630e211878.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.1/skillsnetwork_jupyter_extension/labextension/static/736.7b5f76df818add15df8b.js` & `skillsnetwork_jupyter_extension-2.3.1rc0/skillsnetwork_jupyter_extension/labextension/static/736.7b5f76df818add15df8b.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.1/skillsnetwork_jupyter_extension/labextension/static/944.dddd8170d5a83693b53a.js` & `skillsnetwork_jupyter_extension-2.3.1rc0/skillsnetwork_jupyter_extension/labextension/static/944.dddd8170d5a83693b53a.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.1/skillsnetwork_jupyter_extension/labextension/static/remoteEntry.fc9cbf978ae25d1a7c1a.js` & `skillsnetwork_jupyter_extension-2.3.1rc0/skillsnetwork_jupyter_extension/labextension/static/remoteEntry.87ea629458a4819e8895.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -155,15 +155,15 @@
                         (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     l = [];
-                return "default" === t && (u("axios", "1.6.7", (() => E.e(636).then((() => () => E(636))))), u("form-data", "4.0.0", (() => E.e(956).then((() => () => E(336))))), u("jwt-decode", "3.1.2", (() => E.e(648).then((() => () => E(648))))), u("skillsnetwork_jupyter_extension", "2.3.1", (() => Promise.all([E.e(944), E.e(496)]).then((() => () => E(496)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("axios", "1.6.7", (() => E.e(636).then((() => () => E(636))))), u("form-data", "4.0.0", (() => E.e(956).then((() => () => E(336))))), u("jwt-decode", "3.1.2", (() => E.e(648).then((() => () => E(648))))), u("skillsnetwork_jupyter_extension", "2.3.1-rc0", (() => Promise.all([E.e(944), E.e(496)]).then((() => () => E(496)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         E.g.importScripts && (e = E.g.location + "");
         var r = E.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `skillsnetwork_jupyter_extension-2.3.1/skillsnetwork_jupyter_extension/labextension/static/third-party-licenses.json` & `skillsnetwork_jupyter_extension-2.3.1rc0/skillsnetwork_jupyter_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.1/src/config.ts` & `skillsnetwork_jupyter_extension-2.3.1rc0/src/config.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.1/src/dialog.ts` & `skillsnetwork_jupyter_extension-2.3.1rc0/src/dialog.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.1/src/handler.ts` & `skillsnetwork_jupyter_extension-2.3.1rc0/src/handler.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.1/src/sn-file-library.ts` & `skillsnetwork_jupyter_extension-2.3.1rc0/src/sn-file-library.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.1/src/tools.ts` & `skillsnetwork_jupyter_extension-2.3.1rc0/src/tools.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.1/src/menu/index.ts` & `skillsnetwork_jupyter_extension-2.3.1rc0/src/menu/index.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.1/src/theme/index.ts` & `skillsnetwork_jupyter_extension-2.3.1rc0/src/theme/index.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.1/src/toolbar/index.ts` & `skillsnetwork_jupyter_extension-2.3.1rc0/src/toolbar/index.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.1/static/extension_demo.gif` & `skillsnetwork_jupyter_extension-2.3.1rc0/static/extension_demo.gif`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.1/.gitignore` & `skillsnetwork_jupyter_extension-2.3.1rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.1/LICENSE` & `skillsnetwork_jupyter_extension-2.3.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.1/README.md` & `skillsnetwork_jupyter_extension-2.3.1rc0/README.md`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.1/pyproject.toml` & `skillsnetwork_jupyter_extension-2.3.1rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.1/PKG-INFO` & `skillsnetwork_jupyter_extension-2.3.1rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: skillsnetwork_jupyter_extension
-Version: 2.3.1
+Version: 2.3.1rc0
 Dynamic: Keywords
 Summary: JupterLab/JupyerLite extension for Skills Network Labs
 Project-URL: Homepage, https://github.com/ibm-skills-network/skillsnetwork-jupyter-extension
 Project-URL: Bug Tracker, https://github.com/ibm-skills-network/skillsnetwork-jupyter-extension/issues
 Project-URL: Repository, https://github.com/ibm-skills-network/skillsnetwork-jupyter-extension.git
 Author-email: IBM Skills Network <skills.network@ibm.com>
 License:                                  Apache License
```

