# Comparing `tmp/jupyterlab_unfold-0.3.1.tar.gz` & `tmp/jupyterlab_unfold-0.3.2.tar.gz`

## Comparing `jupyterlab_unfold-0.3.1.tar` & `jupyterlab_unfold-0.3.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/.copier-answers.yml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/.prettierignore
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/.stylelintrc.yaml
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/.yarnrc.yml
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/CHANGELOG.md
--rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/babel.config.js
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/environment.yml
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/jest.config.js
--rw-r--r--   0        0        0     6743 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/setup.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/tsconfig.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/tsconfig.test.json
--rw-r--r--   0        0        0   369864 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/yarn.lock
--rw-r--r--   0        0        0    78194 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/images/screenshot.png
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/jupyterlab_unfold/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/jupyterlab_unfold/_version.py
--rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/jupyterlab_unfold/labextension/package.json
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/jupyterlab_unfold/labextension/schemas/jupyterlab-unfold/jupyterlab-unfold-settings.json
--rw-r--r--   0        0        0     6743 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/jupyterlab_unfold/labextension/schemas/jupyterlab-unfold/package.json.orig
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/jupyterlab_unfold/labextension/schemas/jupyterlab-unfold/plugin.json
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/jupyterlab_unfold/labextension/static/747.85bcc3e88490fafaddb5.js
--rw-r--r--   0        0        0     7919 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/jupyterlab_unfold/labextension/static/874.2dab0411ca57be43f175.js
--rw-r--r--   0        0        0     6981 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/jupyterlab_unfold/labextension/static/remoteEntry.51e9d38969fad5feb467.js
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/jupyterlab_unfold/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/jupyterlab_unfold/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/schema/jupyterlab-unfold-settings.json
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/schema/plugin.json
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/src/index.ts
--rw-r--r--   0        0        0    16729 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/src/unfold.ts
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/src/__tests__/jupyterlab_unfold.spec.ts
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/style/index.js
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/style/icons/folder-open.svg
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/playwright.config.js
--rw-r--r--   0        0        0   151934 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/yarn.lock
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/test_structure/file0.md
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/test_structure/dir1/file11.txt
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/test_structure/dir1/file12.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/test_structure/dir2/file21.txt
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/test_structure/dir2/dir3/file211.txt
--rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/tests/jupyterlab-unfold.spec.ts
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/first-render-linux.png
--rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/fold-dir2-linux.png
--rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/open-file211-linux.png
--rw-r--r--   0        0        0     7278 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/unfold-dir1-linux.png
--rw-r--r--   0        0        0     9741 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/unfold-dir2-2-linux.png
--rw-r--r--   0        0        0     9008 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/unfold-dir2-linux.png
--rw-r--r--   0        0        0     9744 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/unfold-dir3-linux.png
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/.gitignore
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/LICENSE
--rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/README.md
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/.copier-answers.yml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/.prettierignore
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/.stylelintrc.yaml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/.yarnrc.yml
+-rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/CHANGELOG.md
+-rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/babel.config.js
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/environment.yml
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/jest.config.js
+-rw-r--r--   0        0        0     6743 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/setup.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/tsconfig.test.json
+-rw-r--r--   0        0        0   369864 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/yarn.lock
+-rw-r--r--   0        0        0    78194 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/images/screenshot.png
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/jupyterlab_unfold/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/jupyterlab_unfold/_version.py
+-rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/jupyterlab_unfold/labextension/package.json
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/jupyterlab_unfold/labextension/schemas/jupyterlab-unfold/jupyterlab-unfold-settings.json
+-rw-r--r--   0        0        0     6743 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/jupyterlab_unfold/labextension/schemas/jupyterlab-unfold/package.json.orig
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/jupyterlab_unfold/labextension/schemas/jupyterlab-unfold/plugin.json
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/jupyterlab_unfold/labextension/static/747.85bcc3e88490fafaddb5.js
+-rw-r--r--   0        0        0     8052 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/jupyterlab_unfold/labextension/static/874.9589b38c858b813e4ccf.js
+-rw-r--r--   0        0        0     6981 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/jupyterlab_unfold/labextension/static/remoteEntry.dbe81e24c85ee22becd0.js
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/jupyterlab_unfold/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/jupyterlab_unfold/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/schema/jupyterlab-unfold-settings.json
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/schema/plugin.json
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/src/index.ts
+-rw-r--r--   0        0        0    17264 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/src/unfold.ts
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/src/__tests__/jupyterlab_unfold.spec.ts
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/style/index.js
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/style/icons/folder-open.svg
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0   151934 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/ui-tests/yarn.lock
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/ui-tests/test_structure/file0.md
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/ui-tests/test_structure/dir1/file11.txt
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/ui-tests/test_structure/dir1/file12.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/ui-tests/test_structure/dir2/file21.txt
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/ui-tests/test_structure/dir2/dir3/file211.txt
+-rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/ui-tests/tests/jupyterlab-unfold.spec.ts
+-rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/first-render-linux.png
+-rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/fold-dir2-linux.png
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/open-file211-linux.png
+-rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/unfold-dir1-linux.png
+-rw-r--r--   0        0        0     9491 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/unfold-dir2-2-linux.png
+-rw-r--r--   0        0        0     8918 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/unfold-dir2-linux.png
+-rw-r--r--   0        0        0     9571 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/unfold-dir3-linux.png
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/LICENSE
+-rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/README.md
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 jupyterlab_unfold-0.3.2/PKG-INFO
```

### Comparing `jupyterlab_unfold-0.3.1/.stylelintrc.yaml` & `jupyterlab_unfold-0.3.2/.stylelintrc.yaml`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.1/CHANGELOG.md` & `jupyterlab_unfold-0.3.2/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,28 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.3.2
+
+([Full Changelog](https://github.com/jupyterlab-contrib/jupyterlab-unfold/compare/v0.3.1...f8bcc5481cdf0e709604db646c2fcf533f02a9af))
+
+### Bugs fixed
+
+- Fix initialization [#54](https://github.com/jupyterlab-contrib/jupyterlab-unfold/pull/54) ([@martinRenou](https://github.com/martinRenou))
+- Fix issue #52: do not emit if unchanged [#53](https://github.com/jupyterlab-contrib/jupyterlab-unfold/pull/53) ([@michaelchia](https://github.com/michaelchia))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyterlab-contrib/jupyterlab-unfold/graphs/contributors?from=2024-05-28&to=2024-05-31&type=c))
+
+[@github-actions](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-unfold+involves%3Agithub-actions+updated%3A2024-05-28..2024-05-31&type=Issues) | [@martinRenou](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-unfold+involves%3AmartinRenou+updated%3A2024-05-28..2024-05-31&type=Issues) | [@michaelchia](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-unfold+involves%3Amichaelchia+updated%3A2024-05-28..2024-05-31&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.3.1
 
 ([Full Changelog](https://github.com/jupyterlab-contrib/jupyterlab-unfold/compare/v0.3.0...144376fd7baa97e5daf49ccd5c27ed8f348ade4a))
 
 ### Enhancements made
 
 - emit FileBrowserModel.pathChanged signal [#50](https://github.com/jupyterlab-contrib/jupyterlab-unfold/pull/50) ([@michaelchia](https://github.com/michaelchia))
@@ -21,16 +38,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyterlab-contrib/jupyterlab-unfold/graphs/contributors?from=2023-08-24&to=2024-05-28&type=c))
 
 [@fcollonval](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-unfold+involves%3Afcollonval+updated%3A2023-08-24..2024-05-28&type=Issues) | [@github-actions](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-unfold+involves%3Agithub-actions+updated%3A2023-08-24..2024-05-28&type=Issues) | [@martinRenou](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-unfold+involves%3AmartinRenou+updated%3A2023-08-24..2024-05-28&type=Issues) | [@michaelchia](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-unfold+involves%3Amichaelchia+updated%3A2023-08-24..2024-05-28&type=Issues) | [@skbitsp](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-unfold+involves%3Askbitsp+updated%3A2023-08-24..2024-05-28&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.3.0
 
 ([Full Changelog](https://github.com/jupyterlab-contrib/jupyterlab-unfold/compare/0.2.2...4ba3aad147a7cddfae1fc5c890fca99a72907619))
 
 ### Enhancements made
 
 - JupyterLab 4 update [#43](https://github.com/jupyterlab-contrib/jupyterlab-unfold/pull/43) ([@martinRenou](https://github.com/martinRenou))
```

