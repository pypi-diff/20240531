# Comparing `tmp/mo_parsing-8.639.24140.tar.gz` & `tmp/mo_parsing-8.645.24152.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo_parsing-8.639.24140.tar", last modified: Sun May 19 22:36:51 2024, max compression
+gzip compressed data, was "mo_parsing-8.645.24152.tar", last modified: Fri May 31 02:41:50 2024, max compression
```

## Comparing `mo_parsing-8.639.24140.tar` & `mo_parsing-8.645.24152.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 22:36:51.561325 mo_parsing-8.639.24140/
--rw-rw-rw-   0        0        0     1023 2019-10-01 00:43:04.000000 mo_parsing-8.639.24140/LICENSE
--rw-rw-rw-   0        0        0     7824 2024-05-19 22:36:51.560325 mo_parsing-8.639.24140/PKG-INFO
--rw-rw-rw-   0        0        0     6582 2024-04-03 00:06:27.000000 mo_parsing-8.639.24140/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 22:36:51.548293 mo_parsing-8.639.24140/mo_parsing/
--rw-rw-rw-   0        0        0     2970 2024-04-03 00:08:27.000000 mo_parsing-8.639.24140/mo_parsing/__init__.py
--rw-rw-rw-   0        0        0    26520 2024-04-03 00:08:27.000000 mo_parsing-8.639.24140/mo_parsing/core.py
--rw-rw-rw-   0        0        0     3281 2022-12-28 00:45:47.000000 mo_parsing-8.639.24140/mo_parsing/debug.py
--rw-rw-rw-   0        0        0    29257 2024-05-19 22:36:43.000000 mo_parsing-8.639.24140/mo_parsing/enhancement.py
--rw-rw-rw-   0        0        0     6015 2024-05-19 22:36:43.000000 mo_parsing-8.639.24140/mo_parsing/exceptions.py
--rw-rw-rw-   0        0        0    26465 2023-12-26 14:01:39.000000 mo_parsing-8.639.24140/mo_parsing/expressions.py
--rw-rw-rw-   0        0        0    31918 2022-12-04 23:23:35.000000 mo_parsing-8.639.24140/mo_parsing/helpers.py
--rw-rw-rw-   0        0        0    12851 2024-05-19 22:36:43.000000 mo_parsing-8.639.24140/mo_parsing/infix.py
--rw-rw-rw-   0        0        0     3125 2022-12-04 23:23:36.000000 mo_parsing-8.639.24140/mo_parsing/profile.py
--rw-rw-rw-   0        0        0    10153 2024-05-19 22:36:43.000000 mo_parsing-8.639.24140/mo_parsing/regex.py
--rw-rw-rw-   0        0        0    12064 2024-05-19 22:36:43.000000 mo_parsing-8.639.24140/mo_parsing/results.py
--rw-rw-rw-   0        0        0    24539 2023-12-26 14:01:39.000000 mo_parsing-8.639.24140/mo_parsing/tokens.py
--rw-rw-rw-   0        0        0    16529 2024-05-19 22:36:43.000000 mo_parsing-8.639.24140/mo_parsing/utils.py
--rw-rw-rw-   0        0        0     6212 2023-11-26 15:19:47.000000 mo_parsing-8.639.24140/mo_parsing/whitespaces.py
-drwxrwxrwx   0        0        0        0 2024-05-19 22:36:51.559315 mo_parsing-8.639.24140/mo_parsing.egg-info/
--rw-rw-rw-   0        0        0     7824 2024-05-19 22:36:51.000000 mo_parsing-8.639.24140/mo_parsing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      507 2024-05-19 22:36:51.000000 mo_parsing-8.639.24140/mo_parsing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 22:36:51.000000 mo_parsing-8.639.24140/mo_parsing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      145 2024-05-19 22:36:51.000000 mo_parsing-8.639.24140/mo_parsing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-19 22:36:51.000000 mo_parsing-8.639.24140/mo_parsing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 22:36:51.561325 mo_parsing-8.639.24140/setup.cfg
--rw-rw-rw-   0        0        0     7815 2024-05-19 22:36:46.000000 mo_parsing-8.639.24140/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 02:41:50.741139 mo_parsing-8.645.24152/
+-rw-rw-rw-   0        0        0     1023 2019-10-01 00:43:04.000000 mo_parsing-8.645.24152/LICENSE
+-rw-rw-rw-   0        0        0     7824 2024-05-31 02:41:50.740124 mo_parsing-8.645.24152/PKG-INFO
+-rw-rw-rw-   0        0        0     6582 2024-04-03 00:06:27.000000 mo_parsing-8.645.24152/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 02:41:50.726773 mo_parsing-8.645.24152/mo_parsing/
+-rw-rw-rw-   0        0        0     2970 2024-04-03 00:08:27.000000 mo_parsing-8.645.24152/mo_parsing/__init__.py
+-rw-rw-rw-   0        0        0    26520 2024-04-03 00:08:27.000000 mo_parsing-8.645.24152/mo_parsing/core.py
+-rw-rw-rw-   0        0        0     3281 2022-12-28 00:45:47.000000 mo_parsing-8.645.24152/mo_parsing/debug.py
+-rw-rw-rw-   0        0        0    29257 2024-05-19 22:36:43.000000 mo_parsing-8.645.24152/mo_parsing/enhancement.py
+-rw-rw-rw-   0        0        0     6015 2024-05-19 22:36:43.000000 mo_parsing-8.645.24152/mo_parsing/exceptions.py
+-rw-rw-rw-   0        0        0    26465 2023-12-26 14:01:39.000000 mo_parsing-8.645.24152/mo_parsing/expressions.py
+-rw-rw-rw-   0        0        0    31918 2022-12-04 23:23:35.000000 mo_parsing-8.645.24152/mo_parsing/helpers.py
+-rw-rw-rw-   0        0        0    12851 2024-05-19 22:36:43.000000 mo_parsing-8.645.24152/mo_parsing/infix.py
+-rw-rw-rw-   0        0        0     3125 2022-12-04 23:23:36.000000 mo_parsing-8.645.24152/mo_parsing/profile.py
+-rw-rw-rw-   0        0        0    10153 2024-05-19 22:36:43.000000 mo_parsing-8.645.24152/mo_parsing/regex.py
+-rw-rw-rw-   0        0        0    12064 2024-05-19 22:36:43.000000 mo_parsing-8.645.24152/mo_parsing/results.py
+-rw-rw-rw-   0        0        0    24539 2023-12-26 14:01:39.000000 mo_parsing-8.645.24152/mo_parsing/tokens.py
+-rw-rw-rw-   0        0        0    16529 2024-05-19 22:36:43.000000 mo_parsing-8.645.24152/mo_parsing/utils.py
+-rw-rw-rw-   0        0        0     6212 2023-11-26 15:19:47.000000 mo_parsing-8.645.24152/mo_parsing/whitespaces.py
+drwxrwxrwx   0        0        0        0 2024-05-31 02:41:50.737716 mo_parsing-8.645.24152/mo_parsing.egg-info/
+-rw-rw-rw-   0        0        0     7824 2024-05-31 02:41:50.000000 mo_parsing-8.645.24152/mo_parsing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      507 2024-05-31 02:41:50.000000 mo_parsing-8.645.24152/mo_parsing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 02:41:50.000000 mo_parsing-8.645.24152/mo_parsing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      145 2024-05-31 02:41:50.000000 mo_parsing-8.645.24152/mo_parsing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-31 02:41:50.000000 mo_parsing-8.645.24152/mo_parsing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 02:41:50.741139 mo_parsing-8.645.24152/setup.cfg
+-rw-rw-rw-   0        0        0     7815 2024-05-31 02:41:45.000000 mo_parsing-8.645.24152/setup.py
```

### Comparing `mo_parsing-8.639.24140/LICENSE` & `mo_parsing-8.645.24152/LICENSE`

 * *Files identical despite different names*

### Comparing `mo_parsing-8.639.24140/PKG-INFO` & `mo_parsing-8.645.24152/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-parsing
-Version: 8.639.24140
+Version: 8.645.24152
 Summary: Another PEG Parsing Tool
 Home-page: https://github.com/klahnakoski/mo-parsing
 Author: Various
 Author-email: kyle@lahnakoski.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -13,21 +13,21 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots==10.632.24139
