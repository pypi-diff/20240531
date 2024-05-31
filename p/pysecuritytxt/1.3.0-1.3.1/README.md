# Comparing `tmp/pysecuritytxt-1.3.0.tar.gz` & `tmp/pysecuritytxt-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysecuritytxt-1.3.0.tar", max compression
+gzip compressed data, was "pysecuritytxt-1.3.1.tar", max compression
```

## Comparing `pysecuritytxt-1.3.0.tar` & `pysecuritytxt-1.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1516 2022-08-30 12:22:20.250018 pysecuritytxt-1.3.0/LICENSE
--rw-r--r--   0        0        0      628 2022-09-01 12:24:36.102749 pysecuritytxt-1.3.0/README.md
--rw-r--r--   0        0        0     1667 2024-03-02 23:27:53.134621 pysecuritytxt-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      637 2024-02-05 19:08:50.046689 pysecuritytxt-1.3.0/pysecuritytxt/__init__.py
--rw-r--r--   0        0        0     7119 2024-03-02 23:19:22.220560 pysecuritytxt-1.3.0/pysecuritytxt/api.py
--rw-r--r--   0        0        0        0 2022-08-30 12:22:20.250018 pysecuritytxt-1.3.0/pysecuritytxt/py.typed
--rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 pysecuritytxt-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1516 2024-05-31 11:21:31.576980 pysecuritytxt-1.3.1/LICENSE
+-rw-r--r--   0        0        0      628 2024-05-31 11:21:31.576980 pysecuritytxt-1.3.1/README.md
+-rw-r--r--   0        0        0     1668 2024-05-31 11:21:31.576980 pysecuritytxt-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      637 2024-05-31 11:21:31.576980 pysecuritytxt-1.3.1/pysecuritytxt/__init__.py
+-rw-r--r--   0        0        0     8099 2024-05-31 11:21:31.580980 pysecuritytxt-1.3.1/pysecuritytxt/api.py
+-rw-r--r--   0        0        0        0 2024-05-31 11:21:31.580980 pysecuritytxt-1.3.1/pysecuritytxt/py.typed
+-rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 pysecuritytxt-1.3.1/PKG-INFO
```

### Comparing `pysecuritytxt-1.3.0/LICENSE` & `pysecuritytxt-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysecuritytxt-1.3.0/README.md` & `pysecuritytxt-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pysecuritytxt-1.3.0/pyproject.toml` & `pysecuritytxt-1.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysecuritytxt"
-version = "1.3.0"
+version = "1.3.1"
 description = "Python CLI and module for querying security.txt files on domains."
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/pysecuritytxt"
 documentation = "https://pysecuritytxt.readthedocs.io/en/latest/index.html"
 
 readme = "README.md"
@@ -28,29 +28,29 @@
 ]
 
 [tool.poetry.scripts]
 pysecuritytxt = 'pysecuritytxt:main'
 
 [tool.poetry.dependencies]
 python = "^3.8"
-requests = "^2.31.0"
+requests = "^2.32.3"
 Sphinx = [
     {version = "<7.2", python = "<3.9", optional = true},
     {version = "^7.2", python = ">=3.9", optional = true}
 ]
 
 [tool.poetry.group.dev.dependencies]
-mypy = "^1.8.0"
-types-requests = "^2.31.0.20240218"
+mypy = "^1.10.0"
+types-requests = "^2.32.0.20240523"
 ipython = [
     {version = "<8.13.0", python = "<3.9"},
     {version = "^8.18.0", python = ">=3.9"},
     {version = "^8.19.0", python = ">=3.10"}
 ]
