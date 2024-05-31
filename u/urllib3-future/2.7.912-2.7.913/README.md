# Comparing `tmp/urllib3_future-2.7.912.tar.gz` & `tmp/urllib3_future-2.7.913.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon May 27 04:38:09 2024, max compression
+gzip compressed data, last modified: Fri May 31 03:52:38 2024, max compression
```

## Comparing `urllib3_future-2.7.912.tar` & `urllib3_future-2.7.913.tar`

### file list

```diff
@@ -1,312 +1,312 @@
--rw-r--r--   0        0        0    88285 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/CHANGES.rst
--rw-r--r--   0        0        0      490 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/dev-requirements.txt
--rw-r--r--   0        0        0     4602 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/Makefile
--rw-r--r--   0        0        0    54247 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/advanced-usage.rst
--rw-r--r--   0        0        0     4297 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/async.rst
--rw-r--r--   0        0        0       59 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/changelog.rst
--rw-r--r--   0        0        0     5787 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/conf.py
--rw-r--r--   0        0        0     6749 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/contributing.rst
--rw-r--r--   0        0        0     1939 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/index.rst
--rw-r--r--   0        0        0     4513 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/make.bat
--rw-r--r--   0        0        0       92 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/requirements.txt
--rw-r--r--   0        0        0    17426 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/user-guide.rst
--rw-r--r--   0        0        0    15195 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/v2-migration-guide.rst
--rw-r--r--   0        0        0     1770 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/_static/banner.svg
--rw-r--r--   0        0        0     3999 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/_static/banner_github.svg
--rw-r--r--   0        0        0     1818 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/_static/dark-logo.svg
--rw-r--r--   0        0        0   307934 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/_static/logo.png
--rw-r--r--   0        0        0     7872 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/images/demo-button.png
--rw-r--r--   0        0        0      714 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/images/favicon.png
--rw-r--r--   0        0        0     6226 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/images/learn-more-button.png
--rw-r--r--   0        0        0     2165 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/images/logo.png
--rw-r--r--   0        0        0      516 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/images/logo.svg
--rw-r--r--   0        0        0      245 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/reference/index.rst
--rw-r--r--   0        0        0      457 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/reference/urllib3.backend.rst
--rw-r--r--   0        0        0      349 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/reference/urllib3.connection.rst
--rw-r--r--   0        0        0      712 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/reference/urllib3.connectionpool.rst
--rw-r--r--   0        0        0      185 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/reference/urllib3.exceptions.rst
--rw-r--r--   0        0        0      350 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/reference/urllib3.fields.rst
--rw-r--r--   0        0        0      559 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/reference/urllib3.poolmanager.rst
--rw-r--r--   0        0        0       71 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/reference/urllib3.request.rst
--rw-r--r--   0        0        0      905 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/reference/urllib3.response.rst
--rw-r--r--   0        0        0      385 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/reference/urllib3.util.rst
--rw-r--r--   0        0        0      206 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/reference/contrib/index.rst
--rw-r--r--   0        0        0      231 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/reference/contrib/resolver.rst
--rw-r--r--   0        0        0      124 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/reference/contrib/socks.rst
--rw-r--r--   0        0        0      142 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/docs/reference/contrib/ssa.rst
--rw-r--r--   0        0        0        0 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/dummyserver/__init__.py
--rw-r--r--   0        0        0    13408 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/dummyserver/handlers.py
--rwxr-xr-x   0        0        0     1198 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/dummyserver/https_proxy.py
--rwxr-xr-x   0        0        0     4582 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/dummyserver/proxy.py
--rwxr-xr-x   0        0        0     9813 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/dummyserver/server.py
--rw-r--r--   0        0        0    11213 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/dummyserver/testcase.py
--rw-r--r--   0        0        0      511 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/dummyserver/certs/README.rst
--rw-r--r--   0        0        0     1679 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/dummyserver/certs/cacert.key
--rw-r--r--   0        0        0     1273 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/dummyserver/certs/cacert.pem
--rw-r--r--   0        0        0     1265 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/dummyserver/certs/server.crt
--rw-r--r--   0        0        0     1679 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/dummyserver/certs/server.key
--rw-r--r--   0        0        0     6090 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/__init__.py
--rw-r--r--   0        0        0    15956 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/_collections.py
--rw-r--r--   0        0        0     8241 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/_constant.py
--rw-r--r--   0        0        0    21727 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/_request_methods.py
--rw-r--r--   0        0        0     2655 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/_typing.py
--rw-r--r--   0        0        0      100 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/_version.py
--rw-r--r--   0        0        0    38148 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/connection.py
--rw-r--r--   0        0        0    75685 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/connectionpool.py
--rw-r--r--   0        0        0     9988 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/exceptions.py
--rw-r--r--   0        0        0     9151 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/fields.py
--rw-r--r--   0        0        0     2202 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/filepost.py
--rw-r--r--   0        0        0    36048 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/poolmanager.py
--rw-r--r--   0        0        0       93 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/py.typed
--rw-r--r--   0        0        0    35459 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/response.py
--rw-r--r--   0        0        0        0 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/_async/__init__.py
--rw-r--r--   0        0        0    36236 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/_async/connection.py
--rw-r--r--   0        0        0    77458 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/_async/connectionpool.py
--rw-r--r--   0        0        0    32214 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/_async/poolmanager.py
--rw-r--r--   0        0        0    17222 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/_async/response.py
--rw-r--r--   0        0        0      390 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/backend/__init__.py
--rw-r--r--   0        0        0    16166 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/backend/_base.py
--rw-r--r--   0        0        0    45613 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/backend/hface.py
--rw-r--r--   0        0        0      225 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/backend/_async/__init__.py
--rw-r--r--   0        0        0     5987 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/backend/_async/_base.py
--rw-r--r--   0        0        0    43334 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/backend/_async/hface.py
--rw-r--r--   0        0        0        0 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0     4930 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/_socks_override.py
--rw-r--r--   0        0        0      724 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0    13565 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/socks.py
--rw-r--r--   0        0        0     1185 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/hface/__init__.py
--rw-r--r--   0        0        0     1775 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/hface/_configuration.py
--rw-r--r--   0        0        0     1283 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/hface/_error_codes.py
--rw-r--r--   0        0        0     3729 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/hface/_stream_matrix.py
--rw-r--r--   0        0        0      877 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/hface/_typing.py
--rw-r--r--   0        0        0        0 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/hface/py.typed
--rw-r--r--   0        0        0     1161 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/hface/events/__init__.py
--rw-r--r--   0        0        0     4497 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/hface/events/_events.py
--rw-r--r--   0        0        0     1079 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/hface/protocols/__init__.py
--rw-r--r--   0        0        0     4403 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/hface/protocols/_factories.py
--rw-r--r--   0        0        0    10011 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/hface/protocols/_protocols.py
--rw-r--r--   0        0        0      781 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/hface/protocols/http1/__init__.py
--rw-r--r--   0        0        0    10477 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/hface/protocols/http1/_h11.py
--rw-r--r--   0        0        0      780 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/hface/protocols/http2/__init__.py
--rw-r--r--   0        0        0     9160 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/hface/protocols/http2/_h2.py
--rw-r--r--   0        0        0      785 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/hface/protocols/http3/__init__.py
--rw-r--r--   0        0        0    16858 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/hface/protocols/http3/_qh3.py
--rw-r--r--   0        0        0     3314 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/imcc/__init__.py
--rw-r--r--   0        0        0      293 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/__init__.py
--rw-r--r--   0        0        0     8415 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/factories.py
--rw-r--r--   0        0        0    18961 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/protocols.py
--rw-r--r--   0        0        0     4290 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/utils.py
--rw-r--r--   0        0        0      291 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/_async/__init__.py
--rw-r--r--   0        0        0     7871 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/_async/factories.py
--rw-r--r--   0        0        0    10621 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/_async/protocols.py
--rw-r--r--   0        0        0      381 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/_async/doh/__init__.py
--rw-r--r--   0        0        0    22371 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/_async/doh/_urllib3.py
--rw-r--r--   0        0        0      338 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/_async/doq/__init__.py
--rw-r--r--   0        0        0    15402 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/_async/doq/_qh3.py
--rw-r--r--   0        0        0      329 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/_async/dot/__init__.py
--rw-r--r--   0        0        0     5951 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/_async/dot/_ssl.py
--rw-r--r--   0        0        0      292 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/_async/dou/__init__.py
--rw-r--r--   0        0        0    11140 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/_async/dou/_socket.py
--rw-r--r--   0        0        0      105 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/_async/in_memory/__init__.py
--rw-r--r--   0        0        0     5299 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/_async/in_memory/_dict.py
--rw-r--r--   0        0        0     2643 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/_async/null/__init__.py
--rw-r--r--   0        0        0      103 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/_async/system/__init__.py
--rw-r--r--   0        0        0     1770 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/_async/system/_socket.py
--rw-r--r--   0        0        0      381 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/doh/__init__.py
--rw-r--r--   0        0        0    22180 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/doh/_urllib3.py
--rw-r--r--   0        0        0      338 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/doq/__init__.py
--rw-r--r--   0        0        0    14846 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/doq/_qh3.py
--rw-r--r--   0        0        0      329 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/dot/__init__.py
--rw-r--r--   0        0        0     4493 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/dot/_ssl.py
--rw-r--r--   0        0        0      292 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/dou/__init__.py
--rw-r--r--   0        0        0    10836 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/dou/_socket.py
--rw-r--r--   0        0        0      105 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/in_memory/__init__.py
--rw-r--r--   0        0        0     5425 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/in_memory/_dict.py
--rw-r--r--   0        0        0     2539 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/null/__init__.py
--rw-r--r--   0        0        0      103 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/system/__init__.py
--rw-r--r--   0        0        0     1626 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/resolver/system/_socket.py
--rw-r--r--   0        0        0    12158 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/contrib/ssa/__init__.py
--rw-r--r--   0        0        0      999 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/util/__init__.py
--rw-r--r--   0        0        0     3884 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/util/connection.py
--rw-r--r--   0        0        0     1145 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/util/proxy.py
--rw-r--r--   0        0        0     8886 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/util/request.py
--rw-r--r--   0        0        0     1329 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/util/response.py
--rw-r--r--   0        0        0    19245 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/util/retry.py
--rw-r--r--   0        0        0    24862 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5816 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     7226 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10684 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/util/timeout.py
--rw-r--r--   0        0        0    21813 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/util/traffic_police.py
--rw-r--r--   0        0        0    15295 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/util/url.py
--rw-r--r--   0        0        0     1146 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/util/util.py
--rw-r--r--   0        0        0     4423 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/util/wait.py
--rw-r--r--   0        0        0        0 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/util/_async/__init__.py
--rw-r--r--   0        0        0     5492 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/util/_async/ssl_.py
--rw-r--r--   0        0        0    22078 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3/util/_async/traffic_police.py
--rw-r--r--   0        0        0     6090 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/__init__.py
--rw-r--r--   0        0        0    15956 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/_collections.py
--rw-r--r--   0        0        0     8241 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/_constant.py
--rw-r--r--   0        0        0    21727 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/_request_methods.py
--rw-r--r--   0        0        0     2655 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/_typing.py
--rw-r--r--   0        0        0      100 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/_version.py
--rw-r--r--   0        0        0    38148 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/connection.py
--rw-r--r--   0        0        0    75685 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/connectionpool.py
--rw-r--r--   0        0        0     9988 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/exceptions.py
--rw-r--r--   0        0        0     9151 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/fields.py
--rw-r--r--   0        0        0     2202 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/filepost.py
--rw-r--r--   0        0        0    36048 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/poolmanager.py
--rw-r--r--   0        0        0       93 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/py.typed
--rw-r--r--   0        0        0    35459 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/response.py
--rw-r--r--   0        0        0        0 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/_async/__init__.py
--rw-r--r--   0        0        0    36236 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/_async/connection.py
--rw-r--r--   0        0        0    77458 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/_async/connectionpool.py
--rw-r--r--   0        0        0    32214 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/_async/poolmanager.py
--rw-r--r--   0        0        0    17222 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/_async/response.py
--rw-r--r--   0        0        0      390 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/backend/__init__.py
--rw-r--r--   0        0        0    16166 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/backend/_base.py
--rw-r--r--   0        0        0    45613 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/backend/hface.py
--rw-r--r--   0        0        0      225 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/backend/_async/__init__.py
--rw-r--r--   0        0        0     5987 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/backend/_async/_base.py
--rw-r--r--   0        0        0    43334 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/backend/_async/hface.py
--rw-r--r--   0        0        0        0 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/__init__.py
--rw-r--r--   0        0        0     4930 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/_socks_override.py
--rw-r--r--   0        0        0      724 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/pyopenssl.py
--rw-r--r--   0        0        0    13565 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/socks.py
--rw-r--r--   0        0        0     1185 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/hface/__init__.py
--rw-r--r--   0        0        0     1775 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/hface/_configuration.py
--rw-r--r--   0        0        0     1283 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/hface/_error_codes.py
--rw-r--r--   0        0        0     3729 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/hface/_stream_matrix.py
--rw-r--r--   0        0        0      877 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/hface/_typing.py
--rw-r--r--   0        0        0        0 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/hface/py.typed
--rw-r--r--   0        0        0     1161 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/hface/events/__init__.py
--rw-r--r--   0        0        0     4497 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/hface/events/_events.py
--rw-r--r--   0        0        0     1079 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/hface/protocols/__init__.py
--rw-r--r--   0        0        0     4403 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/hface/protocols/_factories.py
--rw-r--r--   0        0        0    10011 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/hface/protocols/_protocols.py
--rw-r--r--   0        0        0      781 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/hface/protocols/http1/__init__.py
--rw-r--r--   0        0        0    10477 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/hface/protocols/http1/_h11.py
--rw-r--r--   0        0        0      780 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/hface/protocols/http2/__init__.py
--rw-r--r--   0        0        0     9160 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/hface/protocols/http2/_h2.py
--rw-r--r--   0        0        0      785 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/hface/protocols/http3/__init__.py
--rw-r--r--   0        0        0    16858 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/hface/protocols/http3/_qh3.py
--rw-r--r--   0        0        0     3314 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/imcc/__init__.py
--rw-r--r--   0        0        0      293 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/__init__.py
--rw-r--r--   0        0        0     8415 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/factories.py
--rw-r--r--   0        0        0    18961 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/protocols.py
--rw-r--r--   0        0        0     4290 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/utils.py
--rw-r--r--   0        0        0      291 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/_async/__init__.py
--rw-r--r--   0        0        0     7871 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/_async/factories.py
--rw-r--r--   0        0        0    10621 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/_async/protocols.py
--rw-r--r--   0        0        0      381 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/_async/doh/__init__.py
--rw-r--r--   0        0        0    22371 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/_async/doh/_urllib3.py
--rw-r--r--   0        0        0      338 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/_async/doq/__init__.py
--rw-r--r--   0        0        0    15402 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/_async/doq/_qh3.py
--rw-r--r--   0        0        0      329 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/_async/dot/__init__.py
--rw-r--r--   0        0        0     5951 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/_async/dot/_ssl.py
--rw-r--r--   0        0        0      292 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/_async/dou/__init__.py
--rw-r--r--   0        0        0    11140 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/_async/dou/_socket.py
--rw-r--r--   0        0        0      105 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/_async/in_memory/__init__.py
--rw-r--r--   0        0        0     5299 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/_async/in_memory/_dict.py
--rw-r--r--   0        0        0     2643 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/_async/null/__init__.py
--rw-r--r--   0        0        0      103 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/_async/system/__init__.py
--rw-r--r--   0        0        0     1770 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/_async/system/_socket.py
--rw-r--r--   0        0        0      381 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/doh/__init__.py
--rw-r--r--   0        0        0    22180 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/doh/_urllib3.py
--rw-r--r--   0        0        0      338 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/doq/__init__.py
--rw-r--r--   0        0        0    14846 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/doq/_qh3.py
--rw-r--r--   0        0        0      329 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/dot/__init__.py
--rw-r--r--   0        0        0     4493 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/dot/_ssl.py
--rw-r--r--   0        0        0      292 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/dou/__init__.py
--rw-r--r--   0        0        0    10836 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/dou/_socket.py
--rw-r--r--   0        0        0      105 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/in_memory/__init__.py
--rw-r--r--   0        0        0     5425 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/in_memory/_dict.py
--rw-r--r--   0        0        0     2539 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/null/__init__.py
--rw-r--r--   0        0        0      103 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/system/__init__.py
--rw-r--r--   0        0        0     1626 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/system/_socket.py
--rw-r--r--   0        0        0    12158 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/contrib/ssa/__init__.py
--rw-r--r--   0        0        0      999 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/util/__init__.py
--rw-r--r--   0        0        0     3884 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/util/connection.py
--rw-r--r--   0        0        0     1145 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/util/proxy.py
--rw-r--r--   0        0        0     8886 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/util/request.py
--rw-r--r--   0        0        0     1329 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/util/response.py
--rw-r--r--   0        0        0    19245 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/util/retry.py
--rw-r--r--   0        0        0    24862 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/util/ssl_.py
--rw-r--r--   0        0        0     5816 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     7226 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/util/ssltransport.py
--rw-r--r--   0        0        0    10684 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/util/timeout.py
--rw-r--r--   0        0        0    21813 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/util/traffic_police.py
--rw-r--r--   0        0        0    15295 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/util/url.py
--rw-r--r--   0        0        0     1146 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/util/util.py
--rw-r--r--   0        0        0     4423 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/util/wait.py
--rw-r--r--   0        0        0        0 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/util/_async/__init__.py
--rw-r--r--   0        0        0     5492 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/util/_async/ssl_.py
--rw-r--r--   0        0        0    22078 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/src/urllib3_future/util/_async/traffic_police.py
--rw-r--r--   0        0        0     9646 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/__init__.py
--rw-r--r--   0        0        0    11926 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/conftest.py
--rw-r--r--   0        0        0     6222 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/port_helpers.py
--rw-r--r--   0        0        0    12638 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/test_collections.py
--rw-r--r--   0        0        0      692 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/test_compatibility.py
--rw-r--r--   0        0        0    10288 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/test_connection.py
--rw-r--r--   0        0        0    22649 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/test_connectionpool.py
--rw-r--r--   0        0        0     1531 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/test_exceptions.py
--rw-r--r--   0        0        0     3882 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/test_fields.py
--rw-r--r--   0        0        0     3778 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/test_filepost.py
--rw-r--r--   0        0        0      978 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/test_no_ssl.py
--rw-r--r--   0        0        0    17951 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/test_poolmanager.py
--rw-r--r--   0        0        0     3657 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/test_proxymanager.py
--rw-r--r--   0        0        0    38863 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/test_response.py
--rw-r--r--   0        0        0    16640 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/test_retry.py
--rw-r--r--   0        0        0     6554 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/test_ssl.py
--rw-r--r--   0        0        0    16917 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/test_ssltransport.py
--rw-r--r--   0        0        0    43037 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/test_util.py
--rw-r--r--   0        0        0     5999 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/test_wait.py
--rw-r--r--   0        0        0     1187 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/tz_stub.py
--rw-r--r--   0        0        0        0 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/contrib/__init__.py
--rw-r--r--   0        0        0     1257 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/contrib/duplicate_san.pem
--rw-r--r--   0        0        0    21281 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/contrib/test_resolver.py
--rw-r--r--   0        0        0    25922 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/contrib/test_socks.py
--rw-r--r--   0        0        0        0 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/contrib/asynchronous/__init__.py
--rw-r--r--   0        0        0    21291 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/contrib/asynchronous/test_resolver.py
--rw-r--r--   0        0        0    21728 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/contrib/asynchronous/test_socks.py
--rw-r--r--   0        0        0        0 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/contrib/hface/__init__.py
--rw-r--r--   0        0        0     3717 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/contrib/hface/test_stream_matrix.py
--rw-r--r--   0        0        0        0 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_dummyserver/__init__.py
--rw-r--r--   0        0        0     9840 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_dummyserver/test_chunked_transfer.py
--rw-r--r--   0        0        0     3702 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_dummyserver/test_connection.py
--rw-r--r--   0        0        0    56059 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_dummyserver/test_connectionpool.py
--rw-r--r--   0        0        0     7756 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_dummyserver/test_happy_eyeballs.py
--rw-r--r--   0        0        0    43193 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_dummyserver/test_https.py
--rw-r--r--   0        0        0     1104 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_dummyserver/test_no_ssl.py
--rw-r--r--   0        0        0    23853 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_dummyserver/test_poolmanager.py
--rw-r--r--   0        0        0    32501 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_dummyserver/test_proxy_poolmanager.py
--rw-r--r--   0        0        0    88179 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_dummyserver/test_socketlevel.py
--rw-r--r--   0        0        0        0 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_dummyserver/asynchronous/__init__.py
--rw-r--r--   0        0        0    59408 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_dummyserver/asynchronous/test_connectionpool.py
--rw-r--r--   0        0        0     7329 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_dummyserver/asynchronous/test_happy_eyeballs.py
--rw-r--r--   0        0        0    19562 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_dummyserver/asynchronous/test_poolmanager.py
--rw-r--r--   0        0        0     2837 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_traefik/__init__.py
--rw-r--r--   0        0        0     3069 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_traefik/test_conn_info.py
--rw-r--r--   0        0        0     4873 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_traefik/test_connection.py
--rw-r--r--   0        0        0     2821 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_traefik/test_connection_multiplexed.py
--rw-r--r--   0        0        0     5912 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_traefik/test_connectionpool_multiplexed.py
--rw-r--r--   0        0        0     3357 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_traefik/test_protolevel.py
--rw-r--r--   0        0        0     3209 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_traefik/test_proxy.py
--rw-r--r--   0        0        0     5622 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_traefik/test_send_data.py
--rw-r--r--   0        0        0     1864 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_traefik/test_stream.py
--rw-r--r--   0        0        0     6683 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_traefik/test_svn.py
--rw-r--r--   0        0        0        0 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_traefik/asynchronous/__init__.py
--rw-r--r--   0        0        0     2217 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_traefik/asynchronous/test_conn_info.py
--rw-r--r--   0        0        0     5177 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_traefik/asynchronous/test_connection.py
--rw-r--r--   0        0        0     3122 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_traefik/asynchronous/test_connection_multiplexed.py
--rw-r--r--   0        0        0     6143 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_traefik/asynchronous/test_connectionpool_multiplexed.py
--rw-r--r--   0        0        0     3481 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_traefik/asynchronous/test_protolevel.py
--rw-r--r--   0        0        0     3274 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_traefik/asynchronous/test_proxy.py
--rw-r--r--   0        0        0     5844 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_traefik/asynchronous/test_send_data.py
--rw-r--r--   0        0        0     1967 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_traefik/asynchronous/test_stream.py
--rw-r--r--   0        0        0     7217 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/test/with_traefik/asynchronous/test_svn.py
--rw-r--r--   0        0        0       85 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/.gitignore
--rw-r--r--   0        0        0     1093 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/LICENSE.txt
--rw-r--r--   0        0        0     4277 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/README.md
--rw-r--r--   0        0        0     1342 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/hatch_build.py
--rw-r--r--   0        0        0     5698 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/pyproject.toml
--rw-r--r--   0        0        0     7087 2024-05-27 04:38:09.000000 urllib3_future-2.7.912/PKG-INFO
+-rw-r--r--   0        0        0    88457 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/CHANGES.rst
+-rw-r--r--   0        0        0      490 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/dev-requirements.txt
+-rw-r--r--   0        0        0     4602 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/Makefile
+-rw-r--r--   0        0        0    54247 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/advanced-usage.rst
+-rw-r--r--   0        0        0     4297 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/async.rst
+-rw-r--r--   0        0        0       59 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/changelog.rst
+-rw-r--r--   0        0        0     5787 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/conf.py
+-rw-r--r--   0        0        0     6749 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/contributing.rst
+-rw-r--r--   0        0        0     1939 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/index.rst
+-rw-r--r--   0        0        0     4513 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/make.bat
+-rw-r--r--   0        0        0       92 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/requirements.txt
+-rw-r--r--   0        0        0    17426 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/user-guide.rst
+-rw-r--r--   0        0        0    15195 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/v2-migration-guide.rst
+-rw-r--r--   0        0        0     1770 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/_static/banner.svg
+-rw-r--r--   0        0        0     3999 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/_static/banner_github.svg
+-rw-r--r--   0        0        0     1818 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/_static/dark-logo.svg
+-rw-r--r--   0        0        0   307934 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/_static/logo.png
+-rw-r--r--   0        0        0     7872 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/images/demo-button.png
+-rw-r--r--   0        0        0      714 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/images/favicon.png
+-rw-r--r--   0        0        0     6226 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/images/learn-more-button.png
+-rw-r--r--   0        0        0     2165 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/images/logo.png
+-rw-r--r--   0        0        0      516 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/images/logo.svg
+-rw-r--r--   0        0        0      245 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/reference/index.rst
+-rw-r--r--   0        0        0      457 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/reference/urllib3.backend.rst
+-rw-r--r--   0        0        0      349 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/reference/urllib3.connection.rst
+-rw-r--r--   0        0        0      712 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/reference/urllib3.connectionpool.rst
+-rw-r--r--   0        0        0      185 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/reference/urllib3.exceptions.rst
+-rw-r--r--   0        0        0      350 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/reference/urllib3.fields.rst
+-rw-r--r--   0        0        0      559 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/reference/urllib3.poolmanager.rst
+-rw-r--r--   0        0        0       71 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/reference/urllib3.request.rst
+-rw-r--r--   0        0        0      905 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/reference/urllib3.response.rst
+-rw-r--r--   0        0        0      385 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/reference/urllib3.util.rst
+-rw-r--r--   0        0        0      206 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/reference/contrib/index.rst
+-rw-r--r--   0        0        0      231 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/reference/contrib/resolver.rst
+-rw-r--r--   0        0        0      124 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/reference/contrib/socks.rst
+-rw-r--r--   0        0        0      142 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/docs/reference/contrib/ssa.rst
+-rw-r--r--   0        0        0        0 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/dummyserver/__init__.py
+-rw-r--r--   0        0        0    13408 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/dummyserver/handlers.py
+-rwxr-xr-x   0        0        0     1198 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/dummyserver/https_proxy.py
+-rwxr-xr-x   0        0        0     4582 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/dummyserver/proxy.py
+-rwxr-xr-x   0        0        0     9813 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/dummyserver/server.py
+-rw-r--r--   0        0        0    11213 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/dummyserver/testcase.py
+-rw-r--r--   0        0        0      511 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/dummyserver/certs/README.rst
+-rw-r--r--   0        0        0     1679 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/dummyserver/certs/cacert.key
+-rw-r--r--   0        0        0     1273 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/dummyserver/certs/cacert.pem
+-rw-r--r--   0        0        0     1265 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/dummyserver/certs/server.crt
+-rw-r--r--   0        0        0     1679 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/dummyserver/certs/server.key
+-rw-r--r--   0        0        0     6090 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/__init__.py
+-rw-r--r--   0        0        0    15956 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/_collections.py
+-rw-r--r--   0        0        0     8241 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/_constant.py
+-rw-r--r--   0        0        0    21727 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/_request_methods.py
+-rw-r--r--   0        0        0     2655 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/_typing.py
+-rw-r--r--   0        0        0      100 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/_version.py
+-rw-r--r--   0        0        0    38148 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/connection.py
+-rw-r--r--   0        0        0    76099 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/connectionpool.py
+-rw-r--r--   0        0        0     9988 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/exceptions.py
+-rw-r--r--   0        0        0     9151 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/fields.py
+-rw-r--r--   0        0        0     2202 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/filepost.py
+-rw-r--r--   0        0        0    36048 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/poolmanager.py
+-rw-r--r--   0        0        0       93 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/py.typed
+-rw-r--r--   0        0        0    35459 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/response.py
+-rw-r--r--   0        0        0        0 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/_async/__init__.py
+-rw-r--r--   0        0        0    36236 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/_async/connection.py
+-rw-r--r--   0        0        0    77884 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/_async/connectionpool.py
+-rw-r--r--   0        0        0    32214 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/_async/poolmanager.py
+-rw-r--r--   0        0        0    17222 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/_async/response.py
+-rw-r--r--   0        0        0      390 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/backend/__init__.py
+-rw-r--r--   0        0        0    16166 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/backend/_base.py
+-rw-r--r--   0        0        0    45773 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/backend/hface.py
+-rw-r--r--   0        0        0      225 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/backend/_async/__init__.py
+-rw-r--r--   0        0        0     5987 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/backend/_async/_base.py
+-rw-r--r--   0        0        0    43500 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/backend/_async/hface.py
+-rw-r--r--   0        0        0        0 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0     4930 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/_socks_override.py
+-rw-r--r--   0        0        0      724 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    13565 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0     1185 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/hface/__init__.py
+-rw-r--r--   0        0        0     1775 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/hface/_configuration.py
+-rw-r--r--   0        0        0     1283 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/hface/_error_codes.py
+-rw-r--r--   0        0        0     3729 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/hface/_stream_matrix.py
+-rw-r--r--   0        0        0      877 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/hface/_typing.py
+-rw-r--r--   0        0        0        0 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/hface/py.typed
+-rw-r--r--   0        0        0     1161 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/hface/events/__init__.py
+-rw-r--r--   0        0        0     4497 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/hface/events/_events.py
+-rw-r--r--   0        0        0     1079 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/hface/protocols/__init__.py
+-rw-r--r--   0        0        0     4403 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/hface/protocols/_factories.py
+-rw-r--r--   0        0        0    10011 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/hface/protocols/_protocols.py
+-rw-r--r--   0        0        0      781 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/hface/protocols/http1/__init__.py
+-rw-r--r--   0        0        0    10477 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/hface/protocols/http1/_h11.py
+-rw-r--r--   0        0        0      780 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/hface/protocols/http2/__init__.py
+-rw-r--r--   0        0        0     9160 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/hface/protocols/http2/_h2.py
+-rw-r--r--   0        0        0      785 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/hface/protocols/http3/__init__.py
+-rw-r--r--   0        0        0    16858 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/hface/protocols/http3/_qh3.py
+-rw-r--r--   0        0        0     3314 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/imcc/__init__.py
+-rw-r--r--   0        0        0      293 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/__init__.py
+-rw-r--r--   0        0        0     8415 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/factories.py
+-rw-r--r--   0        0        0    18961 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/protocols.py
+-rw-r--r--   0        0        0     4290 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/utils.py
+-rw-r--r--   0        0        0      291 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/_async/__init__.py
+-rw-r--r--   0        0        0     7871 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/_async/factories.py
+-rw-r--r--   0        0        0    10621 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/_async/protocols.py
+-rw-r--r--   0        0        0      381 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/_async/doh/__init__.py
+-rw-r--r--   0        0        0    22371 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/_async/doh/_urllib3.py
+-rw-r--r--   0        0        0      338 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/_async/doq/__init__.py
+-rw-r--r--   0        0        0    15402 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/_async/doq/_qh3.py
+-rw-r--r--   0        0        0      329 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/_async/dot/__init__.py
+-rw-r--r--   0        0        0     5951 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/_async/dot/_ssl.py
+-rw-r--r--   0        0        0      292 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/_async/dou/__init__.py
+-rw-r--r--   0        0        0    11140 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/_async/dou/_socket.py
+-rw-r--r--   0        0        0      105 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/_async/in_memory/__init__.py
+-rw-r--r--   0        0        0     5299 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/_async/in_memory/_dict.py
+-rw-r--r--   0        0        0     2643 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/_async/null/__init__.py
+-rw-r--r--   0        0        0      103 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/_async/system/__init__.py
+-rw-r--r--   0        0        0     1770 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/_async/system/_socket.py
+-rw-r--r--   0        0        0      381 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/doh/__init__.py
+-rw-r--r--   0        0        0    22180 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/doh/_urllib3.py
+-rw-r--r--   0        0        0      338 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/doq/__init__.py
+-rw-r--r--   0        0        0    14846 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/doq/_qh3.py
+-rw-r--r--   0        0        0      329 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/dot/__init__.py
+-rw-r--r--   0        0        0     4493 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/dot/_ssl.py
+-rw-r--r--   0        0        0      292 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/dou/__init__.py
+-rw-r--r--   0        0        0    10836 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/dou/_socket.py
+-rw-r--r--   0        0        0      105 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/in_memory/__init__.py
+-rw-r--r--   0        0        0     5425 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/in_memory/_dict.py
+-rw-r--r--   0        0        0     2539 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/null/__init__.py
+-rw-r--r--   0        0        0      103 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/system/__init__.py
+-rw-r--r--   0        0        0     1626 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/resolver/system/_socket.py
+-rw-r--r--   0        0        0    12158 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/contrib/ssa/__init__.py
+-rw-r--r--   0        0        0      999 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     3884 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1145 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/util/proxy.py
+-rw-r--r--   0        0        0     8886 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/util/request.py
+-rw-r--r--   0        0        0     1329 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/util/response.py
+-rw-r--r--   0        0        0    19245 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/util/retry.py
+-rw-r--r--   0        0        0    24862 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     5816 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     7226 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10684 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    21813 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/util/traffic_police.py
+-rw-r--r--   0        0        0    15295 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/util/url.py
+-rw-r--r--   0        0        0     1146 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/util/util.py
+-rw-r--r--   0        0        0     4423 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/util/wait.py
+-rw-r--r--   0        0        0        0 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/util/_async/__init__.py
+-rw-r--r--   0        0        0     5492 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/util/_async/ssl_.py
+-rw-r--r--   0        0        0    22078 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3/util/_async/traffic_police.py
+-rw-r--r--   0        0        0     6090 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/__init__.py
+-rw-r--r--   0        0        0    15956 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/_collections.py
+-rw-r--r--   0        0        0     8241 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/_constant.py
+-rw-r--r--   0        0        0    21727 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/_request_methods.py
+-rw-r--r--   0        0        0     2655 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/_typing.py
+-rw-r--r--   0        0        0      100 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/_version.py
+-rw-r--r--   0        0        0    38148 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/connection.py
+-rw-r--r--   0        0        0    76099 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/connectionpool.py
+-rw-r--r--   0        0        0     9988 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/exceptions.py
+-rw-r--r--   0        0        0     9151 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/fields.py
+-rw-r--r--   0        0        0     2202 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/filepost.py
+-rw-r--r--   0        0        0    36048 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/poolmanager.py
+-rw-r--r--   0        0        0       93 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/py.typed
+-rw-r--r--   0        0        0    35459 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/response.py
+-rw-r--r--   0        0        0        0 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/_async/__init__.py
+-rw-r--r--   0        0        0    36236 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/_async/connection.py
+-rw-r--r--   0        0        0    77884 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/_async/connectionpool.py
+-rw-r--r--   0        0        0    32214 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/_async/poolmanager.py
+-rw-r--r--   0        0        0    17222 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/_async/response.py
+-rw-r--r--   0        0        0      390 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/backend/__init__.py
+-rw-r--r--   0        0        0    16166 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/backend/_base.py
+-rw-r--r--   0        0        0    45773 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/backend/hface.py
+-rw-r--r--   0        0        0      225 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/backend/_async/__init__.py
+-rw-r--r--   0        0        0     5987 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/backend/_async/_base.py
+-rw-r--r--   0        0        0    43500 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/backend/_async/hface.py
+-rw-r--r--   0        0        0        0 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/__init__.py
+-rw-r--r--   0        0        0     4930 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/_socks_override.py
+-rw-r--r--   0        0        0      724 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    13565 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/socks.py
+-rw-r--r--   0        0        0     1185 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/hface/__init__.py
+-rw-r--r--   0        0        0     1775 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/hface/_configuration.py
+-rw-r--r--   0        0        0     1283 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/hface/_error_codes.py
+-rw-r--r--   0        0        0     3729 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/hface/_stream_matrix.py
+-rw-r--r--   0        0        0      877 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/hface/_typing.py
+-rw-r--r--   0        0        0        0 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/hface/py.typed
+-rw-r--r--   0        0        0     1161 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/hface/events/__init__.py
+-rw-r--r--   0        0        0     4497 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/hface/events/_events.py
+-rw-r--r--   0        0        0     1079 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/hface/protocols/__init__.py
+-rw-r--r--   0        0        0     4403 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/hface/protocols/_factories.py
+-rw-r--r--   0        0        0    10011 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/hface/protocols/_protocols.py
+-rw-r--r--   0        0        0      781 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/hface/protocols/http1/__init__.py
+-rw-r--r--   0        0        0    10477 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/hface/protocols/http1/_h11.py
+-rw-r--r--   0        0        0      780 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/hface/protocols/http2/__init__.py
+-rw-r--r--   0        0        0     9160 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/hface/protocols/http2/_h2.py
+-rw-r--r--   0        0        0      785 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/hface/protocols/http3/__init__.py
+-rw-r--r--   0        0        0    16858 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/hface/protocols/http3/_qh3.py
+-rw-r--r--   0        0        0     3314 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/imcc/__init__.py
+-rw-r--r--   0        0        0      293 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/__init__.py
+-rw-r--r--   0        0        0     8415 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/factories.py
+-rw-r--r--   0        0        0    18961 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/protocols.py
+-rw-r--r--   0        0        0     4290 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/utils.py
+-rw-r--r--   0        0        0      291 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/_async/__init__.py
+-rw-r--r--   0        0        0     7871 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/_async/factories.py
+-rw-r--r--   0        0        0    10621 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/_async/protocols.py
+-rw-r--r--   0        0        0      381 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/_async/doh/__init__.py
+-rw-r--r--   0        0        0    22371 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/_async/doh/_urllib3.py
+-rw-r--r--   0        0        0      338 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/_async/doq/__init__.py
+-rw-r--r--   0        0        0    15402 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/_async/doq/_qh3.py
+-rw-r--r--   0        0        0      329 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/_async/dot/__init__.py
+-rw-r--r--   0        0        0     5951 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/_async/dot/_ssl.py
+-rw-r--r--   0        0        0      292 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/_async/dou/__init__.py
+-rw-r--r--   0        0        0    11140 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/_async/dou/_socket.py
+-rw-r--r--   0        0        0      105 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/_async/in_memory/__init__.py
+-rw-r--r--   0        0        0     5299 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/_async/in_memory/_dict.py
+-rw-r--r--   0        0        0     2643 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/_async/null/__init__.py
+-rw-r--r--   0        0        0      103 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/_async/system/__init__.py
+-rw-r--r--   0        0        0     1770 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/_async/system/_socket.py
+-rw-r--r--   0        0        0      381 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/doh/__init__.py
+-rw-r--r--   0        0        0    22180 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/doh/_urllib3.py
+-rw-r--r--   0        0        0      338 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/doq/__init__.py
+-rw-r--r--   0        0        0    14846 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/doq/_qh3.py
+-rw-r--r--   0        0        0      329 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/dot/__init__.py
+-rw-r--r--   0        0        0     4493 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/dot/_ssl.py
+-rw-r--r--   0        0        0      292 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/dou/__init__.py
+-rw-r--r--   0        0        0    10836 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/dou/_socket.py
+-rw-r--r--   0        0        0      105 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/in_memory/__init__.py
+-rw-r--r--   0        0        0     5425 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/in_memory/_dict.py
+-rw-r--r--   0        0        0     2539 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/null/__init__.py
+-rw-r--r--   0        0        0      103 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/system/__init__.py
+-rw-r--r--   0        0        0     1626 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/system/_socket.py
+-rw-r--r--   0        0        0    12158 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/contrib/ssa/__init__.py
+-rw-r--r--   0        0        0      999 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/util/__init__.py
+-rw-r--r--   0        0        0     3884 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/util/connection.py
+-rw-r--r--   0        0        0     1145 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/util/proxy.py
+-rw-r--r--   0        0        0     8886 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/util/request.py
+-rw-r--r--   0        0        0     1329 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/util/response.py
+-rw-r--r--   0        0        0    19245 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/util/retry.py
+-rw-r--r--   0        0        0    24862 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/util/ssl_.py
+-rw-r--r--   0        0        0     5816 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     7226 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/util/ssltransport.py
+-rw-r--r--   0        0        0    10684 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/util/timeout.py
+-rw-r--r--   0        0        0    21813 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/util/traffic_police.py
+-rw-r--r--   0        0        0    15295 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/util/url.py
+-rw-r--r--   0        0        0     1146 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/util/util.py
+-rw-r--r--   0        0        0     4423 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/util/wait.py
+-rw-r--r--   0        0        0        0 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/util/_async/__init__.py
+-rw-r--r--   0        0        0     5492 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/util/_async/ssl_.py
+-rw-r--r--   0        0        0    22078 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/src/urllib3_future/util/_async/traffic_police.py
+-rw-r--r--   0        0        0     9646 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/__init__.py
+-rw-r--r--   0        0        0    11926 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/conftest.py
+-rw-r--r--   0        0        0     6222 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/port_helpers.py
+-rw-r--r--   0        0        0    12638 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/test_collections.py
+-rw-r--r--   0        0        0      692 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/test_compatibility.py
+-rw-r--r--   0        0        0    10288 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/test_connection.py
+-rw-r--r--   0        0        0    22649 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/test_connectionpool.py
+-rw-r--r--   0        0        0     1531 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/test_exceptions.py
+-rw-r--r--   0        0        0     3882 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/test_fields.py
+-rw-r--r--   0        0        0     3778 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/test_filepost.py
+-rw-r--r--   0        0        0      978 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/test_no_ssl.py
+-rw-r--r--   0        0        0    17951 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/test_poolmanager.py
+-rw-r--r--   0        0        0     3657 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/test_proxymanager.py
+-rw-r--r--   0        0        0    38863 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/test_response.py
+-rw-r--r--   0        0        0    16640 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/test_retry.py
+-rw-r--r--   0        0        0     6554 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/test_ssl.py
+-rw-r--r--   0        0        0    16917 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/test_ssltransport.py
+-rw-r--r--   0        0        0    43037 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/test_util.py
+-rw-r--r--   0        0        0     5999 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/test_wait.py
+-rw-r--r--   0        0        0     1187 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/tz_stub.py
+-rw-r--r--   0        0        0        0 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/contrib/__init__.py
+-rw-r--r--   0        0        0     1257 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/contrib/duplicate_san.pem
+-rw-r--r--   0        0        0    21281 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/contrib/test_resolver.py
+-rw-r--r--   0        0        0    25922 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/contrib/test_socks.py
+-rw-r--r--   0        0        0        0 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/contrib/asynchronous/__init__.py
+-rw-r--r--   0        0        0    21291 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/contrib/asynchronous/test_resolver.py
+-rw-r--r--   0        0        0    21728 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/contrib/asynchronous/test_socks.py
+-rw-r--r--   0        0        0        0 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/contrib/hface/__init__.py
+-rw-r--r--   0        0        0     3717 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/contrib/hface/test_stream_matrix.py
+-rw-r--r--   0        0        0        0 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_dummyserver/__init__.py
+-rw-r--r--   0        0        0     9840 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_dummyserver/test_chunked_transfer.py
+-rw-r--r--   0        0        0     3702 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_dummyserver/test_connection.py
+-rw-r--r--   0        0        0    56059 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_dummyserver/test_connectionpool.py
+-rw-r--r--   0        0        0     7756 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_dummyserver/test_happy_eyeballs.py
+-rw-r--r--   0        0        0    43193 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_dummyserver/test_https.py
+-rw-r--r--   0        0        0     1104 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_dummyserver/test_no_ssl.py
+-rw-r--r--   0        0        0    23853 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_dummyserver/test_poolmanager.py
+-rw-r--r--   0        0        0    32501 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_dummyserver/test_proxy_poolmanager.py
+-rw-r--r--   0        0        0    88179 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_dummyserver/test_socketlevel.py
+-rw-r--r--   0        0        0        0 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_dummyserver/asynchronous/__init__.py
+-rw-r--r--   0        0        0    59408 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_dummyserver/asynchronous/test_connectionpool.py
+-rw-r--r--   0        0        0     7329 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_dummyserver/asynchronous/test_happy_eyeballs.py
+-rw-r--r--   0        0        0    19562 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_dummyserver/asynchronous/test_poolmanager.py
+-rw-r--r--   0        0        0     2837 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_traefik/__init__.py
+-rw-r--r--   0        0        0     3069 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_traefik/test_conn_info.py
+-rw-r--r--   0        0        0     4873 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_traefik/test_connection.py
+-rw-r--r--   0        0        0     2821 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_traefik/test_connection_multiplexed.py
+-rw-r--r--   0        0        0     5912 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_traefik/test_connectionpool_multiplexed.py
+-rw-r--r--   0        0        0     3357 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_traefik/test_protolevel.py
+-rw-r--r--   0        0        0     3209 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_traefik/test_proxy.py
+-rw-r--r--   0        0        0     5622 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_traefik/test_send_data.py
+-rw-r--r--   0        0        0     1864 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_traefik/test_stream.py
+-rw-r--r--   0        0        0     6683 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_traefik/test_svn.py
+-rw-r--r--   0        0        0        0 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_traefik/asynchronous/__init__.py
+-rw-r--r--   0        0        0     2217 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_traefik/asynchronous/test_conn_info.py
+-rw-r--r--   0        0        0     5177 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_traefik/asynchronous/test_connection.py
+-rw-r--r--   0        0        0     3122 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_traefik/asynchronous/test_connection_multiplexed.py
+-rw-r--r--   0        0        0     6143 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_traefik/asynchronous/test_connectionpool_multiplexed.py
+-rw-r--r--   0        0        0     3481 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_traefik/asynchronous/test_protolevel.py
+-rw-r--r--   0        0        0     3274 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_traefik/asynchronous/test_proxy.py
+-rw-r--r--   0        0        0     5844 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_traefik/asynchronous/test_send_data.py
+-rw-r--r--   0        0        0     1967 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_traefik/asynchronous/test_stream.py
+-rw-r--r--   0        0        0     7217 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/test/with_traefik/asynchronous/test_svn.py
+-rw-r--r--   0        0        0       85 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/.gitignore
+-rw-r--r--   0        0        0     1093 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/LICENSE.txt
+-rw-r--r--   0        0        0     4277 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/README.md
+-rw-r--r--   0        0        0     1342 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/hatch_build.py
+-rw-r--r--   0        0        0     5698 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/pyproject.toml
+-rw-r--r--   0        0        0     7087 2024-05-31 03:52:38.000000 urllib3_future-2.7.913/PKG-INFO
```

### Comparing `urllib3_future-2.7.912/CHANGES.rst` & `urllib3_future-2.7.913/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+2.7.913 (2024-05-31)
+====================
+
+- Relaxed constraints around ``HTTPConnectionPool._new_conn`` private method in order to ensure a broader compatibility. (#122)
+
 2.7.912 (2024-05-27)
 ====================
 
 - Fixed unset ``tls_version`` within ``ConnectionInfo`` when using the legacy TLSv1 protocol.
 - Fixed license metadata SPDX in package.
 - Fixed custom ssl context with ``OP_NO_TLSv1_3`` option that did not disable HTTP/3.
 - Fixed custom ssl context with ``assert_hostname=False`` parameter not forwarded to QUIC configuration.
```

### Comparing `urllib3_future-2.7.912/docs/Makefile` & `urllib3_future-2.7.913/docs/Makefile`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/docs/advanced-usage.rst` & `urllib3_future-2.7.913/docs/advanced-usage.rst`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/docs/async.rst` & `urllib3_future-2.7.913/docs/async.rst`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/docs/conf.py` & `urllib3_future-2.7.913/docs/conf.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/docs/contributing.rst` & `urllib3_future-2.7.913/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/docs/index.rst` & `urllib3_future-2.7.913/docs/index.rst`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/docs/make.bat` & `urllib3_future-2.7.913/docs/make.bat`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/docs/user-guide.rst` & `urllib3_future-2.7.913/docs/user-guide.rst`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/docs/v2-migration-guide.rst` & `urllib3_future-2.7.913/docs/v2-migration-guide.rst`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/docs/_static/banner.svg` & `urllib3_future-2.7.913/docs/_static/banner.svg`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/docs/_static/banner_github.svg` & `urllib3_future-2.7.913/docs/_static/banner_github.svg`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/docs/_static/dark-logo.svg` & `urllib3_future-2.7.913/docs/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/docs/_static/logo.png` & `urllib3_future-2.7.913/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/docs/images/demo-button.png` & `urllib3_future-2.7.913/docs/images/demo-button.png`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/docs/images/favicon.png` & `urllib3_future-2.7.913/docs/images/favicon.png`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/docs/images/learn-more-button.png` & `urllib3_future-2.7.913/docs/images/learn-more-button.png`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/docs/images/logo.png` & `urllib3_future-2.7.913/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/docs/images/logo.svg` & `urllib3_future-2.7.913/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/docs/reference/urllib3.connectionpool.rst` & `urllib3_future-2.7.913/docs/reference/urllib3.connectionpool.rst`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/docs/reference/urllib3.poolmanager.rst` & `urllib3_future-2.7.913/docs/reference/urllib3.poolmanager.rst`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/docs/reference/urllib3.response.rst` & `urllib3_future-2.7.913/docs/reference/urllib3.response.rst`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/dummyserver/handlers.py` & `urllib3_future-2.7.913/dummyserver/handlers.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/dummyserver/https_proxy.py` & `urllib3_future-2.7.913/dummyserver/https_proxy.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/dummyserver/proxy.py` & `urllib3_future-2.7.913/dummyserver/proxy.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/dummyserver/server.py` & `urllib3_future-2.7.913/dummyserver/server.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/dummyserver/testcase.py` & `urllib3_future-2.7.913/dummyserver/testcase.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/dummyserver/certs/cacert.key` & `urllib3_future-2.7.913/dummyserver/certs/cacert.key`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/dummyserver/certs/cacert.pem` & `urllib3_future-2.7.913/dummyserver/certs/cacert.pem`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/dummyserver/certs/server.crt` & `urllib3_future-2.7.913/dummyserver/certs/server.crt`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/dummyserver/certs/server.key` & `urllib3_future-2.7.913/dummyserver/certs/server.key`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/__init__.py` & `urllib3_future-2.7.913/src/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/_collections.py` & `urllib3_future-2.7.913/src/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/_constant.py` & `urllib3_future-2.7.913/src/urllib3/_constant.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/_request_methods.py` & `urllib3_future-2.7.913/src/urllib3/_request_methods.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/_typing.py` & `urllib3_future-2.7.913/src/urllib3/_typing.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/connection.py` & `urllib3_future-2.7.913/src/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/connectionpool.py` & `urllib3_future-2.7.913/src/urllib3/connectionpool.py`

 * *Files 1% similar despite different names*

```diff
@@ -523,15 +523,24 @@
             pass  # Oh well, we'll create a new connection then
 
         # If this is a persistent connection, check if it got disconnected
         if conn and is_connection_dropped(conn):
             log.debug("Resetting dropped connection: %s", self.host)
             conn.close()
 
-        return conn or self._new_conn(heb_timeout=heb_timeout)
+        try:
+            return conn or self._new_conn(heb_timeout=heb_timeout)
+        except (
+            TypeError
+        ):  # this branch catch overridden pool that don't support Happy-Eyeballs!
+            conn = self._new_conn()
+            # as this branch is meant for people bypassing our main logic, we have to memorize the conn immediately
+            # into our pool of conn.
+            self.pool.put(conn, immediately_unavailable=True)
+            return conn
 
     def _put_conn(self, conn: HTTPConnection) -> None:
         """
         Put a connection back into the pool.
 
         :param conn:
             Connection object for the current host and port as returned by
```

### Comparing `urllib3_future-2.7.912/src/urllib3/exceptions.py` & `urllib3_future-2.7.913/src/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/fields.py` & `urllib3_future-2.7.913/src/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/filepost.py` & `urllib3_future-2.7.913/src/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/poolmanager.py` & `urllib3_future-2.7.913/src/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/response.py` & `urllib3_future-2.7.913/src/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/_async/connection.py` & `urllib3_future-2.7.913/src/urllib3/_async/connection.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/_async/connectionpool.py` & `urllib3_future-2.7.913/src/urllib3/_async/connectionpool.py`

 * *Files 0% similar despite different names*

```diff
@@ -533,15 +533,24 @@
             pass  # Oh well, we'll create a new connection then
 
         # If this is a persistent connection, check if it got disconnected
         if conn and is_connection_dropped(conn):
             log.debug("Resetting dropped connection: %s", self.host)
             await conn.close()
 
-        return conn or await self._new_conn(heb_timeout=heb_timeout)
+        try:
+            return conn or await self._new_conn(heb_timeout=heb_timeout)
+        except (
+            TypeError
+        ):  # this branch catch overridden pool that don't support Happy-Eyeballs!
+            conn = await self._new_conn()
+            # as this branch is meant for people bypassing our main logic, we have to memorize the conn immediately
+            # into our pool of conn.
+            await self.pool.put(conn, immediately_unavailable=True)
+            return conn
 
     async def _put_conn(self, conn: AsyncHTTPConnection) -> None:
         """
         Put a connection back into the pool.
 
         :param conn:
             Connection object for the current host and port as returned by
```

### Comparing `urllib3_future-2.7.912/src/urllib3/_async/poolmanager.py` & `urllib3_future-2.7.913/src/urllib3/_async/poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/_async/response.py` & `urllib3_future-2.7.913/src/urllib3/_async/response.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/backend/_base.py` & `urllib3_future-2.7.913/src/urllib3/backend/_base.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/backend/hface.py` & `urllib3_future-2.7.913/src/urllib3/backend/hface.py`

 * *Files 1% similar despite different names*

```diff
@@ -865,14 +865,18 @@
         *,
         encode_chunked: bool = False,
         expect_body_afterward: bool = False,
     ) -> ResponsePromise | None:
         if self.sock is None:
             self.connect()  # type: ignore[attr-defined]
 
+        # some libraries override connect(), thus bypassing our state machine initialization.
+        if self._protocol is None:
+            self._post_conn()
+
         assert self.sock is not None and self._protocol is not None
 
         # only h2 and h3 support streams, it is faked/simulated for h1.
         self._stream_id = self._protocol.get_available_stream_id()
         # unless anything hint the opposite, the request head frame is the end stream
         should_end_stream: bool = expect_body_afterward is False
```

### Comparing `urllib3_future-2.7.912/src/urllib3/backend/_async/_base.py` & `urllib3_future-2.7.913/src/urllib3/backend/_async/_base.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/backend/_async/hface.py` & `urllib3_future-2.7.913/src/urllib3/backend/_async/hface.py`

 * *Files 1% similar despite different names*

```diff
@@ -803,14 +803,18 @@
         *,
         encode_chunked: bool = False,
         expect_body_afterward: bool = False,
     ) -> ResponsePromise | None:
         if self.sock is None:
             await self.connect()  # type: ignore[attr-defined]
 
+        # some libraries override connect(), thus bypassing our state machine initialization.
+        if self._protocol is None:
+            await self._post_conn()
+
         assert self.sock is not None and self._protocol is not None
 
         # only h2 and h3 support streams, it is faked/simulated for h1.
         self._stream_id = self._protocol.get_available_stream_id()
         # unless anything hint the opposite, the request head frame is the end stream
         should_end_stream: bool = expect_body_afterward is False
```

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/_socks_override.py` & `urllib3_future-2.7.913/src/urllib3/contrib/_socks_override.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/pyopenssl.py` & `urllib3_future-2.7.913/src/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/socks.py` & `urllib3_future-2.7.913/src/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/hface/__init__.py` & `urllib3_future-2.7.913/src/urllib3/contrib/hface/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/hface/_configuration.py` & `urllib3_future-2.7.913/src/urllib3/contrib/hface/_configuration.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/hface/_error_codes.py` & `urllib3_future-2.7.913/src/urllib3/contrib/hface/_error_codes.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/hface/_stream_matrix.py` & `urllib3_future-2.7.913/src/urllib3/contrib/hface/_stream_matrix.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/hface/_typing.py` & `urllib3_future-2.7.913/src/urllib3/contrib/hface/_typing.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/hface/events/__init__.py` & `urllib3_future-2.7.913/src/urllib3/contrib/hface/events/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/hface/events/_events.py` & `urllib3_future-2.7.913/src/urllib3/contrib/hface/events/_events.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/hface/protocols/__init__.py` & `urllib3_future-2.7.913/src/urllib3/contrib/hface/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/hface/protocols/_factories.py` & `urllib3_future-2.7.913/src/urllib3/contrib/hface/protocols/_factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/hface/protocols/_protocols.py` & `urllib3_future-2.7.913/src/urllib3/contrib/hface/protocols/_protocols.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/hface/protocols/http1/__init__.py` & `urllib3_future-2.7.913/src/urllib3/contrib/hface/protocols/http1/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/hface/protocols/http1/_h11.py` & `urllib3_future-2.7.913/src/urllib3/contrib/hface/protocols/http1/_h11.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/hface/protocols/http2/__init__.py` & `urllib3_future-2.7.913/src/urllib3/contrib/hface/protocols/http2/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/hface/protocols/http2/_h2.py` & `urllib3_future-2.7.913/src/urllib3/contrib/hface/protocols/http2/_h2.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/hface/protocols/http3/__init__.py` & `urllib3_future-2.7.913/src/urllib3/contrib/hface/protocols/http3/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/hface/protocols/http3/_qh3.py` & `urllib3_future-2.7.913/src/urllib3/contrib/hface/protocols/http3/_qh3.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/imcc/__init__.py` & `urllib3_future-2.7.913/src/urllib3/contrib/imcc/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/resolver/factories.py` & `urllib3_future-2.7.913/src/urllib3/contrib/resolver/factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/resolver/protocols.py` & `urllib3_future-2.7.913/src/urllib3/contrib/resolver/protocols.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/resolver/utils.py` & `urllib3_future-2.7.913/src/urllib3/contrib/resolver/utils.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/resolver/_async/factories.py` & `urllib3_future-2.7.913/src/urllib3/contrib/resolver/_async/factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/resolver/_async/protocols.py` & `urllib3_future-2.7.913/src/urllib3/contrib/resolver/_async/protocols.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/resolver/_async/doh/_urllib3.py` & `urllib3_future-2.7.913/src/urllib3/contrib/resolver/_async/doh/_urllib3.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/resolver/_async/doq/_qh3.py` & `urllib3_future-2.7.913/src/urllib3/contrib/resolver/_async/doq/_qh3.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/resolver/_async/dot/_ssl.py` & `urllib3_future-2.7.913/src/urllib3/contrib/resolver/_async/dot/_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/resolver/_async/dou/_socket.py` & `urllib3_future-2.7.913/src/urllib3/contrib/resolver/_async/dou/_socket.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/resolver/_async/in_memory/_dict.py` & `urllib3_future-2.7.913/src/urllib3/contrib/resolver/_async/in_memory/_dict.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/resolver/_async/null/__init__.py` & `urllib3_future-2.7.913/src/urllib3/contrib/resolver/_async/null/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/resolver/_async/system/_socket.py` & `urllib3_future-2.7.913/src/urllib3/contrib/resolver/_async/system/_socket.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/resolver/doh/_urllib3.py` & `urllib3_future-2.7.913/src/urllib3/contrib/resolver/doh/_urllib3.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/resolver/doq/_qh3.py` & `urllib3_future-2.7.913/src/urllib3/contrib/resolver/doq/_qh3.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/resolver/dot/_ssl.py` & `urllib3_future-2.7.913/src/urllib3/contrib/resolver/dot/_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/resolver/dou/_socket.py` & `urllib3_future-2.7.913/src/urllib3/contrib/resolver/dou/_socket.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/resolver/in_memory/_dict.py` & `urllib3_future-2.7.913/src/urllib3/contrib/resolver/in_memory/_dict.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/resolver/null/__init__.py` & `urllib3_future-2.7.913/src/urllib3/contrib/resolver/null/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/resolver/system/_socket.py` & `urllib3_future-2.7.913/src/urllib3/contrib/resolver/system/_socket.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/contrib/ssa/__init__.py` & `urllib3_future-2.7.913/src/urllib3/contrib/ssa/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/util/__init__.py` & `urllib3_future-2.7.913/src/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/util/connection.py` & `urllib3_future-2.7.913/src/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/util/proxy.py` & `urllib3_future-2.7.913/src/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/util/request.py` & `urllib3_future-2.7.913/src/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/util/response.py` & `urllib3_future-2.7.913/src/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/util/retry.py` & `urllib3_future-2.7.913/src/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/util/ssl_.py` & `urllib3_future-2.7.913/src/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/util/ssl_match_hostname.py` & `urllib3_future-2.7.913/src/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/util/ssltransport.py` & `urllib3_future-2.7.913/src/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/util/timeout.py` & `urllib3_future-2.7.913/src/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/util/traffic_police.py` & `urllib3_future-2.7.913/src/urllib3/util/traffic_police.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/util/url.py` & `urllib3_future-2.7.913/src/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/util/util.py` & `urllib3_future-2.7.913/src/urllib3/util/util.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/util/wait.py` & `urllib3_future-2.7.913/src/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/util/_async/ssl_.py` & `urllib3_future-2.7.913/src/urllib3/util/_async/ssl_.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3/util/_async/traffic_police.py` & `urllib3_future-2.7.913/src/urllib3/util/_async/traffic_police.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/__init__.py` & `urllib3_future-2.7.913/src/urllib3_future/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/_collections.py` & `urllib3_future-2.7.913/src/urllib3_future/_collections.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/_constant.py` & `urllib3_future-2.7.913/src/urllib3_future/_constant.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/_request_methods.py` & `urllib3_future-2.7.913/src/urllib3_future/_request_methods.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/_typing.py` & `urllib3_future-2.7.913/src/urllib3_future/_typing.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/connection.py` & `urllib3_future-2.7.913/src/urllib3_future/connection.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/connectionpool.py` & `urllib3_future-2.7.913/src/urllib3_future/connectionpool.py`

 * *Files 1% similar despite different names*

```diff
@@ -523,15 +523,24 @@
             pass  # Oh well, we'll create a new connection then
 
         # If this is a persistent connection, check if it got disconnected
         if conn and is_connection_dropped(conn):
             log.debug("Resetting dropped connection: %s", self.host)
             conn.close()
 
-        return conn or self._new_conn(heb_timeout=heb_timeout)
+        try:
+            return conn or self._new_conn(heb_timeout=heb_timeout)
+        except (
+            TypeError
+        ):  # this branch catch overridden pool that don't support Happy-Eyeballs!
+            conn = self._new_conn()
+            # as this branch is meant for people bypassing our main logic, we have to memorize the conn immediately
+            # into our pool of conn.
+            self.pool.put(conn, immediately_unavailable=True)
+            return conn
 
     def _put_conn(self, conn: HTTPConnection) -> None:
         """
         Put a connection back into the pool.
 
         :param conn:
             Connection object for the current host and port as returned by
```

### Comparing `urllib3_future-2.7.912/src/urllib3_future/exceptions.py` & `urllib3_future-2.7.913/src/urllib3_future/exceptions.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/fields.py` & `urllib3_future-2.7.913/src/urllib3_future/fields.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/filepost.py` & `urllib3_future-2.7.913/src/urllib3_future/filepost.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/poolmanager.py` & `urllib3_future-2.7.913/src/urllib3_future/poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/response.py` & `urllib3_future-2.7.913/src/urllib3_future/response.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/_async/connection.py` & `urllib3_future-2.7.913/src/urllib3_future/_async/connection.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/_async/connectionpool.py` & `urllib3_future-2.7.913/src/urllib3_future/_async/connectionpool.py`

 * *Files 0% similar despite different names*

```diff
@@ -533,15 +533,24 @@
             pass  # Oh well, we'll create a new connection then
 
         # If this is a persistent connection, check if it got disconnected
         if conn and is_connection_dropped(conn):
             log.debug("Resetting dropped connection: %s", self.host)
             await conn.close()
 
-        return conn or await self._new_conn(heb_timeout=heb_timeout)
+        try:
+            return conn or await self._new_conn(heb_timeout=heb_timeout)
+        except (
+            TypeError
+        ):  # this branch catch overridden pool that don't support Happy-Eyeballs!
+            conn = await self._new_conn()
+            # as this branch is meant for people bypassing our main logic, we have to memorize the conn immediately
+            # into our pool of conn.
+            await self.pool.put(conn, immediately_unavailable=True)
+            return conn
 
     async def _put_conn(self, conn: AsyncHTTPConnection) -> None:
         """
         Put a connection back into the pool.
 
         :param conn:
             Connection object for the current host and port as returned by
```

### Comparing `urllib3_future-2.7.912/src/urllib3_future/_async/poolmanager.py` & `urllib3_future-2.7.913/src/urllib3_future/_async/poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/_async/response.py` & `urllib3_future-2.7.913/src/urllib3_future/_async/response.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/backend/_base.py` & `urllib3_future-2.7.913/src/urllib3_future/backend/_base.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/backend/hface.py` & `urllib3_future-2.7.913/src/urllib3_future/backend/hface.py`

 * *Files 1% similar despite different names*

```diff
@@ -865,14 +865,18 @@
         *,
         encode_chunked: bool = False,
         expect_body_afterward: bool = False,
     ) -> ResponsePromise | None:
         if self.sock is None:
             self.connect()  # type: ignore[attr-defined]
 
