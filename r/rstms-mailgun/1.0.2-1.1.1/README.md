# Comparing `tmp/rstms_mailgun-1.0.2.tar.gz` & `tmp/rstms_mailgun-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rstms_mailgun-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rstms_mailgun-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rstms_mailgun-1.0.2.tar` & `rstms_mailgun-1.1.1.tar`

### file list

```diff
@@ -1,40 +1,42 @@
--rw-r--r--   0        0        0      380 2024-05-18 17:01:57.987206 rstms_mailgun-1.0.2/.bumpversion.cfg
--rw-r--r--   0        0        0     1344 2024-05-18 17:01:39.323410 rstms_mailgun-1.0.2/.gitignore
--rw-r--r--   0        0        0     1071 2024-04-27 02:57:20.579637 rstms_mailgun-1.0.2/LICENSE
--rw-r--r--   0        0        0      539 2024-04-27 02:57:20.579637 rstms_mailgun-1.0.2/Makefile
--rw-r--r--   0        0        0      660 2024-04-27 02:57:20.595637 rstms_mailgun-1.0.2/README.md
--rw-r--r--   0        0        0        6 2024-05-18 17:01:57.987206 rstms_mailgun-1.0.2/VERSION
--rw-r--r--   0        0        0      614 2024-04-27 02:57:20.663637 rstms_mailgun-1.0.2/docs/Makefile
--rw-r--r--   0        0        0       91 2024-04-27 02:57:20.675636 rstms_mailgun-1.0.2/docs/cli.rst
--rwxr-xr-x   0        0        0     4921 2024-04-27 02:57:20.675636 rstms_mailgun-1.0.2/docs/conf.py
--rw-r--r--   0        0        0       33 2024-04-27 02:57:20.675636 rstms_mailgun-1.0.2/docs/contributing.rst
--rw-r--r--   0        0        0      297 2024-04-27 02:57:20.659637 rstms_mailgun-1.0.2/docs/index.rst
--rw-r--r--   0        0        0     1150 2024-04-27 02:57:20.667636 rstms_mailgun-1.0.2/docs/installation.rst
--rw-r--r--   0        0        0      775 2024-04-27 02:57:20.659637 rstms_mailgun-1.0.2/docs/make.bat
--rw-r--r--   0        0        0       27 2024-04-27 02:57:20.655637 rstms_mailgun-1.0.2/docs/readme.rst
--rw-r--r--   0        0        0      431 2024-04-27 02:57:20.615637 rstms_mailgun-1.0.2/make/browser.mk
--rw-r--r--   0        0        0      694 2024-04-27 02:57:20.627637 rstms_mailgun-1.0.2/make/clean.mk
--rw-r--r--   0        0        0     3808 2024-04-27 02:57:20.623637 rstms_mailgun-1.0.2/make/common.mk
--rw-r--r--   0        0        0      477 2024-04-27 02:57:20.619637 rstms_mailgun-1.0.2/make/depends.mk
--rw-r--r--   0        0        0      441 2024-04-27 02:57:20.611637 rstms_mailgun-1.0.2/make/dist.mk
--rw-r--r--   0        0        0      719 2024-04-27 02:57:20.603637 rstms_mailgun-1.0.2/make/docs.mk
--rw-r--r--   0        0        0      610 2024-04-27 02:57:20.599637 rstms_mailgun-1.0.2/make/lint.mk
--rw-r--r--   0        0        0     1214 2024-04-27 02:57:20.607637 rstms_mailgun-1.0.2/make/publish.mk
--rw-r--r--   0        0        0      517 2024-04-27 02:57:20.611637 rstms_mailgun-1.0.2/make/release.mk
--rw-r--r--   0        0        0      502 2024-04-27 02:57:20.607637 rstms_mailgun-1.0.2/make/requirements.mk
--rw-r--r--   0        0        0      947 2024-04-27 02:57:20.603637 rstms_mailgun-1.0.2/make/test.mk
--rw-r--r--   0        0        0     1610 2024-04-27 02:57:20.615637 rstms_mailgun-1.0.2/make/version.mk
--rw-r--r--   0        0        0     1137 2024-05-18 17:01:57.987206 rstms_mailgun-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      231 2024-04-27 02:57:20.547638 rstms_mailgun-1.0.2/pytest.ini
--rw-r--r--   0        0        0       97 2024-05-18 17:01:57.831207 rstms_mailgun-1.0.2/requirements-dev.txt
--rw-r--r--   0        0        0       47 2024-05-18 17:01:57.883207 rstms_mailgun-1.0.2/requirements-docs.txt
--rw-r--r--   0        0        0       15 2024-05-18 17:01:57.775208 rstms_mailgun-1.0.2/requirements.txt
--rw-r--r--   0        0        0      214 2024-04-27 03:15:02.887230 rstms_mailgun-1.0.2/rstms_mailgun/__init__.py
--rw-r--r--   0        0        0    16057 2024-05-18 16:51:44.889906 rstms_mailgun-1.0.2/rstms_mailgun/cli.py
--rw-r--r--   0        0        0     1067 2024-04-27 02:57:20.651637 rstms_mailgun-1.0.2/rstms_mailgun/exception_handler.py
--rw-r--r--   0        0        0     1092 2024-04-27 03:15:02.915229 rstms_mailgun-1.0.2/rstms_mailgun/shell.py
--rw-r--r--   0        0        0      127 2024-05-18 17:01:57.987206 rstms_mailgun-1.0.2/rstms_mailgun/version.py
--rw-r--r--   0        0        0       43 2024-04-27 02:57:20.631637 rstms_mailgun-1.0.2/tests/__init__.py
--rw-r--r--   0        0        0     2255 2024-04-27 03:15:02.935229 rstms_mailgun-1.0.2/tests/test_cli.py
--rw-r--r--   0        0        0      429 2024-04-27 02:57:20.551638 rstms_mailgun-1.0.2/tox.ini
--rw-r--r--   0        0        0     1864 1970-01-01 00:00:00.000000 rstms_mailgun-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      380 2024-05-30 22:42:00.022787 rstms_mailgun-1.1.1/.bumpversion.cfg
+-rw-r--r--   0        0        0     1344 2024-05-18 17:01:39.323410 rstms_mailgun-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1071 2024-04-27 02:57:20.579637 rstms_mailgun-1.1.1/LICENSE
+-rw-r--r--   0        0        0      539 2024-04-27 02:57:20.579637 rstms_mailgun-1.1.1/Makefile
+-rw-r--r--   0        0        0      660 2024-04-27 02:57:20.595637 rstms_mailgun-1.1.1/README.md
+-rw-r--r--   0        0        0        6 2024-05-30 22:42:00.022787 rstms_mailgun-1.1.1/VERSION
+-rw-r--r--   0        0        0      614 2024-04-27 02:57:20.663637 rstms_mailgun-1.1.1/docs/Makefile
+-rw-r--r--   0        0        0       91 2024-04-27 02:57:20.675636 rstms_mailgun-1.1.1/docs/cli.rst
+-rwxr-xr-x   0        0        0     4921 2024-04-27 02:57:20.675636 rstms_mailgun-1.1.1/docs/conf.py
+-rw-r--r--   0        0        0       33 2024-04-27 02:57:20.675636 rstms_mailgun-1.1.1/docs/contributing.rst
+-rw-r--r--   0        0        0      297 2024-04-27 02:57:20.659637 rstms_mailgun-1.1.1/docs/index.rst
+-rw-r--r--   0        0        0     1150 2024-04-27 02:57:20.667636 rstms_mailgun-1.1.1/docs/installation.rst
+-rw-r--r--   0        0        0      775 2024-04-27 02:57:20.659637 rstms_mailgun-1.1.1/docs/make.bat
+-rw-r--r--   0        0        0       27 2024-04-27 02:57:20.655637 rstms_mailgun-1.1.1/docs/readme.rst
+-rw-r--r--   0        0        0      431 2024-04-27 02:57:20.615637 rstms_mailgun-1.1.1/make/browser.mk
+-rw-r--r--   0        0        0      694 2024-04-27 02:57:20.627637 rstms_mailgun-1.1.1/make/clean.mk
+-rw-r--r--   0        0        0     3808 2024-04-27 02:57:20.623637 rstms_mailgun-1.1.1/make/common.mk
+-rw-r--r--   0        0        0      477 2024-04-27 02:57:20.619637 rstms_mailgun-1.1.1/make/depends.mk
+-rw-r--r--   0        0        0      441 2024-04-27 02:57:20.611637 rstms_mailgun-1.1.1/make/dist.mk
+-rw-r--r--   0        0        0      719 2024-04-27 02:57:20.603637 rstms_mailgun-1.1.1/make/docs.mk
+-rw-r--r--   0        0        0      668 2024-05-30 20:38:32.454502 rstms_mailgun-1.1.1/make/lint.mk
+-rw-r--r--   0        0        0     1258 2024-05-30 22:41:28.735017 rstms_mailgun-1.1.1/make/publish.mk
+-rw-r--r--   0        0        0      517 2024-04-27 02:57:20.611637 rstms_mailgun-1.1.1/make/release.mk
+-rw-r--r--   0        0        0      502 2024-04-27 02:57:20.607637 rstms_mailgun-1.1.1/make/requirements.mk
+-rw-r--r--   0        0        0      947 2024-04-27 02:57:20.603637 rstms_mailgun-1.1.1/make/test.mk
+-rw-r--r--   0        0        0     1610 2024-04-27 02:57:20.615637 rstms_mailgun-1.1.1/make/version.mk
+-rw-r--r--   0        0        0     1137 2024-05-30 22:42:00.022787 rstms_mailgun-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-04-27 02:57:20.547638 rstms_mailgun-1.1.1/pytest.ini
+-rw-r--r--   0        0        0       97 2024-05-30 22:41:59.874788 rstms_mailgun-1.1.1/requirements-dev.txt
+-rw-r--r--   0        0        0       47 2024-05-30 22:41:59.930788 rstms_mailgun-1.1.1/requirements-docs.txt
+-rw-r--r--   0        0        0       15 2024-05-30 22:41:59.818788 rstms_mailgun-1.1.1/requirements.txt
+-rw-r--r--   0        0        0      214 2024-04-27 03:15:02.887230 rstms_mailgun-1.1.1/rstms_mailgun/__init__.py
+-rw-r--r--   0        0        0    12026 2024-05-30 22:27:45.806862 rstms_mailgun-1.1.1/rstms_mailgun/cli.py
+-rw-r--r--   0        0        0     4689 2024-05-30 22:20:33.987075 rstms_mailgun-1.1.1/rstms_mailgun/context.py
+-rw-r--r--   0        0        0     1067 2024-04-27 02:57:20.651637 rstms_mailgun-1.1.1/rstms_mailgun/exception_handler.py
+-rw-r--r--   0        0        0     1092 2024-04-27 03:15:02.915229 rstms_mailgun-1.1.1/rstms_mailgun/shell.py
+-rw-r--r--   0        0        0      127 2024-05-30 22:42:00.018787 rstms_mailgun-1.1.1/rstms_mailgun/version.py
+-rw-r--r--   0        0        0       43 2024-04-27 02:57:20.631637 rstms_mailgun-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     2255 2024-04-27 03:15:02.935229 rstms_mailgun-1.1.1/tests/test_cli.py
+-rw-r--r--   0        0        0      888 2024-05-30 22:35:10.769454 rstms_mailgun-1.1.1/tests/test_ctx.py
+-rw-r--r--   0        0        0      429 2024-04-27 02:57:20.551638 rstms_mailgun-1.1.1/tox.ini
+-rw-r--r--   0        0        0     1864 1970-01-01 00:00:00.000000 rstms_mailgun-1.1.1/PKG-INFO
```