-pytest = "^8.0.2"
+pytest = "^8.2.1"
 
 [tool.poetry.extras]
 docs = ["Sphinx"]
 
 [build-system]
 requires = ["poetry_core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pysecuritytxt-1.3.0/pysecuritytxt/__init__.py` & `pysecuritytxt-1.3.1/pysecuritytxt/__init__.py`

 * *Files identical despite different names*

### Comparing `pysecuritytxt-1.3.0/pysecuritytxt/api.py` & `pysecuritytxt-1.3.1/pysecuritytxt/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import annotations
 
 import ipaddress
 import json
 import logging
 import re
+import socket
 
 from importlib.metadata import version
 from urllib.parse import urljoin, urlparse
 
 import requests
 
 
@@ -37,16 +38,18 @@
         self.session.headers['user-agent'] = useragent if useragent else f'PySecurityTXT / {version("pysecuritytxt")}'
         if proxies:
             self.session.proxies.update(proxies)
         self.expected_paths = ['/.well-known/security.txt', '/security.txt']
 
     def _try_get_url(self, url: str) -> str:
         try:
-            response = self.session.get(url)
+            response = self.session.get(url, timeout=4)
             response.raise_for_status()
+        except requests.Timeout as e:
+            raise e
         except (requests.HTTPError, requests.exceptions.ConnectionError):
             raise SecurityTXTNotAvailable(f'Unable to get the file from: {url}')
         return response.text
 
     def _all_possible_domains(self, hostname: str) -> set[str]:
         hostname_parts = hostname.split('.')
         if len(hostname_parts) <= 2:
@@ -137,37 +140,57 @@
         try:
             ipaddress.ip_address(hostname)
             all_domains = {hostname, }
             ip = True
         except ValueError:
             all_domains = self._all_possible_domains(hostname)
             ip = False
-        test_urls: set[str] = set()
+        test_urls: set[tuple[str, str]] = set()
         for domain in all_domains:
             # we have what should be a domain or an ip, let's try a few things
-            for expected_path in self.expected_paths:
-                test_urls.update([
-                    urljoin(f'https://{domain}', expected_path),
-                    urljoin(f'http://{domain}', expected_path)
-                ])
-
-            if not domain.startswith('www') and not ip:
+            try:
+                if not ip:
+                    # Quick domain name resolution and ignore if it fails
+                    socket.gethostbyname(domain)
+            except Exception as e:
+                self.logger.info(f'Unable to resolve {domain}: {e}')
+            else:
                 for expected_path in self.expected_paths:
                     test_urls.update([
-                        urljoin(f'https://www.{domain}', expected_path),
-                        urljoin(f'http://www.{domain}', expected_path)
+                        (domain, urljoin(f'https://{domain}', expected_path)),
+                        (domain, urljoin(f'http://{domain}', expected_path))
                     ])
 
-        for url in sorted(test_urls, key=len, reverse=True):  # Longest URL first, so /.well-known/ path is prioritized
+            if not domain.startswith('www') and not ip:
+                www_domain = f'www.{domain}'
+                try:
+                    socket.gethostbyname(www_domain)
+                except Exception as e:
+                    self.logger.info(f'Unable to resolve {www_domain}: {e}')
+                else:
+                    for expected_path in self.expected_paths:
+                        test_urls.update([
+                            (www_domain, urljoin(f'https://{www_domain}', expected_path)),
+                            (www_domain, urljoin(f'http://{www_domain}', expected_path))
+                        ])
+
+        timeout_domains = set()
+        tested_urls = set()
+        for domain, url in sorted(test_urls, key=len, reverse=True):  # Longest URL first, so /.well-known/ path is prioritized
+            if domain in timeout_domains:
+                continue
+            tested_urls.add(url)
             try:
                 response = self._try_get_url(url)
                 if re.search("^[C,c]ontact", response, re.MULTILINE):
                     # Because we often get responses that are just plain HTML pages and a 2XX status code.
                     break
+            except requests.Timeout:
+                timeout_domains.add(domain)
             except SecurityTXTNotAvailable:
                 self.logger.debug(f'Not available on {url}')
         else:
-            raise SecurityTXTNotAvailable(f'Unable to file on {", ".join(test_urls)}')
+            raise SecurityTXTNotAvailable(f'Unable to file on {", ".join(tested_urls)}')
 
         if not parse:
             return response
         return json.dumps(self.parse(response))
```

### Comparing `pysecuritytxt-1.3.0/PKG-INFO` & `pysecuritytxt-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysecuritytxt
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python CLI and module for querying security.txt files on domains.
 Home-page: https://github.com/Lookyloo/pysecuritytxt
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Provides-Extra: docs
 Requires-Dist: Sphinx (<7.2) ; (python_version < "3.9") and (extra == "docs")
 Requires-Dist: Sphinx (>=7.2,<8.0) ; (python_version >= "3.9") and (extra == "docs")
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: requests (>=2.32.3,<3.0.0)
 Project-URL: Documentation, https://pysecuritytxt.readthedocs.io/en/latest/index.html
 Project-URL: Repository, https://github.com/Lookyloo/pysecuritytxt
 Description-Content-Type: text/markdown
 
 # Python client and module for querying .well-known/security.txt files
 
 Give it a domain, it tries to fetch the security.txt file
```