### Comparing `jupyterlab_unfold-0.3.1/RELEASE.md` & `jupyterlab_unfold-0.3.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.1/jest.config.js` & `jupyterlab_unfold-0.3.2/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.1/package.json` & `jupyterlab_unfold-0.3.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.3.2'"}*

```diff
@@ -194,9 +194,9 @@
             "csstree/validator": true,
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.3.1"
+    "version": "0.3.2"
 }
```

### Comparing `jupyterlab_unfold-0.3.1/tsconfig.json` & `jupyterlab_unfold-0.3.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.1/yarn.lock` & `jupyterlab_unfold-0.3.2/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.1/images/screenshot.png` & `jupyterlab_unfold-0.3.2/images/screenshot.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.1/jupyterlab_unfold/labextension/package.json` & `jupyterlab_unfold-0.3.2/jupyterlab_unfold/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9787326388888888%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.dbe81e24c85ee22becd0.js'}}",*

 * * "'version'": "'0.3.2'"}*

```diff
@@ -116,15 +116,15 @@
         "style/**/*.{css,svg}",
         "style/index.js"
     ],
     "homepage": "https://github.com/jupyterlab-contrib/jupyterlab-unfold",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.51e9d38969fad5feb467.js",
+            "load": "static/remoteEntry.dbe81e24c85ee22becd0.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab_unfold/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
@@ -199,9 +199,9 @@
             "csstree/validator": true,
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.3.1"
+    "version": "0.3.2"
 }
```

