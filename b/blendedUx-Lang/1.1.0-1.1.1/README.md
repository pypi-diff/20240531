# Comparing `tmp/blendedUx_Lang-1.1.0.tar.gz` & `tmp/blendedUx_Lang-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blendedUx_Lang-1.1.0.tar", last modified: Fri Jul 14 05:41:50 2023, max compression
+gzip compressed data, was "dist\blendedUx_Lang-1.1.1.tar", last modified: Fri May 31 05:21:51 2024, max compression
```

## Comparing `blendedUx_Lang-1.1.0.tar` & `blendedUx_Lang-1.1.1.tar`

### file list

```diff
@@ -1,297 +1,296 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:50.297248 blendedUx_Lang-1.1.0/
--rw-rw-rw-   0        0        0     1096 2023-03-02 07:43:08.000000 blendedUx_Lang-1.1.0/LICENSE
--rw-rw-rw-   0        0        0       29 2023-03-02 07:43:08.000000 blendedUx_Lang-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      261 2023-07-14 05:41:50.296253 blendedUx_Lang-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-13 13:41:32.000000 blendedUx_Lang-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.010924 blendedUx_Lang-1.1.0/blended/
--rw-rw-rw-   0        0        0      161 2023-05-18 08:19:03.000000 blendedUx_Lang-1.1.0/blended/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.149248 blendedUx_Lang-1.1.0/blended/__pycache__/
--rw-rw-rw-   0        0        0      476 2023-05-18 08:27:52.000000 blendedUx_Lang-1.1.0/blended/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      179 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.0/blended/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0     1953 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/__pycache__/_compat.cpython-311.pyc
--rw-rw-rw-   0        0        0     1389 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.0/blended/__pycache__/_compat.cpython-38.pyc
--rw-rw-rw-   0        0        0     6085 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/__pycache__/colormap.cpython-311.pyc
--rw-rw-rw-   0        0        0     3630 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.0/blended/__pycache__/colormap.cpython-38.pyc
--rw-rw-rw-   0        0        0    13894 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/__pycache__/functions.cpython-311.pyc
--rw-rw-rw-   0        0        0     7972 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.0/blended/__pycache__/functions.cpython-38.pyc
--rw-rw-rw-   0        0        0    40556 2023-05-16 15:32:27.000000 blendedUx_Lang-1.1.0/blended/__pycache__/jinjaenv.cpython-311.pyc
--rw-rw-rw-   0        0        0    23364 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.0/blended/__pycache__/jinjaenv.cpython-38.pyc
--rw-rw-rw-   0        0        0     9976 2023-05-16 07:18:27.000000 blendedUx_Lang-1.1.0/blended/__pycache__/sets.cpython-311.pyc
--rw-rw-rw-   0        0        0     6132 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.0/blended/__pycache__/sets.cpython-38.pyc
--rw-rw-rw-   0        0        0    16848 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/__pycache__/trimfloat.cpython-311.pyc
--rw-rw-rw-   0        0        0    10880 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.0/blended/__pycache__/trimfloat.cpython-38.pyc
--rw-rw-rw-   0        0        0      849 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.0/blended/_compat.py
--rw-rw-rw-   0        0        0     4266 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.0/blended/colormap.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.261474 blendedUx_Lang-1.1.0/blended/customtags/
--rw-rw-rw-   0        0        0       79 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.0/blended/customtags/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.518950 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/
--rw-rw-rw-   0        0        0      329 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      289 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0     7101 2023-05-16 07:23:17.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/_compat.cpython-311.pyc
--rw-rw-rw-   0        0        0     4683 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/_compat.cpython-38.pyc
--rw-rw-rw-   0        0        0   210048 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/_stringdefs.cpython-311.pyc
--rw-rw-rw-   0        0        0   208260 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/_stringdefs.cpython-38.pyc
--rw-rw-rw-   0        0        0    49725 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/arguments.cpython-311.pyc
--rw-rw-rw-   0        0        0    26381 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/arguments.cpython-38.pyc
--rw-rw-rw-   0        0        0    14212 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/core.cpython-311.pyc
--rw-rw-rw-   0        0        0     7699 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/core.cpython-38.pyc
--rw-rw-rw-   0        0        0     5726 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/decorators.cpython-311.pyc
--rw-rw-rw-   0        0        0     3317 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/decorators.cpython-38.pyc
--rw-rw-rw-   0        0        0     8652 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/exceptions.cpython-311.pyc
--rw-rw-rw-   0        0        0     6336 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/exceptions.cpython-38.pyc
--rw-rw-rw-   0        0        0    28436 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/expr_parser.cpython-311.pyc
--rw-rw-rw-   0        0        0    13562 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/expr_parser.cpython-38.pyc
--rw-rw-rw-   0        0        0     4256 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/helpers.cpython-311.pyc
--rw-rw-rw-   0        0        0     2842 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/helpers.cpython-38.pyc
--rw-rw-rw-   0        0        0    19689 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/lexer.cpython-311.pyc
--rw-rw-rw-   0        0        0    12473 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/lexer.cpython-38.pyc
--rw-rw-rw-   0        0        0     3181 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/middleware.cpython-311.pyc
--rw-rw-rw-   0        0        0     2053 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/middleware.cpython-38.pyc
--rw-rw-rw-   0        0        0    37791 2023-05-16 07:26:21.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/nodes.cpython-311.pyc
--rw-rw-rw-   0        0        0    22471 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/nodes.cpython-38.pyc
--rw-rw-rw-   0        0        0     6137 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/parser.cpython-311.pyc
--rw-rw-rw-   0        0        0     3264 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/parser.cpython-38.pyc
--rw-rw-rw-   0        0        0     7454 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/tokens.cpython-311.pyc
--rw-rw-rw-   0        0        0     4334 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/tokens.cpython-38.pyc
--rw-rw-rw-   0        0        0    16901 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/trimfloat.cpython-311.pyc
--rw-rw-rw-   0        0        0    10891 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/trimfloat.cpython-38.pyc
--rw-rw-rw-   0        0        0     7096 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/utils.cpython-311.pyc
--rw-rw-rw-   0        0        0     4613 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/utils.cpython-38.pyc
--rw-rw-rw-   0        0        0     7580 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/values.cpython-311.pyc
--rw-rw-rw-   0        0        0     5145 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/__pycache__/values.cpython-38.pyc
--rw-rw-rw-   0        0        0     4200 2023-05-16 07:23:12.000000 blendedUx_Lang-1.1.0/blended/customtags/_compat.py
--rw-rw-rw-   0        0        0   404439 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/_stringdefs.py
--rw-rw-rw-   0        0        0    33426 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/arguments.py
--rw-rw-rw-   0        0        0     8682 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/core.py
--rw-rw-rw-   0        0        0     4103 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/decorators.py
--rw-rw-rw-   0        0        0     4939 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/exceptions.py
--rw-rw-rw-   0        0        0    19676 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/expr_parser.py
--rw-rw-rw-   0        0        0     2779 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/helpers.py
--rw-rw-rw-   0        0        0    17134 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/lexer.py
--rw-rw-rw-   0        0        0     2006 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/middleware.py
--rw-rw-rw-   0        0        0    23316 2023-05-16 07:26:18.000000 blendedUx_Lang-1.1.0/blended/customtags/nodes.py
--rw-rw-rw-   0        0        0     6091 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/parser.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.543008 blendedUx_Lang-1.1.0/blended/customtags/templatetags/
--rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.559003 blendedUx_Lang-1.1.0/blended/customtags/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      220 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      203 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/templatetags/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0      338 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/templatetags/__pycache__/customtags.cpython-311.pyc
--rw-rw-rw-   0        0        0      273 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/templatetags/__pycache__/customtags.cpython-38.pyc
--rw-rw-rw-   0        0        0       60 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/templatetags/customtags.py
--rw-rw-rw-   0        0        0     5689 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/tokens.py
--rw-rw-rw-   0        0        0    10894 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/trimfloat.py
--rw-rw-rw-   0        0        0     6021 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/utils.py
--rw-rw-rw-   0        0        0     3986 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/customtags/values.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.573012 blendedUx_Lang-1.1.0/blended/djangolint/
--rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.686154 blendedUx_Lang-1.1.0/blended/djangolint/__pycache__/
--rw-rw-rw-   0        0        0      207 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      190 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0      262 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/__pycache__/admin.cpython-311.pyc
--rw-rw-rw-   0        0        0      231 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/__pycache__/admin.cpython-38.pyc
--rw-rw-rw-   0        0        0      259 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/__pycache__/models.cpython-311.pyc
--rw-rw-rw-   0        0        0      228 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/__pycache__/models.cpython-38.pyc
--rw-rw-rw-   0        0        0      262 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/__pycache__/tests.cpython-311.pyc
--rw-rw-rw-   0        0        0      231 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/__pycache__/tests.cpython-38.pyc
--rw-rw-rw-   0        0        0      537 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/__pycache__/urls.cpython-311.pyc
--rw-rw-rw-   0        0        0      403 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/__pycache__/urls.cpython-38.pyc
--rw-rw-rw-   0        0        0     1405 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/__pycache__/views.cpython-311.pyc
--rw-rw-rw-   0        0        0      909 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/__pycache__/views.cpython-38.pyc
--rw-rw-rw-   0        0        0       66 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/admin.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.693132 blendedUx_Lang-1.1.0/blended/djangolint/migrations/
--rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.699149 blendedUx_Lang-1.1.0/blended/djangolint/migrations/__pycache__/
--rw-rw-rw-   0        0        0      218 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      201 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/migrations/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0       60 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/models.py
--rw-rw-rw-   0        0        0       63 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/tests.py
--rw-rw-rw-   0        0        0      218 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/urls.py
--rw-rw-rw-   0        0        0      762 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangolint/views.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.713920 blendedUx_Lang-1.1.0/blended/djangotags/
--rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.782221 blendedUx_Lang-1.1.0/blended/djangotags/__pycache__/
--rw-rw-rw-   0        0        0      207 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      190 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0      802 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/djangotags/__pycache__/jinjaenv.cpython-311.pyc
--rw-rw-rw-   0        0        0      576 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/__pycache__/jinjaenv.cpython-38.pyc
--rw-rw-rw-   0        0        0     9257 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/djangotags/__pycache__/loader.cpython-311.pyc
--rw-rw-rw-   0        0        0     4723 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/__pycache__/loader.cpython-38.pyc
--rw-rw-rw-   0        0        0     3985 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/djangotags/__pycache__/models.cpython-311.pyc
--rw-rw-rw-   0        0        0     2991 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/__pycache__/models.cpython-38.pyc
--rw-rw-rw-   0        0        0    77112 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/djangotags/__pycache__/tests.cpython-311.pyc
--rw-rw-rw-   0        0        0    42295 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/__pycache__/tests.cpython-38.pyc
--rw-rw-rw-   0        0        0      345 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/jinjaenv.py
--rw-rw-rw-   0        0        0    13279 2023-07-06 12:10:11.000000 blendedUx_Lang-1.1.0/blended/djangotags/loader.py
--rw-rw-rw-   0        0        0     3349 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/models.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.811106 blendedUx_Lang-1.1.0/blended/djangotags/templates/
--rw-rw-rw-   0        0        0     1127 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/templates/colormacros.html
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.828106 blendedUx_Lang-1.1.0/blended/djangotags/templates/temp/
--rw-rw-rw-   0        0        0       94 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/templates/temp/echotag.html
--rw-rw-rw-   0        0        0       51 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/templates/temp/multilinecomment.html
--rw-rw-rw-   0        0        0       76 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/templates/temp/multilinetag.html
--rw-rw-rw-   0        0        0       15 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/templates/temp/multilinevariable.html
--rw-rw-rw-   0        0        0       71 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/templates/temp/newline.html
--rw-rw-rw-   0        0        0       48 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/templates/temp/whitespace.html
--rw-rw-rw-   0        0        0      125 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/templates/temp/whitespace2.html
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.832115 blendedUx_Lang-1.1.0/blended/djangotags/templatetags/
--rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.850174 blendedUx_Lang-1.1.0/blended/djangotags/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      220 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/djangotags/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      203 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/templatetags/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0    36018 2023-05-16 07:29:05.000000 blendedUx_Lang-1.1.0/blended/djangotags/templatetags/__pycache__/blended_tags.cpython-311.pyc
--rw-rw-rw-   0        0        0    17805 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/templatetags/__pycache__/blended_tags.cpython-38.pyc
--rw-rw-rw-   0        0        0    30325 2023-07-06 12:09:17.000000 blendedUx_Lang-1.1.0/blended/djangotags/templatetags/blended_tags.py
--rw-rw-rw-   0        0        0    53307 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/djangotags/tests.py
--rw-rw-rw-   0        0        0     8530 2023-06-20 10:46:57.000000 blendedUx_Lang-1.1.0/blended/functions.py
--rw-rw-rw-   0        0        0    31394 2023-05-16 08:25:59.000000 blendedUx_Lang-1.1.0/blended/jinjaenv.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.860134 blendedUx_Lang-1.1.0/blended/lint/
--rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.892680 blendedUx_Lang-1.1.0/blended/lint/__pycache__/
--rw-rw-rw-   0        0        0      201 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/lint/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      184 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0     1662 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/lint/__pycache__/lint.cpython-311.pyc
--rw-rw-rw-   0        0        0     1065 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/__pycache__/lint.cpython-38.pyc
--rw-rw-rw-   0        0        0     2418 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/lint/__pycache__/lintcommands.cpython-311.pyc
--rw-rw-rw-   0        0        0     1239 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/__pycache__/lintcommands.cpython-38.pyc
--rw-rw-rw-   0        0        0     1335 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/lint/__pycache__/listeners.cpython-311.pyc
--rw-rw-rw-   0        0        0      893 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/__pycache__/listeners.cpython-38.pyc
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.905699 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/
--rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.917981 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/__pycache__/
--rw-rw-rw-   0        0        0      217 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      200 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0    13027 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/__pycache__/blendedParserListener.cpython-311.pyc
--rw-rw-rw-   0        0        0    12185 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/__pycache__/blendedParserListener.cpython-38.pyc
--rw-rw-rw-   0        0        0     6261 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/blendedLexer.g4
--rw-rw-rw-   0        0        0     4992 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/blendedParser.g4
--rw-rw-rw-   0        0        0     9720 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/blendedParserListener.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.929973 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/
--rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.954983 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/__pycache__/
--rw-rw-rw-   0        0        0      221 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      204 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0    43111 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/__pycache__/blendedLexer.cpython-311.pyc
--rw-rw-rw-   0        0        0    22293 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/__pycache__/blendedLexer.cpython-38.pyc
--rw-rw-rw-   0        0        0   225659 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/__pycache__/blendedParser.cpython-311.pyc
--rw-rw-rw-   0        0        0   118406 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/__pycache__/blendedParser.cpython-38.pyc
--rw-rw-rw-   0        0        0    38068 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/blendedLexer.py
--rw-rw-rw-   0        0        0     1332 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/blendedLexer.tokens
--rw-rw-rw-   0        0        0   140728 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/blendedParser.py
--rw-rw-rw-   0        0        0     1332 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/blendedParser.tokens
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:50.001682 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/
--rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:50.030030 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/__pycache__/
--rw-rw-rw-   0        0        0      221 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      204 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0    42275 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/__pycache__/blendedLexer.cpython-311.pyc
--rw-rw-rw-   0        0        0    22035 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/__pycache__/blendedLexer.cpython-38.pyc
--rw-rw-rw-   0        0        0   227751 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/__pycache__/blendedParser.cpython-311.pyc
--rw-rw-rw-   0        0        0   119493 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/__pycache__/blendedParser.cpython-38.pyc
--rw-rw-rw-   0        0        0    37011 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/blendedLexer.py
--rw-rw-rw-   0        0        0     1332 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/blendedLexer.tokens
--rw-rw-rw-   0        0        0   141316 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/blendedParser.py
--rw-rw-rw-   0        0        0     1332 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/blendedParser.tokens
--rw-rw-rw-   0        0        0      995 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/lint.py
--rw-rw-rw-   0        0        0     1238 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/lintcommands.py
--rw-rw-rw-   0        0        0      405 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/listeners.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:48.929501 blendedUx_Lang-1.1.0/blended/lint/test_files/
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:50.087018 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/
--rw-rw-rw-   0        0        0       16 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/error.html
--rw-rw-rw-   0        0        0      213 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/error_01_0_for_scope.html
--rw-rw-rw-   0        0        0      114 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/error_01_1_for_scope.html
--rw-rw-rw-   0        0        0      180 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/error_02_0_macro_scope.html
--rw-rw-rw-   0        0        0      224 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/error_02_1_macro_scope.html
--rw-rw-rw-   0        0        0      179 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/error_02_2_macro_scope.html
--rw-rw-rw-   0        0        0      105 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/error_03_0_set_block.html
--rw-rw-rw-   0        0        0      187 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/error_04_0_for_dict.html
--rw-rw-rw-   0        0        0      108 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/error_05_0_tilde_expression.html
--rw-rw-rw-   0        0        0       69 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/error_06_0_for_conditional.html
--rw-rw-rw-   0        0        0      196 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/error_07_0_string_iter.html
--rw-rw-rw-   0        0        0      158 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/error_09_0_extends_macro.html
--rw-rw-rw-   0        0        0       40 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/error_10_0_filters_first.html
--rw-rw-rw-   0        0        0      160 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/error_10_1_filters_scope.html
--rw-rw-rw-   0        0        0       65 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/test_04_0_filter.html
--rw-rw-rw-   0        0        0      122 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/test_04_1_filter_echo.html
--rw-rw-rw-   0        0        0      158 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/test_04_2_filter_for.html
--rw-rw-rw-   0        0        0      115 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/test_04_3_filter_sort.html
--rw-rw-rw-   0        0        0      353 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/test_04_4_filter_macro.html
--rw-rw-rw-   0        0        0       81 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/test_08_7_include_macro.html
--rw-rw-rw-   0        0        0       62 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/error_tests/test_08_8_macro_include.html
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:50.093008 blendedUx_Lang-1.1.0/blended/lint/test_files/expr_tests/
--rw-rw-rw-   0        0        0       16 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/expr_tests/error.html
--rw-rw-rw-   0        0        0      286 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/expr_tests/success.html
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:50.240654 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/
--rw-rw-rw-   0        0        0       70 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/modeTest.html
--rw-rw-rw-   0        0        0       93 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_01_0_extends_file.html
--rw-rw-rw-   0        0        0       86 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_01_1_extends_object.html
--rw-rw-rw-   0        0        0      101 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_01_2_extends_parent.html
--rw-rw-rw-   0        0        0       91 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_01_3_extends_inner_block.html
--rw-rw-rw-   0        0        0      104 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_01_4_extends_multiple.html
--rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_01_5_block_scoping.html
--rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_01_5_extends_macro.html
--rw-rw-rw-   0        0        0      353 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_02_0_for_basic.html
--rw-rw-rw-   0        0        0       68 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_02_1_for_expression.html
--rw-rw-rw-   0        0        0      482 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_02_2_for_variables.html
--rw-rw-rw-   0        0        0       93 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_02_4_for_else.html
--rw-rw-rw-   0        0        0      199 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_02_6_for_macro.html
--rw-rw-rw-   0        0        0       96 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_02_7_for_set.html
--rw-rw-rw-   0        0        0      119 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_02_8_for_dict.html
--rw-rw-rw-   0        0        0      140 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_03_0_if_basic.html
--rw-rw-rw-   0        0        0      676 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_03_1_if_expressions.html
--rw-rw-rw-   0        0        0       92 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_03_3_if_scope.html
--rw-rw-rw-   0        0        0      127 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_05_0_set_basic.html
--rw-rw-rw-   0        0        0      137 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_05_1_set_expression.html
--rw-rw-rw-   0        0        0      121 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_05_3_set_macro.html
--rw-rw-rw-   0        0        0       52 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_06_0_do_basic.html
--rw-rw-rw-   0        0        0       49 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_06_1_do_expression.html
--rw-rw-rw-   0        0        0       86 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_06_2_do_macro.html
--rw-rw-rw-   0        0        0      213 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_06_3_do_assign.html
--rw-rw-rw-   0        0        0       22 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_07_0_echo_basic.html
--rw-rw-rw-   0        0        0       50 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_07_1_echo_expression.html
--rw-rw-rw-   0        0        0      102 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_07_2_echo_macro.html
--rw-rw-rw-   0        0        0      219 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_07_3_echo_macro_recur.html
--rw-rw-rw-   0        0        0       37 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_08_0_include_string.html
--rw-rw-rw-   0        0        0       33 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_08_1_include_variable.html
--rw-rw-rw-   0        0        0      520 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_08_3_include_with.html
--rw-rw-rw-   0        0        0       58 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_08_4_include_default_scope.html
--rw-rw-rw-   0        0        0       45 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_08_5_include_ignore_missing.html
--rw-rw-rw-   0        0        0       73 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_08_6_include_only.html
--rw-rw-rw-   0        0        0       83 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_08_7_include_chain.html
--rw-rw-rw-   0        0        0      114 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_08_8_include_scope.html
--rw-rw-rw-   0        0        0      196 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_09_0_raw.html
--rw-rw-rw-   0        0        0       14 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_10_0_variable_filters.html
--rw-rw-rw-   0        0        0      115 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_10_1_comments.html
--rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_11_0_escaping.html
--rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_12_0_whitespace.html
--rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_12_1_string_interpolation.html
--rw-rw-rw-   0        0        0     6340 2023-05-16 07:18:23.000000 blendedUx_Lang-1.1.0/blended/sets.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:50.244664 blendedUx_Lang-1.1.0/blended/testapp/
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:50.250657 blendedUx_Lang-1.1.0/blended/testapp/__pycache__/
--rw-rw-rw-   0        0        0      586 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/testapp/__pycache__/manage.cpython-311.pyc
--rw-rw-rw-   0        0        0      413 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/testapp/__pycache__/manage.cpython-38.pyc
--rw-rw-rw-   0        0        0      260 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/testapp/manage.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:50.261721 blendedUx_Lang-1.1.0/blended/testapp/testapp/
--rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/testapp/testapp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:50.294261 blendedUx_Lang-1.1.0/blended/testapp/testapp/__pycache__/
--rw-rw-rw-   0        0        0      212 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/testapp/testapp/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      195 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/testapp/testapp/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0     2596 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/testapp/testapp/__pycache__/settings.cpython-311.pyc
--rw-rw-rw-   0        0        0     2231 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/testapp/testapp/__pycache__/settings.cpython-38.pyc
--rw-rw-rw-   0        0        0     1123 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/testapp/testapp/__pycache__/urls.cpython-311.pyc
--rw-rw-rw-   0        0        0      984 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/testapp/testapp/__pycache__/urls.cpython-38.pyc
--rw-rw-rw-   0        0        0      734 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.0/blended/testapp/testapp/__pycache__/wsgi.cpython-311.pyc
--rw-rw-rw-   0        0        0      598 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/testapp/testapp/__pycache__/wsgi.cpython-38.pyc
--rw-rw-rw-   0        0        0     3067 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/testapp/testapp/settings.py
--rw-rw-rw-   0        0        0      778 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/testapp/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.0/blended/testapp/testapp/wsgi.py
--rw-rw-rw-   0        0        0    10880 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.0/blended/trimfloat.py
-drwxrwxrwx   0        0        0        0 2023-07-14 05:41:49.110226 blendedUx_Lang-1.1.0/blendedUx_Lang.egg-info/
--rw-rw-rw-   0        0        0      261 2023-07-14 05:41:47.000000 blendedUx_Lang-1.1.0/blendedUx_Lang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    13553 2023-07-14 05:41:48.000000 blendedUx_Lang-1.1.0/blendedUx_Lang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 05:41:47.000000 blendedUx_Lang-1.1.0/blendedUx_Lang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-14 05:41:47.000000 blendedUx_Lang-1.1.0/blendedUx_Lang.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       46 2023-07-14 05:41:47.000000 blendedUx_Lang-1.1.0/blendedUx_Lang.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-14 05:41:47.000000 blendedUx_Lang-1.1.0/blendedUx_Lang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 05:41:50.298258 blendedUx_Lang-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      527 2023-07-14 05:35:03.000000 blendedUx_Lang-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:51.662126 blendedUx_Lang-1.1.1/
+-rw-rw-rw-   0        0        0       29 2023-03-02 07:43:08.000000 blendedUx_Lang-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      247 2024-05-31 05:21:51.662126 blendedUx_Lang-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-13 13:41:32.000000 blendedUx_Lang-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:48.457003 blendedUx_Lang-1.1.1/blended/
+-rw-rw-rw-   0        0        0      161 2023-05-18 08:19:03.000000 blendedUx_Lang-1.1.1/blended/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:48.679341 blendedUx_Lang-1.1.1/blended/__pycache__/
+-rw-rw-rw-   0        0        0      476 2023-05-18 08:27:52.000000 blendedUx_Lang-1.1.1/blended/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      179 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.1/blended/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1953 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/__pycache__/_compat.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1389 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.1/blended/__pycache__/_compat.cpython-38.pyc
+-rw-rw-rw-   0        0        0     6085 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/__pycache__/colormap.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3630 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.1/blended/__pycache__/colormap.cpython-38.pyc
+-rw-rw-rw-   0        0        0    13894 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/__pycache__/functions.cpython-311.pyc
+-rw-rw-rw-   0        0        0     7972 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.1/blended/__pycache__/functions.cpython-38.pyc
+-rw-rw-rw-   0        0        0    40556 2023-05-16 15:32:27.000000 blendedUx_Lang-1.1.1/blended/__pycache__/jinjaenv.cpython-311.pyc
+-rw-rw-rw-   0        0        0    23364 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.1/blended/__pycache__/jinjaenv.cpython-38.pyc
+-rw-rw-rw-   0        0        0     9976 2023-05-16 07:18:27.000000 blendedUx_Lang-1.1.1/blended/__pycache__/sets.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6132 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.1/blended/__pycache__/sets.cpython-38.pyc
+-rw-rw-rw-   0        0        0    16848 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/__pycache__/trimfloat.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10880 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.1/blended/__pycache__/trimfloat.cpython-38.pyc
+-rw-rw-rw-   0        0        0      849 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.1/blended/_compat.py
+-rw-rw-rw-   0        0        0     4266 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.1/blended/colormap.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:49.164106 blendedUx_Lang-1.1.1/blended/customtags/
+-rw-rw-rw-   0        0        0       79 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.1/blended/customtags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:49.351158 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/
+-rw-rw-rw-   0        0        0      329 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      289 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0     7101 2023-05-16 07:23:17.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/_compat.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4683 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/_compat.cpython-38.pyc
+-rw-rw-rw-   0        0        0   210048 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/_stringdefs.cpython-311.pyc
+-rw-rw-rw-   0        0        0   208260 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/_stringdefs.cpython-38.pyc
+-rw-rw-rw-   0        0        0    49725 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/arguments.cpython-311.pyc
+-rw-rw-rw-   0        0        0    26381 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/arguments.cpython-38.pyc
+-rw-rw-rw-   0        0        0    14212 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/core.cpython-311.pyc
+-rw-rw-rw-   0        0        0     7699 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/core.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5726 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/decorators.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3317 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/decorators.cpython-38.pyc
+-rw-rw-rw-   0        0        0     8652 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/exceptions.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6336 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/exceptions.cpython-38.pyc
+-rw-rw-rw-   0        0        0    28436 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/expr_parser.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13562 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/expr_parser.cpython-38.pyc
+-rw-rw-rw-   0        0        0     4256 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/helpers.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2842 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/helpers.cpython-38.pyc
+-rw-rw-rw-   0        0        0    19689 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/lexer.cpython-311.pyc
+-rw-rw-rw-   0        0        0    12473 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/lexer.cpython-38.pyc
+-rw-rw-rw-   0        0        0     3181 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/middleware.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2053 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/middleware.cpython-38.pyc
+-rw-rw-rw-   0        0        0    37791 2023-05-16 07:26:21.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/nodes.cpython-311.pyc
+-rw-rw-rw-   0        0        0    22471 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/nodes.cpython-38.pyc
+-rw-rw-rw-   0        0        0     6137 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/parser.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3264 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/parser.cpython-38.pyc
+-rw-rw-rw-   0        0        0     7454 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/tokens.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4334 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/tokens.cpython-38.pyc
+-rw-rw-rw-   0        0        0    16901 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/trimfloat.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10891 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/trimfloat.cpython-38.pyc
+-rw-rw-rw-   0        0        0     7096 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/utils.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4613 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/utils.cpython-38.pyc
+-rw-rw-rw-   0        0        0     7580 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/values.cpython-311.pyc
+-rw-rw-rw-   0        0        0     5145 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/__pycache__/values.cpython-38.pyc
+-rw-rw-rw-   0        0        0     4200 2023-05-16 07:23:12.000000 blendedUx_Lang-1.1.1/blended/customtags/_compat.py
+-rw-rw-rw-   0        0        0   404439 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/_stringdefs.py
+-rw-rw-rw-   0        0        0    33426 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/arguments.py
+-rw-rw-rw-   0        0        0     8682 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/core.py
+-rw-rw-rw-   0        0        0     4103 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/decorators.py
+-rw-rw-rw-   0        0        0     4939 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/exceptions.py
+-rw-rw-rw-   0        0        0    19676 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/expr_parser.py
+-rw-rw-rw-   0        0        0     2779 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/helpers.py
+-rw-rw-rw-   0        0        0    17134 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/lexer.py
+-rw-rw-rw-   0        0        0     2006 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/middleware.py
+-rw-rw-rw-   0        0        0    23316 2023-05-16 07:26:18.000000 blendedUx_Lang-1.1.1/blended/customtags/nodes.py
+-rw-rw-rw-   0        0        0     6091 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/parser.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:49.382845 blendedUx_Lang-1.1.1/blended/customtags/templatetags/
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:49.407024 blendedUx_Lang-1.1.1/blended/customtags/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      220 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      203 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/templatetags/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0      338 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/templatetags/__pycache__/customtags.cpython-311.pyc
+-rw-rw-rw-   0        0        0      273 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/templatetags/__pycache__/customtags.cpython-38.pyc
+-rw-rw-rw-   0        0        0       60 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/templatetags/customtags.py
+-rw-rw-rw-   0        0        0     5689 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/tokens.py
+-rw-rw-rw-   0        0        0    10894 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/trimfloat.py
+-rw-rw-rw-   0        0        0     6021 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/utils.py
+-rw-rw-rw-   0        0        0     3986 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/customtags/values.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:49.493257 blendedUx_Lang-1.1.1/blended/djangolint/
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangolint/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:49.564411 blendedUx_Lang-1.1.1/blended/djangolint/__pycache__/
+-rw-rw-rw-   0        0        0      207 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangolint/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      190 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangolint/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0      262 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangolint/__pycache__/admin.cpython-311.pyc
+-rw-rw-rw-   0        0        0      231 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangolint/__pycache__/admin.cpython-38.pyc
+-rw-rw-rw-   0        0        0      259 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangolint/__pycache__/models.cpython-311.pyc
+-rw-rw-rw-   0        0        0      228 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangolint/__pycache__/models.cpython-38.pyc
+-rw-rw-rw-   0        0        0      262 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangolint/__pycache__/tests.cpython-311.pyc
+-rw-rw-rw-   0        0        0      231 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangolint/__pycache__/tests.cpython-38.pyc
+-rw-rw-rw-   0        0        0      537 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangolint/__pycache__/urls.cpython-311.pyc
+-rw-rw-rw-   0        0        0      403 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangolint/__pycache__/urls.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1405 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangolint/__pycache__/views.cpython-311.pyc
+-rw-rw-rw-   0        0        0      909 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangolint/__pycache__/views.cpython-38.pyc
+-rw-rw-rw-   0        0        0       66 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangolint/admin.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:49.567407 blendedUx_Lang-1.1.1/blended/djangolint/migrations/
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangolint/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:49.573407 blendedUx_Lang-1.1.1/blended/djangolint/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      218 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangolint/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      201 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangolint/migrations/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0       60 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangolint/models.py
+-rw-rw-rw-   0        0        0       63 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangolint/tests.py
+-rw-rw-rw-   0        0        0      218 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangolint/urls.py
+-rw-rw-rw-   0        0        0      762 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangolint/views.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:49.678676 blendedUx_Lang-1.1.1/blended/djangotags/
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangotags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:49.740191 blendedUx_Lang-1.1.1/blended/djangotags/__pycache__/
+-rw-rw-rw-   0        0        0      207 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangotags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      190 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangotags/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0      802 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.1/blended/djangotags/__pycache__/jinjaenv.cpython-311.pyc
+-rw-rw-rw-   0        0        0      576 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangotags/__pycache__/jinjaenv.cpython-38.pyc
+-rw-rw-rw-   0        0        0     9257 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.1/blended/djangotags/__pycache__/loader.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4723 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangotags/__pycache__/loader.cpython-38.pyc
+-rw-rw-rw-   0        0        0     3985 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.1/blended/djangotags/__pycache__/models.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2991 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangotags/__pycache__/models.cpython-38.pyc
+-rw-rw-rw-   0        0        0    77112 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.1/blended/djangotags/__pycache__/tests.cpython-311.pyc
+-rw-rw-rw-   0        0        0    42295 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangotags/__pycache__/tests.cpython-38.pyc
+-rw-rw-rw-   0        0        0      345 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangotags/jinjaenv.py
+-rw-rw-rw-   0        0        0    13408 2024-05-30 12:46:53.000000 blendedUx_Lang-1.1.1/blended/djangotags/loader.py
+-rw-rw-rw-   0        0        0     3349 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangotags/models.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:49.746805 blendedUx_Lang-1.1.1/blended/djangotags/templates/
+-rw-rw-rw-   0        0        0     1127 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangotags/templates/colormacros.html
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:49.865126 blendedUx_Lang-1.1.1/blended/djangotags/templates/temp/
+-rw-rw-rw-   0        0        0       94 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangotags/templates/temp/echotag.html
+-rw-rw-rw-   0        0        0       51 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangotags/templates/temp/multilinecomment.html
+-rw-rw-rw-   0        0        0       76 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangotags/templates/temp/multilinetag.html
+-rw-rw-rw-   0        0        0       15 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangotags/templates/temp/multilinevariable.html
+-rw-rw-rw-   0        0        0       71 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangotags/templates/temp/newline.html
+-rw-rw-rw-   0        0        0       48 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangotags/templates/temp/whitespace.html
+-rw-rw-rw-   0        0        0      125 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangotags/templates/temp/whitespace2.html
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:49.899321 blendedUx_Lang-1.1.1/blended/djangotags/templatetags/
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangotags/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:49.912845 blendedUx_Lang-1.1.1/blended/djangotags/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      220 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.1/blended/djangotags/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      203 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangotags/templatetags/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0    36018 2023-05-16 07:29:05.000000 blendedUx_Lang-1.1.1/blended/djangotags/templatetags/__pycache__/blended_tags.cpython-311.pyc
+-rw-rw-rw-   0        0        0    17805 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangotags/templatetags/__pycache__/blended_tags.cpython-38.pyc
+-rw-rw-rw-   0        0        0    30611 2024-05-30 13:09:45.000000 blendedUx_Lang-1.1.1/blended/djangotags/templatetags/blended_tags.py
+-rw-rw-rw-   0        0        0    53307 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/djangotags/tests.py
+-rw-rw-rw-   0        0        0     8530 2023-06-20 10:46:57.000000 blendedUx_Lang-1.1.1/blended/functions.py
+-rw-rw-rw-   0        0        0    31394 2023-05-16 08:25:59.000000 blendedUx_Lang-1.1.1/blended/jinjaenv.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:49.988723 blendedUx_Lang-1.1.1/blended/lint/
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:50.012994 blendedUx_Lang-1.1.1/blended/lint/__pycache__/
+-rw-rw-rw-   0        0        0      201 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.1/blended/lint/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      184 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1662 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.1/blended/lint/__pycache__/lint.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1065 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/__pycache__/lint.cpython-38.pyc
+-rw-rw-rw-   0        0        0     2418 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.1/blended/lint/__pycache__/lintcommands.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1239 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/__pycache__/lintcommands.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1335 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.1/blended/lint/__pycache__/listeners.cpython-311.pyc
+-rw-rw-rw-   0        0        0      893 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/__pycache__/listeners.cpython-38.pyc
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:50.088468 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:50.112096 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/__pycache__/
+-rw-rw-rw-   0        0        0      217 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      200 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0    13027 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/__pycache__/blendedParserListener.cpython-311.pyc
+-rw-rw-rw-   0        0        0    12185 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/__pycache__/blendedParserListener.cpython-38.pyc
+-rw-rw-rw-   0        0        0     6261 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/blendedLexer.g4
+-rw-rw-rw-   0        0        0     4992 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/blendedParser.g4
+-rw-rw-rw-   0        0        0     9720 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/blendedParserListener.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:50.333838 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py2/
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py2/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:50.370566 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py2/__pycache__/
+-rw-rw-rw-   0        0        0      221 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py2/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      204 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py2/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0    43111 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py2/__pycache__/blendedLexer.cpython-311.pyc
+-rw-rw-rw-   0        0        0    22293 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py2/__pycache__/blendedLexer.cpython-38.pyc
+-rw-rw-rw-   0        0        0   225659 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py2/__pycache__/blendedParser.cpython-311.pyc
+-rw-rw-rw-   0        0        0   118406 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py2/__pycache__/blendedParser.cpython-38.pyc
+-rw-rw-rw-   0        0        0    38068 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py2/blendedLexer.py
+-rw-rw-rw-   0        0        0     1332 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py2/blendedLexer.tokens
+-rw-rw-rw-   0        0        0   140728 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py2/blendedParser.py
+-rw-rw-rw-   0        0        0     1332 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py2/blendedParser.tokens
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:50.511774 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py3/
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py3/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:50.555224 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py3/__pycache__/
+-rw-rw-rw-   0        0        0      221 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py3/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      204 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py3/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0    42275 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py3/__pycache__/blendedLexer.cpython-311.pyc
+-rw-rw-rw-   0        0        0    22035 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py3/__pycache__/blendedLexer.cpython-38.pyc
+-rw-rw-rw-   0        0        0   227751 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py3/__pycache__/blendedParser.cpython-311.pyc
+-rw-rw-rw-   0        0        0   119493 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py3/__pycache__/blendedParser.cpython-38.pyc
+-rw-rw-rw-   0        0        0    37011 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py3/blendedLexer.py
+-rw-rw-rw-   0        0        0     1332 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py3/blendedLexer.tokens
+-rw-rw-rw-   0        0        0   141316 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py3/blendedParser.py
+-rw-rw-rw-   0        0        0     1332 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py3/blendedParser.tokens
+-rw-rw-rw-   0        0        0      995 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/lint.py
+-rw-rw-rw-   0        0        0     1238 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/lintcommands.py
+-rw-rw-rw-   0        0        0      405 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/listeners.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:48.215526 blendedUx_Lang-1.1.1/blended/lint/test_files/
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:50.878299 blendedUx_Lang-1.1.1/blended/lint/test_files/error_tests/
+-rw-rw-rw-   0        0        0       16 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/error_tests/error.html
+-rw-rw-rw-   0        0        0      213 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/error_tests/error_01_0_for_scope.html
+-rw-rw-rw-   0        0        0      114 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/error_tests/error_01_1_for_scope.html
+-rw-rw-rw-   0        0        0      180 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/error_tests/error_02_0_macro_scope.html
+-rw-rw-rw-   0        0        0      224 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/error_tests/error_02_1_macro_scope.html
+-rw-rw-rw-   0        0        0      179 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/error_tests/error_02_2_macro_scope.html
+-rw-rw-rw-   0        0        0      105 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/error_tests/error_03_0_set_block.html
+-rw-rw-rw-   0        0        0      187 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/error_tests/error_04_0_for_dict.html
+-rw-rw-rw-   0        0        0      108 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/error_tests/error_05_0_tilde_expression.html
+-rw-rw-rw-   0        0        0       69 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/error_tests/error_06_0_for_conditional.html
+-rw-rw-rw-   0        0        0      196 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/error_tests/error_07_0_string_iter.html
+-rw-rw-rw-   0        0        0      158 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/error_tests/error_09_0_extends_macro.html
+-rw-rw-rw-   0        0        0       40 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/error_tests/error_10_0_filters_first.html
+-rw-rw-rw-   0        0        0      160 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/error_tests/error_10_1_filters_scope.html
+-rw-rw-rw-   0        0        0       65 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/error_tests/test_04_0_filter.html
+-rw-rw-rw-   0        0        0      122 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/error_tests/test_04_1_filter_echo.html
+-rw-rw-rw-   0        0        0      158 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/error_tests/test_04_2_filter_for.html
+-rw-rw-rw-   0        0        0      115 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/error_tests/test_04_3_filter_sort.html
+-rw-rw-rw-   0        0        0      353 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/error_tests/test_04_4_filter_macro.html
+-rw-rw-rw-   0        0        0       81 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/error_tests/test_08_7_include_macro.html
+-rw-rw-rw-   0        0        0       62 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/error_tests/test_08_8_macro_include.html
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:50.924530 blendedUx_Lang-1.1.1/blended/lint/test_files/expr_tests/
+-rw-rw-rw-   0        0        0       16 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/expr_tests/error.html
+-rw-rw-rw-   0        0        0      286 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/expr_tests/success.html
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:51.524424 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/
+-rw-rw-rw-   0        0        0       70 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/modeTest.html
+-rw-rw-rw-   0        0        0       93 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_01_0_extends_file.html
+-rw-rw-rw-   0        0        0       86 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_01_1_extends_object.html
+-rw-rw-rw-   0        0        0      101 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_01_2_extends_parent.html
+-rw-rw-rw-   0        0        0       91 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_01_3_extends_inner_block.html
+-rw-rw-rw-   0        0        0      104 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_01_4_extends_multiple.html
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_01_5_block_scoping.html
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_01_5_extends_macro.html
+-rw-rw-rw-   0        0        0      353 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_02_0_for_basic.html
+-rw-rw-rw-   0        0        0       68 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_02_1_for_expression.html
+-rw-rw-rw-   0        0        0      482 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_02_2_for_variables.html
+-rw-rw-rw-   0        0        0       93 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_02_4_for_else.html
+-rw-rw-rw-   0        0        0      199 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_02_6_for_macro.html
+-rw-rw-rw-   0        0        0       96 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_02_7_for_set.html
+-rw-rw-rw-   0        0        0      119 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_02_8_for_dict.html
+-rw-rw-rw-   0        0        0      140 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_03_0_if_basic.html
+-rw-rw-rw-   0        0        0      676 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_03_1_if_expressions.html
+-rw-rw-rw-   0        0        0       92 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_03_3_if_scope.html
+-rw-rw-rw-   0        0        0      127 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_05_0_set_basic.html
+-rw-rw-rw-   0        0        0      137 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_05_1_set_expression.html
+-rw-rw-rw-   0        0        0      121 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_05_3_set_macro.html
+-rw-rw-rw-   0        0        0       52 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_06_0_do_basic.html
+-rw-rw-rw-   0        0        0       49 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_06_1_do_expression.html
+-rw-rw-rw-   0        0        0       86 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_06_2_do_macro.html
+-rw-rw-rw-   0        0        0      213 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_06_3_do_assign.html
+-rw-rw-rw-   0        0        0       22 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_07_0_echo_basic.html
+-rw-rw-rw-   0        0        0       50 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_07_1_echo_expression.html
+-rw-rw-rw-   0        0        0      102 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_07_2_echo_macro.html
+-rw-rw-rw-   0        0        0      219 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_07_3_echo_macro_recur.html
+-rw-rw-rw-   0        0        0       37 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_08_0_include_string.html
+-rw-rw-rw-   0        0        0       33 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_08_1_include_variable.html
+-rw-rw-rw-   0        0        0      520 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_08_3_include_with.html
+-rw-rw-rw-   0        0        0       58 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_08_4_include_default_scope.html
+-rw-rw-rw-   0        0        0       45 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_08_5_include_ignore_missing.html
+-rw-rw-rw-   0        0        0       73 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_08_6_include_only.html
+-rw-rw-rw-   0        0        0       83 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_08_7_include_chain.html
+-rw-rw-rw-   0        0        0      114 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_08_8_include_scope.html
+-rw-rw-rw-   0        0        0      196 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_09_0_raw.html
+-rw-rw-rw-   0        0        0       14 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_10_0_variable_filters.html
+-rw-rw-rw-   0        0        0      115 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_10_1_comments.html
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_11_0_escaping.html
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_12_0_whitespace.html
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_12_1_string_interpolation.html
+-rw-rw-rw-   0        0        0     6340 2023-05-16 07:18:23.000000 blendedUx_Lang-1.1.1/blended/sets.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:51.544795 blendedUx_Lang-1.1.1/blended/testapp/
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:51.569590 blendedUx_Lang-1.1.1/blended/testapp/__pycache__/
+-rw-rw-rw-   0        0        0      586 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.1/blended/testapp/__pycache__/manage.cpython-311.pyc
+-rw-rw-rw-   0        0        0      413 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/testapp/__pycache__/manage.cpython-38.pyc
+-rw-rw-rw-   0        0        0      260 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/testapp/manage.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:51.612125 blendedUx_Lang-1.1.1/blended/testapp/testapp/
+-rw-rw-rw-   0        0        0        0 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/testapp/testapp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:51.659124 blendedUx_Lang-1.1.1/blended/testapp/testapp/__pycache__/
+-rw-rw-rw-   0        0        0      212 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.1/blended/testapp/testapp/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      195 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/testapp/testapp/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0     2596 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.1/blended/testapp/testapp/__pycache__/settings.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2231 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/testapp/testapp/__pycache__/settings.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1123 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.1/blended/testapp/testapp/__pycache__/urls.cpython-311.pyc
+-rw-rw-rw-   0        0        0      984 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/testapp/testapp/__pycache__/urls.cpython-38.pyc
+-rw-rw-rw-   0        0        0      734 2023-05-16 06:28:00.000000 blendedUx_Lang-1.1.1/blended/testapp/testapp/__pycache__/wsgi.cpython-311.pyc
+-rw-rw-rw-   0        0        0      598 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/testapp/testapp/__pycache__/wsgi.cpython-38.pyc
+-rw-rw-rw-   0        0        0     3067 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/testapp/testapp/settings.py
+-rw-rw-rw-   0        0        0      778 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/testapp/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2023-05-16 06:27:59.000000 blendedUx_Lang-1.1.1/blended/testapp/testapp/wsgi.py
+-rw-rw-rw-   0        0        0    10880 2023-05-16 06:27:58.000000 blendedUx_Lang-1.1.1/blended/trimfloat.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:21:48.549222 blendedUx_Lang-1.1.1/blendedUx_Lang.egg-info/
+-rw-rw-rw-   0        0        0      247 2024-05-31 05:21:47.000000 blendedUx_Lang-1.1.1/blendedUx_Lang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    13555 2024-05-31 05:21:48.000000 blendedUx_Lang-1.1.1/blendedUx_Lang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 05:21:47.000000 blendedUx_Lang-1.1.1/blendedUx_Lang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-31 05:21:47.000000 blendedUx_Lang-1.1.1/blendedUx_Lang.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       46 2024-05-31 05:21:47.000000 blendedUx_Lang-1.1.1/blendedUx_Lang.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-31 05:21:47.000000 blendedUx_Lang-1.1.1/blendedUx_Lang.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 05:21:51.667158 blendedUx_Lang-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      527 2024-05-31 05:05:15.000000 blendedUx_Lang-1.1.1/setup.py
```

### Comparing `blendedUx_Lang-1.1.0/blended/__pycache__/_compat.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/__pycache__/_compat.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/__pycache__/_compat.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/__pycache__/_compat.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/__pycache__/colormap.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/__pycache__/colormap.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/__pycache__/colormap.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/__pycache__/colormap.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/__pycache__/functions.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/__pycache__/functions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/__pycache__/functions.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/__pycache__/functions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/__pycache__/jinjaenv.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/__pycache__/jinjaenv.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/__pycache__/jinjaenv.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/__pycache__/jinjaenv.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/__pycache__/sets.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/__pycache__/sets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/__pycache__/sets.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/__pycache__/sets.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/__pycache__/trimfloat.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/__pycache__/trimfloat.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/__pycache__/trimfloat.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/__pycache__/trimfloat.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/_compat.py` & `blendedUx_Lang-1.1.1/blended/_compat.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/colormap.py` & `blendedUx_Lang-1.1.1/blended/colormap.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/_compat.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/_compat.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/_compat.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/_compat.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/_stringdefs.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/_stringdefs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/_stringdefs.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/_stringdefs.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/arguments.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/arguments.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/arguments.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/arguments.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/core.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/core.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/core.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/core.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/decorators.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/decorators.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/decorators.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/decorators.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/exceptions.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/exceptions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/exceptions.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/exceptions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/expr_parser.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/expr_parser.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/expr_parser.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/expr_parser.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/helpers.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/helpers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/helpers.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/helpers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/lexer.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/lexer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/lexer.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/lexer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/middleware.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/middleware.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/middleware.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/middleware.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/nodes.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/nodes.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/nodes.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/nodes.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/parser.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/parser.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/parser.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/parser.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/tokens.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/tokens.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/tokens.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/tokens.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/trimfloat.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/trimfloat.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/trimfloat.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/trimfloat.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/utils.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/utils.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/values.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/values.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/__pycache__/values.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/customtags/__pycache__/values.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/_compat.py` & `blendedUx_Lang-1.1.1/blended/customtags/_compat.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/_stringdefs.py` & `blendedUx_Lang-1.1.1/blended/customtags/_stringdefs.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/arguments.py` & `blendedUx_Lang-1.1.1/blended/customtags/arguments.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/core.py` & `blendedUx_Lang-1.1.1/blended/customtags/core.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/decorators.py` & `blendedUx_Lang-1.1.1/blended/customtags/decorators.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/exceptions.py` & `blendedUx_Lang-1.1.1/blended/customtags/exceptions.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/expr_parser.py` & `blendedUx_Lang-1.1.1/blended/customtags/expr_parser.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/helpers.py` & `blendedUx_Lang-1.1.1/blended/customtags/helpers.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/lexer.py` & `blendedUx_Lang-1.1.1/blended/customtags/lexer.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/middleware.py` & `blendedUx_Lang-1.1.1/blended/customtags/middleware.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/nodes.py` & `blendedUx_Lang-1.1.1/blended/customtags/nodes.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/parser.py` & `blendedUx_Lang-1.1.1/blended/customtags/parser.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/tokens.py` & `blendedUx_Lang-1.1.1/blended/customtags/tokens.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/trimfloat.py` & `blendedUx_Lang-1.1.1/blended/customtags/trimfloat.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/utils.py` & `blendedUx_Lang-1.1.1/blended/customtags/utils.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/customtags/values.py` & `blendedUx_Lang-1.1.1/blended/customtags/values.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/djangolint/__pycache__/urls.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/djangolint/__pycache__/urls.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/djangolint/__pycache__/views.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/djangolint/__pycache__/views.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/djangolint/__pycache__/views.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/djangolint/__pycache__/views.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/djangolint/views.py` & `blendedUx_Lang-1.1.1/blended/djangolint/views.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/djangotags/__pycache__/jinjaenv.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/djangotags/__pycache__/jinjaenv.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/djangotags/__pycache__/jinjaenv.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/djangotags/__pycache__/jinjaenv.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/djangotags/__pycache__/loader.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/djangotags/__pycache__/loader.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/djangotags/__pycache__/loader.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/djangotags/__pycache__/loader.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/djangotags/__pycache__/models.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/djangotags/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/djangotags/__pycache__/models.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/djangotags/__pycache__/models.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/djangotags/__pycache__/tests.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/djangotags/__pycache__/tests.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/djangotags/__pycache__/tests.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/djangotags/__pycache__/tests.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/djangotags/loader.py` & `blendedUx_Lang-1.1.1/blended/djangotags/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,19 +193,22 @@
     template_string = re.sub(
        r'''(?s)((?:{%\s*verbatim\s*%}.*?)?{%\s*endverbatim\s*%})|(\'{{(\s*.*?\s*)?}}\')|(\"{{(\s*.*?\s*)?}}\")|"(.*{{.*?}}.*?)"|'(.*{{.*?}}.*?)'|{{(\s*.*?\s*)}}(?!(\"|\'))''', substitute, template_string, 0, re.S)
 
     return template_string
 
 
 
