# Comparing `tmp/pinnacle_cli-0.0.1.tar.gz` & `tmp/pinnacle_cli-0.0.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinnacle_cli-0.0.1.tar", max compression
+gzip compressed data, was "pinnacle_cli-0.0.2a2.tar", max compression
```

## Comparing `pinnacle_cli-0.0.1.tar` & `pinnacle_cli-0.0.2a2.tar`

### file list

```diff
@@ -1,7 +1,757 @@
--rw-r--r--   0        0        0     2600 2024-05-29 17:20:05.770602 pinnacle_cli-0.0.1/README.md
--rw-r--r--   0        0        0        0 2024-05-29 17:20:05.770697 pinnacle_cli-0.0.1/pinnacle_cli/__init__.py
--rw-r--r--   0        0        0      185 2024-05-29 17:20:05.771088 pinnacle_cli-0.0.1/pinnacle_cli/constants.py
--rw-r--r--   0        0        0     1660 2024-05-29 17:20:05.771365 pinnacle_cli-0.0.1/pinnacle_cli/dev.py
--rw-r--r--   0        0        0      603 2024-05-29 17:20:05.771620 pinnacle_cli-0.0.1/pinnacle_cli/main.py
--rw-r--r--   0        0        0      431 2024-05-29 17:20:05.772982 pinnacle_cli-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2979 1970-01-01 00:00:00.000000 pinnacle_cli-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2600 2024-05-30 00:31:01.338936 pinnacle_cli-0.0.2a2/README.md
+-rw-r--r--   0        0        0        0 2024-05-30 00:31:01.339724 pinnacle_cli-0.0.2a2/pinnacle_cli/__init__.py
+-rw-r--r--   0        0        0      213 2024-05-30 20:22:31.035839 pinnacle_cli-0.0.2a2/pinnacle_cli/constants.py
+-rw-r--r--   0        0        0      311 2024-05-30 22:35:52.104750 pinnacle_cli-0.0.2a2/pinnacle_cli/js/constants.ts
+-rw-r--r--   0        0        0     1153 2024-05-31 00:28:58.305171 pinnacle_cli-0.0.2a2/pinnacle_cli/js/dev.ts
+-rw-r--r--   0        0        0    34433 2024-05-30 22:45:19.744914 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/.package-lock.json
+-rw-r--r--   0        0        0      145 2024-05-30 22:45:19.489025 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@esbuild/darwin-arm64/README.md
+-rwxr-xr-x   0        0        0  9774482 2024-05-30 22:45:19.488834 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@esbuild/darwin-arm64/bin/esbuild
+-rw-r--r--   0        0        0      382 2024-05-30 22:45:19.488992 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@esbuild/darwin-arm64/package.json
+-rw-r--r--   0        0        0     1141 2024-05-30 22:45:19.424746 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/body-parser/LICENSE
+-rw-r--r--   0        0        0      884 2024-05-30 22:45:19.430667 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/body-parser/README.md
+-rw-r--r--   0        0        0     3844 2024-05-30 22:45:19.435065 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/body-parser/index.d.ts
+-rw-r--r--   0        0        0     1779 2024-05-30 22:45:19.438103 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/body-parser/package.json
+-rw-r--r--   0        0        0     1141 2024-05-30 22:45:19.421823 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/connect/LICENSE
+-rw-r--r--   0        0        0      562 2024-05-30 22:45:19.428226 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/connect/README.md
+-rw-r--r--   0        0        0     3239 2024-05-30 22:45:19.434253 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/connect/index.d.ts
+-rw-r--r--   0        0        0      965 2024-05-30 22:45:19.437664 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/connect/package.json
+-rw-r--r--   0        0        0     1141 2024-05-30 22:45:19.421699 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/express/LICENSE
+-rw-r--r--   0        0        0      893 2024-05-30 22:45:19.428694 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/express/README.md
+-rw-r--r--   0        0        0     4414 2024-05-30 22:45:19.434394 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/express/index.d.ts
+-rw-r--r--   0        0        0     1415 2024-05-30 22:45:19.437739 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/express/package.json
+-rw-r--r--   0        0        0     1141 2024-05-30 22:45:19.428333 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/express-serve-static-core/LICENSE
+-rw-r--r--   0        0        0      928 2024-05-30 22:45:19.437849 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/express-serve-static-core/README.md
+-rw-r--r--   0        0        0    42555 2024-05-30 22:45:19.454680 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/express-serve-static-core/index.d.ts
+-rw-r--r--   0        0        0     1594 2024-05-30 22:45:19.457158 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/express-serve-static-core/package.json
+-rw-r--r--   0        0        0     1141 2024-05-30 22:45:19.420980 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/http-errors/LICENSE
+-rw-r--r--   0        0        0      537 2024-05-30 22:45:19.427751 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/http-errors/README.md
+-rw-r--r--   0        0        0     3946 2024-05-30 22:45:19.433915 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/http-errors/index.d.ts
+-rw-r--r--   0        0        0      963 2024-05-30 22:45:19.437346 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/http-errors/package.json
+-rw-r--r--   0        0        0     1141 2024-05-30 22:45:19.421501 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/mime/LICENSE
+-rw-r--r--   0        0        0      270 2024-05-30 22:45:19.427653 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/mime/Mime.d.ts
+-rw-r--r--   0        0        0      511 2024-05-30 22:45:19.433869 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/mime/README.md
+-rw-r--r--   0        0        0      812 2024-05-30 22:45:19.437223 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/mime/index.d.ts
+-rw-r--r--   0        0        0      124 2024-05-30 22:45:19.439943 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/mime/lite.d.ts
+-rw-r--r--   0        0        0      923 2024-05-30 22:45:19.442182 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/mime/package.json
+-rw-r--r--   0        0        0     1141 2024-05-30 22:45:19.421229 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/LICENSE
+-rw-r--r--   0        0        0     2289 2024-05-30 22:45:19.428002 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/README.md
+-rw-r--r--   0        0        0      201 2024-05-30 22:45:19.479642 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/assert/strict.d.ts
+-rw-r--r--   0        0        0    43823 2024-05-30 22:45:19.442253 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/assert.d.ts
+-rw-r--r--   0        0        0    23283 2024-05-30 22:45:19.449290 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/async_hooks.d.ts
+-rw-r--r--   0        0        0   107508 2024-05-30 22:45:19.458459 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/buffer.d.ts
+-rw-r--r--   0        0        0    69699 2024-05-30 22:45:19.461907 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/child_process.d.ts
+-rw-r--r--   0        0        0    28015 2024-05-30 22:45:19.463022 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/cluster.d.ts
+-rw-r--r--   0        0        0    21246 2024-05-30 22:45:19.463756 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/console.d.ts
+-rw-r--r--   0        0        0      623 2024-05-30 22:45:19.464652 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/constants.d.ts
+-rw-r--r--   0        0        0   193135 2024-05-30 22:45:19.468719 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/crypto.d.ts
+-rw-r--r--   0        0        0    27772 2024-05-30 22:45:19.469160 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/dgram.d.ts
+-rw-r--r--   0        0        0    24065 2024-05-30 22:45:19.469342 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/diagnostics_channel.d.ts
+-rw-r--r--   0        0        0    20522 2024-05-30 22:45:19.479828 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/dns/promises.d.ts
+-rw-r--r--   0        0        0    35577 2024-05-30 22:45:19.469667 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/dns.d.ts
+-rw-r--r--   0        0        0     5871 2024-05-30 22:45:19.469964 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/dom-events.d.ts
+-rw-r--r--   0        0        0     7825 2024-05-30 22:45:19.470116 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/domain.d.ts
+-rw-r--r--   0        0        0    42205 2024-05-30 22:45:19.470294 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/events.d.ts
+-rw-r--r--   0        0        0    54679 2024-05-30 22:45:19.480185 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/fs/promises.d.ts
+-rw-r--r--   0        0        0   187489 2024-05-30 22:45:19.471528 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/fs.d.ts
+-rw-r--r--   0        0        0    14300 2024-05-30 22:45:19.471710 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/globals.d.ts
+-rw-r--r--   0        0        0       39 2024-05-30 22:45:19.471965 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/globals.global.d.ts
+-rw-r--r--   0        0        0    85267 2024-05-30 22:45:19.472243 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/http.d.ts
+-rw-r--r--   0        0        0   118661 2024-05-30 22:45:19.472661 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/http2.d.ts
+-rw-r--r--   0        0        0    24892 2024-05-30 22:45:19.472896 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/https.d.ts
+-rw-r--r--   0        0        0     3774 2024-05-30 22:45:19.473039 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/index.d.ts
+-rw-r--r--   0        0        0   125328 2024-05-30 22:45:19.473370 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/inspector.d.ts
+-rw-r--r--   0        0        0    13783 2024-05-30 22:45:19.473521 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/module.d.ts
+-rw-r--r--   0        0        0    46246 2024-05-30 22:45:19.473739 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/net.d.ts
+-rw-r--r--   0        0        0    18963 2024-05-30 22:45:19.473940 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/os.d.ts
+-rw-r--r--   0        0        0     6527 2024-05-30 22:45:19.474150 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/package.json
+-rw-r--r--   0        0        0     7752 2024-05-30 22:45:19.474280 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/path.d.ts
+-rw-r--r--   0        0        0    35856 2024-05-30 22:45:19.474600 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/perf_hooks.d.ts
+-rw-r--r--   0        0        0    87273 2024-05-30 22:45:19.474867 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/process.d.ts
+-rw-r--r--   0        0        0     5482 2024-05-30 22:45:19.475084 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/punycode.d.ts
+-rw-r--r--   0        0        0     7145 2024-05-30 22:45:19.475311 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/querystring.d.ts
+-rw-r--r--   0        0        0     6126 2024-05-30 22:45:19.480441 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/readline/promises.d.ts
+-rw-r--r--   0        0        0    23488 2024-05-30 22:45:19.475466 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/readline.d.ts
+-rw-r--r--   0        0        0    19527 2024-05-30 22:45:19.475751 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/repl.d.ts
+-rw-r--r--   0        0        0     6207 2024-05-30 22:45:19.475941 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/sea.d.ts
+-rw-r--r--   0        0        0      727 2024-05-30 22:45:19.480647 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/stream/consumers.d.ts
+-rw-r--r--   0        0        0     2696 2024-05-30 22:45:19.480749 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/stream/promises.d.ts
+-rw-r--r--   0        0        0    15132 2024-05-30 22:45:19.480895 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/stream/web.d.ts
+-rw-r--r--   0        0        0    83675 2024-05-30 22:45:19.476105 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/stream.d.ts
+-rw-r--r--   0        0        0     2845 2024-05-30 22:45:19.476267 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/string_decoder.d.ts
+-rw-r--r--   0        0        0    69637 2024-05-30 22:45:19.476557 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/test.d.ts
+-rw-r--r--   0        0        0     3475 2024-05-30 22:45:19.481191 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/timers/promises.d.ts
+-rw-r--r--   0        0        0    12284 2024-05-30 22:45:19.476735 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/timers.d.ts
+-rw-r--r--   0        0        0    57293 2024-05-30 22:45:19.476957 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/tls.d.ts
+-rw-r--r--   0        0        0     8949 2024-05-30 22:45:19.477145 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/trace_events.d.ts
+-rw-r--r--   0        0        0    10061 2024-05-30 22:45:19.477356 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/tty.d.ts
+-rw-r--r--   0        0        0    41541 2024-05-30 22:45:19.477663 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/url.d.ts
+-rw-r--r--   0        0        0    88519 2024-05-30 22:45:19.478019 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/util.d.ts
+-rw-r--r--   0        0        0    34820 2024-05-30 22:45:19.478217 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/v8.d.ts
+-rw-r--r--   0        0        0    40339 2024-05-30 22:45:19.478451 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/vm.d.ts
+-rw-r--r--   0        0        0     7933 2024-05-30 22:45:19.478612 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/wasi.d.ts
+-rw-r--r--   0        0        0    33977 2024-05-30 22:45:19.479184 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/worker_threads.d.ts
+-rw-r--r--   0        0        0    20025 2024-05-30 22:45:19.479383 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/node/zlib.d.ts
+-rw-r--r--   0        0        0     1141 2024-05-30 22:45:19.421145 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/qs/LICENSE
+-rw-r--r--   0        0        0      803 2024-05-30 22:45:19.427876 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/qs/README.md
+-rw-r--r--   0        0        0     3450 2024-05-30 22:45:19.434008 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/qs/index.d.ts
+-rw-r--r--   0        0        0     1946 2024-05-30 22:45:19.437405 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/qs/package.json
+-rw-r--r--   0        0        0     1141 2024-05-30 22:45:19.421060 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/range-parser/LICENSE
+-rw-r--r--   0        0        0     1640 2024-05-30 22:45:19.427857 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/range-parser/README.md
+-rw-r--r--   0        0        0     1029 2024-05-30 22:45:19.434100 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/range-parser/index.d.ts
+-rw-r--r--   0        0        0      805 2024-05-30 22:45:19.437378 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/range-parser/package.json
+-rw-r--r--   0        0        0     1141 2024-05-30 22:45:19.421352 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/send/LICENSE
+-rw-r--r--   0        0        0      621 2024-05-30 22:45:19.428036 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/send/README.md
+-rw-r--r--   0        0        0     7077 2024-05-30 22:45:19.434163 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/send/index.d.ts
+-rw-r--r--   0        0        0     1010 2024-05-30 22:45:19.437472 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/send/package.json
+-rw-r--r--   0        0        0     1141 2024-05-30 22:45:19.421289 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/serve-static/LICENSE
+-rw-r--r--   0        0        0      761 2024-05-30 22:45:19.427904 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/serve-static/README.md
+-rw-r--r--   0        0        0     4679 2024-05-30 22:45:19.434078 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/serve-static/index.d.ts
+-rw-r--r--   0        0        0     1209 2024-05-30 22:45:19.437444 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/@types/serve-static/package.json
+-rw-r--r--   0        0        0     5096 2024-05-30 22:45:19.436968 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/accepts/HISTORY.md
+-rw-r--r--   0        0        0     1167 2024-05-30 22:45:19.420439 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/accepts/LICENSE
+-rw-r--r--   0        0        0     4123 2024-05-30 22:45:19.439637 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/accepts/README.md
+-rw-r--r--   0        0        0     5252 2024-05-30 22:45:19.427204 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/accepts/index.js
+-rw-r--r--   0        0        0     1157 2024-05-30 22:45:19.433525 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/accepts/package.json
+-rw-r--r--   0        0        0     1103 2024-05-30 22:45:19.433473 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/array-flatten/LICENSE
+-rw-r--r--   0        0        0     1245 2024-05-30 22:45:19.426917 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/array-flatten/README.md
+-rw-r--r--   0        0        0     1195 2024-05-30 22:45:19.436800 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/array-flatten/array-flatten.js
+-rw-r--r--   0        0        0      879 2024-05-30 22:45:19.420155 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/array-flatten/package.json
+-rw-r--r--   0        0        0    16491 2024-05-30 22:45:19.457048 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/body-parser/HISTORY.md
+-rw-r--r--   0        0        0     1172 2024-05-30 22:45:19.420861 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/body-parser/LICENSE
+-rw-r--r--   0        0        0    18182 2024-05-30 22:45:19.459378 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/body-parser/README.md
+-rw-r--r--   0        0        0     1193 2024-05-30 22:45:19.460880 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/body-parser/SECURITY.md
+-rw-r--r--   0        0        0     2681 2024-05-30 22:45:19.427624 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/body-parser/index.js
+-rw-r--r--   0        0        0     4325 2024-05-30 22:45:19.450110 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/body-parser/lib/read.js
+-rw-r--r--   0        0        0     5299 2024-05-30 22:45:19.439908 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/body-parser/lib/types/json.js
+-rw-r--r--   0        0        0     1884 2024-05-30 22:45:19.441987 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/body-parser/lib/types/raw.js
+-rw-r--r--   0        0        0     2285 2024-05-30 22:45:19.453061 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/body-parser/lib/types/text.js
+-rw-r--r--   0        0        0     5797 2024-05-30 22:45:19.454370 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/body-parser/lib/types/urlencoded.js
+-rw-r--r--   0        0        0     1472 2024-05-30 22:45:19.455189 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/body-parser/package.json
+-rw-r--r--   0        0        0     1775 2024-05-30 22:45:19.435858 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/bytes/History.md
+-rw-r--r--   0        0        0     1153 2024-05-30 22:45:19.418918 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/bytes/LICENSE
+-rw-r--r--   0        0        0     4770 2024-05-30 22:45:19.438600 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/bytes/Readme.md
+-rw-r--r--   0        0        0     3613 2024-05-30 22:45:19.425570 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/bytes/index.js
+-rw-r--r--   0        0        0      959 2024-05-30 22:45:19.431723 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/bytes/package.json
+-rw-r--r--   0        0        0       10 2024-05-30 22:45:19.417925 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/call-bind/.eslintignore
+-rw-r--r--   0        0        0      208 2024-05-30 22:45:19.424710 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/call-bind/.eslintrc
+-rw-r--r--   0        0        0      580 2024-05-30 22:45:19.454859 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/call-bind/.github/FUNDING.yml
+-rw-r--r--   0        0        0      139 2024-05-30 22:45:19.430631 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/call-bind/.nycrc
+-rw-r--r--   0        0        0     8142 2024-05-30 22:45:19.450811 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/call-bind/CHANGELOG.md
+-rw-r--r--   0        0        0     1071 2024-05-30 22:45:19.435023 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/call-bind/LICENSE
+-rw-r--r--   0        0        0     2026 2024-05-30 22:45:19.452410 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/call-bind/README.md
+-rw-r--r--   0        0        0      413 2024-05-30 22:45:19.438044 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/call-bind/callBound.js
+-rw-r--r--   0        0        0     1037 2024-05-30 22:45:19.446254 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/call-bind/index.js
+-rw-r--r--   0        0        0     2304 2024-05-30 22:45:19.449640 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/call-bind/package.json
+-rw-r--r--   0        0        0     2349 2024-05-30 22:45:19.443543 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/call-bind/test/callBound.js
+-rw-r--r--   0        0        0     3839 2024-05-30 22:45:19.448389 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/call-bind/test/index.js
+-rw-r--r--   0        0        0     1020 2024-05-30 22:45:19.439688 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/content-disposition/HISTORY.md
+-rw-r--r--   0        0        0     1094 2024-05-30 22:45:19.420380 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/content-disposition/LICENSE
+-rw-r--r--   0        0        0     5205 2024-05-30 22:45:19.444984 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/content-disposition/README.md
+-rw-r--r--   0        0        0    10594 2024-05-30 22:45:19.427158 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/content-disposition/index.js
+-rw-r--r--   0        0        0     1200 2024-05-30 22:45:19.433502 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/content-disposition/package.json
+-rw-r--r--   0        0        0      523 2024-05-30 22:45:19.437074 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/content-type/HISTORY.md
+-rw-r--r--   0        0        0     1089 2024-05-30 22:45:19.420687 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/content-type/LICENSE
+-rw-r--r--   0        0        0     2782 2024-05-30 22:45:19.439714 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/content-type/README.md
+-rw-r--r--   0        0        0     5002 2024-05-30 22:45:19.427573 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/content-type/index.js
+-rw-r--r--   0        0        0     1075 2024-05-30 22:45:19.433811 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/content-type/package.json
+-rw-r--r--   0        0        0     3189 2024-05-30 22:45:19.437194 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/cookie/HISTORY.md
+-rw-r--r--   0        0        0     1175 2024-05-30 22:45:19.420591 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/cookie/LICENSE
+-rw-r--r--   0        0        0    11769 2024-05-30 22:45:19.442028 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/cookie/README.md
+-rw-r--r--   0        0        0     1180 2024-05-30 22:45:19.447632 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/cookie/SECURITY.md
+-rw-r--r--   0        0        0     5281 2024-05-30 22:45:19.427508 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/cookie/index.js
+-rw-r--r--   0        0        0     1142 2024-05-30 22:45:19.433776 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/cookie/package.json
+-rw-r--r--   0        0        0       29 2024-05-30 22:45:19.426722 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/cookie-signature/.npmignore
+-rw-r--r--   0        0        0      695 2024-05-30 22:45:19.436620 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/cookie-signature/History.md
+-rw-r--r--   0        0        0     1490 2024-05-30 22:45:19.439422 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/cookie-signature/Readme.md
+-rw-r--r--   0        0        0     1230 2024-05-30 22:45:19.433210 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/cookie-signature/index.js
+-rw-r--r--   0        0        0      492 2024-05-30 22:45:19.419896 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/cookie-signature/package.json
+-rw-r--r--   0        0        0     1028 2024-05-30 22:45:19.431275 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/cors/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1169 2024-05-30 22:45:19.435494 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/cors/HISTORY.md
+-rw-r--r--   0        0        0     1095 2024-05-30 22:45:19.438390 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/cors/LICENSE
+-rw-r--r--   0        0        0     9206 2024-05-30 22:45:19.443900 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/cors/README.md
+-rw-r--r--   0        0        0     6623 2024-05-30 22:45:19.449829 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/cors/lib/index.js
+-rw-r--r--   0        0        0      867 2024-05-30 22:45:19.425329 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/cors/package.json
+-rw-r--r--   0        0        0       46 2024-05-30 22:45:19.451637 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/debug/.coveralls.yml
+-rw-r--r--   0        0        0      180 2024-05-30 22:45:19.448833 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/debug/.eslintrc
+-rw-r--r--   0        0        0       72 2024-05-30 22:45:19.427249 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/debug/.npmignore
+-rw-r--r--   0        0        0      140 2024-05-30 22:45:19.454225 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/debug/.travis.yml
+-rw-r--r--   0        0        0    11707 2024-05-30 22:45:19.454994 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/debug/CHANGELOG.md
+-rw-r--r--   0        0        0     1107 2024-05-30 22:45:19.441941 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/debug/LICENSE
+-rw-r--r--   0        0        0     1059 2024-05-30 22:45:19.450059 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/debug/Makefile
+-rw-r--r--   0        0        0    17918 2024-05-30 22:45:19.436999 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/debug/README.md
+-rw-r--r--   0        0        0      321 2024-05-30 22:45:19.452822 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/debug/component.json
+-rw-r--r--   0        0        0     1736 2024-05-30 22:45:19.445010 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/debug/karma.conf.js
+-rw-r--r--   0        0        0       40 2024-05-30 22:45:19.447368 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/debug/node.js
+-rw-r--r--   0        0        0     1138 2024-05-30 22:45:19.420493 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/debug/package.json
+-rw-r--r--   0        0        0     4734 2024-05-30 22:45:19.457345 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/debug/src/browser.js
+-rw-r--r--   0        0        0     4394 2024-05-30 22:45:19.459029 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/debug/src/debug.js
+-rw-r--r--   0        0        0      263 2024-05-30 22:45:19.459691 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/debug/src/index.js
+-rw-r--r--   0        0        0      373 2024-05-30 22:45:19.459991 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/debug/src/inspector-log.js
+-rw-r--r--   0        0        0     6015 2024-05-30 22:45:19.461075 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/debug/src/node.js
+-rw-r--r--   0        0        0      291 2024-05-30 22:45:19.417530 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/define-data-property/.eslintrc
+-rw-r--r--   0        0        0      591 2024-05-30 22:45:19.457149 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/define-data-property/.github/FUNDING.yml
+-rw-r--r--   0        0        0      216 2024-05-30 22:45:19.424301 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/define-data-property/.nycrc
+-rw-r--r--   0        0        0     5390 2024-05-30 22:45:19.451868 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/define-data-property/CHANGELOG.md
+-rw-r--r--   0        0        0     1071 2024-05-30 22:45:19.430116 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/define-data-property/LICENSE
+-rw-r--r--   0        0        0     2431 2024-05-30 22:45:19.454787 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/define-data-property/README.md
+-rw-r--r--   0        0        0      315 2024-05-30 22:45:19.455618 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/define-data-property/index.d.ts
+-rw-r--r--   0        0        0     2336 2024-05-30 22:45:19.434787 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/define-data-property/index.js
+-rw-r--r--   0        0        0     2856 2024-05-30 22:45:19.448123 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/define-data-property/package.json
+-rw-r--r--   0        0        0    10471 2024-05-30 22:45:19.443283 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/define-data-property/test/index.js
+-rw-r--r--   0        0        0     4883 2024-05-30 22:45:19.449359 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/define-data-property/tsconfig.json
+-rw-r--r--   0        0        0     2256 2024-05-30 22:45:19.427005 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/depd/History.md
+-rw-r--r--   0        0        0     1094 2024-05-30 22:45:19.441781 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/depd/LICENSE
+-rw-r--r--   0        0        0     9988 2024-05-30 22:45:19.444929 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/depd/Readme.md
+-rw-r--r--   0        0        0    10932 2024-05-30 22:45:19.436676 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/depd/index.js
+-rw-r--r--   0        0        0     1512 2024-05-30 22:45:19.450042 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/depd/lib/browser/index.js
+-rw-r--r--   0        0        0     1335 2024-05-30 22:45:19.420213 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/depd/package.json
+-rw-r--r--   0        0        0     1173 2024-05-30 22:45:19.418734 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/destroy/LICENSE
+-rw-r--r--   0        0        0     2459 2024-05-30 22:45:19.435791 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/destroy/README.md
+-rw-r--r--   0        0        0     4258 2024-05-30 22:45:19.425845 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/destroy/index.js
+-rw-r--r--   0        0        0     1128 2024-05-30 22:45:19.431657 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/destroy/package.json
+-rw-r--r--   0        0        0    16096 2024-05-30 22:45:19.448979 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/dotenv/CHANGELOG.md
+-rw-r--r--   0        0        0     1294 2024-05-30 22:45:19.421418 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/dotenv/LICENSE
+-rw-r--r--   0        0        0    17203 2024-05-30 22:45:19.453160 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/dotenv/README-es.md
+-rw-r--r--   0        0        0    26833 2024-05-30 22:45:19.456056 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/dotenv/README.md
+-rw-r--r--   0        0        0       11 2024-05-30 22:45:19.457655 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/dotenv/config.d.ts
+-rw-r--r--   0        0        0      176 2024-05-30 22:45:19.437543 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/dotenv/config.js
+-rw-r--r--   0        0        0      289 2024-05-30 22:45:19.434273 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/dotenv/lib/cli-options.js
+-rw-r--r--   0        0        0      633 2024-05-30 22:45:19.440096 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/dotenv/lib/env-options.js
+-rw-r--r--   0        0        0     4903 2024-05-30 22:45:19.458436 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/dotenv/lib/main.d.ts
+-rw-r--r--   0        0        0     9972 2024-05-30 22:45:19.442322 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/dotenv/lib/main.js
+-rw-r--r--   0        0        0     1668 2024-05-30 22:45:19.445492 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/dotenv/package.json
+-rw-r--r--   0        0        0     1099 2024-05-30 22:45:19.431587 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/ee-first/LICENSE
+-rw-r--r--   0        0        0     2617 2024-05-30 22:45:19.425478 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/ee-first/README.md
+-rw-r--r--   0        0        0     1684 2024-05-30 22:45:19.435744 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/ee-first/index.js
+-rw-r--r--   0        0        0      859 2024-05-30 22:45:19.418780 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/ee-first/package.json
+-rw-r--r--   0        0        0      238 2024-05-30 22:45:19.439665 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/encodeurl/HISTORY.md
+-rw-r--r--   0        0        0     1089 2024-05-30 22:45:19.433734 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/encodeurl/LICENSE
+-rw-r--r--   0        0        0     3855 2024-05-30 22:45:19.427329 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/encodeurl/README.md
+-rw-r--r--   0        0        0     1586 2024-05-30 22:45:19.436916 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/encodeurl/index.js
+-rw-r--r--   0        0        0     1091 2024-05-30 22:45:19.420268 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/encodeurl/package.json
+-rw-r--r--   0        0        0      144 2024-05-30 22:45:19.418048 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-define-property/.eslintrc
+-rw-r--r--   0        0        0      564 2024-05-30 22:45:19.453749 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-define-property/.github/FUNDING.yml
+-rw-r--r--   0        0        0      139 2024-05-30 22:45:19.424583 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-define-property/.nycrc
+-rw-r--r--   0        0        0      822 2024-05-30 22:45:19.448224 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-define-property/CHANGELOG.md
+-rw-r--r--   0        0        0     1071 2024-05-30 22:45:19.431085 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-define-property/LICENSE
+-rw-r--r--   0        0        0     2056 2024-05-30 22:45:19.449550 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-define-property/README.md
+-rw-r--r--   0        0        0       93 2024-05-30 22:45:19.450660 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-define-property/index.d.ts
+-rw-r--r--   0        0        0      358 2024-05-30 22:45:19.434923 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-define-property/index.js
+-rw-r--r--   0        0        0     2112 2024-05-30 22:45:19.443403 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-define-property/package.json
+-rw-r--r--   0        0        0     1244 2024-05-30 22:45:19.440785 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-define-property/test/index.js
+-rw-r--r--   0        0        0     3195 2024-05-30 22:45:19.446113 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-define-property/tsconfig.json
+-rw-r--r--   0        0        0       43 2024-05-30 22:45:19.418141 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-errors/.eslintrc
+-rw-r--r--   0        0        0      555 2024-05-30 22:45:19.462212 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-errors/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1833 2024-05-30 22:45:19.456659 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-errors/CHANGELOG.md
+-rw-r--r--   0        0        0     1071 2024-05-30 22:45:19.424825 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-errors/LICENSE
+-rw-r--r--   0        0        0     2114 2024-05-30 22:45:19.457191 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-errors/README.md
+-rw-r--r--   0        0        0       68 2024-05-30 22:45:19.458031 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-errors/eval.d.ts
+-rw-r--r--   0        0        0       75 2024-05-30 22:45:19.430846 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-errors/eval.js
+-rw-r--r--   0        0        0       56 2024-05-30 22:45:19.458665 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-errors/index.d.ts
+-rw-r--r--   0        0        0       66 2024-05-30 22:45:19.435145 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-errors/index.js
+-rw-r--r--   0        0        0     2174 2024-05-30 22:45:19.452029 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-errors/package.json
+-rw-r--r--   0        0        0       71 2024-05-30 22:45:19.459426 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-errors/range.d.ts
+-rw-r--r--   0        0        0       77 2024-05-30 22:45:19.443663 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-errors/range.js
+-rw-r--r--   0        0        0       83 2024-05-30 22:45:19.459910 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-errors/ref.d.ts
+-rw-r--r--   0        0        0       79 2024-05-30 22:45:19.446307 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-errors/ref.js
+-rw-r--r--   0        0        0       74 2024-05-30 22:45:19.460849 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-errors/syntax.d.ts
+-rw-r--r--   0        0        0       79 2024-05-30 22:45:19.448297 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-errors/syntax.js
+-rw-r--r--   0        0        0      356 2024-05-30 22:45:19.440942 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-errors/test/index.js
+-rw-r--r--   0        0        0     3170 2024-05-30 22:45:19.454799 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-errors/tsconfig.json
+-rw-r--r--   0        0        0       67 2024-05-30 22:45:19.461327 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-errors/type.d.ts
+-rw-r--r--   0        0        0       75 2024-05-30 22:45:19.449711 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-errors/type.js
+-rw-r--r--   0        0        0       65 2024-05-30 22:45:19.461590 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-errors/uri.d.ts
+-rw-r--r--   0        0        0       73 2024-05-30 22:45:19.450839 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/es-errors/uri.js
+-rw-r--r--   0        0        0     1069 2024-05-30 22:45:19.456505 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/esbuild/LICENSE.md
+-rw-r--r--   0        0        0      175 2024-05-30 22:45:19.458095 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/esbuild/README.md
+hrwxr-xr-x   0        0        0        0 2024-05-30 22:45:19.488834 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/esbuild/bin/esbuild
+-rw-r--r--   0        0        0    10963 2024-05-30 22:45:19.434473 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/esbuild/install.js
+-rw-r--r--   0        0        0    22928 2024-05-30 22:45:19.459452 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/esbuild/lib/main.d.ts
+-rw-r--r--   0        0        0    88832 2024-05-30 22:45:19.451809 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/esbuild/lib/main.js
+-rw-r--r--   0        0        0     1340 2024-05-30 22:45:19.454754 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/esbuild/package.json
+-rw-r--r--   0        0        0     1157 2024-05-30 22:45:19.426596 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/escape-html/LICENSE
+-rw-r--r--   0        0        0      707 2024-05-30 22:45:19.436570 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/escape-html/Readme.md
+-rw-r--r--   0        0        0     1362 2024-05-30 22:45:19.433165 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/escape-html/index.js
+-rw-r--r--   0        0        0      434 2024-05-30 22:45:19.419926 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/escape-html/package.json
+-rw-r--r--   0        0        0     1732 2024-05-30 22:45:19.439586 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/etag/HISTORY.md
+-rw-r--r--   0        0        0     1094 2024-05-30 22:45:19.433444 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/etag/LICENSE
+-rw-r--r--   0        0        0     4198 2024-05-30 22:45:19.426859 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/etag/README.md
+-rw-r--r--   0        0        0     2479 2024-05-30 22:45:19.436767 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/etag/index.js
+-rw-r--r--   0        0        0     1306 2024-05-30 22:45:19.420309 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/etag/package.json
+-rw-r--r--   0        0        0   113674 2024-05-30 22:45:19.466203 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/express/History.md
+-rw-r--r--   0        0        0     1249 2024-05-30 22:45:19.421756 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/express/LICENSE
+-rw-r--r--   0        0        0     5421 2024-05-30 22:45:19.467076 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/express/Readme.md
+-rw-r--r--   0        0        0      224 2024-05-30 22:45:19.445768 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/express/index.js
+-rw-r--r--   0        0        0    14593 2024-05-30 22:45:19.437753 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/express/lib/application.js
+-rw-r--r--   0        0        0     2409 2024-05-30 22:45:19.442875 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/express/lib/express.js
+-rw-r--r--   0        0        0      853 2024-05-30 22:45:19.454504 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/express/lib/middleware/init.js
+-rw-r--r--   0        0        0      885 2024-05-30 22:45:19.456173 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/express/lib/middleware/query.js
+-rw-r--r--   0        0        0    12505 2024-05-30 22:45:19.457676 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/express/lib/request.js
+-rw-r--r--   0        0        0    28339 2024-05-30 22:45:19.460757 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/express/lib/response.js
+-rw-r--r--   0        0        0    15123 2024-05-30 22:45:19.450634 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/express/lib/router/index.js
+-rw-r--r--   0        0        0     3296 2024-05-30 22:45:19.455462 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/express/lib/router/layer.js
+-rw-r--r--   0        0        0     4399 2024-05-30 22:45:19.461231 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/express/lib/router/route.js
+-rw-r--r--   0        0        0     5871 2024-05-30 22:45:19.461788 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/express/lib/utils.js
+-rw-r--r--   0        0        0     3325 2024-05-30 22:45:19.462372 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/express/lib/view.js
+-rw-r--r--   0        0        0     2597 2024-05-30 22:45:19.462873 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/express/package.json
+-rw-r--r--   0        0        0     4292 2024-05-30 22:45:19.439370 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/finalhandler/HISTORY.md
+-rw-r--r--   0        0        0     1119 2024-05-30 22:45:19.419855 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/finalhandler/LICENSE
+-rw-r--r--   0        0        0     4133 2024-05-30 22:45:19.444749 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/finalhandler/README.md
+-rw-r--r--   0        0        0     1202 2024-05-30 22:45:19.447208 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/finalhandler/SECURITY.md
+-rw-r--r--   0        0        0     6689 2024-05-30 22:45:19.426643 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/finalhandler/index.js
+-rw-r--r--   0        0        0     1207 2024-05-30 22:45:19.433252 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/finalhandler/package.json
+-rw-r--r--   0        0        0      400 2024-05-30 22:45:19.435170 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/forwarded/HISTORY.md
+-rw-r--r--   0        0        0     1094 2024-05-30 22:45:19.418458 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/forwarded/LICENSE
+-rw-r--r--   0        0        0     1654 2024-05-30 22:45:19.438131 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/forwarded/README.md
+-rw-r--r--   0        0        0     1578 2024-05-30 22:45:19.424878 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/forwarded/index.js
+-rw-r--r--   0        0        0     1150 2024-05-30 22:45:19.431133 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/forwarded/package.json
+-rw-r--r--   0        0        0     1500 2024-05-30 22:45:19.439352 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/fresh/HISTORY.md
+-rw-r--r--   0        0        0     1174 2024-05-30 22:45:19.432570 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/fresh/LICENSE
+-rw-r--r--   0        0        0     3374 2024-05-30 22:45:19.426434 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/fresh/README.md
+-rw-r--r--   0        0        0     2711 2024-05-30 22:45:19.436543 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/fresh/index.js
+-rw-r--r--   0        0        0     1357 2024-05-30 22:45:19.419816 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/fresh/package.json
+-rw-r--r--   0        0        0     1133 2024-05-30 22:45:19.417439 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/fsevents/LICENSE
+-rw-r--r--   0        0        0     3203 2024-05-30 22:45:19.434661 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/fsevents/README.md
+-rw-r--r--   0        0        0     1431 2024-05-30 22:45:19.456398 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/fsevents/fsevents.d.ts
+-rw-r--r--   0        0        0     2483 2024-05-30 22:45:19.424245 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/fsevents/fsevents.js
+-rwxr-xr-x   0        0        0   163626 2024-05-30 22:45:19.455543 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/fsevents/fsevents.node
+-rw-r--r--   0        0        0     1348 2024-05-30 22:45:19.430175 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/fsevents/package.json
+-rw-r--r--   0        0        0      253 2024-05-30 22:45:19.417585 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/function-bind/.eslintrc
+-rw-r--r--   0        0        0      584 2024-05-30 22:45:19.458055 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/function-bind/.github/FUNDING.yml
+-rw-r--r--   0        0        0      157 2024-05-30 22:45:19.457283 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/function-bind/.github/SECURITY.md
+-rw-r--r--   0        0        0      216 2024-05-30 22:45:19.434689 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/function-bind/.nycrc
+-rw-r--r--   0        0        0    13812 2024-05-30 22:45:19.453942 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/function-bind/CHANGELOG.md
+-rw-r--r--   0        0        0     1052 2024-05-30 22:45:19.437882 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/function-bind/LICENSE
+-rw-r--r--   0        0        0     1755 2024-05-30 22:45:19.455658 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/function-bind/README.md
+-rw-r--r--   0        0        0     2043 2024-05-30 22:45:19.440559 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/function-bind/implementation.js
+-rw-r--r--   0        0        0      126 2024-05-30 22:45:19.443167 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/function-bind/index.js
+-rw-r--r--   0        0        0     2262 2024-05-30 22:45:19.450693 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/function-bind/package.json
+-rw-r--r--   0        0        0      176 2024-05-30 22:45:19.429988 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/function-bind/test/.eslintrc
+-rw-r--r--   0        0        0     8991 2024-05-30 22:45:19.448165 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/function-bind/test/index.js
+-rw-r--r--   0        0        0      603 2024-05-30 22:45:19.418288 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/get-intrinsic/.eslintrc
+-rw-r--r--   0        0        0      584 2024-05-30 22:45:19.455928 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/get-intrinsic/.github/FUNDING.yml
+-rw-r--r--   0        0        0      139 2024-05-30 22:45:19.425193 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/get-intrinsic/.nycrc
+-rw-r--r--   0        0        0    11640 2024-05-30 22:45:19.451180 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/get-intrinsic/CHANGELOG.md
+-rw-r--r--   0        0        0     1071 2024-05-30 22:45:19.431162 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/get-intrinsic/LICENSE
+-rw-r--r--   0        0        0     2791 2024-05-30 22:45:19.454112 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/get-intrinsic/README.md
+-rw-r--r--   0        0        0    13615 2024-05-30 22:45:19.443946 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/get-intrinsic/index.js
+-rw-r--r--   0        0        0     2414 2024-05-30 22:45:19.448493 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/get-intrinsic/package.json
+-rw-r--r--   0        0        0     8767 2024-05-30 22:45:19.438307 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/get-intrinsic/test/GetIntrinsic.js
+-rw-r--r--   0        0        0     1089 2024-05-30 22:45:19.416782 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/get-tsconfig/LICENSE
+-rw-r--r--   0        0        0     6419 2024-05-30 22:45:19.449098 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/get-tsconfig/README.md
+-rwxr-xr-x   0        0        0    16920 2024-05-30 22:45:19.434331 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/get-tsconfig/dist/index.cjs
+-rw-r--r--   0        0        0    29404 2024-05-30 22:45:19.445518 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/get-tsconfig/dist/index.d.cts
+-rw-r--r--   0        0        0    29404 2024-05-30 22:45:19.456276 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/get-tsconfig/dist/index.d.mts
+-rwxr-xr-x   0        0        0    16902 2024-05-30 22:45:19.451761 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/get-tsconfig/dist/index.mjs
+-rw-r--r--   0        0        0     1030 2024-05-30 22:45:19.447736 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/get-tsconfig/package.json
+-rw-r--r--   0        0        0      224 2024-05-30 22:45:19.417271 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/gopd/.eslintrc
+-rw-r--r--   0        0        0      575 2024-05-30 22:45:19.449132 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/gopd/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1541 2024-05-30 22:45:19.443062 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/gopd/CHANGELOG.md
+-rw-r--r--   0        0        0     1071 2024-05-30 22:45:19.423872 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/gopd/LICENSE
+-rw-r--r--   0        0        0     1562 2024-05-30 22:45:19.445738 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/gopd/README.md
+-rw-r--r--   0        0        0      263 2024-05-30 22:45:19.429678 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/gopd/index.js
+-rw-r--r--   0        0        0     1877 2024-05-30 22:45:19.440478 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/gopd/package.json
+-rw-r--r--   0        0        0      590 2024-05-30 22:45:19.437812 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/gopd/test/index.js
+-rw-r--r--   0        0        0      173 2024-05-30 22:45:19.416919 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-property-descriptors/.eslintrc
+-rw-r--r--   0        0        0      595 2024-05-30 22:45:19.453525 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-property-descriptors/.github/FUNDING.yml
+-rw-r--r--   0        0        0      139 2024-05-30 22:45:19.421660 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-property-descriptors/.nycrc
+-rw-r--r--   0        0        0     2648 2024-05-30 22:45:19.445593 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-property-descriptors/CHANGELOG.md
+-rw-r--r--   0        0        0     1067 2024-05-30 22:45:19.428254 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-property-descriptors/LICENSE
+-rw-r--r--   0        0        0     2206 2024-05-30 22:45:19.449025 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-property-descriptors/README.md
+-rw-r--r--   0        0        0      588 2024-05-30 22:45:19.434305 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-property-descriptors/index.js
+-rw-r--r--   0        0        0     2090 2024-05-30 22:45:19.442796 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-property-descriptors/package.json
+-rw-r--r--   0        0        0     1405 2024-05-30 22:45:19.440150 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-property-descriptors/test/index.js
+-rw-r--r--   0        0        0       43 2024-05-30 22:45:19.417821 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-proto/.eslintrc
+-rw-r--r--   0        0        0      580 2024-05-30 22:45:19.455050 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-proto/.github/FUNDING.yml
+-rw-r--r--   0        0        0     2200 2024-05-30 22:45:19.446183 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-proto/CHANGELOG.md
+-rw-r--r--   0        0        0     1067 2024-05-30 22:45:19.424506 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-proto/LICENSE
+-rw-r--r--   0        0        0     1623 2024-05-30 22:45:19.449757 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-proto/README.md
+-rw-r--r--   0        0        0       57 2024-05-30 22:45:19.452232 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-proto/index.d.ts
+-rw-r--r--   0        0        0      302 2024-05-30 22:45:19.430354 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-proto/index.js
+-rw-r--r--   0        0        0     2004 2024-05-30 22:45:19.440816 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-proto/package.json
+-rw-r--r--   0        0        0      477 2024-05-30 22:45:19.438077 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-proto/test/index.js
+-rw-r--r--   0        0        0     3611 2024-05-30 22:45:19.443457 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-proto/tsconfig.json
+-rw-r--r--   0        0        0      164 2024-05-30 22:45:19.417085 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-symbols/.eslintrc
+-rw-r--r--   0        0        0      582 2024-05-30 22:45:19.459182 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-symbols/.github/FUNDING.yml
+-rw-r--r--   0        0        0      139 2024-05-30 22:45:19.421719 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-symbols/.nycrc
+-rw-r--r--   0        0        0     7690 2024-05-30 22:45:19.456956 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-symbols/CHANGELOG.md
+-rw-r--r--   0        0        0     1071 2024-05-30 22:45:19.428723 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-symbols/LICENSE
+-rw-r--r--   0        0        0     2044 2024-05-30 22:45:19.457745 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-symbols/README.md
+-rw-r--r--   0        0        0      420 2024-05-30 22:45:19.445645 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-symbols/index.js
+-rw-r--r--   0        0        0     2648 2024-05-30 22:45:19.455318 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-symbols/package.json
+-rw-r--r--   0        0        0     1761 2024-05-30 22:45:19.451526 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-symbols/shams.js
+-rw-r--r--   0        0        0      654 2024-05-30 22:45:19.450272 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-symbols/test/index.js
+-rw-r--r--   0        0        0      723 2024-05-30 22:45:19.440284 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-symbols/test/shams/core-js.js
+-rw-r--r--   0        0        0      686 2024-05-30 22:45:19.442848 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-symbols/test/shams/get-own-property-symbols.js
+-rw-r--r--   0        0        0     2021 2024-05-30 22:45:19.453216 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/has-symbols/test/tests.js
+-rw-r--r--   0        0        0       43 2024-05-30 22:45:19.417733 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/hasown/.eslintrc
+-rw-r--r--   0        0        0      552 2024-05-30 22:45:19.450532 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/hasown/.github/FUNDING.yml
+-rw-r--r--   0        0        0      216 2024-05-30 22:45:19.424271 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/hasown/.nycrc
+-rw-r--r--   0        0        0     2579 2024-05-30 22:45:19.443272 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/hasown/CHANGELOG.md
+-rw-r--r--   0        0        0     1083 2024-05-30 22:45:19.430469 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/hasown/LICENSE
+-rw-r--r--   0        0        0     1613 2024-05-30 22:45:19.445868 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/hasown/README.md
+-rw-r--r--   0        0        0      117 2024-05-30 22:45:19.447914 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/hasown/index.d.ts
+-rw-r--r--   0        0        0      206 2024-05-30 22:45:19.434743 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/hasown/index.js
+-rw-r--r--   0        0        0     2283 2024-05-30 22:45:19.437949 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/hasown/package.json
+-rw-r--r--   0        0        0       73 2024-05-30 22:45:19.440757 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/hasown/tsconfig.json
+-rw-r--r--   0        0        0     3973 2024-05-30 22:45:19.436732 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/http-errors/HISTORY.md
+-rw-r--r--   0        0        0     1168 2024-05-30 22:45:19.420128 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/http-errors/LICENSE
+-rw-r--r--   0        0        0     5962 2024-05-30 22:45:19.439560 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/http-errors/README.md
+-rw-r--r--   0        0        0     6391 2024-05-30 22:45:19.426799 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/http-errors/index.js
+-rw-r--r--   0        0        0     1314 2024-05-30 22:45:19.433400 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/http-errors/package.json
+-rw-r--r--   0        0        0     4342 2024-05-30 22:45:19.425541 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/iconv-lite/Changelog.md
+-rw-r--r--   0        0        0     1064 2024-05-30 22:45:19.431552 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/iconv-lite/LICENSE
+-rw-r--r--   0        0        0     6534 2024-05-30 22:45:19.435644 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/iconv-lite/README.md
+-rw-r--r--   0        0        0    21415 2024-05-30 22:45:19.444255 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/iconv-lite/encodings/dbcs-codec.js
+-rw-r--r--   0        0        0     8291 2024-05-30 22:45:19.448793 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/iconv-lite/encodings/dbcs-data.js
+-rw-r--r--   0        0        0      710 2024-05-30 22:45:19.449982 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/iconv-lite/encodings/index.js
+-rw-r--r--   0        0        0     6115 2024-05-30 22:45:19.451098 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/iconv-lite/encodings/internal.js
+-rw-r--r--   0        0        0     2191 2024-05-30 22:45:19.452734 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/iconv-lite/encodings/sbcs-codec.js
+-rw-r--r--   0        0        0    32034 2024-05-30 22:45:19.455823 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/iconv-lite/encodings/sbcs-data-generated.js
+-rw-r--r--   0        0        0     4686 2024-05-30 22:45:19.456611 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/iconv-lite/encodings/sbcs-data.js
+-rw-r--r--   0        0        0    17717 2024-05-30 22:45:19.459517 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/iconv-lite/encodings/tables/big5-added.json
+-rw-r--r--   0        0        0    47320 2024-05-30 22:45:19.461556 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/iconv-lite/encodings/tables/cp936.json
+-rw-r--r--   0        0        0    38122 2024-05-30 22:45:19.462351 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/iconv-lite/encodings/tables/cp949.json
+-rw-r--r--   0        0        0    42356 2024-05-30 22:45:19.463527 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/iconv-lite/encodings/tables/cp950.json
+-rw-r--r--   0        0        0    41064 2024-05-30 22:45:19.464703 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/iconv-lite/encodings/tables/eucjp.json
+-rw-r--r--   0        0        0     2216 2024-05-30 22:45:19.465108 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/iconv-lite/encodings/tables/gb18030-ranges.json
+-rw-r--r--   0        0        0     1227 2024-05-30 22:45:19.465439 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/iconv-lite/encodings/tables/gbk-added.json
+-rw-r--r--   0        0        0    23782 2024-05-30 22:45:19.466393 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/iconv-lite/encodings/tables/shiftjis.json
+-rw-r--r--   0        0        0     5011 2024-05-30 22:45:19.466925 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/iconv-lite/encodings/utf16.js
+-rw-r--r--   0        0        0     9215 2024-05-30 22:45:19.467445 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/iconv-lite/encodings/utf7.js
+-rw-r--r--   0        0        0     1109 2024-05-30 22:45:19.468167 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/iconv-lite/lib/bom-handling.js
+-rw-r--r--   0        0        0     8701 2024-05-30 22:45:19.468285 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/iconv-lite/lib/extend-node.js
+-rw-r--r--   0        0        0      982 2024-05-30 22:45:19.468448 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/iconv-lite/lib/index.d.ts
+-rw-r--r--   0        0        0     5123 2024-05-30 22:45:19.468632 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/iconv-lite/lib/index.js
+-rw-r--r--   0        0        0     3387 2024-05-30 22:45:19.468758 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/iconv-lite/lib/streams.js
+-rw-r--r--   0        0        0     1227 2024-05-30 22:45:19.418686 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/iconv-lite/package.json
+-rw-r--r--   0        0        0      749 2024-05-30 22:45:19.435669 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/inherits/LICENSE
+-rw-r--r--   0        0        0     1625 2024-05-30 22:45:19.438520 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/inherits/README.md
+-rw-r--r--   0        0        0      250 2024-05-30 22:45:19.431426 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/inherits/inherits.js
+-rw-r--r--   0        0        0      753 2024-05-30 22:45:19.425378 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/inherits/inherits_browser.js
+-rw-r--r--   0        0        0      581 2024-05-30 22:45:19.418854 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/inherits/package.json
+-rw-r--r--   0        0        0     1087 2024-05-30 22:45:19.430755 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/ipaddr.js/LICENSE
+-rw-r--r--   0        0        0     8309 2024-05-30 22:45:19.438405 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/ipaddr.js/README.md
+-rw-r--r--   0        0        0     9738 2024-05-30 22:45:19.425030 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/ipaddr.js/ipaddr.min.js
+-rw-r--r--   0        0        0    19333 2024-05-30 22:45:19.448457 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/ipaddr.js/lib/ipaddr.js
+-rw-r--r--   0        0        0     2959 2024-05-30 22:45:19.450950 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/ipaddr.js/lib/ipaddr.js.d.ts
+-rw-r--r--   0        0        0      719 2024-05-30 22:45:19.417985 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/ipaddr.js/package.json
+-rw-r--r--   0        0        0      461 2024-05-30 22:45:19.438161 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/media-typer/HISTORY.md
+-rw-r--r--   0        0        0     1089 2024-05-30 22:45:19.430697 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/media-typer/LICENSE
+-rw-r--r--   0        0        0     2371 2024-05-30 22:45:19.424676 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/media-typer/README.md
+-rw-r--r--   0        0        0     6375 2024-05-30 22:45:19.435124 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/media-typer/index.js
+-rw-r--r--   0        0        0      759 2024-05-30 22:45:19.417953 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/media-typer/package.json
+-rw-r--r--   0        0        0      363 2024-05-30 22:45:19.439500 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/merge-descriptors/HISTORY.md
+-rw-r--r--   0        0        0     1167 2024-05-30 22:45:19.433284 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/merge-descriptors/LICENSE
+-rw-r--r--   0        0        0     1213 2024-05-30 22:45:19.427061 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/merge-descriptors/README.md
+-rw-r--r--   0        0        0     1215 2024-05-30 22:45:19.436664 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/merge-descriptors/index.js
+-rw-r--r--   0        0        0      931 2024-05-30 22:45:19.420065 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/merge-descriptors/package.json
+-rw-r--r--   0        0        0      427 2024-05-30 22:45:19.439283 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/methods/HISTORY.md
+-rw-r--r--   0        0        0     1180 2024-05-30 22:45:19.433124 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/methods/LICENSE
+-rw-r--r--   0        0        0     1694 2024-05-30 22:45:19.426470 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/methods/README.md
+-rw-r--r--   0        0        0     1040 2024-05-30 22:45:19.436600 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/methods/index.js
+-rw-r--r--   0        0        0      947 2024-05-30 22:45:19.419763 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/methods/package.json
+-rw-r--r--   0        0        0        0 2024-05-30 22:45:19.418335 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/mime/.npmignore
+-rw-r--r--   0        0        0     9473 2024-05-30 22:45:19.446471 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/mime/CHANGELOG.md
+-rw-r--r--   0        0        0     1098 2024-05-30 22:45:19.435471 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/mime/LICENSE
+-rw-r--r--   0        0        0     2119 2024-05-30 22:45:19.431256 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/mime/README.md
+-rwxr-xr-x   0        0        0      149 2024-05-30 22:45:19.441216 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/mime/cli.js
+-rw-r--r--   0        0        0     2726 2024-05-30 22:45:19.438339 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/mime/mime.js
+-rw-r--r--   0        0        0      933 2024-05-30 22:45:19.418665 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/mime/package.json
+-rwxr-xr-x   0        0        0     1351 2024-05-30 22:45:19.450917 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/mime/src/build.js
+-rw-r--r--   0        0        0     2334 2024-05-30 22:45:19.452283 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/mime/src/test.js
+-rw-r--r--   0        0        0    31555 2024-05-30 22:45:19.455972 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/mime/types.json
+-rw-r--r--   0        0        0    12581 2024-05-30 22:45:19.458281 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/mime-db/HISTORY.md
+-rw-r--r--   0        0        0     1172 2024-05-30 22:45:19.418107 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/mime-db/LICENSE
+-rw-r--r--   0        0        0     4091 2024-05-30 22:45:19.459493 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/mime-db/README.md
+-rw-r--r--   0        0        0   185882 2024-05-30 22:45:19.454814 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/mime-db/db.json
+-rw-r--r--   0        0        0      189 2024-05-30 22:45:19.424917 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/mime-db/index.js
+-rw-r--r--   0        0        0     1624 2024-05-30 22:45:19.456545 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/mime-db/package.json
+-rw-r--r--   0        0        0     8812 2024-05-30 22:45:19.438914 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/mime-types/HISTORY.md
+-rw-r--r--   0        0        0     1167 2024-05-30 22:45:19.419380 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/mime-types/LICENSE
+-rw-r--r--   0        0        0     3481 2024-05-30 22:45:19.444360 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/mime-types/README.md
+-rw-r--r--   0        0        0     3663 2024-05-30 22:45:19.425980 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/mime-types/index.js
+-rw-r--r--   0        0        0     1149 2024-05-30 22:45:19.432056 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/mime-types/package.json
+-rw-r--r--   0        0        0     2764 2024-05-30 22:45:19.425066 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/ms/index.js
+-rw-r--r--   0        0        0     1077 2024-05-30 22:45:19.431199 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/ms/license.md
+-rw-r--r--   0        0        0      704 2024-05-30 22:45:19.418218 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/ms/package.json
+-rw-r--r--   0        0        0     1721 2024-05-30 22:45:19.435287 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/ms/readme.md
+-rw-r--r--   0        0        0     2499 2024-05-30 22:45:19.451029 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/negotiator/HISTORY.md
+-rw-r--r--   0        0        0     1177 2024-05-30 22:45:19.418965 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/negotiator/LICENSE
+-rw-r--r--   0        0        0     4901 2024-05-30 22:45:19.454076 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/negotiator/README.md
+-rw-r--r--   0        0        0     2451 2024-05-30 22:45:19.438665 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/negotiator/index.js
+-rw-r--r--   0        0        0     3081 2024-05-30 22:45:19.431759 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/negotiator/lib/charset.js
+-rw-r--r--   0        0        0     3506 2024-05-30 22:45:19.435902 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/negotiator/lib/encoding.js
+-rw-r--r--   0        0        0     3409 2024-05-30 22:45:19.444140 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/negotiator/lib/language.js
+-rw-r--r--   0        0        0     5358 2024-05-30 22:45:19.448721 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/negotiator/lib/mediaType.js
+-rw-r--r--   0        0        0      993 2024-05-30 22:45:19.449873 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/negotiator/package.json
+-rw-r--r--   0        0        0     2108 2024-05-30 22:45:19.427469 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-assign/index.js
+-rw-r--r--   0        0        0     1119 2024-05-30 22:45:19.433841 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-assign/license
+-rw-r--r--   0        0        0      764 2024-05-30 22:45:19.420729 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-assign/package.json
+-rw-r--r--   0        0        0     1502 2024-05-30 22:45:19.437103 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-assign/readme.md
+-rw-r--r--   0        0        0     1298 2024-05-30 22:45:19.417667 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/.eslintrc
+-rw-r--r--   0        0        0      585 2024-05-30 22:45:19.468935 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/.github/FUNDING.yml
+-rw-r--r--   0        0        0      236 2024-05-30 22:45:19.424425 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/.nycrc
+-rw-r--r--   0        0        0    33226 2024-05-30 22:45:19.468513 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/CHANGELOG.md
+-rw-r--r--   0        0        0     1071 2024-05-30 22:45:19.430305 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/LICENSE
+-rw-r--r--   0        0        0      391 2024-05-30 22:45:19.438000 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/example/all.js
+-rw-r--r--   0        0        0      116 2024-05-30 22:45:19.446056 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/example/circular.js
+-rw-r--r--   0        0        0      126 2024-05-30 22:45:19.456351 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/example/fn.js
+-rw-r--r--   0        0        0      251 2024-05-30 22:45:19.462651 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/example/inspect.js
+-rw-r--r--   0        0        0    18882 2024-05-30 22:45:19.462042 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/index.js
+-rw-r--r--   0        0        0      365 2024-05-30 22:45:19.467221 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/package-support.json
+-rw-r--r--   0        0        0     2702 2024-05-30 22:45:19.467565 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/package.json
+-rw-r--r--   0        0        0     2934 2024-05-30 22:45:19.467951 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/readme.markdown
+-rw-r--r--   0        0        0     2082 2024-05-30 22:45:19.443309 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/test/bigint.js
+-rw-r--r--   0        0        0      416 2024-05-30 22:45:19.451859 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/test/browser/dom.js
+-rw-r--r--   0        0        0      451 2024-05-30 22:45:19.448021 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/test/circular.js
+-rw-r--r--   0        0        0      400 2024-05-30 22:45:19.449455 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/test/deep.js
+-rw-r--r--   0        0        0     1575 2024-05-30 22:45:19.453690 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/test/element.js
+-rw-r--r--   0        0        0     1536 2024-05-30 22:45:19.454626 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/test/err.js
+-rw-r--r--   0        0        0      683 2024-05-30 22:45:19.455527 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/test/fakes.js
+-rw-r--r--   0        0        0     2227 2024-05-30 22:45:19.457071 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/test/fn.js
+-rw-r--r--   0        0        0      372 2024-05-30 22:45:19.457918 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/test/global.js
+-rw-r--r--   0        0        0      514 2024-05-30 22:45:19.458598 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/test/has.js
+-rw-r--r--   0        0        0      255 2024-05-30 22:45:19.459357 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/test/holes.js
+-rw-r--r--   0        0        0     6633 2024-05-30 22:45:19.460897 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/test/indent-option.js
+-rw-r--r--   0        0        0     4946 2024-05-30 22:45:19.463197 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/test/inspect.js
+-rw-r--r--   0        0        0      268 2024-05-30 22:45:19.463600 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/test/lowbyte.js
+-rw-r--r--   0        0        0     2312 2024-05-30 22:45:19.463872 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/test/number.js
+-rw-r--r--   0        0        0      933 2024-05-30 22:45:19.464792 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/test/quoteStyle.js
+-rw-r--r--   0        0        0     1546 2024-05-30 22:45:19.465733 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/test/toStringTag.js
+-rw-r--r--   0        0        0      302 2024-05-30 22:45:19.465895 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/test/undef.js
+-rw-r--r--   0        0        0     7034 2024-05-30 22:45:19.466839 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/test/values.js
+-rw-r--r--   0        0        0      534 2024-05-30 22:45:19.465359 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/test-core-js.js
+-rw-r--r--   0        0        0       42 2024-05-30 22:45:19.466327 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/object-inspect/util.inspect.js
+-rw-r--r--   0        0        0     1865 2024-05-30 22:45:19.436173 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/on-finished/HISTORY.md
+-rw-r--r--   0        0        0     1167 2024-05-30 22:45:19.419342 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/on-finished/LICENSE
+-rw-r--r--   0        0        0     5160 2024-05-30 22:45:19.441470 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/on-finished/README.md
+-rw-r--r--   0        0        0     4430 2024-05-30 22:45:19.425909 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/on-finished/index.js
+-rw-r--r--   0        0        0     1057 2024-05-30 22:45:19.432177 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/on-finished/package.json
+-rw-r--r--   0        0        0     1043 2024-05-30 22:45:19.426223 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/parseurl/HISTORY.md
+-rw-r--r--   0        0        0     1173 2024-05-30 22:45:19.436350 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/parseurl/LICENSE
+-rw-r--r--   0        0        0     4094 2024-05-30 22:45:19.439261 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/parseurl/README.md
+-rw-r--r--   0        0        0     2809 2024-05-30 22:45:19.432382 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/parseurl/index.js
+-rw-r--r--   0        0        0     1180 2024-05-30 22:45:19.419617 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/parseurl/package.json
+-rw-r--r--   0        0        0      694 2024-05-30 22:45:19.439180 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/path-to-regexp/History.md
+-rw-r--r--   0        0        0     1103 2024-05-30 22:45:19.426553 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/path-to-regexp/LICENSE
+-rw-r--r--   0        0        0     1102 2024-05-30 22:45:19.436450 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/path-to-regexp/Readme.md
+-rw-r--r--   0        0        0     3328 2024-05-30 22:45:19.432498 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/path-to-regexp/index.js
+-rw-r--r--   0        0        0      554 2024-05-30 22:45:19.419698 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/path-to-regexp/package.json
+-rw-r--r--   0        0        0     2991 2024-05-30 22:45:19.436413 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/proxy-addr/HISTORY.md
+-rw-r--r--   0        0        0     1094 2024-05-30 22:45:19.420016 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/proxy-addr/LICENSE
+-rw-r--r--   0        0        0     4131 2024-05-30 22:45:19.441616 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/proxy-addr/README.md
+-rw-r--r--   0        0        0     6000 2024-05-30 22:45:19.426127 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/proxy-addr/index.js
+-rw-r--r--   0        0        0     1183 2024-05-30 22:45:19.432357 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/proxy-addr/package.json
+-rw-r--r--   0        0        0      569 2024-05-30 22:45:19.419493 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/qs/.editorconfig
+-rw-r--r--   0        0        0     1025 2024-05-30 22:45:19.425867 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/qs/.eslintrc
+-rw-r--r--   0        0        0      548 2024-05-30 22:45:19.467868 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/qs/.github/FUNDING.yml
+-rw-r--r--   0        0        0      216 2024-05-30 22:45:19.432088 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/qs/.nycrc
+-rw-r--r--   0        0        0    29661 2024-05-30 22:45:19.465838 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/qs/CHANGELOG.md
+-rw-r--r--   0        0        0     1600 2024-05-30 22:45:19.466237 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/qs/LICENSE.md
+-rw-r--r--   0        0        0    20966 2024-05-30 22:45:19.467129 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/qs/README.md
+-rw-r--r--   0        0        0    69136 2024-05-30 22:45:19.459045 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/qs/dist/qs.js
+-rw-r--r--   0        0        0      476 2024-05-30 22:45:19.439154 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/qs/lib/formats.js
+-rw-r--r--   0        0        0      211 2024-05-30 22:45:19.441511 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/qs/lib/index.js
+-rw-r--r--   0        0        0     9380 2024-05-30 22:45:19.446967 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/qs/lib/parse.js
+-rw-r--r--   0        0        0    10358 2024-05-30 22:45:19.461163 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/qs/lib/stringify.js
+-rw-r--r--   0        0        0     6823 2024-05-30 22:45:19.462957 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/qs/lib/utils.js
+-rw-r--r--   0        0        0     2317 2024-05-30 22:45:19.464528 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/qs/package.json
+-rw-r--r--   0        0        0    35871 2024-05-30 22:45:19.454188 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/qs/test/parse.js
+-rw-r--r--   0        0        0    35186 2024-05-30 22:45:19.462782 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/qs/test/stringify.js
+-rw-r--r--   0        0        0     5112 2024-05-30 22:45:19.463729 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/qs/test/utils.js
+-rw-r--r--   0        0        0      917 2024-05-30 22:45:19.426020 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/range-parser/HISTORY.md
+-rw-r--r--   0        0        0     1178 2024-05-30 22:45:19.436196 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/range-parser/LICENSE
+-rw-r--r--   0        0        0     2278 2024-05-30 22:45:19.439464 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/range-parser/README.md
+-rw-r--r--   0        0        0     2900 2024-05-30 22:45:19.432265 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/range-parser/index.js
+-rw-r--r--   0        0        0     1184 2024-05-30 22:45:19.419446 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/range-parser/package.json
+-rw-r--r--   0        0        0     6048 2024-05-30 22:45:19.438798 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/raw-body/HISTORY.md
+-rw-r--r--   0        0        0     1181 2024-05-30 22:45:19.419072 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/raw-body/LICENSE
+-rw-r--r--   0        0        0     6553 2024-05-30 22:45:19.444201 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/raw-body/README.md
+-rw-r--r--   0        0        0     1188 2024-05-30 22:45:19.446801 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/raw-body/SECURITY.md
+-rw-r--r--   0        0        0     2286 2024-05-30 22:45:19.448665 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/raw-body/index.d.ts
+-rw-r--r--   0        0        0     7171 2024-05-30 22:45:19.425688 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/raw-body/index.js
+-rw-r--r--   0        0        0     1325 2024-05-30 22:45:19.431806 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/raw-body/package.json
+-rw-r--r--   0        0        0     1089 2024-05-30 22:45:19.416692 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/resolve-pkg-maps/LICENSE
+-rw-r--r--   0        0        0     7773 2024-05-30 22:45:19.440255 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/resolve-pkg-maps/README.md
+-rwxr-xr-x   0        0        0     2150 2024-05-30 22:45:19.428068 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/resolve-pkg-maps/dist/index.cjs
+-rw-r--r--   0        0        0      497 2024-05-30 22:45:19.434424 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/resolve-pkg-maps/dist/index.d.cts
+-rw-r--r--   0        0        0      497 2024-05-30 22:45:19.445419 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/resolve-pkg-maps/dist/index.d.mts
+-rwxr-xr-x   0        0        0     2080 2024-05-30 22:45:19.442124 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/resolve-pkg-maps/dist/index.mjs
+-rw-r--r--   0        0        0      951 2024-05-30 22:45:19.437572 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/resolve-pkg-maps/package.json
+-rw-r--r--   0        0        0     1081 2024-05-30 22:45:19.419410 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/safe-buffer/LICENSE
+-rw-r--r--   0        0        0    19555 2024-05-30 22:45:19.439097 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/safe-buffer/README.md
+-rw-r--r--   0        0        0     8738 2024-05-30 22:45:19.447037 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/safe-buffer/index.d.ts
+-rw-r--r--   0        0        0     1670 2024-05-30 22:45:19.426047 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/safe-buffer/index.js
+-rw-r--r--   0        0        0     1057 2024-05-30 22:45:19.432112 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/safe-buffer/package.json
+-rw-r--r--   0        0        0     1094 2024-05-30 22:45:19.431350 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/safer-buffer/LICENSE
+-rw-r--r--   0        0        0    12794 2024-05-30 22:45:19.438216 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/safer-buffer/Porting-Buffer.md
+-rw-r--r--   0        0        0     8261 2024-05-30 22:45:19.443869 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/safer-buffer/Readme.md
+-rw-r--r--   0        0        0     1483 2024-05-30 22:45:19.425154 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/safer-buffer/dangerous.js
+-rw-r--r--   0        0        0      822 2024-05-30 22:45:19.418314 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/safer-buffer/package.json
+-rw-r--r--   0        0        0     2110 2024-05-30 22:45:19.446511 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/safer-buffer/safer.js
+-rw-r--r--   0        0        0    15735 2024-05-30 22:45:19.449894 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/safer-buffer/tests.js
+-rw-r--r--   0        0        0    13301 2024-05-30 22:45:19.444096 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/send/HISTORY.md
+-rw-r--r--   0        0        0     1128 2024-05-30 22:45:19.419150 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/send/LICENSE
+-rw-r--r--   0        0        0     9476 2024-05-30 22:45:19.449922 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/send/README.md
+-rw-r--r--   0        0        0     1170 2024-05-30 22:45:19.452880 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/send/SECURITY.md
+-rw-r--r--   0        0        0    23502 2024-05-30 22:45:19.431985 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/send/index.js
+-rw-r--r--   0        0        0     3024 2024-05-30 22:45:19.424399 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/send/node_modules/ms/index.js
+-rw-r--r--   0        0        0     1079 2024-05-30 22:45:19.434871 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/send/node_modules/ms/license.md
+-rw-r--r--   0        0        0      732 2024-05-30 22:45:19.430265 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/send/node_modules/ms/package.json
+-rw-r--r--   0        0        0     1886 2024-05-30 22:45:19.437978 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/send/node_modules/ms/readme.md
+-rw-r--r--   0        0        0     1571 2024-05-30 22:45:19.438773 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/send/package.json
+-rw-r--r--   0        0        0    10537 2024-05-30 22:45:19.439314 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/serve-static/HISTORY.md
+-rw-r--r--   0        0        0     1189 2024-05-30 22:45:19.419643 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/serve-static/LICENSE
+-rw-r--r--   0        0        0     7812 2024-05-30 22:45:19.444692 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/serve-static/README.md
+-rw-r--r--   0        0        0     4570 2024-05-30 22:45:19.426380 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/serve-static/index.js
+-rw-r--r--   0        0        0     1141 2024-05-30 22:45:19.432438 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/serve-static/package.json
+-rw-r--r--   0        0        0      404 2024-05-30 22:45:19.417360 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/set-function-length/.eslintrc
+-rw-r--r--   0        0        0      563 2024-05-30 22:45:19.455415 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/set-function-length/.github/FUNDING.yml
+-rw-r--r--   0        0        0      216 2024-05-30 22:45:19.423900 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/set-function-length/.nycrc
+-rw-r--r--   0        0        0     4876 2024-05-30 22:45:19.447960 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/set-function-length/CHANGELOG.md
+-rw-r--r--   0        0        0     1083 2024-05-30 22:45:19.429798 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/set-function-length/LICENSE
+-rw-r--r--   0        0        0     2167 2024-05-30 22:45:19.450423 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/set-function-length/README.md
+-rw-r--r--   0        0        0      222 2024-05-30 22:45:19.451947 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/set-function-length/env.d.ts
+-rw-r--r--   0        0        0      867 2024-05-30 22:45:19.434567 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/set-function-length/env.js
+-rw-r--r--   0        0        0      256 2024-05-30 22:45:19.453471 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/set-function-length/index.d.ts
+-rw-r--r--   0        0        0     1273 2024-05-30 22:45:19.437838 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/set-function-length/index.js
+-rw-r--r--   0        0        0     2704 2024-05-30 22:45:19.440366 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/set-function-length/package.json
+-rw-r--r--   0        0        0      116 2024-05-30 22:45:19.443095 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/set-function-length/tsconfig.json
+-rw-r--r--   0        0        0      727 2024-05-30 22:45:19.436324 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/setprototypeof/LICENSE
+-rw-r--r--   0        0        0      844 2024-05-30 22:45:19.439056 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/setprototypeof/README.md
+-rw-r--r--   0        0        0       93 2024-05-30 22:45:19.426305 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/setprototypeof/index.d.ts
+-rw-r--r--   0        0        0      407 2024-05-30 22:45:19.432321 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/setprototypeof/index.js
+-rw-r--r--   0        0        0     1264 2024-05-30 22:45:19.419574 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/setprototypeof/package.json
+-rw-r--r--   0        0        0      690 2024-05-30 22:45:19.444521 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/setprototypeof/test/index.js
+-rw-r--r--   0        0        0      145 2024-05-30 22:45:19.418170 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/side-channel/.editorconfig
+-rw-r--r--   0        0        0      185 2024-05-30 22:45:19.425258 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/side-channel/.eslintrc
+-rw-r--r--   0        0        0      583 2024-05-30 22:45:19.457306 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/side-channel/.github/FUNDING.yml
+-rw-r--r--   0        0        0      216 2024-05-30 22:45:19.431223 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/side-channel/.nycrc
+-rw-r--r--   0        0        0     8802 2024-05-30 22:45:19.452365 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/side-channel/CHANGELOG.md
+-rw-r--r--   0        0        0     1071 2024-05-30 22:45:19.435222 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/side-channel/LICENSE
+-rw-r--r--   0        0        0       98 2024-05-30 22:45:19.453975 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/side-channel/README.md
+-rw-r--r--   0        0        0      765 2024-05-30 22:45:19.454934 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/side-channel/index.d.ts
+-rw-r--r--   0        0        0     3946 2024-05-30 22:45:19.438203 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/side-channel/index.js
+-rw-r--r--   0        0        0     2275 2024-05-30 22:45:19.446458 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/side-channel/package.json
+-rw-r--r--   0        0        0     1959 2024-05-30 22:45:19.443784 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/side-channel/test/index.js
+-rw-r--r--   0        0        0     3195 2024-05-30 22:45:19.449674 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/side-channel/tsconfig.json
+-rw-r--r--   0        0        0     1546 2024-05-30 22:45:19.439030 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/statuses/HISTORY.md
+-rw-r--r--   0        0        0     1172 2024-05-30 22:45:19.419293 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/statuses/LICENSE
+-rw-r--r--   0        0        0     3559 2024-05-30 22:45:19.444235 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/statuses/README.md
+-rw-r--r--   0        0        0     1789 2024-05-30 22:45:19.431911 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/statuses/codes.json
+-rw-r--r--   0        0        0     2610 2024-05-30 22:45:19.425813 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/statuses/index.js
+-rw-r--r--   0        0        0     1440 2024-05-30 22:45:19.436064 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/statuses/package.json
+-rw-r--r--   0        0        0      128 2024-05-30 22:45:19.435568 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/toidentifier/HISTORY.md
+-rw-r--r--   0        0        0     1108 2024-05-30 22:45:19.418561 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/toidentifier/LICENSE
+-rw-r--r--   0        0        0     1803 2024-05-30 22:45:19.438362 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/toidentifier/README.md
+-rw-r--r--   0        0        0      504 2024-05-30 22:45:19.425291 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/toidentifier/index.js
+-rw-r--r--   0        0        0     1142 2024-05-30 22:45:19.431317 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/toidentifier/package.json
+-rw-r--r--   0        0        0     1088 2024-05-30 22:45:19.420939 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/LICENSE
+-rw-r--r--   0        0        0     1657 2024-05-30 22:45:19.468966 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/README.md
+-rwxr-xr-x   0        0        0     1138 2024-05-30 22:45:19.461366 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/cjs/api/index.cjs
+-rw-r--r--   0        0        0      475 2024-05-30 22:45:19.468502 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/cjs/api/index.d.cts
+-rw-r--r--   0        0        0      475 2024-05-30 22:45:19.471872 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/cjs/api/index.d.mts
+-rwxr-xr-x   0        0        0     1034 2024-05-30 22:45:19.470556 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/cjs/api/index.mjs
+-rwxr-xr-x   0        0        0      467 2024-05-30 22:45:19.462298 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/cjs/index.cjs
+-rwxr-xr-x   0        0        0      401 2024-05-30 22:45:19.470595 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/cjs/index.mjs
+-rwxr-xr-x   0        0        0   116894 2024-05-30 22:45:19.450233 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/cli.cjs
+-rwxr-xr-x   0        0        0   116847 2024-05-30 22:45:19.469556 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/cli.mjs
+-rw-r--r--   0        0        0      387 2024-05-30 22:45:19.469849 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/client-Cg7nS93t.mjs
+-rw-r--r--   0        0        0      431 2024-05-30 22:45:19.453290 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/client-DjommMgI.cjs
+-rwxr-xr-x   0        0        0      474 2024-05-30 22:45:19.463832 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/esm/api/index.cjs
+-rw-r--r--   0        0        0     1185 2024-05-30 22:45:19.468668 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/esm/api/index.d.cts
+-rw-r--r--   0        0        0     1185 2024-05-30 22:45:19.471899 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/esm/api/index.d.mts
+-rwxr-xr-x   0        0        0      435 2024-05-30 22:45:19.470716 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/esm/api/index.mjs
+-rwxr-xr-x   0        0        0     4748 2024-05-30 22:45:19.465254 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/esm/index.cjs
+-rwxr-xr-x   0        0        0     4400 2024-05-30 22:45:19.470811 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/esm/index.mjs
+-rw-r--r--   0        0        0      206 2024-05-30 22:45:19.469903 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/get-pipe-path-CmcG6VNd.mjs
+-rw-r--r--   0        0        0      241 2024-05-30 22:45:19.454579 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/get-pipe-path-b8D5AZgV.cjs
+-rw-r--r--   0        0        0     2018 2024-05-30 22:45:19.455304 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/global-require-patch-B-BDRowI.cjs
+-rw-r--r--   0        0        0     1810 2024-05-30 22:45:19.470022 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/global-require-patch-CV_deDyT.mjs
+-rw-r--r--   0        0        0    62522 2024-05-30 22:45:19.459145 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/index-DTCJysGI.cjs
+-rw-r--r--   0        0        0    62467 2024-05-30 22:45:19.470432 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/index-DiuW-CAd.mjs
+-rwxr-xr-x   0        0        0     1110 2024-05-30 22:45:19.466004 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/loader.cjs
+-rwxr-xr-x   0        0        0     1056 2024-05-30 22:45:19.470937 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/loader.mjs
+-rw-r--r--   0        0        0      447 2024-05-30 22:45:19.466286 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/node-features-CKvB621_.cjs
+-rw-r--r--   0        0        0      354 2024-05-30 22:45:19.470986 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/node-features-Dcn4STxq.mjs
+-rw-r--r--   0        0        0       31 2024-05-30 22:45:19.471120 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/package-BHFW_wVM.mjs
+-rw-r--r--   0        0        0       47 2024-05-30 22:45:19.466620 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/package-BKSTPrAs.cjs
+-rw-r--r--   0        0        0      116 2024-05-30 22:45:19.467198 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/pkgroll_create-require-B-Pljx_-.cjs
+-rw-r--r--   0        0        0       80 2024-05-30 22:45:19.471161 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/pkgroll_create-require-CddX1PP_.mjs
+-rwxr-xr-x   0        0        0      884 2024-05-30 22:45:19.467505 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/preflight.cjs
+-rwxr-xr-x   0        0        0      846 2024-05-30 22:45:19.471221 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/preflight.mjs
+-rw-r--r--   0        0        0     1198 2024-05-30 22:45:19.471296 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/register-B0bfVVOZ.mjs
+-rw-r--r--   0        0        0     1372 2024-05-30 22:45:19.467537 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/register-BIOvi1NN.cjs
+-rwxr-xr-x   0        0        0      666 2024-05-30 22:45:19.467811 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/repl.cjs
+-rwxr-xr-x   0        0        0      626 2024-05-30 22:45:19.471371 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/repl.mjs
+-rw-r--r--   0        0        0     1123 2024-05-30 22:45:19.471468 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/resolve-ts-path-DUkQ8uuR.mjs
+-rw-r--r--   0        0        0     1413 2024-05-30 22:45:19.468016 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/resolve-ts-path-VlOGJlUT.cjs
+-rwxr-xr-x   0        0        0      497 2024-05-30 22:45:19.468102 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/suppress-warnings.cjs
+-rwxr-xr-x   0        0        0      484 2024-05-30 22:45:19.471754 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/suppress-warnings.mjs
+-rw-r--r--   0        0        0      166 2024-05-30 22:45:19.468361 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/temporary-directory-B83uKxJF.cjs
+-rw-r--r--   0        0        0      151 2024-05-30 22:45:19.471809 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/dist/temporary-directory-CwHp0_NW.mjs
+-rw-r--r--   0        0        0     1396 2024-05-30 22:45:19.468808 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/tsx/package.json
+-rw-r--r--   0        0        0     5447 2024-05-30 22:45:19.425790 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/type-is/HISTORY.md
+-rw-r--r--   0        0        0     1172 2024-05-30 22:45:19.435994 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/type-is/LICENSE
+-rw-r--r--   0        0        0     5183 2024-05-30 22:45:19.438725 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/type-is/README.md
+-rw-r--r--   0        0        0     5562 2024-05-30 22:45:19.431959 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/type-is/index.js
+-rw-r--r--   0        0        0     1133 2024-05-30 22:45:19.419543 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/type-is/package.json
+-rw-r--r--   0        0        0      455 2024-05-30 22:45:19.427723 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/README.md
+-rw-r--r--   0        0        0     1065 2024-05-30 22:45:19.433894 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/agent.d.ts
+-rw-r--r--   0        0        0     1455 2024-05-30 22:45:19.437253 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/api.d.ts
+-rw-r--r--   0        0        0      609 2024-05-30 22:45:19.440054 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/balanced-pool.d.ts
+-rw-r--r--   0        0        0     1251 2024-05-30 22:45:19.442227 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/cache.d.ts
+-rw-r--r--   0        0        0     4629 2024-05-30 22:45:19.445248 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/client.d.ts
+-rw-r--r--   0        0        0     1029 2024-05-30 22:45:19.447445 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/connector.d.ts
+-rw-r--r--   0        0        0      561 2024-05-30 22:45:19.448952 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/content-type.d.ts
+-rw-r--r--   0        0        0      635 2024-05-30 22:45:19.450163 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/cookies.d.ts
+-rw-r--r--   0        0        0     1634 2024-05-30 22:45:19.451496 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/diagnostics-channel.d.ts
+-rw-r--r--   0        0        0    13412 2024-05-30 22:45:19.454256 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/dispatcher.d.ts
+-rw-r--r--   0        0        0     3730 2024-05-30 22:45:19.456084 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/errors.d.ts
+-rw-r--r--   0        0        0     5458 2024-05-30 22:45:19.456759 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/fetch.d.ts
+-rw-r--r--   0        0        0     1707 2024-05-30 22:45:19.457529 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/file.d.ts
+-rw-r--r--   0        0        0     1453 2024-05-30 22:45:19.458526 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/filereader.d.ts
+-rw-r--r--   0        0        0     5012 2024-05-30 22:45:19.459311 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/formdata.d.ts
+-rw-r--r--   0        0        0      276 2024-05-30 22:45:19.459617 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/global-dispatcher.d.ts
+-rw-r--r--   0        0        0      175 2024-05-30 22:45:19.460254 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/global-origin.d.ts
+-rw-r--r--   0        0        0      387 2024-05-30 22:45:19.461107 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/handlers.d.ts
+-rw-r--r--   0        0        0      133 2024-05-30 22:45:19.461444 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/header.d.ts
+-rw-r--r--   0        0        0     2967 2024-05-30 22:45:19.462087 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/index.d.ts
+-rw-r--r--   0        0        0      215 2024-05-30 22:45:19.463071 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/interceptors.d.ts
+-rw-r--r--   0        0        0     2535 2024-05-30 22:45:19.463491 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/mock-agent.d.ts
+-rw-r--r--   0        0        0     1002 2024-05-30 22:45:19.463654 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/mock-client.d.ts
+-rw-r--r--   0        0        0      338 2024-05-30 22:45:19.464294 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/mock-errors.d.ts
+-rw-r--r--   0        0        0     3892 2024-05-30 22:45:19.464469 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/mock-interceptor.d.ts
+-rw-r--r--   0        0        0      974 2024-05-30 22:45:19.464913 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/mock-pool.d.ts
+-rw-r--r--   0        0        0     1193 2024-05-30 22:45:19.420902 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/package.json
+-rw-r--r--   0        0        0     1678 2024-05-30 22:45:19.465586 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/patch.d.ts
+-rw-r--r--   0        0        0      669 2024-05-30 22:45:19.466081 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/pool-stats.d.ts
+-rw-r--r--   0        0        0     1008 2024-05-30 22:45:19.466510 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/pool.d.ts
+-rw-r--r--   0        0        0      836 2024-05-30 22:45:19.466947 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/proxy-agent.d.ts
+-rw-r--r--   0        0        0     1622 2024-05-30 22:45:19.467325 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/readable.d.ts
+-rw-r--r--   0        0        0     5630 2024-05-30 22:45:19.467695 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/webidl.d.ts
+-rw-r--r--   0        0        0     3428 2024-05-30 22:45:19.467903 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/undici-types/websocket.d.ts
+-rw-r--r--   0        0        0       59 2024-05-30 22:45:19.438981 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/unpipe/HISTORY.md
+-rw-r--r--   0        0        0     1114 2024-05-30 22:45:19.431515 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/unpipe/LICENSE
+-rw-r--r--   0        0        0     1250 2024-05-30 22:45:19.425448 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/unpipe/README.md
+-rw-r--r--   0        0        0     1118 2024-05-30 22:45:19.435590 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/unpipe/index.js
+-rw-r--r--   0        0        0      770 2024-05-30 22:45:19.418601 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/unpipe/package.json
+-rw-r--r--   0        0        0       79 2024-05-30 22:45:19.425615 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/utils-merge/.npmignore
+-rw-r--r--   0        0        0     1084 2024-05-30 22:45:19.435934 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/utils-merge/LICENSE
+-rw-r--r--   0        0        0     1319 2024-05-30 22:45:19.431852 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/utils-merge/README.md
+-rw-r--r--   0        0        0      381 2024-05-30 22:45:19.438866 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/utils-merge/index.js
+-rw-r--r--   0        0        0      857 2024-05-30 22:45:19.419033 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/utils-merge/package.json
+-rw-r--r--   0        0        0      792 2024-05-30 22:45:19.439855 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/vary/HISTORY.md
+-rw-r--r--   0        0        0     1094 2024-05-30 22:45:19.433659 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/vary/LICENSE
+-rw-r--r--   0        0        0     2716 2024-05-30 22:45:19.427372 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/vary/README.md
+-rw-r--r--   0        0        0     2930 2024-05-30 22:45:19.437042 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/vary/index.js
+-rw-r--r--   0        0        0     1215 2024-05-30 22:45:19.420782 pinnacle_cli-0.0.2a2/pinnacle_cli/js/node_modules/vary/package.json
+-rw-r--r--   0        0        0    44865 2024-05-30 22:45:19.735966 pinnacle_cli-0.0.2a2/pinnacle_cli/js/package-lock.json
+-rw-r--r--   0        0        0      379 2024-05-31 00:05:09.721700 pinnacle_cli-0.0.2a2/pinnacle_cli/js/package.json
+-rw-r--r--   0        0        0       92 2024-05-31 00:04:59.191831 pinnacle_cli-0.0.2a2/pinnacle_cli/js/tsconfig.json
+-rw-r--r--   0        0        0      931 2024-05-31 00:25:34.277682 pinnacle_cli-0.0.2a2/pinnacle_cli/main.py
+-rw-r--r--   0        0        0        0 2024-05-30 20:22:31.038770 pinnacle_cli-0.0.2a2/pinnacle_cli/py/__init__.py
+-rw-r--r--   0        0        0     1475 2024-05-31 00:29:01.806456 pinnacle_cli-0.0.2a2/pinnacle_cli/py/dev.py
+-rw-r--r--   0        0        0      480 2024-05-31 00:39:31.711133 pinnacle_cli-0.0.2a2/pyproject.toml
+-rw-r--r--   0        0        0     2981 1970-01-01 00:00:00.000000 pinnacle_cli-0.0.2a2/PKG-INFO
```

### Comparing `pinnacle_cli-0.0.1/README.md` & `pinnacle_cli-0.0.2a2/README.md`

 * *Files identical despite different names*

### Comparing `pinnacle_cli-0.0.1/pinnacle_cli/dev.py` & `pinnacle_cli-0.0.2a2/pinnacle_cli/py/dev.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 import importlib
 from fastapi import FastAPI, Request
 from fastapi.responses import JSONResponse
 from fastapi.middleware.cors import CORSMiddleware
 from pinnacle_python.endpoints import endpoints
