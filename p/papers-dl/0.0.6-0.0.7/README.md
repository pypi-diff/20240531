# Comparing `tmp/papers_dl-0.0.6.tar.gz` & `tmp/papers_dl-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "papers_dl-0.0.6.tar", last modified: Wed May 22 22:55:18 2024, max compression
+gzip compressed data, was "papers_dl-0.0.7.tar", last modified: Fri May 31 19:59:08 2024, max compression
```

## Comparing `papers_dl-0.0.6.tar` & `papers_dl-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-22 22:55:18.022138 papers_dl-0.0.6/
--rw-r--r--   0 ben        (501) staff       (20)     1070 2024-03-23 22:45:07.000000 papers_dl-0.0.6/LICENSE
--rw-r--r--   0 ben        (501) staff       (20)     2615 2024-05-22 22:55:18.021824 papers_dl-0.0.6/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     1296 2024-05-04 19:26:22.000000 papers_dl-0.0.6/README.md
--rw-r--r--   0 ben        (501) staff       (20)     1276 2024-05-07 21:38:53.000000 papers_dl-0.0.6/pyproject.toml
--rw-r--r--   0 ben        (501) staff       (20)       38 2024-05-22 22:55:18.022201 papers_dl-0.0.6/setup.cfg
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-22 22:55:18.018788 papers_dl-0.0.6/src/
--rw-r--r--   0 ben        (501) staff       (20)        1 2024-05-06 22:49:47.000000 papers_dl-0.0.6/src/__init__.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-22 22:55:18.021375 papers_dl-0.0.6/src/papers_dl.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)     2615 2024-05-22 22:55:18.000000 papers_dl-0.0.6/src/papers_dl.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      389 2024-05-22 22:55:18.000000 papers_dl-0.0.6/src/papers_dl.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2024-05-22 22:55:18.000000 papers_dl-0.0.6/src/papers_dl.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)       45 2024-05-22 22:55:18.000000 papers_dl-0.0.6/src/papers_dl.egg-info/entry_points.txt
--rw-r--r--   0 ben        (501) staff       (20)      411 2024-05-22 22:55:18.000000 papers_dl-0.0.6/src/papers_dl.egg-info/requires.txt
--rw-r--r--   0 ben        (501) staff       (20)       40 2024-05-22 22:55:18.000000 papers_dl-0.0.6/src/papers_dl.egg-info/top_level.txt
--rw-r--r--   0 ben        (501) staff       (20)     3735 2024-05-07 21:14:52.000000 papers_dl-0.0.6/src/papers_dl.py
--rw-r--r--   0 ben        (501) staff       (20)     2384 2024-05-04 19:19:49.000000 papers_dl-0.0.6/src/parse.py
--rw-r--r--   0 ben        (501) staff       (20)     7881 2024-05-04 19:19:49.000000 papers_dl-0.0.6/src/scihub.py
--rw-r--r--   0 ben        (501) staff       (20)       20 2024-05-07 21:05:21.000000 papers_dl-0.0.6/src/version.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-22 22:55:18.020750 papers_dl-0.0.6/tests/
--rw-r--r--   0 ben        (501) staff       (20)     1714 2024-05-04 19:19:41.000000 papers_dl-0.0.6/tests/test_cli.py
--rw-r--r--   0 ben        (501) staff       (20)      825 2024-05-04 19:19:41.000000 papers_dl-0.0.6/tests/test_fetch.py
--rw-r--r--   0 ben        (501) staff       (20)     2347 2024-05-04 19:19:41.000000 papers_dl-0.0.6/tests/test_parse.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-31 19:59:08.089096 papers_dl-0.0.7/
+-rw-r--r--   0 ben        (501) staff       (20)     1070 2024-03-23 22:45:07.000000 papers_dl-0.0.7/LICENSE
+-rw-r--r--   0 ben        (501) staff       (20)     1700 2024-05-31 19:59:08.088773 papers_dl-0.0.7/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)      381 2024-05-31 19:58:24.000000 papers_dl-0.0.7/README.md
+-rw-r--r--   0 ben        (501) staff       (20)     1276 2024-05-07 21:38:53.000000 papers_dl-0.0.7/pyproject.toml
+-rw-r--r--   0 ben        (501) staff       (20)       38 2024-05-31 19:59:08.089161 papers_dl-0.0.7/setup.cfg
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-31 19:59:08.085524 papers_dl-0.0.7/src/
+-rw-r--r--   0 ben        (501) staff       (20)        1 2024-05-06 22:49:47.000000 papers_dl-0.0.7/src/__init__.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-31 19:59:08.088338 papers_dl-0.0.7/src/papers_dl.egg-info/
+-rw-r--r--   0 ben        (501) staff       (20)     1700 2024-05-31 19:59:08.000000 papers_dl-0.0.7/src/papers_dl.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)      389 2024-05-31 19:59:08.000000 papers_dl-0.0.7/src/papers_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (501) staff       (20)        1 2024-05-31 19:59:08.000000 papers_dl-0.0.7/src/papers_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (501) staff       (20)       45 2024-05-31 19:59:08.000000 papers_dl-0.0.7/src/papers_dl.egg-info/entry_points.txt
+-rw-r--r--   0 ben        (501) staff       (20)      411 2024-05-31 19:59:08.000000 papers_dl-0.0.7/src/papers_dl.egg-info/requires.txt
+-rw-r--r--   0 ben        (501) staff       (20)       40 2024-05-31 19:59:08.000000 papers_dl-0.0.7/src/papers_dl.egg-info/top_level.txt
+-rw-r--r--   0 ben        (501) staff       (20)     3625 2024-05-31 19:38:07.000000 papers_dl-0.0.7/src/papers_dl.py
+-rw-r--r--   0 ben        (501) staff       (20)     2584 2024-05-31 18:40:47.000000 papers_dl-0.0.7/src/parse.py
+-rw-r--r--   0 ben        (501) staff       (20)     8032 2024-05-26 19:19:04.000000 papers_dl-0.0.7/src/scihub.py
+-rw-r--r--   0 ben        (501) staff       (20)       22 2024-05-31 19:50:50.000000 papers_dl-0.0.7/src/version.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-31 19:59:08.087963 papers_dl-0.0.7/tests/
+-rw-r--r--   0 ben        (501) staff       (20)     1182 2024-05-31 18:22:02.000000 papers_dl-0.0.7/tests/test_cli.py
+-rw-r--r--   0 ben        (501) staff       (20)      775 2024-05-26 19:19:04.000000 papers_dl-0.0.7/tests/test_fetch.py
+-rw-r--r--   0 ben        (501) staff       (20)     2606 2024-05-31 18:26:26.000000 papers_dl-0.0.7/tests/test_parse.py
```

### Comparing `papers_dl-0.0.6/LICENSE` & `papers_dl-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `papers_dl-0.0.6/pyproject.toml` & `papers_dl-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `papers_dl-0.0.6/src/papers_dl.py` & `papers_dl-0.0.7/src/papers_dl.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 import argparse
 import os
