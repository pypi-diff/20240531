# Comparing `tmp/lambdex-0.1.9.tar.gz` & `tmp/lambdex-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambdex-0.1.9.tar", last modified: Wed Feb 15 18:19:07 2023, max compression
+gzip compressed data, was "lambdex-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lambdex-0.1.9.tar` & `lambdex-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0     2433 2023-02-15 18:18:53.356206 lambdex-0.1.9/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1800 2023-02-15 18:18:53.356206 lambdex-0.1.9/.github/workflows/release.yml
--rw-r--r--   0        0        0       64 2023-02-15 18:18:53.356206 lambdex-0.1.9/.gitignore
--rw-r--r--   0        0        0     1050 2023-02-15 18:18:53.356206 lambdex-0.1.9/CHANGES.md
--rw-r--r--   0        0        0      440 2023-02-15 18:18:53.356206 lambdex-0.1.9/Dockerfile
--rw-r--r--   0        0        0    11323 2023-02-15 18:18:53.356206 lambdex-0.1.9/LICENSE
--rw-r--r--   0        0        0     4127 2023-02-15 18:18:53.356206 lambdex-0.1.9/README.md
--rw-r--r--   0        0        0     1450 2023-02-15 18:18:53.356206 lambdex-0.1.9/RELEASE.md
--rw-r--r--   0        0        0      198 2023-02-15 18:18:53.356206 lambdex-0.1.9/TODO
--rw-r--r--   0        0        0      201 2023-02-15 18:18:53.356206 lambdex-0.1.9/examples/event_based/example.sh
--rw-r--r--   0        0        0      247 2023-02-15 18:18:53.356206 lambdex-0.1.9/examples/event_based/example_function.py
--rw-r--r--   0        0        0       91 2023-02-15 18:18:53.356206 lambdex-0.1.9/examples/event_based/requirements.txt
--rwxr-xr-x   0        0        0      243 2023-02-15 18:18:53.356206 lambdex-0.1.9/examples/gcp_http/example.sh
--rw-r--r--   0        0        0      425 2023-02-15 18:18:53.356206 lambdex-0.1.9/examples/gcp_http/example_http_function.py
--rw-r--r--   0        0        0      209 2023-02-15 18:18:53.356206 lambdex-0.1.9/examples/gcp_http/requirements.txt
--rw-r--r--   0        0        0      437 2023-02-15 18:18:53.356206 lambdex-0.1.9/lambdex/__init__.py
--rw-r--r--   0        0        0      251 2023-02-15 18:18:53.356206 lambdex-0.1.9/lambdex/__main__.py
--rw-r--r--   0        0        0      131 2023-02-15 18:18:53.356206 lambdex-0.1.9/lambdex/bin/__init__.py
--rw-r--r--   0        0        0     8614 2023-02-15 18:18:53.360206 lambdex-0.1.9/lambdex/bin/lambdex.py
--rw-r--r--   0        0        0      131 2023-02-15 18:18:53.360206 lambdex-0.1.9/lambdex/resources/__init__.py
--rw-r--r--   0        0        0     1920 2023-02-15 18:18:53.360206 lambdex-0.1.9/lambdex/resources/lambdex_handler.py
--rw-r--r--   0        0        0      154 2023-02-15 18:18:53.360206 lambdex-0.1.9/lambdex/version.py
--rw-r--r--   0        0        0     1821 2023-02-15 18:18:53.360206 lambdex-0.1.9/pyproject.toml
--rwxr-xr-x   0        0        0     1058 2023-02-15 18:18:53.360206 lambdex-0.1.9/scripts/build-lambdex-pex.py
--rw-r--r--   0        0        0     3781 2023-02-15 18:18:53.360206 lambdex-0.1.9/tox.ini
--rw-r--r--   0        0        0     5872 1970-01-01 00:00:00.000000 lambdex-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     3659 2024-05-31 00:12:56.357667 lambdex-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1800 2024-05-31 00:12:56.357667 lambdex-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0       64 2024-05-31 00:12:56.357667 lambdex-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1263 2024-05-31 00:12:56.357667 lambdex-0.2.0/CHANGES.md
+-rw-r--r--   0        0        0      440 2024-05-31 00:12:56.357667 lambdex-0.2.0/Dockerfile
+-rw-r--r--   0        0        0    11323 2024-05-31 00:12:56.357667 lambdex-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1733 2024-05-31 00:12:56.357667 lambdex-0.2.0/MIGRATING.md
+-rw-r--r--   0        0        0     4327 2024-05-31 00:12:56.357667 lambdex-0.2.0/README.md
+-rw-r--r--   0        0        0     1440 2024-05-31 00:12:56.357667 lambdex-0.2.0/RELEASE.md
+-rw-r--r--   0        0        0      198 2024-05-31 00:12:56.357667 lambdex-0.2.0/TODO
+-rw-r--r--   0        0        0      199 2024-05-31 00:12:56.357667 lambdex-0.2.0/examples/event_based/example.sh
+-rw-r--r--   0        0        0      247 2024-05-31 00:12:56.357667 lambdex-0.2.0/examples/event_based/example_function.py
+-rw-r--r--   0        0        0       91 2024-05-31 00:12:56.357667 lambdex-0.2.0/examples/event_based/requirements.txt
+-rwxr-xr-x   0        0        0      241 2024-05-31 00:12:56.357667 lambdex-0.2.0/examples/gcp_http/example.sh
+-rw-r--r--   0        0        0      425 2024-05-31 00:12:56.357667 lambdex-0.2.0/examples/gcp_http/example_http_function.py
+-rw-r--r--   0        0        0      209 2024-05-31 00:12:56.357667 lambdex-0.2.0/examples/gcp_http/requirements.txt
+-rw-r--r--   0        0        0      437 2024-05-31 00:12:56.357667 lambdex-0.2.0/lambdex/__init__.py
+-rw-r--r--   0        0        0      251 2024-05-31 00:12:56.357667 lambdex-0.2.0/lambdex/__main__.py
+-rw-r--r--   0        0        0      131 2024-05-31 00:12:56.357667 lambdex-0.2.0/lambdex/bin/__init__.py
+-rw-r--r--   0        0        0     8929 2024-05-31 00:12:56.357667 lambdex-0.2.0/lambdex/bin/lambdex.py
+-rw-r--r--   0        0        0      131 2024-05-31 00:12:56.357667 lambdex-0.2.0/lambdex/resources/__init__.py
+-rw-r--r--   0        0        0     2359 2024-05-31 00:12:56.357667 lambdex-0.2.0/lambdex/resources/lambdex_handler.py
+-rw-r--r--   0        0        0      154 2024-05-31 00:12:56.357667 lambdex-0.2.0/lambdex/version.py
+-rw-r--r--   0        0        0     1864 2024-05-31 00:12:56.357667 lambdex-0.2.0/pyproject.toml
+-rwxr-xr-x   0        0        0     1058 2024-05-31 00:12:56.357667 lambdex-0.2.0/scripts/build-lambdex-pex.py
+-rw-r--r--   0        0        0     4155 2024-05-31 00:12:56.357667 lambdex-0.2.0/tox.ini
+-rw-r--r--   0        0        0     6122 1970-01-01 00:00:00.000000 lambdex-0.2.0/PKG-INFO
```

### Comparing `lambdex-0.1.9/.github/workflows/release.yml` & `lambdex-0.2.0/.github/workflows/release.yml`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     inputs:
       tag:
         description: The tag to manually run a deploy for.
         required: true
 jobs:
   determine-tag:
     name: Determine the release tag to operate against.
-    runs-on: ubuntu-20.04
+    runs-on: ubuntu-22.04
     outputs:
       release-tag: ${{ steps.determine-tag.outputs.release-tag }}
       release-version: ${{ steps.determine-tag.outputs.release-version }}
     steps:
       - name: Determine Tag
         id: determine-tag
         run: |
@@ -29,24 +29,24 @@
             echo "release-version=${RELEASE_TAG#v}" >> $GITHUB_OUTPUT
           else
             echo "::error::Release tag '${RELEASE_TAG}' must match 'v\d+.\d+.\d+'."
             exit 1
           fi
   pypi:
     name: Publish sdist and wheel to PyPI
-    runs-on: ubuntu-20.04
+    runs-on: ubuntu-22.04
     environment: Release
     needs: determine-tag
     steps:
       - name: Checkout ${{ needs.determine-tag.outputs.release-tag }}
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
         with:
           ref: ${{ needs.determine-tag.outputs.release-tag }}
       - name: Setup Python 3.9
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: 3.9
       - name: Publish ${{ needs.determine-tag.outputs.release-tag }}
         uses: pantsbuild/actions/run-tox@e63d2d0e3c339bdffbe5e51e7c39550e3bc527bb
         env:
           FLIT_USERNAME: ${{ secrets.PYPI_USERNAME }}
           FLIT_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
```

