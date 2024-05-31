# Comparing `tmp/domaintools_api-1.0.1.tar.gz` & `tmp/domaintools_api-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domaintools_api-1.0.1.tar", last modified: Thu Aug 11 13:47:10 2022, max compression
+gzip compressed data, was "domaintools_api-2.0.0.tar", last modified: Fri May 31 16:44:57 2024, max compression
```

## Comparing `domaintools_api-1.0.1.tar` & `domaintools_api-2.0.0.tar`

### file list

```diff
@@ -1,24 +1,46 @@
-drwxr-xr-x   0 jsarmiento   (502) staff       (20)        0 2022-08-11 13:47:10.874152 domaintools_api-1.0.1/
--rw-r--r--   0 jsarmiento   (502) staff       (20)     1078 2022-07-26 16:45:40.000000 domaintools_api-1.0.1/LICENSE
--rw-r--r--   0 jsarmiento   (502) staff       (20)     8142 2022-08-11 13:47:10.874517 domaintools_api-1.0.1/PKG-INFO
--rw-r--r--   0 jsarmiento   (502) staff       (20)     7230 2022-07-26 16:45:40.000000 domaintools_api-1.0.1/README.md
-drwxr-xr-x   0 jsarmiento   (502) staff       (20)        0 2022-08-11 13:47:10.868934 domaintools_api-1.0.1/domaintools/
--rw-r--r--   0 jsarmiento   (502) staff       (20)      134 2022-07-26 16:45:40.000000 domaintools_api-1.0.1/domaintools/__init__.py
--rw-r--r--   0 jsarmiento   (502) staff       (20)     1180 2022-08-11 13:30:30.000000 domaintools_api-1.0.1/domaintools/_version.py
--rw-r--r--   0 jsarmiento   (502) staff       (20)    37211 2022-08-11 13:30:30.000000 domaintools_api-1.0.1/domaintools/api.py
--rw-r--r--   0 jsarmiento   (502) staff       (20)     8893 2022-08-11 13:30:30.000000 domaintools_api-1.0.1/domaintools/base_results.py
--rw-r--r--   0 jsarmiento   (502) staff       (20)     4802 2022-07-26 16:45:40.000000 domaintools_api-1.0.1/domaintools/cli.py
--rw-r--r--   0 jsarmiento   (502) staff       (20)      687 2022-07-26 16:45:40.000000 domaintools_api-1.0.1/domaintools/exceptions.py
--rw-r--r--   0 jsarmiento   (502) staff       (20)     3674 2022-07-26 16:45:40.000000 domaintools_api-1.0.1/domaintools/results.py
--rw-r--r--   0 jsarmiento   (502) staff       (20)     5254 2022-07-26 16:45:40.000000 domaintools_api-1.0.1/domaintools/utils.py
-drwxr-xr-x   0 jsarmiento   (502) staff       (20)        0 2022-08-11 13:47:10.872494 domaintools_api-1.0.1/domaintools_api.egg-info/
--rw-r--r--   0 jsarmiento   (502) staff       (20)     8142 2022-08-11 13:47:10.000000 domaintools_api-1.0.1/domaintools_api.egg-info/PKG-INFO
--rw-r--r--   0 jsarmiento   (502) staff       (20)      486 2022-08-11 13:47:10.000000 domaintools_api-1.0.1/domaintools_api.egg-info/SOURCES.txt
--rw-r--r--   0 jsarmiento   (502) staff       (20)        1 2022-08-11 13:47:10.000000 domaintools_api-1.0.1/domaintools_api.egg-info/dependency_links.txt
--rw-r--r--   0 jsarmiento   (502) staff       (20)       52 2022-08-11 13:47:10.000000 domaintools_api-1.0.1/domaintools_api.egg-info/entry_points.txt
--rw-r--r--   0 jsarmiento   (502) staff       (20)       17 2022-08-11 13:47:10.000000 domaintools_api-1.0.1/domaintools_api.egg-info/requires.txt
--rw-r--r--   0 jsarmiento   (502) staff       (20)       30 2022-08-11 13:47:10.000000 domaintools_api-1.0.1/domaintools_api.egg-info/top_level.txt
-drwxr-xr-x   0 jsarmiento   (502) staff       (20)        0 2022-08-11 13:47:10.873370 domaintools_api-1.0.1/domaintools_async/
--rw-r--r--   0 jsarmiento   (502) staff       (20)     3015 2022-08-11 13:30:30.000000 domaintools_api-1.0.1/domaintools_async/__init__.py
--rw-r--r--   0 jsarmiento   (502) staff       (20)      172 2022-08-11 13:47:10.876094 domaintools_api-1.0.1/setup.cfg
--rwxr-xr-x   0 jsarmiento   (502) staff       (20)     3050 2022-08-11 13:30:30.000000 domaintools_api-1.0.1/setup.py
+drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-31 16:44:57.111316 domaintools_api-2.0.0/
+-rw-r--r--   0 bluza      (502) staff       (20)     1078 2024-02-26 14:17:41.000000 domaintools_api-2.0.0/LICENSE
+-rw-r--r--   0 bluza      (502) staff       (20)     9688 2024-05-31 16:44:57.111084 domaintools_api-2.0.0/PKG-INFO
+-rw-r--r--   0 bluza      (502) staff       (20)     7230 2024-03-04 18:03:36.000000 domaintools_api-2.0.0/README.md
+-rw-r--r--   0 bluza      (502) staff       (20)        5 2024-05-31 16:44:10.000000 domaintools_api-2.0.0/VERSION
+drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-31 16:44:57.100490 domaintools_api-2.0.0/domaintools/
+-rw-r--r--   0 bluza      (502) staff       (20)      135 2024-05-31 16:44:10.000000 domaintools_api-2.0.0/domaintools/__init__.py
+-rw-r--r--   0 bluza      (502) staff       (20)     1181 2024-05-31 16:44:10.000000 domaintools_api-2.0.0/domaintools/_version.py
+-rw-r--r--   0 bluza      (502) staff       (20)    43189 2024-05-31 16:44:10.000000 domaintools_api-2.0.0/domaintools/api.py
+-rw-r--r--   0 bluza      (502) staff       (20)     8893 2024-02-26 14:17:41.000000 domaintools_api-2.0.0/domaintools/base_results.py
+drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-31 16:44:57.102337 domaintools_api-2.0.0/domaintools/cli/
+-rw-r--r--   0 bluza      (502) staff       (20)      141 2024-05-31 16:44:10.000000 domaintools_api-2.0.0/domaintools/cli/__init__.py
+-rw-r--r--   0 bluza      (502) staff       (20)     8096 2024-05-31 16:44:10.000000 domaintools_api-2.0.0/domaintools/cli/api.py
+drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-31 16:44:57.104912 domaintools_api-2.0.0/domaintools/cli/commands/
+-rw-r--r--   0 bluza      (502) staff       (20)      133 2024-05-31 16:44:10.000000 domaintools_api-2.0.0/domaintools/cli/commands/__init__.py
+-rw-r--r--   0 bluza      (502) staff       (20)     2821 2024-05-31 16:44:10.000000 domaintools_api-2.0.0/domaintools/cli/commands/accounts.py
+-rw-r--r--   0 bluza      (502) staff       (20)    18499 2024-05-31 16:44:10.000000 domaintools_api-2.0.0/domaintools/cli/commands/detects.py
+-rw-r--r--   0 bluza      (502) staff       (20)    23353 2024-05-31 16:44:10.000000 domaintools_api-2.0.0/domaintools/cli/commands/domains.py
+-rw-r--r--   0 bluza      (502) staff       (20)     6831 2024-05-31 16:44:10.000000 domaintools_api-2.0.0/domaintools/cli/commands/ips.py
+-rw-r--r--   0 bluza      (502) staff       (20)     6779 2024-05-31 16:44:10.000000 domaintools_api-2.0.0/domaintools/cli/commands/iris.py
+-rw-r--r--   0 bluza      (502) staff       (20)     3313 2024-05-31 16:44:10.000000 domaintools_api-2.0.0/domaintools/cli/commands/phisheye.py
+-rw-r--r--   0 bluza      (502) staff       (20)     1266 2024-05-31 16:44:10.000000 domaintools_api-2.0.0/domaintools/cli/constants.py
+-rw-r--r--   0 bluza      (502) staff       (20)      505 2024-05-31 16:44:10.000000 domaintools_api-2.0.0/domaintools/cli/main.py
+-rw-r--r--   0 bluza      (502) staff       (20)     6424 2024-05-31 16:44:10.000000 domaintools_api-2.0.0/domaintools/cli/utils.py
+-rw-r--r--   0 bluza      (502) staff       (20)      687 2024-02-26 14:17:41.000000 domaintools_api-2.0.0/domaintools/exceptions.py
+-rw-r--r--   0 bluza      (502) staff       (20)     5216 2024-05-31 16:44:10.000000 domaintools_api-2.0.0/domaintools/filters.py
+-rw-r--r--   0 bluza      (502) staff       (20)     3674 2024-02-26 14:17:41.000000 domaintools_api-2.0.0/domaintools/results.py
+-rw-r--r--   0 bluza      (502) staff       (20)     5811 2024-05-31 16:44:10.000000 domaintools_api-2.0.0/domaintools/utils.py
+drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-31 16:44:57.110479 domaintools_api-2.0.0/domaintools_api.egg-info/
+-rw-r--r--   0 bluza      (502) staff       (20)     9688 2024-05-31 16:44:57.000000 domaintools_api-2.0.0/domaintools_api.egg-info/PKG-INFO
+-rw-r--r--   0 bluza      (502) staff       (20)      988 2024-05-31 16:44:57.000000 domaintools_api-2.0.0/domaintools_api.egg-info/SOURCES.txt
+-rw-r--r--   0 bluza      (502) staff       (20)        1 2024-05-31 16:44:57.000000 domaintools_api-2.0.0/domaintools_api.egg-info/dependency_links.txt
+-rw-r--r--   0 bluza      (502) staff       (20)       52 2024-05-31 16:44:57.000000 domaintools_api-2.0.0/domaintools_api.egg-info/entry_points.txt
+-rw-r--r--   0 bluza      (502) staff       (20)       37 2024-05-31 16:44:57.000000 domaintools_api-2.0.0/domaintools_api.egg-info/requires.txt
+-rw-r--r--   0 bluza      (502) staff       (20)       30 2024-05-31 16:44:57.000000 domaintools_api-2.0.0/domaintools_api.egg-info/top_level.txt
+drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-31 16:44:57.106631 domaintools_api-2.0.0/domaintools_async/
+-rw-r--r--   0 bluza      (502) staff       (20)     3015 2024-02-26 14:17:41.000000 domaintools_api-2.0.0/domaintools_async/__init__.py
+-rw-r--r--   0 bluza      (502) staff       (20)     1450 2024-05-31 16:44:10.000000 domaintools_api-2.0.0/pyproject.toml
+-rw-r--r--   0 bluza      (502) staff       (20)      172 2024-05-31 16:44:57.111762 domaintools_api-2.0.0/setup.cfg
+-rwxr-xr-x   0 bluza      (502) staff       (20)     1541 2024-05-31 16:44:10.000000 domaintools_api-2.0.0/setup.py
+drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-31 16:44:57.108276 domaintools_api-2.0.0/tests/
+-rw-r--r--   0 bluza      (502) staff       (20)    15279 2024-05-31 16:44:10.000000 domaintools_api-2.0.0/tests/test_api.py
+-rw-r--r--   0 bluza      (502) staff       (20)     1760 2024-02-26 14:17:41.000000 domaintools_api-2.0.0/tests/test_async.py
+-rw-r--r--   0 bluza      (502) staff       (20)      997 2024-05-31 16:44:10.000000 domaintools_api-2.0.0/tests/test_cli.py
+-rw-r--r--   0 bluza      (502) staff       (20)     3004 2024-05-31 16:44:10.000000 domaintools_api-2.0.0/tests/test_filters.py
+-rw-r--r--   0 bluza      (502) staff       (20)     4055 2024-02-26 14:17:41.000000 domaintools_api-2.0.0/tests/test_utils.py
```

### Comparing `domaintools_api-1.0.1/LICENSE` & `domaintools_api-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `domaintools_api-1.0.1/PKG-INFO` & `domaintools_api-2.0.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: domaintools_api
-Version: 1.0.1
-Summary: DomainTools Official Python API
-Home-page: https://github.com/domaintools/python_api
-Author: DomainTools
-Author-email: integrations@domaintools.com
-License: MIT
-Keywords: Python,Python3
-Classifier: Development Status :: 6 - Mature
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![domaintools](https://github.com/DomainTools/python_api/raw/main/artwork/logo.png)
 ===================
 
 [![PyPI version](https://badge.fury.io/py/domaintools_api.svg)](http://badge.fury.io/py/domaintools_api)
 [![CI Status](https://github.com/domaintools/python_api/workflows/Tests/badge.svg)](https://github.com/domaintools/python_api/actions)
 [![Coverage Status](https://coveralls.io/repos/github/DomainTools/python_api/badge.svg?branch=main)](https://coveralls.io/github/DomainTools/python_api?branch=main)
 [![License](https://img.shields.io/github/license/mashape/apistatus.svg)](https://pypi.python.org/pypi/domaintools_api/)
```