-
-import requests
-from w3lib.encoding import html_body_declared_encoding, http_content_type_encoding
+import sys
 
 from scihub import SciHub
-from parse import parse_file, print_output, id_patterns
+from parse import parse_file, format_output, parse_ids_from_text, id_patterns
 import pdf2doi
 import json
 
 supported_fetch_identifier_types = ["doi", "pmid", "url", "isbn"]
 
 
-DEFAULT_USER_AGENT = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/17.3 Safari/605.1.15"
-
-
 def save_scihub(identifier: str, out: str, user_agent: str, name: str | None = None):
     """
     find a paper with the given identifier and download it to the output
     directory. If given, name will be the name of the output file. otherwise
     we attempt to find a title from the PDF contents.
     """
 
@@ -27,15 +22,15 @@
 
     result = sh.download(identifier, out)
     if not result:
         return
 
     print(f"Successfully downloaded file with identifier {identifier}")
 
-    # try to use actual title of paper
+    # try to find and use the actual title of the paper
     pdf2doi.config.set("verbose", False)
     result_path = os.path.join(out, result["name"])
 
     try:
         result_info = pdf2doi.pdf2doi(result_path)
         validation_info = json.loads(result_info["validation_info"])
     except TypeError:
@@ -48,23 +43,38 @@
     if file_name:
         file_name += ".pdf"
         new_path = os.path.join(out, file_name)
         os.rename(result_path, new_path)
         print(f"File downloaded to {new_path}")
 
 
