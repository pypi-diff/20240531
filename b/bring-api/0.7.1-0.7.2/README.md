# Comparing `tmp/bring_api-0.7.1.tar.gz` & `tmp/bring_api-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bring_api-0.7.1.tar", last modified: Mon Apr 15 10:52:57 2024, max compression
+gzip compressed data, was "bring_api-0.7.2.tar", last modified: Fri May 31 21:22:09 2024, max compression
```

## Comparing `bring_api-0.7.1.tar` & `bring_api-0.7.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:52:57.540104 bring_api-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-04-15 10:52:52.000000 bring_api-0.7.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-15 10:52:52.000000 bring_api-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13501 2024-04-15 10:52:57.540104 bring_api-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8792 2024-04-15 10:52:52.000000 bring_api-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:52:57.536104 bring_api-0.7.1/bring_api/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54803 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/bring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:52:57.540104 bring_api-0.7.1/bring_api/locales/
--rw-r--r--   0 runner    (1001) docker     (127)    10923 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.de-AT.json
--rw-r--r--   0 runner    (1001) docker     (127)    12631 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.de-CH.json
--rw-r--r--   0 runner    (1001) docker     (127)    12661 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.de-DE.json
--rw-r--r--   0 runner    (1001) docker     (127)    11010 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.en-AU.json
--rw-r--r--   0 runner    (1001) docker     (127)    10896 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.en-CA.json
--rw-r--r--   0 runner    (1001) docker     (127)    10966 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.en-GB.json
--rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.en-US.json
--rw-r--r--   0 runner    (1001) docker     (127)    11243 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.es-ES.json
--rw-r--r--   0 runner    (1001) docker     (127)    11310 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.fr-CH.json
--rw-r--r--   0 runner    (1001) docker     (127)     9681 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.fr-FR.json
--rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.hu-HU.json
--rw-r--r--   0 runner    (1001) docker     (127)    11323 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.it-CH.json
--rw-r--r--   0 runner    (1001) docker     (127)     9255 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.it-IT.json
--rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.nb-NO.json
--rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.nl-NL.json
--rw-r--r--   0 runner    (1001) docker     (127)    10703 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.pl-PL.json
--rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.pt-BR.json
--rw-r--r--   0 runner    (1001) docker     (127)    14472 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.ru-RU.json
--rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.sv-SE.json
--rw-r--r--   0 runner    (1001) docker     (127)    10386 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/locales/articles.tr-TR.json
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-15 10:52:52.000000 bring_api-0.7.1/bring_api/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:52:57.540104 bring_api-0.7.1/bring_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13501 2024-04-15 10:52:57.000000 bring_api-0.7.1/bring_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-15 10:52:57.000000 bring_api-0.7.1/bring_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 10:52:57.000000 bring_api-0.7.1/bring_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 10:52:57.000000 bring_api-0.7.1/bring_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 10:52:57.000000 bring_api-0.7.1/bring_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-15 10:52:52.000000 bring_api-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-15 10:52:57.540104 bring_api-0.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:52:57.540104 bring_api-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    45864 2024-04-15 10:52:52.000000 bring_api-0.7.1/tests/test_bring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:22:09.868490 bring_api-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-31 21:22:04.000000 bring_api-0.7.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-31 21:22:04.000000 bring_api-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13543 2024-05-31 21:22:09.868490 bring_api-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8792 2024-05-31 21:22:04.000000 bring_api-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:22:09.860490 bring_api-0.7.2/bring_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-31 21:22:04.000000 bring_api-0.7.2/bring_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55677 2024-05-31 21:22:04.000000 bring_api-0.7.2/bring_api/bring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-31 21:22:04.000000 bring_api-0.7.2/bring_api/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-31 21:22:04.000000 bring_api-0.7.2/bring_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:22:09.864490 bring_api-0.7.2/bring_api/locales/
+-rw-r--r--   0 runner    (1001) docker     (127)    10923 2024-05-31 21:22:04.000000 bring_api-0.7.2/bring_api/locales/articles.de-AT.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12631 2024-05-31 21:22:04.000000 bring_api-0.7.2/bring_api/locales/articles.de-CH.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12661 2024-05-31 21:22:04.000000 bring_api-0.7.2/bring_api/locales/articles.de-DE.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11010 2024-05-31 21:22:04.000000 bring_api-0.7.2/bring_api/locales/articles.en-AU.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10896 2024-05-31 21:22:04.000000 bring_api-0.7.2/bring_api/locales/articles.en-CA.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10966 2024-05-31 21:22:04.000000 bring_api-0.7.2/bring_api/locales/articles.en-GB.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-05-31 21:22:04.000000 bring_api-0.7.2/bring_api/locales/articles.en-US.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11243 2024-05-31 21:22:04.000000 bring_api-0.7.2/bring_api/locales/articles.es-ES.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11310 2024-05-31 21:22:04.000000 bring_api-0.7.2/bring_api/locales/articles.fr-CH.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9681 2024-05-31 21:22:04.000000 bring_api-0.7.2/bring_api/locales/articles.fr-FR.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-05-31 21:22:04.000000 bring_api-0.7.2/bring_api/locales/articles.hu-HU.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11323 2024-05-31 21:22:04.000000 bring_api-0.7.2/bring_api/locales/articles.it-CH.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9255 2024-05-31 21:22:04.000000 bring_api-0.7.2/bring_api/locales/articles.it-IT.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-05-31 21:22:04.000000 bring_api-0.7.2/bring_api/locales/articles.nb-NO.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-05-31 21:22:04.000000 bring_api-0.7.2/bring_api/locales/articles.nl-NL.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10703 2024-05-31 21:22:04.000000 bring_api-0.7.2/bring_api/locales/articles.pl-PL.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-05-31 21:22:04.000000 bring_api-0.7.2/bring_api/locales/articles.pt-BR.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14472 2024-05-31 21:22:04.000000 bring_api-0.7.2/bring_api/locales/articles.ru-RU.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-05-31 21:22:04.000000 bring_api-0.7.2/bring_api/locales/articles.sv-SE.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10386 2024-05-31 21:22:04.000000 bring_api-0.7.2/bring_api/locales/articles.tr-TR.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-31 21:22:04.000000 bring_api-0.7.2/bring_api/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:22:09.868490 bring_api-0.7.2/bring_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13543 2024-05-31 21:22:09.000000 bring_api-0.7.2/bring_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-31 21:22:09.000000 bring_api-0.7.2/bring_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 21:22:09.000000 bring_api-0.7.2/bring_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-31 21:22:09.000000 bring_api-0.7.2/bring_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-31 21:22:09.000000 bring_api-0.7.2/bring_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-05-31 21:22:04.000000 bring_api-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-31 21:22:09.868490 bring_api-0.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:22:09.864490 bring_api-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    45864 2024-05-31 21:22:04.000000 bring_api-0.7.2/tests/test_bring.py
```

### Comparing `bring_api-0.7.1/CHANGELOG.md` & `bring_api-0.7.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # CHANGELOG
 
