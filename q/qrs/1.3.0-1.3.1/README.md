# Comparing `tmp/qrs-1.3.0.tar.gz` & `tmp/qrs-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qrs-1.3.0.tar", last modified: Wed May 15 00:04:03 2024, max compression
+gzip compressed data, was "qrs-1.3.1.tar", last modified: Thu May 30 23:08:53 2024, max compression
```

## Comparing `qrs-1.3.0.tar` & `qrs-1.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:04:03.216973 qrs-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-15 00:03:57.000000 qrs-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-05-15 00:04:03.216973 qrs-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-05-15 00:03:57.000000 qrs-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:04:03.208973 qrs-1.3.0/qrs/
--rw-r--r--   0 runner    (1001) docker     (127)    15389 2024-05-15 00:03:57.000000 qrs-1.3.0/qrs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-15 00:03:57.000000 qrs-1.3.0/qrs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)  2905592 2024-05-15 00:03:57.000000 qrs-1.3.0/qrs/wordlist.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:04:03.216973 qrs-1.3.0/qrs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-05-15 00:04:03.000000 qrs-1.3.0/qrs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-15 00:04:03.000000 qrs-1.3.0/qrs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 00:04:03.000000 qrs-1.3.0/qrs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 00:04:03.000000 qrs-1.3.0/qrs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 00:04:03.000000 qrs-1.3.0/qrs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 00:04:03.000000 qrs-1.3.0/qrs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 00:04:03.000000 qrs-1.3.0/qrs.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 00:04:03.216973 qrs-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-15 00:03:57.000000 qrs-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:08:53.027132 qrs-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-30 23:08:44.000000 qrs-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-05-30 23:08:53.027132 qrs-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6361 2024-05-30 23:08:44.000000 qrs-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:08:53.019132 qrs-1.3.1/qrs/
+-rw-r--r--   0 runner    (1001) docker     (127)    15526 2024-05-30 23:08:44.000000 qrs-1.3.1/qrs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-30 23:08:44.000000 qrs-1.3.1/qrs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2905592 2024-05-30 23:08:44.000000 qrs-1.3.1/qrs/wordlist.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:08:53.027132 qrs-1.3.1/qrs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-05-30 23:08:53.000000 qrs-1.3.1/qrs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-30 23:08:53.000000 qrs-1.3.1/qrs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 23:08:53.000000 qrs-1.3.1/qrs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-30 23:08:53.000000 qrs-1.3.1/qrs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 23:08:53.000000 qrs-1.3.1/qrs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-30 23:08:53.000000 qrs-1.3.1/qrs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 23:08:53.000000 qrs-1.3.1/qrs.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 23:08:53.027132 qrs-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-30 23:08:44.000000 qrs-1.3.1/setup.py
```

### Comparing `qrs-1.3.0/LICENSE` & `qrs-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qrs-1.3.0/PKG-INFO` & `qrs-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qrs
-Version: 1.3.0
+Version: 1.3.1
 Summary: Provides word game-related tools that can be configured with custom settings,
 Home-page: https://github.com/silvncr/qrs
 Author: silvncr
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -13,34 +13,34 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: Topic :: Games/Entertainment :: Puzzle Games
-Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jarguments==0.1.0
 
 <!-- omit from toc -->
 # qrs
 
 tool for *Quarrel* (and other word games)
 