+def parse(args):
+    # if a path isn't passed or is empty, read from stdin
+    if not (hasattr(args, "path") and args.path):
+        return format_output(parse_ids_from_text(sys.stdin.read(), args.match))
+
+    return format_output(parse_file(args.path, args.match), args.format)
+
+
+def fetch(args):
+    save_scihub(args.query, args.output, args.user_agent)
+
+
 def main():
     name = "papers-dl"
     parser = argparse.ArgumentParser(
         prog=name,
         description="Download scientific papers from the command line",
     )
 
     from version import __version__
-    parser.add_argument("--version", "-v", action="version", version=f"{name} {__version__}")
+
+    parser.add_argument(
+        "--version", "-v", action="version", version=f"{name} {__version__}"
+    )
 
     subparsers = parser.add_subparsers()
 
     # FETCH
     parser_fetch = subparsers.add_parser(
         "fetch", help="try to download a paper with the given identifier"
     )
@@ -85,58 +95,49 @@
         type=str,
     )
 
     parser_fetch.add_argument(
         "-A",
         "--user-agent",
         help="",
-        default=DEFAULT_USER_AGENT,
+        default=None,
         type=str,
     )
 
     # PARSE
-    parser_parse = subparsers.add_parser("parse", help="parse identifiers from a file")
+    parser_parse = subparsers.add_parser(
+        "parse", help="parse identifiers from a file or stdin"
+    )
     parser_parse.add_argument(
         "-m",
         "--match",
         metavar="type",
-        help="the type of identifier to match",
+        help="the type of identifier to search for",
         type=str,
-        # choices=id_patterns.keys(),
+        choices=id_patterns.keys(),
         action="append",
-        # nargs="+",
     )
     parser_parse.add_argument(
-        "path",
+        "-p",
+        "--path",
         help="the path of the file to parse",
         type=str,
     )
     parser_parse.add_argument(
         "-f",
         "--format",
         help="the output format for printing",
         metavar="fmt",
         default="raw",
         choices=["raw", "jsonl", "csv"],
         nargs="?",
     )
 
-    parser_fetch.set_defaults(
-        func=lambda fetch_args: save_scihub(
-            fetch_args.query, fetch_args.output, fetch_args.user_agent
-        )
-    )
-    parser_parse.set_defaults(
-        func=lambda parse_args: print_output(
-            parse_file(parse_args.path, parse_args.match),
-            parse_args.format,
-        )
-    )
+    parser_fetch.set_defaults(func=fetch)
+    parser_parse.set_defaults(func=parse)
 
     args = parser.parse_args()