### Comparing `jupyterlab_unfold-0.3.1/jupyterlab_unfold/labextension/schemas/jupyterlab-unfold/package.json.orig` & `jupyterlab_unfold-0.3.2/jupyterlab_unfold/labextension/schemas/jupyterlab-unfold/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.3.2'"}*

```diff
@@ -194,9 +194,9 @@
             "csstree/validator": true,
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.3.1"
+    "version": "0.3.2"
 }
```

### Comparing `jupyterlab_unfold-0.3.1/jupyterlab_unfold/labextension/static/747.85bcc3e88490fafaddb5.js` & `jupyterlab_unfold-0.3.2/jupyterlab_unfold/labextension/static/747.85bcc3e88490fafaddb5.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.1/jupyterlab_unfold/labextension/static/874.2dab0411ca57be43f175.js` & `jupyterlab_unfold-0.3.2/jupyterlab_unfold/labextension/static/874.9589b38c858b813e4ccf.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -75,14 +75,15 @@
                 get model() {
                     return this._model
                 }
                 async _eventDblClick(t) {
                     const e = this.modelForClick(t);
                     "directory" === (null == e ? void 0 : e.type) ? this._singleClickToUnfold || this.model.toggle(e.path): super.handleEvent(t)
                 }
+                _onPathChanged() {}
                 _eventDragEnter(t) {
                     if (t.mimeData.hasData(g)) {
                         const e = this._hitTestNodes(this._items, t);
                         let s;
                         s = -1 !== e ? this._items[e] : t.target, s.classList.add(u), t.preventDefault(), t.stopPropagation()
                     }
                 }