#### html2text {}

```diff
@@ -1,68 +1,55 @@
-Metadata-Version: 2.1 Name: domaintools_api Version: 1.0.1 Summary: DomainTools
-Official Python API Home-page: https://github.com/domaintools/python_api
-Author: DomainTools Author-email: integrations@domaintools.com License: MIT
-Keywords: Python,Python3 Classifier: Development Status :: 6 - Mature
-Classifier: Intended Audience :: Developers Classifier: Natural Language ::
-English Classifier: Environment :: Console Classifier: License :: OSI Approved
-:: MIT License Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3.6 Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Utilities Description-Content-Type: text/markdown License-
-File: LICENSE ![domaintools](https://github.com/DomainTools/python_api/raw/
-main/artwork/logo.png) =================== [![PyPI version](https://
-badge.fury.io/py/domaintools_api.svg)](http://badge.fury.io/py/domaintools_api)
-[![CI Status](https://github.com/domaintools/python_api/workflows/Tests/
-badge.svg)](https://github.com/domaintools/python_api/actions) [![Coverage
-Status](https://coveralls.io/repos/github/DomainTools/python_api/
-badge.svg?branch=main)](https://coveralls.io/github/DomainTools/
-python_api?branch=main) [![License](https://img.shields.io/github/license/
-mashape/apistatus.svg)](https://pypi.python.org/pypi/domaintools_api/
-) DomainTools Official Python API ![domaintools Example](https://github.com/
-DomainTools/python_api/raw/main/artwork/example.gif) The DomainTools Python API
-Wrapper provides an interface to work with our cybersecurity and related data
-tools provided by our Iris Investigateâ¢, Iris Enrichâ¢, and Iris Detectâ¢
-products. It is actively maintained and may be downloaded via _G_i_t_H_u_b or _P_y_P_I.
-See the included README file, the examples folder, and API documentation
-(https://app.swaggerhub.com/apis-docs/DomainToolsLLC/DomainTools_APIs/1.0#) for
-more info. Installing the DomainTools API =================== To install the
-API run ```bash pip install domaintools_api --upgrade ``` Ideally, within a
-virtual environment. Using the API =================== To start out create an
-instance of the API - passing in your credentials ```python from domaintools
-import API api = API(USER_NAME, KEY) ``` Every API endpoint is then exposed as
-a method on the API object, with any parameters that should be passed into that
-endpoint being passed in as method arguments: ```python api.iris_enrich
-('domaintools.com') ``` You can get an overview of every endpoint that you can
-interact with using the builtin help function: ```python help(api) ``` Or if
-you know the endpoint you want to use, you can get more information about it:
-```python help(api.iris_investigate) ``` If applicable, native Python looping
-can be used directly to loop through any results: ```python for result in
-api.iris_enrich('domaintools.com').response().get('results', {}): print(result
-['domain']) ``` You can also use a context manager to ensure processing on the
-results only occurs if the request is successfully made: ```python with
-api.iris_enrich('domaintools.com').response().get('results', {}) as results:
-print(results) ``` For API calls where a single item is expected to be
-returned, you can directly interact with the result: ```python profile =
-api.domain_profile('google.com') title = profile['website_data']['title'] ```
-For any API call where a single type of data is expected you can directly cast
-to the desired type: ```python float(api.reputation('google.com')) == 0.0 int
-(api.reputation('google.com')) == 0 ``` The entire structure returned from
-DomainTools can be retrieved by doing `.data()` while just the actionable
-response information can be retrieved by doing `.response()`: ```python
-api.iris_enrich('domaintools.com').data() == {'response': { ... }}
-api.iris_enrich('domaintools.com').response() == { ... } ``` You can directly
-get the html, xml, or json version of the response by calling `.(html|xml|json)
-()` These only work with non AsyncResults: ```python json = str
-(api.domain_search('google').json()) xml = str(api.domain_search('google').xml
-()) html = str(api.domain_search('google').html()) ``` If any API call is
-unsuccesfull, one of the exceptions defined in `domaintools.exceptions` will be
-raised: ```python-traceback api.domain_profile('notvalid').data() -------------
--------------------------------------------------------------
+![domaintools](https://github.com/DomainTools/python_api/raw/main/artwork/
+logo.png) =================== [![PyPI version](https://badge.fury.io/py/
+domaintools_api.svg)](http://badge.fury.io/py/domaintools_api) [![CI Status]
+(https://github.com/domaintools/python_api/workflows/Tests/badge.svg)](https://
+github.com/domaintools/python_api/actions) [![Coverage Status](https://
+coveralls.io/repos/github/DomainTools/python_api/badge.svg?branch=main)](https:
+//coveralls.io/github/DomainTools/python_api?branch=main) [![License](https://
+img.shields.io/github/license/mashape/apistatus.svg)](https://pypi.python.org/
+pypi/domaintools_api/) DomainTools Official Python API ![domaintools Example]
+(https://github.com/DomainTools/python_api/raw/main/artwork/example.gif) The
+DomainTools Python API Wrapper provides an interface to work with our
+cybersecurity and related data tools provided by our Iris Investigateâ¢, Iris
+Enrichâ¢, and Iris Detectâ¢ products. It is actively maintained and may be
+downloaded via _G_i_t_H_u_b or _P_y_P_I. See the included README file, the examples
+folder, and API documentation (https://app.swaggerhub.com/apis-docs/
+DomainToolsLLC/DomainTools_APIs/1.0#) for more info. Installing the DomainTools
+API =================== To install the API run ```bash pip install
+domaintools_api --upgrade ``` Ideally, within a virtual environment. Using the
+API =================== To start out create an instance of the API - passing in
+your credentials ```python from domaintools import API api = API(USER_NAME,
+KEY) ``` Every API endpoint is then exposed as a method on the API object, with
+any parameters that should be passed into that endpoint being passed in as
+method arguments: ```python api.iris_enrich('domaintools.com') ``` You can get
+an overview of every endpoint that you can interact with using the builtin help
+function: ```python help(api) ``` Or if you know the endpoint you want to use,
+you can get more information about it: ```python help(api.iris_investigate) ```
+If applicable, native Python looping can be used directly to loop through any
+results: ```python for result in api.iris_enrich('domaintools.com').response
+().get('results', {}): print(result['domain']) ``` You can also use a context
+manager to ensure processing on the results only occurs if the request is
+successfully made: ```python with api.iris_enrich('domaintools.com').response
+().get('results', {}) as results: print(results) ``` For API calls where a
+single item is expected to be returned, you can directly interact with the
+result: ```python profile = api.domain_profile('google.com') title = profile
+['website_data']['title'] ``` For any API call where a single type of data is
+expected you can directly cast to the desired type: ```python float
+(api.reputation('google.com')) == 0.0 int(api.reputation('google.com')) == 0
+``` The entire structure returned from DomainTools can be retrieved by doing
+`.data()` while just the actionable response information can be retrieved by
+doing `.response()`: ```python api.iris_enrich('domaintools.com').data() ==
+{'response': { ... }} api.iris_enrich('domaintools.com').response() == { ... }
+``` You can directly get the html, xml, or json version of the response by
+calling `.(html|xml|json)()` These only work with non AsyncResults: ```python
+json = str(api.domain_search('google').json()) xml = str(api.domain_search
+('google').xml()) html = str(api.domain_search('google').html()) ``` If any API
+call is unsuccesfull, one of the exceptions defined in `domaintools.exceptions`
+will be raised: ```python-traceback api.domain_profile('notvalid').data() -----
+---------------------------------------------------------------------
 - BadRequestException Traceback (most recent call last) in () ----> 1
 api.domain_profile('google').data() /home/tcrosley/projects/external/
 python_api/venv/lib/python3.5/site-packages/domaintools-0.0.1-py3.5.egg/
 domaintools/base_results.py in data(self) 25 self.api._request_session =
 Session() 26 results = self.api._request_session.get(self.url,
 params=self.kwargs) ---> 27 self.status = results.status_code 28 if
 self.kwargs.get('format', 'json') == 'json': 29 self._data = results.json() /
```

### Comparing `domaintools_api-1.0.1/domaintools/_version.py` & `domaintools_api-2.0.0/domaintools/_version.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,8 +15,9 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
 TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
 CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 """
-current = "1.0.1"
+
+current = "2.0.0"
```

### Comparing `domaintools_api-1.0.1/domaintools/api.py` & `domaintools_api-2.0.0/domaintools/api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,342 +1,657 @@
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 from hashlib import sha1, sha256, md5
 from hmac import new as hmac
 from types import MethodType
 import re
 
 from domaintools._version import current as version
 from domaintools.results import GroupedIterable, ParsedWhois, Reputation, Results
+from domaintools.filters import (
+    filter_by_riskscore,
+    filter_by_expire_date,
+    filter_by_date_updated_after,
+    filter_by_field,
+    DTResultFilter,
+)
 
-AVAILABLE_KEY_SIGN_HASHES = ['sha1', 'sha256', 'md5']
+AVAILABLE_KEY_SIGN_HASHES = ["sha1", "sha256", "md5"]
 
 
-def delimited(items, character='|'):
+def delimited(items, character="|"):
     """Returns a character delimited version of the provided list as a Python string"""
     return character.join(items) if type(items) in (list, tuple, set) else items
 
 
 class API(object):
     """Enables interacting with the DomainTools API via Python:
 
-           from domaintools import API
+        from domaintools import API
 
-           api = API('my_name', 'my_key')
-           results = api.domain_search('domain')
+        api = API('my_name', 'my_key')
+        results = api.domain_search('domain')
 
-        By default the API will automatically space out your requests to match your rate limits.
-        If your running over multiple Python runtimes, have your own rate limiting approach, or are doing a one-off
-        query (such as for a CLI command) you can set rate_limit=False to turn this feature off.
+     By default the API will automatically space out your requests to match your rate limits.
+     If your running over multiple Python runtimes, have your own rate limiting approach, or are doing a one-off
+     query (such as for a CLI command) you can set rate_limit=False to turn this feature off.
 
-        If you encounter SSL errors you can pass in verify_ssl=False to avoid verification of the SSL cert.
-        To use the API without SSL in it's entirety pass in https=False.
+     If you encounter SSL errors you can pass in verify_ssl=False to avoid verification of the SSL cert.
+     To use the API without SSL in it's entirety pass in https=False.
 
-       For detailed usage information of all API calls see: https://www.domaintools.com/resources/api-documentation/
+    For detailed usage information of all API calls see: https://www.domaintools.com/resources/api-documentation/
     """
+
     limits = {}
     limits_set = False
 
-    def __init__(self, username, key, https=True, verify_ssl=True, rate_limit=True, proxy_url=None,
-                 always_sign_api_key=False, key_sign_hash='sha256', app_name="python_wrapper", app_version=version,
-                 **default_parameters):
+    def __init__(
+        self,
+        username,
+        key,
+        https=True,
+        verify_ssl=True,
+        rate_limit=True,
+        proxy_url=None,
+        always_sign_api_key=False,
+        key_sign_hash="sha256",
+        app_name="python_wrapper",
+        app_version=version,
+        api_url=None,
+        api_port=None,
+        **default_parameters,
+    ):
         if not default_parameters:
             self.default_parameters = {}
         else:
             self.default_parameters = default_parameters
         self.username = username
         self.key = key
         self.https = https
         self.verify_ssl = verify_ssl
         self.rate_limit = rate_limit
         self.proxy_url = proxy_url
         self.extra_request_params = {}
         self.always_sign_api_key = always_sign_api_key
         self.key_sign_hash = key_sign_hash
-        self.default_parameters['app_name'] = app_name
-        self.default_parameters['app_version'] = app_version
+        self.default_parameters["app_name"] = app_name
+        self.default_parameters["app_version"] = app_version
+
+        self._build_api_url(api_url, api_port)
+
         if not https:
-            raise Exception("The DomainTools API endpoints no longer support http traffic. Please make sure https=True.")
+            raise Exception(
+                "The DomainTools API endpoints no longer support http traffic. Please make sure https=True."
+            )
         if proxy_url:
             if isinstance(proxy_url, str):
-                self.proxy_url = {'http://': proxy_url, 'https://': proxy_url}
+                self.proxy_url = {"http://": proxy_url, "https://": proxy_url}
             else:
-                raise Exception("Proxy URL must be a string. For example: '127.0.0.1:8888'")
+                raise Exception(
+                    "Proxy URL must be a string. For example: '127.0.0.1:8888'"
+                )
+
+    def _build_api_url(self, api_url=None, api_port=None):
+        """Build the API url based on the given url and port. Defaults to `https://api.domaintools.com`"""
+        rest_api_url = "https://api.domaintools.com"
+        if api_url:
+            rest_api_url = api_url
+
+        if api_port:
+            rest_api_url = f"{rest_api_url}:{api_port}"
+
+        self._rest_api_url = rest_api_url
 
     def _rate_limit(self):
         """Pulls in and enforces the latest rate limits for the specified user"""
         self.limits_set = True
         for product in self.account_information():
-            limit_minutes = product['per_minute_limit'] or None
-            limit_hours = product['per_hour_limit'] or None
+            limit_minutes = product["per_minute_limit"] or None
+            limit_hours = product["per_hour_limit"] or None
 
-            default = 3600 
+            default = 3600
             hours = limit_hours and 3600 / float(limit_hours)
             minutes = limit_minutes and 60 / float(limit_minutes)
 
-            self.limits[product['id']] = {'interval': timedelta(
-                seconds = minutes or hours or default 
-            )
-        }
+            self.limits[product["id"]] = {
+                "interval": timedelta(seconds=minutes or hours or default)
+            }
 
     def _results(self, product, path, cls=Results, **kwargs):
         """Returns _results for the specified API path with the specified **kwargs parameters"""
-        if product != 'account-information' and self.rate_limit and not self.limits_set and not self.limits:
+        if (
+            product != "account-information"
+            and self.rate_limit
+            and not self.limits_set
+            and not self.limits
+        ):
             self._rate_limit()
 
-        uri = '/'.join(('https://api.domaintools.com', path.lstrip('/')))
+        uri = "/".join((self._rest_api_url, path.lstrip("/")))
         parameters = self.default_parameters.copy()
-        parameters['api_username'] = self.username
+        parameters["api_username"] = self.username
         self.handle_api_key(path, parameters)
         parameters.update(
             {
                 key: str(value).lower() if value in (True, False) else value
                 for key, value in kwargs.items()
                 if value is not None
             }
         )
 
         return cls(self, product, uri, **parameters)
 
     def handle_api_key(self, path, parameters):
         if self.https and not self.always_sign_api_key:
-            parameters['api_key'] = self.key
+            parameters["api_key"] = self.key
         else:
             if self.key_sign_hash and self.key_sign_hash in AVAILABLE_KEY_SIGN_HASHES:
                 signing_hash = eval(self.key_sign_hash)
             else:
-                raise ValueError("Invalid value '{0}' for 'key_sign_hash'. "
-                                 "Values available are {1}".format(self.key_sign_hash, ','.join(AVAILABLE_KEY_SIGN_HASHES)))
-            parameters['timestamp'] = datetime.utcnow().strftime('%Y-%m-%dT%H:%M:%SZ')
-            parameters['signature'] = hmac(self.key.encode('utf8'),
-                                           ''.join([self.username, parameters['timestamp'], path]).encode('utf8'),
-                                           digestmod=signing_hash).hexdigest()
+                raise ValueError(
+                    "Invalid value '{0}' for 'key_sign_hash'. "
+                    "Values available are {1}".format(
+                        self.key_sign_hash, ",".join(AVAILABLE_KEY_SIGN_HASHES)
+                    )
+                )
+
+            parameters["timestamp"] = datetime.now(timezone.utc).strftime(
+                "%Y-%m-%dT%H:%M:%SZ"
+            )
+            parameters["signature"] = hmac(
+                self.key.encode("utf8"),
+                "".join([self.username, parameters["timestamp"], path]).encode("utf8"),
+                digestmod=signing_hash,
+            ).hexdigest()
 
     def account_information(self, **kwargs):
         """Provides a snapshot of your accounts current API usage"""
-        return self._results('account-information', '/v1/account', items_path=('products',), **kwargs)
+        return self._results(
+            "account-information", "/v1/account", items_path=("products",), **kwargs
+        )
 
     def available_api_calls(self):
         """Provides a list of api calls that you can use based on your account information."""
 
         def snakecase(string):
-            string = re.sub(r"[\-\.\s]", '_', str(string))
+            string = re.sub(r"[\-\.\s]", "_", str(string))
             if not string:
                 return string
-            return str(string[0]).lower() + re.sub(r"[A-Z]", lambda matched: '_' + str(matched.group(0)).lower(),
-                                                   string[1:])
+            return str(string[0]).lower() + re.sub(
+                r"[A-Z]",
+                lambda matched: "_" + str(matched.group(0)).lower(),
+                string[1:],
+            )
 
-        api_calls = tuple((api_call for api_call in dir(API) if not api_call.startswith('_') and
-                           callable(getattr(API, api_call, None))))
-        return sorted([snakecase(p["id"]) for p in self.account_information()["products"] if snakecase(p["id"]) in api_calls])
+        api_calls = tuple(
+            (
+                api_call
+                for api_call in dir(API)
+                if not api_call.startswith("_")
+                and callable(getattr(API, api_call, None))
+            )
+        )
+        return sorted(
+            [
+                snakecase(p["id"])
+                for p in self.account_information()["products"]
+                if snakecase(p["id"]) in api_calls
+            ]
+        )
 
-    def brand_monitor(self, query, exclude=None, domain_status=None, days_back=None, **kwargs):
+    def brand_monitor(
+        self, query, exclude=None, domain_status=None, days_back=None, **kwargs
+    ):
         """Pass in one or more terms as a list or separated by the pipe character ( | )"""
         if exclude is None:
             exclude = []
-        return self._results('mark-alert', '/v1/mark-alert', query=delimited(query), exclude=delimited(exclude),
-                             domain_status=domain_status, days_back=days_back, items_path=('alerts',), **kwargs)
+        return self._results(
+            "mark-alert",
+            "/v1/mark-alert",
+            query=delimited(query),
+            exclude=delimited(exclude),
+            domain_status=domain_status,
+            days_back=days_back,
+            items_path=("alerts",),
+            **kwargs,
+        )
 
     def domain_profile(self, query, **kwargs):
         """Returns a profile for the specified domain name"""
-        return self._results('domain-profile', '/v1/{0}'.format(query))
+        return self._results("domain-profile", "/v1/{0}".format(query))
 
-    def domain_search(self, query, exclude_query=None, max_length=25, min_length=2, has_hyphen=True, has_number=True,
-                      active_only=False, deleted_only=False, anchor_left=False, anchor_right=False, page=1, **kwargs):
+    def domain_search(
+        self,
+        query,
+        exclude_query=None,
+        max_length=25,
+        min_length=2,
+        has_hyphen=True,
+        has_number=True,
+        active_only=False,
+        deleted_only=False,
+        anchor_left=False,
+        anchor_right=False,
+        page=1,
+        **kwargs,
+    ):
         """Each term in the query string must be at least three characters long.
-           Pass in a list or use spaces to separate multiple terms.
+        Pass in a list or use spaces to separate multiple terms.
         """
         if exclude_query is None:
             exclude_query = []
-        return self._results('domain-search', '/v2/domain-search', query=delimited(query, ' '),
-                             exclude_query=delimited(exclude_query, ' '),
-                             max_length=max_length, min_length=min_length, has_hyphen=has_hyphen, has_number=has_number,
-                             active_only=active_only, deleted_only=deleted_only, anchor_left=anchor_left,
-                             anchor_right=anchor_right, page=page, items_path=('results',), **kwargs)
+        return self._results(
+            "domain-search",
+            "/v2/domain-search",
+            query=delimited(query, " "),
+            exclude_query=delimited(exclude_query, " "),
+            max_length=max_length,
+            min_length=min_length,
+            has_hyphen=has_hyphen,
+            has_number=has_number,
+            active_only=active_only,
+            deleted_only=deleted_only,
+            anchor_left=anchor_left,
+            anchor_right=anchor_right,
+            page=page,
+            items_path=("results",),
+            **kwargs,
+        )
 
     def hosting_history(self, query, **kwargs):
         """Returns the hosting history from the given domain name"""
-        return self._results('hosting-history', '/v1/{0}/hosting-history'.format(query), cls=GroupedIterable, **kwargs)
+        return self._results(
+            "hosting-history",
+            "/v1/{0}/hosting-history".format(query),
+            cls=GroupedIterable,
+            **kwargs,
+        )
 
     def ip_monitor(self, query, days_back=0, page=1, **kwargs):
         """Pass in the IP Address you wish to query ( i.e. 199.30.228.112 )."""
-        return self._results('ip-monitor', '/v1/ip-monitor', query=query, days_back=days_back, page=page,
-                             items_path=('alerts',), **kwargs)
+        return self._results(
+            "ip-monitor",
+            "/v1/ip-monitor",
+            query=query,
+            days_back=days_back,
+            page=page,
+            items_path=("alerts",),
+            **kwargs,
+        )
 
-    def ip_registrant_monitor(self, query, days_back=0, search_type="all", server=None, country=None, org=None, page=1,
-                              include_total_count=False, **kwargs):
+    def ip_registrant_monitor(
+        self,
+        query,
+        days_back=0,
+        search_type="all",
+        server=None,
+        country=None,
+        org=None,
+        page=1,
+        include_total_count=False,
+        **kwargs,
+    ):
         """Query based on free text query terms"""
-        return self._results('ip-registrant-monitor', '/v1/ip-registrant-monitor', query=query,
-                             days_back=days_back, search_type=search_type, server=server, country=country, org=org,
-                             page=page, include_total_count=include_total_count, **kwargs)
+        return self._results(
+            "ip-registrant-monitor",
+            "/v1/ip-registrant-monitor",
+            query=query,
+            days_back=days_back,
+            search_type=search_type,
+            server=server,
+            country=country,
+            org=org,
+            page=page,
+            include_total_count=include_total_count,
+            **kwargs,
+        )
 
     def name_server_monitor(self, query, days_back=0, page=1, **kwargs):
         """Pass in the hostname of the Name Server you wish to query ( i.e. dynect.net )."""
-        return self._results('name-server-monitor', '/v1/name-server-monitor', query=query, days_back=days_back,
-                             page=page, items_path=('alerts',), **kwargs)
+        return self._results(
+            "name-server-monitor",
+            "/v1/name-server-monitor",
+            query=query,
+            days_back=days_back,
+            page=page,
+            items_path=("alerts",),
+            **kwargs,
+        )
 
     def parsed_whois(self, query, **kwargs):
         """Pass in a domain name"""
-        return self._results('parsed-whois', '/v1/{0}/whois/parsed'.format(query), cls=ParsedWhois, **kwargs)
+        return self._results(
+            "parsed-whois",
+            "/v1/{0}/whois/parsed".format(query),
+            cls=ParsedWhois,
+            **kwargs,
+        )
 
-    def registrant_monitor(self, query, exclude=None, days_back=0, limit=None, **kwargs):
+    def registrant_monitor(
+        self, query, exclude=None, days_back=0, limit=None, **kwargs
+    ):
         """One or more terms as a Python list or separated by the pipe character ( | )."""
         if exclude is None:
             exclude = []
-        return self._results('registrant-alert', '/v1/registrant-alert', query=delimited(query),
-                             exclude=delimited(exclude), days_back=days_back, limit=limit, items_path=('alerts',),
-                             **kwargs)
+        return self._results(
+            "registrant-alert",
+            "/v1/registrant-alert",
+            query=delimited(query),
+            exclude=delimited(exclude),
+            days_back=days_back,
+            limit=limit,
+            items_path=("alerts",),
+            **kwargs,
+        )
 
     def reputation(self, query, include_reasons=False, **kwargs):
         """Pass in a domain name to see its reputation score"""
-        return self._results('reputation', '/v1/reputation', domain=query, include_reasons=include_reasons,
-                             cls=Reputation, **kwargs)
+        return self._results(
+            "reputation",
+            "/v1/reputation",
+            domain=query,
+            include_reasons=include_reasons,
+            cls=Reputation,
+            **kwargs,
+        )
 
     def reverse_ip(self, domain=None, limit=None, **kwargs):
         """Pass in a domain name."""
-        return self._results('reverse-ip', '/v1/{0}/reverse-ip'.format(domain), limit=limit, **kwargs)
+        return self._results(
+            "reverse-ip", "/v1/{0}/reverse-ip".format(domain), limit=limit, **kwargs
+        )
 
     def host_domains(self, ip=None, limit=None, **kwargs):
         """Pass in an IP address."""
-        return self._results('reverse-ip', '/v1/{0}/host-domains'.format(ip), limit=limit, **kwargs)
+        return self._results(
+            "reverse-ip", "/v1/{0}/host-domains".format(ip), limit=limit, **kwargs
+        )
 
-    def reverse_ip_whois(self, query=None, ip=None, country=None, server=None, include_total_count=False, page=1,
-                         **kwargs):
+    def reverse_ip_whois(
+        self,
+        query=None,
+        ip=None,
+        country=None,
+        server=None,
+        include_total_count=False,
+        page=1,
+        **kwargs,
+    ):
         """Pass in an IP address or a list of free text query terms."""
         if (ip and query) or not (ip or query):
-            raise ValueError('Query or IP Address (but not both) must be defined')
+            raise ValueError("Query or IP Address (but not both) must be defined")
 
-        return self._results('reverse-ip-whois', '/v1/reverse-ip-whois', query=query, ip=ip, country=country,
-                             server=server, include_total_count=include_total_count, page=page, items_path=('records',),
-                             **kwargs)
+        return self._results(
+            "reverse-ip-whois",
+            "/v1/reverse-ip-whois",
+            query=query,
+            ip=ip,
+            country=country,
+            server=server,
+            include_total_count=include_total_count,
+            page=page,
+            items_path=("records",),
+            **kwargs,
+        )
 
     def reverse_name_server(self, query, limit=None, **kwargs):
         """Pass in a domain name or a name server."""
-        return self._results('reverse-name-server', '/v1/{0}/name-server-domains'.format(query),
-                             items_path=('primary_domains',), limit=limit, **kwargs)
+        return self._results(
+            "reverse-name-server",
+            "/v1/{0}/name-server-domains".format(query),
+            items_path=("primary_domains",),
+            limit=limit,
+            **kwargs,
+        )
 
-    def reverse_whois(self, query, exclude=None, scope='current', mode='purchase', **kwargs):
+    def reverse_whois(
+        self, query, exclude=None, scope="current", mode="purchase", **kwargs
+    ):
         """List of one or more terms to search for in the Whois record,
-           as a Python list or separated with the pipe character ( | ).
+        as a Python list or separated with the pipe character ( | ).
         """
         if exclude is None:
             exclude = []
-        return self._results('reverse-whois', '/v1/reverse-whois', terms=delimited(query), exclude=delimited(exclude),
-                             scope=scope, mode=mode, **kwargs)
+        return self._results(
+            "reverse-whois",
+            "/v1/reverse-whois",
+            terms=delimited(query),
+            exclude=delimited(exclude),
+            scope=scope,
+            mode=mode,
+            **kwargs,
+        )
 
     def whois(self, query, **kwargs):
         """Pass in a domain name or an IP address to perform a whois lookup."""
-        return self._results('whois', '/v1/{0}/whois'.format(query), **kwargs)
+        return self._results("whois", "/v1/{0}/whois".format(query), **kwargs)
 
-    def whois_history(self, query, mode=None, sort=None, offset=None, limit=None, **kwargs):
+    def whois_history(
+        self, query, mode=None, sort=None, offset=None, limit=None, **kwargs
+    ):
         """Pass in a domain name."""
-        return self._results('whois-history', '/v1/{0}/whois/history'.format(query), mode=mode, sort=sort,
-                             offset=offset, limit=limit, items_path=('history',), **kwargs)
+        return self._results(
+            "whois-history",
+            "/v1/{0}/whois/history".format(query),
+            mode=mode,
+            sort=sort,
+            offset=offset,
+            limit=limit,
+            items_path=("history",),
+            **kwargs,
+        )
 
     def phisheye(self, query, days_back=None, **kwargs):
         """Returns domain results for the specified term for today or the specified number of days_back.
-           Terms must be setup for monitoring via the web interface: https://research.domaintools.com/phisheye.
+        Terms must be setup for monitoring via the web interface: https://research.domaintools.com/phisheye.
 
-           NOTE: Properties of a domain are only provided if we have been able to obtain them.
-                 Many domains will have incomplete data because that information isn't available in their Whois records,
-                 or they don't have DNS results for a name server or IP address.
+        NOTE: Properties of a domain are only provided if we have been able to obtain them.
+              Many domains will have incomplete data because that information isn't available in their Whois records,
+              or they don't have DNS results for a name server or IP address.
         """
-        return self._results('phisheye', '/v1/phisheye', query=query, days_back=days_back, items_path=('domains',),
-                             **kwargs)
+        return self._results(
+            "phisheye",
+            "/v1/phisheye",
+            query=query,
+            days_back=days_back,
+            items_path=("domains",),
+            **kwargs,
+        )
 
     def phisheye_term_list(self, include_inactive=False, **kwargs):
         """Provides a list of terms that are set up for this account.
-           This call is not charged against your API usage limit.
+        This call is not charged against your API usage limit.
 
-           NOTE: The terms must be configured in the PhishEye web interface: https://research.domaintools.com/phisheye.
-                 There is no API call to set up the terms.
+        NOTE: The terms must be configured in the PhishEye web interface: https://research.domaintools.com/phisheye.
+              There is no API call to set up the terms.
         """
-        return self._results('phisheye_term_list', '/v1/phisheye/term-list', include_inactive=include_inactive,
-                             items_path=('terms',), **kwargs)
+        return self._results(
+            "phisheye_term_list",
+            "/v1/phisheye/term-list",
+            include_inactive=include_inactive,
+            items_path=("terms",),
+            **kwargs,
+        )
 
-    def iris(self, domain=None, ip=None, email=None, nameserver=None, registrar=None, registrant=None,
-             registrant_org=None, **kwargs):
+    def iris(
+        self,
+        domain=None,
+        ip=None,
+        email=None,
+        nameserver=None,
+        registrar=None,
+        registrant=None,
+        registrant_org=None,
+        **kwargs,
+    ):
         """Performs a search for the provided search terms ANDed together,
-           returning the pivot engine row data for the resulting domains.
+        returning the pivot engine row data for the resulting domains.
         """
-        if ((not domain and not ip and not email and not nameserver and not registrar and not registrant and not
-             registrant_org and not kwargs)):
-            raise ValueError('At least one search term must be specified')
-
-        return self._results('iris', '/v1/iris', domain=domain, ip=ip, email=email, nameserver=nameserver,
-                             registrar=registrar, registrant=registrant, registrant_org=registrant_org,
-                             items_path=('results',), **kwargs)
+        if (
+            not domain
+            and not ip
+            and not email
+            and not nameserver
+            and not registrar
+            and not registrant
+            and not registrant_org
+            and not kwargs
+        ):
+            raise ValueError("At least one search term must be specified")
+
+        return self._results(
+            "iris",
+            "/v1/iris",
+            domain=domain,
+            ip=ip,
+            email=email,
+            nameserver=nameserver,
+            registrar=registrar,
+            registrant=registrant,
+            registrant_org=registrant_org,
+            items_path=("results",),
+            **kwargs,
+        )
 
     def risk(self, domain, **kwargs):
         """Returns back the risk score for a given domain"""
-        return self._results('risk', '/v1/risk', items_path=('components',), domain=domain, cls=Reputation,
-                             **kwargs)
+        return self._results(
+            "risk",
+            "/v1/risk",
+            items_path=("components",),
+            domain=domain,
+            cls=Reputation,
+            **kwargs,
+        )
 
     def risk_evidence(self, domain, **kwargs):
         """Returns back the detailed risk evidence associated with a given domain"""
-        return self._results('risk-evidence', '/v1/risk/evidence/', items_path=('components',), domain=domain,
-                             **kwargs)
+        return self._results(
+            "risk-evidence",
+            "/v1/risk/evidence/",
+            items_path=("components",),
+            domain=domain,
+            **kwargs,
+        )
 
     def iris_enrich(self, *domains, **kwargs):
         """Returns back enriched data related to the specified domains using our Iris Enrich service
-           each domain should be passed in as an un-named argument to the method:
-               iris_enrich('domaintools.com', 'google.com')
+        each domain should be passed in as an un-named argument to the method:
+            iris_enrich('domaintools.com', 'google.com')
 
-           api.iris_enrich(*DOMAIN_LIST)['results_count'] Returns the number of results
-           api.iris_enrich(*DOMAIN_LIST)['missing_domains'] Returns any domains that we were unable to
-                                                           retrieve enrichment data for
-           api.iris_enrich(*DOMAIN_LIST)['limit_exceeded'] Returns True if you've exceeded your API usage
-
-           for enrichment in api.iris_enrich(*DOMAIN_LIST):  # Enables looping over all returned enriched domains
-
-           for example:
-               enrich_domains = ['google.com', 'amazon.com']
-               assert api.iris_enrich(*enrich_domains)['missing_domains'] == []
+        api.iris_enrich(*DOMAIN_LIST)['results_count'] Returns the number of results
+        api.iris_enrich(*DOMAIN_LIST)['missing_domains'] Returns any domains that we were unable to
+                                                        retrieve enrichment data for
+        api.iris_enrich(*DOMAIN_LIST)['limit_exceeded'] Returns True if you've exceeded your API usage
+
+        for enrichment in api.iris_enrich(*DOMAIN_LIST):  # Enables looping over all returned enriched domains
+
+        for example:
+            enrich_domains = ['google.com', 'amazon.com']
+            assert api.iris_enrich(*enrich_domains)['missing_domains'] == []
         """
         if not domains:
-            raise ValueError('One or more domains to enrich must be provided')
+            raise ValueError("One or more domains to enrich must be provided")
+
+        domains = ",".join(domains)
+        data_updated_after = kwargs.get("data_updated_after", None)
+        if hasattr(data_updated_after, "strftime"):
+            data_updated_after = data_updated_after.strftime("%Y-%m-%d")
+
+        results = self._results(
+            "iris-enrich",
+            "/v1/iris-enrich/",
+            domain=domains,
+            data_updated_after=data_updated_after,
+            items_path=("results",),
+            **kwargs,
+        )
+
+        risk_score = kwargs.pop("risk_score", {}) or None
+        younger_than_date = kwargs.pop("younger_than_date", {}) or None
+        older_than_date = kwargs.pop("older_than_date", {}) or None
+        updated_after = kwargs.pop("updated_after", {}) or None
+        include_domains_with_missing_field = (
+            kwargs.pop("include_domains_with_missing_field", {}) or None
+        )
+        exclude_domains_with_missing_field = (
+            kwargs.pop("exclude_domains_with_missing_field", {}) or None
+        )
+
+        filtered_results = DTResultFilter(result_set=results).by(
+            [
+                filter_by_riskscore(threshold=risk_score),
+                filter_by_expire_date(date=younger_than_date, lookup_type="before"),
+                filter_by_expire_date(date=older_than_date, lookup_type="after"),
+                filter_by_date_updated_after(date=updated_after),
+                filter_by_field(
+                    field=include_domains_with_missing_field, filter_type="include"
+                ),
+                filter_by_field(
+                    field=exclude_domains_with_missing_field, filter_type="exclude"
+                ),
+            ]
+        )
 
-        domains = ','.join(domains)
-        data_updated_after = kwargs.get('data_updated_after', None)
-        if hasattr(data_updated_after, 'strftime'):
-            data_updated_after = data_updated_after.strftime('%Y-%m-%d')
+        results["results"] = filtered_results
+        results["results_count"] = len(filtered_results)
+        results["total_count"] = len(filtered_results)
 
-        return self._results('iris-enrich', '/v1/iris-enrich/', domain=domains, data_updated_after=data_updated_after,
-                             items_path=('results',), **kwargs)
+        return results
 
     def iris_enrich_cli(self, domains=None, **kwargs):
         """Returns back enriched data related to the specified domains using our Iris Enrich service.
-            This is a CLI version of the iris_enrich method to help maintain backwards compatibility.
+         This is a CLI version of the iris_enrich method to help maintain backwards compatibility.
 
-           api.iris_enrich(['domaintools.com', 'google.com'])
+        api.iris_enrich(['domaintools.com', 'google.com'])
 
-           api.iris_enrich(DOMAIN_LIST)['results_count'] Returns the number of results
-           api.iris_enrich(DOMAIN_LIST)['missing_domains'] Returns any domains that we were unable to
-                                                           retrieve enrichment data for
-           api.iris_enrich(DOMAIN_LIST)['limit_exceeded'] Returns True if you've exceeded your API usage
+        api.iris_enrich(DOMAIN_LIST)['results_count'] Returns the number of results
+        api.iris_enrich(DOMAIN_LIST)['missing_domains'] Returns any domains that we were unable to
+                                                        retrieve enrichment data for
+        api.iris_enrich(DOMAIN_LIST)['limit_exceeded'] Returns True if you've exceeded your API usage
 
-           for enrichment in api.iris_enrich(DOMAIN_LIST):  # Enables looping over all returned enriched domains
+        for enrichment in api.iris_enrich(DOMAIN_LIST):  # Enables looping over all returned enriched domains
 
-           for example:
-               enrich_domains = ['google.com', 'amazon.com']
-               assert api.iris_enrich(*enrich_domains)['missing_domains'] == []
+        for example:
+            enrich_domains = ['google.com', 'amazon.com']
+            assert api.iris_enrich(*enrich_domains)['missing_domains'] == []
         """
         if not domains:
-            raise ValueError('One or more domains to enrich must be provided')
+            raise ValueError("One or more domains to enrich must be provided")
 
         if isinstance(domains, (list, tuple)):
-            domains = ','.join(domains)
-        data_updated_after = kwargs.get('data_updated_after', None)
-        if hasattr(data_updated_after, 'strftime'):
-            data_updated_after = data_updated_after.strftime('%Y-%m-%d')
-
-        return self._results('iris-enrich', '/v1/iris-enrich/', domain=domains, data_updated_after=data_updated_after,
-                             items_path=('results',), **kwargs)
+            domains = ",".join(domains)
+        data_updated_after = kwargs.get("data_updated_after", None)
+        if hasattr(data_updated_after, "strftime"):
+            data_updated_after = data_updated_after.strftime("%Y-%m-%d")
+
+        return self._results(
+            "iris-enrich",
+            "/v1/iris-enrich/",
+            domain=domains,
+            data_updated_after=data_updated_after,
+            items_path=("results",),
+            **kwargs,
+        )
 
-    def iris_investigate(self, domains=None, data_updated_after=None, expiration_date=None,
-                         create_date=None, active=None, search_hash=None, **kwargs):
+    def iris_investigate(
+        self,
+        domains=None,
+        data_updated_after=None,
+        expiration_date=None,
+        create_date=None,
+        active=None,
+        search_hash=None,
+        risk_score=None,
+        younger_than_date=None,
+        older_than_date=None,
+        updated_after=None,
+        include_domains_with_missing_field=None,
+        exclude_domains_with_missing_field=None,
+        **kwargs,
+    ):
         """Returns back a list of domains based on the provided filters.
         The following filters are available beyond what is parameterized as kwargs:
 
             - ip: Search for domains having this IP.
             - email: Search for domains with this email in their data.
             - email_domain: Search for domains where the email address uses this domain.
             - nameserver_host: Search for domains with this nameserver.
@@ -370,36 +685,74 @@
             next_page = api.iris_investigate(QUERY, position=api.iris_investigate(QUERY)['position'])
 
         for enrichment in api.iris_enrich(i):  # Enables looping over all returned enriched domains
 
         """
         # We put search_hash in the signature definition so the CLI can see it as a valid arg
         if search_hash:
-            kwargs['search_hash'] = search_hash
+            kwargs["search_hash"] = search_hash
 
         if not (kwargs or domains):
-            raise ValueError('Need to define investigation using kwarg filters or domains')
+            raise ValueError(
+                "Need to define investigation using kwarg filters or domains"
+            )
 
         if isinstance(domains, (list, tuple)):
-            domains = ','.join(domains)
-        if hasattr(data_updated_after, 'strftime'):
-            data_updated_after = data_updated_after.strftime('%Y-%m-%d')
-        if hasattr(expiration_date, 'strftime'):
-            expiration_date = expiration_date.strftime('%Y-%m-%d')
-        if hasattr(create_date, 'strftime'):
-            create_date = create_date.strftime('%Y-%m-%d')
+            domains = ",".join(domains)
+        if hasattr(data_updated_after, "strftime"):
+            data_updated_after = data_updated_after.strftime("%Y-%m-%d")
+        if hasattr(expiration_date, "strftime"):
+            expiration_date = expiration_date.strftime("%Y-%m-%d")
+        if hasattr(create_date, "strftime"):
+            create_date = create_date.strftime("%Y-%m-%d")
         if isinstance(active, bool):
-            kwargs['active'] = str(active).lower()
+            kwargs["active"] = str(active).lower()
 
-        return self._results('iris-investigate', '/v1/iris-investigate/', domain=domains,
-                             data_updated_after=data_updated_after, expiration_date=expiration_date,
-                             create_date=create_date, items_path=('results',), **kwargs)
+        results = self._results(
+            "iris-investigate",
+            "/v1/iris-investigate/",
+            domain=domains,
+            data_updated_after=data_updated_after,
+            expiration_date=expiration_date,
+            create_date=create_date,
+            items_path=("results",),
+            **kwargs,
+        )
 
-    def iris_detect_monitors(self, include_counts=False, datetime_counts_since=None, sort=None, order="desc", offset=0,
-                             limit=None, **kwargs):
+        filtered_results = DTResultFilter(result_set=results).by(
+            [
+                filter_by_riskscore(threshold=risk_score),
+                filter_by_expire_date(date=younger_than_date, lookup_type="before"),
+                filter_by_expire_date(date=older_than_date, lookup_type="after"),
+                filter_by_date_updated_after(date=updated_after),
+                filter_by_field(
+                    field=include_domains_with_missing_field, filter_type="include"
+                ),
+                filter_by_field(
+                    field=exclude_domains_with_missing_field, filter_type="exclude"
+                ),
+            ]
+        )
+
+        results["results"] = filtered_results
+        results["results_count"] = len(filtered_results)
+        results["total_count"] = len(filtered_results)
+
+        return results
+
+    def iris_detect_monitors(
+        self,
+        include_counts=False,
+        datetime_counts_since=None,
+        sort=None,
+        order="desc",
+        offset=0,
+        limit=None,
+        **kwargs,
+    ):
         """Returns back a list of monitors in Iris Detect based on the provided filters.
 
         include_counts: bool: default False. includes counts for each monitor for new, watched, changed, and escalated
         domains
 
         datetime_counts_since: ISO 8601 datetime format: default None. Conditionally required if the include_counts
         parameter is set to True.
@@ -412,29 +765,53 @@
         offset: int: default 0. Offset for pagination
 
         limit: int: default 500. Limit for pagination. Restricted to maximum 100 if include_counts is set to True.
         """
 
         if include_counts:
             if not datetime_counts_since:
-                raise ValueError('Need to define datetime_counts_since when include_counts is True')
+                raise ValueError(
+                    "Need to define datetime_counts_since when include_counts is True"
+                )
             if isinstance(datetime_counts_since, datetime):
                 datetime_counts_since = str(datetime_counts_since.astimezone())
             elif isinstance(datetime_counts_since, str):
                 kwargs["datetime_counts_since"] = datetime_counts_since
             kwargs["include_counts"] = "true"
             kwargs["datetime_counts_since"] = datetime_counts_since
         if sort:
             kwargs["sort[]"] = sort
-        return self._results('iris-detect-monitors', '/v1/iris-detect/monitors/', order=order, offset=offset,
-                             limit=limit, items_path=('monitors',), response_path=(), **kwargs)
+        return self._results(
+            "iris-detect-monitors",
+            "/v1/iris-detect/monitors/",
+            order=order,
+            offset=offset,
+            limit=limit,
+            items_path=("monitors",),
+            response_path=(),
+            **kwargs,
+        )
 
-    def iris_detect_new_domains(self, monitor_id=None, tlds=None, risk_score_ranges=None,
-                                mx_exists=None, discovered_since=None, changed_since=None, search=None, sort=None,
-                                order=None, include_domain_data=False, offset=0, limit=None, preview=None, **kwargs):
+    def iris_detect_new_domains(
+        self,
+        monitor_id=None,
+        tlds=None,
+        risk_score_ranges=None,
+        mx_exists=None,
+        discovered_since=None,
+        changed_since=None,
+        search=None,
+        sort=None,
+        order=None,
+        include_domain_data=False,
+        offset=0,
+        limit=None,
+        preview=None,
+        **kwargs,
+    ):
         """Returns back a list of new domains in Iris Detect based on the provided filters.
 
         monitor_id: str: default None. Monitor ID from monitors response. Only used when requesting domains for a
         specific monitor.
 
         tlds: List[str]: default None. List of TLDs to filter domains by.
 
@@ -482,21 +859,47 @@
             kwargs["risk_score_ranges[]"] = risk_score_ranges
         if sort:
             kwargs["sort[]"] = sort
         if order is not None:
             kwargs["order"] = order
         if mx_exists is not None:
             kwargs["mx_exists"] = mx_exists
-        return self._results('iris-detect-new-domains', '/v1/iris-detect/domains/new/', monitor_id=monitor_id,
-                             search=search, include_domain_data=include_domain_data, preview=preview, offset=offset,
-                             limit=limit, items_path=('watchlist_domains',), response_path=(), **kwargs)
-
-    def iris_detect_watched_domains(self, monitor_id=None, escalation_types=None, tlds=None, risk_score_ranges=None,
-                                mx_exists=None, discovered_since=None, changed_since=None, escalated_since=None, search=None, sort=None,
-                                order=None, include_domain_data=False, offset=0, limit=None, preview=None, **kwargs):
+        return self._results(
+            "iris-detect-new-domains",
+            "/v1/iris-detect/domains/new/",
+            monitor_id=monitor_id,
+            search=search,
+            include_domain_data=include_domain_data,
+            preview=preview,
+            offset=offset,
+            limit=limit,
+            items_path=("watchlist_domains",),
+            response_path=(),
+            **kwargs,
+        )
+
+    def iris_detect_watched_domains(
+        self,
+        monitor_id=None,
+        escalation_types=None,
+        tlds=None,
+        risk_score_ranges=None,
+        mx_exists=None,
+        discovered_since=None,
+        changed_since=None,
+        escalated_since=None,
+        search=None,
+        sort=None,
+        order=None,
+        include_domain_data=False,
+        offset=0,
+        limit=None,
+        preview=None,
+        **kwargs,
+    ):
         """Returns back a list of watched domains in Iris Detect based on the provided filters.
 
         monitor_id: str: default None. Monitor ID from monitors response. Only used when requesting domains for a
         specific monitor.
 
         escalation_types: List[str]: default None. List of escalation types to filter domains by. Valid values are:
         ["blocked", "google_safe"]
@@ -558,46 +961,87 @@
             kwargs["risk_score_ranges[]"] = risk_score_ranges
         if sort:
             kwargs["sort[]"] = sort
         if order is not None:
             kwargs["order"] = order
         if mx_exists is not None:
             kwargs["mx_exists"] = mx_exists
-        return self._results('iris-detect-watched-domains', '/v1/iris-detect/domains/watched/', monitor_id=monitor_id,
-                             search=search, include_domain_data=include_domain_data, preview=preview, offset=offset,
-                             limit=limit, items_path=('watchlist_domains',), response_path=(), **kwargs)
+        return self._results(
+            "iris-detect-watched-domains",
+            "/v1/iris-detect/domains/watched/",
+            monitor_id=monitor_id,
+            search=search,
+            include_domain_data=include_domain_data,
+            preview=preview,
+            offset=offset,
+            limit=limit,
+            items_path=("watchlist_domains",),
+            response_path=(),
+            **kwargs,
+        )
 
-    def iris_detect_manage_watchlist_domains(self, watchlist_domain_ids, state, **kwargs):
+    def iris_detect_manage_watchlist_domains(
+        self, watchlist_domain_ids, state, **kwargs
+    ):
         """Changes the watch state of a list of domains by their Iris Detect domain ID.
 
         watchlist_domain_ids: List[str]: required. List of Iris Detect domain IDs to manage.
 
         state: str: required. Valid values are: ["watched", "ignored"]
         """
         if isinstance(watchlist_domain_ids, str):
-            watchlist_domain_ids = watchlist_domain_ids.split(',')
-        return self._results('iris-detect-manage-watchlist-domains', '/v1/iris-detect/domains/', state=state,
-                             watchlist_domain_ids=watchlist_domain_ids, items_path=('watchlist_domains',),
-                             response_path=(), **kwargs)
+            watchlist_domain_ids = watchlist_domain_ids.split(",")
+        return self._results(
+            "iris-detect-manage-watchlist-domains",
+            "/v1/iris-detect/domains/",
+            state=state,
+            watchlist_domain_ids=watchlist_domain_ids,
+            items_path=("watchlist_domains",),
+            response_path=(),
+            **kwargs,
+        )
 
-    def iris_detect_escalate_domains(self, watchlist_domain_ids, escalation_type, **kwargs):
+    def iris_detect_escalate_domains(
+        self, watchlist_domain_ids, escalation_type, **kwargs
+    ):
         """Changes the escalation type of a list of domains by their Iris Detect domain ID.
 
         watchlist_domain_ids: List[str]: required. List of Iris Detect domain IDs to escalate.
 
         escalation_type: str: required. Valid values are: ["blocked", "google_safe"]
         """
         kwargs["watchlist_domain_ids[]"] = watchlist_domain_ids
-        return self._results('iris-detect-escalate-domains', '/v1/iris-detect/escalations/',
-                             escalation_type=escalation_type, items_path=('escalations',),
-                             response_path=(), **kwargs)
-
-    def iris_detect_ignored_domains(self, monitor_id=None, escalation_types=None, tlds=None, risk_score_ranges=None,
-                                mx_exists=None, discovered_since=None, changed_since=None, escalated_since=None, search=None, sort=None,
-                                order=None, include_domain_data=False, offset=0, limit=None, preview=None, **kwargs):
+        return self._results(
+            "iris-detect-escalate-domains",
+            "/v1/iris-detect/escalations/",
+            escalation_type=escalation_type,
+            items_path=("escalations",),
+            response_path=(),
+            **kwargs,
+        )
+
+    def iris_detect_ignored_domains(
+        self,
+        monitor_id=None,
+        escalation_types=None,
+        tlds=None,
+        risk_score_ranges=None,
+        mx_exists=None,
+        discovered_since=None,
+        changed_since=None,
+        escalated_since=None,
+        search=None,
+        sort=None,
+        order=None,
+        include_domain_data=False,
+        offset=0,
+        limit=None,
+        preview=None,
+        **kwargs,
+    ):
         """Returns back a list of ignored domains in Iris Detect based on the provided filters.
 
         monitor_id: str: default None. Monitor ID from monitors response. Only used when requesting domains for a
         specific monitor.
 
         escalation_types: List[str]: default None. List of escalation types to filter domains by. Valid values are:
         ["blocked", "google_safe"]
@@ -659,10 +1103,20 @@
             kwargs["risk_score_ranges[]"] = risk_score_ranges
         if sort:
             kwargs["sort[]"] = sort
         if order is not None:
             kwargs["order"] = order
         if mx_exists is not None:
             kwargs["mx_exists"] = mx_exists
-        return self._results('iris-detect-ignored-domains', '/v1/iris-detect/domains/ignored/', monitor_id=monitor_id,
-                             search=search, include_domain_data=include_domain_data, preview=preview, offset=offset,
-                             limit=limit, items_path=('watchlist_domains',), response_path=(), **kwargs)
+        return self._results(
+            "iris-detect-ignored-domains",
+            "/v1/iris-detect/domains/ignored/",
+            monitor_id=monitor_id,
+            search=search,
+            include_domain_data=include_domain_data,
+            preview=preview,
+            offset=offset,
+            limit=limit,
+            items_path=("watchlist_domains",),
+            response_path=(),
+            **kwargs,
+        )
```

### Comparing `domaintools_api-1.0.1/domaintools/base_results.py` & `domaintools_api-2.0.0/domaintools/base_results.py`

 * *Files identical despite different names*

### Comparing `domaintools_api-1.0.1/domaintools/exceptions.py` & `domaintools_api-2.0.0/domaintools/exceptions.py`

 * *Files identical despite different names*

### Comparing `domaintools_api-1.0.1/domaintools/results.py` & `domaintools_api-2.0.0/domaintools/results.py`

 * *Files identical despite different names*

### Comparing `domaintools_api-1.0.1/domaintools/utils.py` & `domaintools_api-2.0.0/domaintools/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,33 @@
 from datetime import datetime
-import dateparser
+
+from typing import Optional
+
 import re
 
 
 def get_domain_age(create_date):
     """
     Finds how many days old a domain is given a start date.
     Args:
-        create_date: Date in the form of %Y-%m-%d'
+        create_date: Date in the form of %Y-%m-%d' or %Y%m%d'
 
     Returns: Number of days between now and the create_date.
     """
-    time_diff = datetime.now() - dateparser.parse(create_date, date_formats=['%Y-%m-%d', '%Y%m%d'])
+    try:
+        create_date = datetime.strptime(create_date, "%Y-%m-%d")
+    except ValueError:
+        try:
+            create_date = datetime.strptime(create_date, "%Y%m%d")
+        except ValueError:
+            raise ValueError(
+                "Invalid date format. Supported formats are %Y-%m-%d and %Y%m%d."
+            )
+
+    time_diff = datetime.now() - create_date
 
     return time_diff.days
 
 
 def get_threat_component(components, threat_type):
     """
     Gets a certain threat component out a list of components
@@ -85,36 +97,46 @@
     items_to_prune = []
     if isinstance(data_obj, dict) and len(data_obj):
         for k, v in data_obj.items():
             if isinstance(data_obj[k], dict) or isinstance(data_obj[k], list):
                 prune_data(data_obj[k])
             if not isinstance(v, int) and not v:
                 items_to_prune.append(k)
-            elif k == 'count' and v == 0:
+            elif k == "count" and v == 0:
                 items_to_prune.append(k)
         for k in items_to_prune:
             del data_obj[k]
     elif isinstance(data_obj, list) and len(data_obj):
         for index, item in enumerate(data_obj):
             prune_data(item)
             if not isinstance(item, int) and not item:
                 items_to_prune.append(index)
-        data_obj[:] = [item for index, item in enumerate(data_obj) if index not in items_to_prune and len(item)]
+        data_obj[:] = [
+            item
+            for index, item in enumerate(data_obj)
+            if index not in items_to_prune and len(item)
+        ]
 
 
 def find_emails(data_str):
     """Find and returns all emails"""
-    return set(re.findall(r'[\w\.-]+@[\w\.-]+', data_str))
+    return set(re.findall(r"[\w\.-]+@[\w\.-]+", data_str))
 
 
 def find_ips(data_str):
     """Find and returns all ipv4"""
-    ipv4s = set(re.findall(r'\b(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\b', data_str))
+    ipv4s = set(
+        re.findall(
+            r"\b(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\b",
+            data_str,
+        )
+    )
     return ipv4s
 
+
 def get_pivots(data_obj, name, return_data=None, count=0, pivot_threshold=500):
     """
     Does a deep dive through a data object to check count vs pivot threshold.
     Args:
         data_obj: Either a list or dict that needs to check pivot count
         name: pivot category name
         return_data: Holds data to return once we reach the end of the data_obj
@@ -147,7 +169,13 @@
                 elif isinstance(temp_data, tuple):
                     return_data.append([name[1:].upper().replace("_", " "), temp_data])
     count -= 1
     if count:
         return
     else:
         return return_data
+
+
+def convert_str_to_dateobj(
+    string_date: str, date_format: Optional[str] = "%Y-%m-%d"
+) -> datetime:
+    return datetime.strptime(string_date, date_format)
```

### Comparing `domaintools_api-1.0.1/domaintools_api.egg-info/PKG-INFO` & `domaintools_api-2.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,60 @@
 Metadata-Version: 2.1
-Name: domaintools-api
-Version: 1.0.1
+Name: domaintools_api
+Version: 2.0.0
 Summary: DomainTools Official Python API
-Home-page: https://github.com/domaintools/python_api
-Author: DomainTools
-Author-email: integrations@domaintools.com
-License: MIT
+Author-email: DomainTools <integrations@domaintools.com>
+License: The MIT License (MIT)
+        
+        Copyright (c) 2016 DomainTools
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/domaintools/python_api
 Keywords: Python,Python3
-Classifier: Development Status :: 6 - Mature
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: httpx
+Requires-Dist: rich
+Requires-Dist: typer
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: mock; extra == "test"
 
 ![domaintools](https://github.com/DomainTools/python_api/raw/main/artwork/logo.png)
 ===================
 
 [![PyPI version](https://badge.fury.io/py/domaintools_api.svg)](http://badge.fury.io/py/domaintools_api)
 [![CI Status](https://github.com/domaintools/python_api/workflows/Tests/badge.svg)](https://github.com/domaintools/python_api/actions)
 [![Coverage Status](https://coveralls.io/repos/github/DomainTools/python_api/badge.svg?branch=main)](https://coveralls.io/github/DomainTools/python_api?branch=main)
```

#### html2text {}

```diff
@@ -1,68 +1,85 @@
-Metadata-Version: 2.1 Name: domaintools-api Version: 1.0.1 Summary: DomainTools
-Official Python API Home-page: https://github.com/domaintools/python_api
-Author: DomainTools Author-email: integrations@domaintools.com License: MIT
-Keywords: Python,Python3 Classifier: Development Status :: 6 - Mature
-Classifier: Intended Audience :: Developers Classifier: Natural Language ::
-English Classifier: Environment :: Console Classifier: License :: OSI Approved
-:: MIT License Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3.6 Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Utilities Description-Content-Type: text/markdown License-
-File: LICENSE ![domaintools](https://github.com/DomainTools/python_api/raw/
-main/artwork/logo.png) =================== [![PyPI version](https://
-badge.fury.io/py/domaintools_api.svg)](http://badge.fury.io/py/domaintools_api)
-[![CI Status](https://github.com/domaintools/python_api/workflows/Tests/
-badge.svg)](https://github.com/domaintools/python_api/actions) [![Coverage
-Status](https://coveralls.io/repos/github/DomainTools/python_api/
-badge.svg?branch=main)](https://coveralls.io/github/DomainTools/
-python_api?branch=main) [![License](https://img.shields.io/github/license/
-mashape/apistatus.svg)](https://pypi.python.org/pypi/domaintools_api/
-) DomainTools Official Python API ![domaintools Example](https://github.com/
-DomainTools/python_api/raw/main/artwork/example.gif) The DomainTools Python API
-Wrapper provides an interface to work with our cybersecurity and related data
-tools provided by our Iris Investigateâ¢, Iris Enrichâ¢, and Iris Detectâ¢
-products. It is actively maintained and may be downloaded via _G_i_t_H_u_b or _P_y_P_I.
-See the included README file, the examples folder, and API documentation
-(https://app.swaggerhub.com/apis-docs/DomainToolsLLC/DomainTools_APIs/1.0#) for
-more info. Installing the DomainTools API =================== To install the
-API run ```bash pip install domaintools_api --upgrade ``` Ideally, within a
-virtual environment. Using the API =================== To start out create an
-instance of the API - passing in your credentials ```python from domaintools
-import API api = API(USER_NAME, KEY) ``` Every API endpoint is then exposed as
-a method on the API object, with any parameters that should be passed into that
-endpoint being passed in as method arguments: ```python api.iris_enrich
-('domaintools.com') ``` You can get an overview of every endpoint that you can
-interact with using the builtin help function: ```python help(api) ``` Or if
-you know the endpoint you want to use, you can get more information about it:
-```python help(api.iris_investigate) ``` If applicable, native Python looping
-can be used directly to loop through any results: ```python for result in
-api.iris_enrich('domaintools.com').response().get('results', {}): print(result
-['domain']) ``` You can also use a context manager to ensure processing on the
-results only occurs if the request is successfully made: ```python with
-api.iris_enrich('domaintools.com').response().get('results', {}) as results:
-print(results) ``` For API calls where a single item is expected to be
-returned, you can directly interact with the result: ```python profile =
-api.domain_profile('google.com') title = profile['website_data']['title'] ```
-For any API call where a single type of data is expected you can directly cast
-to the desired type: ```python float(api.reputation('google.com')) == 0.0 int
-(api.reputation('google.com')) == 0 ``` The entire structure returned from
-DomainTools can be retrieved by doing `.data()` while just the actionable
-response information can be retrieved by doing `.response()`: ```python
-api.iris_enrich('domaintools.com').data() == {'response': { ... }}
-api.iris_enrich('domaintools.com').response() == { ... } ``` You can directly
-get the html, xml, or json version of the response by calling `.(html|xml|json)
-()` These only work with non AsyncResults: ```python json = str
-(api.domain_search('google').json()) xml = str(api.domain_search('google').xml
-()) html = str(api.domain_search('google').html()) ``` If any API call is
-unsuccesfull, one of the exceptions defined in `domaintools.exceptions` will be
-raised: ```python-traceback api.domain_profile('notvalid').data() -------------
--------------------------------------------------------------
+Metadata-Version: 2.1 Name: domaintools_api Version: 2.0.0 Summary: DomainTools
+Official Python API Author-email: DomainTools
+domaintools.com> License: The MIT License (MIT) Copyright (c) 2016 DomainTools
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
+of the Software, and to permit persons to whom the Software is furnished to do
+so, subject to the following conditions: The above copyright notice and this
+permission notice shall be included in all copies or substantial portions of
+the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
+EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
+OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
+ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://github.com/
+domaintools/python_api Keywords: Python,Python3 Classifier: Development Status
+:: 5 - Production/Stable Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
+Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Topic :: Software Development :: Libraries Classifier: Topic :: Utilities
+Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
+LICENSE Requires-Dist: httpx Requires-Dist: rich Requires-Dist: typer Provides-
+Extra: test Requires-Dist: pytest; extra == "test" Requires-Dist: mock; extra
+== "test" ![domaintools](https://github.com/DomainTools/python_api/raw/main/
+artwork/logo.png) =================== [![PyPI version](https://badge.fury.io/
+py/domaintools_api.svg)](http://badge.fury.io/py/domaintools_api) [![CI Status]
+(https://github.com/domaintools/python_api/workflows/Tests/badge.svg)](https://
+github.com/domaintools/python_api/actions) [![Coverage Status](https://
+coveralls.io/repos/github/DomainTools/python_api/badge.svg?branch=main)](https:
+//coveralls.io/github/DomainTools/python_api?branch=main) [![License](https://
+img.shields.io/github/license/mashape/apistatus.svg)](https://pypi.python.org/
+pypi/domaintools_api/) DomainTools Official Python API ![domaintools Example]
+(https://github.com/DomainTools/python_api/raw/main/artwork/example.gif) The
+DomainTools Python API Wrapper provides an interface to work with our
+cybersecurity and related data tools provided by our Iris Investigateâ¢, Iris
+Enrichâ¢, and Iris Detectâ¢ products. It is actively maintained and may be
+downloaded via _G_i_t_H_u_b or _P_y_P_I. See the included README file, the examples
+folder, and API documentation (https://app.swaggerhub.com/apis-docs/
+DomainToolsLLC/DomainTools_APIs/1.0#) for more info. Installing the DomainTools
+API =================== To install the API run ```bash pip install
+domaintools_api --upgrade ``` Ideally, within a virtual environment. Using the
+API =================== To start out create an instance of the API - passing in
+your credentials ```python from domaintools import API api = API(USER_NAME,
+KEY) ``` Every API endpoint is then exposed as a method on the API object, with
+any parameters that should be passed into that endpoint being passed in as
+method arguments: ```python api.iris_enrich('domaintools.com') ``` You can get
+an overview of every endpoint that you can interact with using the builtin help
+function: ```python help(api) ``` Or if you know the endpoint you want to use,
+you can get more information about it: ```python help(api.iris_investigate) ```
+If applicable, native Python looping can be used directly to loop through any
+results: ```python for result in api.iris_enrich('domaintools.com').response
+().get('results', {}): print(result['domain']) ``` You can also use a context
+manager to ensure processing on the results only occurs if the request is
+successfully made: ```python with api.iris_enrich('domaintools.com').response
+().get('results', {}) as results: print(results) ``` For API calls where a
+single item is expected to be returned, you can directly interact with the
+result: ```python profile = api.domain_profile('google.com') title = profile
+['website_data']['title'] ``` For any API call where a single type of data is
+expected you can directly cast to the desired type: ```python float
+(api.reputation('google.com')) == 0.0 int(api.reputation('google.com')) == 0
+``` The entire structure returned from DomainTools can be retrieved by doing
+`.data()` while just the actionable response information can be retrieved by
+doing `.response()`: ```python api.iris_enrich('domaintools.com').data() ==
+{'response': { ... }} api.iris_enrich('domaintools.com').response() == { ... }
+``` You can directly get the html, xml, or json version of the response by
+calling `.(html|xml|json)()` These only work with non AsyncResults: ```python
+json = str(api.domain_search('google').json()) xml = str(api.domain_search
+('google').xml()) html = str(api.domain_search('google').html()) ``` If any API
+call is unsuccesfull, one of the exceptions defined in `domaintools.exceptions`
+will be raised: ```python-traceback api.domain_profile('notvalid').data() -----
+---------------------------------------------------------------------
 - BadRequestException Traceback (most recent call last) in () ----> 1
 api.domain_profile('google').data() /home/tcrosley/projects/external/
 python_api/venv/lib/python3.5/site-packages/domaintools-0.0.1-py3.5.egg/
 domaintools/base_results.py in data(self) 25 self.api._request_session =
 Session() 26 results = self.api._request_session.get(self.url,
 params=self.kwargs) ---> 27 self.status = results.status_code 28 if
 self.kwargs.get('format', 'json') == 'json': 29 self._data = results.json() /
```

### Comparing `domaintools_api-1.0.1/domaintools_async/__init__.py` & `domaintools_api-2.0.0/domaintools_async/__init__.py`

 * *Files identical despite different names*