### Comparing `lambdex-0.1.9/CHANGES.md` & `lambdex-0.2.0/CHANGES.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Release Notes
 
+## 0.2.0
+
+This release brings official support for Python 3.12 and is also the last release of Lambdex.
+See [the migration guide](MIGRATING.md) for how modern PEXes can be used directly with no need for
+Lambdex.
+
 ## 0.1.9
 
 This release fixes a bug wherein, when using the -o/--output option Lambdex would fail to write the
 output file if the original input file was not writeable.
 
 ## 0.1.8
```

### Comparing `lambdex-0.1.9/LICENSE` & `lambdex-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lambdex-0.1.9/README.md` & `lambdex-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 # lambdex
 
+> [!WARNING]
+> Lambdex is no longer necessary and the 0.2.0 release of Lambdex is the last.
+> Modern PEXes can be used directly as Lambda zips. See the [the migration guide](MIGRATING.md) for
+> details.
+
 lambdex turns pex files into aws lambda functions.
 
-[pex](https://github.com/pantsbuild/pex) is a tool that simplifies packaging python environments and is ideally suited
+[pex](https://github.com/pex-tool/pex) is a tool that simplifies packaging python environments and is ideally suited
 for aws lambda.  lambdex takes pex files and turns them into aws lambda functions, allowing
 you to more easily run complex applications in the cloud.
 
 aws lambda documentation and concepts can be found [here](https://aws.amazon.com/lambda/getting-started/).
 
 ## using the lambdex cli
 
@@ -83,14 +88,14 @@
 popular packages (e.g. numpy, scipy, matplotlib, PIL, ...) that require building C extensions that can prove tricky
 to get packaged correctly.
 
 Amazon provides an amazonlinux docker image which can be useful for building platform-specific extensions to run
 on AWS Lambda.  See [documentation](http://docs.aws.amazon.com/AmazonECR/latest/userguide/amazon_linux_container_image.html)
 for information about that image.
 
-The minimum Dockerfile to produce can environment that can build Amazon Linux-specific pex files can be found [here](https://github.com/pantsbuild/lambdex/blob/main/Dockerfile)
+The minimum Dockerfile to produce can environment that can build Amazon Linux-specific pex files can be found [here](https://github.com/pex-tool/lambdex/blob/main/Dockerfile)
 
 ### controlling runtime execution
 
 To override the entry point that was specified at build time, you can use the `LAMBDEX_ENTRY_POINT` env var:
 
     LAMBDEX_ENTRY_POINT=mymodule.myapp:other_handler ...
```

### Comparing `lambdex-0.1.9/RELEASE.md` & `lambdex-0.2.0/RELEASE.md`

 * *Files 22% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 ## Preparation
 
 ### Version Bump and Changelog
 
 Bump the version in [`lambdex/version.py`](lambdex/version.py) and update
 [`CHANGES.md`](CHANGES.md) with any changes that are likely to be useful to consumers and then open
-a PR with these changes and land it on https://github.com/pantsbuild/lambdex main.
+a PR with these changes and land it on https://github.com/pex-tool/lambdex main.
 
 ## Release
 
 ### Push Release Tag
 
-Sync a local branch with https://github.com/pantsbuild/lambdex main and confirm it has the version
+Sync a local branch with https://github.com/pex-tool/lambdex main and confirm it has the version
 bump and changelog update as the tip commit:
 
 ```
 $ git log --stat -1 HEAD
 commit 1ce9fa95893b05bc0bc3a9a7d9c415deeb14d447 (HEAD -> main, origin/main, origin/HEAD)
 Author: John Sirois <john.sirois@gmail.com>
 Date:   Mon Apr 26 12:36:53 2021 -0800
@@ -24,19 +24,19 @@
     Prepare the 0.1.4 release. (#21)
 
  lambdex/version.py |   2 +-
  CHANGES.md         |  41 +++++++
  2 files changed, 42 insertions(+), 1 deletions(-)
 ```
 
-Tag the release as `v<version>` and push the tag to https://github.com/pantsbuild/lambdex main:
+Tag the release as `v<version>` and push the tag to https://github.com/pex-tool/lambdex main:
 
 ```
 $ git tag --sign -am 'Release 0.1.4' v0.1.4
-$ git push --tags https://github.com/pantsbuild/lambdex HEAD:main
+$ git push --tags https://github.com/pex-tool/lambdex HEAD:main
 ```
 
 The release to PyPI is automated but requires approval from at least one Core or Maintainers team 
 member. These folks will all get an email with a link to the GitHub release workflow to do this. 
 Alternatively, they can open the Release workflow
-[here](https://github.com/pantsbuild/lambdex/actions?query=workflow%3ARelease) and navigate to the 
-release approval widget.
+[here](https://github.com/pex-tool/lambdex/actions?query=workflow%3ARelease) and navigate to the
+release approval widget.
```

### Comparing `lambdex-0.1.9/lambdex/bin/lambdex.py` & `lambdex-0.2.0/lambdex/bin/lambdex.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,21 +14,14 @@
 import sys
 import zipfile
 
 from pex.pex_bootstrapper import bootstrap_pex_env
 
 from lambdex.version import __version__
 
-try:
-    # PEX >= 1.6.0
-    from pex.third_party.pkg_resources import EntryPoint
-except ImportError:
-    # PEX < 1.6.0 has an install requirement of setuptools which we leverage knowledge of.
-    from pkg_resources import EntryPoint
-
 EVENT_FUNCTION_SIGNATURE = "event"
 GCP_HTTP_FUNCTION_SIGNATURE = "gcp-http"
 
 
 def die(msg):
     print(msg, file=sys.stderr)
     sys.exit(1)
@@ -203,14 +196,29 @@
 def chdir(dirname):
     cwd = os.getcwd()
     os.chdir(dirname)
     yield
     os.chdir(cwd)
 
 
+def load_entry_point(entry_point):
+    if sys.version_info[:2] >= (3, 8):
+        from importlib.metadata import EntryPoint
+
+        return EntryPoint(name=None, value=entry_point, group=None).load()
+    else:
+        try:
+            # PEX >= 1.6.0
+            from pex.third_party.pkg_resources import EntryPoint
+        except ImportError:
+            # PEX < 1.6.0 has an install requirement of setuptools which we leverage knowledge of.
+            from pkg_resources import EntryPoint
+        return EntryPoint.parse("run = {ep}".format(ep=entry_point)).resolve()
+
+
 # lambdex test [context configuration options] foo.pex <foo.json
 def test_lambdex(args):
     bootstrap_pex_env(args.pex)
 
     with cached_environment(args.root, args.pex) as target:
         lambdex_entry_point = os.environ.get("LAMBDEX_ENTRY_POINT")
         if not lambdex_entry_point:
@@ -219,15 +227,15 @@
 
             lambdex_info = LambdexInfo.from_string(lambdex_info_blob)
             lambdex_entry_point = lambdex_info.entry_point
 
         sys.path.append(target)
 
         with chdir(target):
-            runner = EntryPoint.parse("run = %s" % lambdex_entry_point).resolve()
+            runner = load_entry_point(lambdex_entry_point)
             if args.type == EVENT_FUNCTION_SIGNATURE:
                 if args.empty:
                     runner({}, None)
                 else:
                     for filename in args.files:
                         runner(load_json_blob(filename), None)
             elif args.type == GCP_HTTP_FUNCTION_SIGNATURE:
```

### Comparing `lambdex-0.1.9/lambdex/resources/lambdex_handler.py` & `lambdex-0.2.0/lambdex/resources/lambdex_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,19 +21,17 @@
 
 sys.path[0] = os.path.abspath(sys.path[0])
 sys.path.insert(0, os.path.abspath(os.path.join(__entry_point__, ".bootstrap")))
 
 try:
     # PEX >= 1.6.0
     from pex.pex_bootstrapper import bootstrap_pex_env
-    from pex.third_party.pkg_resources import EntryPoint as __EntryPoint
 except ImportError:
     # PEX < 1.6.0 has an install requirement of setuptools which we leverage knowledge of.
     from _pex.pex_bootstrapper import bootstrap_pex_env
-    from pkg_resources import EntryPoint as __EntryPoint
 
 bootstrap_pex_env(__entry_point__)
 
 __lambdex_entry_point = os.environ.get("LAMBDEX_ENTRY_POINT")
 
 if not __lambdex_entry_point:
     import json as __json
@@ -47,12 +45,29 @@
     else:
         with open(os.path.join(__entry_point__, "LAMBDEX-INFO"), "rb") as fp:
             __lambdex_info_blob = fp.read()
 
     __lambdex_info = __json.loads(__lambdex_info_blob)
     __lambdex_entry_point = __lambdex_info["entry_point"]
 
-__RUNNER = __EntryPoint.parse("run = %s" % __lambdex_entry_point).resolve()
+
+def load_entry_point(entry_point):
+    if sys.version_info[:2] >= (3, 8):
+        from importlib.metadata import EntryPoint
+
+        return EntryPoint(name=None, value=entry_point, group=None).load()
+    else:
+        try:
+            # PEX >= 1.6.0
+            from pex.third_party.pkg_resources import EntryPoint
+        except ImportError:
+            # PEX < 1.6.0 has an install requirement of setuptools which we leverage knowledge of.
+            from pkg_resources import EntryPoint
+        return EntryPoint.parse("run = {ep}".format(ep=entry_point)).resolve()
+
+
+__RUNNER = load_entry_point(__lambdex_entry_point)
+del load_entry_point
 
 
 def handler(*args, **kwargs):
     return __RUNNER(*args, **kwargs)
```

### Comparing `lambdex-0.1.9/pyproject.toml` & `lambdex-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["flit_core >=2,<3"]
 build-backend = "flit_core.buildapi"
 
 [tool.flit.metadata]
 module = "lambdex"
 author = "The Lambdex developers"
-author-email = "pantsbuild@gmail.com"
-home-page = "https://github.com/pantsbuild/lambdex"
+author-email = "developers@pex-tool.org"
+home-page = "https://github.com/pex-tool/lambdex"
 description-file = "README.md"
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: Apache Software License",
   "Operating System :: Unix",
   "Operating System :: POSIX :: Linux",
@@ -21,21 +21,22 @@
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.6",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Topic :: Software Development :: Build Tools",
   "Topic :: System :: Archiving :: Packaging",
   "Topic :: System :: Software Distribution",
   "Topic :: Utilities",
 ]
 requires = ["pex>=1.1.15"]
-requires-python = ">=2.7,<3.12,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*"
+requires-python = ">=2.7,<3.13,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*"
 
 [tool.flit.metadata.requires-extra]
 test-gcp-http = [
   "flask==1.1.4; python_version < '3.6'",
   "flask==2.0.3; python_version >= '3.6' and python_version < '3.7'",
   "flask==2.2.2; python_version >= '3.7'",
 ]
@@ -43,15 +44,15 @@
 [tool.flit.scripts]
 lambdex = "lambdex.bin.lambdex:main"
 
 [tool.flit.sdist]
 include = ["CHANGES.md"]
 
 [tool.flit.metadata.urls]
-Changelog = "https://github.com/pantsbuild/lambdex/blob/main/CHANGES.md"
+Changelog = "https://github.com/pex-tool/lambdex/blob/main/CHANGES.md"
 
 [tool.black]
 line-length = 100
 target-version = ["py27"]
 exclude = '''
 /(
   | \.git
```

### Comparing `lambdex-0.1.9/scripts/build-lambdex-pex.py` & `lambdex-0.2.0/scripts/build-lambdex-pex.py`

 * *Files identical despite different names*

### Comparing `lambdex-0.1.9/tox.ini` & `lambdex-0.2.0/tox.ini`

 * *Files 9% similar despite different names*

```diff
@@ -19,51 +19,64 @@
   tox
 commands =
   tox -e pex
 
 [_event_integration]
 deps =
   {[_integration]deps}
+allowlist_externals =
+  chmod
+  cp
+  {toxinidir}/dist/lambdex
+  {toxinidir}/dist/lambda_function_copy.pex
+  {toxinidir}/dist/lambda_function.pex
 commands =
   {[_integration]commands}
   pex --version
   pex -r {toxinidir}/examples/event_based/requirements.txt -o {toxinidir}/dist/lambda_function.pex
   cp {toxinidir}/dist/lambda_function.pex {toxinidir}/dist/lambda_function_ro.pex
   chmod 0544 {toxinidir}/dist/lambda_function_ro.pex
   {toxinidir}/dist/lambdex build -o {toxinidir}/dist/lambda_function_copy.pex -s examples/event_based/example_function.py -H handler -M lambdex_handler.py {toxinidir}/dist/lambda_function_ro.pex
-  {toxinidir}/dist/lambda_function_copy.pex -c 'from lambdex_handler import handler; handler(\{"url":"https://github.com/pantsbuild/lambdex"\}, None)'
+  {toxinidir}/dist/lambda_function_copy.pex -c 'from lambdex_handler import handler; handler(\{"url":"https://github.com/pex-tool/lambdex"\}, None)'
   {toxinidir}/dist/lambdex build -s examples/event_based/example_function.py -H handler -M lambdex_handler.py {toxinidir}/dist/lambda_function.pex
-  {toxinidir}/dist/lambda_function.pex -c 'from lambdex_handler import handler; handler(\{"url":"https://github.com/pantsbuild/lambdex"\}, None)'
+  {toxinidir}/dist/lambda_function.pex -c 'from lambdex_handler import handler; handler(\{"url":"https://github.com/pex-tool/lambdex"\}, None)'
   tox -e entry-point-env-var
 
 [_gcp_http_integration]
 deps =
   {[_integration]deps}
   .[test-gcp-http]
+allowlist_externals =
+  {toxinidir}/dist/lambdex
 commands =
   {[_integration]commands}
   pex --version
   pex -r {toxinidir}/examples/gcp_http/requirements.txt -o {toxinidir}/dist/gcp_http_function.pex
   {toxinidir}/dist/lambdex build -s examples/gcp_http/example_http_function.py -H handler -M main.py {toxinidir}/dist/gcp_http_function.pex
   {toxinidir}/dist/lambdex test --type gcp-http --empty {toxinidir}/dist/gcp_http_function.pex
 
 [testenv:py{27,36,37,38,39}-int-pre-pex1.6]
 # NB: 1.4.8 is the first pre-1.6.0 version to support -c and Python 3.9 is the last version to
 # support collections.Iterable which 1.4.8 uses.
 deps =
   {[_event_integration]deps}
   pex==1.4.8
+allowlist_externals =
+  {[_event_integration]allowlist_externals}
 commands =
   {[_event_integration]commands}
 
-[testenv:py{27,36,37,38,39,310,311}-int-post-pex1.6]
+[testenv:py{27,36,37,38,39,310,311,312}-int-post-pex1.6]
 deps =
   {[_event_integration]deps}
   {[_gcp_http_integration]deps}
   pex>=1.6.0
+allowlist_externals =
+  {[_event_integration]allowlist_externals}
+  {[_gcp_http_integration]allowlist_externals}
 commands =
   {[_event_integration]commands}
   {[_gcp_http_integration]commands}
 
 [testenv:entry-point-env-var]
 setenv =
   LAMBDEX_ENTRY_POINT = example_function:other_handler
@@ -73,16 +86,16 @@
   {toxinidir}/dist/lambdex
   {toxinidir}/dist/lambda_function.pex
   chmod
 
 [testenv:pex]
 deps =
   pex==2.1.43; python_version < "3.10"
-  # N.B.: This is the lowest version of Pex to support up through Python 3.11.
-  pex==2.1.89; python_version >= "3.10"
+  # N.B.: This is the lowest version of Pex to support up through Python 3.12.
+  pex==2.1.139; python_version >= "3.10"
 commands =
   python scripts/build-lambdex-pex.py {toxinidir}/dist/lambdex
 
 [testenv:lambdex]
 commands = lambdex {posargs}
 
 [testenv:fmt]
```

### Comparing `lambdex-0.1.9/PKG-INFO` & `lambdex-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: lambdex
-Version: 0.1.9
+Version: 0.2.0
 Summary: Lambdex turns pex files into aws lambda python functions.
-Home-page: https://github.com/pantsbuild/lambdex
+Home-page: https://github.com/pex-tool/lambdex
 Author: The Lambdex developers
-Author-email: pantsbuild@gmail.com
-Requires-Python: >=2.7,<3.12,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
+Author-email: developers@pex-tool.org
+Requires-Python: >=2.7,<3.13,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
@@ -19,30 +19,36 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: System :: Software Distribution
 Classifier: Topic :: Utilities
 Requires-Dist: pex>=1.1.15
 Requires-Dist: flask==1.1.4 ; extra == "test-gcp-http" and ( python_version < '3.6')
 Requires-Dist: flask==2.0.3 ; extra == "test-gcp-http" and ( python_version >= '3.6' and python_version < '3.7')
 Requires-Dist: flask==2.2.2 ; extra == "test-gcp-http" and ( python_version >= '3.7')
-Project-URL: Changelog, https://github.com/pantsbuild/lambdex/blob/main/CHANGES.md
+Project-URL: Changelog, https://github.com/pex-tool/lambdex/blob/main/CHANGES.md
 Provides-Extra: test-gcp-http
 
 # lambdex
 
+> [!WARNING]
+> Lambdex is no longer necessary and the 0.2.0 release of Lambdex is the last.
+> Modern PEXes can be used directly as Lambda zips. See the [the migration guide](MIGRATING.md) for
+> details.
+
 lambdex turns pex files into aws lambda functions.
 
-[pex](https://github.com/pantsbuild/pex) is a tool that simplifies packaging python environments and is ideally suited
+[pex](https://github.com/pex-tool/pex) is a tool that simplifies packaging python environments and is ideally suited
 for aws lambda.  lambdex takes pex files and turns them into aws lambda functions, allowing
 you to more easily run complex applications in the cloud.
 
 aws lambda documentation and concepts can be found [here](https://aws.amazon.com/lambda/getting-started/).
 
 ## using the lambdex cli
 
@@ -119,15 +125,15 @@
 popular packages (e.g. numpy, scipy, matplotlib, PIL, ...) that require building C extensions that can prove tricky
 to get packaged correctly.
 
 Amazon provides an amazonlinux docker image which can be useful for building platform-specific extensions to run
 on AWS Lambda.  See [documentation](http://docs.aws.amazon.com/AmazonECR/latest/userguide/amazon_linux_container_image.html)
 for information about that image.
 
-The minimum Dockerfile to produce can environment that can build Amazon Linux-specific pex files can be found [here](https://github.com/pantsbuild/lambdex/blob/main/Dockerfile)
+The minimum Dockerfile to produce can environment that can build Amazon Linux-specific pex files can be found [here](https://github.com/pex-tool/lambdex/blob/main/Dockerfile)
 
 ### controlling runtime execution
 
 To override the entry point that was specified at build time, you can use the `LAMBDEX_ENTRY_POINT` env var:
 
     LAMBDEX_ENTRY_POINT=mymodule.myapp:other_handler ...
```