@@ -158,20 +159,19 @@
                 constructor(t) {
                     super(t), this._isRestored = new d.PromiseDelegate, this._savedState = null, this._stateKey = null, this.openState = {}, this.contentManager = this.manager.services.contents, this._savedState = t.state || null, this._path = this.rootPath
                 }
                 get path() {
                     return this._path
                 }
                 set path(t) {
-                    const e = this.pathChanged,
-                        s = this._path;
-                    this._path = t, e.emit({
+                    let e = !1;
+                    this._path !== t && (e = !0), this._path = t, e && this.pathChanged.emit({
                         name: "path",
-                        oldValue: s,
-                        newValue: t
+                        oldValue: this._path,
+                        newValue: p.PathExt.dirname(this._path)
                     })
                 }
                 async cd(t = this.rootPath) {
                     const e = await this.fetchContent(this.rootPath, t);
                     this.handleContents({
                         name: this.rootPath,
                         path: this.rootPath,
@@ -283,19 +283,19 @@
                                     model: h,
                                     restore: !0,
                                     translator: s,
                                     app: t
                                 });
                             return c.listing.singleClickToUnfold = r.get("singleClickToUnfold").composite, r.changed.connect((() => {
                                 c.listing.singleClickToUnfold = r.get("singleClickToUnfold").composite
-                            })), t.restored.then((() => {
-                                const t = window.location.pathname;
-                                let s = t.indexOf("/tree/"),
-                                    i = t.substring(s + 6);
-                                i = decodeURIComponent(i), e.open(i)
+                            })), t.restored.then((async () => {
+                                const s = window.location.pathname,
+                                    i = s.indexOf("/tree/");
+                                let o = s.substring(i + 6);
+                                o = decodeURIComponent(o), "directory" !== (await t.serviceManager.contents.get(o)).type && e.open(o)
                             })), a.add(c), c
                         },
                         tracker: a
                     }
                 }
             }
         }
```

### Comparing `jupyterlab_unfold-0.3.1/jupyterlab_unfold/labextension/static/remoteEntry.51e9d38969fad5feb467.js` & `jupyterlab_unfold-0.3.2/jupyterlab_unfold/labextension/static/remoteEntry.dbe81e24c85ee22becd0.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -44,18 +44,18 @@
     }, m.d = (e, r) => {
         for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
         747: "85bcc3e88490fafaddb5",
-        874: "2dab0411ca57be43f175"
+        874: "9589b38c858b813e4ccf"
     } [e] + ".js?v=" + {
         747: "85bcc3e88490fafaddb5",
-        874: "2dab0411ca57be43f175"
+        874: "9589b38c858b813e4ccf"
     } [e], m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -106,15 +106,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => m.e(874).then((() => () => m(874))),
                         from: i,
                         eager: !1
                     })