+template_dict = {}
 def template_from_string(template_string):
-    # import pdb; pdb.set_trace()
     template_string = preprocess(template_string)
-    template_obj = Template(template_string)
-    return template_obj
+    if template_string in template_dict:
+        return template_dict[template_string]
+    else:
+        template_dict[template_string] = Template(template_string)
+        return template_dict[template_string]
 
 
 
 class Loader(BaseLoader):
     
     is_usable = True
```

### Comparing `blendedUx_Lang-1.1.0/blended/djangotags/models.py` & `blendedUx_Lang-1.1.1/blended/djangotags/models.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/djangotags/templates/colormacros.html` & `blendedUx_Lang-1.1.1/blended/djangotags/templates/colormacros.html`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/djangotags/templatetags/__pycache__/blended_tags.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/djangotags/templatetags/__pycache__/blended_tags.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/djangotags/templatetags/__pycache__/blended_tags.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/djangotags/templatetags/__pycache__/blended_tags.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/djangotags/templatetags/blended_tags.py` & `blendedUx_Lang-1.1.1/blended/djangotags/templatetags/blended_tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,15 @@
         """
         Instantiating RequestContext constructure is causing
         all the context_processors to execute everytime this is being called.
         # deepcopy throwing TypeError("cannot serialize '_io.BufferedReader' object")
         """
         new_context = copy(context)
         new_context.update(builtin_funcs())
+        new_context.update(initial_data)
 
     ## If we don't have a RequestContext, then we need to invoke the builtins
     ## context processor directly.  User functions will not be available
     ## inside the macro body unless added originally to the macro context.
 
     else:
         new_context = Context(autoescape=context.autoescape)
@@ -318,15 +319,15 @@
         relative_name.startswith(('"', "'")) and relative_name[0] == relative_name[-1]
     )
     # if not get_template(new_name):
     #     breakpoint()
     return f'"{new_name}"' if has_quotes else new_name
 
 
-
+render_dict = {}
 class Include(core.Tag):
     options = core.Options(
         arguments.Argument("template"),
         arguments.Optional(
             arguments.Constant("ignore"),
             arguments.Constant("missing"),
         ),
@@ -399,15 +400,20 @@
                 context.autoescape = old_ae_setting
                 return rendered
 
             ## this should be implemented as 'with context.push(**extra_context)'
             ## but we can't do that because we are supporting old Django
             
             context.update(extra_context)
-            rendered = template.render(context)
+            if template in render_dict:
+                rendered = render_dict[template]
+            else:
+                render_dict[template] = template.render(context)
+                rendered = render_dict[template]
+            # rendered = template.render(context)
             context.pop()
             context.autoescape = old_ae_setting
             return rendered
         # modified the exception because Blended support for "ignore missing" argument with include tag
         # Django remove the "ignore missing" functionalities from version 2.x
         except TemplateDoesNotExist:
             bits = self.token.split_contents()
```