+        # some libraries override connect(), thus bypassing our state machine initialization.
+        if self._protocol is None:
+            self._post_conn()
+
         assert self.sock is not None and self._protocol is not None
 
         # only h2 and h3 support streams, it is faked/simulated for h1.
         self._stream_id = self._protocol.get_available_stream_id()
         # unless anything hint the opposite, the request head frame is the end stream
         should_end_stream: bool = expect_body_afterward is False
```

### Comparing `urllib3_future-2.7.912/src/urllib3_future/backend/_async/_base.py` & `urllib3_future-2.7.913/src/urllib3_future/backend/_async/_base.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/backend/_async/hface.py` & `urllib3_future-2.7.913/src/urllib3_future/backend/_async/hface.py`

 * *Files 1% similar despite different names*

```diff
@@ -803,14 +803,18 @@
         *,
         encode_chunked: bool = False,
         expect_body_afterward: bool = False,
     ) -> ResponsePromise | None:
         if self.sock is None:
             await self.connect()  # type: ignore[attr-defined]
 
+        # some libraries override connect(), thus bypassing our state machine initialization.
+        if self._protocol is None:
+            await self._post_conn()
+
         assert self.sock is not None and self._protocol is not None
 
         # only h2 and h3 support streams, it is faked/simulated for h1.
         self._stream_id = self._protocol.get_available_stream_id()
         # unless anything hint the opposite, the request head frame is the end stream
         should_end_stream: bool = expect_body_afterward is False
