# Comparing `tmp/fa-scrapper-0.3.0.tar.gz` & `tmp/fa_scrapper-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fa-scrapper-0.3.0.tar", max compression
+gzip compressed data, was "fa_scrapper-0.4.0.tar", max compression
```

## Comparing `fa-scrapper-0.3.0.tar` & `fa_scrapper-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,4 @@
--rw-r--r--   0        0        0    35149 2021-11-12 15:47:41.118630 fa-scrapper-0.3.0/LICENSE
--rw-r--r--   0        0        0     1804 2021-11-12 15:47:41.118630 fa-scrapper-0.3.0/README.md
--rw-r--r--   0        0        0      183 2021-11-12 15:47:41.118630 fa-scrapper-0.3.0/fa_scrapper/__init__.py
--rw-r--r--   0        0        0     2348 2021-11-12 15:47:41.122630 fa-scrapper-0.3.0/fa_scrapper/cli.py
--rwxr-xr-x   0        0        0     6837 2021-11-12 15:47:41.122630 fa-scrapper-0.3.0/fa_scrapper/fa_scrapper.py
--rw-r--r--   0        0        0      551 2021-11-12 15:47:41.122630 fa-scrapper-0.3.0/fa_scrapper/types.py
--rw-r--r--   0        0        0     1149 2021-11-12 15:47:41.122630 fa-scrapper-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2804 2021-11-12 15:47:55.802220 fa-scrapper-0.3.0/setup.py
--rw-r--r--   0        0        0     3222 2021-11-12 15:47:55.802792 fa-scrapper-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      156 2024-05-30 23:29:05.705028 fa_scrapper-0.4.0/README.md
+-rw-r--r--   0        0        0       77 2024-05-30 23:33:28.121552 fa_scrapper-0.4.0/fa_scrapper/__init__.py
+-rw-r--r--   0        0        0      937 2024-05-30 23:34:20.858674 fa_scrapper-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1382 1970-01-01 00:00:00.000000 fa_scrapper-0.4.0/PKG-INFO
```

### Comparing `fa-scrapper-0.3.0/pyproject.toml` & `fa_scrapper-0.4.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,32 @@
 [tool.poetry]
 name = "fa-scrapper"
-version = "0.3.0"
-description = "A Letterboxd-compatible FilmAffinity scrapper."
+version = "0.4.0"
+description = "A Letterboxd-compatible FilmAffinity scraper."
 license = "GPL-3.0-or-later"
 authors = ["Pablo Baeyens <pbaeyens31+github@gmail.com>"]
 readme = "README.md"
-repository = "https://github.com/mx-psi/fa-scrapper"
+repository = "https://github.com/mx-psi/fa-scraper"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: End Users/Desktop",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Topic :: Utilities",
     "Environment :: Console",
 ]
 
 [tool.poetry.urls]
-"Bug Tracker" = "https://github.com/mx-psi/fa-scrapper/issues"
-"Changelog" = "https://github.com/mx-psi/fa-scrapper/blob/master/CHANGELOG.md"
-"Authors" = "https://github.com/mx-psi/fa-scrapper/blob/master/AUTHORS"
-
-[tool.poetry.scripts]
-fa-scrapper = "fa_scrapper.cli:main"
-fa-scraper = "fa_scrapper.cli:main"
+"Bug Tracker" = "https://github.com/mx-psi/fa-scraper/issues"
+"Changelog" = "https://github.com/mx-psi/fa-scraper/blob/master/CHANGELOG.md"
+"Authors" = "https://github.com/mx-psi/fa-scraper/blob/master/AUTHORS"
 
 [tool.poetry.dependencies]
-python = "^3.6"
-beautifulsoup4 = "^4.9.1"
-requests = "^2.21.0"
-lxml = "^4.5.1"
-arrow = "^1.2.1"
-
-[tool.poetry.dev-dependencies]
-pytest = "^6.1"
+python = "^3.9"
+fa-scraper = "*"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.isort]
 profile = "black"
```