+# 0.7.2
+
+* fix bug in debug log message.
+
 # 0.7.1
 
 * Fix get_list method not returning uuid and status from JSON response
 * Log to debug instead of error where exceptions are already raised.
 * Add raw server response to debug log messages.
 * Update docstrings
```

### Comparing `bring_api-0.7.1/LICENSE` & `bring_api-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bring_api-0.7.1/PKG-INFO` & `bring_api-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bring-api
-Version: 0.7.1
+Version: 0.7.2
 Summary: Unofficial package to access Bring! shopping lists API.
 Home-page: https://github.com/miaucl/python-bring-api
 Author: Cyrill Raccaud
 Author-email: cyrill.raccaud+pypi@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -261,14 +261,18 @@
 Following VSCode integrations may be helpful:
 
 * [ruff](https://marketplace.visualstudio.com/items?itemName=charliermarsh.ruff)
 * [mypy](https://marketplace.visualstudio.com/items?itemName=matangover.mypy)
 
 # CHANGELOG
 
+# 0.7.2
+
+* fix bug in debug log message.
+
 # 0.7.1
 
 * Fix get_list method not returning uuid and status from JSON response
 * Log to debug instead of error where exceptions are already raised.
 * Add raw server response to debug log messages.
 * Update docstrings
```

### Comparing `bring_api-0.7.1/README.md` & `bring_api-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `bring_api-0.7.1/bring_api/bring.py` & `bring_api-0.7.2/bring_api/bring.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,15 +104,22 @@
 
         """
         user_data = {"email": self.mail, "password": self.password}
 
         try:
             url = f"{self.url}v2/bringauth"
             async with self._session.post(url, data=user_data) as r:
-                _LOGGER.debug("Response from %s [%s]: %s", url, r.status, r.text)
+                _LOGGER.debug(
+                    "Response from %s [%s]: %s",
+                    url,
+                    r.status,
+                    await r.text()
+                    if r.status != 200
+                    else "",  # do not log response on success, as it contains sensible data
+                )
 
                 if r.status == HTTPStatus.UNAUTHORIZED:
                     try:
                         errmsg = await r.json()
                     except JSONDecodeError as e:
                         _LOGGER.debug(
                             "Exception: Cannot parse login request response:\n %s",
@@ -195,15 +202,17 @@
         BringAuthException
             If the request fails due to invalid or expired authorization token.
 
         """
         try:
             url = f"{self.url}bringusers/{self.uuid}/lists"
             async with self._session.get(url, headers=self.headers) as r:
-                _LOGGER.debug("Response from %s [%s]: %s", url, r.status, r.text)
+                _LOGGER.debug(
+                    "Response from %s [%s]: %s", url, r.status, await r.text()
+                )
 
                 if r.status == HTTPStatus.UNAUTHORIZED:
                     try:
                         errmsg = await r.json()
                     except JSONDecodeError as e:
                         _LOGGER.debug(
                             "Exception: Cannot parse request response:\n %s",
@@ -274,15 +283,17 @@
         BringAuthException
             If the request fails due to invalid or expired authorization token.
 
         """
         try:
             url = f"{self.url}v2/bringlists/{list_uuid}"
             async with self._session.get(url, headers=self.headers) as r:
-                _LOGGER.debug("Response from %s [%s]: %s", url, r.status, r.text)
+                _LOGGER.debug(
+                    "Response from %s [%s]: %s", url, r.status, await r.text()
+                )
 
                 if r.status == HTTPStatus.UNAUTHORIZED:
                     try:
                         errmsg = await r.json()
                     except JSONDecodeError as e:
                         _LOGGER.debug(
                             "Exception: Cannot parse request response:\n %s",
@@ -375,15 +386,17 @@
         BringAuthException
             If the request fails due to invalid or expired authorization token.
 
         """
         try:
             url = f"{self.url}bringlists/{list_uuid}/details"
             async with self._session.get(url, headers=self.headers) as r:
-                _LOGGER.debug("Response from %s [%s]: %s", url, r.status, r.text)
+                _LOGGER.debug(
+                    "Response from %s [%s]: %s", url, r.status, await r.text()
+                )
 
                 if r.status == HTTPStatus.UNAUTHORIZED:
                     try:
                         errmsg = await r.json()
                     except JSONDecodeError as e:
                         _LOGGER.debug(
                             "Exception: Cannot parse request response:\n %s",
@@ -717,15 +730,17 @@
 
             json_data["arguments"] = [item_name]
         try:
             url = f"{self.url}v2/bringnotifications/lists/{list_uuid}"
             async with self._session.post(
                 url, headers=self.headers, json=json_data
             ) as r:
-                _LOGGER.debug("Response from %s [%s]: %s", url, r.status, r.text)
+                _LOGGER.debug(
+                    "Response from %s [%s]: %s", url, r.status, await r.text()
+                )
 
                 if r.status == HTTPStatus.UNAUTHORIZED:
                     try:
                         errmsg = await r.json()
                     except JSONDecodeError as e:
                         _LOGGER.debug(
                             "Exception: Cannot parse request response:\n %s",
@@ -798,15 +813,17 @@
             raise ValueError("Argument mail missing.")
 
         params = {"email": mail}
 
         try:
             url = f"{self.url}bringusers"
             async with self._session.get(url, headers=self.headers, params=params) as r:
-                _LOGGER.debug("Response from %s [%s]: %s", url, r.status, r.text)
+                _LOGGER.debug(
+                    "Response from %s [%s]: %s", url, r.status, await r.text()
+                )
 
                 if r.status == HTTPStatus.NOT_FOUND:
                     raise BringUserUnknownException(f"User {mail} does not exist.")
 
                 r.raise_for_status()
 
         except asyncio.TimeoutError as e:
@@ -1046,15 +1063,17 @@
         BringAuthException
             If the request fails due to invalid or expired authorization token.
 
         """
         try:
             url = f"{self.url}bringusersettings/{self.uuid}"
             async with self._session.get(url, headers=self.headers) as r:
-                _LOGGER.debug("Response from %s [%s]: %s", url, r.status, r.text)
+                _LOGGER.debug(
+                    "Response from %s [%s]: %s", url, r.status, await r.text()
+                )
 
                 if r.status == HTTPStatus.UNAUTHORIZED:
                     try:
                         errmsg = await r.json()
                     except JSONDecodeError as e:
                         _LOGGER.debug(
                             "Exception: Cannot parse request response:\n %s",
@@ -1221,15 +1240,17 @@
         BringAuthException
             If the request fails due to invalid or expired authorization token.
 
         """
         try:
             url = f"{self.url}v2/bringusers/{self.uuid}"
             async with self._session.get(url, headers=self.headers) as r:
-                _LOGGER.debug("Response from %s [%s]: %s", url, r.status, r.text)
+                _LOGGER.debug(
+                    "Response from %s [%s]: %s", url, r.status, await r.text()
+                )
 
                 if r.status == HTTPStatus.UNAUTHORIZED:
                     try:
                         errmsg = await r.json()
                     except JSONDecodeError as e:
                         _LOGGER.debug(
                             "Exception: Cannot parse request response:\n %s",
@@ -1346,15 +1367,17 @@
         }
 
         try:
             url = f"{self.url}v2/bringlists/{list_uuid}/items"
             async with self._session.put(
                 url, headers=self.headers, json=json_data
             ) as r:
-                _LOGGER.debug("Response from %s [%s]: %s", url, r.status, r.text)
+                _LOGGER.debug(
+                    "Response from %s [%s]: %s", url, r.status, await r.text()
+                )
 
                 if r.status == HTTPStatus.UNAUTHORIZED:
                     try:
                         errmsg = await r.json()
                     except JSONDecodeError as e:
                         _LOGGER.debug(
                             "Exception: Cannot parse request response:\n %s",
@@ -1421,15 +1444,22 @@
 
         user_data = {"grant_type": "refresh_token", "refresh_token": refresh_token}
         try:
             url = f"{self.url}v2/bringauth/token"
             async with self._session.post(
                 url, headers=self.headers, data=user_data
             ) as r:
-                _LOGGER.debug("Response from %s [%s]: %s", url, r.status, r.text)
+                _LOGGER.debug(
+                    "Response from %s [%s]: %s",
+                    url,
+                    r.status,
+                    await r.text()
+                    if r.status != 200
+                    else "",  # do not log response on success, as it contains sensible data
+                )
                 if r.status == HTTPStatus.UNAUTHORIZED:
                     try:
                         errmsg = await r.json()
                     except JSONDecodeError as e:
                         _LOGGER.debug(
                             "Exception: Cannot parse token request response:\n %s",
                             traceback.format_exc(),
```

### Comparing `bring_api-0.7.1/bring_api/const.py` & `bring_api-0.7.2/bring_api/const.py`

 * *Files identical despite different names*

### Comparing `bring_api-0.7.1/bring_api/exceptions.py` & `bring_api-0.7.2/bring_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `bring_api-0.7.1/bring_api/locales/articles.de-AT.json` & `bring_api-0.7.2/bring_api/locales/articles.de-AT.json`

 * *Files identical despite different names*

### Comparing `bring_api-0.7.1/bring_api/locales/articles.de-CH.json` & `bring_api-0.7.2/bring_api/locales/articles.de-CH.json`

 * *Files identical despite different names*

### Comparing `bring_api-0.7.1/bring_api/locales/articles.de-DE.json` & `bring_api-0.7.2/bring_api/locales/articles.de-DE.json`

 * *Files identical despite different names*

### Comparing `bring_api-0.7.1/bring_api/locales/articles.en-AU.json` & `bring_api-0.7.2/bring_api/locales/articles.en-AU.json`

 * *Files identical despite different names*

### Comparing `bring_api-0.7.1/bring_api/locales/articles.en-CA.json` & `bring_api-0.7.2/bring_api/locales/articles.en-CA.json`

 * *Files identical despite different names*

### Comparing `bring_api-0.7.1/bring_api/locales/articles.en-GB.json` & `bring_api-0.7.2/bring_api/locales/articles.en-GB.json`

 * *Files identical despite different names*

### Comparing `bring_api-0.7.1/bring_api/locales/articles.en-US.json` & `bring_api-0.7.2/bring_api/locales/articles.en-US.json`

 * *Files identical despite different names*

### Comparing `bring_api-0.7.1/bring_api/locales/articles.es-ES.json` & `bring_api-0.7.2/bring_api/locales/articles.es-ES.json`

 * *Files identical despite different names*

### Comparing `bring_api-0.7.1/bring_api/locales/articles.fr-CH.json` & `bring_api-0.7.2/bring_api/locales/articles.fr-CH.json`

 * *Files identical despite different names*

### Comparing `bring_api-0.7.1/bring_api/locales/articles.fr-FR.json` & `bring_api-0.7.2/bring_api/locales/articles.fr-FR.json`

 * *Files identical despite different names*

### Comparing `bring_api-0.7.1/bring_api/locales/articles.hu-HU.json` & `bring_api-0.7.2/bring_api/locales/articles.hu-HU.json`

 * *Files identical despite different names*

### Comparing `bring_api-0.7.1/bring_api/locales/articles.it-CH.json` & `bring_api-0.7.2/bring_api/locales/articles.it-CH.json`

 * *Files identical despite different names*

### Comparing `bring_api-0.7.1/bring_api/locales/articles.it-IT.json` & `bring_api-0.7.2/bring_api/locales/articles.it-IT.json`

 * *Files identical despite different names*

### Comparing `bring_api-0.7.1/bring_api/locales/articles.nb-NO.json` & `bring_api-0.7.2/bring_api/locales/articles.nb-NO.json`

 * *Files identical despite different names*

### Comparing `bring_api-0.7.1/bring_api/locales/articles.nl-NL.json` & `bring_api-0.7.2/bring_api/locales/articles.nl-NL.json`

 * *Files identical despite different names*

### Comparing `bring_api-0.7.1/bring_api/locales/articles.pl-PL.json` & `bring_api-0.7.2/bring_api/locales/articles.pl-PL.json`

 * *Files identical despite different names*

### Comparing `bring_api-0.7.1/bring_api/locales/articles.pt-BR.json` & `bring_api-0.7.2/bring_api/locales/articles.pt-BR.json`

 * *Files identical despite different names*

### Comparing `bring_api-0.7.1/bring_api/locales/articles.ru-RU.json` & `bring_api-0.7.2/bring_api/locales/articles.ru-RU.json`

 * *Files identical despite different names*

### Comparing `bring_api-0.7.1/bring_api/locales/articles.sv-SE.json` & `bring_api-0.7.2/bring_api/locales/articles.sv-SE.json`

 * *Files identical despite different names*

### Comparing `bring_api-0.7.1/bring_api/locales/articles.tr-TR.json` & `bring_api-0.7.2/bring_api/locales/articles.tr-TR.json`

 * *Files identical despite different names*

### Comparing `bring_api-0.7.1/bring_api/types.py` & `bring_api-0.7.2/bring_api/types.py`

 * *Files identical despite different names*

### Comparing `bring_api-0.7.1/bring_api.egg-info/PKG-INFO` & `bring_api-0.7.2/bring_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bring-api
-Version: 0.7.1
+Version: 0.7.2
 Summary: Unofficial package to access Bring! shopping lists API.
 Home-page: https://github.com/miaucl/python-bring-api
 Author: Cyrill Raccaud
 Author-email: cyrill.raccaud+pypi@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -261,14 +261,18 @@
 Following VSCode integrations may be helpful:
 
 * [ruff](https://marketplace.visualstudio.com/items?itemName=charliermarsh.ruff)
 * [mypy](https://marketplace.visualstudio.com/items?itemName=matangover.mypy)
 
 # CHANGELOG
 
+# 0.7.2
+
+* fix bug in debug log message.
+
 # 0.7.1
 
 * Fix get_list method not returning uuid and status from JSON response
 * Log to debug instead of error where exceptions are already raised.
 * Add raw server response to debug log messages.
 * Update docstrings
```

### Comparing `bring_api-0.7.1/bring_api.egg-info/SOURCES.txt` & `bring_api-0.7.2/bring_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bring_api-0.7.1/pyproject.toml` & `bring_api-0.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bring_api-0.7.1/setup.cfg` & `bring_api-0.7.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bring-api
-version = 0.7.1
+version = 0.7.2
 author = Cyrill Raccaud
 author_email = cyrill.raccaud+pypi@gmail.com
 description = Unofficial package to access Bring! shopping lists API.
 long_description = file: README.md, CHANGELOG.md, LICENCE
 long_description_content_type = text/markdown
 license_files = LICENSE
 url = https://github.com/miaucl/python-bring-api
```

### Comparing `bring_api-0.7.1/tests/test_bring.py` & `bring_api-0.7.2/tests/test_bring.py`

 * *Files identical despite different names*