-from pinnacle_cli.constants import HOST, PORT, DIRECTORY
+from pinnacle_cli.constants import HOST, PYTHON_PORT, DIRECTORY
 
 app = FastAPI()
 
 sys.path.append(os.getcwd())
 
 for filename in os.listdir(DIRECTORY):
     if filename.endswith(".py"):
@@ -26,15 +26,16 @@
     allow_origins=origins,
     allow_credentials=True,
     allow_methods=["*"],
     allow_headers=["*"],
 )
 available_routes = []
 
-for endpoint in endpoints:
+
+def route_factory(endpoint):
     route_name = endpoint.__name__
     params = endpoint.__annotations__.items()
 
     @app.api_route(f"/{route_name}", methods=["POST"])
     async def route_handler(request: Request):
         params = await request.json()
 
@@ -42,17 +43,14 @@
 
         for param, _ in params.items():
             if param != "return":
                 params_dict[param] = params[param]
 
         return JSONResponse(content={"data": endpoint(**params_dict)})
 
-    available_routes.append((route_name, params))
+    return (route_name, params)
+
+
+for endpoint in endpoints:
+    route_name, params = route_factory(endpoint)
 
-print("Available routes:")
-for route, params in available_routes:
-    print(f"{HOST}:{PORT}/{route}")
-    for param, param_type in params:
-        if param == "return":
-            print(f"Return Type: {param_type.__name__}")
-        else:
-            print(f"Parameter: {param}, Type: {param_type.__name__}")
+    print(f"http://{HOST}:{PYTHON_PORT}/{route_name}")
```

### Comparing `pinnacle_cli-0.0.1/PKG-INFO` & `pinnacle_cli-0.0.2a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinnacle-cli
-Version: 0.0.1
+Version: 0.0.2a2
 Summary: 
 Author: Ivan Zhang
 Author-email: ivanzhangofficial@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
```