-                })("jupyterlab-unfold", "0.3.1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("jupyterlab-unfold", "0.3.2"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         m.g.importScripts && (e = m.g.location + "");
         var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyterlab_unfold-0.3.1/jupyterlab_unfold/labextension/static/third-party-licenses.json` & `jupyterlab_unfold-0.3.2/jupyterlab_unfold/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.1/src/index.ts` & `jupyterlab_unfold-0.3.2/src/index.ts`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+/* eslint-disable @typescript-eslint/ban-ts-comment */
+
 import {
   JupyterFrontEnd,
   JupyterFrontEndPlugin
 } from '@jupyterlab/application';
 
 import { IFileBrowserFactory } from '@jupyterlab/filebrowser';
 
@@ -65,30 +67,34 @@
       widget.listing.singleClickToUnfold = setting.get('singleClickToUnfold')
         .composite as boolean;
 
       setting.changed.connect(() => {
         widget.listing.singleClickToUnfold = setting.get('singleClickToUnfold')
           .composite as boolean;
       });
-   
+
       // check the url in iframe and open
-      app.restored.then(() => {
+      app.restored.then(async () => {
         const windowPathname = window.location.pathname;
-        let treeIndex = windowPathname.indexOf('/tree/');
+        const treeIndex = windowPathname.indexOf('/tree/');
         let path = windowPathname.substring(treeIndex + '/tree/'.length);
         path = decodeURIComponent(path);
-        docManager.open(path);
+        const content = await app.serviceManager.contents.get(path);
+        if (content.type !== 'directory') {
+          docManager.open(path);
+        }
       });
 
       // Track the newly created file browser.
       void tracker.add(widget);
 
       return widget;
     };
 
+    // @ts-ignore: DirListing._onPathChanged is private upstream, need to change this so we can remove the ignore
     return { createFileBrowser, tracker };
   }
 };
 
 export * from './unfold';
 
 export default fileBrowserFactory;
```

### Comparing `jupyterlab_unfold-0.3.1/src/unfold.ts` & `jupyterlab_unfold-0.3.2/src/unfold.ts`

 * *Files 3% similar despite different names*

```diff
@@ -187,14 +187,15 @@
 
   private model: FilterFileTreeBrowserModel;
 }
 
 /**
  * A widget which hosts a filetree.
  */
+// @ts-ignore: _onPathChanged is private upstream, need to change this
 export class DirTreeListing extends DirListing {
   constructor(options: DirTreeListing.IOptions) {
     super({ ...options, renderer: new FileTreeRenderer(options.model) });
   }
 
   set singleClickToUnfold(value: boolean) {
     this._singleClickToUnfold = value;
@@ -225,14 +226,19 @@
         this.model.toggle(entry.path);
       }
     } else {
       super.handleEvent(event);
     }
   }
 
+  _onPathChanged(): void {
+    // It's a no-op to overwrite the base class behavior
+    // We don't want to deselect everything when the path changes
+  }
+
   private _eventDragEnter(event: IDragEvent): void {
     if (event.mimeData.hasData(CONTENTS_MIME)) {
       // @ts-ignore
       const index = this._hitTestNodes(this._items, event);
 
       let target: HTMLElement;
       if (index !== -1) {
@@ -424,24 +430,34 @@
   }
 
   get path(): string {
     return this._path;
   }
 
   set path(value: string) {
-    const pathChanged = this.pathChanged as Signal<this, IChangedArgs<string>>;
-    const oldValue = this._path;
+    let needsToEmit = false;
+
+    if (this._path !== value) {
+      needsToEmit = true;
+    }
 
     this._path = value;
 
-    pathChanged.emit({
-      name: 'path',
-      oldValue,
-      newValue: value
-    });
+    if (needsToEmit) {
+      const pathChanged = this.pathChanged as Signal<
+        this,
+        IChangedArgs<string>
+      >;
+
+      pathChanged.emit({
+        name: 'path',
+        oldValue: this._path,
+        newValue: PathExt.dirname(this._path)
+      });
+    }
   }
 
   /**
    * Change directory.
    *
    * @param path - The path to the file or directory.
    *
@@ -661,21 +677,23 @@
   set showLastModifiedColumn(value: boolean) {
     if (this.listing.setColumnVisibility) {
       this.listing.setColumnVisibility('last_modified', false);
     }
   }
 
   protected createDirListing(options: DirListing.IOptions): DirListing {
+    // @ts-ignore: _onPathChanged is private upstream, need to change this
     return new DirTreeListing({
       model: this.model,
       translator: this.translator
     });
   }
 
   set useFuzzyFilter(value: boolean) {
     // No-op
   }
 
   model: FilterFileTreeBrowserModel;
 
+  // @ts-ignore: _onPathChanged is private upstream, need to change this
   listing: DirTreeListing;
 }
```

### Comparing `jupyterlab_unfold-0.3.1/ui-tests/README.md` & `jupyterlab_unfold-0.3.2/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.1/ui-tests/yarn.lock` & `jupyterlab_unfold-0.3.2/ui-tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.1/ui-tests/tests/jupyterlab-unfold.spec.ts` & `jupyterlab_unfold-0.3.2/ui-tests/tests/jupyterlab-unfold.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.1/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/open-file211-linux.png` & `jupyterlab_unfold-0.3.2/ui-tests/tests/jupyterlab-unfold.spec.ts-snapshots/open-file211-linux.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.1/.gitignore` & `jupyterlab_unfold-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.1/LICENSE` & `jupyterlab_unfold-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.1/README.md` & `jupyterlab_unfold-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.1/pyproject.toml` & `jupyterlab_unfold-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_unfold-0.3.1/PKG-INFO` & `jupyterlab_unfold-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab-unfold
-Version: 0.3.1
+Version: 0.3.2
 Dynamic: Keywords
 Summary: A vscode-like file browser
 Project-URL: Homepage, https://github.com/jupyterlab-contrib/jupyterlab-unfold
 Project-URL: Bug Tracker, https://github.com/jupyterlab-contrib/jupyterlab-unfold/issues
 Project-URL: Repository, https://github.com/jupyterlab-contrib/jupyterlab-unfold.git
 Author-email: Martin Renou <martin.renou@gmail.com>
 License: BSD 3-Clause License
```