### Comparing `rstms_mailgun-1.0.2/.gitignore` & `rstms_mailgun-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.2/LICENSE` & `rstms_mailgun-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.2/Makefile` & `rstms_mailgun-1.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.2/README.md` & `rstms_mailgun-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.2/docs/Makefile` & `rstms_mailgun-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.2/docs/conf.py` & `rstms_mailgun-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.2/docs/installation.rst` & `rstms_mailgun-1.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.2/docs/make.bat` & `rstms_mailgun-1.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.2/make/clean.mk` & `rstms_mailgun-1.1.1/make/clean.mk`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.2/make/common.mk` & `rstms_mailgun-1.1.1/make/common.mk`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.2/make/docs.mk` & `rstms_mailgun-1.1.1/make/docs.mk`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.2/make/publish.mk` & `rstms_mailgun-1.1.1/make/publish.mk`

 * *Files 15% similar despite different names*

```diff
@@ -4,39 +4,40 @@
 # publish to pypi
 publish: release
 	$(call check_private)
 	$(call require_pypi_config)
 	@set -e;\
 	if [ "$(version)" != "$(pypi_version)" ]; then \
 	  $(call verify_action,publish to PyPi) \
-	  echo publishing $(dist_name) $(version) to PyPI...;\
+	  echo publishing $(project) $(version) to PyPI...;\
 	  flit publish;\
 	else \
-	  echo $(dist_name) $(version) is up-to-date on PyPI;\
+	  echo $(project) $(version) is up-to-date on PyPI;\
 	fi
+	which devpi >/dev/null && devpi refresh $(project)
 
 # check current pypi version 
 pypi-check:
 	$(call require_pypi_config)
-	@echo '$(dist_name) local=$(version) pypi=$(call check_pypi_version)'
+	@echo '$(project) local=$(version) pypi=$(call check_pypi_version)'
 
 # clean up publish generated files
 publish-clean:
 	rm -f .dist
 	rm -rf .tox
 
 publish-sterile:
 	@:
 
 # functions
 define require_pypi_config =
 $(if $(wildcard ~/.pypirc),,$(error publish failed; ~/.pypirc required))
 endef
 
-pypi_version := $(shell pip install $(dist_name)==fnord.plough.plover.xyzzy 2>&1 |\
+pypi_version := $(shell pip install $(project)==fnord.plough.plover.xyzzy 2>&1 |\
   awk -F'[,() ]' '/^ERROR: Could not find a version .* \(from versions:.*\)/{print $$(NF-1)}')
 
 define check_null =
 $(if $(1),$(1),$(error $(2)))
 endef
 
 check_pypi_version = $(call check_null,$(pypi_version),PyPi version query failed)
```