-![downloads](https://img.shields.io/pypi/dm/qrs)
-![status](https://img.shields.io/github/actions/workflow/status/silvncr/qrs/python-publish.yml)
 ![version](https://img.shields.io/pypi/v/qrs)
+![status](https://img.shields.io/github/actions/workflow/status/silvncr/qrs/python-publish.yml)
+![downloads](https://img.shields.io/pypi/dm/qrs)
 
 ## Summary
 
 Provides word game-related tools that can be configured with custom settings, letter scores, and wordlists.
 
-> Supports Python 3.8 and above. Tested on Windows 10.
+- :snake: Supports Python 3.8 and above. Tested on Windows 10.
+- :star: Show your support by leaving a star!
 
 ## Contents
 
 - [Summary](#summary)
 - [Contents](#contents)
 - [The qrs library](#the-qrs-library)
 - [Direct execution](#direct-execution)
```

### Comparing `qrs-1.3.0/README.md` & `qrs-1.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 <!-- omit from toc -->
 # qrs
 
 tool for *Quarrel* (and other word games)
 
-![downloads](https://img.shields.io/pypi/dm/qrs)
-![status](https://img.shields.io/github/actions/workflow/status/silvncr/qrs/python-publish.yml)
 ![version](https://img.shields.io/pypi/v/qrs)
+![status](https://img.shields.io/github/actions/workflow/status/silvncr/qrs/python-publish.yml)
+![downloads](https://img.shields.io/pypi/dm/qrs)
 
 ## Summary
 
 Provides word game-related tools that can be configured with custom settings, letter scores, and wordlists.
 
-> Supports Python 3.8 and above. Tested on Windows 10.
+- :snake: Supports Python 3.8 and above. Tested on Windows 10.
+- :star: Show your support by leaving a star!
 
 ## Contents
 
 - [Summary](#summary)
 - [Contents](#contents)
 - [The qrs library](#the-qrs-library)
 - [Direct execution](#direct-execution)
```

### Comparing `qrs-1.3.0/qrs/__init__.py` & `qrs-1.3.1/qrs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,32 +14,32 @@
 from typing import Any, Self
 
 # metadata
 __author__ = 'silvncr'
 __license__ = 'MIT'
 __module_name__ = 'qrs'
 __python_version__ = '3.8'
-__version__ = '1.3.0'
+__version__ = '1.3.1'
 
 
 # get full wordlist from file
 with open(
 	os_path.join(
 		os_path.dirname(__file__),
 		'wordlist.txt',
 	),
 ) as f:
-	wordlist_full = sorted(
+	wordlist_full: list[str] = sorted(
 		f.read().splitlines(),
 	)
-max_length_full = max(len(word) for word in wordlist_full)
+max_length_full: int = max(len(word) for word in wordlist_full)
 
 
 # command line arguments; (arg, sarg, type, default, multiple, help)
-qrs_kwargs = [
+qrs_kwargs: list[tuple] = [
 	('debug', 'd', bool, False, ..., 'Whether to display debug information'),
 	('doubles', 'b', bool, False, ..., 'Whether to show longer, tied words'),
 	('exclude', 'e', str, [], True, 'List of words to exclude'),
 	('game', 'g', str, 'quarrel', None, 'Scoring system to use'),
 	('include', 'i', str, [], True, 'List of words to include'),
 	('lower', 'l', bool, False, ..., 'Whether output should be lowercase'),
 	('max', 'm', int, max_length_full, None, 'Maximum length of words'),
@@ -276,15 +276,16 @@
 		Args:
 		----
 			key: `str`
 				The setting to get the value of.
 
 		Returns:
 		-------
-			The value of the given setting.
+			The value of the given setting. Can be any type, as defined in
+			`qrs_kwargs`.
 		'''
 
 		# return setting, or raise error
 		if key in self.settings:
 			return self.settings[key]
 		msg = f'{key} not found in settings'
 		raise KeyError(msg)
@@ -311,15 +312,15 @@
 			.replace('  ', '\t')
 
 	# solve function
 	def solve(
 		self: Self,
 		query: str,
 		/,
-	) -> tuple[dict[int, list[str]], bool]:
+	) -> tuple[dict[int, tuple[list[str], int]], bool]:
 		'''
 		Finds all possible words that can be formed from the given query
 		string using the set wordlist.
 
 		Args:
 		----
 			query: `str`
@@ -331,28 +332,28 @@
 			by length, and a boolean indicating whether an anagram was found.
 		'''
 
 		# build query
 		query = build_query(query, repeat_letters=not self['repeats'])
 
 		# initialise output object
-		scores = {}
+		scores: dict[int, tuple[list[str], int]] = {}
 
 		# prepare debug output
 		if self['debug']:
 			print('')
 
 		# iterate through possible word lengths
 		for len_iter in range(
 			max(2, min([2, self['min']])),
 			(self['max'] if self['repeats'] else len(query)) + 1,
 		)[::-1]:
 			scores = {
 				**scores,
-				len_iter: [[], 0],
+				len_iter: ([], 0),
 			}
 
 			# iterate through wordlist
 			for word in self.scores:
 				query_iter, word_iter = deepcopy(query), deepcopy(word)
 				word_fits = False
 
@@ -426,15 +427,15 @@
 						print(f'\t[{word}] fits for [{len_iter}]')
 						if not word_iter.strip() and not query_iter.strip() \
 							and len(word) == len(query):
 							print(f'\tanagram found: [{word}]')
 
 					# update score
 					if not self['noscores']:
-						scores[len_iter][1] = self.scores[
+						scores[len_iter] = scores[len_iter][0], self.scores[
 							scores[len_iter][0][0]
 						]
 
 			# debug info
 			if self['debug']:
 				print(f'output for [{len_iter}]: {scores[len_iter][0]}')
 
@@ -501,24 +502,24 @@
 		# build query
 		query = build_query(query, repeat_letters=not self['repeats'])
 
 		# get solved object and anagram status
 		scores, anagram_found = self.solve(query)
 
 		# prepare anagram message
-		anagram_found = '' \
+		anagram_msg = '' \
 			if anagram_found \
 			else '  \t warning: anagram not found\n\n'
 
 		# return output string
 		return str(
 			f'\n  \t--- query: {query} ({len(query)} letters'
 			+ (' + repeats' if self['repeats'] else '') + ') ---\n\n' + (
 				(
-					anagram_found + '\n\n'.join(
+					anagram_msg + '\n\n'.join(
 						f'\t{key} letters'
 						+ (
 							''
 							if self['noscores']
 							else f' - {scores[key][1]} points'
 						) + '\n\t ' + ', '.join(
 							sorted(
```

### Comparing `qrs-1.3.0/qrs/wordlist.txt` & `qrs-1.3.1/qrs/wordlist.txt`

 * *Files identical despite different names*

### Comparing `qrs-1.3.0/qrs.egg-info/PKG-INFO` & `qrs-1.3.1/qrs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qrs
-Version: 1.3.0
+Version: 1.3.1
 Summary: Provides word game-related tools that can be configured with custom settings,
 Home-page: https://github.com/silvncr/qrs
 Author: silvncr
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -13,34 +13,34 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: Topic :: Games/Entertainment :: Puzzle Games
-Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jarguments==0.1.0
 
 <!-- omit from toc -->
 # qrs
 
 tool for *Quarrel* (and other word games)
 
-![downloads](https://img.shields.io/pypi/dm/qrs)
-![status](https://img.shields.io/github/actions/workflow/status/silvncr/qrs/python-publish.yml)
 ![version](https://img.shields.io/pypi/v/qrs)
+![status](https://img.shields.io/github/actions/workflow/status/silvncr/qrs/python-publish.yml)
+![downloads](https://img.shields.io/pypi/dm/qrs)
 
 ## Summary
 
 Provides word game-related tools that can be configured with custom settings, letter scores, and wordlists.
 
-> Supports Python 3.8 and above. Tested on Windows 10.
+- :snake: Supports Python 3.8 and above. Tested on Windows 10.
+- :star: Show your support by leaving a star!
 
 ## Contents
 
 - [Summary](#summary)
 - [Contents](#contents)
 - [The qrs library](#the-qrs-library)
 - [Direct execution](#direct-execution)
```

### Comparing `qrs-1.3.0/setup.py` & `qrs-1.3.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,10 +40,9 @@
 		'Natural Language :: English',
 		'Operating System :: OS Independent',
 		'Programming Language :: Python :: 3.8',
 		'Programming Language :: Python :: 3',
 		'Programming Language :: Python',
 		'Topic :: Games/Entertainment :: Board Games',
 		'Topic :: Games/Entertainment :: Puzzle Games',
-		'Typing :: Typed',
 	],
 )
```