+Requires-Dist: mo-dots==10.645.24152
 Requires-Dist: mo-future==7.584.24095
 Provides-Extra: tests
-Requires-Dist: mo-testing>=7.562.24075; extra == "tests"
-Requires-Dist: mo-threads>=6.562.24075; extra == "tests"
-Requires-Dist: mo-logs>=8.562.24075; extra == "tests"
-Requires-Dist: mo-files>=6.562.24075; extra == "tests"
+Requires-Dist: mo-testing>=8.633.24139; extra == "tests"
+Requires-Dist: mo-threads>=6.634.24139; extra == "tests"
+Requires-Dist: mo-logs>=8.632.24139; extra == "tests"
+Requires-Dist: mo-files>=6.638.24140; extra == "tests"
 
 # More Parsing!
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/mo-parsing.svg)](https://pypi.org/project/mo-parsing/)
  [![Build Status](https://github.com/klahnakoski/mo-parsing/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-parsing/actions/workflows/build.yml)
 [![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-parsing/badge.svg?branch=master)](https://coveralls.io/github/klahnakoski/mo-parsing?branch=master)
```

### Comparing `mo_parsing-8.639.24140/README.md` & `mo_parsing-8.645.24152/README.md`

 * *Files identical despite different names*

### Comparing `mo_parsing-8.639.24140/mo_parsing/__init__.py` & `mo_parsing-8.645.24152/mo_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `mo_parsing-8.639.24140/mo_parsing/core.py` & `mo_parsing-8.645.24152/mo_parsing/core.py`

 * *Files identical despite different names*

### Comparing `mo_parsing-8.639.24140/mo_parsing/debug.py` & `mo_parsing-8.645.24152/mo_parsing/debug.py`

 * *Files identical despite different names*

### Comparing `mo_parsing-8.639.24140/mo_parsing/enhancement.py` & `mo_parsing-8.645.24152/mo_parsing/enhancement.py`

 * *Files identical despite different names*

### Comparing `mo_parsing-8.639.24140/mo_parsing/exceptions.py` & `mo_parsing-8.645.24152/mo_parsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `mo_parsing-8.639.24140/mo_parsing/expressions.py` & `mo_parsing-8.645.24152/mo_parsing/expressions.py`

 * *Files identical despite different names*

### Comparing `mo_parsing-8.639.24140/mo_parsing/helpers.py` & `mo_parsing-8.645.24152/mo_parsing/helpers.py`

 * *Files identical despite different names*

### Comparing `mo_parsing-8.639.24140/mo_parsing/infix.py` & `mo_parsing-8.645.24152/mo_parsing/infix.py`

 * *Files identical despite different names*

### Comparing `mo_parsing-8.639.24140/mo_parsing/profile.py` & `mo_parsing-8.645.24152/mo_parsing/profile.py`

 * *Files identical despite different names*

### Comparing `mo_parsing-8.639.24140/mo_parsing/regex.py` & `mo_parsing-8.645.24152/mo_parsing/regex.py`

 * *Files identical despite different names*

### Comparing `mo_parsing-8.639.24140/mo_parsing/results.py` & `mo_parsing-8.645.24152/mo_parsing/results.py`

 * *Files identical despite different names*

### Comparing `mo_parsing-8.639.24140/mo_parsing/tokens.py` & `mo_parsing-8.645.24152/mo_parsing/tokens.py`

 * *Files identical despite different names*

### Comparing `mo_parsing-8.639.24140/mo_parsing/utils.py` & `mo_parsing-8.645.24152/mo_parsing/utils.py`

 * *Files identical despite different names*

### Comparing `mo_parsing-8.639.24140/mo_parsing/whitespaces.py` & `mo_parsing-8.645.24152/mo_parsing/whitespaces.py`

 * *Files identical despite different names*

### Comparing `mo_parsing-8.639.24140/mo_parsing.egg-info/PKG-INFO` & `mo_parsing-8.645.24152/mo_parsing.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-parsing
-Version: 8.639.24140
+Version: 8.645.24152
 Summary: Another PEG Parsing Tool
 Home-page: https://github.com/klahnakoski/mo-parsing
 Author: Various
 Author-email: kyle@lahnakoski.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -13,21 +13,21 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots==10.632.24139
+Requires-Dist: mo-dots==10.645.24152
 Requires-Dist: mo-future==7.584.24095
 Provides-Extra: tests
-Requires-Dist: mo-testing>=7.562.24075; extra == "tests"
-Requires-Dist: mo-threads>=6.562.24075; extra == "tests"
-Requires-Dist: mo-logs>=8.562.24075; extra == "tests"
-Requires-Dist: mo-files>=6.562.24075; extra == "tests"
+Requires-Dist: mo-testing>=8.633.24139; extra == "tests"
+Requires-Dist: mo-threads>=6.634.24139; extra == "tests"
+Requires-Dist: mo-logs>=8.632.24139; extra == "tests"
+Requires-Dist: mo-files>=6.638.24140; extra == "tests"
 
 # More Parsing!
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/mo-parsing.svg)](https://pypi.org/project/mo-parsing/)
  [![Build Status](https://github.com/klahnakoski/mo-parsing/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-parsing/actions/workflows/build.yml)
 [![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-parsing/badge.svg?branch=master)](https://coveralls.io/github/klahnakoski/mo-parsing?branch=master)
```

### Comparing `mo_parsing-8.639.24140/setup.py` & `mo_parsing-8.645.24152/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from setuptools import setup
 setup(
     author='Various',
     author_email='kyle@lahnakoski.com',
     classifiers=["Development Status :: 4 - Beta","License :: OSI Approved :: MIT License","Programming Language :: Python :: 3.8","Programming Language :: Python :: 3.9","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules","Programming Language :: Python :: 3.10","Programming Language :: Python :: 3.11","Programming Language :: Python :: 3.12"],
     description='Another PEG Parsing Tool',
     description_content_type='text/plain',
-    extras_require={"tests":["mo-testing>=7.562.24075","mo-threads>=6.562.24075","mo-logs>=8.562.24075","mo-files>=6.562.24075"]},
-    install_requires=["mo-dots==10.632.24139","mo-future==7.584.24095"],
+    extras_require={"tests":["mo-testing>=8.633.24139","mo-threads>=6.634.24139","mo-logs>=8.632.24139","mo-files>=6.638.24140"]},
+    install_requires=["mo-dots==10.645.24152","mo-future==7.584.24095"],
     license='MIT',
     long_description='# More Parsing!\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-parsing.svg)](https://pypi.org/project/mo-parsing/)\n [![Build Status](https://github.com/klahnakoski/mo-parsing/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-parsing/actions/workflows/build.yml)\n[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-parsing/badge.svg?branch=master)](https://coveralls.io/github/klahnakoski/mo-parsing?branch=master)\n\nA fork of [pyparsing](https://github.com/pyparsing/pyparsing) for faster parsing\n\n\n## Installation\n\nThis is a pypi package\n\n    pip install mo-parsing\n    \n## Usage\n\nThis module allows you to define a PEG parser using predefined patterns and Python operators.  Here is an example \n\n```\n>>> from mo_parsing import Word\n>>> from mo_parsing.utils import alphas\n>>>\n>>> greet = Word(alphas)("greeting") + "," + Word(alphas)("person") + "!"\n>>> result = greet.parse_string("Hello, World!")\n```\n\nThe `result` can be accessed as a nested list\n\n```\n>>> list(result)\n[\'Hello\', \',\', \'World\', \'!\']\n```\n\nThe `result` can also be accessed as a dictionary\n\n```\n>>> dict(result)\n{\'greeting\': \'Hello\', \'person\': \'World\'}\n```\n\nRead the [pyparsing documentation](https://github.com/pyparsing/pyparsing/#readme) for more\n\n### The `Whitespace` Context\n\nThe `mo_parsing.whitespaces.CURRENT` is used during parser creation: It is effectively defines what "whitespace" to skip during parsing, with additional features to simplify the language definition.  You declare "standard" `Whitespace` like so:\n\n    with Whitespace() as whitespace:\n        # PUT YOUR LANGUAGE DEFINITION HERE (space, tab and CR are "whitespace")\n\nIf you are declaring a large language, and you want to minimize indentation, and you are careful, you may also use this pattern:\n\n    whitespace = Whitespace().use()\n    # PUT YOUR LANGUAGE DEFINITION HERE\n    whitespace.release()\n\nThe whitespace can be used to set global parsing parameters, like\n\n* `set_whitespace()` - set the ignored characters (default: `"\\t\\n "`)\n* `add_ignore()` - include whole patterns that are ignored (like comments)\n* `set_literal()` - Set the definition for what `Literal()` means\n* `set_keyword_chars()` - For default `Keyword()` (important for defining word boundary)\n\n\n### Navigating ParseResults\n\nThe results of parsing are in `ParseResults` and are in the form of an n-ary tree; with the children found in `ParseResults.tokens`.  Each `ParseResult.type` points to the `ParserElement` that made it.  In general, if you want to get fancy with post processing (or in a `parse_action`), you will be required to navigate the raw `tokens` to generate a final result\n\nThere are some convenience methods;  \n* `__iter__()` - allows you to iterate through parse results in **depth first search**. Empty results are skipped, and `Group`ed results are treated as atoms (which can be further iterated if required) \n* `name` is a convenient property for `ParseResults.type.token_name`\n* `__getitem__()` - allows you to jump into the parse tree to the given `name`. This is blocked by any names found inside `Group`ed results (because groups are considered atoms).      \n\n### Parse Actions\n\nParse actions are methods that run after a ParserElement found a match. \n\n* Parameters must be accepted in `(tokens, index, string)` order (the opposite of pyparsing)\n* Parse actions are wrapped to ensure the output is a legitimate ParseResult\n  * If your parse action returns `None` then the result is the original `tokens`\n  * If your parse action returns an object, or list, or tuple, then it will be packaged in a `ParseResult` with same type as `tokens`.\n  * If your parse action returns a `ParseResult` then it is accepted ***even if is belongs to some other pattern***\n  \n#### Simple example:\n\n```\ninteger = Word("0123456789").add_parse_action(lambda t, i, s: int(t[0]))\nresult = integer.parse_string("42")\nassert (result[0] == 42)\n```\n\nFor slightly shorter specification, you may use the `/` operator and only parameters you need:\n\n```\ninteger = Word("0123456789") / (lambda t: int(t[0]))\nresult = integer.parse_string("42")\nassert (result[0] == 42)\n```\n\n### Debugging\n\nThe PEG-style of mo-parsing (from pyparsing) makes a very expressible and readable specification, but debugging a parser is still hard.  To look deeper into what the parser is doing use the `Debugger`:\n\n```\nwith Debugger():\n    expr.parse_string("my new language")\n```\n\nThe debugger will print out details of what\'s happening\n\n* Each attempt, and if it matched or failed\n* A small number of bytes to show you the current position\n* location, line and column for more info about the current position\n* whitespace indicating stack depth\n* print out of the ParserElement performing the attempt\n\nThis should help to isolate the exact position your grammar is failing. \n\n### Regular Expressions\n\n`mo-parsing` can parse and generate regular expressions. `ParserElement` has a `__regex__()` function that returns the regular expression for the given grammar; which works up to a limit, and is used internally to accelerate parsing.  The `Regex` class parses regular expressions into a grammar; it is used to optimize parsing, and you may find it useful to decompose regular expressions that look like line noise.\n\n\n## Differences from PyParsing\n\nThis fork was originally created to support faster parsing for [mo-sql-parsing](https://github.com/klahnakoski/moz-sql-parser).  Since then it has deviated sufficiently to be it\'s own collection of parser specification functions.  Here are the differences:\n\n* Added `Whitespace`, which controls parsing context and whitespace.  It replaces the whitespace modifying methods of pyparsing\n* the wildcard ("`*`") could be used in pyparsing to indicate multi-values are expected; this is not allowed in `mo-parsing`: all values are multi-values\n* ParserElements are static: For example, `expr.add_parse_action(action)` creates a new ParserElement, so must be assigned to variable or it is lost. **This is the biggest source of bugs when converting from pyparsing**\n* removed all backward-compatibility settings\n* no support for binary serialization (no pickle)\n\nFaster Parsing\n\n* faster infix operator parsing (main reason for this fork)\n* ParseResults point to ParserElement for reduced size\n* regex used to reduce the number of failed parse attempts  \n* packrat parser is not need\n* less stack used \n\n\n\n## Contributing\n\nIf you plan to extend or enhance this code, please [see the README in the tests directory](https://github.com/klahnakoski/mo-parsing/blob/dev/tests/README.md)',
     long_description_content_type='text/markdown',
     name='mo-parsing',
     packages=["mo_parsing"],
     url='https://github.com/klahnakoski/mo-parsing',
-    version='8.639.24140'
+    version='8.645.24152'
 )
```