### Comparing `blendedUx_Lang-1.1.0/blended/djangotags/tests.py` & `blendedUx_Lang-1.1.1/blended/djangotags/tests.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/functions.py` & `blendedUx_Lang-1.1.1/blended/functions.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/jinjaenv.py` & `blendedUx_Lang-1.1.1/blended/jinjaenv.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/__pycache__/lint.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/lint/__pycache__/lint.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/__pycache__/lint.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/lint/__pycache__/lint.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/__pycache__/lintcommands.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/lint/__pycache__/lintcommands.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/__pycache__/lintcommands.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/lint/__pycache__/lintcommands.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/__pycache__/listeners.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/lint/__pycache__/listeners.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/__pycache__/listeners.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/lint/__pycache__/listeners.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/blended_grammar/__pycache__/blendedParserListener.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/lint/blended_grammar/__pycache__/blendedParserListener.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/blended_grammar/__pycache__/blendedParserListener.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/lint/blended_grammar/__pycache__/blendedParserListener.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/blended_grammar/blendedLexer.g4` & `blendedUx_Lang-1.1.1/blended/lint/blended_grammar/blendedLexer.g4`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/blended_grammar/blendedParser.g4` & `blendedUx_Lang-1.1.1/blended/lint/blended_grammar/blendedParser.g4`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/blended_grammar/blendedParserListener.py` & `blendedUx_Lang-1.1.1/blended/lint/blended_grammar/blendedParserListener.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/__pycache__/blendedLexer.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py2/__pycache__/blendedLexer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/__pycache__/blendedLexer.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py2/__pycache__/blendedLexer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/__pycache__/blendedParser.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py2/__pycache__/blendedParser.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/__pycache__/blendedParser.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py2/__pycache__/blendedParser.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/blendedLexer.py` & `blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py2/blendedLexer.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/blendedLexer.tokens` & `blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py2/blendedLexer.tokens`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/blendedParser.py` & `blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py2/blendedParser.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py2/blendedParser.tokens` & `blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py2/blendedParser.tokens`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/__pycache__/blendedLexer.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py3/__pycache__/blendedLexer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/__pycache__/blendedLexer.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py3/__pycache__/blendedLexer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/__pycache__/blendedParser.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py3/__pycache__/blendedParser.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/__pycache__/blendedParser.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py3/__pycache__/blendedParser.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/blendedLexer.py` & `blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py3/blendedLexer.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/blendedLexer.tokens` & `blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py3/blendedLexer.tokens`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/blendedParser.py` & `blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py3/blendedParser.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/blended_grammar/py3/blendedParser.tokens` & `blendedUx_Lang-1.1.1/blended/lint/blended_grammar/py3/blendedParser.tokens`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/lint.py` & `blendedUx_Lang-1.1.1/blended/lint/lint.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/lintcommands.py` & `blendedUx_Lang-1.1.1/blended/lint/lintcommands.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_03_1_if_expressions.html` & `blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_03_1_if_expressions.html`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/lint/test_files/success_tests/test_08_3_include_with.html` & `blendedUx_Lang-1.1.1/blended/lint/test_files/success_tests/test_08_3_include_with.html`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/sets.py` & `blendedUx_Lang-1.1.1/blended/sets.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/testapp/__pycache__/manage.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/testapp/__pycache__/manage.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/testapp/testapp/__pycache__/settings.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/testapp/testapp/__pycache__/settings.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/testapp/testapp/__pycache__/settings.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/testapp/testapp/__pycache__/settings.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/testapp/testapp/__pycache__/urls.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/testapp/testapp/__pycache__/urls.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/testapp/testapp/__pycache__/urls.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/testapp/testapp/__pycache__/urls.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/testapp/testapp/__pycache__/wsgi.cpython-311.pyc` & `blendedUx_Lang-1.1.1/blended/testapp/testapp/__pycache__/wsgi.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/testapp/testapp/__pycache__/wsgi.cpython-38.pyc` & `blendedUx_Lang-1.1.1/blended/testapp/testapp/__pycache__/wsgi.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/testapp/testapp/settings.py` & `blendedUx_Lang-1.1.1/blended/testapp/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/testapp/testapp/urls.py` & `blendedUx_Lang-1.1.1/blended/testapp/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blended/trimfloat.py` & `blendedUx_Lang-1.1.1/blended/trimfloat.py`

 * *Files identical despite different names*

### Comparing `blendedUx_Lang-1.1.0/blendedUx_Lang.egg-info/SOURCES.txt` & `blendedUx_Lang-1.1.1/blendedUx_Lang.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-LICENSE
 MANIFEST.in
 README.md
+setup.cfg
 setup.py
 blended/__init__.py
 blended/_compat.py
 blended/colormap.py
 blended/functions.py
 blended/jinjaenv.py
 blended/sets.py
```

### Comparing `blendedUx_Lang-1.1.0/setup.py` & `blendedUx_Lang-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 from setuptools import setup
 
 DESCRIPTION = 'BlendedUx_lang'
 
 setup(
     name='blendedUx_Lang',
-    version="1.1.0",
+    version="1.1.1",
     url='http://blended.dbmonline.net/',
     author='DBM',
     author_email='hbhadu@cognam.com',
     description=('Blended Command Line Application'),
     license='BSD',
     packages=['blended'],
     include_package_data=True,
```