-
-    if hasattr(args, "func"):
-        print(args.func(args))
+    print(args.func(args))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `papers_dl-0.0.6/src/parse.py` & `papers_dl-0.0.7/src/parse.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,72 +1,78 @@
 import re
-import os
 import json
 
-
+# these are the currently supported identifier types that we can parse, along
+# with their regex patterns
 id_patterns = {
     # These come from https://gist.github.com/oscarmorrison/3744fa216dcfdb3d0bcb
     "isbn": [
         r"(?:ISBN(?:-10)?:?\ )?(?=[0-9X]{10}|(?=(?:[0-9]+[-\ ]){3})[-\ 0-9X]{13})[0-9]{1,5}[-\ ]?[0-9]+[-\ ]?[0-9]+[-\ ]?[0-9X]",
         r"(?:ISBN(?:-13)?:?\ )?(?=[0-9]{13}|(?=(?:[0-9]+[-\ ]){4})[-\ 0-9]{17})97[89][-\ ]?[0-9]{1,5}[-\ ]?[0-9]+[-\ ]?[0-9]+[-\ ]?[0-9]",
     ],
     # doi regexes taken from https://www.crossref.org/blog/dois-and-matching-regular-expressions/
-    # listed in decreasing order of goodness. Not tested yet.
+    # listed in decreasing order of goodness. Not fully tested yet.
     "doi": [
         r"10.\d{4,9}\/[-._;()\/:A-Z0-9]+",
         r"10.1002\/[^\s]+",
         r"10.\d{4}\/\d+-\d+X?(\d+)\d+<[\d\w]+:[\d\w]*>\d+.\d+.\w+;\d",
         r"10.1021\/\w\w\d++",
         r"10.1207/[\w\d]+\&\d+_\d+",
     ],
 }
 
-def parse_ids_from_text(s: str, id_types: list[str]) -> list[tuple[str, str]]:
+
+def parse_ids_from_text(
+    s: str, id_types: list[str] | None = None
+) -> list[dict[str, str]]:
+    """
+    Find all matches for the given id types in s. If id_types isn't given,
+    defaults to the types in id_patterns.
+    """
+
+    # we look for all ID patterns by default
+    if id_types is None:
+        id_types = list(id_patterns)
+
+    seen = set()
     matches = []
     for id_type in id_types:
         for regex in id_patterns[id_type]:
             for match in re.findall(regex, s, re.IGNORECASE):
-                matches.append((id_type, match))
+                if match not in seen:
+                    matches.append({"id": match, "type": id_type})
+                seen.add(match)
     return matches
 
 
-def filter_dois(doi_matches: list[str]):
-    # NOTE: Only keeping pdfs and matches without extensions.
-    # Haven't tested if this is a reasonable filter
-    filtered_dois = []
-    for doi_match in doi_matches:
-        if "." in os.path.basename(doi_match):
-            _, ext = os.path.splitext(doi_match)
-            if ext.lower() == ".pdf":
-                filtered_dois.append(doi_match)
-        else:
-            filtered_dois.append(doi_match)
-    return filtered_dois
-
+def parse_file(path, id_types: list[str] | None = None):
+    """
+    Find all matches for the given id types in a file. If id_types isn't given,
+    defaults to the types in id_patterns.
+    """
 
-def parse_file(path, id_type):
-    print(f"Parsing {path}")
+    matches = []
     try:
         with open(path) as f:
             content = f.read()
-        return parse_ids_from_text(content, id_type)
+        matches = parse_ids_from_text(content, id_types)
     except Exception as e:
         print(f"Error: {e}")
-        return []
 
+    return matches
+
+
+def format_output(output: list[dict[str, str]], format: str = "raw") -> str:
+    """
+    Formats a list of dicts of ids and id types into a string according to the
+    given format type. 'raw' formats ids by line, ignoring type. 'jsonl' and
+    'csv' formats ids and types.
+    """
 
-def print_output(output: list[tuple[str, str]], format: str) -> None:
+    lines: list[str] = []
     if format == "raw":
-        for line in output:
-            print(line[1])
+        lines = [line["id"] for line in output]
     elif format == "jsonl":
-        for line in output:
-            print(json.dumps({"id": line[1], "type": line[0]}))
+        lines = [json.dumps(line) for line in output]
     elif format == "csv":
-        for line in output:
-            for i in range(len(line)):
-                if i < len(line) - 1:
-                    print(line[i], end=",")
-                else:
-                    print(line[i])
-    else:
-        print(output)
+        lines = [f"{line["id"]},{line["type"]}" for line in output]
+    return "\n".join(lines)
```

### Comparing `papers_dl-0.0.6/src/scihub.py` & `papers_dl-0.0.7/src/scihub.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from collections.abc import MutableMapping
 import re
 import hashlib
 import logging
 import os
 
 import requests
 import urllib3
@@ -20,14 +19,16 @@
 
 # URL-DIRECT - openly accessible paper
 # URL-NON-DIRECT - pay-walled paper
 # PMID - PubMed ID
 # DOI - digital object identifier
 IDClass = enum.Enum("identifier", ["URL-DIRECT", "URL-NON-DIRECT", "PMD", "DOI"])
 
+DEFAULT_USER_AGENT = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/17.3 Safari/605.1.15"
+
 
 class IdentifierNotFoundError(Exception):
     pass
 
 
 class SiteAccessError(Exception):
     pass
@@ -39,15 +40,15 @@
 
 class SciHub(object):
     """
     SciHub class can search for papers on Google Scholar
     and fetch/download papers from sci-hub.io
     """
 
-    def __init__(self, user_agent):
+    def __init__(self, user_agent=DEFAULT_USER_AGENT):
         self.sess = requests.Session()
         self.sess.headers = {
             "User-Agent": user_agent,
         }
         self.available_base_url_list = self._get_available_scihub_urls()
 
         self.base_url = self.available_base_url_list[0] + "/"