### Comparing `rstms_mailgun-1.0.2/make/release.mk` & `rstms_mailgun-1.1.1/make/release.mk`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.2/make/test.mk` & `rstms_mailgun-1.1.1/make/test.mk`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.2/make/version.mk` & `rstms_mailgun-1.1.1/make/version.mk`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.2/pyproject.toml` & `rstms_mailgun-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 requires_python = ">=3.10"
 
 
 
 [project]
 name = "rstms-mailgun"
-version = "1.0.2"
+version = "1.1.1"
 authors = [{name = "Matt Krueger", email = "mkrueger@rstms.net"}]
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 keywords = ["rstms_mailgun"]
 classifiers = [
   "Intended Audience :: Developers",
```

### Comparing `rstms_mailgun-1.0.2/rstms_mailgun/cli.py` & `rstms_mailgun-1.1.1/rstms_mailgun/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 import shlex
 import subprocess
 import sys
 import time
 
 import click
 import click.core
-import requests
-from requests.auth import HTTPBasicAuth
 
+from .context import Context
 from .exception_handler import ExceptionHandler
 from .shell import _shell_completion
 from .version import __timestamp__, __version__
 
 header = f"{__name__.split('.')[0]} v{__version__} {__timestamp__}"
 
 VERIFY_INTERVAL = 5
@@ -27,108 +26,14 @@
 
 
 def _ehandler(ctx, option, debug):
     ctx.obj = dict(ehandler=ExceptionHandler(debug))
     ctx.obj["debug"] = debug
 
 
-class Context:
-    def __init__(self, api_key, domain):
-        self.api_key = api_key
-        self.base_url = "https://api.mailgun.net"
-        self.auth = HTTPBasicAuth("api", api_key)
-        self.json = True
-        self.domain = domain
-        self.quiet = False
-        self.compact = False
-        self.get_domains()
-
-    def _request(self, func, path, **kwargs):
-        url = f"{self.base_url}/{path}"
-        kwargs["auth"] = self.auth
-        response = func(url, **kwargs)
-        response.raise_for_status()
-        return response.json()
-
-    def get(self, path, **kwargs):
-        return self._request(requests.get, path, **kwargs)
-
-    def put(self, path, **kwargs):
-        return self._request(requests.put, path, **kwargs)
-
-    def delete(self, path, **kwargs):
-        return self._request(requests.delete, path, **kwargs)
-
-    def post(self, path, **kwargs):
-        return self._request(requests.post, path, **kwargs)
-
-    def validate(self, exists=True, dns_domain=True):
-        if exists is True:
-            if self.domain not in self.domain_names:
-                fail(f"Unknown domain: {repr(self.domain)}")
-        elif exists is False:
-            if self.domain in self.domain_names:
-                fail(f"Domain exists: {repr(self.domain)}")
-
-        if dns_domain:
-            if "." not in self.domain:
-                fail(f"Unexpected domain format: {repr(self.domain)}")
-
-    def get_domains(self):
-        result = self.get("v4/domains")
-        self.domains = {item["name"]: item for item in result["items"]}
-        self.domain_names = list(self.domains.keys())
-        return self.domains
-
-    def exit(self, exit_code=0, output=None):
-        if output and not self.quiet:
-            if self.json:
-                if self.compact:
-                    output = json.dumps(output, separators=(",", ":"))
-                else:
-                    output = json.dumps(output, indent=2)
-            else:
-                if isinstance(output, dict):
-                    output = "\n".join([f"{k}: {v}" for k, v in output.items()])
-                elif isinstance(output, list):
-                    output = "\n".join(output)
-            click.echo(output)
-        sys.exit(exit_code)
-
-    def list(self):
-        ret = 0 if (self.domain is None or self.domain in self.domain_names) else -1
-        self.exit(ret, self.domain_names)
-
-    def get_status(self):
-        result = self.get(f"v4/domains/{self.domain}")
-        records = self.get_dns_records(result)
-        return dict(
-            domain=self.domain,
-            state=result["domain"]["state"],
-            spf=records["SPF"]["valid"],
-            dkim=records["DKIM"]["valid"],
-        )
-
-    def get_dns_records(self, result=None):
-        if not result:
-            result = self.get(f"v4/domains/{self.domain}")
-        ret = {}
-        for record in result["sending_dns_records"]:
-            _type = record["record_type"]
-            value = record["value"]
-            name = record["name"]
-            if _type == "TXT" and "spf" in value:
-                ret["SPF"] = record
-            elif _type == "TXT" and "domainkey" in name:
-                ret["DKIM"] = record
-            elif _type == "CNAME":
-                ret["CNAME"] = record
-        return ret
-
-
 @click.group("mailgun", context_settings={"auto_envvar_prefix": "MAILGUN"})
 @click.version_option(message=header)
 @click.option("-k", "--api-key", envvar="MAILGUN_API_KEY", show_envvar=True, help="mailgun API key")
 @click.option("-d", "--debug", is_eager=True, is_flag=True, callback=_ehandler, help="debug mode")
 @click.option("-v", "--verbose", is_flag=True, help="enable verbose output")
 @click.option("-q", "--quiet", is_flag=True, help="suppress stdout")
 @click.option("-c", "--compact", is_flag=True, help="compact JSON output")
@@ -241,15 +146,15 @@
     if web_scheme:
         params["web_scheme"] = web_scheme
     if not ctx.force:
         click.echo("Creating domain {ctx.domain}:")
         click.echo(json.dumps(params, indent=2))
         click.confirm("Confirm?", abort=True)
     result = ctx.post("v4/domains", params=params)
-    ctx.exit(0, result['message'])
+    ctx.exit(0, result["message"])
 
 
 @cli.command
 @click.option("-P", "--smtp-password", help="SMTP authentication password")
 @click.option("-w", "--wildcard", is_flag=True, help="accept email from subdomains when sending")
 @click.option("-W", "--web-scheme", type=click.Choice(["http", "https"]), default=None, help="domain web scheme")
 @click.option("-f", "--mail-from", help="MAILFROM hostname for outbound email")
@@ -304,31 +209,30 @@
     else:
         timeout_time = 0
 
     while status["state"] != "active":
 
         if time.time() > request_time:
             if ctx.verbose:
-                click.echo(f"\nRequesting verification...", nl=False)
+                click.echo("\nRequesting verification...", nl=False)
             response = ctx.put(f"v4/domains/{ctx.domain}/verify")
             requested = True
             if ctx.verbose:
                 click.echo(f"{response['message']}")
-                first = True
             request_time = time.time() + interval
 
         if not wait:
             break
 
         if ctx.verbose:
             if requested:
                 requested = False
                 click.echo(f"Status: {status['state']}; waiting...", nl=False)
             else:
-                click.echo('.', nl=False)
+                click.echo(".", nl=False)
 
         if timeout and time.time() > timeout_time:
             fail("Timeout")
 
         time.sleep(1)
         status = ctx.get_status()
 
@@ -358,44 +262,31 @@
         if parse_json:
             ret = json.loads(proc.stdout)
         else:
             ret = proc.stdout.strip()
     return ret
 
 
-def find_dns_record(record, dns_records, domain_name):
-    if record["name"] in ["@", domain_name]:
-        name = domain_name
-    else:
-        name = ".".join([record["name"], domain_name])
+def find_dns_record(record, dns_records):
     for dns in dns_records:
-        if dns["name"] == name and dns["type"] == record["type"]:
+        if dns["domain"] == record["domain"] and dns["name"] == record["name"] and dns["type"] == record["type"]:
             return dns
     return {}
 
 
 @cli.command
-@click.option(
-    "-e",
-    "--exec",
-    "dns_exec",
-    envvar="MAILGUN_DNS_EXEC",
-    show_envvar=True,
-    default="cloudflare",
-    help="execute dns update command",
-)
 @click.option("-d", "--delete", "dns_delete", is_flag=True, help="delete from DNS")
 @click.option("-u", "--update", "dns_update", is_flag=True, help="update to DNS")
 @click.option("-q/-Q", "--query/--no-query", "dns_query", is_flag=True, default=True, help="query DNS")
 @click.option("-c/-C", "--cname/--no-cname", is_flag=True, default=False, help="include CNAME record")
 @click.option("-s/-S", "--spf/--no-spf", is_flag=True, default=True, help="include SPF record")
 @click.option("-k/-K", "--dkim/--no-dkim", is_flag=True, default=True, help="include DKIM record")
-@click.option("--dry-run", is_flag=True, help="output dns-exec command line to stdout")
+@click.option("-t", "--ttl", type=int, default=60, show_default=True, help="DNS TTL")
 @click.pass_obj
-def dns(ctx, dns_exec, dry_run, dns_update, dns_delete, dns_query, cname, spf, dkim):  # noqa: C901
+def dns(ctx, dns_update, dns_delete, dns_query, ttl, cname, spf, dkim):  # noqa: C901
     """show|update|delete required DNS records"""
 
     ctx.validate(exists=True)
     mailgun_records = ctx.get_dns_records()
 
     records = []
     for record in mailgun_records.values():
@@ -404,87 +295,77 @@
             continue
         if record["record_type"] == "TXT":
             if "_domainkey" in record["name"] and not dkim:
                 continue
             if "v=spf1" in record["value"] and not spf:
                 continue
 
-        name = record["name"]
-        if name.endswith(ctx.domain):
-            name = name[: -1 - len(ctx.domain)]
-        if not name:
-            name = "@"
         out["domain"] = ctx.domain
-        out["name"] = name
+        out["name"] = ctx.record_name(record)
         out["type"] = record["record_type"]
         out["value"] = record["value"]
-        out['dns'] = 'unknown'
+        out["dns"] = "unknown"
         records.append(out)
 
+    dns_records = []
+
     if dns_update or dns_delete or dns_query:
-        dns_records = dns_cmd(dns_exec, "--json", "list", ctx.domain, dry_run=dry_run)
+
+        dns_records = ctx.get_deployed_dns_records(
+            spf=spf,
+            dkim=ctx.record_name(mailgun_records["DKIM"]) if dkim else False,
+            cname=ctx.record_name(mailgun_records["CNAME"]) if cname else False,
+        )
 
         for record in records:
-            dns_record = find_dns_record(record, dns_records, ctx.domain)
+            dns_record = find_dns_record(record, dns_records)
             record["id"] = dns_record.get("id", None)
-            if dns_record.get("content", None) is None:
+            if dns_record.get("value", None) is None:
                 record["dns"] = "absent"
-            elif record["value"] == dns_record.get("content", None):
+            elif record["value"] == dns_record.get("value", None):
                 record["dns"] = "present"
             else:
                 record["dns"] = "mismatch"
 
-    if dns_delete:
-        for record in records:
-            if record["dns"] in ["present", "mismatch"]:
-                dns_cmd(dns_exec, "delete", ctx.domain, "ID", record["id"], dry_run=dry_run, parse_json=False)
-                record["id"] = None
-                record["dns"] = "deleted"
+    if dns_delete or dns_update:
+        for dns in dns_records:
+            deleted_id = ctx.cloudflare.delete_record(dns)
+            for record in records:
+                if record["id"] == deleted_id:
+                    record["id"] = None
+                    record["dns"] = "deleted"
 
     if dns_update:
         for record in records:
-            if record["dns"] == "mismatch":
-                dns_cmd(dns_exec, "delete", ctx.domain, "ID", record["id"], dry_run=dry_run, parse_json=False)
-                record["dns"] == "deleted"
-            if record["dns"] != "present":
-                result = dns_cmd(
-                    dns_exec,
-                    "create",
-                    ctx.domain,
-                    record["type"],
-                    record["name"],
-                    record["value"],
-                    dry_run=dry_run,
-                    parse_json=False,
-                )
-                record["dns"] = "updated"
-                record["id"] = result.strip().split()[0]
+            added_id = ctx.cloudflare.add_record(ctx.domain, record["type"], record["name"], record["value"], ttl)
+            record["dns"] = "updated"
+            record["id"] = added_id
 
     for record in records:
         record.pop("id", None)
 
-
     if ctx.json:
         ret = records
     else:
         ret = []
         for record in records:
             name = record["name"]
             if name == ctx.domain or name == "@":
                 name = ctx.domain
             else:
                 name = ".".join([name, ctx.domain])
-            ret.append(" ".join(
-                [
-                    name,
-                    record["type"],
-                    record["value"],
-                    record.get("dns", ""),
-                ]
-
-            ))
+            ret.append(
+                " ".join(
+                    [
+                        record["type"],
+                        name,
+                        record["value"],
+                        record.get("dns", ""),
+                    ]
+                )
+            )
 
     ctx.exit(0, ret)
 
 
 if __name__ == "__main__":
     sys.exit(cli())  # pragma: no cover
```

### Comparing `rstms_mailgun-1.0.2/rstms_mailgun/exception_handler.py` & `rstms_mailgun-1.1.1/rstms_mailgun/exception_handler.py`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.2/rstms_mailgun/shell.py` & `rstms_mailgun-1.1.1/rstms_mailgun/shell.py`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.2/tests/test_cli.py` & `rstms_mailgun-1.1.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `rstms_mailgun-1.0.2/PKG-INFO` & `rstms_mailgun-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rstms-mailgun
-Version: 1.0.2
+Version: 1.1.1
 Summary: Top-level package for rstms-mailgun.
 Keywords: rstms_mailgun
 Author-email: Matt Krueger <mkrueger@rstms.net>
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