```

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/_socks_override.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/_socks_override.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/pyopenssl.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/socks.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/hface/__init__.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/hface/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/hface/_configuration.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/hface/_configuration.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/hface/_error_codes.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/hface/_error_codes.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/hface/_stream_matrix.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/hface/_stream_matrix.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/hface/_typing.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/hface/_typing.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/hface/events/__init__.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/hface/events/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/hface/events/_events.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/hface/events/_events.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/hface/protocols/__init__.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/hface/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/hface/protocols/_factories.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/hface/protocols/_factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/hface/protocols/_protocols.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/hface/protocols/_protocols.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/hface/protocols/http1/__init__.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/hface/protocols/http1/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/hface/protocols/http1/_h11.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/hface/protocols/http1/_h11.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/hface/protocols/http2/__init__.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/hface/protocols/http2/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/hface/protocols/http2/_h2.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/hface/protocols/http2/_h2.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/hface/protocols/http3/__init__.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/hface/protocols/http3/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/hface/protocols/http3/_qh3.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/hface/protocols/http3/_qh3.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/imcc/__init__.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/imcc/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/factories.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/protocols.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/protocols.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/utils.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/utils.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/_async/factories.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/_async/factories.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/_async/protocols.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/_async/protocols.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/_async/doh/_urllib3.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/_async/doh/_urllib3.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/_async/doq/_qh3.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/_async/doq/_qh3.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/_async/dot/_ssl.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/_async/dot/_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/_async/dou/_socket.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/_async/dou/_socket.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/_async/in_memory/_dict.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/_async/in_memory/_dict.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/_async/null/__init__.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/_async/null/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/_async/system/_socket.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/_async/system/_socket.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/doh/_urllib3.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/doh/_urllib3.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/doq/_qh3.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/doq/_qh3.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/dot/_ssl.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/dot/_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/dou/_socket.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/dou/_socket.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/in_memory/_dict.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/in_memory/_dict.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/null/__init__.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/null/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/resolver/system/_socket.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/resolver/system/_socket.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/contrib/ssa/__init__.py` & `urllib3_future-2.7.913/src/urllib3_future/contrib/ssa/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/util/__init__.py` & `urllib3_future-2.7.913/src/urllib3_future/util/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/util/connection.py` & `urllib3_future-2.7.913/src/urllib3_future/util/connection.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/util/proxy.py` & `urllib3_future-2.7.913/src/urllib3_future/util/proxy.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/util/request.py` & `urllib3_future-2.7.913/src/urllib3_future/util/request.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/util/response.py` & `urllib3_future-2.7.913/src/urllib3_future/util/response.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/util/retry.py` & `urllib3_future-2.7.913/src/urllib3_future/util/retry.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/util/ssl_.py` & `urllib3_future-2.7.913/src/urllib3_future/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/util/ssl_match_hostname.py` & `urllib3_future-2.7.913/src/urllib3_future/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/util/ssltransport.py` & `urllib3_future-2.7.913/src/urllib3_future/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/util/timeout.py` & `urllib3_future-2.7.913/src/urllib3_future/util/timeout.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/util/traffic_police.py` & `urllib3_future-2.7.913/src/urllib3_future/util/traffic_police.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/util/url.py` & `urllib3_future-2.7.913/src/urllib3_future/util/url.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/util/util.py` & `urllib3_future-2.7.913/src/urllib3_future/util/util.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/util/wait.py` & `urllib3_future-2.7.913/src/urllib3_future/util/wait.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/util/_async/ssl_.py` & `urllib3_future-2.7.913/src/urllib3_future/util/_async/ssl_.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/src/urllib3_future/util/_async/traffic_police.py` & `urllib3_future-2.7.913/src/urllib3_future/util/_async/traffic_police.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/__init__.py` & `urllib3_future-2.7.913/test/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/conftest.py` & `urllib3_future-2.7.913/test/conftest.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/port_helpers.py` & `urllib3_future-2.7.913/test/port_helpers.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/test_collections.py` & `urllib3_future-2.7.913/test/test_collections.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/test_compatibility.py` & `urllib3_future-2.7.913/test/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/test_connection.py` & `urllib3_future-2.7.913/test/test_connection.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/test_connectionpool.py` & `urllib3_future-2.7.913/test/test_connectionpool.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/test_exceptions.py` & `urllib3_future-2.7.913/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/test_fields.py` & `urllib3_future-2.7.913/test/test_fields.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/test_filepost.py` & `urllib3_future-2.7.913/test/test_filepost.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/test_no_ssl.py` & `urllib3_future-2.7.913/test/test_no_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/test_poolmanager.py` & `urllib3_future-2.7.913/test/test_poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/test_proxymanager.py` & `urllib3_future-2.7.913/test/test_proxymanager.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/test_response.py` & `urllib3_future-2.7.913/test/test_response.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/test_retry.py` & `urllib3_future-2.7.913/test/test_retry.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/test_ssl.py` & `urllib3_future-2.7.913/test/test_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/test_ssltransport.py` & `urllib3_future-2.7.913/test/test_ssltransport.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/test_util.py` & `urllib3_future-2.7.913/test/test_util.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/test_wait.py` & `urllib3_future-2.7.913/test/test_wait.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/tz_stub.py` & `urllib3_future-2.7.913/test/tz_stub.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/contrib/duplicate_san.pem` & `urllib3_future-2.7.913/test/contrib/duplicate_san.pem`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/contrib/test_resolver.py` & `urllib3_future-2.7.913/test/contrib/test_resolver.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/contrib/test_socks.py` & `urllib3_future-2.7.913/test/contrib/test_socks.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/contrib/asynchronous/test_resolver.py` & `urllib3_future-2.7.913/test/contrib/asynchronous/test_resolver.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/contrib/asynchronous/test_socks.py` & `urllib3_future-2.7.913/test/contrib/asynchronous/test_socks.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/contrib/hface/test_stream_matrix.py` & `urllib3_future-2.7.913/test/contrib/hface/test_stream_matrix.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_dummyserver/test_chunked_transfer.py` & `urllib3_future-2.7.913/test/with_dummyserver/test_chunked_transfer.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_dummyserver/test_connection.py` & `urllib3_future-2.7.913/test/with_dummyserver/test_connection.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_dummyserver/test_connectionpool.py` & `urllib3_future-2.7.913/test/with_dummyserver/test_connectionpool.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_dummyserver/test_happy_eyeballs.py` & `urllib3_future-2.7.913/test/with_dummyserver/test_happy_eyeballs.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_dummyserver/test_https.py` & `urllib3_future-2.7.913/test/with_dummyserver/test_https.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_dummyserver/test_no_ssl.py` & `urllib3_future-2.7.913/test/with_dummyserver/test_no_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_dummyserver/test_poolmanager.py` & `urllib3_future-2.7.913/test/with_dummyserver/test_poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_dummyserver/test_proxy_poolmanager.py` & `urllib3_future-2.7.913/test/with_dummyserver/test_proxy_poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_dummyserver/test_socketlevel.py` & `urllib3_future-2.7.913/test/with_dummyserver/test_socketlevel.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_dummyserver/asynchronous/test_connectionpool.py` & `urllib3_future-2.7.913/test/with_dummyserver/asynchronous/test_connectionpool.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_dummyserver/asynchronous/test_happy_eyeballs.py` & `urllib3_future-2.7.913/test/with_dummyserver/asynchronous/test_happy_eyeballs.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_dummyserver/asynchronous/test_poolmanager.py` & `urllib3_future-2.7.913/test/with_dummyserver/asynchronous/test_poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_traefik/__init__.py` & `urllib3_future-2.7.913/test/with_traefik/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_traefik/test_conn_info.py` & `urllib3_future-2.7.913/test/with_traefik/test_conn_info.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_traefik/test_connection.py` & `urllib3_future-2.7.913/test/with_traefik/test_connection.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_traefik/test_connection_multiplexed.py` & `urllib3_future-2.7.913/test/with_traefik/test_connection_multiplexed.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_traefik/test_connectionpool_multiplexed.py` & `urllib3_future-2.7.913/test/with_traefik/test_connectionpool_multiplexed.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_traefik/test_protolevel.py` & `urllib3_future-2.7.913/test/with_traefik/test_protolevel.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_traefik/test_proxy.py` & `urllib3_future-2.7.913/test/with_traefik/test_proxy.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_traefik/test_send_data.py` & `urllib3_future-2.7.913/test/with_traefik/test_send_data.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_traefik/test_stream.py` & `urllib3_future-2.7.913/test/with_traefik/test_stream.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_traefik/test_svn.py` & `urllib3_future-2.7.913/test/with_traefik/test_svn.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_traefik/asynchronous/test_conn_info.py` & `urllib3_future-2.7.913/test/with_traefik/asynchronous/test_conn_info.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_traefik/asynchronous/test_connection.py` & `urllib3_future-2.7.913/test/with_traefik/asynchronous/test_connection.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_traefik/asynchronous/test_connection_multiplexed.py` & `urllib3_future-2.7.913/test/with_traefik/asynchronous/test_connection_multiplexed.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_traefik/asynchronous/test_connectionpool_multiplexed.py` & `urllib3_future-2.7.913/test/with_traefik/asynchronous/test_connectionpool_multiplexed.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_traefik/asynchronous/test_protolevel.py` & `urllib3_future-2.7.913/test/with_traefik/asynchronous/test_protolevel.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_traefik/asynchronous/test_proxy.py` & `urllib3_future-2.7.913/test/with_traefik/asynchronous/test_proxy.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_traefik/asynchronous/test_send_data.py` & `urllib3_future-2.7.913/test/with_traefik/asynchronous/test_send_data.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_traefik/asynchronous/test_stream.py` & `urllib3_future-2.7.913/test/with_traefik/asynchronous/test_stream.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/test/with_traefik/asynchronous/test_svn.py` & `urllib3_future-2.7.913/test/with_traefik/asynchronous/test_svn.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/LICENSE.txt` & `urllib3_future-2.7.913/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/README.md` & `urllib3_future-2.7.913/README.md`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/hatch_build.py` & `urllib3_future-2.7.913/hatch_build.py`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/pyproject.toml` & `urllib3_future-2.7.913/pyproject.toml`

 * *Files identical despite different names*

### Comparing `urllib3_future-2.7.912/PKG-INFO` & `urllib3_future-2.7.913/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: urllib3-future
-Version: 2.7.912
+Version: 2.7.913
 Summary: urllib3.future is a powerful HTTP 1.1, 2, and 3 client with both sync and async interfaces
 Project-URL: Changelog, https://github.com/jawah/urllib3.future/blob/main/CHANGES.rst
 Project-URL: Documentation, https://urllib3future.readthedocs.io
 Project-URL: Code, https://github.com/jawah/urllib3.future
 Project-URL: Issue tracker, https://github.com/jawah/urllib3.future/issues
 Author-email: Andrey Petrov <andrey.petrov@shazow.net>
 Maintainer-email: "Ahmed R. TAHRI" <ahmed.tahri@cloudnursery.dev>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: urllib3-future Version: 2.7.912 Summary:
+Metadata-Version: 2.3 Name: urllib3-future Version: 2.7.913 Summary:
 urllib3.future is a powerful HTTP 1.1, 2, and 3 client with both sync and async
 interfaces Project-URL: Changelog, https://github.com/jawah/urllib3.future/
 blob/main/CHANGES.rst Project-URL: Documentation, https://
 urllib3future.readthedocs.io Project-URL: Code, https://github.com/jawah/
 urllib3.future Project-URL: Issue tracker, https://github.com/jawah/
 urllib3.future/issues Author-email: Andrey Petrov
 shazow.net> Maintainer-email: "Ahmed R. TAHRI"
```