@@ -143,15 +144,17 @@
                     "pdf": res.content,
                     "url": url,
                     "name": self._generate_name(res),
                 }
 
         except Exception as e:
             logger.info(
-                "Cannot access %s: %s, changing url...", self.available_base_url_list[0], e
+                "Cannot access %s: %s, changing url...",
+                self.available_base_url_list[0],
+                e,
             )
             self._change_base_url()
             raise SiteAccessError("Failed to access site")
 
     def _get_direct_url(self, identifier: str) -> str | None:
         """
         Finds the direct source url for a given identifier.
```

### Comparing `papers_dl-0.0.6/tests/test_fetch.py` & `papers_dl-0.0.7/tests/test_fetch.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from src.scihub import SciHub
-from src.papers_dl import DEFAULT_USER_AGENT
 import unittest
 
+
 class TestSciHub(unittest.TestCase):
     def setUp(self):
-        self.scihub = SciHub(DEFAULT_USER_AGENT)
+        self.scihub = SciHub()
 
     def test_scihub_up(self):
         """
         Test to verify that `scihub.now.sh` is available
         """
         urls = self.scihub.available_base_url_list
         self.assertIsNotNone(urls, "Failed to find Sci-Hub domains")
         print(f"number of candidate urls: {len(urls)}")
 
     # NOTE: This test is flaky. Retrieval doesn't work consistently
-    def test_fetch(self):
-        with open("tests/identifiers/ids.txt") as f:
-            ids = f.read().splitlines()
-            for id in ids:
-                res = self.scihub.fetch(id)
-                self.assertIsNotNone(res, f"Failed to fetch url from id {id}")
+    # def test_fetch(self):
+    #     with open("tests/identifiers/ids.txt") as f:
+    #         ids = f.read().splitlines()
+    #         for id in ids:
+    #             res = self.scihub.fetch(id)
+    #             self.assertIsNotNone(res, f"Failed to fetch url from id {id}")
```

### Comparing `papers_dl-0.0.6/tests/test_parse.py` & `papers_dl-0.0.7/tests/test_parse.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,55 @@
 from src.parse import parse_ids_from_text, id_patterns
 import unittest
 import os
 
 target_ids = ("doi", "pmid", "isbn", "issn", "url")
 
+
 class TestParser(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.test_material_dir = "tests/identifiers"
         cls.valid_id_types = id_patterns.keys()
         for id_type in target_ids:
             if id_type not in cls.valid_id_types:
                 print(f"Skipping testing for {id_type} parsing!")
 
     def test_parse_text(self):
         """
-            Test to parse identifiers from arbitrary text.
+        Test to parse identifiers from a set of files.
         """
+        # NOTE: this test does not fail on false positive matches
+        # for file in test_document_ids:
         for file in test_document_ids:
+            print(f"testing {file}")
             with open(os.path.join(TestParser.test_material_dir, file)) as f:
                 file_content = f.read()
-            for id_type in TestParser.valid_id_types:
-                parsed_ids = parse_ids_from_text(file_content, id_type)
-                expected_ids = test_document_ids[file].get(id_type)
-                if not expected_ids:
-                    continue
-
-                parsed_ids = [id[1] for id in parsed_ids]
-                for expected_id in expected_ids:
-                    self.assertIn(
-                        expected_id,
-                        parsed_ids,
-                        f"ID {expected_id} not found in {file} for ID type {id_type}",
-                    )
+
+            parsed_results = parse_ids_from_text(file_content)
+
+            # just include the matching id, not the type
+            parsed_results = [result["id"] for result in parsed_results]
+
+            expected_ids = []
+            for type in test_document_ids:
+                if type in id_patterns:
+                    for id in test_document_ids[file][type]:
+                        expected_ids.append(id)
+
+            if not expected_ids:
+                continue
+
+            for expected_id in expected_ids:
+                self.assertIn(
+                    expected_id,
+                    parsed_results,
+                    f"ID {expected_id} not found in {file}",
+                )
+
 
 test_document_ids = {
     "ids.txt": {
         "url": ["https://www.cell.com/current-biology/fulltext/S0960-9822(19)31469-1"],
         "doi": ["10.1016/j.cub.2019.11.030"],
     },
     "bsp-tree.html": {
```

