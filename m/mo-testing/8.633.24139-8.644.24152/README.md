# Comparing `tmp/mo_testing-8.633.24139.tar.gz` & `tmp/mo_testing-8.644.24152.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo_testing-8.633.24139.tar", last modified: Sat May 18 04:28:54 2024, max compression
+gzip compressed data, was "mo_testing-8.644.24152.tar", last modified: Fri May 31 01:44:18 2024, max compression
```

## Comparing `mo_testing-8.633.24139.tar` & `mo_testing-8.644.24152.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 04:28:54.399289 mo_testing-8.633.24139/
--rw-rw-rw-   0        0        0    16725 2019-11-12 20:39:14.000000 mo_testing-8.633.24139/LICENSE
--rw-rw-rw-   0        0        0     2836 2024-05-18 04:28:54.398257 mo_testing-8.633.24139/PKG-INFO
--rw-rw-rw-   0        0        0     1630 2024-04-21 13:20:38.000000 mo_testing-8.633.24139/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 04:28:54.382758 mo_testing-8.633.24139/mo_testing/
--rw-rw-rw-   0        0        0      493 2024-04-28 20:32:37.000000 mo_testing-8.633.24139/mo_testing/__init__.py
--rw-rw-rw-   0        0        0    12607 2024-05-18 04:28:46.000000 mo_testing-8.633.24139/mo_testing/fuzzytestcase.py
-drwxrwxrwx   0        0        0        0 2024-05-18 04:28:54.396981 mo_testing-8.633.24139/mo_testing.egg-info/
--rw-rw-rw-   0        0        0     2836 2024-05-18 04:28:54.000000 mo_testing-8.633.24139/mo_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-05-18 04:28:54.000000 mo_testing-8.633.24139/mo_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 04:28:54.000000 mo_testing-8.633.24139/mo_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      135 2024-05-18 04:28:54.000000 mo_testing-8.633.24139/mo_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-18 04:28:54.000000 mo_testing-8.633.24139/mo_testing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 04:28:54.399289 mo_testing-8.633.24139/setup.cfg
--rw-rw-rw-   0        0        0     2819 2024-05-18 04:28:49.000000 mo_testing-8.633.24139/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 01:44:18.437208 mo_testing-8.644.24152/
+-rw-rw-rw-   0        0        0    16725 2019-11-12 20:39:14.000000 mo_testing-8.644.24152/LICENSE
+-rw-rw-rw-   0        0        0     2836 2024-05-31 01:44:18.435629 mo_testing-8.644.24152/PKG-INFO
+-rw-rw-rw-   0        0        0     1630 2024-04-21 13:20:38.000000 mo_testing-8.644.24152/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 01:44:18.424837 mo_testing-8.644.24152/mo_testing/
+-rw-rw-rw-   0        0        0      493 2024-04-28 20:32:37.000000 mo_testing-8.644.24152/mo_testing/__init__.py
+-rw-rw-rw-   0        0        0    12607 2024-05-31 01:44:09.000000 mo_testing-8.644.24152/mo_testing/fuzzytestcase.py
+drwxrwxrwx   0        0        0        0 2024-05-31 01:44:18.434615 mo_testing-8.644.24152/mo_testing.egg-info/
+-rw-rw-rw-   0        0        0     2836 2024-05-31 01:44:18.000000 mo_testing-8.644.24152/mo_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-05-31 01:44:18.000000 mo_testing-8.644.24152/mo_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 01:44:18.000000 mo_testing-8.644.24152/mo_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2024-05-31 01:44:18.000000 mo_testing-8.644.24152/mo_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-31 01:44:18.000000 mo_testing-8.644.24152/mo_testing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 01:44:18.437208 mo_testing-8.644.24152/setup.cfg
+-rw-rw-rw-   0        0        0     2819 2024-05-31 01:44:13.000000 mo_testing-8.644.24152/setup.py
```

### Comparing `mo_testing-8.633.24139/LICENSE` & `mo_testing-8.644.24152/LICENSE`

 * *Files identical despite different names*

### Comparing `mo_testing-8.633.24139/PKG-INFO` & `mo_testing-8.644.24152/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-testing
-Version: 8.633.24139
+Version: 8.644.24152
 Summary: More Testing! Extends the `unittest.TestCase` to provide deep, yet fuzzy, structural comparisons
 Home-page: https://github.com/klahnakoski/mo-testing
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `mo_testing-8.633.24139/README.md` & `mo_testing-8.644.24152/README.md`

 * *Files identical despite different names*

### Comparing `mo_testing-8.633.24139/mo_testing/fuzzytestcase.py` & `mo_testing-8.644.24152/mo_testing/fuzzytestcase.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     first_cause = None
     if is_list(test) and len(test)==1 and is_many(test[0]) and is_many(expected):
         try:
             return assertAlmostEqual(test[0], expected, msg=msg, digits=digits, places=places, delta=delta)
         except Exception as cause:
             first_cause = cause
 
-    if is_list(test) and isinstance(expected, set):
+    if is_many(test) and isinstance(expected, set):
         test = set(to_data(t) for t in test)
         if len(test) != len(expected):
             Log.error(
                 "Sets do not match, element count"
                 " different:\n{test|json|indent}\nexpecting{expectedtest|json|indent}",
                 test=test,
                 expected=expected,
```

### Comparing `mo_testing-8.633.24139/mo_testing.egg-info/PKG-INFO` & `mo_testing-8.644.24152/mo_testing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-testing
-Version: 8.633.24139
+Version: 8.644.24152
 Summary: More Testing! Extends the `unittest.TestCase` to provide deep, yet fuzzy, structural comparisons
 Home-page: https://github.com/klahnakoski/mo-testing
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `mo_testing-8.633.24139/setup.py` & `mo_testing-8.644.24152/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,9 +11,9 @@
     install_requires=["mo-dots==10.632.24139","mo-future==7.584.24095","mo-logs==8.632.24139","mo-math==7.632.24139","mo-times==5.632.24139"],
     license='MPL 2.0',
     long_description='# More Testing\n\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-testing.svg)](https://pypi.org/project/mo-testing/)\n[![Build Status](https://github.com/klahnakoski/mo-testing/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-testing/actions/workflows/build.yml)\n[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-testing/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-testing?branch=dev)\n[![Downloads](https://pepy.tech/badge/mo-testing/month)](https://pepy.tech/project/mo-testing)\n\n\n`FuzzyTestCase` extends the `unittest.TestCase` to provide deep, yet fuzzy, structural comparisons; intended for use in test cases dealing with JSON.\n\n\n## Details\n\nThe primary method is the `assertAlmostEqual` method with the following arguments:\n\n* `test_value` - the value, or structure being tested\n* `expected` - the expected value or structure.  In the case of a number, the accuracy is controlled by the following parameters.  In the case of a structure, only the not-null parameters of `expected` are tested for existence.\n* `msg` - Detailed error message if there is no match\n\nKeyword arguments:\n* `digits` - number of decimal places of accuracy required to consider two values equal\n* `places` - number of significant digits used to compare values for accuracy\n* `delta` - maximum difference between values for them to be equal\n\nThis method `assertEqual` is recursive; it does a deep comparison; it can not handle cycles in the data structure.\n\n## Major Changes\n\n### Version 8\n\n* `digits`, `places`, and `delta` must be specified as keyword arguments\n',
     long_description_content_type='text/markdown',
     name='mo-testing',
     packages=["mo_testing"],
     url='https://github.com/klahnakoski/mo-testing',
-    version='8.633.24139'
+    version='8.644.24152'
 )
```

